# Comparing `tmp/airbyte_source_shopify-2.1.4.tar.gz` & `tmp/airbyte_source_shopify-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.1.4.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.2.0.tar", max compression
```

## Comparing `airbyte_source_shopify-2.1.4.tar` & `airbyte_source_shopify-2.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4529 2024-05-24 12:51:12.116168 airbyte_source_shopify-2.1.4/README.md
--rw-r--r--   0        0        0      800 2024-05-24 12:57:56.400493 airbyte_source_shopify-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1773 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0    10425 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4886 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    14495 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/scopes.py
--rw-r--r--   0        0        0        0 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/__init__.py
--rw-r--r--   0        0        0     1813 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20372 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    84915 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6526 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     1704 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/retry.py
--rw-r--r--   0        0        0      328 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/status.py
--rw-r--r--   0        0        0     3629 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8518 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/spec.json
--rw-r--r--   0        0        0    37215 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11715 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/transform.py
--rw-r--r--   0        0        0    13468 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/utils.py
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/README.md
+-rw-r--r--   0        0        0      800 2024-05-29 13:53:19.927800 airbyte_source_shopify-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2161 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1773 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0    10425 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4886 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    14495 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/scopes.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/__init__.py
+-rw-r--r--   0        0        0     1813 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20372 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    84915 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6526 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1704 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8518 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/spec.json
+-rw-r--r--   0        0        0    37215 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11715 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-29 13:05:33.000000 airbyte_source_shopify-2.2.0/source_shopify/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.2.0/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.1.4/README.md` & `airbyte_source_shopify-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/pyproject.toml` & `airbyte_source_shopify-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.4"
+version = "2.2.0"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/__init__.py` & `airbyte_source_shopify-2.2.0/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/auth.py` & `airbyte_source_shopify-2.2.0/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.2.0/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/countries.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999948330026456%*

 * *Differences: {"'properties'": "{'provinces': {'items': {'properties': {'tax_percentage': {'type': {insert: [(1, "*

 * *                 "'number')], delete: [1]}}}}}}"}*

```diff
@@ -68,15 +68,15 @@
                             "string"
                         ]
                     },
                     "tax_percentage": {
                         "description": "Percentage value of tax applicable in the province.",
                         "type": [
                             "null",
-                            "integer"
+                            "number"
                         ]
                     },
                     "tax_type": {
                         "description": "Type of tax (e.g., sales tax, VAT) applicable in the province.",
                         "type": [
                             "null",
                             "string"
```

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.2.0/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/scopes.py` & `airbyte_source_shopify-2.2.0/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/retry.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/retry.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.2.0/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/source.py` & `airbyte_source_shopify-2.2.0/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/spec.json` & `airbyte_source_shopify-2.2.0/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.2.0/source_shopify/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.2.0/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/transform.py` & `airbyte_source_shopify-2.2.0/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/source_shopify/utils.py` & `airbyte_source_shopify-2.2.0/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.4/PKG-INFO` & `airbyte_source_shopify-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.1.4
+Version: 2.2.0
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

