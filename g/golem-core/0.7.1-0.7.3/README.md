# Comparing `tmp/golem_core-0.7.1.tar.gz` & `tmp/golem_core-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_core-0.7.1.tar", max compression
+gzip compressed data, was "golem_core-0.7.3.tar", max compression
```

## Comparing `golem_core-0.7.1.tar` & `golem_core-0.7.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0    35149 2024-04-17 13:45:08.432969 golem_core-0.7.1/LICENSE
--rw-r--r--   0        0        0        0 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/__init__.py
--rw-r--r--   0        0        0       64 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/__main__.py
--rw-r--r--   0        0        0       50 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/cli.py
--rw-r--r--   0        0        0     4463 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/cli/utils.py
--rw-r--r--   0        0        0      151 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/base.py
--rw-r--r--   0        0        0       98 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/in_memory/__init__.py
--rw-r--r--   0        0        0     6737 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/event_bus/in_memory/event_bus.py
--rw-r--r--   0        0        0      332 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/exceptions.py
--rw-r--r--   0        0        0     2554 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/__init__.py
--rw-r--r--   0        0        0      475 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/__init__.py
--rw-r--r--   0        0        0      476 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/defaults.py
--rw-r--r--   0        0        0     2111 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/mixins.py
--rw-r--r--   0        0        0     3872 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/pool.py
--rw-r--r--   0        0        0     1734 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/activity/single_use.py
--rw-r--r--   0        0        0      109 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/agreement/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/agreement/default.py
--rw-r--r--   0        0        0     5925 2024-04-17 13:45:08.440969 golem_core-0.7.1/golem/managers/base.py
--rw-r--r--   0        0        0      218 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/aggregating.py
--rw-r--r--   0        0        0     5488 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/demand/refreshing.py
--rw-r--r--   0        0        0     1658 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/mixins.py
--rw-r--r--   0        0        0      100 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/network/__init__.py
--rw-r--r--   0        0        0     2197 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/network/single.py
--rw-r--r--   0        0        0      103 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/payment/__init__.py
--rw-r--r--   0        0        0     5937 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/payment/default.py
--rw-r--r--   0        0        0      980 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/__init__.py
--rw-r--r--   0        0        0     1586 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/default.py
--rw-r--r--   0        0        0     1155 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/blacklist.py
--rw-r--r--   0        0        0     5125 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/buffer.py
--rw-r--r--   0        0        0     1054 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/linear_coeffs.py
--rw-r--r--   0        0        0      422 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/__init__.py
--rw-r--r--   0        0        0     4671 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
--rw-r--r--   0        0        0     5467 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
--rw-r--r--   0        0        0     1567 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/payment_platform.py
--rw-r--r--   0        0        0     2441 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/reject_costs_exceeds.py
--rw-r--r--   0        0        0      738 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/__init__.py
--rw-r--r--   0        0        0     1738 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/map.py
--rw-r--r--   0        0        0     4008 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/mixins.py
--rw-r--r--   0        0        0     1938 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/pricings.py
--rw-r--r--   0        0        0     3457 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/property_value_lerp.py
--rw-r--r--   0        0        0      505 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/random.py
--rw-r--r--   0        0        0     4217 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/scoring/scoring_buffer.py
--rw-r--r--   0        0        0      996 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/proposal/plugins/whitelist.py
--rw-r--r--   0        0        0      474 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/__init__.py
--rw-r--r--   0        0        0     2087 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/concurrent.py
--rw-r--r--   0        0        0     2024 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/mixins.py
--rw-r--r--   0        0        0     2038 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/plugins.py
--rw-r--r--   0        0        0     1201 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/managers/work/sequential.py
--rw-r--r--   0        0        0      257 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/__init__.py
--rw-r--r--   0        0        0      856 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/events.py
--rw-r--r--   0        0        0    16730 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/node/node.py
--rw-r--r--   0        0        0     1153 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/__init__.py
--rw-r--r--   0        0        0     6649 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/base.py
--rw-r--r--   0        0        0     1939 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/constraints.py
--rw-r--r--   0        0        0     5156 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/defaults.py
--rw-r--r--   0        0        0      284 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/exceptions.py
--rw-r--r--   0        0        0      973 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/generic.py
--rw-r--r--   0        0        0     1405 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/mixins.py
--rw-r--r--   0        0        0     1186 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/parser.py
--rw-r--r--   0        0        0      621 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/parser.tx
--rw-r--r--   0        0        0      868 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/properties.py
--rw-r--r--   0        0        0     5677 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/payload/vm.py
--rw-r--r--   0        0        0      504 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/__init__.py
--rw-r--r--   0        0        0     4535 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/buffer.py
--rw-r--r--   0        0        0     1847 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/chain.py
--rw-r--r--   0        0        0     3704 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/default_payment_handler.py
--rw-r--r--   0        0        0     1363 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/exceptions.py
--rw-r--r--   0        0        0      842 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/limit.py
--rw-r--r--   0        0        0     3990 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/map.py
--rw-r--r--   0        0        0     4152 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/sort.py
--rw-r--r--   0        0        0     2453 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/pipeline/zip.py
--rw-r--r--   0        0        0     3462 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/__init__.py
--rw-r--r--   0        0        0      592 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/__init__.py
--rw-r--r--   0        0        0     6327 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/activity.py
--rw-r--r--   0        0        0     6903 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/commands.py
--rw-r--r--   0        0        0      391 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/events.py
--rw-r--r--   0        0        0      735 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/activity/pipeline.py
--rw-r--r--   0        0        0      360 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/__init__.py
--rw-r--r--   0        0        0     6718 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/agreement.py
--rw-r--r--   0        0        0      375 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/data.py
--rw-r--r--   0        0        0      400 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/events.py
--rw-r--r--   0        0        0      289 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/agreement/pipeline.py
--rw-r--r--   0        0        0      410 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/__init__.py
--rw-r--r--   0        0        0     3220 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/allocation.py
--rw-r--r--   0        0        0      409 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/events.py
--rw-r--r--   0        0        0      835 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/allocation/exceptions.py
--rw-r--r--   0        0        0    11150 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/base.py
--rw-r--r--   0        0        0      372 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/__init__.py
--rw-r--r--   0        0        0     9169 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/debit_note.py
--rw-r--r--   0        0        0      784 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/event_collectors.py
--rw-r--r--   0        0        0      402 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/debit_note/events.py
--rw-r--r--   0        0        0      379 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/__init__.py
--rw-r--r--   0        0        0      315 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/data.py
--rw-r--r--   0        0        0     5532 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/demand.py
--rw-r--r--   0        0        0     2959 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/demand_builder.py
--rw-r--r--   0        0        0      373 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/demand/events.py
--rw-r--r--   0        0        0     1559 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/event_collectors.py
--rw-r--r--   0        0        0     4215 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/events.py
--rw-r--r--   0        0        0     1016 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/exceptions.py
--rw-r--r--   0        0        0      340 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/__init__.py
--rw-r--r--   0        0        0      760 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/event_collectors.py
--rw-r--r--   0        0        0      382 2024-04-17 13:45:08.444969 golem_core-0.7.1/golem/resources/invoice/events.py
--rw-r--r--   0        0        0     5307 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/invoice/invoice.py
--rw-r--r--   0        0        0      394 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/__init__.py
--rw-r--r--   0        0        0      382 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/events.py
--rw-r--r--   0        0        0      590 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/exceptions.py
--rw-r--r--   0        0        0     5803 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/network/network.py
--rw-r--r--   0        0        0      509 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/__init__.py
--rw-r--r--   0        0        0      456 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/events.py
--rw-r--r--   0        0        0     2122 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/exceptions.py
--rw-r--r--   0        0        0     5510 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/pooling_batch/pooling_batch.py
--rw-r--r--   0        0        0      499 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/__init__.py
--rw-r--r--   0        0        0      508 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/data.py
--rw-r--r--   0        0        0      391 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/events.py
--rw-r--r--   0        0        0      664 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/exceptions.py
--rw-r--r--   0        0        0      860 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/pipeline.py
--rw-r--r--   0        0        0     9303 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/proposal/proposal.py
--rw-r--r--   0        0        0        0 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/__init__.py
--rw-r--r--   0        0        0      626 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/infrastructure.py
--rw-r--r--   0        0        0     6911 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/resources/utils/payment.py
--rw-r--r--   0        0        0        0 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/__init__.py
--rw-r--r--   0        0        0      704 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/__init__.py
--rw-r--r--   0        0        0    13751 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/buffer.py
--rw-r--r--   0        0        0     2044 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/queue.py
--rw-r--r--   0        0        0     2056 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/semaphore.py
--rw-r--r--   0        0        0     2820 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/tasks.py
--rw-r--r--   0        0        0     1726 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/asyncio/waiter.py
--rw-r--r--   0        0        0      741 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/http.py
--rw-r--r--   0        0        0     7521 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/logging.py
--rw-r--r--   0        0        0      307 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/__init__.py
--rw-r--r--   0        0        0     6571 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/api.py
--rw-r--r--   0        0        0     3323 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/low/event_collector.py
--rw-r--r--   0        0        0      105 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/base.py
--rw-r--r--   0        0        0       88 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/gftp/__init__.py
--rw-r--r--   0        0        0    16077 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/gftp/provider.py
--rw-r--r--   0        0        0      673 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/storage/utils.py
--rw-r--r--   0        0        0      767 2024-04-17 13:45:08.448969 golem_core-0.7.1/golem/utils/typing.py
--rw-r--r--   0        0        0     4722 2024-04-17 13:45:08.448969 golem_core-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 golem_core-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-13 08:05:36.792448 golem_core-0.7.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/__init__.py
+-rw-r--r--   0        0        0       64 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/__main__.py
+-rw-r--r--   0        0        0       50 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/cli/__init__.py
+-rw-r--r--   0        0        0     2641 2023-11-25 08:20:36.562759 golem_core-0.7.3/golem/cli/cli.py
+-rw-r--r--   0        0        0     4463 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/cli/utils.py
+-rw-r--r--   0        0        0      151 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/event_bus/__init__.py
+-rw-r--r--   0        0        0     1280 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/event_bus/base.py
+-rw-r--r--   0        0        0       98 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/event_bus/in_memory/__init__.py
+-rw-r--r--   0        0        0     6737 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/event_bus/in_memory/event_bus.py
+-rw-r--r--   0        0        0      332 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/exceptions.py
+-rw-r--r--   0        0        0     2554 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/managers/__init__.py
+-rw-r--r--   0        0        0      475 2023-10-10 09:27:48.015544 golem_core-0.7.3/golem/managers/activity/__init__.py
+-rw-r--r--   0        0        0      476 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/activity/defaults.py
+-rw-r--r--   0        0        0     2111 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/activity/mixins.py
+-rw-r--r--   0        0        0     3872 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/activity/pool.py
+-rw-r--r--   0        0        0     1734 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/activity/single_use.py
+-rw-r--r--   0        0        0      109 2023-10-03 11:48:04.547546 golem_core-0.7.3/golem/managers/agreement/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/managers/agreement/default.py
+-rw-r--r--   0        0        0     5925 2024-03-28 09:34:26.737805 golem_core-0.7.3/golem/managers/base.py
+-rw-r--r--   0        0        0      218 2024-02-28 10:31:22.882324 golem_core-0.7.3/golem/managers/demand/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-09 07:23:27.117157 golem_core-0.7.3/golem/managers/demand/aggregating.py
+-rw-r--r--   0        0        0     5488 2024-02-15 12:52:48.457251 golem_core-0.7.3/golem/managers/demand/refreshing.py
+-rw-r--r--   0        0        0     1658 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/mixins.py
+-rw-r--r--   0        0        0      100 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/network/__init__.py
+-rw-r--r--   0        0        0     2197 2023-12-13 09:08:00.946133 golem_core-0.7.3/golem/managers/network/single.py
+-rw-r--r--   0        0        0      103 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/managers/payment/__init__.py
+-rw-r--r--   0        0        0     5945 2024-05-29 14:12:26.327190 golem_core-0.7.3/golem/managers/payment/default.py
+-rw-r--r--   0        0        0      980 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/proposal/__init__.py
+-rw-r--r--   0        0        0     1586 2023-11-02 09:14:12.499044 golem_core-0.7.3/golem/managers/proposal/default.py
+-rw-r--r--   0        0        0     1155 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/proposal/plugins/__init__.py
+-rw-r--r--   0        0        0     1005 2023-10-13 09:42:33.129828 golem_core-0.7.3/golem/managers/proposal/plugins/blacklist.py
+-rw-r--r--   0        0        0     5331 2024-05-29 14:12:26.327190 golem_core-0.7.3/golem/managers/proposal/plugins/buffer.py
+-rw-r--r--   0        0        0     1054 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/managers/proposal/plugins/linear_coeffs.py
+-rw-r--r--   0        0        0      422 2024-01-23 10:41:17.114958 golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/__init__.py
+-rw-r--r--   0        0        0     4671 2024-01-23 10:41:17.114958 golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
+-rw-r--r--   0        0        0     5467 2024-04-09 07:23:27.117157 golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
+-rw-r--r--   0        0        0     1567 2024-01-23 10:41:17.114958 golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/payment_platform.py
+-rw-r--r--   0        0        0     2441 2024-01-05 09:59:46.197955 golem_core-0.7.3/golem/managers/proposal/plugins/reject_costs_exceeds.py
+-rw-r--r--   0        0        0      738 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/__init__.py
+-rw-r--r--   0        0        0     1738 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/map.py
+-rw-r--r--   0        0        0     4008 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/mixins.py
+-rw-r--r--   0        0        0     1938 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/pricings.py
+-rw-r--r--   0        0        0     3457 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py
+-rw-r--r--   0        0        0      505 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/random.py
+-rw-r--r--   0        0        0     4217 2024-05-28 13:12:06.279559 golem_core-0.7.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py
+-rw-r--r--   0        0        0      996 2023-10-13 09:42:33.129828 golem_core-0.7.3/golem/managers/proposal/plugins/whitelist.py
+-rw-r--r--   0        0        0      474 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/managers/work/__init__.py
+-rw-r--r--   0        0        0     2087 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/work/concurrent.py
+-rw-r--r--   0        0        0     2024 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/work/mixins.py
+-rw-r--r--   0        0        0     2038 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/managers/work/plugins.py
+-rw-r--r--   0        0        0     1201 2023-10-10 09:27:48.019544 golem_core-0.7.3/golem/managers/work/sequential.py
+-rw-r--r--   0        0        0      257 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/node/__init__.py
+-rw-r--r--   0        0        0      856 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/node/events.py
+-rw-r--r--   0        0        0    16726 2024-05-24 12:15:32.449823 golem_core-0.7.3/golem/node/node.py
+-rw-r--r--   0        0        0     1153 2023-11-30 13:59:47.049268 golem_core-0.7.3/golem/payload/__init__.py
+-rw-r--r--   0        0        0     6649 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/payload/base.py
+-rw-r--r--   0        0        0     1939 2023-11-30 13:59:47.049268 golem_core-0.7.3/golem/payload/constraints.py
+-rw-r--r--   0        0        0     5157 2024-05-24 12:15:32.449823 golem_core-0.7.3/golem/payload/defaults.py
+-rw-r--r--   0        0        0      284 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/payload/exceptions.py
+-rw-r--r--   0        0        0      973 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/payload/generic.py
+-rw-r--r--   0        0        0     1405 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/payload/mixins.py
+-rw-r--r--   0        0        0     1186 2024-01-08 09:28:36.246646 golem_core-0.7.3/golem/payload/parser.py
+-rw-r--r--   0        0        0      621 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/payload/parser.tx
+-rw-r--r--   0        0        0      868 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/payload/properties.py
+-rw-r--r--   0        0        0     5677 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/payload/vm.py
+-rw-r--r--   0        0        0      504 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/__init__.py
+-rw-r--r--   0        0        0     4535 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/buffer.py
+-rw-r--r--   0        0        0     1847 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/chain.py
+-rw-r--r--   0        0        0     3704 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/default_payment_handler.py
+-rw-r--r--   0        0        0     1363 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/exceptions.py
+-rw-r--r--   0        0        0      842 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/limit.py
+-rw-r--r--   0        0        0     3990 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/map.py
+-rw-r--r--   0        0        0     4152 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/pipeline/sort.py
+-rw-r--r--   0        0        0     2453 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/pipeline/zip.py
+-rw-r--r--   0        0        0     3462 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/resources/__init__.py
+-rw-r--r--   0        0        0      592 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/activity/__init__.py
+-rw-r--r--   0        0        0     6327 2024-03-28 09:34:26.737805 golem_core-0.7.3/golem/resources/activity/activity.py
+-rw-r--r--   0        0        0     6903 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/activity/commands.py
+-rw-r--r--   0        0        0      391 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/activity/events.py
+-rw-r--r--   0        0        0      735 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/activity/pipeline.py
+-rw-r--r--   0        0        0      360 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/agreement/__init__.py
+-rw-r--r--   0        0        0     6718 2024-04-11 10:33:47.493987 golem_core-0.7.3/golem/resources/agreement/agreement.py
+-rw-r--r--   0        0        0      375 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/resources/agreement/data.py
+-rw-r--r--   0        0        0      400 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/agreement/events.py
+-rw-r--r--   0        0        0      289 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/agreement/pipeline.py
+-rw-r--r--   0        0        0      410 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/allocation/__init__.py
+-rw-r--r--   0        0        0     3220 2024-03-05 09:03:20.980633 golem_core-0.7.3/golem/resources/allocation/allocation.py
+-rw-r--r--   0        0        0      409 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/allocation/events.py
+-rw-r--r--   0        0        0      835 2023-09-13 08:05:36.800448 golem_core-0.7.3/golem/resources/allocation/exceptions.py
+-rw-r--r--   0        0        0    11150 2024-03-28 09:34:26.737805 golem_core-0.7.3/golem/resources/base.py
+-rw-r--r--   0        0        0      372 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/debit_note/__init__.py
+-rw-r--r--   0        0        0     9169 2024-04-11 10:33:47.493987 golem_core-0.7.3/golem/resources/debit_note/debit_note.py
+-rw-r--r--   0        0        0      784 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/debit_note/event_collectors.py
+-rw-r--r--   0        0        0      402 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/debit_note/events.py
+-rw-r--r--   0        0        0      379 2023-11-30 13:59:47.049268 golem_core-0.7.3/golem/resources/demand/__init__.py
+-rw-r--r--   0        0        0      315 2023-11-30 13:59:47.049268 golem_core-0.7.3/golem/resources/demand/data.py
+-rw-r--r--   0        0        0     5532 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/demand/demand.py
+-rw-r--r--   0        0        0     2959 2023-11-25 08:20:36.566756 golem_core-0.7.3/golem/resources/demand/demand_builder.py
+-rw-r--r--   0        0        0      373 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/demand/events.py
+-rw-r--r--   0        0        0     1559 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/event_collectors.py
+-rw-r--r--   0        0        0     4215 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/events.py
+-rw-r--r--   0        0        0     1016 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/exceptions.py
+-rw-r--r--   0        0        0      340 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/invoice/__init__.py
+-rw-r--r--   0        0        0      760 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/invoice/event_collectors.py
+-rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/invoice/events.py
+-rw-r--r--   0        0        0     5307 2024-04-11 10:33:47.493987 golem_core-0.7.3/golem/resources/invoice/invoice.py
+-rw-r--r--   0        0        0      394 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/network/__init__.py
+-rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/network/events.py
+-rw-r--r--   0        0        0      590 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/network/exceptions.py
+-rw-r--r--   0        0        0     5803 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/network/network.py
+-rw-r--r--   0        0        0      509 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/pooling_batch/__init__.py
+-rw-r--r--   0        0        0      456 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/pooling_batch/events.py
+-rw-r--r--   0        0        0     2122 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/pooling_batch/exceptions.py
+-rw-r--r--   0        0        0     5510 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/pooling_batch/pooling_batch.py
+-rw-r--r--   0        0        0      499 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/proposal/__init__.py
+-rw-r--r--   0        0        0      508 2023-11-30 13:59:47.049268 golem_core-0.7.3/golem/resources/proposal/data.py
+-rw-r--r--   0        0        0      391 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/proposal/events.py
+-rw-r--r--   0        0        0      664 2023-11-02 09:14:12.503044 golem_core-0.7.3/golem/resources/proposal/exceptions.py
+-rw-r--r--   0        0        0      860 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/resources/proposal/pipeline.py
+-rw-r--r--   0        0        0     9303 2024-02-20 09:06:29.551136 golem_core-0.7.3/golem/resources/proposal/proposal.py
+-rw-r--r--   0        0        0        0 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/utils/__init__.py
+-rw-r--r--   0        0        0      626 2024-03-05 09:03:20.984633 golem_core-0.7.3/golem/resources/utils/infrastructure.py
+-rw-r--r--   0        0        0     6911 2024-04-17 13:30:09.635204 golem_core-0.7.3/golem/resources/utils/payment.py
+-rw-r--r--   0        0        0        0 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/__init__.py
+-rw-r--r--   0        0        0      704 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/utils/asyncio/__init__.py
+-rw-r--r--   0        0        0    13829 2024-05-29 14:12:26.327190 golem_core-0.7.3/golem/utils/asyncio/buffer.py
+-rw-r--r--   0        0        0     2044 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/utils/asyncio/queue.py
+-rw-r--r--   0        0        0     2056 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/utils/asyncio/semaphore.py
+-rw-r--r--   0        0        0     2820 2024-04-09 07:23:27.117157 golem_core-0.7.3/golem/utils/asyncio/tasks.py
+-rw-r--r--   0        0        0     1726 2024-02-08 13:35:10.791354 golem_core-0.7.3/golem/utils/asyncio/waiter.py
+-rw-r--r--   0        0        0      741 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/http.py
+-rw-r--r--   0        0        0     7521 2024-02-08 13:35:10.795401 golem_core-0.7.3/golem/utils/logging.py
+-rw-r--r--   0        0        0      307 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/low/__init__.py
+-rw-r--r--   0        0        0     6571 2024-05-24 12:15:32.449823 golem_core-0.7.3/golem/utils/low/api.py
+-rw-r--r--   0        0        0     3323 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/low/event_collector.py
+-rw-r--r--   0        0        0      105 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/storage/__init__.py
+-rw-r--r--   0        0        0     4024 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/storage/base.py
+-rw-r--r--   0        0        0       88 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/storage/gftp/__init__.py
+-rw-r--r--   0        0        0    16077 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/storage/gftp/provider.py
+-rw-r--r--   0        0        0      673 2023-09-13 08:05:36.804448 golem_core-0.7.3/golem/utils/storage/utils.py
+-rw-r--r--   0        0        0      767 2024-02-08 13:35:10.795401 golem_core-0.7.3/golem/utils/typing.py
+-rw-r--r--   0        0        0     4722 2024-05-29 14:17:32.181602 golem_core-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 golem_core-0.7.3/PKG-INFO
```

### Comparing `golem_core-0.7.1/LICENSE` & `golem_core-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/cli/cli.py` & `golem_core-0.7.3/golem/cli/cli.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/cli/utils.py` & `golem_core-0.7.3/golem/cli/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/event_bus/base.py` & `golem_core-0.7.3/golem/event_bus/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/event_bus/in_memory/event_bus.py` & `golem_core-0.7.3/golem/event_bus/in_memory/event_bus.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/__init__.py` & `golem_core-0.7.3/golem/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/activity/mixins.py` & `golem_core-0.7.3/golem/managers/activity/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/activity/pool.py` & `golem_core-0.7.3/golem/managers/activity/pool.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/activity/single_use.py` & `golem_core-0.7.3/golem/managers/activity/single_use.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/agreement/default.py` & `golem_core-0.7.3/golem/managers/agreement/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/base.py` & `golem_core-0.7.3/golem/managers/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/demand/aggregating.py` & `golem_core-0.7.3/golem/managers/demand/aggregating.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/demand/refreshing.py` & `golem_core-0.7.3/golem/managers/demand/refreshing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/mixins.py` & `golem_core-0.7.3/golem/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/network/single.py` & `golem_core-0.7.3/golem/managers/network/single.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/payment/default.py` & `golem_core-0.7.3/golem/managers/payment/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             raise ManagerException(json.loads(e.body)["message"]) from e
 
     @trace_span("Stopping DefaultPaymentManager", log_level=logging.INFO)
     async def stop(self):
         """Terminate all related agreements."""
         try:
             await asyncio.wait_for(self._wait_for_invoices(), timeout=self._shutdown_timeout)
-        except TimeoutError:
+        except asyncio.TimeoutError:
             logger.error(
                 "Waiting for invoices failed with timeout! Those agreements did not sent invoices:"
                 f" {[a for a in self._agreements]}"
             )
 
         await asyncio.gather(*[agreement.close_all() for agreement in self._agreements.values()])
         self._agreements.clear()
```

### Comparing `golem_core-0.7.1/golem/managers/proposal/__init__.py` & `golem_core-0.7.3/golem/managers/proposal/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/default.py` & `golem_core-0.7.3/golem/managers/proposal/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/__init__.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/blacklist.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/blacklist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/buffer.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/buffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 import logging
 import re
 from datetime import timedelta
 from typing import Callable, Optional
 
 from ya_market import ApiException
@@ -31,14 +32,16 @@
         self._min_size = min_size
         self._max_size = max_size
         self._fill_concurrency_size = fill_concurrency_size
         self._fill_at_start = fill_at_start
         self._get_expiration_func = get_expiration_func
         self._on_expiration_func = on_expiration_func
 
+        self._proposal_semaphore = asyncio.Semaphore(value=max_size)
+
         # TODO: Consider moving buffer composition from here to plugin level
         buffer: Buffer[Proposal] = SimpleBuffer()
 
         if self._get_expiration_func:
             buffer = ExpirableBuffer(
                 buffer=buffer,
                 get_expiration_func=self._get_expiration_func,
@@ -116,35 +119,36 @@
             self._max_size,
         )
 
         await self._buffer.request(requested)
 
     @trace_span(show_results=True)
     async def get_proposal(self) -> Proposal:
-        if not self._get_buffered_proposals_count():
-            logger.debug("No proposals to get, requesting fill")
-            await self._request_proposals()
-
-        proposal = await self._get_buffered_proposal()
-
-        proposals_count = self._get_buffered_proposals_count()
-        if proposals_count < self._min_size:
-            logger.debug(
-                "Proposals count %d is below minimum size %d, requesting fill",
-                proposals_count,
-                self._min_size,
-            )
-            await self._request_proposals()
-        else:
-            logger.debug(
-                "Proposals count %d is above minimum size %d, skipping fill",
-                proposals_count,
-                self._min_size,
-            )
+        async with self._proposal_semaphore:
+            if not self._get_buffered_proposals_count():
+                logger.debug("No proposals to get, requesting fill")
+                await self._request_proposals()
+
+            proposal = await self._get_buffered_proposal()
+
+            proposals_count = self._get_buffered_proposals_count()
+            if proposals_count < self._min_size:
+                logger.debug(
+                    "Proposals count %d is below minimum size %d, requesting fill",
+                    proposals_count,
+                    self._min_size,
+                )
+                await self._request_proposals()
+            else:
+                logger.debug(
+                    "Proposals count %d is above minimum size %d, skipping fill",
+                    proposals_count,
+                    self._min_size,
+                )
 
-        return proposal
+            return proposal
 
     async def _get_buffered_proposal(self) -> Proposal:
         return await self._buffer.get()
 
     def _get_buffered_proposals_count(self) -> int:
         return self._buffer.size()
```

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/linear_coeffs.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/linear_coeffs.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/negotiating/payment_platform.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/negotiating/payment_platform.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/reject_costs_exceeds.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/reject_costs_exceeds.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/__init__.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/map.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/mixins.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/pricings.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/pricings.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/property_value_lerp.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/scoring/scoring_buffer.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/proposal/plugins/whitelist.py` & `golem_core-0.7.3/golem/managers/proposal/plugins/whitelist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/work/concurrent.py` & `golem_core-0.7.3/golem/managers/work/concurrent.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/work/mixins.py` & `golem_core-0.7.3/golem/managers/work/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/work/plugins.py` & `golem_core-0.7.3/golem/managers/work/plugins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/managers/work/sequential.py` & `golem_core-0.7.3/golem/managers/work/sequential.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/node/events.py` & `golem_core-0.7.3/golem/node/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/node/node.py` & `golem_core-0.7.3/golem/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,35 +49,35 @@
 
     """
 
     def __init__(
         self,
         app_key: Optional[str] = None,
         *,
-        base_url: Optional[str] = None,
+        api_url: Optional[str] = None,
         collect_payment_events: bool = True,
         app_session_id: Optional[Union[str, Type[_RandomSessionId]]] = _RandomSessionId,
     ):
         """Init GolemNode.
 
         :param app_key: App key used as an authentication token for all `yagna` calls.
                         Defaults to the `YAGNA_APPKEY` env variable.
-        :param base_url: Base url for all `yagna` APIs. Defaults to `YAGNA_API_URL` env
+        :param api_url: Base url for all `yagna` APIs. Defaults to `YAGNA_API_URL` env
                          variable or http://127.0.0.1:7465.
         :param collect_payment_events: If True, GolemNode will watch for incoming
             debit notes/invoices and create corresponding objects (--> :any:`NewResource` events
             will be emitted).
         :param app_session_id: A correlation/session identifier. :any:`GolemNode` objects with the
             same `app_session_id` will receive the same debit note/invoice/agreement events.
             Defaults to a random sting. If set to `None`, this GolemNode will receive all events
             regardless of their corresponding session ids.
         """
         config_kwargs = {
             param: value
-            for param, value in {"app_key": app_key, "base_url": base_url}.items()
+            for param, value in {"app_key": app_key, "api_url": api_url}.items()
             if value is not None
         }
         self._api_config = ApiConfig(**config_kwargs)
         self._collect_payment_events = collect_payment_events
         self.app_session_id = uuid4().hex if app_session_id is _RandomSessionId else app_session_id
 
         #   All created Resources will be stored here
```

### Comparing `golem_core-0.7.1/golem/payload/__init__.py` & `golem_core-0.7.3/golem/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/base.py` & `golem_core-0.7.3/golem/payload/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/constraints.py` & `golem_core-0.7.3/golem/payload/constraints.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/defaults.py` & `golem_core-0.7.3/golem/payload/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 PROP_PAYMENT_TIMEOUT = "golem.com.scheme.payu.payment-timeout-sec?"
 
 PROP_PRICING_MODEL = "golem.com.pricing.model"
 PROP_PRICING_LINEAR_COEFFS = "golem.com.pricing.model.linear.coeffs"
 PROP_USAGE_VECTOR = "golem.com.usage.vector"
 
 DEFAULT_PAYMENT_DRIVER: str = getenv("YAGNA_PAYMENT_DRIVER", "erc20").lower()
-DEFAULT_PAYMENT_NETWORK: str = getenv("YAGNA_PAYMENT_NETWORK", "goerli").lower()
+DEFAULT_PAYMENT_NETWORK: str = getenv("YAGNA_PAYMENT_NETWORK", "holesky").lower()
 
 DEFAULT_LIFETIME = timedelta(minutes=30)
 DEFAULT_SUBNET: str = getenv("YAGNA_SUBNET", "public")
 
 
 @dataclass
 class NodeInfo(Payload):
```

### Comparing `golem_core-0.7.1/golem/payload/generic.py` & `golem_core-0.7.3/golem/payload/generic.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/mixins.py` & `golem_core-0.7.3/golem/payload/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/parser.py` & `golem_core-0.7.3/golem/payload/parser.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/parser.tx` & `golem_core-0.7.3/golem/payload/parser.tx`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/properties.py` & `golem_core-0.7.3/golem/payload/properties.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/payload/vm.py` & `golem_core-0.7.3/golem/payload/vm.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/buffer.py` & `golem_core-0.7.3/golem/pipeline/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/chain.py` & `golem_core-0.7.3/golem/pipeline/chain.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/default_payment_handler.py` & `golem_core-0.7.3/golem/pipeline/default_payment_handler.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/exceptions.py` & `golem_core-0.7.3/golem/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/limit.py` & `golem_core-0.7.3/golem/pipeline/limit.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/map.py` & `golem_core-0.7.3/golem/pipeline/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/sort.py` & `golem_core-0.7.3/golem/pipeline/sort.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/pipeline/zip.py` & `golem_core-0.7.3/golem/pipeline/zip.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/__init__.py` & `golem_core-0.7.3/golem/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/activity/__init__.py` & `golem_core-0.7.3/golem/resources/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/activity/activity.py` & `golem_core-0.7.3/golem/resources/activity/activity.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/activity/commands.py` & `golem_core-0.7.3/golem/resources/activity/commands.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/activity/pipeline.py` & `golem_core-0.7.3/golem/resources/activity/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/agreement/agreement.py` & `golem_core-0.7.3/golem/resources/agreement/agreement.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/allocation/allocation.py` & `golem_core-0.7.3/golem/resources/allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/allocation/exceptions.py` & `golem_core-0.7.3/golem/resources/allocation/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/base.py` & `golem_core-0.7.3/golem/resources/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/debit_note/debit_note.py` & `golem_core-0.7.3/golem/resources/debit_note/debit_note.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/debit_note/event_collectors.py` & `golem_core-0.7.3/golem/resources/debit_note/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/demand/demand.py` & `golem_core-0.7.3/golem/resources/demand/demand.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/demand/demand_builder.py` & `golem_core-0.7.3/golem/resources/demand/demand_builder.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/event_collectors.py` & `golem_core-0.7.3/golem/resources/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/events.py` & `golem_core-0.7.3/golem/resources/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/exceptions.py` & `golem_core-0.7.3/golem/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/invoice/event_collectors.py` & `golem_core-0.7.3/golem/resources/invoice/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/invoice/invoice.py` & `golem_core-0.7.3/golem/resources/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/network/exceptions.py` & `golem_core-0.7.3/golem/resources/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/network/network.py` & `golem_core-0.7.3/golem/resources/network/network.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/pooling_batch/exceptions.py` & `golem_core-0.7.3/golem/resources/pooling_batch/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/pooling_batch/pooling_batch.py` & `golem_core-0.7.3/golem/resources/pooling_batch/pooling_batch.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/proposal/exceptions.py` & `golem_core-0.7.3/golem/resources/proposal/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/proposal/pipeline.py` & `golem_core-0.7.3/golem/resources/proposal/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/proposal/proposal.py` & `golem_core-0.7.3/golem/resources/proposal/proposal.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/utils/infrastructure.py` & `golem_core-0.7.3/golem/resources/utils/infrastructure.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/resources/utils/payment.py` & `golem_core-0.7.3/golem/resources/utils/payment.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/asyncio/__init__.py` & `golem_core-0.7.3/golem/utils/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/asyncio/buffer.py` & `golem_core-0.7.3/golem/utils/asyncio/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 class ComposableBuffer(Buffer[TItem]):
     """Utility class for composable/stackable buffer implementations to help with calling \
     the underlying buffer."""
 
     def __init__(self, buffer: Buffer[TItem]):
         self._buffer = buffer
 
+    @property
+    def condition(self):
+        return self._buffer.condition
+
     @asynccontextmanager
     async def _handle_lock(self, lock: bool):
         if lock:
             async with self._buffer.condition:
                 yield
         else:
             yield
```

### Comparing `golem_core-0.7.1/golem/utils/asyncio/queue.py` & `golem_core-0.7.3/golem/utils/asyncio/queue.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/asyncio/semaphore.py` & `golem_core-0.7.3/golem/utils/asyncio/semaphore.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/asyncio/tasks.py` & `golem_core-0.7.3/golem/utils/asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/asyncio/waiter.py` & `golem_core-0.7.3/golem/utils/asyncio/waiter.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/http.py` & `golem_core-0.7.3/golem/utils/http.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/logging.py` & `golem_core-0.7.3/golem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/low/api.py` & `golem_core-0.7.3/golem/utils/low/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         if self.app_key is None:
             raise MissingConfiguration(key="YAGNA_APPKEY", description="API authentication token")
         self.market_url: str = self.__resolve_url(self.market_url, "/market-api/v1")
         self.payment_url: str = self.__resolve_url(self.payment_url, "/payment-api/v1")
         self.activity_url: str = self.__resolve_url(self.activity_url, "/activity-api/v1")
         self.net_url: str = self.__resolve_url(self.net_url, "/net-api/v1")
 
-    def __resolve_url(self, given_url: Optional[str], prefix: str) -> str:
-        return given_url or f"{self.api_url}{prefix}"
+    def __resolve_url(self, given_url: Optional[str], suffix: str) -> str:
+        return given_url or f"{self.api_url}{suffix}"
 
 
 class ApiFactory(object):
     """
     REST API's setup and top-level access utility.
 
     By default, it expects the yagna daemon to be available locally and listening on the
```

### Comparing `golem_core-0.7.1/golem/utils/low/event_collector.py` & `golem_core-0.7.3/golem/utils/low/event_collector.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/storage/base.py` & `golem_core-0.7.3/golem/utils/storage/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/storage/gftp/provider.py` & `golem_core-0.7.3/golem/utils/storage/gftp/provider.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/storage/utils.py` & `golem_core-0.7.3/golem/utils/storage/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/golem/utils/typing.py` & `golem_core-0.7.3/golem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.7.1/pyproject.toml` & `golem_core-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "golem-core"
-version = "0.7.1"
+version = "0.7.3"
 description = "Golem Network (https://golem.network/) API for Python"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `golem_core-0.7.1/PKG-INFO` & `golem_core-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: golem-core
-Version: 0.7.1
+Version: 0.7.3
 Summary: Golem Network (https://golem.network/) API for Python
 Home-page: https://github.com/golemfactory/golem-core-python
 License: LGPL-3.0-or-later
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: async-exit-stack (==1.0.1)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jsonrpc-base (>=1.0.3,<2.0.0)
 Requires-Dist: prettytable (>=3.4.1,<4.0.0)
 Requires-Dist: semantic-version (>=2.8,<3.0)
```

