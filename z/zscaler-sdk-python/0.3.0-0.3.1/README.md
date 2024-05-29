# Comparing `tmp/zscaler_sdk_python-0.3.0.tar.gz` & `tmp/zscaler_sdk_python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.3.0.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.3.1.tar", max compression
```

## Comparing `zscaler_sdk_python-0.3.0.tar` & `zscaler_sdk_python-0.3.1.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0        0        0     1113 2024-05-25 00:09:19.060317 zscaler_sdk_python-0.3.0/LICENSE.md
--rw-r--r--   0        0        0    15746 2024-05-25 00:09:19.060317 zscaler_sdk_python-0.3.0/README.md
--rw-r--r--   0        0        0     2325 2024-05-25 00:09:57.476060 zscaler_sdk_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1277 2024-05-25 00:09:57.480060 zscaler_sdk_python-0.3.0/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      853 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24891 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    15006 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     8054 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3844 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20849 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    33962 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0    27713 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/isolation.py
--rw-r--r--   0        0        0    21546 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    31713 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/policies.py
--rw-r--r--   0        0        0    70610 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/policiesv2.py
--rw-r--r--   0        0        0     5640 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    31880 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     3691 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7775 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     3684 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17529 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-29 17:30:06.573418 zscaler_sdk_python-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0    15746 2024-05-29 17:30:06.573418 zscaler_sdk_python-0.3.1/README.md
+-rw-r--r--   0        0        0     2351 2024-05-29 17:30:44.149212 zscaler_sdk_python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1277 2024-05-29 17:30:44.153212 zscaler_sdk_python-0.3.1/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4975 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      853 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-05-29 17:30:06.605417 zscaler_sdk_python-0.3.1/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    25271 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    15018 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     8054 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3844 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-05-29 17:30:06.609417 zscaler_sdk_python-0.3.1/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    33962 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0    27713 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/isolation.py
+-rw-r--r--   0        0        0    21546 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0   118552 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     5640 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    31880 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     3691 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7775 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     3684 2024-05-29 17:30:06.613417 zscaler_sdk_python-0.3.1/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17570 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.3.1/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.3.0/LICENSE.md` & `zscaler_sdk_python-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/README.md` & `zscaler_sdk_python-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/pyproject.toml` & `zscaler_sdk_python-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.3.0"
+version = "0.3.1"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
@@ -44,19 +44,20 @@
 xmltodict = "*"
 yarl = "*"
 pycryptodomex = "*"
 aenum = "*"
 pydash = "*"
 flake8 = "*"
 pytz = "*"
-black = "*"
+black = ">=24.3.0"
 cryptography = ">=3.4,<43.0"
+okta = ">=2.9.7"
 
 [tool.poetry.dev-dependencies]
-black = "24.3.0"
+black = ">=24.3.0"
 pytest = "^8.2.1"
 pytest-asyncio = ">=0.23.7"
 pytest-mock = "*"
 pytest-recording = "*"
 pytest-cov = "*"
 pyfakefs = "*"
 isort = "*"
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/__init__.py` & `zscaler_sdk_python-0.3.1/zscaler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/cache/cache.py` & `zscaler_sdk_python-0.3.1/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.3.1/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.3.1/zscaler/cache/zscaler_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,16 @@
                 del self._store[other_key]
                 logger.info(f'Removed also value from cache for key "{other_key}".')
 
     def clear(self):
         """
         Clear the cache.
         """
+        logger.info("Clearing the entire cache.")
         self._store.clear()
-        logger.info("Cleared the cache.")
 
     def _clean_cache(self):
         """
         Updates cache by removing expired entries at time of call
         """
         expired = []
         # Check every entry
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/constants.py` & `zscaler_sdk_python-0.3.1/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.3.1/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.3.1/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.3.1/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/logger.py` & `zscaler_sdk_python-0.3.1/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.3.1/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/user_agent.py` & `zscaler_sdk_python-0.3.1/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/utils.py` & `zscaler_sdk_python-0.3.1/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/activate.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/client.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/errors.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/labels.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/locations.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/security.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/users.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.3.1/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/README.md` & `zscaler_sdk_python-0.3.1/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from zscaler.zpa.emergency_access import EmergencyAccessAPI
 from zscaler.zpa.idp import IDPControllerAPI
 from zscaler.zpa.inspection import InspectionControllerAPI
 from zscaler.zpa.isolation import IsolationAPI
 from zscaler.zpa.lss import LSSConfigControllerAPI
 from zscaler.zpa.machine_groups import MachineGroupsAPI
 from zscaler.zpa.policies import PolicySetsAPI
-from zscaler.zpa.policiesv2 import PolicySetsV2API
 from zscaler.zpa.posture_profiles import PostureProfilesAPI
 from zscaler.zpa.privileged_remote_access import PrivilegedRemoteAccessAPI
 from zscaler.zpa.provisioning import ProvisioningKeyAPI
 from zscaler.zpa.saml_attributes import SAMLAttributesAPI
 from zscaler.zpa.scim_attributes import ScimAttributeHeaderAPI
 from zscaler.zpa.scim_groups import SCIMGroupsAPI
 from zscaler.zpa.segment_groups import SegmentGroupsAPI
@@ -114,14 +113,15 @@
         self.cloud = cloud
         self.url = f"{self.baseurl}/mgmtconfig/v1/admin/customers/{customer_id}"
         self.user_config_url = f"{self.baseurl}/userconfig/v1/customers/{customer_id}"
         self.v2_url = f"{self.baseurl}/mgmtconfig/v2/admin/customers/{customer_id}"
         self.v2_lss_url = f"{self.baseurl}/mgmtconfig/v2/admin/lssConfig/customers/{customer_id}"
         self.cbi_url = f"{self.baseurl}/cbiconfig/cbi/api/customers/{customer_id}"
         self.fail_safe = fail_safe
+
         # Cache setup
         cache_enabled = os.environ.get("ZSCALER_CLIENT_CACHE_ENABLED", "true").lower() == "true"
         if cache is None:
             if cache_enabled:
                 ttl = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTL", 3600))
                 tti = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTI", 1800))
                 self.cache = ZscalerCache(ttl=ttl, tti=tti)
@@ -129,84 +129,71 @@
                 self.cache = NoOpCache()
         else:
             self.cache = cache
 
         # Initialize user-agent
         ua = UserAgent()
         self.user_agent = ua.get_user_agent_string()
+        self.access_token = None
+        self.headers = {}
         self.refreshToken()
 
     def refreshToken(self):
-        # login
-        response = self.login()
-        if response is None or response.status_code > 299 or not response.json():
-            logger.error("Failed to login using provided credentials, response: %s", response)
-            raise Exception("Failed to login using provided credentials.")
-        self.access_token = response.json().get("access_token")
-        self.headers = {
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-            "Authorization": f"Bearer {self.access_token}",
-            "User-Agent": self.user_agent,
-        }
+        if not self.access_token or is_token_expired(self.access_token):
+            response = self.login()
+            if response is None or response.status_code > 299 or not response.json():
+                logger.error("Failed to login using provided credentials, response: %s", response)
+                raise Exception("Failed to login using provided credentials.")
+            self.access_token = response.json().get("access_token")
+            self.headers = {
+                "Content-Type": "application/json",
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.access_token}",
+                "User-Agent": self.user_agent,
+            }
 
     @retry_with_backoff(retries=5)
     def login(self):
-        """Log in to the ZPA API and set the access token for subsequent requests."""
         params = {"client_id": self.client_id, "client_secret": self.client_secret}
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Accept": "application/json",
             "User-Agent": self.user_agent,
         }
         try:
             url = f"{self.baseurl}/signin"
             if self.cloud == "DEV":
                 url = DEV_AUTH_URL + "?grant_type=CLIENT_CREDENTIALS"
             data = urllib.parse.urlencode(params)
             resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
-            # Avoid logging all data from the response, focus on the status and a summary instead
             logger.info("Login attempt with status: %d", resp.status_code)
             return resp
         except Exception as e:
             logger.error("Login failed due to an exception: %s", str(e))
             return None
 
     def send(self, method, path, json=None, params=None, api_version: str = None):
-        """
-        Send a request to the ZPA API.
-
-        Parameters:
-        - method (str): The HTTP method.
-        - path (str): API endpoint path.
-        - json (dict, optional): Request payload. Defaults to None.
-        Returns:
-        - Response: Response object from the request.
-        """
         api = self.url
         if api_version is None:
             api = self.url
         elif api_version == "v2":
             api = self.v2_url
         elif api_version == "v2_lss":
             api = self.v2_lss_url
         elif api_version == "userconfig_v1":
             api = self.user_config_url
         elif api_version == "cbiconfig_v1":
             api = self.cbi_url
 
         url = f"{api}/{path.lstrip('/')}"
         start_time = time.time()
-        # Update headers to include the user agent
         headers_with_user_agent = self.headers.copy()
         headers_with_user_agent["User-Agent"] = self.user_agent
-        # Generate a unique UUID for this request
         request_uuid = uuid.uuid4()
         dump_request(logger, url, method, json, params, headers_with_user_agent, request_uuid)
-        # Check cache before sending request
         cache_key = self.cache.create_key(url, params)
         if method == "GET" and self.cache.contains(cache_key):
             resp = self.cache.get(cache_key)
             dump_response(
                 logger=logger,
                 url=url,
                 method=method,
@@ -215,20 +202,21 @@
                 request_uuid=request_uuid,
                 start_time=start_time,
                 from_cache=True,
             )
             return resp
 
         attempts = 0
-        while attempts < 5:  # Trying a maximum of 5 times
+        while attempts < 5:
             try:
-                # If the token is None or expired, fetch a new token
-                if is_token_expired(self.access_token):
-                    logger.warning("The provided or fetched token was already expired. Refreshing...")
-                    self.refreshToken()
+                self.refreshToken()
+                should_wait, delay = self.rate_limiter.wait(method)
+                if should_wait:
+                    logger.warning(f"Rate limit exceeded. Retrying in {delay} seconds.")
+                    time.sleep(delay)
                 resp = requests.request(
                     method,
                     url,
                     json=json,
                     headers=headers_with_user_agent,
                     timeout=self.timeout,
                 )
@@ -237,100 +225,136 @@
                     url=url,
                     params=params,
                     method=method,
                     resp=resp,
                     request_uuid=request_uuid,
                     start_time=start_time,
                 )
-                if resp.status_code == 429:  # HTTP Status code 429 indicates "Too Many Requests"
-                    sleep_time = int(
-                        resp.headers.get("Retry-After", 2)
-                    )  # Default to 60 seconds if 'Retry-After' header is missing
-                    logger.warning(f"Rate limit exceeded. Retrying in {sleep_time} seconds.")
-                    sleep(sleep_time)
+                if resp.status_code == 429:
+                    retry_after = resp.headers.get("Retry-After")
+                    if retry_after:
+                        try:
+                            sleep_time = int(retry_after)
+                        except ValueError:
+                            sleep_time = int(retry_after[:-1])
+                        logger.warning(f"Rate limit exceeded. Retrying in {sleep_time} seconds.")
+                        time.sleep(sleep_time)
+                    else:
+                        time.sleep(60)
                     attempts += 1
                     continue
                 else:
                     break
             except requests.RequestException as e:
-                if attempts == 4:  # If it's the last attempt, raise the exception
+                if attempts == 4:
                     logger.error(f"Failed to send {method} request to {url} after 5 attempts. Error: {str(e)}")
                     raise e
                 else:
                     logger.warning(f"Failed to send {method} request to {url}. Retrying... Error: {str(e)}")
                     attempts += 1
-                    sleep(5)  # Sleep for 5 seconds before retrying
+                    time.sleep(5)
 
-        # If Non-GET call, clear the
         if method != "GET":
-            self.cache.delete(cache_key)
+            logger.info(f"Clearing cache for non-GET request: {method} {url}")
+            self.cache.clear()
 
-        # Detailed logging for request and response
         try:
             response_data = resp.json()
-        except ValueError:  # Using ValueError for JSON decoding errors
+        except ValueError:
             response_data = resp.text
-        # check if call was succesful
         if 200 > resp.status_code or resp.status_code > 299:
-            # create errors
             try:
                 error = ZscalerAPIError(url, resp, response_data)
                 if self.fail_safe:
                     raise ZscalerAPIException(response_data)
             except ZscalerAPIException:
                 raise
             except Exception:
                 error = HTTPError(url, resp, response_data)
                 if self.fail_safe:
                     logger.error(response_data)
                     raise HTTPException(response_data)
             logger.error(error)
-        # Cache the response if it's a successful GET request
         if method == "GET" and resp.status_code == 200:
             self.cache.add(cache_key, resp)
         return resp
 
     def get(self, path, json=None, params=None, api_version: str = None):
         """
         Send a GET request to the ZPA API.
 
         Parameters:
-        - path (str): API endpoint path.
-        - data (dict, optional): Request payload. Defaults to None.
+        path (str): API endpoint path.
+        json (dict, optional): Request payload. Defaults to None.
+        params (dict, optional): Query parameters. Defaults to None.
+        api_version (str, optional): API version to use. Defaults to None.
+
         Returns:
-        - Response: Response object from the request.
+        dict: Formatted JSON response from the API.
         """
-
-        # Use rate limiter before making a request
         should_wait, delay = self.rate_limiter.wait("GET")
         if should_wait:
             time.sleep(delay)
-
-        # Now proceed with sending the request
         resp = self.send("GET", path, json, params, api_version=api_version)
         formatted_resp = format_json_response(resp, box_attrs=dict())
         return formatted_resp
 
     def put(self, path, json=None, params=None, api_version: str = None):
+        """
+        Send a PUT request to the ZPA API.
+
+        Parameters:
+        path (str): API endpoint path.
+        json (dict, optional): Request payload. Defaults to None.
+        params (dict, optional): Query parameters. Defaults to None.
+        api_version (str, optional): API version to use. Defaults to None.
+
+        Returns:
+        dict: Formatted JSON response from the API.
+        """
         should_wait, delay = self.rate_limiter.wait("PUT")
         if should_wait:
             time.sleep(delay)
         resp = self.send("PUT", path, json, params, api_version=api_version)
         formatted_resp = format_json_response(resp, box_attrs=dict())
         return formatted_resp
 
     def post(self, path, json=None, params=None, api_version: str = None):
+        """
+        Send a POST request to the ZPA API.
+
+        Parameters:
+        path (str): API endpoint path.
+        json (dict, optional): Request payload. Defaults to None.
+        params (dict, optional): Query parameters. Defaults to None.
+        api_version (str, optional): API version to use. Defaults to None.
+
+        Returns:
+        dict: Formatted JSON response from the API.
+        """
         should_wait, delay = self.rate_limiter.wait("POST")
         if should_wait:
             time.sleep(delay)
         resp = self.send("POST", path, json, params, api_version=api_version)
         formatted_resp = format_json_response(resp, box_attrs=dict())
         return formatted_resp
 
     def delete(self, path, json=None, params=None, api_version: str = None):
+        """
+        Send a DELETE request to the ZPA API.
+
+        Parameters:
+        path (str): API endpoint path.
+        json (dict, optional): Request payload. Defaults to None.
+        params (dict, optional): Query parameters. Defaults to None.
+        api_version (str, optional): API version to use. Defaults to None.
+
+        Returns:
+        Response: Response object from the DELETE request.
+        """
         should_wait, delay = self.rate_limiter.wait("DELETE")
         if should_wait:
             time.sleep(delay)
         return self.send("DELETE", path, json, params, api_version=api_version)
 
     def get_paginated_data(
         self,
@@ -572,22 +596,14 @@
         """
         The interface object for the :ref:`ZPA Policy Sets interface <zpa-policies>`.
 
         """
         return PolicySetsAPI(self)
 
     @property
-    def policiesv2(self):
-        """
-        The interface object for the :ref:`ZPA Policy Sets V2 interface <zpa-policiesv2>`.
-
-        """
-        return PolicySetsV2API(self)
-
-    @property
     def posture_profiles(self):
         """
         The interface object for the :ref:`ZPA Posture Profiles interface <zpa-posture_profiles>`.
 
         """
         return PostureProfilesAPI(self)
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         return None
 
     def get_segments_by_type(self, application_type: str, expand_all: bool = False, **kwargs) -> Box:
         """
         Retrieve all configured application segments of a specified type, optionally expanding all related data.
 
         Args:
-            application_type (str): Type of application segment to retrieve. Must be one of "BROWSER_ACCESS", "INSPECT", "SECURE_REMOTE_ACCESS".
+            application_type (str): Type of application segment to retrieve.
+            Must be one of "BROWSER_ACCESS", "INSPECT", "SECURE_REMOTE_ACCESS".
             expand_all (bool, optional): Whether to expand all related data. Defaults to False.
 
         Keyword Args:
             max_items (int, optional): The maximum number of items to request before stopping iteration.
             max_pages (int, optional): The maximum number of pages to request before stopping iteration.
             pagesize (int, optional): Specifies the page size. The default size is 20, but the maximum size is 500.
             page (int, optional): Specifies the page number to begin fetching from.
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/client.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/isolation.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/isolation.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/policiesv2.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/policies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+# -*- coding: utf-8 -*-
+
+# Copyright (c) 2023, Zscaler Inc.
+#
+# Permission to use, copy, modify, and/or distribute this software for any
+# purpose with or without fee is hereby granted, provided that the above
+# copyright notice and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
+# WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
+# MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
+# ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+# WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+# ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
+# OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+
+
 import functools
 
 from box import Box, BoxList
 from requests import Response
 
 from zscaler.utils import add_id_groups, convert_keys, snake_to_camel
 from zscaler.zpa.client import ZPAClient
 
 
-class PolicySetsV2API:
+class PolicySetsAPI:
     def __init__(self, client: ZPAClient):
         self.rest = client
 
     POLICY_MAP = {
         "access": "ACCESS_POLICY",
         "capabilities": "CAPABILITIES_POLICY",
         "client_forwarding": "CLIENT_FORWARDING_POLICY",
@@ -26,15 +43,121 @@
 
     reformat_params = [
         ("app_server_group_ids", "appServerGroups"),
         ("app_connector_group_ids", "appConnectorGroups"),
         ("service_edge_group_ids", "serviceEdgeGroups"),
     ]
 
-    def _create_conditions(self, conditions: list) -> list:
+    @staticmethod
+    def _create_conditions_v1(conditions: list) -> list:
+        """
+        Creates a dict template for feeding conditions into the ZPA Policies API when adding or updating a policy.
+
+        Args:
+            conditions (list): List of condition dicts or tuples.
+
+        Returns:
+            :obj:`dict`: The conditions template.
+
+        """
+        template = []
+        app_and_app_group_operands = []
+        object_types_to_operands = {
+            "CONSOLE": [],
+            "MACHINE_GRP": [],
+            "LOCATION": [],
+            "BRANCH_CONNECTOR_GROUP": [],
+            "EDGE_CONNECTOR_GROUP": [],
+            "CLIENT_TYPE": [],
+            "IDP": [],
+            "PLATFORM": [],
+            "POSTURE": [],
+            "TRUSTED_NETWORK": [],
+            "SAML": [],
+            "SCIM": [],
+            "SCIM_GROUP": [],
+            "COUNTRY_CODE": [],
+        }
+
+        for condition in conditions:
+            if isinstance(condition, tuple) and len(condition) == 3:
+                # Handle each object type according to its pattern
+                object_type = condition[0].upper()
+                lhs = condition[1]
+                rhs = condition[2]
+
+                if object_type in ["APP", "APP_GROUP"]:
+                    app_and_app_group_operands.append({"objectType": object_type, "lhs": "id", "rhs": rhs})
+                elif object_type in object_types_to_operands:
+                    if object_type == "CLIENT_TYPE":
+                        if rhs in {
+                            "zpn_client_type_exporter",
+                            "zpn_client_type_machine_tunnel",
+                            "zpn_client_type_ip_anchoring",
+                            "zpn_client_type_edge_connector",
+                            "zpn_client_type_zapp",
+                            "zpn_client_type_slogger",
+                        }:
+                            object_types_to_operands[object_type].append({"objectType": object_type, "lhs": "id", "rhs": rhs})
+                    elif object_type in [
+                        "PLATFORM",
+                        "POSTURE",
+                        "TRUSTED_NETWORK",
+                        "SAML",
+                        "SCIM",
+                        "SCIM_GROUP",
+                        "COUNTRY_CODE",
+                    ]:
+                        object_types_to_operands[object_type].append({"objectType": object_type, "lhs": lhs, "rhs": rhs})
+                    else:
+                        object_types_to_operands[object_type].append({"objectType": object_type, "lhs": "id", "rhs": rhs})
+            elif isinstance(condition, dict):
+                # Handle the dictionary logic based on the Go code schema
+                condition_template = {}
+
+                # Extracting keys from the condition dictionary
+                for key in ["id", "negated", "operator"]:
+                    if key in condition:
+                        condition_template[key] = condition[key]
+
+                # Handling the operands
+                operands = condition.get("operands", [])
+                condition_template["operands"] = []
+
+                for operand in operands:
+                    operand_template = {}
+
+                    # Extracting keys from the operand dictionary
+                    for operand_key in [
+                        "id",
+                        "idp_id",
+                        "name",
+                        "lhs",
+                        "rhs",
+                        "objectType",
+                    ]:
+                        if operand_key in operand:
+                            operand_template[operand_key] = operand[operand_key]
+
+                    condition_template["operands"].append(operand_template)
+
+                template.append(condition_template)
+
+        # Combine APP and APP_GROUP operands into one block
+        if app_and_app_group_operands:
+            template.append({"operator": "OR", "operands": app_and_app_group_operands})
+
+        # Combine other object types into their own blocks
+        for object_type, operands in object_types_to_operands.items():
+            if operands:
+                template.append({"operator": "OR", "operands": operands})
+
+        return template
+
+    def _create_conditions_v2(self, conditions: list) -> list:
         """
         Creates a dict template for feeding conditions into the ZPA Policies API when adding or updating a policy.
 
         Args:
             conditions (list): List of condition tuples where each tuple represents a specific policy condition.
 
         Returns:
@@ -90,15 +213,15 @@
 
         Args:
             policy_type (str): The type of policy to be returned. Accepted values are:
 
                  |  ``access`` - returns the Access Policy
                  |  ``capabilities`` - returns the Capabilities Policy
                  |  ``client_forwarding`` - returns the Client Forwarding Policy
-                 |  ``clientless`` - returns the Clientlesss Session Protection Policy
+                 |  ``clientless`` - returns the Clientless Session Protection Policy
                  |  ``credential`` - returns the Credential Policy
                  |  ``inspection`` - returns the Inspection Policy
                  |  ``isolation`` - returns the Isolation Policy
                  |  ``redirection`` - returns the Redirection Policy
                  |  ``siem`` - returns the SIEM Policy
                  |  ``timeout`` - returns the Timeout Policy
 
@@ -143,15 +266,15 @@
 
             rule_id (str): The unique identifier for the policy rule.
 
         Returns:
             :obj:`Box`: The resource record for the requested rule.
 
         Examples:
-            >>> policy_rule = zpa.policies.get_rule(policy_id='99999',
+            >>> policy_rule = zpa.policies.get_rule(policy_type='access',
             ...    rule_id='88888')
 
         """
         # Get the policy id for the supplied policy_type
         policy_id = self.get_policy(policy_type).id
 
         return self.rest.get(f"policySet/{policy_id}/rule/{rule_id}")
@@ -242,49 +365,53 @@
 
                 |  ``allow``
                 |  ``deny``
             **kwargs:
                 Optional keyword args.
 
         Keyword Args:
-            custom_msg (str):
-                A custom message.
-            description (str):
-                A description for the rule.
-            app_connector_group_ids (:obj:`list` of :obj:`str`):
-                A list of application connector IDs that will be attached to the access policy rule.
-            app_server_group_ids (:obj:`list` of :obj:`str`):
-                A list of application server group IDs that will be attached to the access policy rule.
-
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
                 `RHS value`. If you are adding multiple values for the same object type then you will need
                 a new entry for each value.
                 E.g.
 
                 .. code-block:: python
 
                     [('app', 'id', '99999'),
                     ('app', 'id', '88888'),
                     ('app_group', 'id', '77777),
                     ('client_type', 'zpn_client_type_exporter', 'zpn_client_type_zapp'),
                     ('trusted_network', 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx', True)]
-
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+            app_connector_group_ids (:obj:`list` of :obj:`str`):
+                A list of application connector IDs that will be attached to the access policy rule.
+            app_server_group_ids (:obj:`list` of :obj:`str`):
+                A list of application server group IDs that will be attached to the access policy rule.
         Returns:
             :obj:`Box`: The resource record of the newly created access policy rule.
 
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": action.upper(),
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
         }
 
+        # Create conditions if provided
+        conditions = kwargs.pop("conditions", [])
+        if conditions:
+            payload["conditions"] = self._create_conditions_v1(conditions)
+        else:
+            payload["conditions"] = []
+
         if app_connector_group_ids:
             payload["appConnectorGroups"] = [{"id": group_id} for group_id in app_connector_group_ids]
 
         if app_server_group_ids:
             payload["appServerGroups"] = [{"id": group_id} for group_id in app_server_group_ids]
 
         add_id_groups(self.reformat_params, kwargs, payload)
@@ -292,87 +419,105 @@
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("access").id
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload, api_version="v2")
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_access_rule(
         self,
-        policy_type: str,
         rule_id: str,
         app_connector_group_ids: list = None,
         app_server_group_ids: list = None,
         **kwargs,
     ) -> Box:
         """
         Update an existing policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
-            policy_type (str):
-                The policy type. Accepted values are:
-                 |  ``access``
             rule_id (str):
                 The unique identifier for the rule to be updated.
-
             **kwargs:
                 Optional keyword args.
 
         Keyword Args:
             action (str):
                 The action for the policy. Accepted values are:
+
                 |  ``allow``
                 |  ``deny``
             app_connector_group_ids (:obj:`list` of :obj:`str`):
                 A list of application connector IDs that will be attached to the access policy rule. Defaults to an empty list.
             app_server_group_ids (:obj:`list` of :obj:`str`):
                 A list of server group IDs that will be attached to the access policy rule. Defaults to an empty list.
         Returns:
-            :obj:`Box`: The updated policy-rule resource record.
+            :obj:`Box`: The  policy-rule resource record.
 
         Examples:
-            ...
+            Update the name and description of the Access Policy Rule:
+
+            >>> zpa.policies.update_access_rule(
+            ...    name='Update_Access_Policy_Rule_v1',
+            ...    description='Update_Access_Policy_Rule_v1',
+            ... )
         """
         # Handle default values for app_connector_group_ids and app_server_group_ids
         app_connector_group_ids = app_connector_group_ids or []
         app_server_group_ids = app_server_group_ids or []
 
-        # Get policy id for specified policy type
-        policy_id = self.get_policy(policy_type).id
+        # Pre-set the policy_type to "client_forwarding"
+        policy_type = "access"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
 
-        payload = convert_keys(self.get_rule(policy_type, rule_id))
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
 
         # Update kwargs with app_connector_group_ids and app_server_group_ids for processing with add_id_groups
         kwargs["app_connector_group_ids"] = app_connector_group_ids
         kwargs["app_server_group_ids"] = app_server_group_ids
 
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v1(value)
             else:
                 payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2").status_code
+        # If conditions are not provided, set conditions to an empty list to remove existing conditions
+        if "conditions" not in kwargs:
+            payload["conditions"] = []
 
-        # Return the object if it was updated successfully
-        if not isinstance(resp, Response):
-            return self.get_rule(policy_type, rule_id)
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        # Make the PUT request to update the rule
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v1")
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
     def add_timeout_rule(self, name: str, **kwargs) -> Box:
         """
         Add a new Timeout Policy rule.
 
         See the `ZPA Timeout Policy API reference <https://help.zscaler.com/zpa/timeout-policy-use-cases>`_
         for further detail on optional keyword parameter structures.
@@ -411,60 +556,959 @@
 
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": "RE_AUTH",
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v1(kwargs.pop("conditions", [])),
         }
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("timeout").id
 
         # Use specified timeouts or default to UI values
         payload["reauthTimeout"] = kwargs.get("re_auth_timeout", 172800)
         payload["reauthIdleTimeout"] = kwargs.get("re_auth_idle_timeout", 600)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload, api_version="v2")
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_timeout_rule(self, rule_id: str, **kwargs) -> Box:
         """
-        Update an existing policy rule.
+        Update an existing Timeout Policy Rule rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
-            policy_type (str):
-                The policy type. Accepted values are:
-
-                 |  ``timeout``
             rule_id (str):
                 The unique identifier for the rule to be updated.
             **kwargs:
                 Optional keyword args.
 
         Keyword Args:
             action (str):
+                The only supported action for this policy is RE_AUTH and it's pre-set during the payload submission.
+
+                |  ``RE_AUTH``
+
+            description (str):
+                Additional information about the Timeout Policy Rule rule.
+            enabled (bool):
+                Whether or not the Timeout Policy Rule rule. is enabled.
+            rule_order (str):
+                The rule evaluation order number of the rule.
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+            re_auth_idle_timeout (int):
+                The re-authentication idle timeout value in seconds.
+            re_auth_timeout (int):
+                The re-authentication timeout value in seconds.
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', 'app_segment_id'),
+                    ('app', 'id', 'app_segment_id'),
+                    ('app_group', 'id', 'segment_group_id),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ('client_type', 'zpn_client_type_exporter')]
+
+        Returns:
+            :obj:`Box`: The updated policy-rule resource record.
+
+        Examples:
+            Updates the name only for an Timeout Policy Rule rule:
+
+            >>> zpa.policies.update_timeout_rule(
+            ...    rule_id='216199618143320419',
+            ...    name='Update_Timeout_Rule_v1',
+            ...    description='Update_Timeout_Rule_v1',
+            ...    conditions=[
+            ...         ("app", ["216199618143361683"]),
+            ...         ("app_group", ["216199618143360301"]),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...     ],
+            ... )
+        """
+        # Pre-set the policy_type to "timeout"
+        policy_type = "timeout"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Pre-set the action to "RE_AUTH"
+        payload["action"] = "RE_AUTH"
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            if key == "conditions":
+                payload["conditions"] = self._create_conditions_v1(value)
+            else:
+                payload[snake_to_camel(key)] = value
+
+        # If conditions are not provided, set conditions to an empty list to remove existing conditions
+        if "conditions" not in kwargs:
+            payload["conditions"] = []
+
+        # Use specified timeouts or default to UI values
+        payload["reauthTimeout"] = kwargs.get("re_auth_timeout", 172800)
+        payload["reauthIdleTimeout"] = kwargs.get("re_auth_idle_timeout", 600)
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        # Make the PUT request to update the rule
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v1")
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_client_forwarding_rule(self, name: str, action: str, **kwargs) -> Box:
+        """
+        Add a new Client Forwarding Policy rule.
+
+        See the
+        `ZPA Client Forwarding Policy API reference <https://help.zscaler.com/zpa/client-forwarding-policy-use-cases>`_
+        for further detail on optional keyword parameter structures.
+
+        Args:
+            name (str):
+                The name of the new rule.
+            action (str):
                 The action for the policy. Accepted values are:
 
+                |  ``intercept``
+                |  ``intercept_accessible``
                 |  ``bypass``
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '926196382959075416'),
+                    ('app', 'id', '926196382959075417'),
+                    ('app_group', 'id', '926196382959075332),
+                    ('client_type', 'zpn_client_type_exporter', 'zpn_client_type_zapp'),
+                    ('trusted_network', 'b15e4cad-fa6e-8182-9fc3-8125ee6a65e1', True)]
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+
+        Returns:
+            :obj:`Box`: The resource record of the newly created Client Forwarding Policy rule.
+
+        Examples:
+            Add a new Client Forwarding Policy rule:
+
+            >>> zpa.policies.add_client_forwarding_rule(
+            ...    name='Add_Forwarding_Rule_v1',
+            ...    description='Update_Forwarding_Rule_v1',
+            ...    action='isolate',
+            ...    conditions=[
+            ...         ("app", ["216199618143361683"]),
+            ...         ("app_group", ["216199618143360301"]),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...     ],
+            ... )
+
+        """
+        # Initialise the payload
+        payload = {
+            "name": name,
+            "action": action.upper(),
+        }
+
+        # Create conditions if provided
+        conditions = kwargs.pop("conditions", [])
+        if conditions:
+            payload["conditions"] = self._create_conditions_v1(conditions)
+        else:
+            payload["conditions"] = []
+
+        # Get the policy id of the provided policy type for the URL.
+        policy_id = self.get_policy("client_forwarding").id
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[snake_to_camel(key)] = value
+
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload, api_version="v1")
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_client_forwarding_rule(self, rule_id: str, **kwargs) -> Box:
+        """
+        Update an existing Client Forwarding Policy rule.
+
+        Ensure you are using the correct arguments for the policy type that you want to update.
+
+        Args:
+            rule_id (str):
+                The unique identifier for the rule to be updated.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            action (str):
+                The action for the policy. Accepted values are:
+
                 |  ``intercept``
                 |  ``intercept_accessible``
+                |  ``bypass``
+            description (str):
+                Additional information about the Client Forwarding Policy rule.
+            enabled (bool):
+                Whether or not the Client Forwarding Policy rule. is enabled.
+            rule_order (str):
+                The rule evaluation order number of the rule.
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', 'app_segment_id'),
+                    ('app', 'id', 'app_segment_id'),
+                    ('app_group', 'id', 'segment_group_id),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ('client_type', 'zpn_client_type_exporter')]
+
+        Returns:
+            :obj:`Box`: The updated policy-rule resource record.
 
+        Examples:
+            Updates the name only for an Client Forwarding Policy rule:
+
+            >>> zpa.policies.update_client_forwarding_rule(
+            ...    rule_id='216199618143320419',
+            ...    name='Update_Forwarding_Rule_v1',
+            ...    description='Update_Forwarding_Rule_v1',
+            ...    action='isolate',
+            ...    conditions=[
+            ...         ("app", ["216199618143361683"]),
+            ...         ("app_group", ["216199618143360301"]),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...     ],
+            ... )
+        """
+        # Pre-set the policy_type to "client_forwarding"
+        policy_type = "client_forwarding"
+
+        # Ensure the action is provided and convert to uppercase
+        if "action" not in kwargs:
+            raise ValueError("The 'action' attribute is mandatory.")
+
+        action = kwargs.pop("action").upper()
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            if key == "conditions":
+                payload["conditions"] = self._create_conditions_v1(value)
+            else:
+                payload[snake_to_camel(key)] = value
+
+        # If conditions are not provided, set conditions to an empty list to remove existing conditions
+        if "conditions" not in kwargs:
+            payload["conditions"] = []
+
+        # Set the action in the payload
+        payload["action"] = action
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        # Make the PUT request to update the rule
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v1")
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_isolation_rule(self, name: str, action: str, zpn_isolation_profile_id: str, **kwargs) -> Box:
+        """
+        Add a new Isolation Policy rule.
+
+        See the
+        `ZPA Isolation Policy API reference <https://help.zscaler.com/zpa/configuring-isolation-policies-using-api>`_
+        for further detail on optional keyword parameter structures.
+
+        Args:
+            name (str):
+                The name of the new rule.
+            action (str):
+                The action for the policy. Accepted values are:
+
+                |  ``isolate``
+                |  ``bypass_isolate``
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '926196382959075416'),
+                    ('app', 'id', '926196382959075417'),
+                    ('app_group', 'id', '926196382959075332),
+                    ('client_type', 'zpn_client_type_exporter')]
+            zpn_isolation_profile_id (str):
+                The isolation profile ID associated with the rule
+            description (str):
+                A description for the rule.
+
+        Returns:
+            :obj:`Box`: The resource record of the newly created Client Isolation Policy rule.
+
+        """
+
+        # Initialise the payload
+        payload = {
+            "name": name,
+            "action": action.upper(),
+            "zpnIsolationProfileId": zpn_isolation_profile_id,
+        }
+
+        # Create conditions if provided
+        conditions = kwargs.pop("conditions", [])
+        if conditions:
+            payload["conditions"] = self._create_conditions_v1(conditions)
+        else:
+            payload["conditions"] = []
+
+        # Ensure CLIENT_TYPE is always included
+        client_type_present = any(
+            cond.get("operands", [{}])[0].get("objectType", "") == "CLIENT_TYPE" for cond in payload["conditions"]
+        )
+        if not client_type_present:
+            payload["conditions"].append(
+                {"operator": "OR", "operands": [{"objectType": "CLIENT_TYPE", "lhs": "id", "rhs": "zpn_client_type_exporter"}]}
+            )
+
+        # Get the policy id of the provided policy type for the URL.
+        policy_id = self.get_policy("isolation").id
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[snake_to_camel(key)] = value
+
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_isolation_rule(self, rule_id: str, **kwargs) -> Box:
+        """
+        Update an existing client isolation policy rule.
+
+        Ensure you are using the correct arguments for the policy type that you want to update.
+
+        Args:
+            rule_id (str):
+                The unique identifier for the rule to be updated.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            action (str):
+                The action for the policy. Accepted values are:
+
+                |  ``isolate``
+                |  ``bypass_isolate``
+            description (str):
+                Additional information about the client forwarding policy rule.
+            enabled (bool):
+                Whether or not the client forwarding policy rule is enabled.
+            rule_order (str):
+                The rule evaluation order number of the rule.
+            zpn_isolation_profile_id (str):
+                The unique identifier of the inspection profile. This field is applicable only for inspection policies.
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '926196382959075416'),
+                    ('app', 'id', '926196382959075417'),
+                    ('app_group', 'id', '926196382959075332),
+                    ('client_type', 'zpn_client_type_exporter')]
+
+        Returns:
+            :obj:`Box`: The updated policy-rule resource record.
+
+        Examples:
+            Updates the name only for an Isolation Policy rule:
+
+            >>> zpa.policiesv2.update_isolation_rule_v1(
+            ...    rule_id='216199618143320419',
+            ...    name='Update_Isolation_Rule_v2',
+            ...    description='Update_Isolation_Rule_v2',
+            ...    action='isolate',
+            ...    conditions=[
+            ...         ("app", ["216199618143361683"]),
+            ...         ("app_group", ["216199618143360301"]),
+            ...         ("scim_group", [("216199618143191058", "2079468"), ("216199618143191058", "2079446")]),
+            ...     ],
+            ... )
+        """
+
+        # Pre-set the policy_type to "isolation"
+        policy_type = "isolation"
+
+        # Ensure the action is provided and convert to uppercase
+        if "action" not in kwargs:
+            raise ValueError("The 'action' attribute is mandatory.")
+
+        action = kwargs.pop("action").upper()
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            if key == "conditions":
+                payload["conditions"] = self._create_conditions_v1(value)
+            else:
+                payload[snake_to_camel(key)] = value
+
+        # If conditions are not provided, set conditions to an empty list to remove existing conditions
+        if "conditions" not in kwargs:
+            payload["conditions"] = []
+
+        # Ensure CLIENT_TYPE is always included
+        client_type_present = any(
+            cond.get("operands", [{}])[0].get("objectType", "") == "CLIENT_TYPE" for cond in payload["conditions"]
+        )
+        if not client_type_present:
+            payload["conditions"].append(
+                {"operator": "OR", "operands": [{"objectType": "CLIENT_TYPE", "lhs": "id", "rhs": "zpn_client_type_exporter"}]}
+            )
+
+        # Set the action in the payload
+        payload["action"] = action
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        # Make the PUT request to update the rule
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v1")
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_app_protection_rule(self, name: str, action: str, zpn_inspection_profile_id: str, **kwargs) -> Box:
+        """
+        Add a new AppProtection Policy rule.
+
+        See the
+        `ZPA AppProtection Policy API reference <https://help.zscaler.com/zpa/configuring-appprotection-policies-using-api>`_
+        for further detail on optional keyword parameter structures.
+
+        Args:
+            name (str):
+                The name of the new rule.
+            action (str):
+                The action for the policy. Accepted values are:
+
+                |  ``inspect``
+                |  ``bypass_inspect``
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '926196382959075416'),
+                    ('app', 'id', '926196382959075417'),
+                    ('app_group', 'id', '926196382959075332),
+                    ('client_type', 'zpn_client_type_exporter')]
+            zpn_inspection_profile_id (str):
+                The AppProtection profile ID associated with the rule
+            description (str):
+                A description for the rule.
+
+        Returns:
+            :obj:`Box`: The resource record of the newly created Client Inspection Policy rule.
+
+        """
+
+        # Initialise the payload
+        payload = {
+            "name": name,
+            "action": action.upper(),
+            "zpnInspectionProfileId": zpn_inspection_profile_id,
+        }
+
+        # Create conditions if provided
+        conditions = kwargs.pop("conditions", [])
+        if conditions:
+            payload["conditions"] = self._create_conditions_v1(conditions)
+        else:
+            payload["conditions"] = []
+
+        # Get the policy id of the provided policy type for the URL.
+        policy_id = self.get_policy("inspection").id
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[snake_to_camel(key)] = value
+
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_app_protection_rule(self, rule_id: str, **kwargs) -> Box:
+        """
+        Update an existing App Protection Policy Rule rule.
+
+        Ensure you are using the correct arguments for the policy type that you want to update.
+
+        Args:
+            rule_id (str):
+                The unique identifier for the rule to be updated.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            action (str):
+                The action for the policy. Accepted values are:
+
+                |  ``inspect``
+                |  ``bypass_inspect``
+            description (str):
+                Additional information about the App Protection Policy Rule rule.
+            enabled (bool):
+                Whether or not the App Protection Policy Rule rule. is enabled.
+            rule_order (str):
+                The rule evaluation order number of the rule.
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', 'app_segment_id'),
+                    ('app', 'id', 'app_segment_id'),
+                    ('app_group', 'id', 'segment_group_id),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ("scim_group", "idp_id", "scim_group_id"),
+                    ('client_type', 'zpn_client_type_exporter')]
+
+        Returns:
+            :obj:`Box`: The updated policy-rule resource record.
+
+        Examples:
+            Updates the name only for an App Protection Policy Rule rule:
+
+            >>> zpa.policies.update_app_protection_rule(
+            ...    rule_id='216199618143320419',
+            ...    name='Update_App_Protection_Rule_v1',
+            ...    description='Update_App_Protection_Rule_v1',
+            ...    action='bypass_inspect',
+            ...    conditions=[
+            ...         ("app", ["216199618143361683"]),
+            ...         ("app_group", ["216199618143360301"]),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...         ("scim_group", "idp_id", "scim_group_id"),
+            ...     ],
+            ... )
+        """
+        # Pre-set the policy_type to "client_forwarding"
+        policy_type = "inspection"
+
+        # Ensure the action is provided and convert to uppercase
+        if "action" not in kwargs:
+            raise ValueError("The 'action' attribute is mandatory.")
+
+        action = kwargs.pop("action").upper()
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            if key == "conditions":
+                payload["conditions"] = self._create_conditions_v1(value)
+            else:
+                payload[snake_to_camel(key)] = value
+
+        # If conditions are not provided, set conditions to an empty list to remove existing conditions
+        if "conditions" not in kwargs:
+            payload["conditions"] = []
+
+        # Set the action in the payload
+        payload["action"] = action
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        # Make the PUT request to update the rule
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v1")
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_access_rule_v2(
+        self,
+        name: str,
+        action: str,
+        app_connector_group_ids: list = [],
+        app_server_group_ids: list = [],
+        **kwargs,
+    ) -> Box:
+        """
+        Add a new Access Policy rule.
+
+        See the `ZPA Access Policy API reference <https://help.zscaler.com/zpa/access-policy-use-cases>`_
+        for further detail on optional keyword parameter structures.
+
+        Args:
+            name (str):
+                The name of the new rule.
+            action (str):
+                The action for the policy. Accepted values are:
+
+                |  ``allow``
+                |  ``deny``
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+            app_connector_group_ids (:obj:`list` of :obj:`str`):
+                A list of application connector IDs that will be attached to the access policy rule.
+            app_server_group_ids (:obj:`list` of :obj:`str`):
+                A list of application server group IDs that will be attached to the access policy rule.
+
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '99999'),
+                    ('app', 'id', '88888'),
+                    ('app_group', 'id', '77777),
+                    ('client_type', 'zpn_client_type_exporter', 'zpn_client_type_zapp'),
+                    ('trusted_network', 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx', True)]
+
+        Returns:
+            :obj:`Box`: The resource record of the newly created access policy rule.
+
+        """
+
+        # Initialise the payload
+        payload = {
+            "name": name,
+            "action": action.upper(),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
+        }
+
+        if app_connector_group_ids:
+            payload["appConnectorGroups"] = [{"id": group_id} for group_id in app_connector_group_ids]
+
+        if app_server_group_ids:
+            payload["appServerGroups"] = [{"id": group_id} for group_id in app_server_group_ids]
+
+        add_id_groups(self.reformat_params, kwargs, payload)
+
+        # Get the policy id of the provided policy type for the URL.
+        policy_id = self.get_policy("access").id
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[snake_to_camel(key)] = value
+
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload, api_version="v2")
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_access_rule_v2(
+        self,
+        rule_id: str,
+        app_connector_group_ids: list = None,
+        app_server_group_ids: list = None,
+        **kwargs,
+    ) -> Box:
+        """
+        Update an existing policy rule.
+
+        Ensure you are using the correct arguments for the policy type that you want to update.
+
+        Args:
+            rule_id (str):
+                The unique identifier for the rule to be updated.
+            app_connector_group_ids (:obj:`list` of :obj:`str`, optional):
+                A list of application connector IDs that will be attached to the access policy rule. Defaults to an empty list.
+            app_server_group_ids (:obj:`list` of :obj:`str`, optional):
+                A list of server group IDs that will be attached to the access policy rule. Defaults to an empty list.
+
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            action (str):
+                The action for the policy. Accepted values are:
+                |  ``ALLOW``
+                |  ``DENY``
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+
+        Returns:
+            :obj:`Box`: The updated policy-rule resource record.
+
+        Examples:
+            Updates the description for an Access Policy rule:
+
+            >>> zpa.policiesv2.update_access_rule(
+            ...    rule_id='216199618143320419',
+            ...    description='Updated Description',
+            ...    action='ALLOW',
+            ...    conditions=[
+            ...         ("client_type", ['zpn_client_type_exporter', 'zpn_client_type_zapp']),
+            ...     ],
+            ... )
+        """
+        # Handle default values for app_connector_group_ids and app_server_group_ids
+        app_connector_group_ids = app_connector_group_ids or []
+        app_server_group_ids = app_server_group_ids or []
+
+        # Pre-set the policy_type to "access"
+        policy_type = "access"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
+
+        # Add or update optional parameters to the payload
+        for key, value in kwargs.items():
+            if key == "conditions":
+                payload["conditions"] = self._create_conditions_v2(value)
+            elif key == "action":
+                payload["action"] = value.upper()
+            else:
+                payload[snake_to_camel(key)] = value
+
+        # Add id groups to the payload
+        add_id_groups(self.reformat_params, kwargs, payload)
+
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
+
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_timeout_rule_v2(self, name: str, **kwargs) -> Box:
+        """
+        Add a new Timeout Policy rule.
+
+        See the `ZPA Timeout Policy API reference <https://help.zscaler.com/zpa/timeout-policy-use-cases>`_
+        for further detail on optional keyword parameter structures.
+
+        Args:
+            name (str):
+                The name of the new rule.
+            **kwargs:
+                Optional parameters.
+
+        Keyword Args:
+            conditions (list):
+                A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
+                `RHS value`. If you are adding multiple values for the same object type then you will need
+                a new entry for each value.
+                E.g.
+
+                .. code-block:: python
+
+                    [('app', 'id', '926196382959075416'),
+                    ('app', 'id', '926196382959075417'),
+                    ('app_group', 'id', '926196382959075332),
+                    ('client_type', 'zpn_client_type_exporter', 'zpn_client_type_zapp'),
+                    ('trusted_network', 'b15e4cad-fa6e-8182-9fc3-8125ee6a65e1', True)]
+            custom_msg (str):
+                A custom message.
+            description (str):
+                A description for the rule.
+            re_auth_idle_timeout (int):
+                The re-authentication idle timeout value in seconds.
+            re_auth_timeout (int):
+                The re-authentication timeout value in seconds.
+
+        Returns:
+            :obj:`Box`: The resource record of the newly created Timeout Policy rule.
+
+        """
+
+        # Initialise the payload
+        payload = {
+            "name": name,
+            "action": "RE_AUTH",
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
+        }
+
+        # Get the policy id of the provided policy type for the URL.
+        policy_id = self.get_policy("timeout").id
+
+        # Use specified timeouts or default to UI values
+        payload["reauthTimeout"] = kwargs.get("re_auth_timeout", 172800)
+        payload["reauthIdleTimeout"] = kwargs.get("re_auth_idle_timeout", 600)
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[snake_to_camel(key)] = value
+
+        response = self.rest.post(f"policySet/{policy_id}/rule", json=payload, api_version="v2")
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_timeout_rule_v2(self, rule_id: str, **kwargs) -> Box:
+        """
+        Update an existing policy rule.
+
+        Ensure you are using the correct arguments for the policy type that you want to update.
+
+        Args:
+            rule_id (str):
+                The unique identifier for the rule to be updated.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
                 `RHS value`. If you are adding multiple values for the same object type then you will need
                 a new entry for each value.
                 E.g.
 
                 .. code-block:: python
@@ -483,42 +1527,67 @@
             re_auth_timeout (int):
                 The re-authentication timeout value in seconds.
 
         Returns:
             :obj:`Box`: The updated policy-rule resource record.
 
         Examples:
-            Updates the name only for an Timeout Policy rule:
-
-            >>> zpa.policies.update_rule('timeout', '99999', name='new_rule_name')
+            Updates the name only for a Timeout Policy rule:
 
-            Updates the action only for a Timeout Policy rule:
+            >>> zpa.policies.update_timeout_rule('99999', name='new_rule_name')
 
-            >>> zpa.policies.update_rule('timeout', '888888', action='BYPASS')
+            Updates the description for a Timeout Policy rule:
 
+            >>> zpa.policies.update_timeout_rule('888888', description='Updated Description')
         """
-        # Get policy id for specified policy type
-        policy_id = self.get_policy("timeout").id
 
-        payload = convert_keys(self.get_rule(policy_id, rule_id))
+        # Pre-set the policy_type to "timeout"
+        policy_type = "timeout"
 
-        # Add optional parameters to payload
+        # Pre-set the action to "RE_AUTH"
+        kwargs["action"] = "RE_AUTH"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
+
+        # Add or update optional parameters to the payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
+            elif key == "action":
+                payload["action"] = value.upper()
             else:
                 payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2").status_code
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
 
-        # Return the object if it was updated successfully
-        if not isinstance(resp, Response):
-            return self.get_rule(policy_id, rule_id)
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
 
-    def add_client_forwarding_rule(self, name: str, action: str, **kwargs) -> Box:
+        response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
+
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
+
+    def add_client_forwarding_rule_v2(self, name: str, action: str, **kwargs) -> Box:
         """
         Add a new Client Forwarding Policy rule.
 
         See the
         `ZPA Client Forwarding Policy API reference <https://help.zscaler.com/zpa/client-forwarding-policy-use-cases>`_
         for further detail on optional keyword parameter structures.
 
@@ -558,15 +1627,15 @@
 
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": action.upper(),
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("client_forwarding").id
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
@@ -576,15 +1645,15 @@
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_client_forwarding_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_client_forwarding_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing client forwarding policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
 
@@ -611,61 +1680,84 @@
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
                 `RHS value`. If you are adding multiple values for the same object type then you will need
                 a new entry for each value.
                 E.g.
 
                 .. code-block:: python
 
-                    ("client_type", ['zpn_client_type_edge_connector', 'zpn_client_type_branch_connector', 'zpn_client_type_machine_tunnel', 'zpn_client_type_zapp', 'zpn_client_type_zapp_partner']),
+                    ("client_type",
+                        ['zpn_client_type_edge_connector',
+                        'zpn_client_type_branch_connector',
+                        'zpn_client_type_machine_tunnel',
+                        'zpn_client_type_zapp', 'zpn_client_type_zapp_partner'
+                    ]),
 
         Returns:
             :obj:`Box`: The updated policy-rule resource record.
 
         Examples:
             Updates the name only for an Access Policy rule:
 
             >>> zpa.policiesv2.update_client_forwarding_rule(
             ...    rule_id='216199618143320419',
             ...    name='Update_Redirection_Rule_v2',
             ...    description='Update_Redirection_Rule_v2',
             ...    action='redirect_default',
             ...    conditions=[
-            ...         ("client_type", ['zpn_client_type_edge_connector', 'zpn_client_type_branch_connector', 'zpn_client_type_machine_tunnel', 'zpn_client_type_zapp', 'zpn_client_type_zapp_partner']),
+            ...         ("client_type",
+            ...         ['zpn_client_type_edge_connector',
+            ...          'zpn_client_type_branch_connector',
+            ...          'zpn_client_type_machine_tunnel',
+            ...          'zpn_client_type_zapp',
+            ...          'zpn_client_type_zapp_partner']),
             ...     ],
-            ...         )
+            ... )
         """
 
-        # Ensure the action is provided and convert to uppercase
-        if "action" not in kwargs:
-            raise ValueError("The 'action' attribute is mandatory.")
+        # Pre-set the policy_type to "timeout"
+        policy_type = "client_forwarding"
 
-        action = kwargs.pop("action").upper()
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
 
-        # Get policy id for specified policy type
-        policy_id = self.get_policy("client_forwarding").id
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
 
-        payload = convert_keys(self.get_rule("client_forwarding", rule_id))
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
 
-        # Add optional parameters to payload
+        # Add or update optional parameters to the payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
+            elif key == "action":
+                payload["action"] = value.upper()
             else:
                 payload[snake_to_camel(key)] = value
 
-        # Set the action in the payload
-        payload["action"] = action
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
 
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("client_forwarding", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
-    def add_isolation_rule(self, name: str, action: str, zpn_isolation_profile_id: str, **kwargs) -> Box:
+    def add_isolation_rule_v2(self, name: str, action: str, zpn_isolation_profile_id: str, **kwargs) -> Box:
         """
         Add a new Isolation Policy rule.
 
         See the
         `ZPA Isolation Policy API reference <https://help.zscaler.com/zpa/configuring-isolation-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -704,15 +1796,15 @@
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": action.upper(),
             "zpnIsolationProfileId": zpn_isolation_profile_id,
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         # Pre-configure client_type to 'zpn_client_type_exporter'
         payload["conditions"].append({"operands": [{"objectType": "CLIENT_TYPE", "values": ["zpn_client_type_exporter"]}]})
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("isolation").id
@@ -725,15 +1817,15 @@
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_isolation_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_isolation_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing client isolation policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
             rule_id (str):
@@ -783,45 +1875,58 @@
             ...         ("app", ["216199618143361683"]),
             ...         ("app_group", ["216199618143360301"]),
             ...         ("scim_group", [("216199618143191058", "2079468"), ("216199618143191058", "2079446")]),
             ...     ],
             ... )
         """
 
+        # Pre-set the policy_type to "timeout"
+        policy_type = "isolation"
+
         # Ensure the action is provided and convert to uppercase
         if "action" not in kwargs:
             raise ValueError("The 'action' attribute is mandatory.")
 
         action = kwargs.pop("action").upper()
 
-        # Get policy id for specified policy type
-        policy_id = self.get_policy("isolation").id
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
 
-        payload = convert_keys(self.get_rule("isolation", rule_id))
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
             else:
                 payload[snake_to_camel(key)] = value
 
         # Pre-configure client_type to 'zpn_client_type_exporter'
         payload["conditions"].append({"operands": [{"objectType": "CLIENT_TYPE", "values": ["zpn_client_type_exporter"]}]})
 
         # Set the action in the payload
         payload["action"] = action
 
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("isolation", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
-    def add_app_protection_rule(self, name: str, action: str, zpn_inspection_profile_id: str, **kwargs) -> Box:
+    def add_app_protection_rule_v2(self, name: str, action: str, zpn_inspection_profile_id: str, **kwargs) -> Box:
         """
         Add a new AppProtection Policy rule.
 
         See the
         `ZPA AppProtection Policy API reference <https://help.zscaler.com/zpa/configuring-appprotection-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -860,15 +1965,15 @@
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": action.upper(),
             "zpnInspectionProfileId": zpn_inspection_profile_id,
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("inspection").id
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
@@ -878,15 +1983,15 @@
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_app_protection_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_app_protection_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing app protection policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
             rule_id (str):
@@ -937,42 +2042,64 @@
             ...         ("app", ["216199618143361683"]),
             ...         ("app_group", ["216199618143360301"]),
             ...         ("scim_group", [("216199618143191058", "2079468"), ("216199618143191058", "2079446")]),
             ...     ],
             ... )
         """
 
+        # Pre-set the policy_type to "timeout"
+        policy_type = "inspection"
+
         # Ensure the action is provided and convert to uppercase
         if "action" not in kwargs:
             raise ValueError("The 'action' attribute is mandatory.")
 
         action = kwargs.pop("action").upper()
 
-        # Get policy id for specified policy type
-        policy_id = self.get_policy("inspection").id
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
 
-        payload = convert_keys(self.get_rule("inspection", rule_id))
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
 
-        # Add optional parameters to payload
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
+
+        # Add or update optional parameters to the payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
+            elif key == "action":
+                payload["action"] = value.upper()
             else:
                 payload[snake_to_camel(key)] = value
 
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
         # Set the action in the payload
         payload["action"] = action
 
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("inspection", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
-    def add_privileged_credential_rule(self, name: str, credential_id: str, **kwargs) -> Box:
+    def add_privileged_credential_rule_v2(self, name: str, credential_id: str, **kwargs) -> Box:
         """
         Add a new Privileged Remote Access Credential Policy rule.
 
         See the
         `ZPA Privileged Policies API reference <https://help.zscaler.com/zpa/configuring-privileged-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -994,15 +2121,16 @@
             rule_order (str):
                 The rule evaluation order number of the rule.
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`, `RHS value`.
                 If you are adding multiple values for the same object type then you will need a new entry for each value.
 
                 * `conditions`: This is for providing the set of conditions for the policy
-                    * `object_type`: This is for specifying the policy criteria. The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
+                    * `object_type`: This is for specifying the policy criteria.
+                        The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
                         * `saml`: The unique Identity Provider ID and SAML attribute ID
                         * `scim`: The unique Identity Provider ID and SCIM attribute ID
                         * `scim_group`: The unique Identity Provider ID and SCIM_GROUP ID
 
                 .. code-block:: python
 
                     zpa.policiesv2.add_privileged_credential_rule(
@@ -1020,15 +2148,15 @@
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": "INJECT_CREDENTIALS",
             "credential": {"id": credential_id},
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("credential").id
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
@@ -1038,15 +2166,15 @@
         if isinstance(response, Response):
             # This is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_privileged_credential_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_privileged_credential_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing privileged credential policy rule.
 
         Args:
             rule_id (str):
                 The unique identifier for the rule to be updated.
             **kwargs: Optional keyword args.
@@ -1083,44 +2211,64 @@
             Updates the name only for an Credential Policy rule:
 
             >>> zpa.policiesv2.update_privileged_credential_rule(
             ...   rule_id='888888',
             ...   name='credential_rule_new_name')
 
         """
-        # Get the policy id for the specified policy type
-        policy_id = self.get_policy("credential").id
+        # Pre-set the policy_type to "timeout"
+        policy_type = "credential"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
 
-        # Retrieve the existing rule to update
-        payload = convert_keys(self.get_rule("credential", rule_id))
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
             elif key == "credential_id":
                 payload["credential"] = {"id": value}
             else:
                 payload[snake_to_camel(key)] = value
 
         # Ensure the action is set to CHECK_CAPABILITIES
         payload["action"] = "INJECT_CREDENTIALS"
 
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("credential", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
-    def add_capabilities_rule(self, name: str, **kwargs) -> Box:
+    def add_capabilities_rule_v2(self, name: str, **kwargs) -> Box:
         """
         Add a new Capability Access rule.
 
         See the
-        `ZPA Capabilities Policies API reference <https://help.zscaler.com/zpa/configuring-privileged-policies-using-api#postV2cap>`_
+        `ZPA Capabilities Policies API reference:
+        <https://help.zscaler.com/zpa/configuring-privileged-policies-using-api#postV2cap>`_
         for further detail on optional keyword parameter structures.
 
         Args:
             name (str):
                 The name of the new capability rule.
             action (str):
                 The action for the policy. Accepted value is: ``CHECK_CAPABILITIES``
@@ -1132,45 +2280,46 @@
             rule_order (str):
                 The new order for the rule.
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`, `RHS value`.
                 If you are adding multiple values for the same object type then you will need a new entry for each value.
 
                 - `conditions`: This is for providing the set of conditions for the policy
-                    - `object_type`: This is for specifying the policy criteria. The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
+                    - `object_type`: This is for specifying the policy criteria.
+                        The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
                         - `app`: The unique Application Segment ID
                         - `app_group`: The unique Segment Group ID
                         - `saml`: The unique Identity Provider ID and SAML attribute ID
                         - `scim`: The unique Identity Provider ID and SCIM attribute ID
                         - `scim_group`: The unique Identity Provider ID and SCIM_GROUP ID
 
-            privileged_capabilities (dict): A dictionary specifying the privileged capabilities with boolean values. The supported capabilities are:
+            privileged_capabilities (dict): A dictionary specifying the privileged capabilities with boolean values.
+                The supported capabilities are:
 
                 - clipboard_copy (bool): Indicates the PRA Clipboard Copy function.
                 - clipboard_paste (bool): Indicates the PRA Clipboard Paste function.
                 - file_upload (bool): Indicates the PRA File Transfer capabilities that enables the File Upload function.
                 - file_download (bool): Indicates the PRA File Transfer capabilities that enables the File Download function.
-                - inspect_file_upload (bool): Inspects the file via ZIA sandbox and uploads the file following the inspection.
-                - inspect_file_download (bool): Inspects the file via ZIA sandbox and downloads the file following the inspection.
-                - monitor_session (bool): Indicates the PRA Monitoring Capabilities to enable the PRA Session Monitoring function.
-                - record_session (bool): Indicates the PRA Session Recording capabilities to enable PRA Session Recording.
-                - share_session (bool): Indicates the PRA Session Control and Monitoring capabilities to enable PRA Session Monitoring.
+                - inspect_file_upload (bool): Inspects the file via ZIA sandbox and uploads the file after inspection.
+                - inspect_file_download (bool): Inspects the file via ZIA sandbox and downloads the file after the inspection.
+                - monitor_session (bool): Indicates the PRA Monitoring Capabilities to enable the PRA Session Monitoring.
+                - record_session (bool): Indicates PRA Session Recording capabilities to enable PRA Session Recording.
+                - share_session (bool): Indicates PRA Session Control/Monitoring capabilities to enable PRA Session Monitoring.
 
         Returns:
             :obj:`Box`: The resource record of the newly created Capabilities rule.
 
         Example:
             Add a new capability rule with various capabilities and conditions:
 
             .. code-block:: python
 
                 zpa.policiesv2.add_capabilities_rule(
                     name='New_Capability_Rule',
                     description='New_Capability_Rule',
-                    action='check_capabilities',
                     conditions=[
                         ("app", ["app_segment_id"]),
                         ("app_group", ["segment_group_id"]),
                         ("scim_group", [("idp_id", "scim_group_id"), ("idp_id", "scim_group_id")])
                     ],
                     privileged_capabilities={
                         "clipboard_copy": True,
@@ -1184,15 +2333,15 @@
                 )
         """
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": "CHECK_CAPABILITIES",
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         # Process privileged capabilities
         if "privileged_capabilities" in kwargs:
             capabilities = []
             priv_caps_map = kwargs.pop("privileged_capabilities")
 
@@ -1200,17 +2349,17 @@
                 capabilities.append("CLIPBOARD_COPY")
             if priv_caps_map.get("clipboard_paste", False):
                 capabilities.append("CLIPBOARD_PASTE")
             if priv_caps_map.get("file_download", False):
                 capabilities.append("FILE_DOWNLOAD")
 
             # Handling the edge case for file_upload
-            if priv_caps_map.get("file_upload") == True:
+            if priv_caps_map.get("file_upload") is True:
                 capabilities.append("FILE_UPLOAD")
-            elif priv_caps_map.get("file_upload") == False:
+            elif priv_caps_map.get("file_upload") is False:
                 capabilities.append("INSPECT_FILE_UPLOAD")
             # If file_upload is not present or set to None, do not append either capability
 
             if priv_caps_map.get("inspect_file_download", False):
                 capabilities.append("INSPECT_FILE_DOWNLOAD")
             if priv_caps_map.get("inspect_file_upload", False):
                 capabilities.append("INSPECT_FILE_UPLOAD")
@@ -1234,20 +2383,21 @@
         if isinstance(response, Response):
             # This is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_capabilities_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_capabilities_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing capabilities policy rule.
 
         See the
-        `ZPA Capabilities Policies API reference <https://help.zscaler.com/zpa/configuring-privileged-policies-using-api#postV2cap>`_
+        `ZPA Capabilities Policies API reference:
+        <https://help.zscaler.com/zpa/configuring-privileged-policies-using-api#postV2cap>`_
         for further detail on optional keyword parameter structures.
 
         Args:
             rule_id (str):
                 The unique identifier for the rule to be updated.
             **kwargs:
                 Optional keyword args.
@@ -1256,40 +2406,42 @@
             rule_order (str):
                 The new order for the rule.
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`, `RHS value`.
                 If you are adding multiple values for the same object type then you will need a new entry for each value.
 
                 - `conditions`: This is for providing the set of conditions for the policy
-                    - `object_type`: This is for specifying the policy criteria. The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
+                    - `object_type`: This is for specifying the policy criteria.
+                        The following values are supported: "app", "app_group", "saml", "scim", "scim_group"
                         - `app`: The unique Application Segment ID
                         - `app_group`: The unique Segment Group ID
                         - `saml`: The unique Identity Provider ID and SAML attribute ID
                         - `scim`: The unique Identity Provider ID and SCIM attribute ID
                         - `scim_group`: The unique Identity Provider ID and SCIM_GROUP ID
 
-            privileged_capabilities (dict): A dictionary specifying the privileged capabilities with boolean values. The supported capabilities are:
+            privileged_capabilities (dict): A dictionary specifying the privileged capabilities with boolean values.
+                The supported capabilities are:
 
                 - clipboard_copy (bool): Indicates the PRA Clipboard Copy function.
                 - clipboard_paste (bool): Indicates the PRA Clipboard Paste function.
                 - file_upload (bool): Indicates the PRA File Transfer capabilities that enables the File Upload function.
                 - file_download (bool): Indicates the PRA File Transfer capabilities that enables the File Download function.
-                - inspect_file_upload (bool): Inspects the file via ZIA sandbox and uploads the file following the inspection.
-                - inspect_file_download (bool): Inspects the file via ZIA sandbox and downloads the file following the inspection.
-                - monitor_session (bool): Indicates the PRA Monitoring Capabilities to enable the PRA Session Monitoring function.
-                - record_session (bool): Indicates the PRA Session Recording capabilities to enable PRA Session Recording.
-                - share_session (bool): Indicates the PRA Session Control and Monitoring capabilities to enable PRA Session Monitoring.
+                - inspect_file_upload (bool): Inspects the file via ZIA sandbox and uploads the file after the inspection.
+                - inspect_file_download (bool): Inspects the file via ZIA sandbox and downloads the file after inspection.
+                - monitor_session (bool): Indicates PRA Monitoring Capabilities to enable the PRA Session Monitoring.
+                - record_session (bool): Indicates PRA Session Recording capabilities to enable PRA Session Recording.
+                - share_session (bool): Indicates PRA Session Control/Monitoring capabilities to enable PRA Session Monitoring.
 
         Returns:
             :obj:`Box`: The updated policy-capability-rule resource record.
 
         Examples:
             Updates the name and capabilities for an existing Capability Policy rule:
 
-            >>> zpa.policiesv2.update_capabilities_rule(
+            >>> zpa.policiesv2.update_capabilities_rule_v2(
             ... rule_id='888888',
             ... name='Updated_Capability_Rule',
             ... conditions=[
             ...     ("app", ["216199618143361683"]),
             ...     ("app_group", ["216199618143360301"]),
             ...     ("scim_group", [("216199618143191058", "2079468"), ("216199618143191058", "2079446")])
             ... ],
@@ -1297,39 +2449,47 @@
             ...     "clipboard_copy": True,
             ...     "clipboard_paste": True,
             ...     "file_download": True,
             ...     "file_upload": None
             ... }
             ... )
         """
-        # Get the policy id for the specified policy type
-        policy_id = self.get_policy("capabilities").id
 
-        # Retrieve the existing rule to update
-        payload = convert_keys(self.get_rule("capabilities", rule_id))
+        # Pre-set the policy_type to "access"
+        policy_type = "capabilities"
+
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
+
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
             elif key == "privileged_capabilities":
                 capabilities = []
                 priv_caps_map = value
 
                 if priv_caps_map.get("clipboard_copy", False):
                     capabilities.append("CLIPBOARD_COPY")
                 if priv_caps_map.get("clipboard_paste", False):
                     capabilities.append("CLIPBOARD_PASTE")
                 if priv_caps_map.get("file_download", False):
                     capabilities.append("FILE_DOWNLOAD")
 
                 # Handling the edge case for file_upload
-                if priv_caps_map.get("file_upload") == True:
+                if priv_caps_map.get("file_upload") is True:
                     capabilities.append("FILE_UPLOAD")
-                elif priv_caps_map.get("file_upload") == False:
+                elif priv_caps_map.get("file_upload") is False:
                     capabilities.append("INSPECT_FILE_UPLOAD")
                 # If file_upload is not present or set to None, do not append either capability
 
                 if priv_caps_map.get("inspect_file_download", False):
                     capabilities.append("INSPECT_FILE_DOWNLOAD")
                 if priv_caps_map.get("inspect_file_upload", False):
                     capabilities.append("INSPECT_FILE_UPLOAD")
@@ -1342,21 +2502,33 @@
 
                 payload["privilegedCapabilities"] = {"capabilities": capabilities}
             else:
                 payload[snake_to_camel(key)] = value
 
         payload["action"] = "CHECK_CAPABILITIES"
 
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("capabilities", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
-    def add_redirection_rule(self, name: str, action: str, service_edge_group_ids: list = [], **kwargs) -> Box:
+    def add_redirection_rule_v2(self, name: str, action: str, service_edge_group_ids: list = [], **kwargs) -> Box:
         """
         Add a new Redirection Policy rule.
 
         See the
         `ZPA Redirection Policy API reference <https://help.zscaler.com/zpa/configuring-redirection-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -1375,15 +2547,16 @@
         Keyword Args:
             conditions (list):
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
                 `RHS value`. If you are adding multiple values for the same object type then you will need
                 a new entry for each value.
 
                 * `conditions`: This is for providing the set of conditions for the policy
-                    * `object_type`: This is for specifying the policy criteria. The following values are supported: "app", "app_group", "saml", "scim", "scim_group", "client_type"
+                    * `object_type`: This is for specifying the policy criteria.
+                        The following values are supported: "app", "app_group", "saml", "scim", "scim_group", "client_type"
                         * `client_type`: The client type, must be one of the following:
                             - 'zpn_client_type_edge_connector'
                             - 'zpn_client_type_branch_connector'
                             - 'zpn_client_type_machine_tunnel'
                             - 'zpn_client_type_zapp'
                             - 'zpn_client_type_zapp_partner'
 
@@ -1396,29 +2569,34 @@
             .. code-block:: python
 
                 zpa.policiesv2.add_redirection_rule(
                     name='New_Redirection_Rule',
                     action='redirect_preferred',
                     service_edge_group_ids=['12345', '67890'],
                     conditions=[
-                        ("client_type", 'zpn_client_type_edge_connector', 'zpn_client_type_branch_connector', 'zpn_client_type_machine_tunnel', 'zpn_client_type_zapp', 'zpn_client_type_zapp_partner'),
+                        ("client_type",
+                            'zpn_client_type_edge_connector',
+                            'zpn_client_type_branch_connector',
+                            'zpn_client_type_machine_tunnel',
+                            'zpn_client_type_zapp',
+                            'zpn_client_type_zapp_partner'),
                     ]
                 )
         """
         # Validate action and service_edge_group_ids based on action type
         if action.lower() == "redirect_default" and service_edge_group_ids:
             raise ValueError("service_edge_group_ids cannot be set when action is 'redirect_default'.")
         elif action.lower() in ["redirect_preferred", "redirect_always"] and not service_edge_group_ids:
             raise ValueError("service_edge_group_ids must be set when action is 'redirect_preferred' or 'redirect_always'.")
 
         # Initialise the payload
         payload = {
             "name": name,
             "action": action.upper(),
-            "conditions": self._create_conditions(kwargs.pop("conditions", [])),
+            "conditions": self._create_conditions_v2(kwargs.pop("conditions", [])),
         }
 
         if service_edge_group_ids:
             payload["serviceEdgeGroups"] = [{"id": group_id} for group_id in service_edge_group_ids]
 
         # Validate client_type values within conditions
         valid_client_types = [
@@ -1445,15 +2623,15 @@
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_redirection_rule(self, rule_id: str, **kwargs) -> Box:
+    def update_redirection_rule_v2(self, rule_id: str, **kwargs) -> Box:
         """
         Update an existing policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
 
         Args:
 
@@ -1479,83 +2657,112 @@
                 A list of conditional rule tuples. Tuples must follow the convention: `Object Type`, `LHS value`,
                 `RHS value`. If you are adding multiple values for the same object type then you will need
                 a new entry for each value.
                 E.g.
 
                 .. code-block:: python
 
-                    ("client_type", ['zpn_client_type_edge_connector', 'zpn_client_type_branch_connector', 'zpn_client_type_machine_tunnel', 'zpn_client_type_zapp', 'zpn_client_type_zapp_partner']),
+                    ("client_type", [
+                        'zpn_client_type_edge_connector',
+                        'zpn_client_type_branch_connector',
+                        'zpn_client_type_machine_tunnel',
+                        'zpn_client_type_zapp',
+                        'zpn_client_type_zapp_partner'
+                    ]),
 
         Returns:
             :obj:`Box`: The updated policy-rule resource record.
 
         Examples:
             Updates the name only for an Access Policy rule:
 
             >>> zpa.policiesv2.update_redirection_rule(
             ...    rule_id='216199618143320419',
             ...    name='Update_Redirection_Rule_v2',
             ...    description='Update_Redirection_Rule_v2',
             ...    action='redirect_default',
             ...    conditions=[
-            ...         ("client_type", ['zpn_client_type_edge_connector', 'zpn_client_type_branch_connector', 'zpn_client_type_machine_tunnel', 'zpn_client_type_zapp', 'zpn_client_type_zapp_partner']),
+            ...         ("client_type", [
+            ...          'zpn_client_type_edge_connector',
+            ...          'zpn_client_type_branch_connector',
+            ...          'zpn_client_type_machine_tunnel',
+            ...          'zpn_client_type_zapp',
+            ...          'zpn_client_type_zapp_partner']),
             ...     ],
-            ...         )
+            ... )
         """
 
+        # Pre-set the policy_type to "access"
+        policy_type = "redirection"
+
         # Ensure the action is provided and convert to uppercase
         if "action" not in kwargs:
             raise ValueError("The 'action' attribute is mandatory.")
 
         action = kwargs.pop("action").upper()
 
-        # Get policy id for specified policy type
-        policy_id = self.get_policy("redirection").id
+        # Get the current rule details
+        current_rule = self.get_rule(policy_type, rule_id)
+
+        # Initialize the payload with existing rule details
+        payload = convert_keys(current_rule)
 
-        payload = convert_keys(self.get_rule("redirection", rule_id))
+        # Remove any existing conditions if they are not being updated
+        if "conditions" in payload and "conditions" not in kwargs:
+            del payload["conditions"]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
-                payload["conditions"] = self._create_conditions(value)
+                payload["conditions"] = self._create_conditions_v2(value)
             else:
                 payload[snake_to_camel(key)] = value
 
         # Set the action in the payload
         payload["action"] = action
 
+        # Remove the conditions key if it exists but is empty
+        payload = {k: v for k, v in payload.items() if k != "conditions" or v}
+
+        # Get policy id for specified policy type
+        policy_id = self.get_policy(policy_type).id
+
         # Make the PUT request to update the rule
         response = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload, api_version="v2")
-        # Return the object if it was updated successfully
-        if not isinstance(response, Response):
-            return self.get_rule("redirection", rule_id)
+        if response.status_code == 204:
+            # Return the updated rule if the response was successful
+            updated_rule = self.get_rule(policy_type, rule_id)
+            if not updated_rule:
+                raise Exception(f"Failed to retrieve the updated rule with ID {rule_id}")
+            return updated_rule
+        else:
+            # Handle error response
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
     def reorder_rule(self, policy_type: str, rule_id: str, rule_order: str) -> Box:
         """
         Change the order of an existing policy rule.
 
         Args:
             rule_id (str):
                 The unique id of the rule that will be reordered.
             rule_order (str):
                 The new order for the rule.
             policy_type (str):
                 The policy type. Accepted values are:
 
-                 |  ``access`` - returns the Access Policy
-                 |  ``capabilities`` - returns the Capabilities Policy
-                 |  ``client_forwarding`` - returns the Client Forwarding Policy
-                 |  ``clientless`` - returns the Clientlesss Session Protection Policy
-                 |  ``credential`` - returns the Credential Policy
-                 |  ``inspection`` - returns the Inspection Policy
-                 |  ``isolation`` - returns the Isolation Policy
-                 |  ``redirection`` - returns the Redirection Policy
-                 |  ``siem`` - returns the SIEM Policy
-                 |  ``timeout`` - returns the Timeout Policy
-
+                 |  ``access``
+                 |  ``timeout``
+                 |  ``client_forwarding``
+                 |  ``isolation``
+                 |  ``inspection``
+                 |  ``redirection``
+                 |  ``credential``
+                 |  ``capabilities``
+                 |  ``siem``
 
         Returns:
              :obj:`Box`: The updated policy rule resource record.
 
         Examples:
             Updates the order for an existing policy rule:
 
@@ -1595,25 +2802,23 @@
 
         Args:
             rules_orders (dict(rule_id=>order)):
                 A map of rule IDs and orders
             policy_type (str):
                 The policy type. Accepted values are:
 
-                 |  ``access`` - returns the Access Policy
-                 |  ``capabilities`` - returns the Capabilities Policy
-                 |  ``client_forwarding`` - returns the Client Forwarding Policy
-                 |  ``clientless`` - returns the Clientlesss Session Protection Policy
-                 |  ``credential`` - returns the Credential Policy
-                 |  ``inspection`` - returns the Inspection Policy
-                 |  ``isolation`` - returns the Isolation Policy
-                 |  ``redirection`` - returns the Redirection Policy
-                 |  ``siem`` - returns the SIEM Policy
-                 |  ``timeout`` - returns the Timeout Policy
-
+                 |  ``access``
+                 |  ``timeout``
+                 |  ``client_forwarding``
+                 |  ``isolation``
+                 |  ``inspection``
+                 |  ``redirection``
+                 |  ``credential``
+                 |  ``capabilities``
+                 |  ``siem``
 
         """
         # Get policy id for specified policy type
         policy_set = self.get_policy(policy_type).id
         all = self.list_rules(policy_type)
         all.sort(key=functools.cmp_to_key(self.sort_key(rules_orders=rules_orders)))
         orderedRules = [r.id for r in all]
```

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.3.1/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.3.0/PKG-INFO` & `zscaler_sdk_python-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
@@ -19,21 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Requires-Dist: aenum ; extra == "dev"
 Requires-Dist: arrow
-Requires-Dist: black ; extra == "dev"
+Requires-Dist: black (>=24.3.0) ; extra == "dev"
 Requires-Dist: certifi
 Requires-Dist: charset-normalizer
 Requires-Dist: cryptography (>=3.4,<43.0)
 Requires-Dist: flake8
 Requires-Dist: flatdict
 Requires-Dist: idna
+Requires-Dist: okta (>=2.9.7)
 Requires-Dist: pycryptodomex
 Requires-Dist: pydash ; extra == "dev"
 Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: pyyaml
 Requires-Dist: requests (>=2.32.0)
```

