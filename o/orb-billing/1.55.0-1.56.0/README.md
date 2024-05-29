# Comparing `tmp/orb_billing-1.55.0.tar.gz` & `tmp/orb_billing-1.56.0.tar.gz`

## Comparing `orb_billing-1.55.0.tar` & `orb_billing-1.56.0.tar`

### file list

```diff
@@ -1,184 +1,185 @@
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/__init__.py
--rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_base_client.py
--rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_constants.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_files.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_legacy_response.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_qs.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_resource.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_response.py
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_streaming.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_version.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/lib/.keep
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/__init__.py
--rw-r--r--   0        0        0    38318 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/alerts.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/credit_notes.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/invoice_line_items.py
--rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/invoices.py
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/items.py
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/metrics.py
--rw-r--r--   0        0        0   163156 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/subscriptions.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/top_level.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/webhooks.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/coupons/__init__.py
--rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/coupons/coupons.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/coupons/subscriptions.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/__init__.py
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/balance_transactions.py
--rw-r--r--   0        0        0    44995 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/costs.py
--rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/customers.py
--rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/usage.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/credits/__init__.py
--rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/credits/credits.py
--rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/credits/ledger.py
--rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/customers/credits/top_ups.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/events/__init__.py
--rw-r--r--   0        0        0    28366 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/events/backfills.py
--rw-r--r--   0        0        0    52972 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/events/events.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/plans/__init__.py
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/plans/external_plan_id.py
--rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/plans/plans.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/prices/__init__.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/prices/external_price_id.py
--rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/resources/prices/prices.py
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/alert.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/alert_create_for_customer_params.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/alert_create_for_external_customer_params.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/alert_create_for_subscription_params.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/alert_list_params.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/coupon.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/coupon_create_params.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/coupon_list_params.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/credit_note.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/credit_note_list_params.py
--rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customer.py
--rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customer_create_params.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customer_list_params.py
--rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customer_update_by_external_id_params.py
--rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customer_update_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/evaluate_price_group.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_deprecate_response.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_ingest_params.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_ingest_response.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_search_params.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_search_response.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_update_params.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/event_update_response.py
--rw-r--r--   0        0        0    38126 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_create_params.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_fetch_upcoming_params.py
--rw-r--r--   0        0        0    38167 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_fetch_upcoming_response.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_line_item_create_params.py
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_line_item_create_response.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_list_params.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/invoice_mark_paid_params.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/item.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/item_create_params.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/item_list_params.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/metric_create_params.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/metric_create_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/metric_fetch_response.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/metric_list_params.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/metric_list_response.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plan.py
--rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plan_create_params.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plan_list_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plan_update_params.py
--rw-r--r--   0        0        0    36618 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/price.py
--rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/price_create_params.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/price_evaluate_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/price_evaluate_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/price_list_params.py
--rw-r--r--   0        0        0    20584 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_cancel_params.py
--rw-r--r--   0        0        0    31030 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_create_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_fetch_costs_params.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_fetch_costs_response.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_fetch_schedule_params.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_fetch_schedule_response.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_fetch_usage_params.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_list_params.py
--rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_price_intervals_params.py
--rw-r--r--   0        0        0    31436 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_schedule_plan_change_params.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_trigger_phase_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_update_params.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscription_usage.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/subscriptions.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/top_level_ping_response.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/beta/evaluate_price_group.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/beta/price_evaluate_params.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/beta/price_evaluate_response.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/coupons/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/coupons/subscription_list_params.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/balance_transaction_create_params.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/balance_transaction_create_response.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/balance_transaction_list_params.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/balance_transaction_list_response.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/cost_list_by_external_id_params.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/cost_list_by_external_id_response.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/cost_list_params.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/cost_list_response.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credit_list_by_external_id_params.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credit_list_by_external_id_response.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credit_list_params.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credit_list_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/usage_update_by_external_id_params.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/usage_update_by_external_id_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/usage_update_params.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/usage_update_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/__init__.py
--rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_params.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_response.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_params.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_response.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_params.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_params.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_response.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_close_response.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_create_params.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_create_response.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_fetch_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_list_params.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_list_response.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/events/backfill_revert_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plans/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/plans/external_plan_id_update_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/prices/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared/billing_cycle_relative_date.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared/discount.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared/pagination_metadata.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared_params/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.55.0/src/orb/types/shared_params/billing_cycle_relative_date.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.55.0/.gitignore
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.55.0/LICENSE
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.55.0/pyproject.toml
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.55.0/PKG-INFO
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/__init__.py
+-rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_base_client.py
+-rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_constants.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_files.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_legacy_response.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_qs.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_resource.py
+-rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_response.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_streaming.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_version.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/lib/.keep
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/__init__.py
+-rw-r--r--   0        0        0    38318 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/alerts.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/credit_notes.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/invoice_line_items.py
+-rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/invoices.py
+-rw-r--r--   0        0        0    16843 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/items.py
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/metrics.py
+-rw-r--r--   0        0        0   163156 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/subscriptions.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/top_level.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/webhooks.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/coupons/__init__.py
+-rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/coupons/coupons.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/coupons/subscriptions.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/__init__.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/balance_transactions.py
+-rw-r--r--   0        0        0    44995 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/costs.py
+-rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/customers.py
+-rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/usage.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/credits/__init__.py
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/credits/credits.py
+-rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/credits/ledger.py
+-rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/customers/credits/top_ups.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/events/__init__.py
+-rw-r--r--   0        0        0    28366 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/events/backfills.py
+-rw-r--r--   0        0        0    52972 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/events/events.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/plans/__init__.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/plans/external_plan_id.py
+-rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/plans/plans.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/prices/__init__.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/prices/external_price_id.py
+-rw-r--r--   0        0        0   148549 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/resources/prices/prices.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/alert.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/alert_create_for_customer_params.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/alert_create_for_external_customer_params.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/alert_create_for_subscription_params.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/alert_list_params.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/coupon.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/coupon_create_params.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/coupon_list_params.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/credit_note.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/credit_note_list_params.py
+-rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customer.py
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customer_create_params.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customer_list_params.py
+-rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customer_update_by_external_id_params.py
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customer_update_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/evaluate_price_group.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_deprecate_response.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_ingest_params.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_ingest_response.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_search_params.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_search_response.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_update_params.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/event_update_response.py
+-rw-r--r--   0        0        0    38126 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_create_params.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_fetch_upcoming_params.py
+-rw-r--r--   0        0        0    38167 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_fetch_upcoming_response.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_line_item_create_params.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_line_item_create_response.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_list_params.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/invoice_mark_paid_params.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/item.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/item_create_params.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/item_list_params.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/item_update_params.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/metric_create_params.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/metric_create_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/metric_fetch_response.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/metric_list_params.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/metric_list_response.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plan.py
+-rw-r--r--   0        0        0    27460 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plan_create_params.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plan_list_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plan_update_params.py
+-rw-r--r--   0        0        0    40796 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/price.py
+-rw-r--r--   0        0        0    31218 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/price_create_params.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/price_evaluate_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/price_evaluate_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/price_list_params.py
+-rw-r--r--   0        0        0    20584 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_cancel_params.py
+-rw-r--r--   0        0        0    31030 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_create_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_fetch_costs_params.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_fetch_costs_response.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_fetch_schedule_params.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_fetch_schedule_response.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_fetch_usage_params.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_list_params.py
+-rw-r--r--   0        0        0    36841 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_price_intervals_params.py
+-rw-r--r--   0        0        0    31436 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_schedule_plan_change_params.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_trigger_phase_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_update_params.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscription_usage.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/subscriptions.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/top_level_ping_response.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/beta/evaluate_price_group.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/beta/price_evaluate_params.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/beta/price_evaluate_response.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/coupons/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/coupons/subscription_list_params.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/balance_transaction_create_params.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/balance_transaction_create_response.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/balance_transaction_list_params.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/balance_transaction_list_response.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/cost_list_by_external_id_params.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/cost_list_by_external_id_response.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/cost_list_params.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/cost_list_response.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credit_list_by_external_id_params.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credit_list_by_external_id_response.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credit_list_params.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credit_list_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/usage_update_by_external_id_params.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/usage_update_by_external_id_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/usage_update_params.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/usage_update_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/__init__.py
+-rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_params.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_response.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_params.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_response.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_params.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_response.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_params.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_response.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_close_response.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_create_params.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_create_response.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_fetch_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_list_params.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_list_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/events/backfill_revert_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plans/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/plans/external_plan_id_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/prices/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared/discount.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared/pagination_metadata.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.56.0/src/orb/types/shared_params/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.56.0/.gitignore
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.56.0/LICENSE
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.56.0/pyproject.toml
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.56.0/PKG-INFO
```

### Comparing `orb_billing-1.55.0/src/orb/__init__.py` & `orb_billing-1.56.0/src/orb/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_base_client.py` & `orb_billing-1.56.0/src/orb/_base_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_client.py` & `orb_billing-1.56.0/src/orb/_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_compat.py` & `orb_billing-1.56.0/src/orb/_compat.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_exceptions.py` & `orb_billing-1.56.0/src/orb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_files.py` & `orb_billing-1.56.0/src/orb/_files.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_legacy_response.py` & `orb_billing-1.56.0/src/orb/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_models.py` & `orb_billing-1.56.0/src/orb/_models.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_qs.py` & `orb_billing-1.56.0/src/orb/_qs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_resource.py` & `orb_billing-1.56.0/src/orb/_resource.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_response.py` & `orb_billing-1.56.0/src/orb/_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_streaming.py` & `orb_billing-1.56.0/src/orb/_streaming.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_types.py` & `orb_billing-1.56.0/src/orb/_types.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/pagination.py` & `orb_billing-1.56.0/src/orb/pagination.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/__init__.py` & `orb_billing-1.56.0/src/orb/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_logs.py` & `orb_billing-1.56.0/src/orb/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_proxy.py` & `orb_billing-1.56.0/src/orb/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_sync.py` & `orb_billing-1.56.0/src/orb/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_transform.py` & `orb_billing-1.56.0/src/orb/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_typing.py` & `orb_billing-1.56.0/src/orb/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/_utils/_utils.py` & `orb_billing-1.56.0/src/orb/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     overload,
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
-from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
+from .._types import NotGiven, FileTypes, NotGivenOr, HeadersLike
 from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
@@ -366,15 +366,14 @@
     file_name = os.path.basename(path)
     return (file_name, contents)
 
 
 def get_required_header(headers: HeadersLike, header: str) -> str:
     lower_header = header.lower()
     if isinstance(headers, Mapping):
-        headers = cast(Headers, headers)
         for k, v in headers.items():
             if k.lower() == lower_header and isinstance(v, str):
                 return v
 
     """ to deal with the case where the header looks like Stainless-Event-Id """
     intercaps_header = re.sub(r"([^\w])(\w)", lambda pat: pat.group(1) + pat.group(2).upper(), header.capitalize())
```

### Comparing `orb_billing-1.55.0/src/orb/resources/__init__.py` & `orb_billing-1.56.0/src/orb/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/alerts.py` & `orb_billing-1.56.0/src/orb/resources/alerts.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/credit_notes.py` & `orb_billing-1.56.0/src/orb/resources/credit_notes.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/invoice_line_items.py` & `orb_billing-1.56.0/src/orb/resources/invoice_line_items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/invoices.py` & `orb_billing-1.56.0/src/orb/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/items.py` & `orb_billing-1.56.0/src/orb/resources/items.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Dict, Iterable, Optional
 
 import httpx
 
 from .. import _legacy_response
-from ..types import item_list_params, item_create_params
+from ..types import item_list_params, item_create_params, item_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -72,14 +72,68 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Item,
         )
 
+    def update(
+        self,
+        item_id: str,
+        *,
+        external_connections: Optional[Iterable[item_update_params.ExternalConnection]],
+        metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Item:
+        """Update items
+
+        Args:
+          metadata: User-specified key/value pairs for the resource.
+
+        Individual keys can be removed
+              by setting the value to `null`, and the entire metadata mapping can be cleared
+              by setting `metadata` to `null`.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not item_id:
+            raise ValueError(f"Expected a non-empty value for `item_id` but received {item_id!r}")
+        return self._put(
+            f"/items/{item_id}",
+            body=maybe_transform(
+                {
+                    "external_connections": external_connections,
+                    "metadata": metadata,
+                },
+                item_update_params.ItemUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=Item,
+        )
+
     def list(
         self,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -205,14 +259,68 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Item,
         )
 
+    async def update(
+        self,
+        item_id: str,
+        *,
+        external_connections: Optional[Iterable[item_update_params.ExternalConnection]],
+        metadata: Optional[Dict[str, Optional[str]]] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Item:
+        """Update items
+
+        Args:
+          metadata: User-specified key/value pairs for the resource.
+
+        Individual keys can be removed
+              by setting the value to `null`, and the entire metadata mapping can be cleared
+              by setting `metadata` to `null`.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        if not item_id:
+            raise ValueError(f"Expected a non-empty value for `item_id` but received {item_id!r}")
+        return await self._put(
+            f"/items/{item_id}",
+            body=await async_maybe_transform(
+                {
+                    "external_connections": external_connections,
+                    "metadata": metadata,
+                },
+                item_update_params.ItemUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=Item,
+        )
+
     def list(
         self,
         *,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -295,14 +403,17 @@
 class ItemsWithRawResponse:
     def __init__(self, items: Items) -> None:
         self._items = items
 
         self.create = _legacy_response.to_raw_response_wrapper(
             items.create,
         )
+        self.update = _legacy_response.to_raw_response_wrapper(
+            items.update,
+        )
         self.list = _legacy_response.to_raw_response_wrapper(
             items.list,
         )
         self.fetch = _legacy_response.to_raw_response_wrapper(
             items.fetch,
         )
 
@@ -310,14 +421,17 @@
 class AsyncItemsWithRawResponse:
     def __init__(self, items: AsyncItems) -> None:
         self._items = items
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             items.create,
         )
+        self.update = _legacy_response.async_to_raw_response_wrapper(
+            items.update,
+        )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             items.list,
         )
         self.fetch = _legacy_response.async_to_raw_response_wrapper(
             items.fetch,
         )
 
@@ -325,14 +439,17 @@
 class ItemsWithStreamingResponse:
     def __init__(self, items: Items) -> None:
         self._items = items
 
         self.create = to_streamed_response_wrapper(
             items.create,
         )
+        self.update = to_streamed_response_wrapper(
+            items.update,
+        )
         self.list = to_streamed_response_wrapper(
             items.list,
         )
         self.fetch = to_streamed_response_wrapper(
             items.fetch,
         )
 
@@ -340,13 +457,16 @@
 class AsyncItemsWithStreamingResponse:
     def __init__(self, items: AsyncItems) -> None:
         self._items = items
 
         self.create = async_to_streamed_response_wrapper(
             items.create,
         )
+        self.update = async_to_streamed_response_wrapper(
+            items.update,
+        )
         self.list = async_to_streamed_response_wrapper(
             items.list,
         )
         self.fetch = async_to_streamed_response_wrapper(
             items.fetch,
         )
```

### Comparing `orb_billing-1.55.0/src/orb/resources/metrics.py` & `orb_billing-1.56.0/src/orb/resources/metrics.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/subscriptions.py` & `orb_billing-1.56.0/src/orb/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/top_level.py` & `orb_billing-1.56.0/src/orb/resources/top_level.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/webhooks.py` & `orb_billing-1.56.0/src/orb/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/coupons/__init__.py` & `orb_billing-1.56.0/src/orb/resources/coupons/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/coupons/coupons.py` & `orb_billing-1.56.0/src/orb/resources/coupons/coupons.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/coupons/subscriptions.py` & `orb_billing-1.56.0/src/orb/resources/coupons/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/__init__.py` & `orb_billing-1.56.0/src/orb/resources/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/balance_transactions.py` & `orb_billing-1.56.0/src/orb/resources/customers/balance_transactions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/costs.py` & `orb_billing-1.56.0/src/orb/resources/customers/costs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/customers.py` & `orb_billing-1.56.0/src/orb/resources/customers/customers.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/usage.py` & `orb_billing-1.56.0/src/orb/resources/customers/usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/credits/__init__.py` & `orb_billing-1.56.0/src/orb/resources/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/credits/credits.py` & `orb_billing-1.56.0/src/orb/resources/customers/credits/credits.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/credits/ledger.py` & `orb_billing-1.56.0/src/orb/resources/customers/credits/ledger.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/customers/credits/top_ups.py` & `orb_billing-1.56.0/src/orb/resources/customers/credits/top_ups.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/events/__init__.py` & `orb_billing-1.56.0/src/orb/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/events/backfills.py` & `orb_billing-1.56.0/src/orb/resources/events/backfills.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/events/events.py` & `orb_billing-1.56.0/src/orb/resources/events/events.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/plans/__init__.py` & `orb_billing-1.56.0/src/orb/resources/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/plans/external_plan_id.py` & `orb_billing-1.56.0/src/orb/resources/plans/external_plan_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/plans/plans.py` & `orb_billing-1.56.0/src/orb/resources/plans/plans.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/prices/__init__.py` & `orb_billing-1.56.0/src/orb/resources/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/prices/external_price_id.py` & `orb_billing-1.56.0/src/orb/resources/prices/external_price_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/resources/prices/prices.py` & `orb_billing-1.56.0/src/orb/resources/prices/prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1215,14 +1215,160 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
+    @overload
+    def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        item_id: str,
+        model_type: Literal["tiered_with_proration"],
+        name: str,
+        tiered_with_proration_config: Dict[str, object],
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
+    @overload
+    def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        item_id: str,
+        model_type: Literal["unit_with_proration"],
+        name: str,
+        unit_with_proration_config: Dict[str, object],
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
     @required_args(
         ["cadence", "currency", "item_id", "model_type", "name", "unit_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_config"],
         ["cadence", "currency", "item_id", "matrix_config", "model_type", "name"],
         ["cadence", "currency", "item_id", "matrix_with_allocation_config", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_bps_config"],
@@ -1232,14 +1378,16 @@
         ["cadence", "currency", "item_id", "model_type", "name", "threshold_total_amount_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_config"],
         ["cadence", "currency", "grouped_tiered_config", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_with_allocation_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "unit_with_percent_config"],
+        ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_proration_config"],
+        ["cadence", "currency", "item_id", "model_type", "name", "unit_with_proration_config"],
     )
     def create(
         self,
         *,
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
@@ -1254,15 +1402,17 @@
         | Literal["bulk"]
         | Literal["threshold_total_amount"]
         | Literal["tiered_package"]
         | Literal["grouped_tiered"]
         | Literal["tiered_with_minimum"]
         | Literal["package_with_allocation"]
         | Literal["tiered_package_with_minimum"]
-        | Literal["unit_with_percent"],
+        | Literal["unit_with_percent"]
+        | Literal["tiered_with_proration"]
+        | Literal["unit_with_proration"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig | NotGiven = NOT_GIVEN,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
         conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
@@ -1279,14 +1429,16 @@
         threshold_total_amount_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         grouped_tiered_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         package_with_allocation_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         unit_with_percent_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        tiered_with_proration_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        unit_with_proration_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -1320,14 +1472,16 @@
                         "threshold_total_amount_config": threshold_total_amount_config,
                         "tiered_package_config": tiered_package_config,
                         "grouped_tiered_config": grouped_tiered_config,
                         "tiered_with_minimum_config": tiered_with_minimum_config,
                         "package_with_allocation_config": package_with_allocation_config,
                         "tiered_package_with_minimum_config": tiered_package_with_minimum_config,
                         "unit_with_percent_config": unit_with_percent_config,
+                        "tiered_with_proration_config": tiered_with_proration_config,
+                        "unit_with_proration_config": unit_with_proration_config,
                     },
                     price_create_params.PriceCreateParams,
                 ),
                 options=make_request_options(
                     extra_headers=extra_headers,
                     extra_query=extra_query,
                     extra_body=extra_body,
@@ -2694,14 +2848,160 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         ...
 
+    @overload
+    async def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        item_id: str,
+        model_type: Literal["tiered_with_proration"],
+        name: str,
+        tiered_with_proration_config: Dict[str, object],
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
+    @overload
+    async def create(
+        self,
+        *,
+        cadence: Literal["annual", "monthly", "quarterly", "one_time"],
+        currency: str,
+        item_id: str,
+        model_type: Literal["unit_with_proration"],
+        name: str,
+        unit_with_proration_config: Dict[str, object],
+        billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
+        billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
+        conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
+        external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
+        fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
+        invoice_grouping_key: Optional[str] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> Price:
+        """This endpoint is used to create a [price](../reference/price).
+
+        A price created
+        using this endpoint is always an add-on, meaning that it’s not associated with a
+        specific plan and can instead be individually added to subscriptions, including
+        subscriptions on different plans.
+
+        An `external_price_id` can be optionally specified as an alias to allow
+        ergonomic interaction with prices in the Orb API.
+
+        See the [Price resource](../reference/price) for the specification of different
+        price model configurations possible in this endpoint.
+
+        Args:
+          cadence: The cadence to bill for this price on.
+
+          currency: An ISO 4217 currency string for which this price is billed in.
+
+          item_id: The id of the item the plan will be associated with.
+
+          name: The name of the price.
+
+          billable_metric_id: The id of the billable metric for the price. Only needed if the price is
+              usage-based.
+
+          billed_in_advance: If the Price represents a fixed cost, the price will be billed in-advance if
+              this is true, and in-arrears if this is false.
+
+          conversion_rate: The per unit conversion rate of the price currency to the invoicing currency.
+
+          external_price_id: An alias for the price.
+
+          fixed_price_quantity: If the Price represents a fixed cost, this represents the quantity of units
+              applied.
+
+          invoice_grouping_key: The property used to group this price on an invoice
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        ...
+
     @required_args(
         ["cadence", "currency", "item_id", "model_type", "name", "unit_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_config"],
         ["cadence", "currency", "item_id", "matrix_config", "model_type", "name"],
         ["cadence", "currency", "item_id", "matrix_with_allocation_config", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_bps_config"],
@@ -2711,14 +3011,16 @@
         ["cadence", "currency", "item_id", "model_type", "name", "threshold_total_amount_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_config"],
         ["cadence", "currency", "grouped_tiered_config", "item_id", "model_type", "name"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "package_with_allocation_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "tiered_package_with_minimum_config"],
         ["cadence", "currency", "item_id", "model_type", "name", "unit_with_percent_config"],
+        ["cadence", "currency", "item_id", "model_type", "name", "tiered_with_proration_config"],
+        ["cadence", "currency", "item_id", "model_type", "name", "unit_with_proration_config"],
     )
     async def create(
         self,
         *,
         cadence: Literal["annual", "monthly", "quarterly", "one_time"],
         currency: str,
         item_id: str,
@@ -2733,15 +3035,17 @@
         | Literal["bulk"]
         | Literal["threshold_total_amount"]
         | Literal["tiered_package"]
         | Literal["grouped_tiered"]
         | Literal["tiered_with_minimum"]
         | Literal["package_with_allocation"]
         | Literal["tiered_package_with_minimum"]
-        | Literal["unit_with_percent"],
+        | Literal["unit_with_percent"]
+        | Literal["tiered_with_proration"]
+        | Literal["unit_with_proration"],
         name: str,
         unit_config: price_create_params.NewFloatingUnitPriceUnitConfig | NotGiven = NOT_GIVEN,
         billable_metric_id: Optional[str] | NotGiven = NOT_GIVEN,
         billed_in_advance: Optional[bool] | NotGiven = NOT_GIVEN,
         conversion_rate: Optional[float] | NotGiven = NOT_GIVEN,
         external_price_id: Optional[str] | NotGiven = NOT_GIVEN,
         fixed_price_quantity: Optional[float] | NotGiven = NOT_GIVEN,
@@ -2758,14 +3062,16 @@
         threshold_total_amount_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         grouped_tiered_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         package_with_allocation_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         tiered_package_with_minimum_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         unit_with_percent_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        tiered_with_proration_config: Dict[str, object] | NotGiven = NOT_GIVEN,
+        unit_with_proration_config: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
@@ -2799,14 +3105,16 @@
                         "threshold_total_amount_config": threshold_total_amount_config,
                         "tiered_package_config": tiered_package_config,
                         "grouped_tiered_config": grouped_tiered_config,
                         "tiered_with_minimum_config": tiered_with_minimum_config,
                         "package_with_allocation_config": package_with_allocation_config,
                         "tiered_package_with_minimum_config": tiered_package_with_minimum_config,
                         "unit_with_percent_config": unit_with_percent_config,
+                        "tiered_with_proration_config": tiered_with_proration_config,
+                        "unit_with_proration_config": unit_with_proration_config,
                     },
                     price_create_params.PriceCreateParams,
                 ),
                 options=make_request_options(
                     extra_headers=extra_headers,
                     extra_query=extra_query,
                     extra_body=extra_body,
```

### Comparing `orb_billing-1.55.0/src/orb/types/__init__.py` & `orb_billing-1.56.0/src/orb/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .subscriptions import Subscriptions as Subscriptions
 from .item_list_params import ItemListParams as ItemListParams
 from .plan_list_params import PlanListParams as PlanListParams
 from .alert_list_params import AlertListParams as AlertListParams
 from .price_list_params import PriceListParams as PriceListParams
 from .coupon_list_params import CouponListParams as CouponListParams
 from .item_create_params import ItemCreateParams as ItemCreateParams
+from .item_update_params import ItemUpdateParams as ItemUpdateParams
 from .metric_list_params import MetricListParams as MetricListParams
 from .plan_create_params import PlanCreateParams as PlanCreateParams
 from .plan_update_params import PlanUpdateParams as PlanUpdateParams
 from .subscription_usage import SubscriptionUsage as SubscriptionUsage
 from .event_ingest_params import EventIngestParams as EventIngestParams
 from .event_search_params import EventSearchParams as EventSearchParams
 from .event_update_params import EventUpdateParams as EventUpdateParams
```

### Comparing `orb_billing-1.55.0/src/orb/types/alert.py` & `orb_billing-1.56.0/src/orb/types/alert.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/alert_create_for_customer_params.py` & `orb_billing-1.56.0/src/orb/types/alert_create_for_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/alert_create_for_external_customer_params.py` & `orb_billing-1.56.0/src/orb/types/alert_create_for_external_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/alert_create_for_subscription_params.py` & `orb_billing-1.56.0/src/orb/types/alert_create_for_subscription_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/alert_list_params.py` & `orb_billing-1.56.0/src/orb/types/alert_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/coupon.py` & `orb_billing-1.56.0/src/orb/types/coupon.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/coupon_create_params.py` & `orb_billing-1.56.0/src/orb/types/coupon_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/coupon_list_params.py` & `orb_billing-1.56.0/src/orb/types/coupon_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/credit_note.py` & `orb_billing-1.56.0/src/orb/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customer.py` & `orb_billing-1.56.0/src/orb/types/customer.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customer_create_params.py` & `orb_billing-1.56.0/src/orb/types/customer_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customer_list_params.py` & `orb_billing-1.56.0/src/orb/types/customer_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customer_update_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customer_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customer_update_params.py` & `orb_billing-1.56.0/src/orb/types/customer_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/event_ingest_params.py` & `orb_billing-1.56.0/src/orb/types/event_ingest_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/event_ingest_response.py` & `orb_billing-1.56.0/src/orb/types/event_ingest_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/event_search_params.py` & `orb_billing-1.56.0/src/orb/types/event_search_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/event_search_response.py` & `orb_billing-1.56.0/src/orb/types/event_search_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/event_update_params.py` & `orb_billing-1.56.0/src/orb/types/event_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice.py` & `orb_billing-1.56.0/src/orb/types/invoice.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_create_params.py` & `orb_billing-1.56.0/src/orb/types/invoice_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_fetch_upcoming_response.py` & `orb_billing-1.56.0/src/orb/types/invoice_fetch_upcoming_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_line_item_create_params.py` & `orb_billing-1.56.0/src/orb/types/invoice_line_item_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_line_item_create_response.py` & `orb_billing-1.56.0/src/orb/types/invoice_line_item_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_list_params.py` & `orb_billing-1.56.0/src/orb/types/invoice_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/invoice_mark_paid_params.py` & `orb_billing-1.56.0/src/orb/types/invoice_mark_paid_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/item.py` & `orb_billing-1.56.0/src/orb/types/item.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/metric_create_params.py` & `orb_billing-1.56.0/src/orb/types/metric_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/metric_create_response.py` & `orb_billing-1.56.0/src/orb/types/metric_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/metric_fetch_response.py` & `orb_billing-1.56.0/src/orb/types/metric_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/metric_list_params.py` & `orb_billing-1.56.0/src/orb/types/metric_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/metric_list_response.py` & `orb_billing-1.56.0/src/orb/types/metric_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/plan.py` & `orb_billing-1.56.0/src/orb/types/plan.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/plan_create_params.py` & `orb_billing-1.56.0/src/orb/types/plan_create_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     "PriceNewPlanBulkPriceBulkConfig",
     "PriceNewPlanBulkPriceBulkConfigTier",
     "PriceNewPlanThresholdTotalAmountPrice",
     "PriceNewPlanTieredPackagePrice",
     "PriceNewPlanTieredWithMinimumPrice",
     "PriceNewPlanUnitWithPercentPrice",
     "PriceNewPlanPackageWithAllocationPrice",
+    "PriceNewPlanTierWithProrationPrice",
+    "PriceNewPlanUnitWithProrationPrice",
 ]
 
 
 class PlanCreateParams(TypedDict, total=False):
     currency: Required[str]
     """
     An ISO 4217 currency string for invoices generated by subscriptions on this
@@ -812,22 +814,120 @@
     applied.
     """
 
     invoice_grouping_key: Optional[str]
     """The property used to group this price on an invoice"""
 
 
+class PriceNewPlanTierWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["tiered_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    tiered_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
+class PriceNewPlanUnitWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["unit_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    unit_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    currency: Optional[str]
+    """
+    An ISO 4217 currency string, or custom pricing unit identifier, in which this
+    price is billed.
+    """
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
 Price = Union[
     PriceNewPlanUnitPrice,
     PriceNewPlanPackagePrice,
     PriceNewPlanMatrixPrice,
     PriceNewPlanTieredPrice,
     PriceNewPlanTieredBpsPrice,
     PriceNewPlanBpsPrice,
     PriceNewPlanBulkBpsPrice,
     PriceNewPlanBulkPrice,
     PriceNewPlanThresholdTotalAmountPrice,
     PriceNewPlanTieredPackagePrice,
     PriceNewPlanTieredWithMinimumPrice,
     PriceNewPlanUnitWithPercentPrice,
     PriceNewPlanPackageWithAllocationPrice,
+    PriceNewPlanTierWithProrationPrice,
+    PriceNewPlanUnitWithProrationPrice,
 ]
```

### Comparing `orb_billing-1.55.0/src/orb/types/plan_list_params.py` & `orb_billing-1.56.0/src/orb/types/plan_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/plan_update_params.py` & `orb_billing-1.56.0/src/orb/types/plan_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/price.py` & `orb_billing-1.56.0/src/orb/types/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,26 @@
     "MatrixWithAllocationPriceBillableMetric",
     "MatrixWithAllocationPriceCreditAllocation",
     "MatrixWithAllocationPriceItem",
     "MatrixWithAllocationPriceMatrixWithAllocationConfig",
     "MatrixWithAllocationPriceMatrixWithAllocationConfigMatrixValue",
     "MatrixWithAllocationPriceMaximum",
     "MatrixWithAllocationPriceMinimum",
+    "TieredWithProrationPrice",
+    "TieredWithProrationPriceBillableMetric",
+    "TieredWithProrationPriceCreditAllocation",
+    "TieredWithProrationPriceItem",
+    "TieredWithProrationPriceMaximum",
+    "TieredWithProrationPriceMinimum",
+    "UnitWithProrationPrice",
+    "UnitWithProrationPriceBillableMetric",
+    "UnitWithProrationPriceCreditAllocation",
+    "UnitWithProrationPriceItem",
+    "UnitWithProrationPriceMaximum",
+    "UnitWithProrationPriceMinimum",
 ]
 
 
 class UnitPriceBillableMetric(BaseModel):
     id: str
 
 
@@ -1546,14 +1558,174 @@
     name: str
 
     plan_phase_order: Optional[int] = None
 
     price_type: Literal["usage_price", "fixed_price"]
 
 
+class TieredWithProrationPriceBillableMetric(BaseModel):
+    id: str
+
+
+class TieredWithProrationPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
+class TieredWithProrationPriceItem(BaseModel):
+    id: str
+
+    name: str
+
+
+class TieredWithProrationPriceMaximum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this maximum amount applies to.
+
+    For plan/plan phase maximums, this can be a subset of prices.
+    """
+
+    maximum_amount: str
+    """Maximum amount applied"""
+
+
+class TieredWithProrationPriceMinimum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this minimum amount applies to.
+
+    For plan/plan phase minimums, this can be a subset of prices.
+    """
+
+    minimum_amount: str
+    """Minimum amount applied"""
+
+
+class TieredWithProrationPrice(BaseModel):
+    id: str
+
+    billable_metric: Optional[TieredWithProrationPriceBillableMetric] = None
+
+    cadence: Literal["one_time", "monthly", "quarterly", "annual"]
+
+    conversion_rate: Optional[float] = None
+
+    created_at: datetime
+
+    credit_allocation: Optional[TieredWithProrationPriceCreditAllocation] = None
+
+    currency: str
+
+    discount: Optional[Discount] = None
+
+    external_price_id: Optional[str] = None
+
+    fixed_price_quantity: Optional[float] = None
+
+    item: TieredWithProrationPriceItem
+
+    maximum: Optional[TieredWithProrationPriceMaximum] = None
+
+    maximum_amount: Optional[str] = None
+
+    minimum: Optional[TieredWithProrationPriceMinimum] = None
+
+    minimum_amount: Optional[str] = None
+
+    price_model_type: Literal["tiered_with_proration"] = FieldInfo(alias="model_type")
+
+    name: str
+
+    plan_phase_order: Optional[int] = None
+
+    price_type: Literal["usage_price", "fixed_price"]
+
+    tiered_with_proration_config: Dict[str, object]
+
+
+class UnitWithProrationPriceBillableMetric(BaseModel):
+    id: str
+
+
+class UnitWithProrationPriceCreditAllocation(BaseModel):
+    allows_rollover: bool
+
+    currency: str
+
+
+class UnitWithProrationPriceItem(BaseModel):
+    id: str
+
+    name: str
+
+
+class UnitWithProrationPriceMaximum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this maximum amount applies to.
+
+    For plan/plan phase maximums, this can be a subset of prices.
+    """
+
+    maximum_amount: str
+    """Maximum amount applied"""
+
+
+class UnitWithProrationPriceMinimum(BaseModel):
+    applies_to_price_ids: List[str]
+    """List of price_ids that this minimum amount applies to.
+
+    For plan/plan phase minimums, this can be a subset of prices.
+    """
+
+    minimum_amount: str
+    """Minimum amount applied"""
+
+
+class UnitWithProrationPrice(BaseModel):
+    id: str
+
+    billable_metric: Optional[UnitWithProrationPriceBillableMetric] = None
+
+    cadence: Literal["one_time", "monthly", "quarterly", "annual"]
+
+    conversion_rate: Optional[float] = None
+
+    created_at: datetime
+
+    credit_allocation: Optional[UnitWithProrationPriceCreditAllocation] = None
+
+    currency: str
+
+    discount: Optional[Discount] = None
+
+    external_price_id: Optional[str] = None
+
+    fixed_price_quantity: Optional[float] = None
+
+    item: UnitWithProrationPriceItem
+
+    maximum: Optional[UnitWithProrationPriceMaximum] = None
+
+    maximum_amount: Optional[str] = None
+
+    minimum: Optional[UnitWithProrationPriceMinimum] = None
+
+    minimum_amount: Optional[str] = None
+
+    price_model_type: Literal["unit_with_proration"] = FieldInfo(alias="model_type")
+
+    name: str
+
+    plan_phase_order: Optional[int] = None
+
+    price_type: Literal["usage_price", "fixed_price"]
+
+    unit_with_proration_config: Dict[str, object]
+
+
 Price = Annotated[
     Union[
         UnitPrice,
         PackagePrice,
         MatrixPrice,
         TieredPrice,
         TieredBpsPrice,
@@ -1564,10 +1736,12 @@
         TieredPackagePrice,
         GroupedTieredPrice,
         TieredWithMinimumPrice,
         TieredPackageWithMinimumPrice,
         PackageWithAllocationPrice,
         UnitWithPercentPrice,
         MatrixWithAllocationPrice,
+        TieredWithProrationPrice,
+        UnitWithProrationPrice,
     ],
     PropertyInfo(discriminator="price_model_type"),
 ]
```

### Comparing `orb_billing-1.55.0/src/orb/types/price_create_params.py` & `orb_billing-1.56.0/src/orb/types/price_create_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "NewFloatingThresholdTotalAmountPrice",
     "NewFloatingTieredPackagePrice",
     "NewFloatingGroupedTieredPrice",
     "NewFloatingTieredWithMinimumPrice",
     "NewFloatingPackageWithAllocationPrice",
     "NewFloatingTieredPackageWithMinimumPrice",
     "NewFloatingUnitWithPercentPrice",
+    "NewFloatingTieredWithProrationPrice",
+    "NewFloatingUnitWithProrationPrice",
 ]
 
 
 class NewFloatingUnitPrice(TypedDict, total=False):
     cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
     """The cadence to bill for this price on."""
 
@@ -901,14 +903,104 @@
     applied.
     """
 
     invoice_grouping_key: Optional[str]
     """The property used to group this price on an invoice"""
 
 
+class NewFloatingTieredWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["tiered_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    tiered_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
+class NewFloatingUnitWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["unit_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    unit_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
 PriceCreateParams = Union[
     NewFloatingUnitPrice,
     NewFloatingPackagePrice,
     NewFloatingMatrixPrice,
     NewFloatingMatrixWithAllocationPrice,
     NewFloatingTieredPrice,
     NewFloatingTieredBpsPrice,
@@ -918,8 +1010,10 @@
     NewFloatingThresholdTotalAmountPrice,
     NewFloatingTieredPackagePrice,
     NewFloatingGroupedTieredPrice,
     NewFloatingTieredWithMinimumPrice,
     NewFloatingPackageWithAllocationPrice,
     NewFloatingTieredPackageWithMinimumPrice,
     NewFloatingUnitWithPercentPrice,
+    NewFloatingTieredWithProrationPrice,
+    NewFloatingUnitWithProrationPrice,
 ]
```

### Comparing `orb_billing-1.55.0/src/orb/types/price_evaluate_params.py` & `orb_billing-1.56.0/src/orb/types/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription.py` & `orb_billing-1.56.0/src/orb/types/subscription.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_cancel_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_cancel_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_create_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_fetch_costs_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_fetch_costs_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_fetch_costs_response.py` & `orb_billing-1.56.0/src/orb/types/subscription_fetch_costs_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_fetch_schedule_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_fetch_schedule_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_fetch_schedule_response.py` & `orb_billing-1.56.0/src/orb/types/subscription_fetch_schedule_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_fetch_usage_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_fetch_usage_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_list_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_price_intervals_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_price_intervals_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     "AddPriceNewFloatingThresholdTotalAmountPrice",
     "AddPriceNewFloatingTieredPackagePrice",
     "AddPriceNewFloatingGroupedTieredPrice",
     "AddPriceNewFloatingTieredWithMinimumPrice",
     "AddPriceNewFloatingPackageWithAllocationPrice",
     "AddPriceNewFloatingTieredPackageWithMinimumPrice",
     "AddPriceNewFloatingUnitWithPercentPrice",
+    "AddPriceNewFloatingTieredWithProrationPrice",
+    "AddPriceNewFloatingUnitWithProrationPrice",
     "Edit",
     "EditFixedFeeQuantityTransition",
 ]
 
 
 class SubscriptionPriceIntervalsParams(TypedDict, total=False):
     add: Iterable[Add]
@@ -964,14 +966,104 @@
     applied.
     """
 
     invoice_grouping_key: Optional[str]
     """The property used to group this price on an invoice"""
 
 
+class AddPriceNewFloatingTieredWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["tiered_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    tiered_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
+class AddPriceNewFloatingUnitWithProrationPrice(TypedDict, total=False):
+    cadence: Required[Literal["annual", "monthly", "quarterly", "one_time"]]
+    """The cadence to bill for this price on."""
+
+    currency: Required[str]
+    """An ISO 4217 currency string for which this price is billed in."""
+
+    item_id: Required[str]
+    """The id of the item the plan will be associated with."""
+
+    model_type: Required[Literal["unit_with_proration"]]
+
+    name: Required[str]
+    """The name of the price."""
+
+    unit_with_proration_config: Required[Dict[str, object]]
+
+    billable_metric_id: Optional[str]
+    """The id of the billable metric for the price.
+
+    Only needed if the price is usage-based.
+    """
+
+    billed_in_advance: Optional[bool]
+    """
+    If the Price represents a fixed cost, the price will be billed in-advance if
+    this is true, and in-arrears if this is false.
+    """
+
+    conversion_rate: Optional[float]
+    """The per unit conversion rate of the price currency to the invoicing currency."""
+
+    external_price_id: Optional[str]
+    """An alias for the price."""
+
+    fixed_price_quantity: Optional[float]
+    """
+    If the Price represents a fixed cost, this represents the quantity of units
+    applied.
+    """
+
+    invoice_grouping_key: Optional[str]
+    """The property used to group this price on an invoice"""
+
+
 AddPrice = Union[
     AddPriceNewFloatingUnitPrice,
     AddPriceNewFloatingPackagePrice,
     AddPriceNewFloatingMatrixPrice,
     AddPriceNewFloatingMatrixWithAllocationPrice,
     AddPriceNewFloatingTieredPrice,
     AddPriceNewFloatingTieredBpsPrice,
@@ -981,14 +1073,16 @@
     AddPriceNewFloatingThresholdTotalAmountPrice,
     AddPriceNewFloatingTieredPackagePrice,
     AddPriceNewFloatingGroupedTieredPrice,
     AddPriceNewFloatingTieredWithMinimumPrice,
     AddPriceNewFloatingPackageWithAllocationPrice,
     AddPriceNewFloatingTieredPackageWithMinimumPrice,
     AddPriceNewFloatingUnitWithPercentPrice,
+    AddPriceNewFloatingTieredWithProrationPrice,
+    AddPriceNewFloatingUnitWithProrationPrice,
 ]
 
 
 class Add(TypedDict, total=False):
     start_date: Required[
         Annotated[Union[Union[str, datetime], BillingCycleRelativeDate], PropertyInfo(format="iso8601")]
     ]
```

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_schedule_plan_change_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_schedule_plan_change_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_trigger_phase_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_trigger_phase_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_update_params.py` & `orb_billing-1.56.0/src/orb/types/subscription_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/subscription_usage.py` & `orb_billing-1.56.0/src/orb/types/subscription_usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/beta/price_evaluate_params.py` & `orb_billing-1.56.0/src/orb/types/beta/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/coupons/subscription_list_params.py` & `orb_billing-1.56.0/src/orb/types/coupons/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/__init__.py` & `orb_billing-1.56.0/src/orb/types/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/balance_transaction_create_response.py` & `orb_billing-1.56.0/src/orb/types/customers/balance_transaction_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/balance_transaction_list_params.py` & `orb_billing-1.56.0/src/orb/types/customers/balance_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/balance_transaction_list_response.py` & `orb_billing-1.56.0/src/orb/types/customers/balance_transaction_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/cost_list_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/cost_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/cost_list_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/cost_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/cost_list_params.py` & `orb_billing-1.56.0/src/orb/types/customers/cost_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/cost_list_response.py` & `orb_billing-1.56.0/src/orb/types/customers/cost_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credit_list_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credit_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credit_list_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credit_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credit_list_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credit_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/usage_update_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/usage_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/usage_update_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/usage_update_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/usage_update_params.py` & `orb_billing-1.56.0/src/orb/types/customers/usage_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/__init__.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_create_entry_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_create_entry_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/ledger_list_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/ledger_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_create_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/customers/credits/top_up_list_response.py` & `orb_billing-1.56.0/src/orb/types/customers/credits/top_up_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/__init__.py` & `orb_billing-1.56.0/src/orb/types/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_close_response.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_close_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_create_params.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_create_response.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_fetch_response.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_list_response.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/events/backfill_revert_response.py` & `orb_billing-1.56.0/src/orb/types/events/backfill_revert_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/plans/external_plan_id_update_params.py` & `orb_billing-1.56.0/src/orb/types/plans/external_plan_id_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/src/orb/types/shared/discount.py` & `orb_billing-1.56.0/src/orb/types/shared/discount.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/LICENSE` & `orb_billing-1.56.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orb_billing-1.55.0/pyproject.toml` & `orb_billing-1.56.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "orb-billing"
-version = "1.55.0"
+version = "1.56.0"
 description = "The official Python library for the orb API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Orb", email = "team@withorb.com" },
 ]
 dependencies = [
```

### Comparing `orb_billing-1.55.0/PKG-INFO` & `orb_billing-1.56.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: orb-billing
-Version: 1.55.0
+Version: 1.56.0
 Summary: The official Python library for the orb API
 Project-URL: Homepage, https://github.com/orbcorp/orb-python
 Project-URL: Repository, https://github.com/orbcorp/orb-python
 Author-email: Orb <team@withorb.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

