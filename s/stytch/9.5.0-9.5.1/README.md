# Comparing `tmp/stytch-9.5.0.tar.gz` & `tmp/stytch-9.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-9.5.0.tar", last modified: Mon May 20 17:51:00 2024, max compression
+gzip compressed data, was "stytch-9.5.1.tar", last modified: Wed May 29 20:18:28 2024, max compression
```

## Comparing `stytch-9.5.0.tar` & `stytch-9.5.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-20 17:50:47.000000 stytch-9.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-20 17:51:00.052755 stytch-9.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-20 17:50:47.000000 stytch-9.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:51:00.052755 stytch-9.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-20 17:50:47.000000 stytch-9.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.032755 stytch-9.5.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.036755 stytch-9.5.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.040755 stytch-9.5.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31710 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    55751 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.044755 stytch-9.5.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/totps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.044755 stytch-9.5.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.048755 stytch-9.5.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/lazy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/method_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/policy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/rbac_local.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-20 17:50:47.000000 stytch-9.5.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-20 17:50:47.000000 stytch-9.5.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 20:18:10.000000 stytch-9.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-29 20:18:28.828014 stytch-9.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-29 20:18:10.000000 stytch-9.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 20:18:28.828014 stytch-9.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-29 20:18:10.000000 stytch-9.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.808014 stytch-9.5.1/stytch/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.808014 stytch-9.5.1/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.816014 stytch-9.5.1/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31710 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55751 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.820014 stytch-9.5.1/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/b2b/models/totps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.820014 stytch-9.5.1/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.824014 stytch-9.5.1/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/stytch/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/lazy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/method_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/policy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/shared/rbac_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 20:18:10.000000 stytch-9.5.1/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-29 20:18:28.000000 stytch-9.5.1/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-29 20:18:28.000000 stytch-9.5.1/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:18:28.000000 stytch-9.5.1/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 20:18:28.000000 stytch-9.5.1/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 20:18:28.000000 stytch-9.5.1/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:18:28.828014 stytch-9.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-29 20:18:10.000000 stytch-9.5.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-29 20:18:10.000000 stytch-9.5.1/test/test_integration_async.py
```

### Comparing `stytch-9.5.0/LICENSE.txt` & `stytch-9.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/PKG-INFO` & `stytch-9.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.5.0
+Version: 9.5.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.5.0/README.md` & `stytch-9.5.1/README.md`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/setup.py` & `stytch-9.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/discovery.py` & `stytch-9.5.1/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-9.5.1/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/discovery_organizations.py` & `stytch-9.5.1/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/magic_links.py` & `stytch-9.5.1/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-9.5.1/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/magic_links_email.py` & `stytch-9.5.1/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-9.5.1/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/oauth.py` & `stytch-9.5.1/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/oauth_discovery.py` & `stytch-9.5.1/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/organizations.py` & `stytch-9.5.1/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/organizations_members.py` & `stytch-9.5.1/stytch/b2b/api/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/organizations_members_oauth_providers.py` & `stytch-9.5.1/stytch/b2b/api/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/otp.py` & `stytch-9.5.1/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/otp_sms.py` & `stytch-9.5.1/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/passwords.py` & `stytch-9.5.1/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/passwords_email.py` & `stytch-9.5.1/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-9.5.1/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/passwords_session.py` & `stytch-9.5.1/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/rbac.py` & `stytch-9.5.1/stytch/b2b/api/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/recovery_codes.py` & `stytch-9.5.1/stytch/b2b/api/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/scim.py` & `stytch-9.5.1/stytch/b2b/api/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/scim_connections.py` & `stytch-9.5.1/stytch/b2b/api/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/sessions.py` & `stytch-9.5.1/stytch/b2b/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/sso.py` & `stytch-9.5.1/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/sso_oidc.py` & `stytch-9.5.1/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/sso_saml.py` & `stytch-9.5.1/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/api/totps.py` & `stytch-9.5.1/stytch/b2b/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/client.py` & `stytch-9.5.1/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/discovery.py` & `stytch-9.5.1/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-9.5.1/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/discovery_organizations.py` & `stytch-9.5.1/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/magic_links.py` & `stytch-9.5.1/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-9.5.1/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/magic_links_email.py` & `stytch-9.5.1/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/mfa.py` & `stytch-9.5.1/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/oauth.py` & `stytch-9.5.1/stytch/b2b/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/oauth_discovery.py` & `stytch-9.5.1/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/organizations.py` & `stytch-9.5.1/stytch/b2b/models/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/organizations_members.py` & `stytch-9.5.1/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/organizations_members_oauth_providers.py` & `stytch-9.5.1/stytch/b2b/models/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/otp_sms.py` & `stytch-9.5.1/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/passwords.py` & `stytch-9.5.1/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/passwords_email.py` & `stytch-9.5.1/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-9.5.1/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/passwords_session.py` & `stytch-9.5.1/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/rbac.py` & `stytch-9.5.1/stytch/b2b/models/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/recovery_codes.py` & `stytch-9.5.1/stytch/b2b/models/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/scim.py` & `stytch-9.5.1/stytch/b2b/models/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/scim_connections.py` & `stytch-9.5.1/stytch/b2b/models/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/sessions.py` & `stytch-9.5.1/stytch/b2b/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/sso.py` & `stytch-9.5.1/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/sso_oidc.py` & `stytch-9.5.1/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/sso_saml.py` & `stytch-9.5.1/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/b2b/models/totps.py` & `stytch-9.5.1/stytch/b2b/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/crypto_wallets.py` & `stytch-9.5.1/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/m2m.py` & `stytch-9.5.1/stytch/consumer/api/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/m2m_clients.py` & `stytch-9.5.1/stytch/consumer/api/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/m2m_clients_secrets.py` & `stytch-9.5.1/stytch/consumer/api/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/magic_links.py` & `stytch-9.5.1/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/magic_links_email.py` & `stytch-9.5.1/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/oauth.py` & `stytch-9.5.1/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/otp.py` & `stytch-9.5.1/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/otp_email.py` & `stytch-9.5.1/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/otp_sms.py` & `stytch-9.5.1/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-9.5.1/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/passwords.py` & `stytch-9.5.1/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/passwords_email.py` & `stytch-9.5.1/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/passwords_existing_password.py` & `stytch-9.5.1/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/passwords_session.py` & `stytch-9.5.1/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/project.py` & `stytch-9.5.1/stytch/consumer/api/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/sessions.py` & `stytch-9.5.1/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/totps.py` & `stytch-9.5.1/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/users.py` & `stytch-9.5.1/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/api/webauthn.py` & `stytch-9.5.1/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/client.py` & `stytch-9.5.1/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/crypto_wallets.py` & `stytch-9.5.1/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/m2m.py` & `stytch-9.5.1/stytch/consumer/models/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/m2m_clients.py` & `stytch-9.5.1/stytch/consumer/models/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/m2m_clients_secrets.py` & `stytch-9.5.1/stytch/consumer/models/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/magic_links.py` & `stytch-9.5.1/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/magic_links_email.py` & `stytch-9.5.1/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/oauth.py` & `stytch-9.5.1/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/otp.py` & `stytch-9.5.1/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/otp_email.py` & `stytch-9.5.1/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/otp_sms.py` & `stytch-9.5.1/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-9.5.1/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/passwords.py` & `stytch-9.5.1/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/passwords_email.py` & `stytch-9.5.1/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-9.5.1/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/passwords_session.py` & `stytch-9.5.1/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/project.py` & `stytch-9.5.1/stytch/consumer/models/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/sessions.py` & `stytch-9.5.1/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/totps.py` & `stytch-9.5.1/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/users.py` & `stytch-9.5.1/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/consumer/models/webauthn.py` & `stytch-9.5.1/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/core/api_base.py` & `stytch-9.5.1/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/core/client_base.py` & `stytch-9.5.1/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/core/http/client.py` & `stytch-9.5.1/stytch/core/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,24 @@
         project_id: str,
         secret: str,
         session: Optional[aiohttp.ClientSession] = None,
     ) -> None:
         super().__init__(project_id, secret)
         self.auth = aiohttp.BasicAuth(project_id, secret)
         self._external_session = session is not None
-        self._session = session or aiohttp.ClientSession()
+        self.__session = session
+
+    @property
+    def _session(self) -> aiohttp.ClientSession:
+        if self.__session is None:
+            self.__session = aiohttp.ClientSession()
+        return self.__session
 
     def __del__(self) -> None:
-        if self._external_session:
+        if self._external_session or self.__session is None:
             return
 
         # If we're responsible for the session, close it now
         try:
             loop = asyncio.get_event_loop()
             if loop.is_running():
                 loop.create_task(self._session.close())
```

### Comparing `stytch-9.5.0/stytch/core/response_base.py` & `stytch-9.5.1/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/shared/jwt_helpers.py` & `stytch-9.5.1/stytch/shared/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/shared/lazy_cache.py` & `stytch-9.5.1/stytch/shared/lazy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/shared/method_options.py` & `stytch-9.5.1/stytch/shared/method_options.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/shared/policy_cache.py` & `stytch-9.5.1/stytch/shared/policy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch/shared/rbac_local.py` & `stytch-9.5.1/stytch/shared/rbac_local.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/stytch.egg-info/PKG-INFO` & `stytch-9.5.1/stytch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.5.0
+Version: 9.5.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.5.0/stytch.egg-info/SOURCES.txt` & `stytch-9.5.1/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/test/test_integration.py` & `stytch-9.5.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-9.5.0/test/test_integration_async.py` & `stytch-9.5.1/test/test_integration_async.py`

 * *Files identical despite different names*

