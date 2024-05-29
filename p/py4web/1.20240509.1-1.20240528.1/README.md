# Comparing `tmp/py4web-1.20240509.1.tar.gz` & `tmp/py4web-1.20240528.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240509.1.tar", last modified: Fri May 10 05:27:06 2024, max compression
+gzip compressed data, was "py4web-1.20240528.1.tar", last modified: Wed May 29 05:04:11 2024, max compression
```

## Comparing `py4web-1.20240509.1.tar` & `py4web-1.20240528.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.565761 py4web-1.20240509.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240509.1/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-10 05:27:06.565761 py4web-1.20240509.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-28 19:36:37.000000 py4web-1.20240509.1/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.532426 py4web-1.20240509.1/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      764 2024-05-10 05:26:17.000000 py4web-1.20240509.1/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.552427 py4web-1.20240509.1/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-10 05:26:59.000000 py4web-1.20240509.1/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392764 2024-05-10 05:26:59.000000 py4web-1.20240509.1/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68805 2024-05-10 05:25:35.000000 py4web-1.20240509.1/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.559094 py4web-1.20240509.1/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72777 2024-05-08 05:42:38.000000 py4web-1.20240509.1/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.562427 py4web-1.20240509.1/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240509.1/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35921 2024-05-02 06:57:14.000000 py4web-1.20240509.1/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69667 2024-05-02 06:57:02.000000 py4web-1.20240509.1/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.532426 py4web-1.20240509.1/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-05-10 05:26:03.000000 py4web-1.20240509.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-28 20:10:23.000000 py4web-1.20240509.1/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-10 05:27:06.565761 py4web-1.20240509.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.565761 py4web-1.20240509.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240509.1/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8104 2024-04-28 20:10:23.000000 py4web-1.20240509.1/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240509.1/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.657328 py4web-1.20240528.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240528.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 05:04:11.657328 py4web-1.20240528.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240528.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.623994 py4web-1.20240528.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-29 04:58:50.000000 py4web-1.20240528.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.643995 py4web-1.20240528.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199954 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394058 2024-05-29 05:04:05.000000 py4web-1.20240528.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74611 2024-05-28 00:14:10.000000 py4web-1.20240528.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.650661 py4web-1.20240528.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-25 08:37:03.000000 py4web-1.20240528.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.653995 py4web-1.20240528.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240528.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69783 2024-05-24 05:08:52.000000 py4web-1.20240528.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-27 07:35:43.000000 py4web-1.20240528.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.627328 py4web-1.20240528.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-29 04:58:33.000000 py4web-1.20240528.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240528.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-29 05:04:11.657328 py4web-1.20240528.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.657328 py4web-1.20240528.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240528.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_url.py
```

### Comparing `py4web-1.20240509.1/LICENSE.md` & `py4web-1.20240528.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/PKG-INFO` & `py4web-1.20240528.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240509.1
+Version: 1.20240528.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -191,8 +191,8 @@
 - `John M. Wolf <https://github.com/jmwolff3>`__
 - `Micah Beasley <https://github.com/MBfromOK>`__
 - `Nico Zanferrari <https://github.com/nicozanf>`__
 - `Pirsch <https://github.com/Pirsch>`__
 - `sugizo <https://github.com/sugizo>`__
 - `valq7711 <https://github.com/valq7711>`__
 - `Kevin Keller <https://github.com/Kkeller83>`__
-- `Sam de Alfaro <sam@dealfaro.com>`__ (logo design)
+- Sam de Alfaro sam@dealfaro.com (logo design)
```

### Comparing `py4web-1.20240509.1/README.rst` & `py4web-1.20240528.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -176,8 +176,8 @@
 - `John M. Wolf <https://github.com/jmwolff3>`__
 - `Micah Beasley <https://github.com/MBfromOK>`__
 - `Nico Zanferrari <https://github.com/nicozanf>`__
 - `Pirsch <https://github.com/Pirsch>`__
 - `sugizo <https://github.com/sugizo>`__
 - `valq7711 <https://github.com/valq7711>`__
 - `Kevin Keller <https://github.com/Kkeller83>`__
-- `Sam de Alfaro <sam@dealfaro.com>`__ (logo design)
+- Sam de Alfaro sam@dealfaro.com (logo design)
```

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 2990688 bytes, number of entries: 378
+Zip file size: 2990686 bytes, number of entries: 378
 -rw-r--r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
--rw-r--r--  3.0 unx    20588 tx defN 24-Apr-28 19:36 __init__.py
+-rw-r--r--  3.0 unx    20588 tx defN 24-May-27 23:35 __init__.py
 -rw-r--r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
 -rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
 -rw-r--r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
 -rw-r--r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
 -rw-r--r--  3.0 unx    12305 bx defN 23-May-08 00:39 static/images/alert-blue.gif
 -rw-r--r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
 -rw-r--r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
 -rw-r--r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
 -rw-r--r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
 -rw-r--r--  3.0 unx     5926 tx defN 23-May-08 00:39 static/css/future.css
 -rw-r--r--  3.0 unx      708 tx defN 23-May-08 00:39 static/css/gitlog.min.css
--rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
--rw-r--r--  3.0 unx     8104 tx defN 23-Nov-12 21:24 static/components/mtable.js
+-rw-r--r--  3.0 unx     7447 tx defN 24-May-27 23:55 static/components/mtable.html
+-rw-r--r--  3.0 unx     8097 tx defN 24-May-28 00:04 static/components/mtable.js
 -rw-r--r--  3.0 unx    10486 tx defN 23-Dec-28 07:17 static/js/index.js
 -rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
 -rw-r--r--  3.0 unx     7189 tx defN 23-May-08 00:39 static/js/ace/mode-sh.js
 -rw-r--r--  3.0 unx     3874 tx defN 23-May-08 00:39 static/js/ace/mode-latex.js
 -rw-r--r--  3.0 unx    55541 tx defN 23-May-08 00:39 static/js/ace/worker-xml.js
 -rw-r--r--  3.0 unx    16415 tx defN 23-May-08 00:39 static/js/ace/mode-sqlserver.js
 -rw-r--r--  3.0 unx    54512 tx defN 23-May-08 00:39 static/js/ace/mode-objectivec.js
@@ -373,8 +373,8 @@
 -rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
 -rw-r--r--  3.0 unx    88145 tx defN 23-Nov-12 21:44 static/js/jquery.min.js
 -rw-r--r--  3.0 unx      951 tx defN 23-Nov-12 21:32 templates/dbadmin.html
 -rw-r--r--  3.0 unx     4760 tx defN 23-Nov-12 21:32 templates/gitlog.html
 -rw-r--r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
 -rw-r--r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
 -rw-r--r--  3.0 unx     2953 tx defN 23-Nov-12 21:32 templates/translations.html
-378 files, 8005852 bytes uncompressed, 2919902 bytes compressed:  63.5%
+378 files, 8005845 bytes uncompressed, 2919900 bytes compressed:  63.5%
```

#### static/components/mtable.js

##### js-beautify {}

```diff
@@ -162,36 +162,38 @@
                     alert("Invalid field value: " + field.name);
                     break;
                 }
             }
         }
         if (item.id) {
             url += '/' + item.id;
-            Q.put(url, item).then(mtable.handle_response('put', this),
+            var data = JSON.parse(JSON.stringify(item));
+            delete data["id"];
+            Q.put(url, data).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
             Q.post(url, item).then(mtable.handle_response('post', this),
                 mtable.handle_response('post', this));
         }
-        location.reload();
     };
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
-            if (res.response) res = res.response; // deal with error weirdness
+            res = res.json();
             if (method == 'post') {
                 data.table.items = [];
                 mtable.methods.load.call(data);
             }
-            if (res.data.status == 'success') {
+            if (res.status == 'success') {
                 data.clear();
+                location.reload();
             } else {
-                data.errors = res.data.errors;
-                data.message = res.data.message;
+                data.errors = res.errors;
+                data.message = res.message;
             }
         };
     };
 
     mtable.methods.close = function() {
         this.clear();
     };
```

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app._default.zip`

 * *Files 8% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    187155 (000000000002DB13h)
-  Actual end-cent-dir record offset:        187133 (000000000002DAFDh)
-  Expected end-cent-dir record offset:      187133 (000000000002DAFDh)
+  Zip archive file size:                    199954 (0000000000030D12h)
+  Actual end-cent-dir record offset:        199932 (0000000000030CFCh)
+  Expected end-cent-dir record offset:      199932 (0000000000030CFCh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 4 entries.
-  The central directory is 351 (000000000000015Fh) bytes long,
+  central directory contains 6 entries.
+  The central directory is 526 (000000000000020Eh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 186782 (000000000002D99Eh).
+  is 199406 (0000000000030AEEh).
 
 
 Central directory entry #1:
 ---------------------------
 
   __init__.py
 
@@ -26,20 +26,20 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 7 17:39:44
-  file last modified on (UT extra field modtime): 2023 May 8 00:39:43 local
-  file last modified on (UT extra field modtime): 2023 May 8 00:39:43 UTC
-  32-bit CRC value (hex):                         de02d24c
-  compressed size:                                101 bytes
-  uncompressed size:                              135 bytes
+  file last modified on (DOS date/time):          2024 May 28 21:39:26
+  file last modified on (UT extra field modtime): 2024 May 29 04:39:26 local
+  file last modified on (UT extra field modtime): 2024 May 29 04:39:26 UTC
+  32-bit CRC value (hex):                         8391dc8d
+  compressed size:                                179 bytes
+  uncompressed size:                              271 bytes
   length of filename:                             11 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -53,16 +53,16 @@
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
   static/favicon.ico
 
-  offset of local header from start of archive:   170
-                                                  (00000000000000AAh) bytes
+  offset of local header from start of archive:   248
+                                                  (00000000000000F8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -90,16 +90,16 @@
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
   static/images/logo.png
 
-  offset of local header from start of archive:   4918
-                                                  (0000000000001336h) bytes
+  offset of local header from start of archive:   4996
+                                                  (0000000000001384h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -125,40 +125,114 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  templates/index.html
+  static/index.html
 
-  offset of local header from start of archive:   185803
-                                                  (000000000002D5CBh) bytes
+  offset of local header from start of archive:   185881
+                                                  (000000000002D619h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 7 17:39:44
-  file last modified on (UT extra field modtime): 2023 May 8 00:39:43 local
-  file last modified on (UT extra field modtime): 2023 May 8 00:39:43 UTC
-  32-bit CRC value (hex):                         242a0dc9
-  compressed size:                                901 bytes
-  uncompressed size:                              1811 bytes
+  file last modified on (DOS date/time):          2024 May 28 21:58:14
+  file last modified on (UT extra field modtime): 2024 May 29 04:58:14 local
+  file last modified on (UT extra field modtime): 2024 May 29 04:58:14 UTC
+  32-bit CRC value (hex):                         8f5ff323
+  compressed size:                                4505 bytes
+  uncompressed size:                              13879 bytes
+  length of filename:                             17 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #5:
+---------------------------
+
+  static/css/prism.css
+
+  offset of local header from start of archive:   190461
+                                                  (000000000002E7FDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 28 21:20:34
+  file last modified on (UT extra field modtime): 2024 May 29 04:20:34 local
+  file last modified on (UT extra field modtime): 2024 May 29 04:20:34 UTC
+  32-bit CRC value (hex):                         22a19de0
+  compressed size:                                683 bytes
+  uncompressed size:                              1490 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  static/js/prism.js
+
+  offset of local header from start of archive:   191222
+                                                  (000000000002EAF6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 28 21:20:20
+  file last modified on (UT extra field modtime): 2024 May 29 04:20:19 local
+  file last modified on (UT extra field modtime): 2024 May 29 04:20:19 UTC
+  32-bit CRC value (hex):                         26cc400b
+  compressed size:                                8108 bytes
+  uncompressed size:                              22341 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
```

#### zipnote {}

```diff
@@ -3,11 +3,17 @@
 
 Filename: static/favicon.ico
 Comment: 
 
 Filename: static/images/logo.png
 Comment: 
 
-Filename: templates/index.html
+Filename: static/index.html
+Comment: 
+
+Filename: static/css/prism.css
+Comment: 
+
+Filename: static/js/prism.js
 Comment: 
 
 Zip file comment:
```

#### __init__.py

```diff
@@ -1,7 +1,10 @@
-from py4web import action, __version__
-
+import os
+from py4web import action, Cache
+cache = Cache(size=1000)
 
 @action("index")
-@action.uses("index.html")
+@cache.memoize(expiration=1)
 def index():
-    return dict(version=__version__)
+    filename = os.path.join(os.path.dirname(__file__), "static", "index.html")
+    with open(filename) as stream:
+        return stream.read()
```

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21723 bytes, number of entries: 16
+Zip file size: 21891 bytes, number of entries: 16
 -rw-r--r--  3.0 unx     1394 tx defN 24-Apr-28 19:36 controllers.py
 -rw-r--r--  3.0 unx      852 tx defN 23-May-08 00:39 tasks.py
 -rw-r--r--  3.0 unx      254 tx defN 23-May-08 00:39 models.py
--rw-r--r--  3.0 unx     8029 tx defN 23-Aug-06 13:41 common.py
+-rw-r--r--  3.0 unx     8168 tx defN 24-May-16 06:31 common.py
 -rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 __init__.py
--rw-r--r--  3.0 unx     3212 tx defN 23-Aug-06 13:41 settings.py
+-rw-r--r--  3.0 unx     3403 tx defN 24-May-27 07:35 settings.py
 -rw-r--r--  3.0 unx       97 tx defN 23-May-08 00:39 translations/it.json
 -rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
 -rw-r--r--  3.0 unx    11431 tx defN 23-May-08 00:39 static/css/no.css
 -rw-r--r--  3.0 unx    12182 tx defN 23-Nov-12 21:26 static/js/utils.js
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
 -rw-r--r--  3.0 unx      103 tx defN 23-May-08 00:39 templates/index.html
 -rw-r--r--  3.0 unx     2738 tx defN 24-Apr-28 19:36 templates/layout.html
 -rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 templates/generic.html
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 templates/README.md
 -rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
-16 files, 73249 bytes uncompressed, 19149 bytes compressed:  73.9%
+16 files, 73579 bytes uncompressed, 19317 bytes compressed:  73.7%
```

#### common.py

```diff
@@ -48,31 +48,34 @@
 T = Translator(settings.T_FOLDER)
 
 # #######################################################
 # pick the session type that suits you best
 # #######################################################
 if settings.SESSION_TYPE == "cookies":
     session = Session(secret=settings.SESSION_SECRET_KEY)
+
 elif settings.SESSION_TYPE == "redis":
     import redis
 
     host, port = settings.REDIS_SERVER.split(":")
     # for more options: https://github.com/andymccurdy/redis-py/blob/master/redis/client.py
     conn = redis.Redis(host=host, port=int(port))
     conn.set = (
         lambda k, v, e, cs=conn.set, ct=conn.ttl: cs(k, v, ct(k))
         if ct(k) >= 0
         else cs(k, v, e)
     )
     session = Session(secret=settings.SESSION_SECRET_KEY, storage=conn)
+
 elif settings.SESSION_TYPE == "memcache":
     import memcache, time
 
     conn = memcache.Client(settings.MEMCACHE_CLIENTS, debug=0)
     session = Session(secret=settings.SESSION_SECRET_KEY, storage=conn)
+
 elif settings.SESSION_TYPE == "database":
     from py4web.utils.dbstore import DBStore
 
     session = Session(secret=settings.SESSION_SECRET_KEY, storage=DBStore(db))
 
 # #######################################################
 # Instantiate the object and actions that handle auth
@@ -80,15 +83,15 @@
 auth = Auth(session, db, define_tables=False)
 auth.use_username = True
 auth.param.registration_requires_confirmation = settings.VERIFY_EMAIL
 auth.param.registration_requires_approval = settings.REQUIRES_APPROVAL
 auth.param.login_after_registration = settings.LOGIN_AFTER_REGISTRATION
 auth.param.allowed_actions = settings.ALLOWED_ACTIONS
 auth.param.login_expiration_time = 3600
-auth.param.password_complexity = {"entropy": 50}
+auth.param.password_complexity = {"entropy": settings.PASSWORD_ENTROPY}
 auth.param.block_previous_password_num = 3
 auth.param.default_login_enabled = settings.DEFAULT_LOGIN_ENABLED
 auth.define_tables()
 auth.fix_actions()
 
 flash = auth.flash
 
@@ -201,18 +204,19 @@
 
     # to use "from .common import scheduler" and then use it according
     # to celery docs, examples in tasks.py
     scheduler = Celery(
         "apps.%s.tasks" % settings.APP_NAME, broker=settings.CELERY_BROKER
     )
 
-
 # #######################################################
 # Enable authentication
 # #######################################################
 auth.enable(uses=(session, T, db), env=dict(T=T))
 
 # #######################################################
 # Define convenience decorators
+# They can be used instead of @action and @action.uses
+# They should NEVER BE MIXED with @action and @action.uses
 # #######################################################
 unauthenticated = ActionFactory(db, session, T, flash, auth)
 authenticated = ActionFactory(db, session, T, flash, auth.user)
```

#### settings.py

```diff
@@ -4,33 +4,40 @@
 - session settings
 - i18n settings
 This file is provided as an example:
 """
 import os
 from py4web.core import required_folder
 
+# mode (default or development)
+MODE = os.environ.get("PY4WEB_MODE")
+
 # db settings
 APP_FOLDER = os.path.dirname(__file__)
 APP_NAME = os.path.split(APP_FOLDER)[-1]
+
 # DB_FOLDER:    Sets the place where migration files will be created
 #               and is the store location for SQLite databases
 DB_FOLDER = required_folder(APP_FOLDER, "databases")
 DB_URI = "sqlite://storage.db"
 DB_POOL_SIZE = 1
 DB_MIGRATE = True
-DB_FAKE_MIGRATE = False  # maybe?
+DB_FAKE_MIGRATE = False
 
 # location where static files are stored:
 STATIC_FOLDER = required_folder(APP_FOLDER, "static")
 
 # location where to store uploaded files:
 UPLOAD_FOLDER = required_folder(APP_FOLDER, "uploads")
 
 # send verification email on registration
-VERIFY_EMAIL = True
+VERIFY_EMAIL = MODE != "development"
+
+# complexity of the password 0: no constraints, 50: safe!
+PASSWORD_ENTROPY = 0 if MODE == "development" else 50
 
 # account requires to be approved ?
 REQUIRES_APPROVAL = False
 
 # auto login after registration
 # requires False VERIFY_EMAIL & REQUIRES_APPROVAL
 LOGIN_AFTER_REGISTRATION = False
```

### Comparing `py4web-1.20240509.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240528.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1392764 bytes, number of entries: 143
+Zip file size: 1394058 bytes, number of entries: 143
 -rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
--rw-r--r--  3.0 unx     4206 tx defN 24-May-09 05:43 __init__.py
+-rw-r--r--  3.0 unx     4221 tx defN 24-May-28 00:48 __init__.py
 -rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
 -rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
 -rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
 -rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
 -rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
 -rw-r--r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
 -rw-r--r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
@@ -59,16 +59,16 @@
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/socketio/README.md
 -rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
 -rw-r--r--  3.0 unx     9998 tx defN 23-May-08 00:39 static/error.html
 -rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/ws/README.md
 -rw-r--r--  3.0 unx  7330359 tx defN 23-May-08 00:39 static/data/uscities.json
 -rw-r--r--  3.0 unx   295408 tx defN 23-May-08 00:39 static/data/zip_codes.json
 -rw-r--r--  3.0 unx      977 tx defN 23-May-08 00:39 static/firebase-push.html
--rw-r--r--  3.0 unx    11417 tx defN 23-May-08 00:39 static/css/no.css
--rw-r--r--  3.0 unx     1903 tx defN 23-May-08 00:39 static/css/prism.css
+-rw-r--r--  3.0 unx    11421 tx defN 24-May-28 02:14 static/css/no.css
+-rw-r--r--  3.0 unx     1490 tx defN 24-May-28 03:45 static/css/prism.css
 -rw-r--r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components/fileupload/fileupload.css
 -rw-r--r--  3.0 unx     1232 tx defN 23-Nov-12 21:35 static/components/fileupload/fileupload.js
 -rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.html
 -rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components/starrater/starrater.css
 -rw-r--r--  3.0 unx     1681 tx defN 23-Nov-12 21:35 static/components/starrater/starrater.js
 -rw-r--r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components/starrater/starrater.html
 -rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
@@ -76,17 +76,17 @@
 -rw-r--r--  3.0 unx     5384 tx defN 23-Nov-12 21:35 static/components/grid/grid.js
 -rw-r--r--  3.0 unx     3299 tx defN 23-May-08 00:39 static/components/grid/grid.html
 -rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components/vueform/vueform.css
 -rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components/vueform/luxon.js
 -rw-r--r--  3.0 unx     7263 tx defN 23-Nov-12 21:35 static/components/vueform/vueform.js
 -rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components/vueform/luxon.min.js
 -rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components/vueform/vueform.html
--rw-r--r--  3.0 unx     8097 tx defN 23-Nov-12 21:35 static/components/mtable.js
+-rw-r--r--  3.0 unx     8097 tx defN 24-May-28 00:05 static/components/mtable.js
 -rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
--rw-r--r--  3.0 unx    19055 tx defN 23-May-08 00:39 static/js/prism.js
+-rw-r--r--  3.0 unx    22341 tx defN 24-May-28 03:44 static/js/prism.js
 -rw-r--r--  3.0 unx      868 tx defN 23-May-08 00:39 static/js/firebase-push.js
 -rw-r--r--  3.0 unx     8311 tx defN 23-May-08 00:39 static/js/utils.min.js
 -rw-r--r--  3.0 unx    11888 tx defN 23-Nov-12 21:35 static/js/utils.js
 -rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
 -rw-r--r--  3.0 unx    32337 tx defN 23-Nov-12 21:45 static/js/axios.min.js
 -rw-r--r--  3.0 unx   342147 tx defN 23-Dec-11 08:15 static/js/vue.js
 -rw-r--r--  3.0 unx      496 tx defN 23-May-08 00:39 static/js/star_rater_vue.js
@@ -102,31 +102,31 @@
 -rw-r--r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.js
 -rw-r--r--  3.0 unx     3369 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.html
 -rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components-bulma/vueform/vueform.css
 -rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.js
 -rw-r--r--  3.0 unx     7257 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.js
 -rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.min.js
 -rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.html
--rw-r--r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components-bulma/mtable.js
+-rw-r--r--  3.0 unx     8097 tx defN 24-May-28 00:05 static/components-bulma/mtable.js
 -rw-r--r--  3.0 unx       12 tx stor 23-May-08 00:39 static/hello.txt
 -rw-r--r--  3.0 unx     1913 tx defN 23-May-08 00:39 templates/socketio/socketio_index.html
 -rw-r--r--  3.0 unx     2156 tx defN 23-May-08 00:39 templates/layout_bulma.html
 -rw-r--r--  3.0 unx      488 tx defN 23-May-08 00:39 templates/vue/insert_form.html
 -rw-r--r--  3.0 unx      392 tx defN 23-May-08 00:39 templates/vue/vuegrid_bulma.html
 -rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 templates/vue/file_uploader.html
 -rw-r--r--  3.0 unx      544 tx defN 23-May-08 00:39 templates/vue/star_rater_vue_bulma.html
 -rw-r--r--  3.0 unx      502 tx defN 23-May-08 00:39 templates/vue/star_rater_vue.html
 -rw-r--r--  3.0 unx      374 tx defN 23-May-08 00:39 templates/vue/vuegrid.html
 -rw-r--r--  3.0 unx      448 tx defN 23-May-08 00:39 templates/vue/starrating.html
 -rw-r--r--  3.0 unx      683 tx defN 23-May-08 00:39 templates/vue/vue_grid_and_forms.html
 -rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/edit_form.html
 -rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/view_form.html
 -rw-r--r--  3.0 unx     2172 tx defN 23-May-08 00:39 templates/ws/ws_index.html
--rw-r--r--  3.0 unx     6788 tx defN 23-May-08 00:39 templates/index.html
--rw-r--r--  3.0 unx      430 tx defN 23-Aug-06 14:14 templates/show.html
+-rw-r--r--  3.0 unx     7368 tx defN 24-May-28 04:20 templates/index.html
+-rw-r--r--  3.0 unx      446 tx defN 24-May-28 00:47 templates/show.html
 -rw-r--r--  3.0 unx       26 tx stor 23-May-08 00:39 templates/examples/flash_example_next.html
 -rw-r--r--  3.0 unx      551 tx defN 23-May-08 00:39 templates/examples/auth_custom_login.html
 -rw-r--r--  3.0 unx      189 tx defN 23-May-08 00:39 templates/examples/hcaptcha_form.html
 -rw-r--r--  3.0 unx     1025 tx defN 23-May-08 00:39 templates/examples/rest_info.html
 -rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/flash_example.html
 -rw-r--r--  3.0 unx       69 tx defN 23-May-08 00:39 templates/examples/ajax_grid.html
 -rw-r--r--  3.0 unx      263 tx defN 23-May-08 00:39 templates/examples/session_counter.html
@@ -138,8 +138,8 @@
 -rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
 -rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
 -rw-r--r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
 -rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
 -rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
-143 files, 9348899 bytes uncompressed, 1365608 bytes compressed:  85.4%
+143 files, 9352387 bytes uncompressed, 1366902 bytes compressed:  85.4%
```

#### __init__.py

```diff
@@ -90,9 +90,9 @@
             continue
         filename = other[1:].replace(".", "/") + ".py"
         with open(f"apps/showcase/{filename}") as stream:
             content = stream.read().strip()
             data.append({"shortname": filename, "content": content, "language": "python"})
     # drop the subfolder name
     path = "/".join(path.split("/")[1:])
-    executable = MODE == "full" or name in globals()
+    executable = MODE == "full" or name.split("/")[-1] in globals()
     return {"files": data, "mode": MODE, "path": path, "executable": executable}
```

#### static/css/no.css

```diff
@@ -111,15 +111,15 @@
   display:block;
   width:100%;
 }
 
 code {
   background: #f4f5f6;
   border-radius: .4rem;
-  font-size: 90;
+  font-size: 0.8em;
   margin: 0 .2rem;
   padding: .2rem .5rem;
   white-space: nowrap;
 }
 
 p,li,button,fieldset,input,select,textarea,blockquote,table {
   margin-bottom: 1.0rem;
@@ -536,8 +536,8 @@
   cursor: pointer;
   opacity: 0.2;
   text-transform: capitalize;
 }
 
 ul.tags-list li[data-selected=true] {
   opacity: 1.0;
-}
+}
```

#### static/css/prism.css

```diff
@@ -1,3 +1,3 @@
-/* PrismJS 1.28.0
-https://prismjs.com/download.html#themes=prism&languages=markup+css+clike+javascript+python */
-code[class*=language-],pre[class*=language-]{color:#000;background:0 0;text-shadow:0 1px #fff;font-family:Consolas,Monaco,'Andale Mono','Ubuntu Mono',monospace;font-size:1em;text-align:left;white-space:pre;word-spacing:normal;word-break:normal;word-wrap:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-hyphens:none;-moz-hyphens:none;-ms-hyphens:none;hyphens:none}code[class*=language-] ::-moz-selection,code[class*=language-]::-moz-selection,pre[class*=language-] ::-moz-selection,pre[class*=language-]::-moz-selection{text-shadow:none;background:#b3d4fc}code[class*=language-] ::selection,code[class*=language-]::selection,pre[class*=language-] ::selection,pre[class*=language-]::selection{text-shadow:none;background:#b3d4fc}@media print{code[class*=language-],pre[class*=language-]{text-shadow:none}}pre[class*=language-]{padding:1em;margin:.5em 0;overflow:auto}:not(pre)>code[class*=language-],pre[class*=language-]{background:#f5f2f0}:not(pre)>code[class*=language-]{padding:.1em;border-radius:.3em;white-space:normal}.token.cdata,.token.comment,.token.doctype,.token.prolog{color:#708090}.token.punctuation{color:#999}.token.namespace{opacity:.7}.token.boolean,.token.constant,.token.deleted,.token.number,.token.property,.token.symbol,.token.tag{color:#905}.token.attr-name,.token.builtin,.token.char,.token.inserted,.token.selector,.token.string{color:#690}.language-css .token.string,.style .token.string,.token.entity,.token.operator,.token.url{color:#9a6e3a;background:hsla(0,0%,100%,.5)}.token.atrule,.token.attr-value,.token.keyword{color:#07a}.token.class-name,.token.function{color:#dd4a68}.token.important,.token.regex,.token.variable{color:#e90}.token.bold,.token.important{font-weight:700}.token.italic{font-style:italic}.token.entity{cursor:help}
+/* PrismJS 1.29.0
+https://prismjs.com/download.html#themes=prism-tomorrow&languages=markup+css+clike+javascript+python&plugins=remove-initial-line-feed+normalize-whitespace */
+code[class*=language-],pre[class*=language-]{color:#ccc;background:0 0;font-family:Consolas,Monaco,'Andale Mono','Ubuntu Mono',monospace;font-size:1em;text-align:left;white-space:pre;word-spacing:normal;word-break:normal;word-wrap:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-hyphens:none;-moz-hyphens:none;-ms-hyphens:none;hyphens:none}pre[class*=language-]{padding:1em;margin:.5em 0;overflow:auto}:not(pre)>code[class*=language-],pre[class*=language-]{background:#2d2d2d}:not(pre)>code[class*=language-]{padding:.1em;border-radius:.3em;white-space:normal}.token.block-comment,.token.cdata,.token.comment,.token.doctype,.token.prolog{color:#999}.token.punctuation{color:#ccc}.token.attr-name,.token.deleted,.token.namespace,.token.tag{color:#e2777a}.token.function-name{color:#6196cc}.token.boolean,.token.function,.token.number{color:#f08d49}.token.class-name,.token.constant,.token.property,.token.symbol{color:#f8c555}.token.atrule,.token.builtin,.token.important,.token.keyword,.token.selector{color:#cc99cd}.token.attr-value,.token.char,.token.regex,.token.string,.token.variable{color:#7ec699}.token.entity,.token.operator,.token.url{color:#67cdcc}.token.bold,.token.important{font-weight:700}.token.italic{font-style:italic}.token.entity{cursor:help}.token.inserted{color:green}
```

#### static/components/mtable.js

##### js-beautify {}

```diff
@@ -62,18 +62,18 @@
             return ((negate ? 'not.' : '') +
                 parts[0].replace(/ /ig, '') +
                 '=' + parts[parts.length - 1].replace(/^ /, ''));
         });
         if (filters.length) url += '&' + filters.join('&');
         if (self.order) url += '&@order=' + self.order;
         self.busy = true;
-        axios.get(url).then(function(res) {
+        Q.get(url).then(function(res) {
             self.busy = false;
-            if (!length) self.table = res.data;
-            else self.table.items = self.table.items.concat(res.data.items);
+            if (!length) self.table = res.json();
+            else self.table.items = self.table.items.concat(res.json().items);
         });
     };
 
     mtable.methods.reorder = function(field) {
         if (this.order == '~' + field.name) this.order = null;
         else if (this.order == field.name) this.order = '~' + field.name;
         else this.order = field.name;
@@ -110,16 +110,16 @@
             } else if (field.type == "reference") {
                 if (!(field.references in this.reference_options)) {
                     Vue.set(this.reference_options, field.references, []);
                     let reference_table_url = self.url.split('/');
                     reference_table_url.pop()
                     reference_table_url.push(field.references)
                     reference_table_url = reference_table_url.join('/') + '?@options_list=true';
-                    axios.get(reference_table_url).then(function(res) {
-                        let url_components = res.config.url.split('?')[0].split('/');
+                    Q.get(reference_table_url).then(function(res) {
+                        let url_components = res.json().config.url.split('?')[0].split('/');
                         self.reference_options[url_components[url_components.length - 1]] = res.data.items;
                     });
 
                 }
             }
         }
         this.$nextTick(function() {
@@ -141,15 +141,15 @@
 
     mtable.methods.trash = function(item) {
         if (window.confirm("Really delete record?")) {
             let url = this.url + '/' + item.id;
             this.table.items = this.table.items.filter((i) => {
                 return i.id != item.id;
             });
-            axios.delete(url);
+            Q.delete(url);
             if (item == this.item) this.item = null;
         }
     };
 
     mtable.methods.save = function(item) {
         let url = this.url;
         self.busy = true;
@@ -162,35 +162,38 @@
                     alert("Invalid field value: " + field.name);
                     break;
                 }
             }
         }
         if (item.id) {
             url += '/' + item.id;
-            axios.put(url, item).then(mtable.handle_response('put', this),
+            var data = JSON.parse(JSON.stringify(item));
+            delete data["id"];
+            Q.put(url, data).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
-            axios.post(url, item).then(mtable.handle_response('post', this),
+            Q.post(url, item).then(mtable.handle_response('post', this),
                 mtable.handle_response('post', this));
         }
     };
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
-            if (res.response) res = res.response; // deal with error weirdness
+            res = res.json();
             if (method == 'post') {
                 data.table.items = [];
                 mtable.methods.load.call(data);
             }
-            if (res.data.status == 'success') {
+            if (res.status == 'success') {
                 data.clear();
+                location.reload();
             } else {
-                data.errors = res.data.errors;
-                data.message = res.data.message;
+                data.errors = res.errors;
+                data.message = res.message;
             }
         };
     };
 
     mtable.methods.close = function() {
         this.clear();
     };
```

#### static/js/prism.js

##### js-beautify {}

```diff
@@ -1,9 +1,9 @@
-/* PrismJS 1.28.0
-https://prismjs.com/download.html#themes=prism&languages=markup+css+clike+javascript+python */
+/* PrismJS 1.29.0
+https://prismjs.com/download.html#themes=prism-tomorrow&languages=markup+css+clike+javascript+python&plugins=remove-initial-line-feed+normalize-whitespace */
 var _self = "undefined" != typeof window ? window : "undefined" != typeof WorkerGlobalScope && self instanceof WorkerGlobalScope ? self : {},
     Prism = function(e) {
         var n = /(?:^|\s)lang(?:uage)?-([\w-]+)(?=\s|$)/i,
             t = 0,
             r = {},
             a = {
                 manual: e.Prism && e.Prism.manual,
@@ -677,8 +677,123 @@
     },
     keyword: /\b(?:_(?=\s*:)|and|as|assert|async|await|break|case|class|continue|def|del|elif|else|except|exec|finally|for|from|global|if|import|in|is|lambda|match|nonlocal|not|or|pass|print|raise|return|try|while|with|yield)\b/,
     builtin: /\b(?:__import__|abs|all|any|apply|ascii|basestring|bin|bool|buffer|bytearray|bytes|callable|chr|classmethod|cmp|coerce|compile|complex|delattr|dict|dir|divmod|enumerate|eval|execfile|file|filter|float|format|frozenset|getattr|globals|hasattr|hash|help|hex|id|input|int|intern|isinstance|issubclass|iter|len|list|locals|long|map|max|memoryview|min|next|object|oct|open|ord|pow|property|range|raw_input|reduce|reload|repr|reversed|round|set|setattr|slice|sorted|staticmethod|str|sum|super|tuple|type|unichr|unicode|vars|xrange|zip)\b/,
     boolean: /\b(?:False|None|True)\b/,
     number: /\b0(?:b(?:_?[01])+|o(?:_?[0-7])+|x(?:_?[a-f0-9])+)\b|(?:\b\d+(?:_\d+)*(?:\.(?:\d+(?:_\d+)*)?)?|\B\.\d+(?:_\d+)*)(?:e[+-]?\d+(?:_\d+)*)?j?(?!\w)/i,
     operator: /[-+%=]=?|!=|:=|\*\*?=?|\/\/?=?|<[<=>]?|>[=>]?|[&|^~]/,
     punctuation: /[{}[\];(),.:]/
-}, Prism.languages.python["string-interpolation"].inside.interpolation.inside.rest = Prism.languages.python, Prism.languages.py = Prism.languages.python;
+}, Prism.languages.python["string-interpolation"].inside.interpolation.inside.rest = Prism.languages.python, Prism.languages.py = Prism.languages.python;
+"undefined" != typeof Prism && "undefined" != typeof document && Prism.hooks.add("before-sanity-check", (function(e) {
+    if (e.code) {
+        var n = e.element.parentNode,
+            o = /(?:^|\s)keep-initial-line-feed(?:\s|$)/;
+        !n || "pre" !== n.nodeName.toLowerCase() || o.test(n.className) || o.test(e.element.className) || (e.code = e.code.replace(/^(?:\r?\n|\r)/, ""))
+    }
+}));
+! function() {
+    if ("undefined" != typeof Prism) {
+        var e = Object.assign || function(e, t) {
+                for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n]);
+                return e
+            },
+            t = {
+                "remove-trailing": "boolean",
+                "remove-indent": "boolean",
+                "left-trim": "boolean",
+                "right-trim": "boolean",
+                "break-lines": "number",
+                indent: "number",
+                "remove-initial-line-feed": "boolean",
+                "tabs-to-spaces": "number",
+                "spaces-to-tabs": "number"
+            };
+        n.prototype = {
+            setDefaults: function(t) {
+                this.defaults = e(this.defaults, t)
+            },
+            normalize: function(t, n) {
+                for (var r in n = e(this.defaults, n)) {
+                    var i = r.replace(/-(\w)/g, (function(e, t) {
+                        return t.toUpperCase()
+                    }));
+                    "normalize" !== r && "setDefaults" !== i && n[r] && this[i] && (t = this[i].call(this, t, n[r]))
+                }
+                return t
+            },
+            leftTrim: function(e) {
+                return e.replace(/^\s+/, "")
+            },
+            rightTrim: function(e) {
+                return e.replace(/\s+$/, "")
+            },
+            tabsToSpaces: function(e, t) {
+                return t = 0 | t || 4, e.replace(/\t/g, new Array(++t).join(" "))
+            },
+            spacesToTabs: function(e, t) {
+                return t = 0 | t || 4, e.replace(RegExp(" {" + t + "}", "g"), "\t")
+            },
+            removeTrailing: function(e) {
+                return e.replace(/\s*?$/gm, "")
+            },
+            removeInitialLineFeed: function(e) {
+                return e.replace(/^(?:\r?\n|\r)/, "")
+            },
+            removeIndent: function(e) {
+                var t = e.match(/^[^\S\n\r]*(?=\S)/gm);
+                return t && t[0].length ? (t.sort((function(e, t) {
+                    return e.length - t.length
+                })), t[0].length ? e.replace(RegExp("^" + t[0], "gm"), "") : e) : e
+            },
+            indent: function(e, t) {
+                return e.replace(/^[^\S\n\r]*(?=\S)/gm, new Array(++t).join("\t") + "$&")
+            },
+            breakLines: function(e, t) {
+                t = !0 === t ? 80 : 0 | t || 80;
+                for (var n = e.split("\n"), i = 0; i < n.length; ++i)
+                    if (!(r(n[i]) <= t)) {
+                        for (var o = n[i].split(/(\s+)/g), a = 0, l = 0; l < o.length; ++l) {
+                            var s = r(o[l]);
+                            (a += s) > t && (o[l] = "\n" + o[l], a = s)
+                        }
+                        n[i] = o.join("")
+                    } return n.join("\n")
+            }
+        }, "undefined" != typeof module && module.exports && (module.exports = n), Prism.plugins.NormalizeWhitespace = new n({
+            "remove-trailing": !0,
+            "remove-indent": !0,
+            "left-trim": !0,
+            "right-trim": !0
+        }), Prism.hooks.add("before-sanity-check", (function(e) {
+            var n = Prism.plugins.NormalizeWhitespace;
+            if ((!e.settings || !1 !== e.settings["whitespace-normalization"]) && Prism.util.isActive(e.element, "whitespace-normalization", !0))
+                if (e.element && e.element.parentNode || !e.code) {
+                    var r = e.element.parentNode;
+                    if (e.code && r && "pre" === r.nodeName.toLowerCase()) {
+                        for (var i in null == e.settings && (e.settings = {}), t)
+                            if (Object.hasOwnProperty.call(t, i)) {
+                                var o = t[i];
+                                if (r.hasAttribute("data-" + i)) try {
+                                    var a = JSON.parse(r.getAttribute("data-" + i) || "true");
+                                    typeof a === o && (e.settings[i] = a)
+                                } catch (e) {}
+                            } for (var l = r.childNodes, s = "", c = "", u = !1, m = 0; m < l.length; ++m) {
+                            var f = l[m];
+                            f == e.element ? u = !0 : "#text" === f.nodeName && (u ? c += f.nodeValue : s += f.nodeValue, r.removeChild(f), --m)
+                        }
+                        if (e.element.children.length && Prism.plugins.KeepMarkup) {
+                            var d = s + e.element.innerHTML + c;
+                            e.element.innerHTML = n.normalize(d, e.settings), e.code = e.element.textContent
+                        } else e.code = s + e.code + c, e.code = n.normalize(e.code, e.settings)
+                    }
+                } else e.code = n.normalize(e.code, e.settings)
+        }))
+    }
+
+    function n(t) {
+        this.defaults = e({}, t)
+    }
+
+    function r(e) {
+        for (var t = 0, n = 0; n < e.length; ++n) e.charCodeAt(n) == "\t".charCodeAt(0) && (t += 3);
+        return e.length + t
+    }
+}();
```

#### static/components-bulma/mtable.js

##### js-beautify {}

```diff
@@ -62,18 +62,18 @@
             return ((negate ? 'not.' : '') +
                 parts[0].replace(/ /ig, '') +
                 '=' + parts[parts.length - 1].replace(/^ /, ''));
         });
         if (filters.length) url += '&' + filters.join('&');
         if (self.order) url += '&@order=' + self.order;
         self.busy = true;
-        axios.get(url).then(function(res) {
+        Q.get(url).then(function(res) {
             self.busy = false;
-            if (!length) self.table = res.data;
-            else self.table.items = self.table.items.concat(res.data.items);
+            if (!length) self.table = res.json();
+            else self.table.items = self.table.items.concat(res.json().items);
         });
     };
 
     mtable.methods.reorder = function(field) {
         if (this.order == '~' + field.name) this.order = null;
         else if (this.order == field.name) this.order = '~' + field.name;
         else this.order = field.name;
@@ -110,16 +110,16 @@
             } else if (field.type == "reference") {
                 if (!(field.references in this.reference_options)) {
                     Vue.set(this.reference_options, field.references, []);
                     let reference_table_url = self.url.split('/');
                     reference_table_url.pop()
                     reference_table_url.push(field.references)
                     reference_table_url = reference_table_url.join('/') + '?@options_list=true';
-                    axios.get(reference_table_url).then(function(res) {
-                        let url_components = res.config.url.split('?')[0].split('/');
+                    Q.get(reference_table_url).then(function(res) {
+                        let url_components = res.json().config.url.split('?')[0].split('/');
                         self.reference_options[url_components[url_components.length - 1]] = res.data.items;
                     });
 
                 }
             }
         }
         this.$nextTick(function() {
@@ -141,15 +141,15 @@
 
     mtable.methods.trash = function(item) {
         if (window.confirm("Really delete record?")) {
             let url = this.url + '/' + item.id;
             this.table.items = this.table.items.filter((i) => {
                 return i.id != item.id;
             });
-            axios.delete(url);
+            Q.delete(url);
             if (item == this.item) this.item = null;
         }
     };
 
     mtable.methods.save = function(item) {
         let url = this.url;
         self.busy = true;
@@ -162,35 +162,38 @@
                     alert("Invalid field value: " + field.name);
                     break;
                 }
             }
         }
         if (item.id) {
             url += '/' + item.id;
-            axios.put(url, item).then(mtable.handle_response('put', this),
+            var data = JSON.parse(JSON.stringify(item));
+            delete data["id"];
+            Q.put(url, data).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
-            axios.post(url, item).then(mtable.handle_response('post', this),
+            Q.post(url, item).then(mtable.handle_response('post', this),
                 mtable.handle_response('post', this));
         }
     };
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
-            if (res.response) res = res.response; // deal with error weirdness
+            res = res.json();
             if (method == 'post') {
                 data.table.items = [];
                 mtable.methods.load.call(data);
             }
-            if (res.data.status == 'success') {
+            if (res.status == 'success') {
                 data.clear();
+                location.reload();
             } else {
-                data.errors = res.data.errors;
-                data.message = res.data.message;
+                data.errors = res.errors;
+                data.message = res.message;
             }
         };
     };
 
     mtable.methods.close = function() {
         this.clear();
     };
```

#### templates/index.html

```diff
@@ -1,12 +1,26 @@
 [[extend 'layout.html']]
 
+
+
 <div id="vue">
+
   <table class="table">
     <tr style="background:#e1e1e1">
+      <th colspan="2" class="is-info">Complete Example Apps</th>      
+    </tr>
+    <tr>
+      <td colspan="2">
+	<a href="https://github.com/web2py/py4web/tree/master/apps/todo">Start with a Todo app</a><br/>    
+	<a href="https://github.com/web2py/py4web/tree/master/apps/fadebook">A minimalist Facebook clone</a><br/>
+	<a href="https://github.com/web2py/py4web/tree/master/apps/tagged_posts">A minimalist Twitter clone</a><br/>
+	<a href="https://github.com/ali96343/facep4w">More third party contributed apps...</a>
+      </td>
+    </tr>
+    <tr style="background:#e1e1e1">
       <th colspan="2" class="is-info">Simple Serverside Examples</th>      
     </tr>
     <tr>
       <td>A normal page without template</td>
       <td><a role="button" href="[[=URL('show/examples/page_without_template')]]">example</a></td>
     </tr>
     <tr>
```

##### html2text {}

```diff
@@ -1,8 +1,13 @@
 [[extend 'layout.html']]
+CCoommpplleettee EExxaammppllee AAppppss
+_S_t_a_r_t_ _w_i_t_h_ _a_ _T_o_d_o_ _a_p_p
+_A_ _m_i_n_i_m_a_l_i_s_t_ _F_a_c_e_b_o_o_k_ _c_l_o_n_e
+_A_ _m_i_n_i_m_a_l_i_s_t_ _T_w_i_t_t_e_r_ _c_l_o_n_e
+_M_o_r_e_ _t_h_i_r_d_ _p_a_r_t_y_ _c_o_n_t_r_i_b_u_t_e_d_ _a_p_p_s_._._.
 SSiimmppllee SSeerrvveerrssiiddee EExxaammpplleess
 A normal page without template                                        _e_x_a_m_p_l_e
 A normal page with template                                           _e_x_a_m_p_l_e
 A page causing an internal error                                      _e_x_a_m_p_l_e
 Page which raises HTTP                                                _e_x_a_m_p_l_e
 Page with a redirect                                                  _e_x_a_m_p_l_e
 Page with parameters                                                  _e_x_a_m_p_l_e
```

#### templates/show.html

```diff
@@ -1,15 +1,15 @@
 [[extend 'layout.html']]
 <style>
   code {margin: 0; padding: 0}
 </style>
 
 <a role="button" href="../index">Back to Examples</a>
 [[if executable:]]
-<a role="button" href="../[[=path]]">Run Example</a>
+<a role="button" target="_blank" href="../[[=path]]">Run Example</a>
 [[else:]]
 Run this application locally to try examples
 [[pass]]
 
 [[for file in files:]]
 <div>
   <h3>[[=file['name'] ]]</h3>
```

### Comparing `py4web-1.20240509.1/py4web/core.py` & `py4web-1.20240528.1/py4web/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+# pylint: disable=too-many-lines,line-too-long,too-many-branches,use-dict-literal,too-many-arguments,too-few-public-methods,too-many-locals,broad-exception-caught,cell-var-from-loop
+
 """PY4WEB - a web framework for rapid development of efficient database driven web applications"""
 
 # Standard modules
 import asyncio
 import code
 import collections
 import copy
 import datetime
 import enum
 import functools
+import html as sanitize_html
 import http.client
 import http.cookies
 import importlib.machinery
 import importlib.util
 import inspect
 import io
 import json
@@ -30,39 +33,38 @@
 import traceback
 import types
 import urllib.parse
 import uuid
 import zipfile
 from collections import OrderedDict
 from contextlib import redirect_stderr, redirect_stdout
-import html as sanitize_html
 
 import portalocker
 from watchgod import awatch
 
-from . import server_adapters
-
 # Optional web servers for speed
 try:
     import gunicorn
 except ImportError:
     gunicorn = None
 
 import click
 
 # Third party modules
 import ombott as bottle
 import pluralize
 import pydal
+import pydal.validators
 import renoir
 import renoir.constants
 import renoir.writers
 import threadsafevariable
 import yatl
 
+from . import server_adapters
 from .utils.misc import secure_dumps, secure_loads
 
 bottle.DefaultConfig.max_memfile_size = 16 * 1024 * 1024
 bottle.DefaultConfig.app_name_header = "HTTP_X_PY4WEB_APPNAME"
 # apply DefaultConfig changes to default_app
 bottle.default_app().setup()
 
@@ -97,23 +99,19 @@
     PY4WEB_SERVICE_FOLDER=".service",
     PY4WEB_SERVICE_DB_URI="sqlite://service.storage",
 )
 
 HELPERS = {name: getattr(yatl.helpers, name) for name in yatl.helpers.__all__}
 
 ART = r"""
- /#######  /##     /##/##   /## /##      /## /######## /####### 
-| ##__  ##|  ##   /##/ ##  | ##| ##  /# | ##| ##_____/| ##__  ##
-| ##  \ ## \  ## /##/| ##  | ##| ## /###| ##| ##      | ##  \ ##
-| #######/  \  ####/ | ########| ##/## ## ##| #####   | ####### 
-| ##____/    \  ##/  |_____  ##| ####_  ####| ##__/   | ##__  ##
-| ##          | ##         | ##| ###/ \  ###| ##      | ##  \ ##
-| ##          | ##         | ##| ##/   \  ##| ########| #######/
-|__/          |__/         |__/|__/     \__/|________/|_______/
-Is still experimental...
+██████◣◥█◣  ◢█◤ ██   ██ ██      ██ ███████ ██████◣  
+██   ██ ◥█◣◢█◤  ██   ██ ██      ██ ██      ██   ██ 
+██████◤  ◥██◤   ███████ ██  ◢◣  ██ ██████  ██████  
+██        ██         ██ ◥█◣◢██◣◢█◤ ██      ██   ██ 
+██        ██         ██  ◥██◤◥██◤  ███████ ██████◤
 """
 
 Field = pydal.Field
 request = bottle.request
 response = bottle.response
 abort = bottle.abort
 
@@ -121,25 +119,34 @@
     {key: value for key, value in DEFAULTS.items() if key not in os.environ}
 )
 os.environ["PY4WEB_PATH"] = str(pathlib.Path(__file__).resolve().parents[1])
 
 
 # hold all framework hooks in one place
 # NOTE: `after_request` hooks are not currently used
-_REQUEST_HOOKS = types.SimpleNamespace(before=set())
-
+REQUEST_HOOKS = type("Object", (), dict(before=[]))  # pylint: disable=invalid-name
 
-def _before_request(*args, **kw):
-    [h(*args, **kw) for h in _REQUEST_HOOKS.before]
+# set to true to debug issues with fixtures
+DEBUG = False
 
 
-bottle.default_app().add_hook("before_request", _before_request)
+def register_hooks():
+    """register hooks with ombott if they exist"""
+    if not REQUEST_HOOKS.before:
+        return
+    bottle.default_app().add_hook(
+        "before_request",
+        lambda *args, **kwargs: [
+            func(*args, **kwargs) for func in REQUEST_HOOKS.before
+        ],
+    )
 
 
 def module2filename(module):
+    """given a module name as a string, convert to filename"""
     filename = os.path.join(*module.split(".")[1:])
     filename = (
         os.path.join(filename, "__init__.py")
         if not filename.count(os.sep)
         else filename + ".py"
     )
     return filename
@@ -155,38 +162,43 @@
 
 
 def required_folder(*parts):
     """joins the args and creates the folder if not exists"""
     path = os.path.join(*parts)
     if not os.path.exists(path):
         os.makedirs(path)
-    assert os.path.isdir(path), "%s is not a folder as required" % path
+    assert os.path.isdir(path), f"{path} is not a folder as required"
     return path
 
 
 def safely(func, exceptions=(Exception,), log=False, default=None):
     """
     runs the funnction and returns True on success,
     False if one of the exceptions is raised
     """
     try:
         return func()
     except exceptions as err:
         if log:
-            logging.warn(str(err))
+            logging.warning(str(err))
         return default() if callable(default) else default
 
 
 ########################################################################################
 # Implement a O(1) LRU cache and memoize with expiration and monitoring (using linked list)
 #########################################################################################
 
 
 class Node:
-    def __init__(self, key=None, value=None, t=None, m=None, prev=None, next=None):
+    """A node for the LRU cache"""
+
+    def __init__(
+        self, key=None, value=None, t=None, m=None, prev=None, next=None
+    ):  # pylint: disable=redefined-builtin
+        """create a node of the LRU cache"""
         self.key, self.value, self.t, self.m, self.prev, self.next = (
             key,
             value,
             t,
             m,
             prev,
             next,
@@ -203,25 +215,31 @@
             open(filename).read()), 60, lambda: os.path.getmtime())
 
     (computes and cashes the hash of file filename but only reads the file if mtime changes and
      does not check the mtime more oftern than every 60. caches the 1000 most recent hashes)
     """
 
     def __init__(self, size=1000):
+        """Create an LRU caching object"""
         self.free = size
         self.head = Node()
         self.tail = Node()
         self.head.next = self.tail
         self.tail.prev = self.head
         self.mapping = {}
         self.lock = threading.Lock()
 
     def get(self, key, callback, expiration=3600, monitor=None):
         """If key not stored or key has expired and monitor == None or monitor() value has changed, returns value = callback()"""
-        node, t0 = self.mapping.get(key), time.time()
+        # set defaults
+        node = self.mapping.get(key)
+        t0 = time.time()
+        value = None
+        t = t0
+        # update
         with self.lock:
             if node:
                 # if a node was found remove it from storage
                 value, t, node.next.prev, node.prev.next = (
                     node.value,
                     node.t,
                     node.prev,
@@ -234,31 +252,34 @@
         # check if cache expired
         if node and node.t + expiration < t0:
             # if cache should always be invalidated or m changed
             if m is None or node.m != m:
                 # ignore the value found
                 node = None
         if node is None:
-            value, t = callback(), t0
+            value = callback()
+            t = t0
         # add the new node back into storage
         with self.lock:
             new_node = Node(key, value, t, m, prev=self.head, next=self.head.next)
             self.mapping[key] = self.head.next = new_node.next.prev = new_node
             if self.free < 0:
                 last_node = self.tail.prev
                 self.tail.prev, last_node.prev.next = last_node.prev, self.tail
                 del self.mapping[last_node.key]
                 self.free += 1
         return value
 
     def memoize(self, expiration=3600):
+        """Decorator to memorize the output of any fuction"""
+
         def decorator(func):
             @functools.wraps(func)
             def memoized_func(*args, **kwargs):
-                key = "%s:%s:%s:%s" % (func.__module__, func.__name__, args, kwargs)
+                key = f"{func.__module__}:{func.__name__}:{args}:{kwargs}"
                 return self.get(
                     key,
                     lambda args=args, kwargs=kwargs: func(*args, **kwargs),
                     expiration=expiration,
                 )
 
             return memoized_func
@@ -267,133 +288,156 @@
 
 
 #########################################################################################
 # A Better JSON Serializer
 #########################################################################################
 
 
-def objectify(obj):
+def objectify(obj):  # pylint: disable=too-many-return-statements
     """converts the obj(ect) into a json serializable object"""
     if isinstance(obj, numbers.Integral):
         return int(obj)
-    elif isinstance(obj, (numbers.Rational, numbers.Real)):
+    if isinstance(obj, (numbers.Rational, numbers.Real)):
         return float(obj)
-    elif isinstance(obj, (datetime.date, datetime.datetime, datetime.time)):
+    if isinstance(obj, (datetime.date, datetime.datetime, datetime.time)):
         return obj.isoformat().replace("T", " ")
-    elif isinstance(obj, str):
+    if isinstance(obj, str):
         return obj
-    elif isinstance(obj, dict):
+    if isinstance(obj, dict):
         return obj
-    elif hasattr(obj, "as_list"):
+    if hasattr(obj, "as_list"):
         return obj.as_list()
-    elif hasattr(obj, "as_dict"):
+    if hasattr(obj, "as_dict"):
         return obj.as_dict()
-    elif hasattr(obj, "__iter__") or isinstance(obj, types.GeneratorType):
+    if hasattr(obj, "__iter__") or isinstance(obj, types.GeneratorType):
         return list(obj)
-    elif hasattr(obj, "xml"):
+    if hasattr(obj, "xml"):
         return obj.xml()
-    elif isinstance(
+    if isinstance(
         obj, enum.Enum
     ):  # Enum class handled specially to address self reference in __dict__
         return dict(name=obj.name, value=obj.value, __class__=obj.__class__.__name__)
-    elif hasattr(obj, "__dict__") and hasattr(obj, "__class__"):
+    if hasattr(obj, "__dict__") and hasattr(obj, "__class__"):
         d = dict(obj.__dict__)
         d["__class__"] = obj.__class__.__name__
         return d
     return str(obj)
 
 
 def dumps(obj, sort_keys=True, indent=2):
+    """General purpose memoize function with sane default"""
     return json.dumps(obj, default=objectify, sort_keys=sort_keys, indent=indent)
 
 
 #########################################################################################
 # Base Fixture (database connections, templates, sessions, and requirements are fixtures)
 #########################################################################################
 
 
-class Fixture:
-    __request_master_ctx__ = threading.local()
-    __fixture_debug__ = False
+class LocalUndefined(RuntimeError):
+    """
+    Exception raised trying to access an unitialized thread local
+    from a Fixture
+    """
+
+
+class BareFixture:
+    """Minimal Fixture class - without thread local logic"""
 
     # normally on_success/on_error are only called if none of the previous
     # on_request failed, if a fixture is_hook then on_error is always called.
     is_hook = False
 
-    @classmethod
-    def __init_request_ctx__(cls):
-        cls.__request_master_ctx__.request_ctx = dict()
-
-    @classmethod
-    def __mount_local__(cls, self, storage):
-        cls.__request_master_ctx__.request_ctx[self] = storage
+    def on_request(self, context):  # pylint: disable=unused-argument
+        """Method that will be called when a new HTTP request arrives"""
 
-    @property
-    def _safe_local(self):
-        try:
-            ret = self.__request_master_ctx__.request_ctx[self]
-        except (KeyError, AttributeError) as err:
-            msg = "py4web hint: check @action.uses() for the missing fixture {}".format(
-                self
-            )
-            raise RuntimeError(msg) from err
-        return ret
+    def on_error(self, context):  # pylint: disable=unused-argument
+        """Method that will be called when an HTTP request errors"""
 
-    @_safe_local.setter
-    def _safe_local(self, storage):
-        self.__mount_local__(self, storage)
+    def on_success(self, context):  # pylint: disable=unused-argument
+        """Method that will be called when an HTTP request succeeds"""
 
-    def is_valid(self):
-        """check if the fixture is valid in context"""
 
-        ctx = getattr(self.__request_master_ctx__, "request_ctx", None)
-        if not ctx or self not in ctx:
-            logging.warn(
-                "attempted access to fixture %s from outside a request",
-                self.__class__.__name__,
-            )
-            return False
-        return True
+class Fixture(BareFixture):
+    """
+    Fixture class - with thread local logic
+    all fixtures should inherit from this class
+    """
 
-    def on_request(self, context):
-        pass  # called when a request arrives
+    ### being logic to handle safe thread local
 
-    def on_error(self, context):
-        pass  # called when a request errors
+    _local = threading.local()
 
-    def on_success(self, context):
-        pass  # called when a request is successful
+    @staticmethod
+    def local_initialize(obj):
+        """To be called in on_request if the Fixtures needs a thread local dict"""
+        if not hasattr(Fixture._local, "request_ctx"):
+            Fixture._local.request_ctx = {}
+        if obj in Fixture._local.request_ctx:
+            raise RuntimeError(f"initialize_thread_local called twice for {obj}")
+        Fixture._local.request_ctx[obj] = types.SimpleNamespace()
 
+    @staticmethod
+    def local_delete(obj):
+        """To be called in on_success and on_error to cleat the thread local"""
+        del Fixture._local.request_ctx[obj]
 
-_REQUEST_HOOKS.before.add(Fixture.__init_request_ctx__)
+    @property
+    def local(self):
+        """Returns the fixture thread local dict if initialized else a default one"""
+        try:
+            return Fixture._local.request_ctx[self]
+        except (AttributeError, KeyError):
+            raise LocalUndefined(f"thread local not initialized for {self}") from None
+
+    def is_valid(self):
+        """Checks if the fixture has a valid thread local dict"""
+        try:
+            Fixture._local.request_ctx[self]  # pylint: disable=pointless-statement
+            return True
+        except (AttributeError, KeyError):
+            return False
+
+    ### end logic to handle safe thread local
 
 
-class Translator(pluralize.Translator, Fixture):
+class Translator(BareFixture, pluralize.Translator):
+    """a Fixture wrapper for the pluralize.Translator"""
+
     def on_request(self, context):
+        """Sets the request language from the request header"""
+        # important: pluralize.Translator has its own thread local
         self.select(request.headers.get("Accept-Language", "en"))
 
     def on_success(self, context):
-        response.headers["Content-Language"] = self.local.tag
+        """Inject the selected language in the response header"""
+        response.headers.setdefault("Content-Language", self.local.tag)
 
 
 class DAL(pydal.DAL, Fixture):
+    """a Fixture wrappre for pydal.DAL"""
+
     def on_request(self, context):
+        """Retrieves a database connection from the pool"""
+        # important: the connection pool handles its own thread local
         self.get_connection_from_pool_or_new()
         threadsafevariable.ThreadSafeVariable.restore(ICECUBE)
 
     def on_error(self, context):
+        """Rollback and recycle connection"""
         self.recycle_connection_in_pool_or_close("rollback")
 
     def on_success(self, context):
+        """Commit and recycle connection"""
         self.recycle_connection_in_pool_or_close("commit")
 
 
 # make sure some variables in pydal are thread safe
 def thread_safe_pydal_patch():
-    Field = pydal.DAL.Field
+    """Make the selected fields attributes thread local variables"""
     tsafe_attrs = [
         "readable",
         "writable",
         "default",
         "filter_in",
         "filter_out",
         "label",
@@ -447,82 +491,73 @@
         flash.set('hello', _class='important')
         return dict()
 
     Flash messages are added to the dict and, upon redirect, carry forward
     Also notice all Flash objects share the same threading local so act as singletons
     """
 
-    # this essential makes flash a singleton
-    # necessary because auth defines its own flash
-    # possible because flash does not depend on the app
-
-    @property
-    def local(self):
-        return self._safe_local
-
     def on_request(self, context):
-        self._safe_local = types.SimpleNamespace()
+        """Retrieves flash message from cookie if present"""
+        Fixture.local_initialize(self)
         # when a new request arrives we look for a flash message in the cookie
         flash = request.get_cookie("py4web-flash")
         if flash:
             self.local.flash = safely(lambda: json.loads(flash), default=None)
         else:
             self.local.flash = None
 
     def on_success(self, context):
+        """Stores the flash message in cookie"""
         # if we redirect and have a flash message we move it to the session
         status = context["status"]
         if status == 303 and self.local.flash:
             response.set_cookie("py4web-flash", json.dumps(self.local.flash), path="/")
         else:
             response.delete_cookie("py4web-flash", path="/")
         # if we have a valid flash message, we store it for the template to use later
         output = context["output"]
         flash = self.local.flash or ""
         if isinstance(output, dict):
             if "template_inject" in context:
                 context["template_inject"]["flash"] = flash
             else:
                 context["template_inject"] = dict(flash=flash)
-        else:
-            if self.local.flash is not None:
-                response.headers["component-flash"] = json.dumps(flash)
-        self.local.flash = None
-        self.local.__dict__.clear()
-
-    def on_error(self, context):
-        """Clears the local to prevent leakage."""
-        self.local.__dict__.clear()
+        elif self.local.flash is not None:
+            response.headers.setdefault("component-flash", json.dumps(flash))
 
     def set(self, message, _class="", sanitize=True):
+        """Stores a message in the object thread safe storage"""
         # we set a flash message
         if sanitize:
             message = yatl.sanitizer.xmlescape(message)
         self.local.flash = {"message": message, "class": _class}
 
 
 #########################################################################################
 # The Template Rendered Fixture
 #########################################################################################
 
 
 class RenoirXMLEscapeMixin:
+    """for internal Renoir use"""
+
     def _escape_data(self, data):
         """Allows Renoir to convert yatl helpers to strings"""
         return safely(
-            lambda: data.xml(), default=lambda: self._to_html(self._to_unicode(data))
+            lambda: data.xml(),  # pylint: disable=unnecessary-lambda
+            default=lambda: self._to_html(self._to_unicode(data)),
         )
 
 
-class RenoirCustomWriter(RenoirXMLEscapeMixin, renoir.writers.Writer): ...
+class RenoirCustomWriter(RenoirXMLEscapeMixin, renoir.writers.Writer):
+    """for internal Renoir use"""
 
 
-class RenoirCustomEscapeAllWriter(
-    RenoirXMLEscapeMixin, renoir.writers.EscapeAllWriter
-): ...
+class RenoirCustomEscapeAllWriter(RenoirXMLEscapeMixin, renoir.writers.EscapeAllWriter):
+    """for internal Renoir use"""
 
 
 class Renoir(renoir.Renoir):
     """Custom Renoir Engine that understands yatl helpers"""
 
     _writers = {
         renoir.constants.ESCAPES.common: RenoirCustomWriter,
@@ -530,43 +565,55 @@
     }
 
 
 def render(
     content=None,
     filename=None,
     path=".",
-    context={},
+    context=None,
     delimiters="[[ ]]",
     cached_renoir_engines=Cache(100),
 ):
     """
-    renders the template using renoire, same API as yatl.render, does caching of
+    Renders the template using renoire, same API as yatl.render, does caching of
     both Renoire engine and source files
     """
+    context = context or {}
     engine = cached_renoir_engines.get(
         (path, delimiters),
         lambda: Renoir(path=path, delimiters=delimiters.split(" "), reload=True),
     )
     if content is not None:
-        return engine._render(content, context=context)
+        return engine._render(  # pylint: disable=protected-access
+            content, context=context
+        )
     return engine.render(filename, context=context)
 
 
 class Template(Fixture):
+    """The Template Fixture class"""
+
     cache = Cache(100)
 
     def __init__(self, filename, path=None, delimiters="[[ ]]"):
+        """Initialized the template object"""
         self.filename = filename
         self.path = path
         self.delimiters = delimiters
 
     def on_success(self, context):
+        """
+        Filters the context output through the template
+        Also injects helpers in the output dict
+        """
         output = context["output"]
+
+        # we only proceed furthed if the output is a dict
         if not isinstance(output, dict):
-            return output
+            return
 
         ctx = dict(request=request)
         ctx.update(HELPERS)
         ctx.update(URL=URL)
         ctx.update(context.get("template_inject", {}))
         ctx.update(output)
         ctx["__vars__"] = output
@@ -584,222 +631,267 @@
 
 #########################################################################################
 # The Session Fixture
 #########################################################################################
 
 
 class Session(Fixture):
+    """The Session Fixture"""
+
     # All apps share the same default secret if not specified.
     # important for _dashboard reload
     # the actual value is loaded from a file
     SECRET = None
-    __slots__ = ["_safe", "secret", "expiration", "algorithm", "storage", "same_site"]
+    _params = {}
 
     @property
-    def local(self):
-        return self._safe_local
+    def params(self):
+        """Returns the object parameters"""
+        return Session._params[self]
 
     def __init__(
         self,
         secret=None,
         expiration=None,
         algorithm="HS256",
         storage=None,
         same_site="Lax",
         name="{app_name}_session",
     ):
         """
+        Creates a session object.
+
         secret is the shared key used to encrypt the session (using algorithm)
         expiration is in seconds
         (optional) storage must have a get(key) and set(key,value,expiration) methods
         session is stored signed and encrypted in the cookie
         """
-        # assert Session.SECRET, "Missing Session.SECRET"
-        self.secret = secret or Session.SECRET
-        self.expiration = expiration
-        self.algorithm = algorithm
-        self.storage = storage
-        self.same_site = same_site
-        self.name = name
+        secret = secret or Session.SECRET
+        assert (
+            isinstance(secret, str)
+            and not pydal.validators.IS_STRONG(entropy=50)(secret)[1]
+        ), "Not a good secret"
+
         if isinstance(storage, Session):
-            self.__prerequisites__ = [storage]
-        if hasattr(storage, "__prerequisites__"):
-            self.__prerequisites__ = storage.__prerequisites__
-
-    def initialize(self, app_name="unknown", data=None, changed=False, secure=False):
-        self._safe_local = types.SimpleNamespace()
-        local = self.local
-        local.changed = changed
-        local.data = data or {}
-        local.session_cookie_name = self.name.format(app_name=app_name)
-        local.secure = secure
+            prerequisites = [storage]
+        elif hasattr(storage, "__prerequisites__"):
+            prerequisites = storage.__prerequisites__
+        else:
+            prerequisites = []
+        Session._params[self] = type(
+            "Object",
+            (),
+            dict(
+                secret=secret,
+                expiration=expiration,
+                algorithm=algorithm,
+                storage=storage,
+                same_site=same_site,
+                name=name,
+                prerequisites=prerequisites,
+            ),
+        )
+
+    @property
+    def __prerequisites__(self):
+        """Returns the session prerequisite fixtures"""
+        return self.params.prerequisites
 
     def load(self):
-        self.initialize(
-            app_name=request.app_name,
-            changed=False,
-            secure=request.url.startswith("https"),
-        )
+        """Loads a session"""
+        app_name = request.app_name
+        params = self.params
         self_local = self.local
-        raw_token = request.get_cookie(
-            self_local.session_cookie_name
-        ) or request.query.get("_session_token")
+        self_local.changed = False
+        self_local.data = {}
+        self_local.cookie_name = params.name.format(app_name=app_name)
+        self_local.secure = request.url.startswith("https")
+        raw_token = request.get_cookie(self_local.cookie_name) or request.query.get(
+            "_session_token"
+        )
         if not raw_token and request.method in {"POST", "PUT", "DELETE", "PATCH"}:
             raw_token = (
                 request.forms
                 and request.forms.get("_session_token")
                 or request.json
                 and request.json.get("_session_token")
             )
-        if Fixture.__fixture_debug__:
+        if DEBUG:
             logging.debug("Session token found %s", raw_token)
+        data = {}
+        # if we have a token in the query string of cookie
         if raw_token:
             try:
-                if self.storage:
+                # if session i stored serverside
+                if params.storage:
+                    # used token as id and retrieve data
                     token_data = raw_token.encode()
-                    json_data = self.storage.get(token_data)
+                    json_data = params.storage.get(token_data)
                     if isinstance(json_data, bytes):
                         json_data = json_data.decode("utf8")
                     if json_data:
-                        self_local.data = json.loads(json_data)
+                        data = json.loads(json_data)
                 else:
+                    # rertieve the data from inside the token itself
                     try:
-                        self_local.data = secure_loads(raw_token, self.secret.encode())
+                        data = secure_loads(raw_token, params.secret.encode())
                     except (AssertionError, json.JSONDecodeError):
-                        self_local.data = {}
-                if self.expiration is not None and self.storage is None:
-                    assert self_local.data["timestamp"] > time.time() - int(
-                        self.expiration
-                    )
-                assert self.get_data().get("secure") == self_local.secure
+                        data = {}
             except Exception as err:
-                if Fixture.__fixture_debug__:
+                # something went wrong, unable to load session data
+                if DEBUG:
                     logging.debug("Session error %s", err)
+        # if the session data is valid update the current session
         if (
-            self.get_data().get("session_cookie_name") != self_local.session_cookie_name
-            or "uuid" not in self.get_data()
+            data.get("cookie_name") == self_local.cookie_name  # have valid cookie
+            and data.get("secure") == self_local.secure  # have valid security
+            and data.get("uuid") is not None  # have a uuid
+            and (
+                params.expiration is None  # has not expired
+                or data["timestamp"] > time.time() - int(params.expiration)
+            )
         ):
-            self.clear()
-
-    def get_data(self):
-        return getattr(self.local, "data", {})
+            self_local.data.update(data)  # the take the loaded data
 
     def save(self):
+        """Saves the session"""
+        params = self.params
         self_local = self.local
+        # make sure the session constain these basic veriables
+        if "uuid" not in self_local.data:
+            self_local.data["uuid"] = str(uuid.uuid4())
         self_local.data["timestamp"] = time.time()
-        self_local.data["session_cookie_name"] = self_local.session_cookie_name
-        if self.storage:
+        self_local.data["secure"] = self_local.secure
+        self_local.data["cookie_name"] = self_local.cookie_name
+        if params.storage:
             cookie_data = self_local.data["uuid"]
-            self.storage.set(cookie_data, json.dumps(self_local.data), self.expiration)
+            params.storage.set(
+                cookie_data, json.dumps(self_local.data), params.expiration
+            )
         else:
-            cookie_data = secure_dumps(self_local.data, self.secret.encode())
-        if Fixture.__fixture_debug__:
+            cookie_data = secure_dumps(self_local.data, params.secret.encode())
+        if DEBUG:
             logging.debug("Session stored %s", cookie_data)
         response.set_cookie(
-            self_local.session_cookie_name,
+            self_local.cookie_name,
             cookie_data,
             path="/",
             secure=self_local.secure,
-            same_site=self.same_site,
+            same_site=params.same_site,
             httponly=True,
         )
 
     def get(self, key, default=None):
-        return self.get_data().get(key, default)
+        """Get the value for the key from session"""
+        try:
+            return self.local.data.get(key, default)
+        except LocalUndefined:
+            return default
 
     def __getitem__(self, key):
-        return self.get_data()[key]
+        """Session key getter"""
+        return self.local.data[key]
 
     def __delitem__(self, key):
-        if key in self.get_data():
+        """Deletes a key from the session"""
+        if key in self.local.data:
             self.local.changed = True
             del self.local.data[key]
 
     def __setitem__(self, key, value):
+        """Session key setter"""
         self.local.changed = True
         self.local.data[key] = value
 
     def __contains__(self, other):
-        return other in self.get_data()
+        """Checks if a key in session"""
+        return other in self.local.data
 
     def keys(self):
-        return self.get_data().keys()
+        """Returns the session keys"""
+        return self.local.data.keys()
 
     def items(self):
-        return self.get_data().items()
+        """Returns the (key, value) in session"""
+        return self.local.data.items()
 
     def __iter__(self):
-        yield from self.get_data().keys()
+        """Iterates over the session keys"""
+        yield from self.local.data.keys()
+
+    __getattr__ = get
+    __setattr__ = __setitem__
+    __delattr__ = __delitem__
 
     def clear(self):
-        """Produces a brand-new session."""
+        """Clears the session key"""
         self_local = self.local
         self_local.changed = True
         self_local.data.clear()
-        self_local.data["uuid"] = str(uuid.uuid1())
-        self_local.data["secure"] = self_local.secure
 
     def on_request(self, context):
+        """Initializes the session thread local and tries to load a session"""
+        Fixture.local_initialize(self)
         self.load()
 
-    def on_error(self, context):
-        if self.local.changed:
-            self.save()
-
     def on_success(self, context):
+        """Saves the session if its content changed"""
         if self.local.changed:
             self.save()
 
 
 #########################################################################################
 # The URL Helper
 #########################################################################################
 
 
-def URL(
+def URL(  # pylint: disable=invalid-name
     *parts,
-    vars=None,
-    hash=None,
+    vars=None,  # pylint: disable=redefined-builtin
+    hash=None,  # pylint: disable=redefined-builtin
     scheme=False,
     signer=None,
     use_appname=None,
     static_version=None,
 ):
     """
+    Generates a URL for the action.
+
     Examples:
     URL('a','b',vars=dict(x=1),hash='y')       -> /{script_name?}/{app_name?}/a/b?x=1#y
     URL('a','b',vars=dict(x=1),scheme=None)    -> //{domain}/{script_name?}/{app_name?}/a/b?x=1
     URL('a','b',vars=dict(x=1),scheme=True)    -> http://{domain}/{script_name?}/{app_name?}/a/b?x=1
     URL('a','b',vars=dict(x=1),scheme='https') -> https://{domain}/{script_name?}/{app_name?}/a/b?x=1
     URL('a','b',vars=dict(x=1),use_appname=False) -> /{script_name?}/a/b?x=1
     """
     if use_appname is None:
         # force use_appname on domain-unmapped apps
         use_appname = not request.environ.get("HTTP_X_PY4WEB_APPNAME")
+    has_appname = False
     if use_appname:
         # app_name is not set by py4web shell
         app_name = getattr(request, "app_name", None)
-    has_appname = use_appname and app_name
+        has_appname = use_appname and app_name
     script_name = (
         request.environ.get("SCRIPT_NAME", "")
         or request.environ.get("HTTP_X_SCRIPT_NAME", "")
     ).rstrip("/")
     if parts and parts[0].startswith("/"):
         prefix = ""
     elif has_appname and app_name != "_default":
-        prefix = "%s/%s/" % (script_name, app_name)
+        prefix = f"{script_name}/{app_name}/"
     else:
-        prefix = "%s/" % script_name
+        prefix = f"{script_name}/"
     broken_parts = []
     for part in parts:
         broken_parts += str(part).rstrip("/").split("/")
     if static_version != "" and broken_parts and broken_parts[0] == "static":
         if not static_version:
             # try to retrieve from __init__.py
-            app_module = "apps.%s" % app_name if has_appname else "apps"
+            app_module = f"apps.{app_name}" if has_appname else "apps"
             try:
                 static_version = getattr(
                     sys.modules[app_module], "__static_version__", None
                 )
             except KeyError:
                 static_version = None
         if static_version:
@@ -811,89 +903,91 @@
     urlvars = dict(vars) if vars else {}
     if signer:
         # Note that we need to sign the non-urlencoded URL, since
         # at verification time, it will be already URLdecoded.
         signer.sign(prefix + "/".join(broken_parts), urlvars)
     if urlvars:
         url += "?" + "&".join(
-            "%s=%s" % (k, urllib.parse.quote(str(v))) for k, v in urlvars.items()
+            f"{k}={urllib.parse.quote(str(v))}" for k, v in urlvars.items()
         )
     if hash:
-        url += "#%s" % hash
+        url += f"#{hash}"
     if scheme is not False:
         original_url = request.environ.get("HTTP_ORIGIN") or request.url
         orig_scheme, _, domain = original_url.split("/", 3)[:3]
         if scheme is True:
             scheme = orig_scheme
         elif scheme is None:
             scheme = ""
         else:
             scheme += ":"
-        url = "%s//%s%s" % (scheme, domain, url)
+        url = f"{scheme}//{domain}{url}"
     return url
 
 
 #########################################################################################
 # The Action Decorator
 #########################################################################################
 
 
 class HTTP(BaseException):
     """An exception that is considered success"""
 
-    def __init__(self, status, body="", headers={}):
+    def __init__(self, status, body="", headers=None):
+        """Makes an HTTP object"""
         self.status = status
         self.body = body
-        self.headers = headers
+        self.headers = headers or {}
 
 
 def redirect(location):
-    """raises HTTP(303) to the specified location"""
-    response.headers["Location"] = location
+    """Raises HTTP(303) to redirect to the specified location"""
+    response.headers.setdefault("Location", location)
     raise HTTP(303)
 
 
-class action:
+class action:  # pylint: disable=invalid-name
     """@action(...) is a decorator for functions to be exposed as actions"""
 
     registered = set()
     app_name = "_default"
 
     def __init__(self, path, **kwargs):
+        """Constructs the action decorator"""
         self.path = path
         self.kwargs = kwargs
 
     @staticmethod
     def uses(*fixtures_in):
-        """Find all fixtures, including dependencies, topologically sorted"""
+        """Used to declare needed fixtures, they will be topologically sorted"""
         fixtures = []
         reversed_fixtures = []
         stack = list(fixtures_in)
         while stack:
             fixture = stack.pop()
             reversed_fixtures.append(fixture)
             stack.extend(getattr(fixture, "__prerequisites__", ()))
         for fixture in reversed(reversed_fixtures):
             if isinstance(fixture, str):
                 fixture = Template(fixture)
             if fixture not in fixtures:
                 fixtures.append(fixture)
 
         def decorator(func):
-            if Fixture.__fixture_debug__:
+            if DEBUG:
                 # in debug mode log all calls to fixtures
-                def call(f, context):
+                def call_f(f, context):
                     logging.debug(
-                        f"Calling {f.__self__.__class__.__name__}.{f.__name__}"
+                        "Calling %s.%s", f.__self__.__class__.__name__, f.__name__
                     )
                     return f(context)
 
             else:
 
-                def call(f, context):
+                def call_f(f, context):
                     return f(context)
 
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 # data shared by all fixtures in the pipeline for each request
                 processed = []
                 context = {
@@ -901,38 +995,40 @@
                     "status": 200,
                     "output": None,
                     "exception": None,
                     "processed": processed,
                 }
                 try:
                     for fixture in fixtures:
-                        call(fixture.on_request, context)
+                        call_f(fixture.on_request, context)
                         processed.append(fixture)
                     context["output"] = func(*args, **kwargs)
-                except HTTP as http:
-                    context["status"] = http.status
-                    raise http
+                except HTTP as http_exception:
+                    context["status"] = http_exception.status
+                    raise http_exception
                 except bottle.HTTPError as error:
                     context["exception"] = error
                 except bottle.HTTPResponse:
                     raise
                 except Exception as error:
                     context["exception"] = error
                 finally:
                     for fixture in reversed(fixtures):
                         if fixture in processed or getattr(fixture, "is_hook", False):
                             try:
                                 if context.get("exception"):
-                                    call(fixture.on_error, context)
+                                    call_f(fixture.on_error, context)
                                 else:
-                                    call(fixture.on_success, context)
-                            except Exception as error:
-                                context["exception"] = context.get("exception") or error
-                    if context.get("exception"):
-                        raise context["exception"]
+                                    call_f(fixture.on_success, context)
+                            except Exception as err:
+                                context["exception"] = context.get("exception") or err
+                        safely(lambda: Fixture.local_delete(fixture))
+                    exception = context.get("exception")
+                    if isinstance(exception, Exception):
+                        raise exception
                 return context.get("output", "")
 
             return wrapper
 
         return decorator
 
     @staticmethod
@@ -941,31 +1037,31 @@
 
         @functools.wraps(func)
         def wrapper(*func_args, **func_kwargs):
             try:
                 request.app_name = app_name
                 ret = func(*func_args, **func_kwargs)
                 if isinstance(ret, (list, dict)):
-                    response.headers["Content-Type"] = "application/json"
+                    response.headers.setdefault("Content-Type", "application/json")
                     ret = dumps(ret)
                 elif ret is None:
                     ret = ""
                 elif isinstance(ret, yatl.helpers.TAGGER):
                     ret = str(ret)
                 elif not hasattr(ret, "__iter__"):
                     raise RuntimeError(f"Cannot return type {ret.__class__.__name__}")
                 return ret
-            except HTTP as http:
-                response.status = http.status
-                response.headers.update(http.headers)
-                body = http.body
+            except HTTP as http_exception:
+                response.status = http_exception.status
+                response.headers.update(http_exception.headers)
+                body = http_exception.body
                 return dumps(body) if isinstance(body, (list, dict)) else str(body)
             except bottle.HTTPResponse:
                 raise
-            except Exception:
+            except Exception:  # pylint: disable=broad-exception-caught
                 snapshot = get_error_snapshot()
                 logging.error(snapshot["traceback"])
                 ticket_uuid = error_logger.log(request.app_name, snapshot) or "unknown"
                 response.status = 500
                 return error_page(
                     500,
                     button_text=ticket_uuid,
@@ -986,31 +1082,37 @@
         if path.endswith("/index"):  # /index is always optional
             short_path = path[:-6] or "/"
             Reloader.register_route(app_name, short_path, self.kwargs, func)
         return func
 
 
 class Condition(Fixture):
+    """The Condition Fixture"""
+
     def __init__(self, condition, on_false=None, exception=HTTP(400)):
+        """Creates a fixture that checks for a given condition"""
         self.condition = condition
         self.on_false = on_false
         self.exception = exception
 
     def on_request(self, context):
+        """Checks if the condition is true or false"""
         if not self.condition():
             if self.on_false is not None:
                 self.on_false()
             raise self.exception
 
 
 #########################################################################################
 # Monkey Patch: Cookies
 #########################################################################################
 
-http.cookies.Morsel._reserved["same-site"] = "SameSite"
+http.cookies.Morsel._reserved[  # pylint: disable=protected-access
+    "same-site"
+] = "SameSite"
 
 #########################################################################################
 # Monkey Patch: ssl bug for gevent
 #########################################################################################
 
 __ssl__ = __import__("ssl")
 _ssl = getattr(__ssl__, "_ssl") or getattr(__ssl__, "_ssl2")
@@ -1022,24 +1124,27 @@
     keyfile=None,
     certfile=None,
     cert_reqs=__ssl__.CERT_NONE,
     ssl_version=__ssl__.PROTOCOL_SSLv23,
     ca_certs=None,
     ciphers=None,
 ):
+    """Used to support HTTP"""
     context = __ssl__.SSLContext(ssl_version)
     context.verify_mode = cert_reqs or __ssl__.CERT_NONE
     if ca_certs:
         context.load_verify_locations(ca_certs)
     if certfile:
         context.load_cert_chain(certfile, keyfile)
     if ciphers:
         context.set_ciphers(ciphers)
     caller_self = inspect.currentframe().f_back.f_locals["self"]
-    return context._wrap_socket(sock, server_side=server_side, ssl_sock=caller_self)
+    return context._wrap_socket(  # pylint: disable=protected-access
+        sock, server_side=server_side, ssl_sock=caller_self
+    )
 
 
 #########################################################################################
 # Error Handling
 #########################################################################################
 
 
@@ -1051,15 +1156,15 @@
     if errorlog:
         msg = f"[{datetime.datetime.now().isoformat()}]: {tb}\n"
         if errorlog == ":stderr":
             sys.stderr.write(msg)
         elif errorlog == ":stdout":
             sys.stdout.write(msg)
         elif errorlog == "tickets_only":
-            pass
+            ...
         else:
             with portalocker.Lock(errorlog, "a", timeout=2) as fp:
                 fp.write(msg)
 
     etype, evalue, etb = sys.exc_info()
     if isinstance(etype, type):
         etype = etype.__name__
@@ -1092,35 +1197,38 @@
     data["exception_value"] = str(evalue)
 
     # Loopover the stack frames
     items = inspect.getinnerframes(etb, depth)
     del etb  # Prevent circular references that would cause memory leaks
     data["stackframes"] = stackframes = []
 
-    for frame, file, lnum, func, lines, idx in items:
+    for frame, file, lnum, func, lines, idx in items:  # pylint: disable=unused-variable
         file = file and os.path.abspath(file) or "?"
-        args, varargs, varkw, locals = inspect.getargvalues(frame)
+        # TODO: call inspect.getargvalues(frame) and get more info
         # Basic frame information
         f = {"file": file, "func": func, "lnum": lnum}
         f["code"] = lines
         stackframes.append(f)
 
     return data
 
 
 class SimpleErrorLogger:
+    """Simple Error Logger"""
+
     def log(self, app_name, snapshot):
-        """logs the error"""
-        logging.error("%s error:\n%s" % (app_name, snapshot["traceback"]))
-        return None
+        """Logs the error"""
+        logging.error("%s error:\n%s", app_name, snapshot["traceback"])
 
 
 class DatabaseErrorLogger:
+    """Database Error Logger"""
+
     def __init__(self):
-        """creates the py4web_error table in the service database"""
+        """Creates the py4web_error table in the service database"""
         uri = os.environ["PY4WEB_SERVICE_DB_URI"]
         folder = os.environ["PY4WEB_SERVICE_FOLDER"]
         self.db = DAL(uri, folder=folder)
         self.db.define_table(
             "py4web_error",
             Field("uuid"),
             Field("app_name"),
@@ -1130,36 +1238,36 @@
             Field("client_ip", "string"),
             Field("error", "string"),
             Field("snapshot", "json"),
         )
         self.db.commit()
 
     def log(self, app_name, error_snapshot):
-        """store error snapshot (ticket) in the database"""
+        """Store error snapshot (ticket) in the database"""
         ticket_uuid = str(uuid.uuid4())
         try:
             self.db.py4web_error.insert(
                 uuid=ticket_uuid,
                 app_name=app_name,
                 method=request.method,
                 path=request.path,
                 timestamp=datetime.datetime.utcnow(),
                 client_ip=request.environ.get("REMOTE_ADDR"),
                 error=error_snapshot["exception_value"],
                 snapshot=error_snapshot,
             )
             self.db.commit()
             return ticket_uuid
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             logging.error(str(err))
             self.db.rollback()
             return None
 
     def get(self, ticket_uuid=None):
-        """retrieve a ticket from error database"""
+        """Retrieve a ticket from error database"""
         db = self.db
         if ticket_uuid:
             query, orderby = db.py4web_error.uuid == ticket_uuid, None
             rows = db(query).select(orderby=orderby, limitby=(0, 1)).as_list()
         else:
             orderby = ~db.py4web_error.timestamp
             groupby = db.py4web_error.path | db.py4web_error.error
@@ -1176,15 +1284,15 @@
             for item in list_rows:
                 row = item["py4web_error"]
                 row["count"] = item["_extra"][str(db.py4web_error.id.count())]
                 rows.append(row)
         return rows if not ticket_uuid else rows[0] if rows else None
 
     def clear(self):
-        """erase all tickets from database"""
+        """Erase all tickets from database"""
         db = self.db
         db(db.py4web_error).delete()
         self.db.commit()
 
 
 class ErrorLogger:
     """
@@ -1200,69 +1308,68 @@
 
     def __init__(self):
         self.fallback_logger = SimpleErrorLogger()
         self.database_logger = None
         self.plugins = {}
 
     def initialize(self):
-        """try inizalize database if we have service folder"""
+        """Try inizalize database if we have service folder"""
         self.database_logger = safely(DatabaseErrorLogger, log=True)
 
     def _get_logger(self, app_name):
-        """get the appropriate logger for the app"""
+        """Get the appropriate logger for the app"""
         return (
             self.plugins.get(app_name) or self.database_logger or self.fallback_logger
         )
 
     def log(self, app_name, error_snapshot):
-        """log the error snapshot"""
+        """Log the error snapshot"""
         logger = self._get_logger(app_name)
         ticket_uuid = safely(lambda: logger.log(app_name, error_snapshot))
         if not ticket_uuid:
             self.fallback_logger.log(app_name, error_snapshot)
         return ticket_uuid
 
 
 error_logger = ErrorLogger()
 
 #########################################################################################
 # Loading &  Reloading Logic
 #########################################################################################
 
 
-class StreamProxy:
-    def __init__(self, stream):
-        self._stream = stream
-
-    def write(self, *args, **kwargs):
-        return self._stream.write(*args, **kwargs)
-
-
 class Reloader:
+    """
+    Class responsible for loading/readloading apps
+    """
+
     ROUTES = collections.defaultdict(list)
     MODULES = {}
     ERRORS = {}
 
     @staticmethod
     def install_reloader_hook():
+        """Installs the Reloader hook, checks for changes at every request"""
+
         # used by watcher
-        def hook(*a, **k):
+        def hook(*args, **kwargs):  # pylint: disable=unused-argument
             app_name = request.path.split("/")[1]
             if app_name not in Reloader.ROUTES:
                 app_name = "_default"
             if DIRTY_APPS.get(app_name):
                 Reloader.import_app(app_name)
                 DIRTY_APPS[app_name] = False
             ## APP_WATCH tasks, if used by any app
             try_app_watch_tasks()
 
-        _REQUEST_HOOKS.before.add(hook)
+        REQUEST_HOOKS.before.append(hook)
 
     @staticmethod
     def clear_routes(app_names=None):
+        """Clears all stored routes"""
         remove_route = bottle.default_app().router.remove
         if app_names is None:
             app_names = Reloader.ROUTES.keys()
         for app_name in app_names:
             for route in Reloader.ROUTES[app_name]:
                 remove_route(route["rule"])
             Reloader.ROUTES[app_name] = []
@@ -1271,113 +1378,117 @@
     def import_apps():
         """Import or reimport modules and exposed static files"""
         Reloader.clear_routes()
         folder = os.environ["PY4WEB_APPS_FOLDER"]
         # if first time reload dummy top module
         if not Reloader.MODULES:
             path = os.path.join(folder, "__init__.py")
-            module = load_module("apps", path)  # noqa: F841
+            load_module("apps", path)  # noqa: F841
         # Then load all the apps as submodules
         if os.environ.get("PY4WEB_APP_NAMES"):
             app_names = os.environ.get("PY4WEB_APP_NAMES").split(",")
         else:
             app_names = os.listdir(folder)
         for app_name in app_names:
             Reloader.import_app(app_name, clear_before_import=False)
 
     @staticmethod
     def import_app(app_name, clear_before_import=True):
+        """Imports a specified app and its routes"""
         if clear_before_import:
             Reloader.clear_routes([app_name])
         Reloader.ROUTES[app_name] = []
         folder = os.environ["PY4WEB_APPS_FOLDER"]
         path = os.path.join(folder, app_name)
         init = os.path.join(path, "__init__.py")
 
         if os.path.isdir(path) and not path.endswith("__") and os.path.exists(init):
             action.app_name = app_name
-            module_name = "apps.%s" % app_name
+            module_name = f"apps.{app_name}"
 
             def clear_modules():
                 # all files/submodules
                 names = [
                     name
                     for name in sys.modules
                     if (name + ".").startswith(module_name + ".")
                 ]
                 for name in names:
                     del sys.modules[name]
 
             try:
                 module = Reloader.MODULES.get(app_name)
                 if not module:
-                    click.echo("[ ] loading %s ..." % app_name)
+                    click.echo(f"[ ] loading {app_name} ...")
                 else:
-                    click.echo("[ ] reloading %s ..." % app_name)
+                    click.echo(f"[ ] reloading {app_name} ...")
                     # forget the module
                     del Reloader.MODULES[app_name]
                     clear_modules()
 
                 load_module_message = None
-                buf_out = StreamProxy(io.StringIO())
-                buf_err = StreamProxy(buf_out._stream)
+                buf_out = io.StringIO()
+                buf_err = buf_out
                 with redirect_stdout(buf_out), redirect_stderr(buf_err):
                     module = load_module(module_name, init)
-                    load_module_message = buf_out._stream.getvalue()
-                buf_out._stream.close()
-                buf_out._stream = sys.stdout
-                buf_err._stream = sys.stderr
+                    load_module_message = buf_out.getvalue()
+                buf_out.close()
+                buf_out = sys.stdout
+                buf_err = sys.stderr
 
                 if load_module_message:
-                    click.secho("\x1b[A    output %s       " % app_name, fg="yellow")
+                    click.secho(f"\x1b[A    output {app_name}       ", fg="yellow")
                     click.echo(load_module_message)
 
-                click.secho("\x1b[A[X] loaded %s       " % app_name, fg="green")
+                click.secho(f"\x1b[A[X] loaded {app_name}       ", fg="green")
                 Reloader.MODULES[app_name] = module
                 Reloader.ERRORS[app_name] = None
-            except Exception as err:
+            except Exception as err:  # pylint: disable=broad-exception-caught
                 Reloader.ERRORS[app_name] = traceback.format_exc()
                 error_logger.log(app_name, get_error_snapshot())
                 click.secho(
-                    "\x1b[A[FAILED] loading %s (%s)" % (app_name, err),
+                    f"\x1b[A[FAILED] loading {app_name} ({err})",
                     fg="red",
                 )
                 # clear all files/submodules if the loading fails
                 clear_modules()
-                return None
 
         # Expose static files with support for static asset management
         static_folder = os.path.join(path, "static")
 
         if os.path.exists(static_folder):
             app_name = path.split(os.path.sep)[-1]
             prefix = "" if app_name == "_default" else f"/{app_name}"
             path = prefix + r"/static/<re((_\d+(\.\d+){2}/)?)><fp.path()>"
 
             def server_static(fp, static_folder=static_folder):
+                """Action that serves static/ files"""
                 filename = fp
                 response.headers.setdefault("Pragma", "cache")
                 response.headers.setdefault("Cache-Control", "private")
                 return bottle.static_file(filename, root=static_folder)
 
             Reloader.register_route(app_name, path, {"method": "GET"}, server_static)
 
+        # Very important to make sure actions can modify Field attributes
+        # in a thread safe manner
         ICECUBE.update(threadsafevariable.ThreadSafeVariable.freeze())
 
     @staticmethod
     def register_route(app_name, rule, kwargs, func):
+        """Given an app_name and a rule registers the corresponding routes"""
         url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
         if url_prefix and rule == "/":
             rule = ""
         else:
             rule = url_prefix + rule
         dec_func = action.catch_errors(app_name, func)
         bottle.route(rule, **kwargs)(dec_func)
         filename = module2filename(func.__module__)
-        methods = kwargs.get("method", ["GET"])
+        methods = kwargs.get("method", ["GET", "POST"])
         if isinstance(methods, str):
             methods = [methods]
         for method in methods:
             Reloader.ROUTES[app_name].append(
                 {
                     "rule": rule,
                     "method": method,
@@ -1398,38 +1509,40 @@
         "a{color:white;text-decoration:none;font-weight:bold;padding:10px 10px;border-radius:10px;border:2px solid #fff;transition: all .5s ease} "
         "a:hover{background:rgba(0,0,0,0.1);padding:10px 30px}</style></head>"
         '<body><h1>[[=code]]</h1><h2>[[=message]]</h2>[[if button_text:]]<a href="[[=href]]">[[=button_text]]</a>[[pass]]</body></html>'
     ),
 }
 
 
-def error_page(code, button_text=None, href="#", color=None, message=None):
+def error_page(token, button_text=None, href="#", color=None, message=None):
+    """Generates an error page"""
     if button_text:
         button_text = sanitize_html.escape(button_text)
     href = sanitize_html.escape(href)
-    message = http.client.responses[code].upper() if message is None else message
+    message = http.client.responses[token].upper() if message is None else message
     color = (
-        {"4": "#F44336", "5": "#607D8B"}.get(str(code)[0], "#2196F3")
+        {"4": "#F44336", "5": "#607D8B"}.get(str(token)[0], "#2196F3")
         if not color
         else color
     )
     context = dict(
-        code=code, message=message, button_text=button_text, href=href, color=color
+        code=token, message=message, button_text=button_text, href=href, color=color
     )
     # if client accepts 'application/json' - return json
     if re.search(REGEX_APPJSON, request.headers.get("accept", "")):
         response.status = code
         return json.dumps(context)
     # else - return html error-page
     content = ERROR_PAGES.get(code) or ERROR_PAGES["*"]
     return render(content=content, context=context, delimiters="[[ ]]")
 
 
 @bottle.error(404)
-def error404(error):
+def error404(error):  # pylint: disable=unused-argument
+    """Generates a 404 page"""
     guess_app_name = (
         "index"
         if request.environ.get("HTTP_X_PY4WEB_APPNAME")
         else request.path.split("/")[1]
     )
     if guess_app_name == "index":
         href = "/"
@@ -1459,57 +1572,61 @@
 def sass_compile(changed_files):
     print(changed_files); # paths of files that changed, for info
     sass.compile()
 """
 
 
 def app_watch_handler(watched_app_subpaths):
+    """Finds files to watch for changes"""
     stack = inspect.stack
     invoker = pathlib.Path(stack()[1].filename)
     apps_path = pathlib.Path(os.environ["PY4WEB_APPS_FOLDER"])
     app = invoker.relative_to(os.environ["PY4WEB_APPS_FOLDER"]).parts[0]
 
     def decorator(func):
-        handler = "{}.{}".format(func.__module__, func.__name__)
+        handler = f"{func.__module__}.{func.__name__}"
         APP_WATCH["handlers"][handler] = func
         for subpath in watched_app_subpaths:
             app_path = apps_path.joinpath(app, subpath).as_posix()
             if app_path not in APP_WATCH["files"]:
                 APP_WATCH["files"][app_path] = []
             APP_WATCH["files"][app_path].append(handler)
         return func
 
     return decorator
 
 
 def try_app_watch_tasks():
+    """If there are watch tasks, executes them when files change"""
     if APP_WATCH["tasks"]:
         tried_tasks = []
         for handler in APP_WATCH["tasks"]:
             changed_files_dict = APP_WATCH["tasks"][handler]
             try:
                 APP_WATCH["handlers"][handler](changed_files_dict.keys())
                 tried_tasks.append(handler)
-            except Exception:
+            except Exception:  # pylint: disable=broad-exception-caught
                 logging.error(traceback.format_exc())
         ## remove executed tasks from register
         for handler in tried_tasks:
             del APP_WATCH["tasks"][handler]
 
 
 def watch(apps_folder, server_config, mode="sync"):
+    """Watches files for change"""
+
     def watch_folder_event_loop(apps_folder):
+        """Main event loop looking for file changes"""
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
         loop.run_until_complete(watch_folder(apps_folder))
 
     async def watch_folder(apps_folder):
-        click.echo(
-            "watching (%s-mode) python file changes in: %s" % (mode, apps_folder)
-        )
+        """Async function that watches a folder for changes"""
+        click.echo(f"watching ({mode}-mode) python file changes in: {apps_folder}")
         async for changes in awatch(os.path.join(apps_folder)):
             apps = []
             for subpath in [pathlib.Path(pair[1]) for pair in changes]:
                 name = subpath.relative_to(apps_folder).parts[0]
                 if subpath.suffix == ".py":
                     apps.append(name)
                 ## manage `app_watch_handler` decorators
@@ -1528,15 +1645,16 @@
             ## in 'lazy' mode it's done in bottle's 'before_request' hook
             if mode != "lazy":
                 try_app_watch_tasks()
 
     if server_config["number_workers"] > 1:
         click.echo("--watch option has no effect in multi-process environment \n")
         return
-    elif server_config["server"].startswith(("wsgiref", "waitress", "rocket")):
+
+    if server_config["server"].startswith(("wsgiref", "waitress", "rocket")):
         # these servers block the main thread so we open a new thread for the file watcher
         threading.Thread(
             target=watch_folder_event_loop, args=(apps_folder,), daemon=True
         ).start()
     elif server_config["server"] == "tornado":
         if server_config["platform"] == "windows" and sys.version_info >= (3, 8):
             # see  https://bugs.python.org/issue37373 FIX: tornado/py3.8 on window
@@ -1550,32 +1668,34 @@
         return
 
     if mode == "lazy":
         Reloader.install_reloader_hook()
 
 
 def log_routes(apps_routes, out_file="routes-py4web.txt"):
+    """Logs defined routes to a file"""
     tmp = os.environ.get("TEMPDIR", "/tmp")
     path_out_file = os.path.join(tmp, out_file)
     try:
-        with open(path_out_file, "w") as f:
+        with open(path_out_file, "w", encoding="utf8") as f:
             f.write(
                 "\n".join(
                     [
                         v.rule if "\r" in k else ("/" + k)
                         for k, v in sorted(apps_routes.items())
                     ]
                 )
             )
         print(f"{len(apps_routes)} routes written to {path_out_file}")
     except OSError as ex:
         sys.exit(ex)
 
 
 def start_server(kwargs):
+    """Starts the web server"""
     host = kwargs["host"]
     port = int(kwargs["port"])
     apps_folder = kwargs["apps_folder"]
     number_workers = kwargs["number_workers"]
     quiet = kwargs["quiet"]
     logging_level = kwargs["logging_level"]
     params = dict(
@@ -1597,19 +1717,17 @@
             server_config["server"] = "gunicorn"
 
     # Catch interrupts like Ctrl-C if needed
     if server_config["server"] not in {"rocketServer", "wsgirefWsTwistedServer"}:
         signal.signal(
             signal.SIGINT,
             lambda signal, frame: click.echo(
-                "KeyboardInterrupt (ID: {}) has been caught. Cleaning up...".format(
-                    signal
-                )
-                and sys.exit(0),
-            ),
+                "KeyboardInterrupt (ID: {signal}) has been caught. Cleaning up..."
+            )
+            and sys.exit(0),
         )
 
     params["server"] = server_config["server"]
     if params["server"] in server_adapters.__all__:
         params["server"] = getattr(server_adapters, params["server"])()
     if number_workers > 1:
         params["workers"] = number_workers
@@ -1619,34 +1737,36 @@
         params["certfile"] = kwargs["ssl_cert"]
         params["keyfile"] = kwargs["ssl_key"]
 
     if server_config["server"] == "gevent":
         if kwargs["watch"] != "off":
             print("Error: watch doesn't work with gevent. ")
             print("invoke py4web with `--watch off` or choose another server. ")
-            exit(255)
+            sys.exit(255)
 
         if not hasattr(_ssl, "sslwrap"):
             _ssl.sslwrap = new_sslwrap
 
+    register_hooks()
+
     if kwargs["watch"] != "off":
         watch(apps_folder, server_config, kwargs["watch"])
 
     if kwargs["routes"]:
         log_routes(bottle.default_app().routes)
 
     bottle.run(**params)
 
 
-def check_compatible(version):
+def check_compatible(py4web_version):
     """To be called by apps to check if module version is compatible with py4web requirements"""
-    from . import __version__
+    from . import __version__  # pylint: disable=import-outside-toplevel
 
     return tuple(map(int, __version__.split("."))) >= tuple(
-        map(int, version.split("."))
+        map(int, py4web_version.split("."))
     )
 
 
 #########################################################################################
 # WSGI Adapter
 #########################################################################################
 
@@ -1672,70 +1792,76 @@
         assert pkg
         if pkg != pkg_alias:
             self.pkg_alias = pkg_alias
             self.pkg = pkg
             # register as path finder
             sys.meta_path.append(self)
 
-    def find_spec(self, fullname, path=None, target=None):
+    def find_spec(self, fullname, path=None):
+        """Loads the spec for the module at fullname"""
         if fullname == self.pkg_alias and path is None:
             spec = importlib.util.find_spec(self.pkg)
             if spec:
                 spec.name = fullname
                 spec.loader = importlib.machinery.SourceFileLoader(
                     fullname, spec.origin
                 )
                 return spec
+        return None
 
 
-def install_args(kwargs, reinstall_apps=False):
+def install_args(kwargs, reinstall_apps=False):  # pylint: disable=too-many-statements
+    """Handles the command line argumens and adds them to the os.environ"""
     # always convert apps_folder to an absolute path
     apps_folder = kwargs["apps_folder"] = os.path.abspath(kwargs["apps_folder"])
     kwargs["service_folder"] = os.path.join(
         kwargs["apps_folder"], DEFAULTS["PY4WEB_SERVICE_FOLDER"]
     )
     kwargs["service_db_uri"] = DEFAULTS["PY4WEB_SERVICE_DB_URI"]
     for key, val in kwargs.items():
         os.environ["PY4WEB_" + key.upper()] = str(val)
-    Fixture.__fixture_debug__ = kwargs.get("debug", False)
+
+    global DEBUG  # pylint: disable=global-statement
+    DEBUG = kwargs.get("debug", False)
+
     logging.getLogger().setLevel(
-        0 if Fixture.__fixture_debug__ else kwargs.get("logging_level", logging.WARNING)
+        0 if DEBUG else kwargs.get("logging_level", logging.WARNING)
     )
     yes2 = yes = kwargs.get("yes", False)
     # If the apps folder does not exist create it and populate it
     if not os.path.exists(apps_folder):
-        if yes or click.confirm("Create missing folder %s?" % apps_folder):
+        if yes or click.confirm(f"Create missing folder {apps_folder}?"):
             os.makedirs(apps_folder)
             yes2 = True
         else:
             click.echo("Command aborted")
             sys.exit(0)
     init_py = os.path.join(apps_folder, "__init__.py")
     if not os.path.exists(init_py):
-        if yes2 or click.confirm("Create missing init file %s?" % init_py):
+        if yes2 or click.confirm(f"Create missing init file {init_py}?"):
             with open(init_py, "wb"):
-                pass
+                ...
         else:
             click.echo("Command aborted")
             sys.exit(0)
     # ensure that "import apps.someapp" works
     apps_folder_parent, apps_folder_name = os.path.split(apps_folder)
     if apps_folder_parent not in sys.path:
         sys.path.insert(0, apps_folder_parent)
     if apps_folder_name != "apps":
         MetaPathRouter(apps_folder_name)
 
     if not os.path.exists(kwargs["service_folder"]):
         os.mkdir(kwargs["service_folder"])
     session_secret_filename = os.path.join(kwargs["service_folder"], "session.secret")
     if not os.path.exists(session_secret_filename):
-        with open(session_secret_filename, "w") as fp:
+        with open(session_secret_filename, "w", encoding="utf8") as fp:
             fp.write(str(uuid.uuid4()))
 
-    with open(session_secret_filename) as fp:
+    with open(session_secret_filename, "r", encoding="utf8") as fp:
         Session.SECRET = fp.read()
 
     # after everything is etup but before installing apps, init
     error_logger.initialize()
 
     # Reinstall apps from zipped ones in assets
     if reinstall_apps:
@@ -1745,16 +1871,16 @@
             for filename in apps:
                 zip_filename = os.path.join(assets_dir, filename)
                 # These filenames do not necessarily exist if one has
                 # downloaded from source and deleted them.
                 app_name = filename.split(".")[-2]
                 target_dir = os.path.join(apps_folder, app_name)
                 if not os.path.exists(target_dir):
-                    if yes or click.confirm("Create app %s?" % app_name):
-                        click.echo("[ ] Unzipping app %s" % filename)
+                    if yes or click.confirm(f"Create app {app_name}?"):
+                        click.echo(f"[ ] Unzipping app {filename}")
                         with zipfile.ZipFile(zip_filename, "r") as zip_file:
                             os.makedirs(target_dir)
                             zip_file.extractall(target_dir)
                             click.echo("\x1b[A[X]")
 
 
 def wsgi(**kwargs):
@@ -1767,36 +1893,36 @@
 #########################################################################################
 # CLI
 #########################################################################################
 
 
 @click.group(
     context_settings=dict(help_option_names=["-h", "-help", "--help"]),
-    help='%s\n\nType "%s COMMAND -h" for available options on commands'
-    % (__doc__, PY4WEB_CMD),
+    help=f'{__doc__}\n\nType "{PY4WEB_CMD} COMMAND -h" for available options on commands',
 )
 def cli():
-    pass
+    """The Command Line Interface"""
 
 
 @cli.command()
 @click.option(
     "-a", "--all", is_flag=True, default=False, help="List version of all modules"
 )
-def version(all):
+def version(verbose=False):
     """Show versions and exit"""
-    from . import __version__
+    from . import __version__  # pylint: disable=import-outside-toplevel
 
-    click.echo("py4web: %s" % __version__)
-    if all:
-        click.echo("system: %s" % platform.platform())
-        click.echo("python: %s" % sys.version.replace("\n", " "))
+    click.echo(f"py4web: {__version__}")
+    if verbose:
+        sys_version = sys.version.replace("\n", " ")
+        click.echo(f"system: {platform.platform()}")
+        click.echo(f"python: {sys_version}")
         for name in sorted(sys.modules):
             if hasattr(sys.modules[name], "__version__"):
-                click.echo("%s: %s" % (name, sys.modules[name].__version__))
+                click.echo(f"{name}: {sys.modules[name].__version__}")
 
 
 @cli.command()
 @click.argument("apps_folder")
 @click.option(
     "-Y",
     "--yes",
@@ -1820,15 +1946,15 @@
     help="No prompt, assume yes to questions",
     show_default=True,
 )
 def shell(**kwargs):
     """Open a python shell with apps_folder's parent added to the path"""
     if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
         # running in the PyInstaller binary bundle
-        import site  # noqa: F401
+        import site  # pylint: disable=possibly-unused-variable,import-outside-toplevel
     install_args(kwargs)
     code.interact(local=dict(globals(), **locals()))
 
 
 @cli.command()
 @click.argument("apps_folder", type=click.Path(exists=True))
 @click.argument("func")
@@ -1848,17 +1974,17 @@
 )
 def call(apps_folder, func, yes, args):
     """Call a function inside apps_folder"""
     kwargs = json.loads(args)
     install_args(dict(apps_folder=apps_folder, yes=yes))
     apps_folder_name = os.path.basename(os.environ["PY4WEB_APPS_FOLDER"])
     app_name = func.split(".")[0]
-    module, name = ("%s.%s" % (apps_folder_name, func)).rsplit(".", 1)
+    module, name = f"{apps_folder_name}.{func}".rsplit(".", 1)
     env = {}
-    exec("from %s import %s" % (module, name), {}, env)
+    exec(f"from {module} import {name}", {}, env)  # pylint: disable=exec-used
     request.app_name = app_name
     env[name](**kwargs)
 
 
 @cli.command(name="set_password")
 @click.option(
     "--password",
@@ -1872,16 +1998,16 @@
     "--password_file",
     default="password.txt",
     help="File for the encrypted password",
     show_default=True,
 )
 def set_password(password, password_file):
     """Set administrator's password for the Dashboard"""
-    click.echo('Storing the hashed password in file "%s"\n' % password_file)
-    with open(password_file, "w") as fp:
+    click.echo(f'Storing the hashed password in file "{password_file}"\n')
+    with open(password_file, "w", encoding="utf8") as fp:
         fp.write(str(pydal.validators.CRYPT()(password)[0]))
 
 
 @cli.command(name="new_app")
 @click.argument("apps_folder")
 @click.argument("app_name")
 @click.option(
@@ -1903,23 +2029,22 @@
     """Create a new app copying the scaffolding one"""
     install_args(dict(apps_folder=apps_folder, yes=yes))
     source = scaffold_zip or os.path.join(
         os.path.dirname(__file__), "assets", "py4web.app._scaffold.zip"
     )
     target_dir = os.path.join(os.environ["PY4WEB_APPS_FOLDER"], app_name)
     if not os.path.exists(source):
-        click.echo("Source app %s does not exists" % source)
+        click.echo(f"Source app {source} does not exists")
         sys.exit(1)
     elif os.path.exists(target_dir):
-        click.echo("Target folder %s already exists" % target_dir)
+        click.echo(f"Target folder {target_dir} already exists")
         sys.exit(1)
     else:
-        zfile = zipfile.ZipFile(source, "r")
-        zfile.extractall(target_dir)
-        zfile.close()
+        with zipfile.ZipFile(source, "r") as zfile:
+            zfile.extractall(target_dir)
 
 
 @cli.command()
 @click.argument("apps_folder", type=click.Path(exists=True))
 @click.option(
     "-Y",
     "--yes",
@@ -2022,34 +2147,38 @@
 @click.option(
     "-U",
     "--url_prefix",
     default="",
     help="Prefix to add to all URLs in and out",
     show_default=True,
 )
+@click.option(
+    "-m",
+    "--mode",
+    default="default",
+    help="default or development",
+    show_default=True,
+)
 def run(**kwargs):
     """Run the applications on apps_folder"""
     install_args(kwargs)
 
-    from py4web import __version__
-
     click.secho(ART, fg="blue")
-    click.echo("Py4web: %s on Python %s\n\n" % (__version__, sys.version))
+    click.echo(f"Py4web: {version} on Python {sys.version}\n\n")
 
     # Start
     Reloader.import_apps()
 
     # If we know where the password is stored, read it, otherwise ask for one
     if os.path.exists(os.path.join(os.environ["PY4WEB_APPS_FOLDER"], "_dashboard")):
         if kwargs["dashboard_mode"] not in ("demo", "none") and not os.path.exists(
             kwargs["password_file"]
         ):
             click.echo(
-                'You have not set a dashboard password. Run "%s set_password" to do so.'
-                % PY4WEB_CMD
+                f'You have not set a dashboard password. Run "{PY4WEB_CMD} set_password" to do so.'
             )
         elif "_dashboard" in Reloader.ROUTES and (
             not kwargs["host"].startswith("unix:/")
         ):
             click.echo(
                 f"Dashboard is at: http{'s' if kwargs.get('ssl_cert', None) else ''}://{kwargs['host']}:{kwargs['port']}/_dashboard"
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py4web-1.20240509.1/py4web/server_adapters.py` & `py4web-1.20240528.1/py4web/server_adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,16 @@
     try:
         return opts["workers"] if opts["workers"] else default
     except KeyError:
         return default
 
 
 def check_port(host="127.0.0.1", port=8000):
-    import socket
     import errno
+    import socket
     import subprocess
 
     def os_cmd(run_cmd):
         try:
             subprocess.run(
                 run_cmd,
                 shell=True,
@@ -173,17 +173,18 @@
     s.close()
 
 
 # ---------------------- servers -----------------------------------------------
 
 
 def gunicorn():
-    from gevent import local  # pip install gevent gunicorn setproctitle
     import threading
 
+    from gevent import local  # pip install gevent gunicorn setproctitle
+
     if isinstance(threading.local(), local.local):
         print("gunicorn: monkey.patch_all() applied")
 
     class GunicornServer(ServerAdapter):
         def run(self, app_handler):
             try:
                 from gunicorn.app.base import Application
@@ -382,15 +383,14 @@
             server.serve_forever()
 
     return GeventServer
 
 
 def geventWebSocketServer():
     from gevent import pywsgi
-
     # from geventwebsocket.handler import WebSocketHandler # pip install gevent-websocket
     from gevent_ws import WebSocketHandler  # pip install gevent gevent-ws
 
     # https://stackoverflow.com/questions/5312311/secure-websockets-with-self-signed-certificate
     # https://pypi.org/project/gevent-ws/
     # ./py4web.py run apps -s geventWebSocketServer --watch=off --ssl_cert=server.pem -H 192.168.1.161 -P 9000 -L 10
     # vi apps/_websocket/templates/index.html    set: ws, wss, host, port
@@ -441,15 +441,16 @@
 
 def wsgirefThreadingServer():
     # https://www.electricmonk.nl/log/2016/02/15/multithreaded-dev-web-server-for-the-python-bottle-web-framework/
 
     import socket
     from concurrent.futures import ThreadPoolExecutor  # pip install futures
     from socketserver import ThreadingMixIn
-    from wsgiref.simple_server import WSGIRequestHandler, WSGIServer, make_server
+    from wsgiref.simple_server import (WSGIRequestHandler, WSGIServer,
+                                       make_server)
 
     class WSGIRefThreadingServer(ServerAdapter):
         def run(self, app_handler):
 
             self.log = None
 
             if not self.quiet:
```

### Comparing `py4web-1.20240509.1/py4web/utils/auth.py` & `py4web-1.20240528.1/py4web/utils/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,16 @@
 import datetime
 import hashlib
 import random
 import re
 import time
 import uuid
 
-from pydal.validators import (
-    CRYPT,
-    IS_EMAIL,
-    IS_EQUAL_TO,
-    IS_MATCH,
-    IS_NOT_EMPTY,
-    IS_NOT_IN_DB,
-    IS_STRONG,
-)
+from pydal.validators import (CRYPT, IS_EMAIL, IS_EQUAL_TO, IS_MATCH,
+                              IS_NOT_EMPTY, IS_NOT_IN_DB, IS_STRONG)
 from yatl.helpers import DIV, A
 
 from py4web import HTTP, URL, Field, action, redirect, request, response
 from py4web.core import REGEX_APPJSON, Fixture, Flash, Translator
 from py4web.utils.form import Form, FormStyleDefault
 from py4web.utils.param import Param
```

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from . import OAuth2
 import requests
 
+from . import OAuth2
+
 
 class OAuth2Facebook(OAuth2):
     name = "oauth2facebook"
     label = "Facebook"
 
     login_url = "https://www.facebook.com/v3.3/dialog/oauth"
     token_url = "https://graph.facebook.com/v3.3/oauth/access_token"
```

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/pam.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,16 @@
 Provides an authenticate function that will allow the caller to authenticate
 a user against the Pluggable Authentication Modules (PAM) on the system.
 Implemented using ctypes, so no compilation is necessary.
 """
 __all__ = ["authenticate"]
 
 import sys
-from ctypes import (
-    CDLL,
-    CFUNCTYPE,
-    POINTER,
-    Structure,
-    byref,
-    c_char,
-    c_char_p,
-    c_int,
-    c_uint,
-    c_void_p,
-    cast,
-    sizeof,
-)
+from ctypes import (CDLL, CFUNCTYPE, POINTER, Structure, byref, c_char,
+                    c_char_p, c_int, c_uint, c_void_p, cast, sizeof)
 from ctypes.util import find_library
 
 libpam = CDLL(find_library("pam"))
 libc = CDLL(find_library("c"))
 
 calloc = libc.calloc
 calloc.restype = c_void_p
```

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240528.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 Ported from web2py - Work in Pogress
 """
 
 from functools import reduce
 
 from gluon.globals import current
 from gluon.storage import Storage
-
 # requires M2Crypto
 from M2Crypto import X509
 
 
 class x509Plugin:
 
     name = "x509"
```

### Comparing `py4web-1.20240509.1/py4web/utils/cors.py` & `py4web-1.20240528.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/dbstore.py` & `py4web-1.20240528.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/downloader.py` & `py4web-1.20240528.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/factories.py` & `py4web-1.20240528.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/form.py` & `py4web-1.20240528.1/py4web/utils/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,16 @@
 import os
 import time
 import uuid
 
 import jwt
 from pydal._compat import to_native
 from pydal.objects import FieldVirtual
-from yatl.helpers import (
-    CAT,
-    DIV,
-    FORM,
-    INPUT,
-    LABEL,
-    OPTION,
-    SELECT,
-    SPAN,
-    TEXTAREA,
-    XML,
-    A,
-    P,
-)
+from yatl.helpers import (CAT, DIV, FORM, INPUT, LABEL, OPTION, SELECT, SPAN,
+                          TEXTAREA, XML, A, P)
 
 from py4web import HTTP, request, response
 from py4web.utils.param import Param
 
 
 def to_id(field):
     """get an identified for a field"""
```

### Comparing `py4web-1.20240509.1/py4web/utils/grid.py` & `py4web-1.20240528.1/py4web/utils/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,16 @@
 #
 import base64
 import copy
 import datetime
 from urllib.parse import urlparse
 
 from pydal.objects import Expression, Field, FieldVirtual
-from yatl.helpers import (
-    CAT,
-    DIV,
-    FORM,
-    INPUT,
-    OPTION,
-    SELECT,
-    SPAN,
-    TABLE,
-    TAG,
-    TBODY,
-    TD,
-    TH,
-    THEAD,
-    TR,
-    XML,
-    A,
-    I,
-)
+from yatl.helpers import (CAT, DIV, FORM, INPUT, OPTION, SELECT, SPAN, TABLE,
+                          TAG, TBODY, TD, TH, THEAD, TR, XML, A, I)
 
 from py4web import HTTP, URL, redirect, request, safely
 from py4web.utils.form import Form, FormStyleDefault, join_classes
 from py4web.utils.param import Param
 
 NAV = TAG.nav
 HEADER = TAG.header
@@ -400,15 +383,14 @@
 
     def render(self, row, index=None):
         """renders a row al position index (optional)"""
         return self.represent(row)
 
 
 class Grid:
-
     FORMATTERS_BY_TYPE = {
         "boolean": lambda value: (
             INPUT(_type="checkbox", _checked=value, _disabled="disabled")
             if value
             else ""
         ),
         "datetime": lambda value: (
@@ -420,35 +402,41 @@
                     value.day,
                     value.hour,
                     value.minute,
                     value.second,
                 )
             )
             if value and isinstance(value, datetime.datetime)
-            else value if value else ""
+            else value
+            if value
+            else ""
         ),
         "time": lambda value: (
             XML(
                 "<script>document.write((new Date(0, 0, 0,%s,%s,%s)).toLocaleString().split(', ')[1])</script>"
                 % (value.hour, value.minute, value.second)
             )
             if value and isinstance(value, datetime.time)
-            else value if value else ""
+            else value
+            if value
+            else ""
         ),
         "date": lambda value: (
             XML(
                 '<script>document.write((new Date(%s,%s,%s)).toLocaleString().split(",")[0])</script>'
                 % (
                     value.year,
                     value.month - 1,
                     value.day,
                 )
             )
             if value and isinstance(value, datetime.date)
-            else value if value else ""
+            else value
+            if value
+            else ""
         ),
         "list:string": lambda value: ", ".join(str(x) for x in value) if value else "",
         "list:integer": lambda value: ", ".join(x for x in value) if value else "",
         "default": lambda value: str(value) if value is not None else "",
     }
 
     def __init__(
@@ -723,15 +711,14 @@
         if self.action == "delete" and not self.is_deletable(record):
             raise HTTP(
                 403,
                 f"You do not have access to delete a record in the {self.tablename} table.",
             )
 
         if self.action in ["new", "details", "edit"]:
-
             readonly = self.action == "details"
 
             attrs = self.attributes_plugin.form(url=request.url.split(":", 1)[1])
             self.form = Form(
                 table,
                 record=record,
                 readonly=readonly,
@@ -754,18 +741,15 @@
             if self.action == "edit" and self.is_editable(record):
                 if self.param.edit_sidecar:
                     self.form.param.sidecar.append(self.param.edit_sidecar)
                 if self.param.edit_submit_value:
                     self.form.param.submit_value = self.param.edit_submit_value
 
             # redirect to the referrer
-            if (
-                self.form.accepted
-                or (readonly and request.method == "POST")
-            ):
+            if self.form.accepted or (readonly and request.method == "POST"):
                 referrer = request.query.get("_referrer")
                 if referrer:
                     redirect(base64.b16decode(referrer.encode("utf8")).decode("utf8"))
                 else:
                     redirect(self.endpoint)
 
         elif self.action == "delete" and self.is_deletable(record):
@@ -797,39 +781,38 @@
                 self.param.columns.append(pt._id)
                 self.param.show_id = False
 
             self.current_page_number = safe_int(request.query.get("page"), default=1)
 
             select_params = dict()
             #  try getting sort order from the request
-            sort_order = request.query.get("orderby", "")
+            sort_order = request.query.get("orderby")
 
-            try:
+            select_params["orderby"] = self.param.orderby
+            if sort_order:
                 parts = sort_order.lstrip("~").split(".")
-                orderby = db[parts[0]][parts[1]]
-                if sort_order.startswith("~"):
-                    orderby = ~orderby
-                select_params["orderby"] = orderby
-            except (IndexError, KeyError, TypeError, AttributeError):
-                select_params["orderby"] = self.param.orderby
+                if (
+                    len(parts) == 2
+                    and parts[0] in db.tables
+                    and parts[1] in db[parts[p]]
+                ):
+                    orderby = db[parts[0]][parts[1]]
+                    if sort_order.startswith("~"):
+                        orderby = ~orderby
+                    select_params["orderby"] = orderby
 
             if self.param.left:
                 select_params["left"] = self.param.left
 
             if self.param.groupby:
                 select_params["groupby"] = self.param.groupby
 
-            if self.param.groupby:
+            if self.param.groupby or self.param.left:
                 #  need groupby fields in select to get proper count
                 self.total_number_of_rows = len(
-                    db(query).select(*self.param.groupby, **select_params)
-                )
-            elif self.param.left:
-                # TODO: maybe this can be made more efficient
-                self.total_number_of_rows = len(
                     db(query).select(db[self.tablename].id, **select_params)
                 )
             else:
                 self.total_number_of_rows = db(query).count()
 
             #  if at a high page number and then filter causes less records to be displayed, reset to page 1
             if (
@@ -1217,19 +1200,23 @@
                 if isinstance(column, (Field, FieldVirtual)):
                     field = column
                     if field.readable and (field.type != "id" or self.param.show_id):
                         tr.append(self._make_field(row, field, index))
                 elif isinstance(column, Column):
                     classes = self.param.grid_class_style.classes.get(
                         column.td_class_style,
-                        self.param.grid_class_style.classes.get("grid-td"),
+                        column.td_class_style(row)
+                        if callable(column.td_class_style)
+                        else self.param.grid_class_style.classes.get("grid-td"),
                     )
                     style = self.param.grid_class_style.styles.get(
                         column.td_class_style,
-                        self.param.grid_class_style.styles.get("grid-td"),
+                        column.td_class_style(row)
+                        if callable(column.td_class_style)
+                        else self.param.grid_class_style.styles.get("grid-td"),
                     )
                     tr.append(
                         TD(
                             column.render(row, index),
                             **clean_sc(_class=classes, _style=style),
                         )
                     )
@@ -1397,15 +1384,14 @@
                     **attrs,
                 )
             )
             previous_page_number = page_number
         return pager
 
     def _make_table(self):
-
         html = DIV(**self.param.grid_class_style.get("grid-wrapper"))
         grid_header = DIV(**self.param.grid_class_style.get("grid-header"))
 
         #  build the New button if needed
         if self.param.create and self.param.create != "":
             if isinstance(self.param.create, str):
                 create_url = self.param.create
@@ -1647,34 +1633,32 @@
     fn = parent_field.name
 
     #  find the record id of the parent from the child table record
     if path:
         parts = path.split("/")
         record_id = parts[1] if len(parts) > 1 else None
         if record_id:
-            r = child_table(record_id)
-            if r:
-                parent_id = r[fn]
+            record = child_table(record_id)
+            if record:
+                parent_id = record[fn]
 
     #  not passed in, check in the form
     if not parent_id:
         parent_id = request.forms.get(fn)
 
     #  not found yet, check in the referer
     if not parent_id:
         referrer = request.query.get("_referrer")
         if referrer:
             kvp = base64.b16decode(referrer.encode("utf8")).decode("utf8")
             if "parent_id" in kvp:
                 parent_id = kvp.split("parent_id=")[1]
 
-    try:
+    if parent_id and "&" in parent_id:
         parent_id = parent_id.split("&")[0]
-    except Exception:
-        pass
 
     return parent_id
 
 
 class AttributesPlugin:
     def __init__(self, target_element=None):
         self.target_element = target_element
```

### Comparing `py4web-1.20240509.1/py4web/utils/jsonrpc.py` & `py4web-1.20240528.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/mailer.py` & `py4web-1.20240528.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/misc.py` & `py4web-1.20240528.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/populate.py` & `py4web-1.20240528.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/publisher.py` & `py4web-1.20240528.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/recaptcha.py` & `py4web-1.20240528.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/security.py` & `py4web-1.20240528.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/py4web/utils/url_signer.py` & `py4web-1.20240528.1/py4web/utils/url_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,14 @@
         self.key = key or Session.SECRET
         self.variables_to_sign = variables_to_sign or []
         self.signing_info = signing_info
         self.lifespan = lifespan
         assert "_signature" not in self.variables_to_sign
         self.algo = algo or hashlib.sha256
 
-    @property
-    def local(self):
-        return self._safe_local
-
     def on_request(self, context):
         """Creates the signing key if necessary."""
         if self.session is not None and self.session.get("_signature_key") is None:
             key = str(uuid.uuid1())
             self.session["_signature_key"] = key
             # Note that we CANNOT save the key in the URLsigner object,
             # because there is only one object -- it's not thread-local in
```

### Comparing `py4web-1.20240509.1/py4web.egg-info/PKG-INFO` & `py4web-1.20240528.1/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240509.1
+Version: 1.20240528.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -191,8 +191,8 @@
 - `John M. Wolf <https://github.com/jmwolff3>`__
 - `Micah Beasley <https://github.com/MBfromOK>`__
 - `Nico Zanferrari <https://github.com/nicozanf>`__
 - `Pirsch <https://github.com/Pirsch>`__
 - `sugizo <https://github.com/sugizo>`__
 - `valq7711 <https://github.com/valq7711>`__
 - `Kevin Keller <https://github.com/Kkeller83>`__
-- `Sam de Alfaro <sam@dealfaro.com>`__ (logo design)
+- Sam de Alfaro sam@dealfaro.com (logo design)
```

### Comparing `py4web-1.20240509.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20240528.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240509.1/pyproject.toml` & `py4web-1.20240528.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "py4web"
-version = "1.20240509.1"
+version = "1.20240528.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
       "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = {file = "requirements.txt"}
 
-[tool.setuptools]    
+[tool.setuptools]
 packages = ["py4web", "py4web.utils", "py4web.utils.auth_plugins",]
 
 [tool.setuptools.package-data]
 py4web = ["assets/*"]
 
 [project.scripts]
 py4web = "py4web.core:cli"
```

### Comparing `py4web-1.20240509.1/tests/test_action.py` & `py4web-1.20240528.1/tests/test_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,58 @@
+# pylint: disable=assignment-from-none
 import copy
 import multiprocessing
 import os
+import threading
 import time
 import unittest
 import uuid
 
 import mechanize
 import requests
 
-from py4web import abort, action, DAL, Field, Session, Cache, HTTP, Condition
-from py4web.core import bottle, request, error404, Fixture
+from py4web import DAL, HTTP, Cache, Condition, Field, Session, abort, action
+from py4web.core import Fixture, bottle, error404, request
 
 os.environ["PY4WEB_APPS_FOLDER"] = os.path.sep.join(
     os.path.normpath(__file__).split(os.path.sep)[:-2]
 )
 
+SECRET = str(uuid.uuid4())
 db = DAL("sqlite://storage_%s" % uuid.uuid4(), folder="/tmp/")
 db.define_table("thing", Field("name"))
-session = Session(secret="my secret")
+session = Session(secret=SECRET)
 cache = Cache()
 
 action.app_name = "tests"
 
 
 @action("index")
 @cache.memoize(expiration=1)
 @action.uses(db, session)
 @action.uses(Condition(lambda: True))
 def index():
-    db.thing.insert(name="test")
+    new_id = db.thing.insert(name="test")
     session["number"] = session.get("number", 0) + 1
 
     # test copying Field ThreadSafe attr
     db.thing.name.default = "test_clone"
-    field_clone = copy.copy(db.thing.name)
-    clone_ok = 1 if field_clone.default == db.thing.name.default == "test_clone" else 0
-    return "ok %s %s %s" % (session["number"], db(db.thing).count(), clone_ok)
+    return "ok %s %s %s" % (session["number"], db(db.thing).count(), new_id)
+
 
 def fail():
     raise HTTP(404)
 
+
 @action("conditional")
 @action.uses(Condition(lambda: False, on_false=fail))
 def conditional():
     return "OK"
 
+
 @action("raise300")
 def raise300():
     raise HTTP(300)
 
 
 @action("bottle_httpresponse")
 def bottle_httpresponse():
@@ -68,22 +72,36 @@
 
 
 corrector = Corrector()
 
 
 @action("abort_caught")
 @action.uses(corrector)
-def abort_response():
+def abort_response_corrected():
     abort(400)
 
 
 def run_server():
     bottle.run(host="localhost", port=8001)
 
 
+class FieldTest(unittest.TestCase):
+    """Check that we chat we can safely clone Field(s)"""
+
+    def test_fiel_clone(self):
+        def test():
+            db.thing.name.default = "test"
+            field_clone = copy.copy(db.thing.name)
+            assert field_clone.default == db.thing.name.default == "test"
+
+        thread = threading.Thread(target=test)
+        thread.start()
+        thread.join()
+
+
 class CacheAction(unittest.TestCase):
     def setUp(self):
         self.server = multiprocessing.Process(target=run_server)
         self.server.start()
         self.browser = mechanize.Browser()
         time.sleep(3)
 
@@ -96,36 +114,35 @@
 
         res = self.browser.open("http://127.0.0.1:8001/tests/index")
         self.assertEqual(res.read(), b"ok 1 1 1")
 
         time.sleep(2)
 
         res = self.browser.open("http://127.0.0.1:8001/tests/index")
-        self.assertEqual(res.read(), b"ok 2 2 1")
+        self.assertEqual(res.read(), b"ok 2 2 2")
 
     def test_error(self):
-        res = requests.get("http://127.0.0.1:8001/tests/conditional")
+        res = requests.get("http://127.0.0.1:8001/tests/conditional", timeout=5)
         self.assertEqual(res.status_code, 404)
 
-        res = requests.get("http://127.0.0.1:8001/tests/raise300")
+        res = requests.get("http://127.0.0.1:8001/tests/raise300", timeout=5)
         self.assertEqual(res.status_code, 300)
 
-        res = requests.get("http://127.0.0.1:8001/tests/abort")
+        res = requests.get("http://127.0.0.1:8001/tests/abort", timeout=5)
         self.assertEqual(res.status_code, 400)
 
-        res = requests.get("http://127.0.0.1:8001/tests/abort_caught")
+        res = requests.get("http://127.0.0.1:8001/tests/abort_caught", timeout=5)
         self.assertEqual(res.status_code, 200)
         self.assertEqual(res.content, b"caught")
 
-        res = requests.get("http://127.0.0.1:8001/tests/bottle_httpresponse")
+        res = requests.get("http://127.0.0.1:8001/tests/bottle_httpresponse", timeout=5)
         self.assertEqual(res.status_code, 200)
         self.assertEqual(res.content, b"ok")
 
     def test_local(self):
         # for test coverage
         request.app_name = "example"
-        Session.__init_request_ctx__()  # mimic before_request-hook
         index()
 
     def test_error_page(self):
         request.path = "hello/world"
         self.assertTrue("NOT FOUND" in error404("oops"))
```

### Comparing `py4web-1.20240509.1/tests/test_auth.py` & `py4web-1.20240528.1/tests/test_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,61 @@
+import io
 import os
 import unittest
-from py4web.core import Session, DAL, request, HTTP, Field, bottle, _before_request
+import uuid
+
+from py4web.core import DAL, HTTP, Field, Fixture, Session, bottle, request, safely
 from py4web.utils.auth import Auth, AuthAPI
 
+SECRET = str(uuid.uuid4())
+
 
 class TestAuth(unittest.TestCase):
     def setUp(self):
         os.environ["PY4WEB_APPS_FOLDER"] = "apps"
-        _before_request()  # mimic before_request bottle-hook
         self.db = DAL("sqlite:memory")
-        self.session = Session(secret="a", expiration=10)
-        self.session.initialize()
+        self.session = Session(secret=SECRET, expiration=10)
         self.auth = Auth(
             self.session, self.db, define_tables=True, password_complexity=None
         )
         self.auth.enable()
         self.auth.action = self.action
         request.app_name = "_scaffold"
 
     def tearDown(self):
+        # this is normally done by @action
+        safely(lambda: Fixture.local_delete(self.session))
         bottle.app.router.remove("/*")
 
     def action(self, name, method, query, data):
         request.environ["REQUEST_METHOD"] = method
         request.environ["ombott.request.query"] = query
         request.environ["ombott.request.json"] = data
+        request.environ["wsgi.input"] = io.BytesIO()
         # we break a symmetry below. should fix in auth.py
         if name.startswith("api/"):
             return getattr(AuthAPI, name[4:])(self.auth)
-        else:
-            return getattr(self.auth.form_source, name)()
-
-    def on_request(self, context={}, keep_session=False):
-        storage = self.session._safe_local
+        return getattr(self.auth.form_source, name)()
 
-        # mimic before_request bottle-hook
-        _before_request()
-
-        # mimic action.uses()
-        self.session.initialize()
+    def on_request(self, context=None, keep_session=False):
+        # store the current session
+        context = context or {}
+        try:
+            storage = self.session.local.__dict__
+        except RuntimeError:
+            storage = None
+        # reinitialize everything
+        safely(lambda: Fixture.local_delete(self.session))
+        safely(lambda: Fixture.local_delete(self.auth.flash))
+        self.session.on_request(context)
         self.auth.flash.on_request(context)
         self.auth.on_request(context)
-        if keep_session:
-            self.session._safe_local = storage
+        # restore the previous session
+        if keep_session and storage:
+            self.session.local.__dict__.update(storage)
 
     def test_extra_fields(self):
         db = DAL("sqlite:memory")
         self.auth = Auth(
             self.session, db, define_tables=True, extra_fields=[Field("favorite_color")]
         )
         self.on_request()
@@ -69,15 +78,15 @@
                 "status": "error",
                 "message": "validation errors",
                 "code": 401,
             },
         )
 
     def test_register(self):
-        self.on_request()        
+        self.on_request()
         body = {
             "username": "ppallino",
             "email": "pinco.pallino@example.com",
             "password": "123456789",
             "first_name": "Pinco",
             "last_name": "Pallino",
         }
@@ -93,15 +102,14 @@
         body = {"email": "pinco.pallino@example.com", "password": "1234567"}
         self.assertEqual(
             self.auth.action("api/login", "POST", {}, body),
             {"status": "error", "message": "Invalid Credentials", "code": 400},
         )
 
         self.on_request()
-        self.on_request()
         body = {"email": "pinco.pallino@example.com", "password": "123456789"}
         self.assertEqual(
             self.auth.action("api/login", "POST", {}, body),
             {"status": "error", "message": "Registration is pending", "code": 400},
         )
 
         self.on_request()
```

### Comparing `py4web-1.20240509.1/tests/test_cache.py` & `py4web-1.20240528.1/tests/test_cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,52 +14,54 @@
         self.assertEqual(cache.head, cache.tail.prev.prev)
         self.assertEqual(cache.head.next.key, "x")
         self.assertEqual(cache.head.next.value, "y")
 
     def test_different_keys(self):
         cache = py4web.Cache()
         results = set()
-        for k in range(100):
+        for _ in range(100):
             results.add(cache.get("a", random.random))
             results.add(cache.get("b", random.random))
             results.add(cache.get("c", random.random))
         self.assertEqual(len(results), 3)
 
     def test_change_detection(self):
         cache = py4web.Cache()
         results = set()
         for k in range(30):
             results.add(
-                cache.get("a", random.random, expiration=0, monitor=lambda: int(k / 10))
+                cache.get(
+                    "a", random.random, expiration=0, monitor=lambda k=k: int(k / 10)
+                )
             )
         self.assertEqual(len(results), 3)
         time.sleep(0.02)
         results.add(cache.get("a", random.random, expiration=0.01, monitor=lambda: 5))
         self.assertEqual(len(results), 4)
 
     def test_timing(self):
         M = N = 100000
         cache = py4web.Cache()
         for k in range(M):
             cache.get(k, random.random)
         t0 = time.time()
-        for k in range(N):
+        for _ in range(N):
             cache.get("new", random.random)
         self.assertTrue((time.time() - t0) / N, 1 - 5)
         self.assertTrue(cache.free == 0)
 
     def test_memoize_and_expiration(self):
         memoize = py4web.Cache().memoize(expiration=0.1)
 
         @memoize
         def f(x):
             return x + random.random()
 
         results = set()
-        for k in range(10):
+        for _ in range(10):
             results.add(f(1))
             results.add(f(2))
         time.sleep(0.2)
-        for k in range(10):
+        for _ in range(10):
             results.add(f(1))
             results.add(f(2))
         self.assertEqual(len(results), 4)
```

### Comparing `py4web-1.20240509.1/tests/test_fixture.py` & `py4web-1.20240528.1/tests/test_fixture.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-from types import SimpleNamespace
-import pytest
 import threading
-from py4web.core import Fixture
+import pytest
 
-result = {"seq": []}
+from py4web.core import Fixture
 
 
 def run_thread(func, *a):
     t = threading.Thread(target=func, args=a)
     return t
 
 
 class Foo(Fixture):
-    def on_request(self):
-        self._safe_local = SimpleNamespace()
+    def on_request(self, context):
+        Fixture.local_initialize(self)
 
     @property
     def bar(self):
-        return self._safe_local.a
+        return self.local.a
 
     @bar.setter
     def bar(self, a):
-        self._safe_local.a = a
+        self.local.a = a
 
 
+results = {}
 foo = Foo()
 
 
-def before_request():
-    Fixture.__init_request_ctx__()
-
-
 @pytest.fixture
 def init_foo():
     def init(key, a, evnt_done=None, evnt_play=None):
-        result["seq"].append(key)
-        before_request()
-        foo.on_request()
+        Fixture.local_initialize(foo)
         foo.bar = a
         evnt_done and evnt_done.set()
         evnt_play and evnt_play.wait()
-        result[key] = foo.bar
+        results[key] = foo.bar
+        Fixture.local_delete(foo)
         return foo
 
     return init
 
 
-def test_fixtute_local_storage(init_foo):
+def test_fixture_local_storage(init_foo):
     assert init_foo("t1", "a1") is foo
     evnt_done = threading.Event()
     evnt_play = threading.Event()
     t2 = run_thread(init_foo, "t2", "a2", evnt_done, evnt_play)
     t3 = run_thread(init_foo, "t3", "a3", None, None)
     t2.start()
     evnt_done.wait()
     t3.start()
     t3.join()
     evnt_play.set()
     t2.join()
-    assert foo.bar == "a1"
-    assert result["t2"] == "a2"
-    assert result["t3"] == "a3"
-    assert ",".join(result["seq"]) == "t1,t2,t3"
+    assert results["t1"] == "a1"
+    assert results["t2"] == "a2"
+    assert results["t3"] == "a3"
 
 
-def test_fixtute_error():
-    before_request()
+def test_fixture_error():
     # attempt to access _safe_local prop without on_request-call
     with pytest.raises(RuntimeError) as err:
         foo.bar
-    assert "py4web hint" in err.value.args[0]
+    assert "not initialized" in err.value.args[0]
     assert "Foo object" in err.value.args[0]
```

### Comparing `py4web-1.20240509.1/tests/test_form.py` & `py4web-1.20240528.1/tests/test_form.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import io
-import os
 import unittest
-from py4web import request, response, Field, Session
+import uuid
+
+from py4web import Field, Session, request, response
 from py4web.utils.form import Form
 
+SECRET = str(uuid.uuid4())
+
 
 class FormTest(unittest.TestCase):
     def setUp(self):
         request.environ["wsgi.input"] = io.BytesIO()
         request.cookies.clear()
         response._cookies = ""
 
     def test_form(self):
-        session = Session()
-        session.initialize()
+        session = Session(secret=SECRET)
+        session.on_request({})
         table = [Field("name")]
         form_name = "testing_form"
         f = Form(table, form_name=form_name, csrf_session=session)
         value = f.formkey
         post_vars = dict(_formname=form_name, _formkey=value)
         self.assertTrue(f._verify_form(post_vars))
+        session.on_success({})
```

### Comparing `py4web-1.20240509.1/tests/test_get_error_snapshot.py` & `py4web-1.20240528.1/tests/test_get_error_snapshot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os
 import unittest
+
 from py4web.core import get_error_snapshot
 
 
 class ErrorTest(unittest.TestCase):
     def test_get_error_snapshot(self):
         try:
             1 / 0
         except Exception:
             snapshot = get_error_snapshot()
             keys = list(sorted(snapshot.keys()))
-        self.assertEqual(
-            keys,
-            [
-                "exception_type",
-                "exception_value",
-                "os_environ",
-                "platform_info",
-                "python_version",
-                "stackframes",
-                "timestamp",
-                "traceback",
-            ],
-        )
+            self.assertEqual(
+                keys,
+                [
+                    "exception_type",
+                    "exception_value",
+                    "os_environ",
+                    "platform_info",
+                    "python_version",
+                    "stackframes",
+                    "timestamp",
+                    "traceback",
+                ],
+            )
```

### Comparing `py4web-1.20240509.1/tests/test_json.py` & `py4web-1.20240528.1/tests/test_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
+import fractions
 import json
 import unittest
-import fractions
 
 from py4web.core import dumps, objectify
 
 
 class TestJson(unittest.TestCase):
     def test_objectify(self):
         """Check if we can serialize objects, generators, and dates"""
 
-        class A(object):
+        class A:
             def __init__(self, x):
                 self.x = x
 
         def f(n):
             for k in range(n):
                 yield k + 1
```

### Comparing `py4web-1.20240509.1/tests/test_main.py` & `py4web-1.20240528.1/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
-import unittest
-import tempfile
 import signal
-from py4web.core import cli
+import tempfile
+import unittest
+
 from click.testing import CliRunner
 
+from py4web.core import cli
+
 
 def run_cli():
     dirpath = tempfile.mkdtemp()
     dir = os.path.join(dirpath, "apps")
     runner = CliRunner()
 
     testargs = ["setup", dir]
@@ -20,17 +22,14 @@
     res = runner.invoke(cli, testargs)
     if res.exception:
         raise res.exception
 
 
 class MainTest(unittest.TestCase):
     def test_main(self):
-        class MyException(Exception):
-            pass
-
         def handler(signum, frame):
             raise KeyboardInterrupt
 
         signal.signal(signal.SIGALRM, handler)
         signal.alarm(10)
         try:
             run_cli()
```

### Comparing `py4web-1.20240509.1/tests/test_tags.py` & `py4web-1.20240528.1/tests/test_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 from pydal import DAL, Field
 from pydal.tools.tags import Tags
 
 
 class TestTags(unittest.TestCase):
     def test_tags(self):
         db = DAL("sqlite:memory")
```

