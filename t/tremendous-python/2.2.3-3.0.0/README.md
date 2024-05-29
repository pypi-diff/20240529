# Comparing `tmp/tremendous-python-2.2.3.tar.gz` & `tmp/tremendous_python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tremendous-python-2.2.3.tar", last modified: Thu Nov 17 14:39:22 2022, max compression
+gzip compressed data, was "tremendous_python-3.0.0.tar", last modified: Wed May 29 13:35:44 2024, max compression
```

## Comparing `tremendous-python-2.2.3.tar` & `tremendous_python-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,157 @@
-drwxr-xr-x   0 nardelli   (501) staff       (20)        0 2022-11-17 14:39:22.201126 tremendous-python-2.2.3/
--rw-r--r--   0 nardelli   (501) staff       (20)     1105 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/LICENSE.txt
--rw-r--r--   0 nardelli   (501) staff       (20)      679 2022-11-17 14:39:22.201197 tremendous-python-2.2.3/PKG-INFO
--rw-r--r--   0 nardelli   (501) staff       (20)     1866 2022-05-26 18:37:28.000000 tremendous-python-2.2.3/README.md
--rw-r--r--   0 nardelli   (501) staff       (20)       79 2022-11-17 14:39:22.201545 tremendous-python-2.2.3/setup.cfg
--rw-r--r--   0 nardelli   (501) staff       (20)      994 2022-05-26 18:37:28.000000 tremendous-python-2.2.3/setup.py
-drwxr-xr-x   0 nardelli   (501) staff       (20)        0 2022-11-17 14:39:22.200006 tremendous-python-2.2.3/tremendous/
--rw-r--r--   0 nardelli   (501) staff       (20)      125 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/__init__.py
--rw-r--r--   0 nardelli   (501) staff       (20)      270 2022-11-16 22:01:02.000000 tremendous-python-2.2.3/tremendous/campaign.py
--rw-r--r--   0 nardelli   (501) staff       (20)      990 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/client.py
--rw-r--r--   0 nardelli   (501) staff       (20)      298 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/funding_source.py
--rw-r--r--   0 nardelli   (501) staff       (20)     3148 2022-11-17 14:33:33.000000 tremendous-python-2.2.3/tremendous/http.py
--rw-r--r--   0 nardelli   (501) staff       (20)      351 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/member.py
--rw-r--r--   0 nardelli   (501) staff       (20)      269 2022-11-17 14:33:33.000000 tremendous-python-2.2.3/tremendous/order.py
--rw-r--r--   0 nardelli   (501) staff       (20)      391 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/organization.py
--rw-r--r--   0 nardelli   (501) staff       (20)      168 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/product.py
--rw-r--r--   0 nardelli   (501) staff       (20)      182 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/reward.py
--rw-r--r--   0 nardelli   (501) staff       (20)       22 2022-11-17 14:33:33.000000 tremendous-python-2.2.3/tremendous/version.py
--rw-r--r--   0 nardelli   (501) staff       (20)      512 2022-05-26 16:41:06.000000 tremendous-python-2.2.3/tremendous/webhook.py
-drwxr-xr-x   0 nardelli   (501) staff       (20)        0 2022-11-17 14:39:22.201003 tremendous-python-2.2.3/tremendous_python.egg-info/
--rw-r--r--   0 nardelli   (501) staff       (20)      679 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/PKG-INFO
--rw-r--r--   0 nardelli   (501) staff       (20)      554 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/SOURCES.txt
--rw-r--r--   0 nardelli   (501) staff       (20)        1 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/dependency_links.txt
--rw-r--r--   0 nardelli   (501) staff       (20)        1 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/not-zip-safe
--rw-r--r--   0 nardelli   (501) staff       (20)       17 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/requires.txt
--rw-r--r--   0 nardelli   (501) staff       (20)       11 2022-11-17 14:39:22.000000 tremendous-python-2.2.3/tremendous_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.777372 tremendous_python-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 13:35:44.777372 tremendous_python-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 13:35:44.777372 tremendous_python-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.753372 tremendous_python-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_funding_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_invoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/test/test_products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.753372 tremendous_python-3.0.0/tremendous/
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.753372 tremendous_python-3.0.0/tremendous/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   476599 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/api/tremendous_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25977 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.773372 tremendous_python-3.0.0/tremendous/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_api_key200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_campaign201_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_campaign_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_invoice200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_invoice_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_member200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order200_response_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order200_response_order_rewards_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order200_response_order_rewards_inner_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order201_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order_request_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order_request_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order_request_reward_custom_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_order_request_reward_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_organization200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_organization200_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_organization_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_organization_request_copy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_webhook200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/create_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/currency_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/delivery_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/delivery_details_with_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/delivery_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/funding_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/generate_reward_link200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/generate_reward_link200_response_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/generate_reward_link403_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/generate_reward_token200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/generate_reward_token200_response_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_funding_source200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_member200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_member200_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_member200_response_member_events_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_organization200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/get_reward200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_balance_transactions200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_balance_transactions200_response_invoices_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_campaigns200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_campaigns200_response_campaigns_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_campaigns200_response_campaigns_inner_email_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_campaigns200_response_campaigns_inner_webpage_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_fields200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_fields200_response_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_funding_sources200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_funding_sources200_response_funding_sources_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_funding_sources200_response_funding_sources_inner_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_invoices200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_invoices200_response_invoices_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_members200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_members200_response_members_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_orders200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_orders200_response_orders_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_orders200_response_orders_inner_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_orders200_response_orders_inner_payment_refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_organizations200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_organizations200_response_organizations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_products_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_products_response_products_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_products_response_products_inner_countries_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_products_response_products_inner_images_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_products_response_products_inner_skus_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response_rewards_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response_rewards_inner_custom_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response_rewards_inner_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response_rewards_inner_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards200_response_rewards_inner_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards401_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards401_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_rewards429_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_webhook_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_webhooks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/list_webhooks200_response_webhooks_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/member_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/member_with_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/member_without_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_base_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_for_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_for_create_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_with_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_with_link_rewards_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_without_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/order_without_link_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/payment_details_refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/refund_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/resend_reward422_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_base_custom_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_for_order_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_with_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_with_link_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_without_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/reward_without_link_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/simulate_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/models/webhook_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 13:35:35.000000 tremendous_python-3.0.0/tremendous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:35:44.777372 tremendous_python-3.0.0/tremendous_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 13:35:44.000000 tremendous_python-3.0.0/tremendous_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-29 13:35:44.000000 tremendous_python-3.0.0/tremendous_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:35:44.000000 tremendous_python-3.0.0/tremendous_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 13:35:44.000000 tremendous_python-3.0.0/tremendous_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 13:35:44.000000 tremendous_python-3.0.0/tremendous_python.egg-info/top_level.txt
```

### Comparing `tremendous-python-2.2.3/LICENSE.txt` & `tremendous_python-3.0.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 The MIT License
 
 Copyright (c) 2018 Tremendous, Inc. <developers@tremendous.com>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `tremendous-python-2.2.3/README.md` & `tremendous_python-3.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,92 @@
-tremendous-python
-==============
+# Tremendous
 
-A python client library for the [Tremendous API][1].
+A Python client library for the [Tremendous API][docs].
+
+> [!NOTE]
+> This branch includes the v3 version of the Tremendous Python client, a new version based
+> on our [API schema][ref] docs. If you are using the v2 versions, please check our
+> [`UPGRADING`](UPGRADING.md) guide
 
 ## Installation
 
-```console
+```sh
 $ pip install tremendous-python
 ```
 
 ## Getting started
 
-All API requests require an access token.  A sandbox access token is assigned upon signup through the [Tremendous Dashboard][2]. Once you are ready to move to production, you will be assigned a production access token.
+All API requests require an access token.  A sandbox access token is assigned upon signup through the [Tremendous Sandbox Environment][docs]. Once you are ready to move to production, you will be assigned a production access token.
 
 ### Authentication
 
-```python
-from tremendous import Tremendous
-
-# Sandbox environment
-client = Tremendous("[SANDBOX_ACCESS_TOKEN]", "https://testflight.tremendous.com/api/v2")
 
-```
+```py
+from tremendous import Configuration, ApiClient, TremendousApi
 
-Campaigns are created within the dashboard by team admins.
-They define the catalog and presentation of your reward.
-API requests can always override these settings
-within the specific reward object by specifying the catalog, message, etc.
+# you can use `Configuration.Environment["production"]` when ready to use our production environment.
+configuration = Configuration(server_index=Configuration.Environment["testflight"], access_token="[SANDBOX_ACCESS_TOKEN]")
 
-```python
-campaigns = client.campaigns.list()
-campaign_id = campaigns[0]["id"]
+api = ApiClient(configuration)
+client = TremendousApi(api)
 ```
 
-The funding source you select is how you are charged for the order.
+### Examples
 
-```python
-funding_sources = client.funding_sources.list()
-funding_source_id = funding_sources[0]["id"]
-```
-
-Optionally pass a unique external_id for each order create call
-to guarantee that your order is idempotent and not executed multiple times.
+Submitting an order:
 
-```python
-external_id = "[ID FROM YOUR SYSTEM]"
-```
+```py
+from tremendous import CreateOrderRequest
 
-An array data representing the rewards you'd like to send.
-
-```python
-order_data = {
-  "external_id": external_id,
-  "payment": {
-    "funding_source_id": funding_source_id,
+request = CreateOrderRequest(
+  payment = {
+    "funding_source_id": "balance"
   },
-  "reward": {
-    "value": {
-      "denomination": 20,
-      "currency_code": "USD"
-    },
-    "campaign_id": campaign_id,
+  reward = {
+    "campaign_id": "CAMPAIGN_ID",
     "delivery": {
-      "method": "EMAIL",
+        "method": "EMAIL"
     },
     "recipient": {
-      "email": "sam@yourdomain.com",
-      "name": "Sam Stevens"
+      "email": "sarah@tremendous.com",
+      "name": "Sarah Smith"
+    },
+    "value": {
+        "denomination": 20,
+        "currency_code": "USD"
     }
-  }
-}
+  })
+
+response = client.create_order(request)
+print("Order created! ID: %s" % response.order.id)
+```
+
+Retrieving an Order and a Reward
+
+```py
+order = client.get_order("[ORDER_ID]").order
+reward = client.get_reward("[REWARD_ID]").reward
+
+print("The order status is %s" % order.status)
+print("The reward was delivered to %s" % reward.recipient.email)
 ```
 
-Submit the order.
+Listing products:
+
+```py
+products = api_client.list_products().products
+
+for product in products:
+  print(product.name)
 ```
-client.orders.create(order_data)
+
+Listing funding sources:
+
+```py
+funding_sources = client.funding_sources().funding_sources
+
+for funding_source in funding_sources:
+  print("* %s => %s" % (funding_source.method, funding_source.id))
 ```
 
-[1]: https://www.tremendous.com/docs
-[2]: https://testflight.tremendous.com/login
+[ref]: https://developers.tremendous.com/reference
+[docs]: https://tremendous.com/docs
```

