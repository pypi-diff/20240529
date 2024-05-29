# Comparing `tmp/nucliadb-4.0.1.post551-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.1.post552-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,471 +1,471 @@
-Zip file size: 767764 bytes, number of entries: 469
--rw-r--r--  2.0 unx     1135 b- defN 24-May-28 10:00 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-28 10:00 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-28 10:00 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-28 10:00 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-28 10:00 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-28 10:00 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-28 10:00 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-28 10:00 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-28 10:00 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-28 10:00 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-28 10:00 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-28 10:00 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-28 10:00 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-28 10:00 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-28 10:00 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-28 10:00 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-28 10:00 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-28 10:00 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-28 10:00 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-28 10:00 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-28 10:00 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-28 10:00 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-28 10:00 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-28 10:00 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-28 10:00 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-May-28 10:00 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-28 10:00 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-28 10:00 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-28 10:00 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-28 10:00 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-28 10:00 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-28 10:00 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-28 10:00 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-28 10:00 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-28 10:00 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-28 10:00 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-28 10:00 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-28 10:00 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-28 10:00 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-28 10:00 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-28 10:00 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1940 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     2651 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    12177 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     3305 b- defN 24-May-28 10:00 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-28 10:00 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-28 10:00 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-28 10:00 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-28 10:00 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-28 10:00 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-28 10:00 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-28 10:00 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-28 10:00 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-28 10:00 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-28 10:00 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-28 10:00 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-28 10:00 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-28 10:00 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-28 10:00 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-28 10:00 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-28 10:00 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-28 10:00 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-28 10:00 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-28 10:00 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-28 10:00 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-28 10:00 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-28 10:00 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-28 10:00 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-28 10:00 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-28 10:00 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/ingest/py.typed
--rw-r--r--  2.0 unx    20277 b- defN 24-May-28 10:00 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-28 10:00 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-28 10:00 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-28 10:00 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-28 10:00 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-28 10:00 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-28 10:00 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-28 10:00 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-28 10:00 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-28 10:00 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-28 10:00 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-28 10:00 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-28 10:00 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-28 10:00 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-28 10:00 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-28 10:00 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-28 10:00 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    15621 b- defN 24-May-28 10:00 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-28 10:00 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    58955 b- defN 24-May-28 10:00 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-28 10:00 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-28 10:00 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-28 10:00 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-28 10:00 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-28 10:00 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    30462 b- defN 24-May-28 10:00 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-28 10:00 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-28 10:00 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-28 10:00 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-28 10:00 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-28 10:00 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-28 10:00 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-28 10:00 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-28 10:00 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-28 10:00 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-28 10:00 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-28 10:00 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-28 10:00 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-28 10:00 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-28 10:00 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-28 10:00 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-28 10:00 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-28 10:00 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-28 10:00 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-28 10:00 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-28 10:00 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-28 10:00 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-28 10:00 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/reader/py.typed
--rw-r--r--  2.0 unx     1447 b- defN 24-May-28 10:00 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-28 10:00 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-28 10:00 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-28 10:00 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-28 10:00 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-28 10:00 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-28 10:00 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-28 10:00 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-28 10:00 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-28 10:00 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-28 10:00 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-28 10:00 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-28 10:00 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-28 10:00 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-28 10:00 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-28 10:00 nucliadb/search/predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/search/py.typed
--rw-r--r--  2.0 unx     1402 b- defN 24-May-28 10:00 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-28 10:00 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-28 10:00 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-28 10:00 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-28 10:00 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-28 10:00 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-28 10:00 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-28 10:00 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-28 10:00 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-28 10:00 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-28 10:00 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-28 10:00 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-28 10:00 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-28 10:00 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-28 10:00 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-28 10:00 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-28 10:00 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-28 10:00 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-28 10:00 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-28 10:00 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-28 10:00 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-28 10:00 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-28 10:00 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-28 10:00 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-28 10:00 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-28 10:00 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-28 10:00 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-28 10:00 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-28 10:00 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-28 10:00 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-28 10:00 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-28 10:00 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-28 10:00 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-28 10:00 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-28 10:00 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-28 10:00 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-28 10:00 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-28 10:00 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-28 10:00 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-28 10:00 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-28 10:00 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-28 10:00 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-28 10:00 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-28 10:00 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-28 10:00 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-28 10:00 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-28 10:00 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-28 10:00 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-28 10:00 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/standalone/py.typed
--rw-r--r--  2.0 unx     5636 b- defN 24-May-28 10:00 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-28 10:00 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-28 10:00 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-28 10:00 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-28 10:00 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-28 10:00 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-28 10:00 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-28 10:00 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-28 10:00 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-28 10:00 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-28 10:00 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-28 10:00 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-28 10:00 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-28 10:00 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-28 10:00 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-28 10:00 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-28 10:00 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-28 10:00 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-28 10:00 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-28 10:00 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-28 10:00 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-28 10:00 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-28 10:00 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-28 10:00 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-28 10:00 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-28 10:00 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-28 10:00 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-28 10:00 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-28 10:00 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-28 10:00 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-28 10:00 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-28 10:00 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-28 10:00 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-28 10:00 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-28 10:00 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-28 10:00 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-28 10:00 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-28 10:00 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-28 10:00 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-28 10:00 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-28 10:00 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-28 10:00 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-28 10:00 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-28 10:00 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-28 10:00 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-28 10:00 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-28 10:00 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/train/py.typed
--rw-r--r--  2.0 unx     1400 b- defN 24-May-28 10:00 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-28 10:00 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-28 10:00 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-28 10:00 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-28 10:00 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-28 10:00 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-28 10:00 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-28 10:00 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-28 10:00 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-28 10:00 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-28 10:00 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-28 10:00 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-28 10:00 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-28 10:00 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-28 10:00 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-28 10:00 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-28 10:00 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-28 10:00 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-28 10:00 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-28 10:00 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-28 10:00 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-28 10:00 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-28 10:00 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-28 10:00 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-28 10:00 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-28 10:00 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-28 10:00 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2201 b- defN 24-May-28 10:00 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-28 10:00 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-28 10:00 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-28 10:00 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-28 10:00 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-28 10:00 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-28 10:00 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-28 10:00 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-28 10:00 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-28 10:00 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-28 10:00 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-28 10:00 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-28 10:00 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-28 10:00 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-28 10:00 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-28 10:00 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-28 10:00 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-28 10:00 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-28 10:00 nucliadb/writer/py.typed
--rw-r--r--  2.0 unx     1448 b- defN 24-May-28 10:00 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-28 10:00 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-28 10:00 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-28 10:00 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-May-28 10:00 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-28 10:00 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-28 10:00 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-28 10:00 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-28 10:00 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-28 10:00 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-28 10:00 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-28 10:00 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-28 10:00 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-28 10:00 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-28 10:00 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-28 10:00 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-28 10:00 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-28 10:00 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-28 10:00 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-28 10:00 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-28 10:00 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-28 10:00 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-28 10:00 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-28 10:00 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-28 10:00 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4474 b- defN 24-May-28 10:02 nucliadb-4.0.1.post551.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 10:02 nucliadb-4.0.1.post551.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-28 10:02 nucliadb-4.0.1.post551.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-28 10:02 nucliadb-4.0.1.post551.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-28 10:01 nucliadb-4.0.1.post551.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43936 b- defN 24-May-28 10:02 nucliadb-4.0.1.post551.dist-info/RECORD
-469 files, 2264876 bytes uncompressed, 697496 bytes compressed:  69.2%
+Zip file size: 768049 bytes, number of entries: 469
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-28 14:23 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 14:23 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-28 14:23 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 14:23 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 14:23 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-28 14:23 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-28 14:23 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-28 14:23 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-28 14:23 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-28 14:23 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-28 14:23 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-28 14:23 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-28 14:23 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-28 14:23 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-28 14:23 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-28 14:23 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-28 14:23 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-28 14:23 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-28 14:23 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-28 14:23 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-28 14:23 nucliadb/health.py
+-rw-r--r--  2.0 unx    11793 b- defN 24-May-28 14:23 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-28 14:23 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-28 14:23 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-28 14:23 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5134 b- defN 24-May-28 14:23 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-28 14:23 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-28 14:23 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-28 14:23 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22378 b- defN 24-May-28 14:23 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-28 14:23 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-May-28 14:23 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-28 14:23 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-28 14:23 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-28 14:23 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-28 14:23 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-28 14:23 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-28 14:23 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-28 14:23 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-28 14:23 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-28 14:23 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1940 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     3305 b- defN 24-May-28 14:23 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-28 14:23 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-28 14:23 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-28 14:23 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-28 14:23 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-28 14:23 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-28 14:23 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-28 14:23 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-28 14:23 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-28 14:23 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-28 14:23 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-28 14:23 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-28 14:23 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-28 14:23 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-28 14:23 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-28 14:23 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-28 14:23 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-28 14:23 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-28 14:23 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-28 14:23 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-28 14:23 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-28 14:23 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-28 14:23 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-28 14:23 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-28 14:23 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-28 14:23 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-28 14:23 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-28 14:23 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-28 14:23 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-28 14:23 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-28 14:23 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-28 14:23 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-28 14:23 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-28 14:23 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-28 14:23 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-28 14:23 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-28 14:23 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-28 14:23 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-28 14:23 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-28 14:23 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-28 14:23 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-28 14:23 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-28 14:23 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    15621 b- defN 24-May-28 14:23 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-28 14:23 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-28 14:23 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-28 14:23 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-28 14:23 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-28 14:23 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-28 14:23 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-28 14:23 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-28 14:23 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-28 14:23 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24111 b- defN 24-May-28 14:23 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-28 14:23 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-28 14:23 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-28 14:23 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-28 14:23 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-28 14:23 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-28 14:23 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-28 14:23 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-28 14:23 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-28 14:23 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-28 14:23 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-28 14:23 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-28 14:23 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-28 14:23 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-28 14:23 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-28 14:23 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-28 14:23 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 14:23 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-28 14:23 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-28 14:23 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-28 14:23 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-28 14:23 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-28 14:23 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-28 14:23 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-28 14:23 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-28 14:23 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-28 14:23 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-28 14:23 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-28 14:23 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-28 14:23 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-28 14:23 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-28 14:23 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-28 14:23 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-28 14:23 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-28 14:23 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-28 14:23 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-28 14:23 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-28 14:23 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-28 14:23 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-28 14:23 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-28 14:23 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-28 14:23 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-28 14:23 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-28 14:23 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-28 14:23 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-28 14:23 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-28 14:23 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-28 14:23 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-28 14:23 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-28 14:23 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-28 14:23 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-28 14:23 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-28 14:23 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-28 14:23 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-28 14:23 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-28 14:23 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-28 14:23 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-28 14:23 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-28 14:23 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-28 14:23 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-28 14:23 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-28 14:23 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-28 14:23 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-28 14:23 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-28 14:23 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-28 14:23 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-28 14:23 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-28 14:23 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-28 14:23 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-28 14:23 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-28 14:23 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-28 14:23 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-28 14:23 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-28 14:23 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-28 14:23 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-28 14:23 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-28 14:23 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-28 14:23 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-28 14:23 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-28 14:23 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-28 14:23 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-28 14:23 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-28 14:23 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-28 14:23 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-28 14:23 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-28 14:23 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-28 14:23 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-28 14:23 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-28 14:23 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-28 14:23 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-28 14:23 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-28 14:23 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-28 14:23 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-28 14:23 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-28 14:23 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-28 14:23 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-28 14:23 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-28 14:23 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-28 14:23 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-28 14:23 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-28 14:23 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-28 14:23 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-28 14:23 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-28 14:23 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-28 14:23 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-28 14:23 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-28 14:23 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-28 14:23 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-28 14:23 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-28 14:23 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-28 14:23 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-28 14:23 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-28 14:23 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-28 14:23 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-28 14:23 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-28 14:23 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-28 14:23 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-28 14:23 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-28 14:23 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-28 14:23 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-28 14:23 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-28 14:23 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-28 14:23 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-28 14:23 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-28 14:23 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-28 14:23 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-28 14:23 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-28 14:23 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-28 14:23 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-28 14:23 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-28 14:23 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-28 14:23 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-28 14:23 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-28 14:23 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-28 14:23 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-28 14:23 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-28 14:23 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-28 14:23 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-28 14:23 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-28 14:23 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-28 14:23 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-28 14:23 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-28 14:23 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-28 14:23 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-28 14:23 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-28 14:23 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-28 14:23 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-28 14:23 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-28 14:23 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-28 14:23 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-28 14:23 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-28 14:23 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-28 14:23 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-28 14:23 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-28 14:23 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-28 14:23 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-28 14:23 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-28 14:23 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-28 14:23 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-28 14:23 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-May-28 14:23 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-28 14:23 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-28 14:23 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-28 14:23 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-28 14:23 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-28 14:23 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-28 14:23 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-28 14:23 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-28 14:23 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-28 14:23 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-28 14:23 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-28 14:23 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 14:23 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-28 14:23 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-28 14:23 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-28 14:23 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-28 14:23 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-28 14:23 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 14:23 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-28 14:23 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-28 14:23 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-28 14:23 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-28 14:23 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-May-28 14:23 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-28 14:23 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-28 14:23 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-28 14:23 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-28 14:23 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-28 14:23 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-28 14:23 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 14:23 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-28 14:23 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-28 14:23 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-28 14:23 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-28 14:23 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-28 14:23 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-28 14:23 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-28 14:23 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-28 14:23 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-28 14:23 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-28 14:23 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-28 14:23 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-28 14:23 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-28 14:23 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43936 b- defN 24-May-28 14:24 nucliadb-4.0.1.post552.dist-info/RECORD
+469 files, 2265745 bytes uncompressed, 697781 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1383,26 +1383,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/METADATA
+Filename: nucliadb-4.0.1.post552.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/WHEEL
+Filename: nucliadb-4.0.1.post552.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/entry_points.txt
+Filename: nucliadb-4.0.1.post552.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/top_level.txt
+Filename: nucliadb-4.0.1.post552.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/zip-safe
+Filename: nucliadb-4.0.1.post552.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.1.post551.dist-info/RECORD
+Filename: nucliadb-4.0.1.post552.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/learning_proxy.py

```diff
@@ -16,14 +16,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import contextlib
 import json
 import logging
+import os
 from collections.abc import AsyncIterator
 from enum import Enum
 from typing import Any, Optional, Union
 
 import backoff
 import httpx
 from fastapi import Request, Response
@@ -323,15 +324,19 @@
     async def delete(self, *args: Any, **kwargs: Any):
         return self._handle_request("DELETE", *args, **kwargs)
 
     def get_config(self, *args: Any, **kwargs: Any):
         lconfig = LearningConfiguration(
             semantic_model="multilingual",
             semantic_vector_similarity="cosine",
-            semantic_vector_size=None,
+            semantic_vector_size=(
+                768
+                if os.environ.get("TEST_SENTENCE_ENCODER") == "multilingual-2023-02-21"
+                else 512
+            ),
             semantic_threshold=None,
             semantic_matryoshka_dims=[],
         )
         return self._response(content=lconfig.dict())
 
     async def request(  # type: ignore
         self,
```

## nucliadb/common/cluster/base.py

```diff
@@ -21,14 +21,15 @@
 from typing import AsyncIterator, Optional
 
 from nucliadb_protos.nodereader_pb2_grpc import NodeReaderStub
 from nucliadb_protos.nodewriter_pb2 import (
     NewShardRequest,
     NewVectorSetRequest,
     OpStatus,
+    VectorIndexConfig,
 )
 from nucliadb_protos.nodewriter_pb2_grpc import NodeWriterStub
 
 from nucliadb_protos import nodereader_pb2, noderesources_pb2, utils_pb2
 
 
 class AbstractIndexNode(metaclass=ABCMeta):
@@ -89,23 +90,24 @@
         req = nodereader_pb2.GetShardRequest()
         req.shard_id.id = shard_id
         return await self.reader.GetShard(req)  # type: ignore
 
     async def new_shard(
         self,
         kbid: str,
-        similarity: utils_pb2.VectorSimilarity.ValueType,
         release_channel: utils_pb2.ReleaseChannel.ValueType,
-        normalize_vectors: bool,
+        vector_index_config: VectorIndexConfig,
     ) -> noderesources_pb2.ShardCreated:
         req = NewShardRequest(
             kbid=kbid,
-            similarity=similarity,
             release_channel=release_channel,
-            normalize_vectors=normalize_vectors,
+            config=vector_index_config,
+            # Deprecated fields, only for backwards compatibility with older nodes
+            similarity=vector_index_config.similarity,
+            normalize_vectors=vector_index_config.normalize_vectors,
         )
 
         resp = await self.writer.NewShard(req)  # type: ignore
         return resp
 
     async def list_shards(self) -> list[str]:
         shards = await self.writer.ListShards(noderesources_pb2.EmptyQuery())  # type: ignore
@@ -116,23 +118,23 @@
         resp: noderesources_pb2.ShardId = await self.writer.DeleteShard(req)  # type: ignore
         return resp.id
 
     async def add_vectorset(
         self,
         shard_id: str,
         vectorset: str,
-        *,
-        similarity: utils_pb2.VectorSimilarity.ValueType = utils_pb2.VectorSimilarity.COSINE,
-        normalize_vectors: bool = False,
+        config: VectorIndexConfig,
     ) -> OpStatus:
-        req = NewVectorSetRequest()
-        req.id.shard.id = shard_id
-        req.id.vectorset = vectorset
-        req.similarity = similarity
-        req.normalize_vectors = normalize_vectors
+        req = NewVectorSetRequest(
+            id=noderesources_pb2.VectorSetID(
+                shard=noderesources_pb2.ShardId(id=shard_id), vectorset=vectorset
+            ),
+            config=config,
+        )
+
         resp = await self.writer.AddVectorSet(req)  # type: ignore
         return resp
 
     async def list_vectorsets(self, shard_id: str) -> list[str]:
         req = noderesources_pb2.ShardId()
         req.id = shard_id
         resp = await self.writer.ListVectorSets(req)  # type: ignore
```

## nucliadb/common/cluster/manager.py

```diff
@@ -225,20 +225,25 @@
                     raise ExhaustedNodesError()
 
                 node = get_index_node(node_id)
                 if node is None:
                     logger.error(f"Node {node_id} is not found or not available")
                     continue
                 is_matryoshka = len(kb_shards.model.matryoshka_dimensions) > 0
+                vector_index_config = nodewriter_pb2.VectorIndexConfig(
+                    similarity=kb_shards.similarity,
+                    vector_type=nodewriter_pb2.VectorType.DENSE_F32,
+                    vector_dimension=kb_shards.model.vector_dimension,
+                    normalize_vectors=is_matryoshka,
+                )
                 try:
                     shard_created = await node.new_shard(
                         kbid,
-                        similarity=kb_shards.similarity,
                         release_channel=kb_shards.release_channel,
-                        normalize_vectors=is_matryoshka,
+                        vector_index_config=vector_index_config,
                     )
                 except Exception as e:
                     errors.capture_exception(e)
                     logger.exception(f"Error creating new shard at {node}: {e}")
                     continue
 
                 replica = writer_pb2.ShardReplica(node=str(node_id))
```

## nucliadb/common/cluster/rollover.py

```diff
@@ -23,15 +23,15 @@
 import logging
 from datetime import datetime
 from typing import Optional
 
 from nucliadb.common import datamanagers, locking
 from nucliadb.common.cluster import manager as cluster_manager
 from nucliadb.common.context import ApplicationContext
-from nucliadb_protos import writer_pb2
+from nucliadb_protos import nodewriter_pb2, writer_pb2
 from nucliadb_telemetry import errors
 
 from .manager import get_index_node
 from .settings import settings
 from .utils import delete_resource_from_shard, index_resource_to_shard, wait_for_node
 
 logger = logging.getLogger(__name__)
@@ -101,20 +101,25 @@
                     node_id = nodes.pop(0)
 
                     node = get_index_node(node_id)
                     if node is None:
                         logger.error(f"Node {node_id} is not found or not available")
                         continue
                     is_matryoshka = len(kb_shards.model.matryoshka_dimensions) > 0
+                    vector_index_config = nodewriter_pb2.VectorIndexConfig(
+                        similarity=kb_shards.similarity,
+                        vector_type=nodewriter_pb2.VectorType.DENSE_F32,
+                        vector_dimension=kb_shards.model.vector_dimension,
+                        normalize_vectors=is_matryoshka,
+                    )
                     try:
                         shard_created = await node.new_shard(
                             kbid,
-                            similarity=kb_shards.similarity,
                             release_channel=kb_shards.release_channel,
-                            normalize_vectors=is_matryoshka,
+                            vector_index_config=vector_index_config,
                         )
                     except Exception as e:
                         errors.capture_exception(e)
                         logger.exception(f"Error creating new shard at {node}")
                         continue
 
                     replica = writer_pb2.ShardReplica(node=str(node_id))
```

## nucliadb/ingest/tests/fixtures.py

```diff
@@ -179,15 +179,15 @@
 
 
 @pytest.fixture()
 def learning_config():
     lconfig = LearningConfiguration(
         semantic_model="multilingual",
         semantic_threshold=None,
-        semantic_vector_size=None,
+        semantic_vector_size=len(V1),
         semantic_vector_similarity="cosine",
     )
     with patch("nucliadb.ingest.service.writer.learning_proxy") as mocked:
         mocked.set_configuration = AsyncMock(return_value=None)
         mocked.get_configuration = AsyncMock(return_value=lconfig)
         mocked.delete_configuration = AsyncMock(return_value=None)
         yield mocked
@@ -196,15 +196,17 @@
 @pytest.fixture(scope="function")
 async def knowledgebox_ingest(
     storage, maindb_driver: Driver, shard_manager, learning_config
 ):
     kbid = str(uuid.uuid4())
     kbslug = str(uuid.uuid4())
     async with maindb_driver.transaction() as txn:
-        model = SemanticModelMetadata(similarity_function=upb.VectorSimilarity.COSINE)
+        model = SemanticModelMetadata(
+            similarity_function=upb.VectorSimilarity.COSINE, vector_dimension=len(V1)
+        )
         await KnowledgeBox.create(txn, kbslug, model, uuid=kbid)
         await txn.commit()
 
     yield kbid
 
     async with maindb_driver.transaction() as txn:
         await KnowledgeBox.delete_kb(txn, kbid)
```

## Comparing `nucliadb-4.0.1.post551.dist-info/METADATA` & `nucliadb-4.0.1.post552.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.1.post551
+Version: 4.0.1.post552
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
-Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post551
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post551
-Requires-Dist: nucliadb-protos >=4.0.1.post551
-Requires-Dist: nucliadb-models >=4.0.1.post551
+Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post552
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post552
+Requires-Dist: nucliadb-protos >=4.0.1.post552
+Requires-Dist: nucliadb-models >=4.0.1.post552
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.1.post551.dist-info/entry_points.txt` & `nucliadb-4.0.1.post552.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.1.post551.dist-info/RECORD` & `nucliadb-4.0.1.post552.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
 migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
 migrations/0019_upgrade_to_paragraphs_v3.py,sha256=Jf1ljYQoLj1QExz9-tDIxI7QrwPhixIHxvQJvHOl6WA,2506
 migrations/0020_drain_nodes_from_cluster.py,sha256=86HCbrIF9Q4-TC-Js8d5LDJFc2_18AcntwfCtqlXwho,3282
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
-nucliadb/learning_proxy.py,sha256=WuUpkMdvLBnv1uzUn-9_eLaKefpbM7I1QgX_4IHhwXE,11639
+nucliadb/learning_proxy.py,sha256=LC_4iKUrJvvnfQbOT_YG-IFuBviJgOWMvT7klzJ89UE,11793
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=bYfDSrWDyziKVxcmfM1HmB9pwDpOx6fPkyUviHgCK9Q,5175
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/common/cluster/base.py,sha256=j6F6w7KjNtuZS0aSDYFDeUc_D_Y1GY8flIpn0fYMKPU,5080
+nucliadb/common/cluster/base.py,sha256=13ACuaNosUVsAkF1TqNv2xOMh_CJ9jpNv_bySiH1-ZI,5134
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=rqco9bKGw77ssbKCakURWm5oGD4J0huEO5c30tvcA7Q,3793
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=FgUYnPaMv2Ts9lUvzpl87wk-Otp6Hd_2Q8H7tYtPv1E,22091
+nucliadb/common/cluster/manager.py,sha256=5EQxi-q33n_NtQKPVSTLD5x36Y8lkwhjKbAsl1KM4Rg,22378
 nucliadb/common/cluster/rebalance.py,sha256=9jYILsIC93N3s62XltL2HLacQbLiXTNdMlG50v1ONR4,8853
-nucliadb/common/cluster/rollover.py,sha256=okF5Y-b-s-thk6cbTI-86wrB32jZ-NE2JwwI2D-RtRM,20209
+nucliadb/common/cluster/rollover.py,sha256=bXnnZjWiq2GxPPcQuyMhFBiDrPGhWTyPFsyMejYnVVw,20532
 nucliadb/common/cluster/settings.py,sha256=-H30-AVnSe3iUUyFUga78xcMPScq7ZR6aNgRuVgQdu8,3016
 nucliadb/common/cluster/utils.py,sha256=15dQBg4XKmdD5iOZsOwU7YGx01h84HRZIWv48EtaUOE,5713
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=7ag_lluBoXqA-6C5M9PS3RmNmBG0QT2aZGyLAd6ltwI,12512
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
@@ -126,15 +126,15 @@
 nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/service/writer.py,sha256=OffZlErS9ndAEnTptFnbwOJqEXujvKd9Dbsgf5vSh3I,30462
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
-nucliadb/ingest/tests/fixtures.py,sha256=L4HeWexZwgpzPl872er2sAisfrW0OdmgOvx7SzCDrWM,24060
+nucliadb/ingest/tests/fixtures.py,sha256=FA62vAdJ_geh3V4wu3vnVaIE0PIct2f50Chdkr6wfgA,24111
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=kUUrdaR-iDFjmkip025rpYP5v6x3MIXLWd_n_c8-DXY,2500
 nucliadb/ingest/tests/integration/consumer/test_materializer.py,sha256=K7IQXCoJeZyqfrnT90-Uw2W4pPiGYmubUGMHhZyPhyc,3836
 nucliadb/ingest/tests/integration/consumer/test_pull.py,sha256=9teutVGwcirjXEFfIw0zKD8dbTR-Zwqr-ZH01OpnmwY,4470
 nucliadb/ingest/tests/integration/consumer/test_service.py,sha256=4xl19y1ad9TddI0cIJgFKGkfgz7Vht9nFZn1t22eUNc,2763
@@ -457,13 +457,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.1.post551.dist-info/METADATA,sha256=nPd6gEd0u-BGR1jM4M1KWzi3uEhI-GvW-mn8RO5c--4,4474
-nucliadb-4.0.1.post551.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.1.post551.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.1.post551.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.1.post551.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.1.post551.dist-info/RECORD,,
+nucliadb-4.0.1.post552.dist-info/METADATA,sha256=ww7uq0xzWd19lYOWdDka_dzBorZBEKJA8ryDcHXY9rg,4474
+nucliadb-4.0.1.post552.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.1.post552.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.1.post552.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.1.post552.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.1.post552.dist-info/RECORD,,
```

