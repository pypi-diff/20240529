# Comparing `tmp/nucliadb-4.0.1.post553-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.1.post554-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,471 +1,473 @@
-Zip file size: 768043 bytes, number of entries: 469
--rw-r--r--  2.0 unx     1135 b- defN 24-May-29 12:14 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-29 12:14 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-29 12:14 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-29 12:14 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-29 12:14 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-29 12:14 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-29 12:14 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-29 12:14 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-29 12:14 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-29 12:14 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-29 12:14 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-29 12:14 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-29 12:14 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-29 12:14 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-29 12:14 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-29 12:14 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-29 12:14 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-29 12:14 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-29 12:14 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-29 12:14 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-29 12:14 nucliadb/health.py
--rw-r--r--  2.0 unx    11793 b- defN 24-May-29 12:14 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-29 12:14 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-29 12:14 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-29 12:14 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5134 b- defN 24-May-29 12:14 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-29 12:14 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-29 12:14 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-29 12:14 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22378 b- defN 24-May-29 12:14 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-29 12:14 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20532 b- defN 24-May-29 12:14 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-29 12:14 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-29 12:14 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-29 12:14 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-29 12:14 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-29 12:14 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-29 12:14 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-29 12:14 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-29 12:14 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-29 12:14 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1940 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     2651 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    12177 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     3305 b- defN 24-May-29 12:14 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-29 12:14 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-29 12:14 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-29 12:14 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-29 12:14 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-29 12:14 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-29 12:14 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-29 12:14 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-29 12:14 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-29 12:14 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-29 12:14 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-29 12:14 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-29 12:14 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-29 12:14 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-29 12:14 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-29 12:14 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-29 12:14 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-29 12:14 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-29 12:14 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-29 12:14 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-29 12:14 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-29 12:14 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-29 12:14 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-29 12:14 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-29 12:14 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-29 12:14 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/ingest/py.typed
--rw-r--r--  2.0 unx    20277 b- defN 24-May-29 12:14 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-29 12:14 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-29 12:14 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-29 12:14 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-29 12:14 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-29 12:14 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-29 12:14 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-29 12:14 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-29 12:14 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-29 12:14 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-29 12:14 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-29 12:14 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-29 12:14 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-29 12:14 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-29 12:14 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-29 12:14 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-29 12:14 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    15621 b- defN 24-May-29 12:14 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-29 12:14 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    58955 b- defN 24-May-29 12:14 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-29 12:14 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-29 12:14 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-29 12:14 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-29 12:14 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-29 12:14 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    30462 b- defN 24-May-29 12:14 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-29 12:14 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24111 b- defN 24-May-29 12:14 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-29 12:14 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-29 12:14 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-29 12:14 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-29 12:14 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-29 12:14 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-29 12:14 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-29 12:14 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-29 12:14 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-29 12:14 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-29 12:14 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-29 12:14 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-29 12:14 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-29 12:14 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-29 12:14 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-29 12:14 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-29 12:14 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-29 12:14 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-29 12:14 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-29 12:14 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-29 12:14 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/reader/py.typed
--rw-r--r--  2.0 unx     1447 b- defN 24-May-29 12:14 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-29 12:14 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-29 12:14 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12457 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-29 12:14 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-29 12:14 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-29 12:14 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-29 12:14 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-29 12:14 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-29 12:14 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-29 12:14 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-29 12:14 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-29 12:14 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-29 12:14 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-29 12:14 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-29 12:14 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-29 12:14 nucliadb/search/predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/search/py.typed
--rw-r--r--  2.0 unx     1402 b- defN 24-May-29 12:14 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-29 12:14 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-29 12:14 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-29 12:14 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-29 12:14 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-29 12:14 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-29 12:14 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-29 12:14 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-29 12:14 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-29 12:14 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-29 12:14 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-29 12:14 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-29 12:14 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-29 12:14 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-29 12:14 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-29 12:14 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-29 12:14 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-29 12:14 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-29 12:14 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-29 12:14 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-29 12:14 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-29 12:14 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-29 12:14 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-29 12:14 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-29 12:14 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-29 12:14 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-29 12:14 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-29 12:14 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-29 12:14 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-29 12:14 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-29 12:14 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-29 12:14 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-29 12:14 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-29 12:14 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-29 12:14 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-29 12:14 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-29 12:14 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-29 12:14 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-29 12:14 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-29 12:14 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-29 12:14 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-29 12:14 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-29 12:14 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-29 12:14 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-29 12:14 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-29 12:14 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-29 12:14 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-29 12:14 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-29 12:14 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/standalone/py.typed
--rw-r--r--  2.0 unx     5636 b- defN 24-May-29 12:14 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-29 12:14 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-29 12:14 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-29 12:14 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-29 12:14 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-29 12:14 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-29 12:14 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-29 12:14 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-29 12:14 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-29 12:14 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-29 12:14 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-29 12:14 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-29 12:14 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-29 12:14 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-29 12:14 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-29 12:14 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-29 12:14 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-29 12:14 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-29 12:14 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-29 12:14 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-29 12:14 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-29 12:14 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-29 12:14 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-29 12:14 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-29 12:14 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-29 12:14 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-29 12:14 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-29 12:14 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-29 12:14 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-29 12:14 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-29 12:14 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-29 12:14 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-29 12:14 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-29 12:14 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-29 12:14 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-29 12:14 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-29 12:14 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-29 12:14 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-29 12:14 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-29 12:14 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-29 12:14 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-29 12:14 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-29 12:14 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-29 12:14 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-29 12:14 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-29 12:14 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-29 12:14 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/train/py.typed
--rw-r--r--  2.0 unx     1400 b- defN 24-May-29 12:14 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-29 12:14 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-29 12:14 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-29 12:14 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-29 12:14 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-29 12:14 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-29 12:14 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-29 12:14 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-29 12:14 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-29 12:14 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-29 12:14 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-29 12:14 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-29 12:14 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-29 12:14 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-29 12:14 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-29 12:14 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-29 12:14 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-29 12:14 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-29 12:14 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-29 12:14 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-29 12:14 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-29 12:14 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-29 12:14 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-29 12:14 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-29 12:14 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-29 12:14 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-29 12:14 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2201 b- defN 24-May-29 12:14 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-29 12:14 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-29 12:14 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-29 12:14 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-29 12:14 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-29 12:14 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-29 12:14 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-29 12:14 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-29 12:14 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-29 12:14 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-29 12:14 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-29 12:14 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-29 12:14 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-29 12:14 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-29 12:14 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-29 12:14 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-29 12:14 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-29 12:14 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 12:14 nucliadb/writer/py.typed
--rw-r--r--  2.0 unx     1448 b- defN 24-May-29 12:14 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-29 12:14 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-29 12:14 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-29 12:14 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-May-29 12:14 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-29 12:14 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-29 12:14 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-29 12:14 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-29 12:14 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-29 12:14 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-29 12:14 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-29 12:14 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-29 12:14 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-29 12:14 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-29 12:14 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-29 12:14 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-29 12:14 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-29 12:14 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-29 12:14 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-29 12:14 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-29 12:14 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-29 12:14 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-29 12:14 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-29 12:14 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-29 12:14 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4474 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43936 b- defN 24-May-29 12:16 nucliadb-4.0.1.post553.dist-info/RECORD
-469 files, 2265810 bytes uncompressed, 697775 bytes compressed:  69.2%
+Zip file size: 770586 bytes, number of entries: 471
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-29 14:07 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-29 14:07 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-29 14:07 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-29 14:07 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-29 14:07 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-29 14:07 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-29 14:07 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-29 14:07 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-29 14:07 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-29 14:07 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-29 14:07 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-29 14:07 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-29 14:07 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-29 14:07 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-29 14:07 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-29 14:07 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-29 14:07 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-29 14:07 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-29 14:07 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx     1734 b- defN 24-May-29 14:07 migrations/0021_overwrite_vectorsets_key.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-29 14:07 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-29 14:07 nucliadb/health.py
+-rw-r--r--  2.0 unx    11793 b- defN 24-May-29 14:07 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-29 14:07 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-29 14:07 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-29 14:07 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5134 b- defN 24-May-29 14:07 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-29 14:07 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-29 14:07 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-29 14:07 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    23442 b- defN 24-May-29 14:07 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-29 14:07 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-May-29 14:07 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-29 14:07 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-29 14:07 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-29 14:07 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-29 14:07 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-29 14:07 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-29 14:07 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-29 14:07 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-29 14:07 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-29 14:07 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1940 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-May-29 14:07 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-29 14:07 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-29 14:07 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-29 14:07 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-29 14:07 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-29 14:07 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-29 14:07 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-29 14:07 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-29 14:07 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-29 14:07 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-29 14:07 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-29 14:07 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-29 14:07 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-29 14:07 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-29 14:07 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-29 14:07 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-29 14:07 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-29 14:07 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-29 14:07 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-29 14:07 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-29 14:07 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-29 14:07 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-29 14:07 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-29 14:07 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-29 14:07 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-29 14:07 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-29 14:07 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-29 14:07 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-29 14:07 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-29 14:07 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-29 14:07 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-29 14:07 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-29 14:07 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-29 14:07 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-29 14:07 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-29 14:07 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-29 14:07 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-29 14:07 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-29 14:07 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-29 14:07 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-29 14:07 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-29 14:07 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-29 14:07 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    15687 b- defN 24-May-29 14:07 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-29 14:07 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-29 14:07 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-29 14:07 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-29 14:07 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-29 14:07 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-29 14:07 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-29 14:07 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-29 14:07 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-29 14:07 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24111 b- defN 24-May-29 14:07 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-29 14:07 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-29 14:07 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-29 14:07 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-29 14:07 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-29 14:07 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-29 14:07 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-29 14:07 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-29 14:07 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-29 14:07 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-29 14:07 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-29 14:07 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-29 14:07 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-29 14:07 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-29 14:07 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-29 14:07 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-29 14:07 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-29 14:07 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-29 14:07 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-29 14:07 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-29 14:07 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-29 14:07 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-29 14:07 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-29 14:07 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12457 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-29 14:07 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-29 14:07 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-29 14:07 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-29 14:07 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-29 14:07 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-29 14:07 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-29 14:07 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-29 14:07 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-29 14:07 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-29 14:07 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-29 14:07 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-29 14:07 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-29 14:07 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-29 14:07 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-29 14:07 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-29 14:07 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-29 14:07 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-29 14:07 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-29 14:07 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-29 14:07 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-29 14:07 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-29 14:07 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-29 14:07 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-29 14:07 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-29 14:07 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-29 14:07 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-29 14:07 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-29 14:07 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-29 14:07 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-29 14:07 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-29 14:07 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-29 14:07 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-29 14:07 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-29 14:07 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-29 14:07 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-29 14:07 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-29 14:07 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-29 14:07 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-29 14:07 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-29 14:07 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-29 14:07 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-29 14:07 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-29 14:07 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-29 14:07 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-29 14:07 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-29 14:07 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-29 14:07 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-29 14:07 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-29 14:07 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-29 14:07 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-29 14:07 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-29 14:07 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-29 14:07 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-29 14:07 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-29 14:07 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-29 14:07 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-29 14:07 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-29 14:07 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-29 14:07 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-29 14:07 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-29 14:07 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-29 14:07 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-29 14:07 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-29 14:07 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-29 14:07 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-29 14:07 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-29 14:07 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-29 14:07 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-29 14:07 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-29 14:07 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-29 14:07 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-29 14:07 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-29 14:07 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-29 14:07 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-29 14:07 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-29 14:07 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-29 14:07 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-29 14:07 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-29 14:07 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-29 14:07 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-29 14:07 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-29 14:07 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-29 14:07 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-29 14:07 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-29 14:07 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-29 14:07 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-29 14:07 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-29 14:07 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-May-29 14:07 nucliadb/tests/migrations/test_migration_0021.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-29 14:07 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-29 14:07 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-29 14:07 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-29 14:07 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-29 14:07 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-29 14:07 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-29 14:07 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-29 14:07 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-29 14:07 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-29 14:07 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-29 14:07 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-29 14:07 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-29 14:07 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-29 14:07 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-29 14:07 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-29 14:07 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-29 14:07 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-29 14:07 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-29 14:07 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-29 14:07 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-29 14:07 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-29 14:07 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-29 14:07 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-29 14:07 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-29 14:07 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-29 14:07 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-29 14:07 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-29 14:07 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-29 14:07 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-29 14:07 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-29 14:07 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-29 14:07 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-29 14:07 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-29 14:07 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-29 14:07 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-29 14:07 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-29 14:07 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-29 14:07 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-29 14:07 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-29 14:07 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-29 14:07 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-29 14:07 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-29 14:07 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-29 14:07 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-29 14:07 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-29 14:07 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-29 14:07 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-29 14:07 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-May-29 14:07 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-29 14:07 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-29 14:07 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-29 14:07 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-29 14:07 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-29 14:07 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-29 14:07 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-29 14:07 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-29 14:07 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-29 14:07 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-29 14:07 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-29 14:07 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-29 14:07 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-29 14:07 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-29 14:07 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-29 14:07 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-29 14:07 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-29 14:07 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 14:07 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-29 14:07 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-29 14:07 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-29 14:07 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-29 14:07 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-May-29 14:07 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-29 14:07 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-29 14:07 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-29 14:07 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-29 14:07 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-29 14:07 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-29 14:07 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-29 14:07 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-29 14:07 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-29 14:07 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-29 14:07 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-29 14:07 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-29 14:07 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-29 14:07 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-29 14:07 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-29 14:07 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-29 14:07 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-29 14:07 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-29 14:07 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-29 14:07 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-29 14:07 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    44141 b- defN 24-May-29 14:08 nucliadb-4.0.1.post554.dist-info/RECORD
+471 files, 2272793 bytes uncompressed, 699984 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -51,14 +51,17 @@
 
 Filename: migrations/0019_upgrade_to_paragraphs_v3.py
 Comment: 
 
 Filename: migrations/0020_drain_nodes_from_cluster.py
 Comment: 
 
+Filename: migrations/0021_overwrite_vectorsets_key.py
+Comment: 
+
 Filename: migrations/__init__.py
 Comment: 
 
 Filename: nucliadb/__init__.py
 Comment: 
 
 Filename: nucliadb/health.py
@@ -972,14 +975,17 @@
 
 Filename: nucliadb/tests/migrations/test_migration_0017.py
 Comment: 
 
 Filename: nucliadb/tests/migrations/test_migration_0018.py
 Comment: 
 
+Filename: nucliadb/tests/migrations/test_migration_0021.py
+Comment: 
+
 Filename: nucliadb/tests/unit/__init__.py
 Comment: 
 
 Filename: nucliadb/tests/unit/test_field_ids.py
 Comment: 
 
 Filename: nucliadb/tests/unit/test_health.py
@@ -1383,26 +1389,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/METADATA
+Filename: nucliadb-4.0.1.post554.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/WHEEL
+Filename: nucliadb-4.0.1.post554.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/entry_points.txt
+Filename: nucliadb-4.0.1.post554.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/top_level.txt
+Filename: nucliadb-4.0.1.post554.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/zip-safe
+Filename: nucliadb-4.0.1.post554.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.1.post553.dist-info/RECORD
+Filename: nucliadb-4.0.1.post554.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## migrations/0018_purge_orphan_kbslugs.py

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-"""Migration #17
+"""Migration #18
 
 Due to a bug on backend services, some kbslugs were not properly deleted and got
 orphan. Let's delete them!
 
 """
 import logging
```

## nucliadb/common/cluster/manager.py

```diff
@@ -242,14 +242,37 @@
                         vector_index_config=vector_index_config,
                     )
                 except Exception as e:
                     errors.capture_exception(e)
                     logger.exception(f"Error creating new shard at {node}: {e}")
                     continue
 
+                shard_id = shard_created.id
+                try:
+                    async for vectorset_config in datamanagers.vectorsets.iter(
+                        txn, kbid=kbid
+                    ):
+                        response = await node.add_vectorset(
+                            shard_id,
+                            vectorset=vectorset_config.vectorset_id,
+                            config=vectorset_config.vectorset_index_config,
+                        )
+                        if response.status != response.Status.OK:
+                            raise Exception(response.detail)
+                except Exception as e:
+                    errors.capture_exception(e)
+                    logger.exception(
+                        "Error creating vectorset '{vectorset_id}' new shard at {node}: {details}".format(
+                            vectorset_id=vectorset_config.vectorset_id,
+                            node=node,
+                            details=e,
+                        )
+                    )
+                    continue
+
                 replica = writer_pb2.ShardReplica(node=str(node_id))
                 replica.shard.CopyFrom(shard_created)
                 shard.replicas.append(replica)
                 replicas_created += 1
         except Exception as e:
             errors.capture_exception(e)
             logger.error(f"Unexpected error creating new shard: {e}")
```

## nucliadb/common/datamanagers/vectorsets.py

```diff
@@ -13,23 +13,30 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
-from typing import Optional
+from typing import AsyncIterator, Optional
 
 from nucliadb.common.datamanagers.utils import get_kv_pb
 from nucliadb.common.maindb.driver import Transaction
 from nucliadb_protos import knowledgebox_pb2
 
 KB_VECTORSETS = "/kbs/{kbid}/vectorsets"
 
 
+async def initialize(txn: Transaction, *, kbid: str):
+    key = KB_VECTORSETS.format(kbid=kbid)
+    await txn.set(
+        key, knowledgebox_pb2.KnowledgeBoxVectorSetsConfig().SerializeToString()
+    )
+
+
 async def get(
     txn: Transaction, *, kbid: str, vectorset_id: str
 ) -> Optional[knowledgebox_pb2.VectorSetConfig]:
     kb_vectorsets = await _get_or_default(txn, kbid=kbid)
     index = _find_vectorset(kb_vectorsets, vectorset_id)
     if index is None:
         return None
@@ -37,30 +44,38 @@
 
 
 async def exists(txn, *, kbid: str, vectorset_id: str) -> bool:
     kb_vectorsets = await _get_or_default(txn, kbid=kbid)
     return _find_vectorset(kb_vectorsets, vectorset_id) is not None
 
 
-async def set(txn, *, kbid: str, config: knowledgebox_pb2.VectorSetConfig):
+async def iter(
+    txn: Transaction, *, kbid: str
+) -> AsyncIterator[knowledgebox_pb2.VectorSetConfig]:
+    kb_vectorsets = await _get_or_default(txn, kbid=kbid)
+    for config in kb_vectorsets.vectorsets:
+        yield config
+
+
+async def set(txn: Transaction, *, kbid: str, config: knowledgebox_pb2.VectorSetConfig):
     """Create or update a vectorset configuration"""
     kb_vectorsets = await _get_or_default(txn, kbid=kbid)
     index = _find_vectorset(kb_vectorsets, config.vectorset_id)
     if index is None:
         # adding a new vectorset
         kb_vectorsets.vectorsets.append(config)
     else:
         # updating a vectorset
         kb_vectorsets.vectorsets[index].CopyFrom(config)
 
     key = KB_VECTORSETS.format(kbid=kbid)
     await txn.set(key, kb_vectorsets.SerializeToString())
 
 
-async def delete(txn, *, kbid: str, vectorset_id: str):
+async def delete(txn: Transaction, *, kbid: str, vectorset_id: str):
     kb_vectorsets = await _get_or_default(txn, kbid=kbid)
     index = _find_vectorset(kb_vectorsets, vectorset_id)
     if index is None:
         # already deleted
         return
 
     del kb_vectorsets.vectorsets[index]
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -128,14 +128,16 @@
         await txn.set(
             datamanagers.kb.KB_SLUGS.format(slug=slug),
             uuid.encode(),
         )
         if config is None:
             config = KnowledgeBoxConfig()
 
+        await datamanagers.vectorsets.initialize(txn, kbid=uuid)
+
         config.migration_version = get_latest_version()
         config.slug = slug
         await txn.set(
             datamanagers.kb.KB_UUID.format(kbid=uuid),
             config.SerializeToString(),
         )
         # Create Storage
```

## Comparing `nucliadb-4.0.1.post553.dist-info/METADATA` & `nucliadb-4.0.1.post554.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.1.post553
+Version: 4.0.1.post554
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post553
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post553
-Requires-Dist: nucliadb-protos >=4.0.1.post553
-Requires-Dist: nucliadb-models >=4.0.1.post553
+Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post554
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post554
+Requires-Dist: nucliadb-protos >=4.0.1.post554
+Requires-Dist: nucliadb-models >=4.0.1.post554
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.1.post553.dist-info/entry_points.txt` & `nucliadb-4.0.1.post554.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.1.post553.dist-info/RECORD` & `nucliadb-4.0.1.post554.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 migrations/0011_materialize_labelset_ids.py,sha256=nu9mzkwwVD3mw-_jE6YJZAV8r2gXfigL-wUzIaR8iiw,1843
 migrations/0012_rollover_shards.py,sha256=3ShFPB11vFEYvso5vc8NZwYhXwuA0R4inA16k15GAkI,1443
 migrations/0013_rollover_shards.py,sha256=c3IU8zinlWeVRN8T6o5eLpvGzkQOHX_Yz5xuFVRUy5U,1024
 migrations/0014_rollover_shards.py,sha256=24yLtXAwlVvCwtHLx9Tz-VWCzeMuy-0o3M6QNESi_Iw,1382
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
-migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
+migrations/0018_purge_orphan_kbslugs.py,sha256=rlNPRkp04GGf88RrKV5ZavoDwrSnxtNlyT-P3_jB1gA,2264
 migrations/0019_upgrade_to_paragraphs_v3.py,sha256=Jf1ljYQoLj1QExz9-tDIxI7QrwPhixIHxvQJvHOl6WA,2506
 migrations/0020_drain_nodes_from_cluster.py,sha256=86HCbrIF9Q4-TC-Js8d5LDJFc2_18AcntwfCtqlXwho,3282
+migrations/0021_overwrite_vectorsets_key.py,sha256=omQbVYdssyWJ_asHmwtkezqsnmEde8oXQR9LIZY-6kg,1734
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=LC_4iKUrJvvnfQbOT_YG-IFuBviJgOWMvT7klzJ89UE,11793
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=bYfDSrWDyziKVxcmfM1HmB9pwDpOx6fPkyUviHgCK9Q,5175
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=13ACuaNosUVsAkF1TqNv2xOMh_CJ9jpNv_bySiH1-ZI,5134
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=rqco9bKGw77ssbKCakURWm5oGD4J0huEO5c30tvcA7Q,3793
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=5EQxi-q33n_NtQKPVSTLD5x36Y8lkwhjKbAsl1KM4Rg,22378
+nucliadb/common/cluster/manager.py,sha256=4I8CRFhP9Ly64dH4xJeV7yxj5Ykp2pj0eIOltGhzpFw,23442
 nucliadb/common/cluster/rebalance.py,sha256=9jYILsIC93N3s62XltL2HLacQbLiXTNdMlG50v1ONR4,8853
 nucliadb/common/cluster/rollover.py,sha256=bXnnZjWiq2GxPPcQuyMhFBiDrPGhWTyPFsyMejYnVVw,20532
 nucliadb/common/cluster/settings.py,sha256=-H30-AVnSe3iUUyFUga78xcMPScq7ZR6aNgRuVgQdu8,3016
 nucliadb/common/cluster/utils.py,sha256=15dQBg4XKmdD5iOZsOwU7YGx01h84HRZIWv48EtaUOE,5713
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=7ag_lluBoXqA-6C5M9PS3RmNmBG0QT2aZGyLAd6ltwI,12512
@@ -58,15 +59,15 @@
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
 nucliadb/common/datamanagers/resources.py,sha256=7YI2-KN22fXbj9FqKGZQGN-bUH26hCt9CBrJUtAclsI,12177
 nucliadb/common/datamanagers/rollover.py,sha256=oxrvnCWM69MG7liMekwQx8TXuNzwixEKJT_--f5Uf-0,5634
 nucliadb/common/datamanagers/synonyms.py,sha256=f7m3N7SXoYSDWvrNDcAeWoWVAHKI8ByZhnBrZ8rVdec,1548
 nucliadb/common/datamanagers/utils.py,sha256=Ll17Pbn1AunTUcGjrk7F2d1SJ0RBOejdmAAlE1BaNmM,1631
-nucliadb/common/datamanagers/vectorsets.py,sha256=RDKjxbMzD-hkxc64-3x_dli1mV8pt-mcgsmdpw9OUw4,3305
+nucliadb/common/datamanagers/vectorsets.py,sha256=uEn7FPTkn2UCNZRAmZaqdwoUHjkLW3xQMIjPK9dodqc,3780
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
 nucliadb/common/maindb/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -114,15 +115,15 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=kwV3KxSn6bZNYBBHljMEN9qNXPlNv80guoKqQib8ivc,4212
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=qayvpXdkR_Hq7tw7UmDK8-BH-vFNuRdmkW2EWyk1lLs,28311
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=MquwOlw5hI_yzZtVsZ3mZc86loOouj-w5a6_f1naTKQ,15621
+nucliadb/ingest/orm/knowledgebox.py,sha256=L-oRMutI8_9KezL1t7t7qvdsf44YpnKHtTiGXuhDUgE,15687
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=vIpyFpftCgj4sBi5FfRlTLOxJnBuG57uyYH4DK0p6U4,58955
 nucliadb/ingest/orm/utils.py,sha256=A3_EsRw7Nub54qZPF08cv391caxpLQWJURR0_5qP9mU,2685
 nucliadb/ingest/orm/processor/__init__.py,sha256=sVQkEd-TGjTUMHGXJS3IIEtydLD-jSOoAYQK05pO_rA,27042
 nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
@@ -320,14 +321,15 @@
 nucliadb/tests/benchmarks/test_search.py,sha256=1Icz4bXwLJtzZGnc8xY4bXmVmgWJGXmv0Zq0NlZHIuk,3032
 nucliadb/tests/knowledgeboxes/__init__.py,sha256=u4paaCDL4YOUPUW5iZOzP72yMkdqTA_dMr6hRQEnf5k,919
 nucliadb/tests/knowledgeboxes/philosophy_books.py,sha256=CFPR5ARHpaWJm8KA5gPmSmrUyZBHCaFfuhkQFpmZKbM,7002
 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py,sha256=8yvWnAcYrlHTvfEntN9309LHFqchLd1BTIGKimFQab0,3037
 nucliadb/tests/migrations/__init__.py,sha256=1alcOjjpC6F2MmwnUGz3O4DQ0AbuMKtkkDsVbRyQec8,1148
 nucliadb/tests/migrations/test_migration_0017.py,sha256=U0Fy7bjwn61hfUZ-K9SYty6_dwS55V3E1r18UjFuNdM,2726
 nucliadb/tests/migrations/test_migration_0018.py,sha256=YmvAhog2CHQLK3BM3AH0m6rdJ83jNUdWCyRl4ilv5Ik,3662
+nucliadb/tests/migrations/test_migration_0021.py,sha256=G31SLYqLwwHNsgQFtXEZombcDyQ13ARXKYpndzZ5GJQ,3439
 nucliadb/tests/unit/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/test_field_ids.py,sha256=pwtHELSrfGtmKI3n4HBtsiRZFHlps6z2Nlb4kc7p5p4,1487
 nucliadb/tests/unit/test_health.py,sha256=G0c1Mpi5y_z94D3OSP-s2hEIfW1p0kkoY0tSmEg_8Bc,2780
 nucliadb/tests/unit/test_kb_slugs.py,sha256=XlifR2gz0e1WmqjMiCah0D7YXoceF1Sn8WGXqxGEeD8,1543
 nucliadb/tests/unit/test_learning_proxy.py,sha256=e3-wL_gsv0nQoChfvHR6NfDqSBzesnoq5MeGaHjzyNM,7892
 nucliadb/tests/unit/test_metrics_exporter.py,sha256=t__hVxV0Fo0duKtnJQl7BjyOXtP7QcD0pzHD9936z4o,2642
 nucliadb/tests/unit/test_openapi.py,sha256=ivwIs7UcTDfGyWD85VtzcmurPyU-ez9hvEmSCfFexrs,1341
@@ -457,13 +459,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.1.post553.dist-info/METADATA,sha256=CMfpY0ll0cbps3gqAUOj6A3kKR1yYJVjw3lxZiel5wQ,4474
-nucliadb-4.0.1.post553.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.1.post553.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.1.post553.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.1.post553.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.1.post553.dist-info/RECORD,,
+nucliadb-4.0.1.post554.dist-info/METADATA,sha256=519G0NOCwAD_ip4Q9mMfIyM2Cx5junocHLfp1plVu20,4474
+nucliadb-4.0.1.post554.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.1.post554.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.1.post554.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.1.post554.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.1.post554.dist-info/RECORD,,
```

