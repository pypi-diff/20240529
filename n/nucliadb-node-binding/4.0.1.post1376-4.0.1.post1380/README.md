# Comparing `tmp/nucliadb_node_binding-4.0.1.post1376.tar.gz` & `tmp/nucliadb_node_binding-4.0.1.post1380.tar.gz`

## Comparing `nucliadb_node_binding-4.0.1.post1376.tar` & `nucliadb_node_binding-4.0.1.post1380.tar`

### file list

```diff
@@ -1,349 +1,352 @@
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    43269 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17239 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    19055 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1496 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    11343 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13965 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2300 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12999 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3394 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2489 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      332 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1455 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8294 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11334 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    19577 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1553 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13111 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14260 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11563 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    15700 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11202 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/indexes.rs
--rw-r--r--   0     1001      127    10055 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1168 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    28646 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    27248 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     7048 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/tests.rs
--rw-r--r--   0     1001      127     1890 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10199 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8386 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     9372 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     2508 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
--rw-r--r--   0     1001      127     6862 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5554 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0     1001      127     5337 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     7990 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9523 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2340 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127     8473 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/audit.rs
--rw-r--r--   0     1001      127    46350 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127    13228 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1271 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    95906 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    17860 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    62254 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    24308 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    50492 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127    10160 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127     2484 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/config.rs
--rw-r--r--   0     1001      127    12340 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24377 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    15068 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1741 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14194 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2513 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127     8419 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2607 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    23110 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     7189 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2264 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18009 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15340 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2933 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43324 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18147 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     3063 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     5462 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2944 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2023 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8450 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2557 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     5683 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10092 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3435 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2152 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3523 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/Cargo.toml
--rw-r--r--   0     1001      127     1017 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/.cargo/config.toml
--rw-r--r--   0     1001      127     1553 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/Makefile
--rw-r--r--   0     1001      127       52 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/README.md
--rwxr-xr-x   0     1001      127      978 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/cov.sh
--rw-r--r--   0     1001      127     1642 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/audit.proto
--rw-r--r--   0     1001      127     1938 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/dataset.proto
--rw-r--r--   0     1001      127     4424 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/knowledgebox.proto
--rw-r--r--   0     1001      127      129 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/migrations.proto
--rw-r--r--   0     1001      127    10792 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/nodereader.proto
--rw-r--r--   0     1001      127     4554 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/noderesources.proto
--rw-r--r--   0     1001      127     2907 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/nodewriter.proto
--rw-r--r--   0     1001      127       13 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/.gitignore
--rw-r--r--   0     1001      127      106 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/MANIFEST.in
--rw-r--r--   0     1001      127       93 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/README.rst
--rw-r--r--   0     1001      127        0 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/__init__.py
--rw-r--r--   0     1001      127     5729 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
--rw-r--r--   0     1001      127    11478 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
--rw-r--r--   0     1001      127     5708 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
--rw-r--r--   0     1001      127    14374 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
--rw-r--r--   0     1001      127    13093 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
--rw-r--r--   0     1001      127    30463 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
--rw-r--r--   0     1001      127     1152 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
--rw-r--r--   0     1001      127      844 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
--rw-r--r--   0     1001      127    22792 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
--rw-r--r--   0     1001      127    60294 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
--rw-r--r--   0     1001      127    27532 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
--rw-r--r--   0     1001      127    12923 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
--rw-r--r--   0     1001      127    14299 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
--rw-r--r--   0     1001      127    35337 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
--rw-r--r--   0     1001      127     7995 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
--rw-r--r--   0     1001      127    13432 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
--rw-r--r--   0     1001      127    20793 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
--rw-r--r--   0     1001      127     9143 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/py.typed
--rw-r--r--   0     1001      127     5175 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
--rw-r--r--   0     1001      127     9274 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
--rw-r--r--   0     1001      127     6379 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
--rw-r--r--   0     1001      127     3969 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
--rw-r--r--   0     1001      127    35561 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
--rw-r--r--   0     1001      127    95697 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
--rw-r--r--   0     1001      127     2192 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
--rw-r--r--   0     1001      127     2533 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
--rw-r--r--   0     1001      127     4407 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
--rw-r--r--   0     1001      127     2145 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
--rw-r--r--   0     1001      127    12447 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2.py
--rw-r--r--   0     1001      127    28142 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
--rw-r--r--   0     1001      127    13970 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
--rw-r--r--   0     1001      127    11812 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
--rw-r--r--   0     1001      127     6683 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
--rw-r--r--   0     1001      127    18303 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
--rw-r--r--   0     1001      127    32011 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
--rw-r--r--   0     1001      127    78244 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
--rw-r--r--   0     1001      127    39118 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
--rw-r--r--   0     1001      127    20858 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
--rw-r--r--   0     1001      127       96 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/setup.cfg
--rw-r--r--   0     1001      127      761 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/setup.py
--rw-r--r--   0     1001      127      708 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/reader.proto
--rw-r--r--   0     1001      127     1863 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/replication.proto
--rw-r--r--   0     1001      127    12098 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/resources.proto
--rw-r--r--   0     1001      127      558 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/standalone.proto
--rw-r--r--   0     1001      127     3469 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/train.proto
--rw-r--r--   0     1001      127     2301 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/utils.proto
--rw-r--r--   0     1001      127    12100 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/writer.proto
--rw-r--r--   0     1001      127     1461 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1621 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/update.rs
--rw-r--r--   0     1001      127    12085 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-05-27 20:22:13.000000 nucliadb_node_binding-4.0.1.post1376/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1376/PKG-INFO
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19055 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1496 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11343 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13965 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2300 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12999 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3394 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      332 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1455 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8294 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11334 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    19577 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1553 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13111 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14260 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11563 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    15700 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11202 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/indexes.rs
+-rw-r--r--   0     1001      127    10055 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1168 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    28646 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    27248 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     7048 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/tests.rs
+-rw-r--r--   0     1001      127     1890 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10199 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8386 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     9372 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2508 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5554 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0     1001      127     5337 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2340 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127     8473 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/audit.rs
+-rw-r--r--   0     1001      127    46350 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127    14122 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1271 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    95906 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    17860 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    62254 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    24308 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    50492 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127    10160 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    43269 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17239 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10092 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3435 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2152 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3523 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127     4424 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/config.rs
+-rw-r--r--   0     1001      127    12340 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    29379 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11821 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    15068 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1741 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    11691 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2513 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127     8487 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2607 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    23029 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    25379 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     7189 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     2157 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127    10472 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2282 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    18009 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15288 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     3267 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32.rs
+-rw-r--r--   0     1001      127     4415 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs
+-rw-r--r--   0     1001      127      903 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/vector_types/mod.rs
+-rw-r--r--   0     1001      127     3877 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/tests/test_basic_search.rs
+-rw-r--r--   0     1001      127     2895 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43324 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18147 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     3063 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2944 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2023 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8450 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2557 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     5688 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     7990 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9523 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/Cargo.toml
+-rw-r--r--   0     1001      127     1017 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/.cargo/config.toml
+-rw-r--r--   0     1001      127     1553 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/Makefile
+-rw-r--r--   0     1001      127       52 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/README.md
+-rwxr-xr-x   0     1001      127      978 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/cov.sh
+-rw-r--r--   0     1001      127     1642 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/audit.proto
+-rw-r--r--   0     1001      127     1938 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/dataset.proto
+-rw-r--r--   0     1001      127     4911 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/knowledgebox.proto
+-rw-r--r--   0     1001      127      129 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/migrations.proto
+-rw-r--r--   0     1001      127    10792 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/nodereader.proto
+-rw-r--r--   0     1001      127     4554 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/noderesources.proto
+-rw-r--r--   0     1001      127     2907 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/nodewriter.proto
+-rw-r--r--   0     1001      127       13 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/.gitignore
+-rw-r--r--   0     1001      127      106 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/MANIFEST.in
+-rw-r--r--   0     1001      127       93 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/README.rst
+-rw-r--r--   0     1001      127        0 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/__init__.py
+-rw-r--r--   0     1001      127     5729 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
+-rw-r--r--   0     1001      127    11478 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
+-rw-r--r--   0     1001      127     5708 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
+-rw-r--r--   0     1001      127    14374 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
+-rw-r--r--   0     1001      127    14324 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
+-rw-r--r--   0     1001      127    33126 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
+-rw-r--r--   0     1001      127     1152 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
+-rw-r--r--   0     1001      127      844 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
+-rw-r--r--   0     1001      127    22792 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
+-rw-r--r--   0     1001      127    60294 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
+-rw-r--r--   0     1001      127    27532 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
+-rw-r--r--   0     1001      127    12923 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    14299 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
+-rw-r--r--   0     1001      127    35337 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
+-rw-r--r--   0     1001      127     7995 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
+-rw-r--r--   0     1001      127    13432 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
+-rw-r--r--   0     1001      127    20793 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
+-rw-r--r--   0     1001      127     9143 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/py.typed
+-rw-r--r--   0     1001      127     5175 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
+-rw-r--r--   0     1001      127     9274 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
+-rw-r--r--   0     1001      127     6379 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
+-rw-r--r--   0     1001      127     3969 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    35561 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
+-rw-r--r--   0     1001      127    95697 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
+-rw-r--r--   0     1001      127     2192 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
+-rw-r--r--   0     1001      127     2533 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
+-rw-r--r--   0     1001      127     4407 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
+-rw-r--r--   0     1001      127     2145 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    13931 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2.py
+-rw-r--r--   0     1001      127    28248 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
+-rw-r--r--   0     1001      127    13970 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
+-rw-r--r--   0     1001      127    11918 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
+-rw-r--r--   0     1001      127     6683 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
+-rw-r--r--   0     1001      127    18303 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
+-rw-r--r--   0     1001      127    32771 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
+-rw-r--r--   0     1001      127    78350 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
+-rw-r--r--   0     1001      127    39118 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
+-rw-r--r--   0     1001      127    20964 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
+-rw-r--r--   0     1001      127       96 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/setup.cfg
+-rw-r--r--   0     1001      127      761 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/setup.py
+-rw-r--r--   0     1001      127      708 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/reader.proto
+-rw-r--r--   0     1001      127     1863 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/replication.proto
+-rw-r--r--   0     1001      127    12098 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/resources.proto
+-rw-r--r--   0     1001      127      558 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/standalone.proto
+-rw-r--r--   0     1001      127     3469 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/train.proto
+-rw-r--r--   0     1001      127     2301 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/utils.proto
+-rw-r--r--   0     1001      127    12100 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/writer.proto
+-rw-r--r--   0     1001      127     1461 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1621 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/update.rs
+-rw-r--r--   0     1001      127    12085 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-05-28 14:23:21.000000 nucliadb_node_binding-4.0.1.post1380/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1380/PKG-INFO
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/indexes.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/indexes.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/tests.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_node/tests/test_vectorsets.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_node/tests/test_vectorsets.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/audit.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/audit.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,36 @@
 pub struct VectorSets {
     #[prost(map = "string, message", tag = "1")]
     pub vectorsets: ::std::collections::HashMap<
         ::prost::alloc::string::String,
         VectorSet,
     >,
 }
+/// Configuration values for a vectorset
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct VectorSetConfig {
+    #[prost(string, tag = "1")]
+    pub vectorset_id: ::prost::alloc::string::String,
+    #[prost(message, optional, tag = "2")]
+    pub vectorset_index_config: ::core::option::Option<
+        super::nodewriter::VectorIndexConfig,
+    >,
+    /// list of possible subdivisions of the matryoshka embeddings (if the model
+    /// supports it)
+    #[prost(uint32, repeated, tag = "3")]
+    pub matryoshka_dimensions: ::prost::alloc::vec::Vec<u32>,
+}
+/// KB vectorsets and their configuration
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct KnowledgeBoxVectorSetsConfig {
+    #[prost(message, repeated, tag = "1")]
+    pub vectorsets: ::prost::alloc::vec::Vec<VectorSetConfig>,
+}
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct TermSynonyms {
     #[prost(string, repeated, tag = "1")]
     pub synonyms: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 [package]
-name = "nucliadb_vectors"
+name = "nucliadb_paragraphs2"
 version = "0.1.0"
 edition = "2021"
-license = "AGPL-3.0-or-later"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-serde = { version = "1.0", features = ["derive"] }
-uuid = { version = "1.1", features = ["serde", "v4"] }
 tempfile = "3"
-rand = "0.8.4"
-memmap2 = "0.5.3"
-fs2 = "0.4.3"
-thiserror = "1.0.31"
-serde_json = "1.0.82"
-crossbeam = "0.8.2"
-fst = "0.4.7"
-bincode = "1.3.3"
+lazy_static = "1.4.0"
+regex = "1.5.5"
+tantivy = { git = "https://github.com/nuclia/tantivy.git", branch = "original-17" }
+levenshtein_automata = "0.2.1"
+once_cell = "1.13.1"
+tantivy-fst = "0.3.0"
+tantivy-common = "0.2.0"
+itertools = "0.12"
+
+serde_json = "1.0.86"
 
 nucliadb_core = { path = "../nucliadb_core" }
 nucliadb_procs = { path = "../nucliadb_procs" }
-bit-set = "0.5.3"
-fxhash = "0.2.1"
-libc = "0.2.153"
-lazy_static = "1.4.0"
-
-[dev-dependencies]
-lazy_static = "1.4.0"
 
-[lib]
-name = "nucliadb_vectors"
-path = "src/lib.rs"
+[build-dependencies]
+serde_json = "1.0.86"
+itertools = "0.12"
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 pub mod ops_hnsw;
 pub mod ram_hnsw;
 
 mod params;
 #[cfg(test)]
 mod tests;
 
-use crate::config::Similarity;
-use crate::data_types::{data_store, trie, trie_ram, vector, DeleteLog};
+use crate::config::{VectorConfig, VectorType};
+use crate::data_types::{data_store, trie, trie_ram, DeleteLog};
 use crate::formula::Formula;
+use crate::vector_types::dense_f32_unaligned;
 use crate::VectorR;
 use data_store::Interpreter;
 use disk_hnsw::DiskHnsw;
 use fs::{File, OpenOptions};
 use fs2::FileExt;
 use io::{BufWriter, ErrorKind, Write};
 use memmap2::Mmap;
@@ -170,15 +171,15 @@
         index,
     })
 }
 
 pub fn merge<Dlog>(
     pin: &DataPointPin,
     operants: &[(Dlog, &OpenDataPoint)],
-    similarity: Similarity,
+    config: &VectorConfig,
     merge_time: SystemTime,
 ) -> VectorR<OpenDataPoint>
 where
     Dlog: DeleteLog,
 {
     let data_point_id = pin.data_point_id;
     let data_point_path = &pin.data_point_path;
@@ -206,15 +207,15 @@
 
     // Sort largest operant first so we reuse as much of the HNSW as possible
     let mut operants = operants.iter().collect::<Vec<_>>();
     operants.sort_unstable_by_key(|o| std::cmp::Reverse(o.1.journal().no_nodes()));
 
     // Creating the node store
     let node_producers: Vec<_> = operants.iter().map(|dp| ((&dp.0, Node), dp.1.nodes.as_ref())).collect();
-    let has_deletions = data_store::merge(&mut nodes_file, &node_producers)?;
+    let has_deletions = data_store::merge(&mut nodes_file, &node_producers, config)?;
     let nodes = unsafe { Mmap::map(&nodes_file)? };
     let no_nodes = data_store::stored_elements(&nodes);
 
     let mut index;
     let start_node_index;
     if has_deletions {
         index = RAMHnsw::new();
@@ -223,24 +224,15 @@
         // If there are no deletions, we can reuse the first segment
         // HNSW since its indexes will match the the ones in data_store
         index = DiskHnsw::deserialize(&operants[0].1.index);
         start_node_index = data_store::stored_elements(&operants[0].1.nodes);
     }
 
     // Creating the hnsw for the new node store.
-    let tracker = Retriever::new(
-        &[],
-        &nodes,
-        &NoDLog,
-        SearchParams {
-            similarity,
-            min_score: -1.0,
-            dimension: operants[0].1.stored_len().unwrap_or(0) as usize,
-        },
-    );
+    let tracker = Retriever::new(&[], &nodes, &NoDLog, config, -1.0);
     let mut ops = HnswOps::new(&tracker);
     for id in start_node_index..no_nodes {
         ops.insert(Address(id), &mut index)
     }
 
     {
         let mut hnswf_buffer = BufWriter::new(&mut hnsw_file);
@@ -276,16 +268,23 @@
     })
 }
 
 pub fn create(
     pin: &DataPointPin,
     elems: Vec<Elem>,
     time: Option<SystemTime>,
-    similarity: Similarity,
+    config: &VectorConfig,
 ) -> VectorR<OpenDataPoint> {
+    // Check dimensions
+    if let Some(dim) = config.vector_type.dimension() {
+        if elems.iter().any(|elem| elem.vector.len() != dim) {
+            return Err(crate::VectorErr::InconsistentDimensions);
+        }
+    }
+
     let data_point_id = pin.data_point_id;
     let data_point_path = &pin.data_point_path;
     let mut nodes_file_options = OpenOptions::new();
     nodes_file_options.read(true);
     nodes_file_options.write(true);
     nodes_file_options.create(true);
     let mut nodesf = nodes_file_options.open(data_point_path.join(file_names::NODES))?;
@@ -300,36 +299,24 @@
     hnsw_file_options.read(true);
     hnsw_file_options.write(true);
     hnsw_file_options.create(true);
     let mut hnswf = hnsw_file_options.open(data_point_path.join(file_names::HNSW))?;
 
     // Serializing nodes on disk
     // Nodes are stored on disk and mmaped.
-    let dimension = elems.first().map(|e| e.vector.len());
-    data_store::create_key_value(&mut nodesf, elems)?;
+    data_store::create_key_value(&mut nodesf, elems, &config.vector_type)?;
     let nodes = unsafe { Mmap::map(&nodesf)? };
     let no_nodes = data_store::stored_elements(&nodes);
 
     // Creating the HNSW using the mmaped nodes
     let mut index = RAMHnsw::new();
-    if let Some(dimension) = dimension {
-        let tracker = Retriever::new(
-            &[],
-            &nodes,
-            &NoDLog,
-            SearchParams {
-                similarity,
-                min_score: -1.0,
-                dimension,
-            },
-        );
-        let mut ops = HnswOps::new(&tracker);
-        for id in 0..no_nodes {
-            ops.insert(Address(id), &mut index)
-        }
+    let tracker = Retriever::new(&[], &nodes, &NoDLog, config, -1.0);
+    let mut ops = HnswOps::new(&tracker);
+    for id in 0..no_nodes {
+        ops.insert(Address(id), &mut index)
     }
 
     {
         // The HNSW is on RAM
         // Serializing the HNSW into disk
         let mut hnswf_buffer = BufWriter::new(&mut hnswf);
         DiskHnsw::serialize_into(&mut hnswf_buffer, no_nodes, index)?;
@@ -411,49 +398,48 @@
         }
     }
     pub fn run<DR: DataRetriever>(&self, address: Address, tracker: &DR) -> bool {
         self.filter.run(address, tracker)
     }
 }
 
-pub struct SearchParams {
-    pub similarity: Similarity,
-    pub min_score: f32,
-    pub dimension: usize,
-}
-
 pub struct Retriever<'a, Dlog> {
     similarity_function: fn(&[u8], &[u8]) -> f32,
     no_nodes: usize,
     temp: &'a [u8],
     nodes: &'a Mmap,
     delete_log: &'a Dlog,
     min_score: f32,
-    dimension: usize,
+    vector_len_bytes: Option<usize>,
 }
 impl<'a, Dlog: DeleteLog> Retriever<'a, Dlog> {
     pub fn new(
         temp: &'a [u8],
         nodes: &'a Mmap,
         delete_log: &'a Dlog,
-        search_params: SearchParams,
+        config: &VectorConfig,
+        min_score: f32,
     ) -> Retriever<'a, Dlog> {
         let no_nodes = data_store::stored_elements(nodes);
-        let similarity_function = match search_params.similarity {
-            Similarity::Cosine => vector::cosine_similarity,
-            Similarity::Dot => vector::dot_similarity,
+        let vector_len_bytes = if config.known_dimensions() {
+            config.vector_len_bytes()
+        } else if data_store::stored_elements(nodes) > 0 {
+            let node = data_store::get_value(Node, nodes, 0);
+            Some(dense_f32_unaligned::vector_len(Node::vector(node)) as usize)
+        } else {
+            None
         };
         Retriever {
             temp,
             nodes,
             delete_log,
-            similarity_function,
+            similarity_function: config.similarity_function(),
             no_nodes,
-            min_score: search_params.min_score,
-            dimension: search_params.dimension,
+            min_score,
+            vector_len_bytes,
         }
     }
     fn find_node(&self, Address(x): Address) -> &[u8] {
         if x == self.no_nodes {
             self.temp
         } else {
             data_store::get_value(Node, self.nodes, x)
@@ -468,15 +454,17 @@
         } else {
             let x = self.find_node(x);
             Node::key(x)
         }
     }
 
     fn will_need(&self, Address(x): Address) {
-        data_store::will_need(self.nodes, x, self.dimension);
+        if let Some(len) = self.vector_len_bytes {
+            data_store::will_need(self.nodes, x, len);
+        }
     }
 
     fn get_vector(&self, x @ Address(addr): Address) -> &[u8] {
         if addr == self.no_nodes {
             self.temp
         } else {
             let x = self.find_node(x);
@@ -536,32 +524,39 @@
         let ram_trie = trie_ram::create_trie(&labels);
         LabelDictionary(trie::serialize(ram_trie))
     }
 }
 #[derive(Clone, Debug)]
 pub struct Elem {
     pub key: Vec<u8>,
-    pub vector: Vec<u8>,
+    pub vector: Vec<f32>,
     pub metadata: Option<Vec<u8>>,
     pub labels: LabelDictionary,
 }
 impl Elem {
     pub fn new(key: String, vector: Vec<f32>, labels: LabelDictionary, metadata: Option<Vec<u8>>) -> Elem {
         Elem {
             labels,
             metadata,
             key: key.as_bytes().to_vec(),
-            vector: vector::encode_vector(&vector),
+            vector,
         }
     }
 }
 
 impl data_store::IntoBuffer for Elem {
-    fn serialize_into<W: io::Write>(self, w: W) -> io::Result<()> {
-        Node::serialize_into(w, self.key, self.vector, self.labels.0, self.metadata.as_ref())
+    fn serialize_into<W: io::Write>(self, w: W, vector_type: &VectorType) -> io::Result<()> {
+        Node::serialize_into(
+            w,
+            self.key,
+            vector_type.encode(&self.vector),
+            vector_type.vector_alignment(),
+            self.labels.0,
+            self.metadata.as_ref(),
+        )
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Neighbour {
     score: f32,
     node: Vec<u8>,
@@ -589,15 +584,15 @@
 }
 
 impl Neighbour {
     #[cfg(test)]
     pub fn dummy_neighbour(key: &[u8], score: f32) -> Neighbour {
         Neighbour {
             score,
-            node: Node::serialize(key, [1, 2, 3, 4], [], None as Option<&[u8]>),
+            node: Node::serialize(key, [1, 2, 3, 4], 1, [], None as Option<&[u8]>),
         }
     }
     fn new(Address(addr): Address, data: &[u8], score: f32) -> Neighbour {
         let node = data_store::get_value(Node, data, addr);
         let (exact, _) = Node.read_exact(node);
         Neighbour {
             score,
@@ -631,20 +626,20 @@
 impl AsRef<OpenDataPoint> for OpenDataPoint {
     fn as_ref(&self) -> &OpenDataPoint {
         self
     }
 }
 
 impl OpenDataPoint {
-    pub fn stored_len(&self) -> Option<u64> {
+    pub fn stored_len(&self) -> Option<usize> {
         if data_store::stored_elements(&self.nodes) == 0 {
             return None;
         }
         let node = data_store::get_value(Node, &self.nodes, 0);
-        Some(vector::vector_len(Node::vector(node)))
+        Some(dense_f32_unaligned::vector_len(Node::vector(node)) as usize)
     }
     pub fn get_id(&self) -> DpId {
         self.journal.uid
     }
     pub fn journal(&self) -> Journal {
         self.journal
     }
@@ -667,37 +662,46 @@
     pub fn search<Dlog: DeleteLog>(
         &self,
         delete_log: &Dlog,
         query: &[f32],
         filter: &Formula,
         with_duplicates: bool,
         results: usize,
-        search_params: SearchParams,
+        config: &VectorConfig,
+        min_score: f32,
     ) -> impl Iterator<Item = Neighbour> + '_ {
-        let encoded_query = vector::encode_vector(query);
-        let tracker = Retriever::new(&encoded_query, &self.nodes, delete_log, search_params);
+        let encoded_query = config.vector_type.encode(query);
+        let tracker = Retriever::new(&encoded_query, &self.nodes, delete_log, config, min_score);
         let filter = FormulaFilter::new(filter);
         let ops = HnswOps::new(&tracker);
         let neighbours = ops.search(Address(self.journal.nodes), self.index.as_ref(), results, filter, with_duplicates);
 
         neighbours.into_iter().map(|(address, dist)| (Neighbour::new(address, &self.nodes, dist))).take(results)
     }
 }
 
 #[cfg(test)]
 mod test {
-    use std::collections::BTreeMap;
+    use std::{collections::BTreeMap, time::SystemTime};
 
-    use nucliadb_core::NodeResult;
+    use nucliadb_core::{
+        protos::{Position, Representation, SentenceMetadata},
+        NodeResult,
+    };
     use rand::{rngs::SmallRng, Rng, SeedableRng};
     use tempfile::tempdir;
 
-    use crate::data_types::vector::{dot_similarity, encode_vector};
+    use crate::{
+        config::{Similarity, VectorConfig},
+        data_types::data_store,
+        vector_types::dense_f32_unaligned::{dot_similarity, encode_vector},
+    };
+    use nucliadb_core::protos::prost::Message;
 
-    use super::{create, DataPointPin, Elem, NoDLog, SearchParams, Similarity};
+    use super::{create, merge, node::Node, DataPointPin, Elem, LabelDictionary, NoDLog};
 
     const DIMENSION: usize = 128;
 
     fn random_vector(rng: &mut impl Rng) -> Vec<f32> {
         let v: Vec<f32> = (0..DIMENSION).map(|_| rng.gen_range(-1.0..1.0)).collect();
         normalize(v)
     }
@@ -719,18 +723,138 @@
         normalize(v)
     }
 
     fn random_key(rng: &mut impl Rng) -> String {
         format!("{:032x?}", rng.gen::<u128>())
     }
 
+    fn random_string(rng: &mut impl Rng) -> String {
+        String::from_utf8_lossy(&[rng.gen_range(40..110)].repeat(rng.gen_range(1..16))).to_string()
+    }
+
     fn similarity(x: &[f32], y: &[f32]) -> f32 {
         dot_similarity(&encode_vector(x), &encode_vector(y))
     }
 
+    fn random_elem(rng: &mut impl Rng) -> (Elem, Vec<String>) {
+        let labels: Vec<_> = (0..rng.gen_range(0..=2)).map(|_| random_string(rng)).collect();
+        let metadata = SentenceMetadata {
+            position: Some(Position {
+                index: 1,
+                start: 2,
+                end: 3,
+                page_number: 4,
+                in_page: true,
+                start_seconds: vec![],
+                end_seconds: vec![],
+            }),
+            page_with_visual: false,
+            representation: Some(Representation {
+                is_a_table: false,
+                file: random_string(rng),
+            }),
+        };
+        (
+            Elem::new(
+                random_key(rng),
+                random_vector(rng),
+                LabelDictionary::new(labels.clone()),
+                Some(metadata.encode_to_vec()),
+            ),
+            labels,
+        )
+    }
+
+    #[test]
+    fn test_save_recall_aligned_data() -> NodeResult<()> {
+        let config = VectorConfig {
+            similarity: Similarity::Dot,
+            vector_type: crate::config::VectorType::DenseF32 {
+                dimension: DIMENSION,
+            },
+            normalize_vectors: false,
+        };
+        let mut rng = SmallRng::seed_from_u64(1234567890);
+        let temp_dir = tempdir()?;
+
+        // Create a data point with random data of different length
+        let pin = DataPointPin::create_pin(temp_dir.path())?;
+        let elems = (0..100).map(|_| random_elem(&mut rng)).collect::<Vec<_>>();
+        let dp = create(&pin, elems.iter().cloned().map(|x| x.0).collect(), None, &config)?;
+        let nodes = dp.nodes;
+
+        for (i, (elem, mut labels)) in elems.into_iter().enumerate() {
+            let node = data_store::get_value(Node, &nodes, i);
+            assert_eq!(elem.key, Node::key(node));
+            assert_eq!(config.vector_type.encode(&elem.vector), Node::vector(node));
+
+            // Compare metadata as the decoded protobug. Tthe absolute stored value may have trailing padding
+            // from vectors, but the decoding step should ignore it
+            assert_eq!(
+                SentenceMetadata::decode(elem.metadata.as_ref().unwrap().as_slice()),
+                SentenceMetadata::decode(Node::metadata(node))
+            );
+
+            // Compare labels
+            labels.sort();
+            let mut node_labels = Node::labels(node);
+            node_labels.sort();
+            assert_eq!(labels, node_labels);
+        }
+
+        Ok(())
+    }
+
+    #[test]
+    fn test_save_recall_aligned_data_after_merge() -> NodeResult<()> {
+        let config = VectorConfig {
+            similarity: Similarity::Dot,
+            vector_type: crate::config::VectorType::DenseF32 {
+                dimension: DIMENSION,
+            },
+            normalize_vectors: false,
+        };
+        let mut rng = SmallRng::seed_from_u64(1234567890);
+        let temp_dir = tempdir()?;
+
+        // Create two data points with random data of different length
+        let pin1 = DataPointPin::create_pin(temp_dir.path())?;
+        let elems1 = (0..10).map(|_| random_elem(&mut rng)).collect::<Vec<_>>();
+        let dp1 = create(&pin1, elems1.iter().cloned().map(|x| x.0).collect(), None, &config)?;
+
+        let pin2 = DataPointPin::create_pin(temp_dir.path())?;
+        let elems2 = (0..10).map(|_| random_elem(&mut rng)).collect::<Vec<_>>();
+        let dp2 = create(&pin2, elems2.iter().cloned().map(|x| x.0).collect(), None, &config)?;
+
+        let pin_merged = DataPointPin::create_pin(temp_dir.path())?;
+        let merged_dp = merge(&pin_merged, &[(NoDLog, &dp1), (NoDLog, &dp2)], &config, SystemTime::now())?;
+        let nodes = merged_dp.nodes;
+
+        for (i, (elem, mut labels)) in elems1.into_iter().chain(elems2.into_iter()).enumerate() {
+            let node = data_store::get_value(Node, &nodes, i);
+            assert_eq!(elem.key, Node::key(node));
+            assert_eq!(config.vector_type.encode(&elem.vector), Node::vector(node));
+
+            // Compare metadata as the decoded protobug. Tthe absolute stored value may have trailing padding
+            // from vectors, but the decoding step should ignore it
+            assert_eq!(
+                SentenceMetadata::decode(elem.metadata.as_ref().unwrap().as_slice()),
+                SentenceMetadata::decode(Node::metadata(node))
+            );
+
+            // Compare labels
+            labels.sort();
+            let mut node_labels = Node::labels(node);
+            node_labels.sort();
+            assert_eq!(labels, node_labels);
+        }
+
+        Ok(())
+    }
+
     #[test]
     fn test_recall_clustered_data() -> NodeResult<()> {
         // This test is a simplified version of the synthetic_recall_benchmark, with smaller data for faster runs
         // It's run here as a sanity check to get a big warning in case we mess up recall too badly
         // You can play with the benchmark version in order to get more information, tweak parameters, etc.
         let mut rng = SmallRng::seed_from_u64(1234567890);
         let mut elems = BTreeMap::new();
@@ -746,48 +870,43 @@
             for _ in 0..80 {
                 elems.insert(random_key(&mut rng), random_nearby_vector(&mut rng, &center, 0.03));
             }
             // Next cluster is nearby
             center = random_nearby_vector(&mut rng, &center, 0.1);
         }
 
+        let config = VectorConfig {
+            similarity: Similarity::Dot,
+            vector_type: crate::config::VectorType::DenseF32 {
+                dimension: DIMENSION,
+            },
+            normalize_vectors: false,
+        };
+
         // Create a data point
         let temp_dir = tempdir()?;
         let pin = DataPointPin::create_pin(temp_dir.path())?;
         let dp = create(
             &pin,
             elems.iter().map(|(k, v)| Elem::new(k.clone(), v.clone(), Default::default(), None)).collect(),
             None,
-            Similarity::Dot,
+            &config,
         )?;
 
         // Search a few times
         let correct = (0..100)
             .map(|_| {
                 // Search near an existing datapoint (simulates that the query is related to the data)
                 let base_v = elems.values().nth(rng.gen_range(0..elems.len())).unwrap();
                 let query = random_nearby_vector(&mut rng, base_v, 0.05);
 
                 let mut similarities: Vec<_> = elems.iter().map(|(k, v)| (k, similarity(v, &query))).collect();
                 similarities.sort_unstable_by(|a, b| a.1.total_cmp(&b.1).reverse());
 
-                let results: Vec<_> = dp
-                    .search(
-                        &NoDLog,
-                        &query,
-                        &Default::default(),
-                        false,
-                        5,
-                        SearchParams {
-                            similarity: Similarity::Dot,
-                            min_score: 0.0,
-                            dimension: DIMENSION,
-                        },
-                    )
-                    .collect();
+                let results: Vec<_> = dp.search(&NoDLog, &query, &Default::default(), false, 5, &config, 0.0).collect();
 
                 let search: Vec<_> = results.iter().map(|r| String::from_utf8(r.id().to_vec()).unwrap()).collect();
                 let brute_force: Vec<_> = similarities.iter().take(5).map(|r| r.0.clone()).collect();
                 search == brute_force
             })
             .filter(|x| *x)
             .count();
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files 21% similar despite different names*

```diff
@@ -64,27 +64,34 @@
         let strie = trie.as_ref();
         let svector_len = svector.len() + USIZE_LEN;
         let skey_len = skey.len() + USIZE_LEN;
         let slabels_len = strie.len();
         let metadata_len = metadata.map(|m| m.as_ref().len()).unwrap_or_default();
         HEADER_LEN + svector_len + skey_len + slabels_len + metadata_len
     }
-    pub fn serialize<S, V, T, M>(key: S, vector: V, labels: T, metadata: Option<M>) -> Vec<u8>
+    pub fn serialize<S, V, T, M>(key: S, vector: V, alignment: usize, labels: T, metadata: Option<M>) -> Vec<u8>
     where
         S: AsRef<[u8]>,
         V: AsRef<[u8]>,
         T: AsRef<[u8]>,
         M: AsRef<[u8]>,
     {
         let mut buf = vec![];
-        Node::serialize_into(&mut buf, key, vector, labels, metadata).unwrap();
+        Node::serialize_into(&mut buf, key, vector, alignment, labels, metadata).unwrap();
         buf
     }
     // labels must be sorted.
-    pub fn serialize_into<W, S, V, T, M>(mut w: W, key: S, vector: V, trie: T, metadata: Option<M>) -> io::Result<()>
+    pub fn serialize_into<W, S, V, T, M>(
+        mut w: W,
+        key: S,
+        vector: V,
+        alignment: usize,
+        trie: T,
+        metadata: Option<M>,
+    ) -> io::Result<()>
     where
         W: io::Write,
         S: AsRef<[u8]>,
         V: AsRef<[u8]>,
         T: AsRef<[u8]>,
         M: AsRef<[u8]>,
     {
@@ -95,28 +102,36 @@
         // Reading lens
         let svector_len = svector.len() + USIZE_LEN;
         let skey_len = skey.len() + USIZE_LEN;
         let slabels_len = strie.len();
         let metadata_len = metadata.as_ref().map(|m| m.as_ref().len()).unwrap_or_default();
 
         // Pointer computations
-        let len = HEADER_LEN + svector_len + skey_len + slabels_len + metadata_len;
         let vector_start = HEADER_LEN + metadata_len;
-        let key_start = vector_start + svector_len;
+        let vector_pad = if vector_start % alignment > 0 {
+            alignment - (vector_start % alignment)
+        } else {
+            0
+        };
+        let key_start = vector_start + svector_len + vector_pad;
         let labels_start = key_start + skey_len;
 
+        let len = HEADER_LEN + vector_pad + svector_len + skey_len + slabels_len + metadata_len;
+
         // Write pointers
         w.write_all(&len.to_le_bytes())?;
         w.write_all(&vector_start.to_le_bytes())?;
         w.write_all(&key_start.to_le_bytes())?;
         w.write_all(&labels_start.to_le_bytes())?;
         // Metadata segment
         metadata.map_or(Ok(()), |m| w.write_all(m.as_ref()))?;
         // Values
-        w.write_all(&svector.len().to_le_bytes())?;
+        w.write_all(&(svector.len() as u32).to_le_bytes())?;
+        w.write_all(&(vector_pad as u32).to_le_bytes())?;
+        w.write_all(&[0].repeat(vector_pad))?;
         w.write_all(svector)?;
         w.write_all(&skey.len().to_le_bytes())?;
         w.write_all(skey)?;
         w.write_all(strie)?;
         w.flush()
     }
     // x must be serialized using Node, may have trailing bytes.
@@ -140,16 +155,17 @@
         let xkey_len = usize_from_slice_le(&x[xkey_ptr..(xkey_ptr + USIZE_LEN)]);
         let xkey_start = xkey_ptr + USIZE_LEN;
         &x[xkey_start..(xkey_start + xkey_len)]
     }
     // x must be serialized using Node, may have trailing bytes.
     pub fn vector(x: &[u8]) -> &[u8] {
         let xvec_ptr = usize_from_slice_le(&x[VECTOR_START.0..VECTOR_START.1]);
-        let xvec_len = usize_from_slice_le(&x[xvec_ptr..(xvec_ptr + USIZE_LEN)]);
-        let xvec_start = xvec_ptr + USIZE_LEN;
+        let xvec_len = u32_from_slice_le(&x[xvec_ptr..(xvec_ptr + U32_LEN)]) as usize;
+        let xvec_pad = u32_from_slice_le(&x[(xvec_ptr + U32_LEN)..(xvec_ptr + 2 * U32_LEN)]);
+        let xvec_start = xvec_ptr + 2 * U32_LEN + xvec_pad as usize;
         &x[xvec_start..(xvec_start + xvec_len)]
     }
     // x must be serialized using Node, may have trailing bytes.
     pub fn has_label(x: &[u8], label: &[u8]) -> bool {
         let xlabel_ptr = usize_from_slice_le(&x[LABEL_START.0..LABEL_START.1]);
         trie::has_word(&x[xlabel_ptr..], label)
     }
@@ -163,29 +179,29 @@
         (&x[0..len], &x[len..])
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use crate::data_types::{trie_ram, vector};
+    use crate::{data_types::trie_ram, vector_types::dense_f32_unaligned};
     lazy_static::lazy_static! {
         static ref NO_LABELS_TRIE: Vec<u8> = trie::serialize(trie_ram::create_trie(&NO_LABELS));
         static ref LABELS_TRIE: Vec<u8> = trie::serialize(trie_ram::create_trie(&LABELS));
     }
     const NO_LABELS: [&[u8]; 0] = [];
     const LABELS: [&[u8]; 3] = [b"L1", b"L2", b"L3"];
     const NO_METADATA: Option<&[u8]> = None;
 
     #[test]
     fn create_test() {
         let key = b"NODE1";
-        let vector = vector::encode_vector(&[12.; 1000]);
+        let vector = dense_f32_unaligned::encode_vector(&[12.; 1000]);
         let mut buf = Vec::new();
-        Node::serialize_into(&mut buf, key, &vector, NO_LABELS_TRIE.clone(), NO_METADATA).unwrap();
+        Node::serialize_into(&mut buf, key, &vector, 1, NO_LABELS_TRIE.clone(), NO_METADATA).unwrap();
         let len = usize_from_slice_le(&buf[LEN.0..LEN.1]);
         let vector_start = usize_from_slice_le(&buf[VECTOR_START.0..VECTOR_START.1]);
         let key_start = usize_from_slice_le(&buf[KEY_START.0..KEY_START.1]);
         let vector_len = usize_from_slice_le(&buf[vector_start..(vector_start + USIZE_LEN)]);
         let key_len = usize_from_slice_le(&buf[key_start..(key_start + USIZE_LEN)]);
         let svector = (vector_start + USIZE_LEN)..(vector_start + USIZE_LEN + vector_len);
         let skey = (key_start + USIZE_LEN)..(key_start + USIZE_LEN + key_len);
@@ -197,17 +213,17 @@
         assert_eq!(&buf[svector], &vector);
         assert_eq!(&buf[skey], key.as_slice());
         assert_eq!(Node::vector(&buf), &vector);
         assert_eq!(Node::key(&buf), key);
 
         let key = b"NODE2";
         let metadata = b"THIS ARE THE METADATA CONTENTS";
-        let vector = vector::encode_vector(&[13.; 1000]);
+        let vector = dense_f32_unaligned::encode_vector(&[13.; 1000]);
         let mut buf = Vec::new();
-        Node::serialize_into(&mut buf, key, &vector, LABELS_TRIE.clone(), Some(metadata)).unwrap();
+        Node::serialize_into(&mut buf, key, &vector, 1, LABELS_TRIE.clone(), Some(metadata)).unwrap();
         let len = usize_from_slice_le(&buf[LEN.0..LEN.1]);
         let vector_start = usize_from_slice_le(&buf[VECTOR_START.0..VECTOR_START.1]);
         let key_start = usize_from_slice_le(&buf[KEY_START.0..KEY_START.1]);
         let vector_len = usize_from_slice_le(&buf[vector_start..(vector_start + USIZE_LEN)]);
         let key_len = usize_from_slice_le(&buf[key_start..(key_start + USIZE_LEN)]);
         let svector = (vector_start + USIZE_LEN)..(vector_start + USIZE_LEN + vector_len);
         let skey = (key_start + USIZE_LEN)..(key_start + USIZE_LEN + key_len);
@@ -224,22 +240,22 @@
     }
 
     #[test]
     fn look_up_test() {
         let mut buf = Vec::new();
         let key1 = b"NODE1";
         let metadata1 = b"The node 1 has metadata";
-        let vector1 = vector::encode_vector(&[12.; 1000]);
+        let vector1 = dense_f32_unaligned::encode_vector(&[12.; 1000]);
         let node1 = buf.len();
-        Node::serialize_into(&mut buf, key1, &vector1, NO_LABELS_TRIE.clone(), Some(&metadata1)).unwrap();
+        Node::serialize_into(&mut buf, key1, &vector1, 1, NO_LABELS_TRIE.clone(), Some(&metadata1)).unwrap();
         let key2 = b"NODE2";
         let metadata2 = b"Tuns out node 2 also has metadata";
-        let vector2 = vector::encode_vector(&[15.; 1000]);
+        let vector2 = dense_f32_unaligned::encode_vector(&[15.; 1000]);
         let node2 = buf.len();
-        Node::serialize_into(&mut buf, key2, &vector2, NO_LABELS_TRIE.clone(), Some(&metadata2)).unwrap();
+        Node::serialize_into(&mut buf, key2, &vector2, 1, NO_LABELS_TRIE.clone(), Some(&metadata2)).unwrap();
         assert_eq!(Node::key(&buf[node1..]), key1);
         assert_eq!(Node::key(&buf[node2..]), key2);
         assert_eq!(Node::vector(&buf[node1..]), vector1);
         assert_eq!(Node::vector(&buf[node2..]), vector2);
         assert!(Node.keep_in_merge(&buf[node1..]));
         assert!(Node.keep_in_merge(&buf[node2..]));
         assert_eq!(Node::metadata(&buf[node1..]), metadata1);
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-use crate::data_point::{self, DataPointPin, OpenDataPoint, SearchParams};
+use crate::data_point::{self, DataPointPin, OpenDataPoint};
 pub use crate::data_point::{DpId, Neighbour};
 use crate::data_point_provider::state::read_state;
 use crate::data_point_provider::VectorConfig;
 use crate::data_point_provider::{IndexMetadata, SearchRequest, OPENING_FLAG, STATE};
 use crate::data_types::dtrie_ram::DTrie;
 use crate::data_types::DeleteLog;
 use crate::utils;
@@ -101,15 +101,15 @@
 
 pub struct Reader {
     config: VectorConfig,
     path: PathBuf,
     open_data_points: FxHashMap<DpId, OpenDataPoint>,
     delete_log: DTrie,
     number_of_embeddings: usize,
-    dimension: Option<u64>,
+    dimension: Option<usize>,
     state_last_modified: SystemTime,
 }
 
 fn last_modified(path: &Path) -> std::io::Result<SystemTime> {
     std::fs::metadata(path)?.modified()
 }
 
@@ -160,55 +160,58 @@
             dimension,
             path: path.to_path_buf(),
             state_last_modified,
         })
     }
 
     pub fn search(&self, request: &dyn SearchRequest) -> VectorR<Vec<Neighbour>> {
-        let Some(dimension) = self.dimension else {
-            return Ok(Vec::with_capacity(0));
-        };
-
         let normalized_query;
         let query = if self.config.normalize_vectors {
             normalized_query = utils::normalize_vector(request.get_query());
             &normalized_query
         } else {
             request.get_query()
         };
 
-        if dimension != query.len() as u64 {
+        // Validate vector dimensions
+        let valid_dims = match self.config.vector_type {
+            crate::config::VectorType::DenseF32Unaligned => {
+                let Some(dimension) = self.dimension else {
+                    return Ok(Vec::with_capacity(0));
+                };
+                dimension == query.len()
+            }
+            crate::config::VectorType::DenseF32 {
+                dimension,
+            } => dimension == query.len(),
+        };
+        if !valid_dims {
             return Err(VectorErr::InconsistentDimensions);
         }
 
-        let similarity = self.config.similarity;
         let filter = request.get_filter();
         let with_duplicates = request.with_duplicates();
         let no_results = request.no_results();
         let min_score = request.min_score();
         let mut ffsv = Fssc::new(request.no_results(), with_duplicates);
 
         for open_data_point in self.open_data_points.values() {
             let data_point_journal = open_data_point.journal();
             let delete_log = TimeSensitiveDLog {
                 time: data_point_journal.time(),
                 dlog: &self.delete_log,
             };
-            // Skipping the formatter only because the search interface is quite bad right now.
-            #[rustfmt::skip] let partial_solution = open_data_point.search(
+            let partial_solution = open_data_point.search(
                 &delete_log,
                 query,
                 filter,
                 with_duplicates,
                 no_results,
-                SearchParams {
-                    similarity,
-                    min_score,
-                    dimension: dimension as usize,
-                }
+                &self.config,
+                min_score,
             );
             for candidate in partial_solution {
                 ffsv.add(candidate);
             }
         }
 
         Ok(ffsv.into())
@@ -236,15 +239,15 @@
         &self.path
     }
 
     pub fn config(&self) -> &VectorConfig {
         &self.config
     }
 
-    pub fn embedding_dimension(&self) -> Option<u64> {
+    pub fn embedding_dimension(&self) -> Option<usize> {
         self.dimension
     }
 
     pub fn needs_update(&self) -> VectorR<bool> {
         let state_path = self.path.join(STATE);
         let state_modified = last_modified(&state_path)?;
         Ok(self.state_last_modified < state_modified)
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-use crate::config::{Similarity, VectorConfig};
+use crate::config::VectorConfig;
 use crate::data_point::{self, DataPointPin, DpId, Journal, OpenDataPoint};
 use crate::data_point_provider::state::*;
 use crate::data_point_provider::state::{read_state, write_state};
 use crate::data_point_provider::TimeSensitiveDLog;
 use crate::data_point_provider::{IndexMetadata, OPENING_FLAG, STATE, TEMP_STATE, WRITING_FLAG};
 use crate::data_types::dtrie_ram::DTrie;
 use crate::{VectorErr, VectorR};
@@ -98,15 +98,15 @@
     }
 }
 
 pub struct PreparedMerge {
     dtrie_copy: DTrie,
     destination: Option<DataPointPin>,
     inputs: Vec<OpenDataPoint>,
-    similarity: Similarity,
+    config: VectorConfig,
     segments_left: usize,
     merge_time: SystemTime,
 }
 
 impl MergeRunner for PreparedMerge {
     fn run(&mut self) -> NodeResult<Box<dyn nucliadb_core::vectors::MergeResults>> {
         let start = Instant::now();
@@ -121,15 +121,15 @@
                             dlog: &self.dtrie_copy,
                         },
                         dp,
                     )
                 })
                 .collect::<Vec<_>>()
                 .as_slice(),
-            self.similarity,
+            &self.config,
             self.merge_time,
         )?;
         let metrics = MergeMetrics {
             seconds_elapsed: start.elapsed().as_secs_f64(),
             merged: self.inputs.len(),
             segments_left: self.segments_left,
             input_segment_sizes: self.inputs.iter().map(|dp| dp.journal().no_nodes()).collect(),
@@ -152,15 +152,16 @@
     has_uncommitted_changes: bool,
     config: VectorConfig,
     path: PathBuf,
     added_data_points: Vec<DataPointPin>,
     added_to_delete_log: Vec<(Vec<u8>, SystemTime)>,
     online_data_points: Vec<OnlineDataPoint>,
     delete_log: DTrie,
-    dimension: Option<u64>,
+    /// Only set when not specified by the vector config. TODO: To be removed
+    dimension: Option<usize>,
     number_of_embeddings: usize,
     #[allow(unused)]
     writing: File,
     shard_id: String,
 }
 
 impl Writer {
@@ -226,15 +227,15 @@
         }
 
         let destination = DataPointPin::create_pin(self.location())?;
         Ok(Some(Box::new(PreparedMerge {
             dtrie_copy,
             destination: Some(destination),
             inputs,
-            similarity: self.config.similarity,
+            config: self.config.clone(),
             segments_left: live_segments.len() + 1,
             merge_time: SystemTime::now(),
         })))
     }
 
     pub fn record_merge(&mut self, merge: &dyn MergeResults) -> VectorR<()> {
         let online_data_points = mem::take(&mut self.online_data_points);
@@ -414,15 +415,15 @@
                 journal: data_point_journal,
             };
 
             number_of_embeddings += online_data_point.journal.no_nodes();
             online_data_points.push(online_data_point);
         }
 
-        if dimension.is_none() {
+        if !config.known_dimensions() {
             if let Some(online_data_point) = online_data_points.first() {
                 let open_data_point = data_point::open(&online_data_point.pin)?;
                 dimension = open_data_point.stored_len();
             }
         }
 
         Ok(Writer {
@@ -456,15 +457,15 @@
         let mut new_number_of_embeddings = 0;
         let mut new_data_points = Vec::new();
 
         for data_point_id in data_point_list {
             let data_point_pin = DataPointPin::open_pin(&self.path, data_point_id)?;
             let data_point_journal = data_point_pin.read_journal()?;
 
-            if new_dimension.is_none() {
+            if !self.config.known_dimensions() && new_dimension.is_none() {
                 let data_point = data_point::open(&data_point_pin)?;
                 new_dimension = data_point.stored_len();
             }
 
             let online_data_point = OnlineDataPoint {
                 pin: data_point_pin,
                 journal: data_point_journal,
@@ -513,19 +514,18 @@
         let merge_parameters = MergeParameters {
             segments_before_merge: 10,
             max_nodes_in_merge: 50_000,
             maximum_deleted_entries: 25_000,
         };
 
         for _ in 0..100 {
-            let similarity = Similarity::Cosine;
             let embeddings = vec![];
             let time = Some(SystemTime::now());
             let data_point_pin = DataPointPin::create_pin(&vectors_path).unwrap();
-            create(&data_point_pin, embeddings, time, similarity).unwrap();
+            create(&data_point_pin, embeddings, time, &writer.config).unwrap();
 
             let online_data_point = OnlineDataPoint {
                 journal: data_point_pin.read_journal().unwrap(),
                 pin: data_point_pin,
             };
             data_points.push(online_data_point);
         }
@@ -548,19 +548,18 @@
         let merge_parameters = MergeParameters {
             segments_before_merge: 1000,
             max_nodes_in_merge: 50_000,
             maximum_deleted_entries: 25_000,
         };
 
         for _ in 0..50 {
-            let similarity = Similarity::Cosine;
             let embeddings = vec![];
             let time = Some(SystemTime::now());
             let data_point_pin = DataPointPin::create_pin(&vectors_path).unwrap();
-            create(&data_point_pin, embeddings, time, similarity).unwrap();
+            create(&data_point_pin, embeddings, time, &writer.config).unwrap();
 
             let online_data_point = OnlineDataPoint {
                 journal: data_point_pin.read_journal().unwrap(),
                 pin: data_point_pin,
             };
             data_points.push(online_data_point);
         }
@@ -581,19 +580,18 @@
         let merge_parameters = MergeParameters {
             segments_before_merge: 100,
             max_nodes_in_merge: 50_000,
             maximum_deleted_entries: 25_000,
         };
 
         for _ in 0..100 {
-            let similarity = Similarity::Cosine;
             let embeddings = vec![];
             let time = Some(SystemTime::now());
             let data_point_pin = DataPointPin::create_pin(&vectors_path).unwrap();
-            create(&data_point_pin, embeddings, time, similarity).unwrap();
+            create(&data_point_pin, embeddings, time, &writer.config).unwrap();
 
             let online_data_point = OnlineDataPoint {
                 journal: data_point_pin.read_journal().unwrap(),
                 pin: data_point_pin,
             };
             data_points.push(online_data_point);
         }
@@ -618,20 +616,18 @@
         // Writer with a single empty vector
         let mut writer = Writer::new(&vectors_path, VectorConfig::default(), "abc".into()).unwrap();
         let merge_parameters = MergeParameters {
             segments_before_merge: 1,
             max_nodes_in_merge: 50_000,
             maximum_deleted_entries: 10,
         };
-
-        let similarity = Similarity::Cosine;
         let embeddings = vec![];
         let time = Some(SystemTime::now());
         let data_point_pin = DataPointPin::create_pin(&vectors_path).unwrap();
-        create(&data_point_pin, embeddings, time, similarity).unwrap();
+        create(&data_point_pin, embeddings, time, &writer.config).unwrap();
 
         let online_data_point = OnlineDataPoint {
             journal: data_point_pin.read_journal().unwrap(),
             pin: data_point_pin,
         };
         writer.online_data_points = vec![online_data_point];
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::fs::File;
 use std::io::{self, BufWriter, Seek, SeekFrom, Write};
 
+use crate::config::{VectorConfig, VectorType};
+
 use super::usize_utils::*;
 
 // A data store schema.
 // The data is arrange in a way such that the following operations can be performed:
 // -> Given an id, find its value. O(1).
 // -> Get the total number of values, or valid ids.
 // N = Address size in bytes.
@@ -64,19 +66,20 @@
     // Slot.
     fn keep_in_merge(&self, _: &[u8]) -> bool {
         true
     }
 }
 
 pub trait IntoBuffer {
-    fn serialize_into<W: io::Write>(self, w: W) -> io::Result<()>;
+    fn serialize_into<W: io::Write>(self, w: W, vector_type: &VectorType) -> io::Result<()>;
 }
 
+#[cfg(test)]
 impl<T: AsRef<[u8]>> IntoBuffer for T {
-    fn serialize_into<W: io::Write>(self, mut w: W) -> io::Result<()> {
+    fn serialize_into<W: io::Write>(self, mut w: W, _: &VectorType) -> io::Result<()> {
         w.write_all(self.as_ref())
     }
 }
 
 // O(1)
 // Returns how many elements are in x, alive or deleted.
 pub fn stored_elements(x: &[u8]) -> usize {
@@ -89,24 +92,23 @@
     interpreter.read_exact(&src[pointer..]).0
 }
 
 use lazy_static::lazy_static;
 use libc;
 
 #[cfg(not(target_os = "windows"))]
-pub fn will_need(src: &[u8], id: usize, dimension: usize) {
+pub fn will_need(src: &[u8], id: usize, vector_len: usize) {
     lazy_static! {
         static ref PAGE_SIZE: usize = unsafe { libc::sysconf(libc::_SC_PAGESIZE) } as usize;
     };
 
     // Calculate node struct size without reading anything, so make some estimates
     // Will only load up to the vectors section, it ignores the key/labels because
     // they are harder to estimate and less useful (only when filtering, similarity is always used)
     let metadata_len = 16; // Estimate
-    let vector_len = dimension * 4 + 4;
     let node_size = HEADER_LEN + metadata_len + vector_len;
 
     // Align node pointer to the start page, as required by madvise
     let start = src.as_ptr().wrapping_add(get_pointer(src, id));
     let offset = start.align_offset(*PAGE_SIZE);
     let (start_page, advise_size) = if offset > 0 {
         (start.wrapping_add(offset).wrapping_sub(*PAGE_SIZE), node_size + *PAGE_SIZE - offset)
@@ -114,49 +116,63 @@
         (start, node_size)
     };
 
     unsafe { libc::madvise(start_page as *mut libc::c_void, advise_size, libc::MADV_WILLNEED) };
 }
 
 #[cfg(target_os = "windows")]
-pub fn will_need(src: &[u8], id: usize, dimension: usize) {}
+pub fn will_need(src: &[u8], id: usize, vector_len: usize) {}
 
-pub fn create_key_value<D: IntoBuffer>(recipient: &mut File, slots: Vec<D>) -> io::Result<()> {
+pub fn create_key_value<D: IntoBuffer>(
+    recipient: &mut File,
+    slots: Vec<D>,
+    vector_type: &VectorType,
+) -> io::Result<()> {
     let fixed_size = (HEADER_LEN + (POINTER_LEN * slots.len())) as u64;
     recipient.set_len(fixed_size)?;
 
     let number_of_values: [u8; POINTER_LEN] = slots.len().to_le_bytes();
     let mut recipient_buffer = BufWriter::new(recipient);
 
     // Writing the storage header
     recipient_buffer.seek(SeekFrom::Start(0))?;
     recipient_buffer.write_all(&number_of_values)?;
 
     // Serializing values into the recipient. Each slot is serialized at the end of the
     // loop and its address pointer is written in the pointer section.
     let mut pointer_section_cursor = HEADER_LEN as u64;
+    let alignment = vector_type.vector_alignment();
     for slot in slots {
         // slot serialization
-        let slot_address = recipient_buffer.seek(SeekFrom::End(0))?;
-        slot.serialize_into(&mut recipient_buffer)?;
+        let mut slot_address = recipient_buffer.seek(SeekFrom::End(0))?;
+        if slot_address as usize % alignment > 0 {
+            let pad = alignment - (slot_address as usize % alignment);
+            recipient_buffer.seek(SeekFrom::Current(pad as i64))?;
+            slot_address += pad as u64;
+        }
+        slot.serialize_into(&mut recipient_buffer, vector_type)?;
 
         // The slot address needs to be written in the pointer section
         recipient_buffer.seek(SeekFrom::Start(pointer_section_cursor))?;
         let slot_address_as_bytes = slot_address.to_le_bytes();
         recipient_buffer.write_all(&slot_address_as_bytes)?;
 
         // The cursor need to be moved forward
         pointer_section_cursor += POINTER_LEN as u64;
     }
 
     recipient_buffer.flush()
 }
 
 // Merge algorithm. Returns the number of elements merged into the file.
-pub fn merge<S: Interpreter + Copy>(recipient: &mut File, producers: &[(S, &[u8])]) -> io::Result<bool> {
+pub fn merge<S: Interpreter + Copy>(
+    recipient: &mut File,
+    producers: &[(S, &[u8])],
+    config: &VectorConfig,
+) -> io::Result<bool> {
     // Number of elements, deleted or alive.
     let mut prologue_section_size = HEADER_LEN;
     // To know the range of valid ids per producer
     let mut lengths = Vec::with_capacity(producers.len());
 
     // Computing lengths and total sizes
     for (_, store) in producers.iter().copied() {
@@ -180,14 +196,15 @@
     let mut written_elements: usize = 0;
     // Using a buffered writer for efficient transferring.
     let mut recipient_buffer = BufWriter::new(recipient);
     // Pointer to the next unused id slot
     let mut id_section_cursor = HEADER_LEN;
     let mut has_deletions = false;
 
+    let alignment = config.vector_type.vector_alignment();
     while producer_cursor < producers.len() {
         // If the end of the current producer was reached we move
         // to the start of the next producer.
         if element_cursor == lengths[producer_cursor] {
             element_cursor = 0;
             producer_cursor += 1;
             continue;
@@ -197,15 +214,20 @@
         // is transferred to the recipient.
         let (interpreter, store) = producers[producer_cursor];
         let element_pointer = get_pointer(store, element_cursor);
         let element_slice = &store[element_pointer..];
         if interpreter.keep_in_merge(element_slice) {
             // Moving to the end of the file to write the current element.
             let (exact_element, _) = interpreter.read_exact(element_slice);
-            let element_pointer = recipient_buffer.seek(SeekFrom::End(0))?;
+            let mut element_pointer = recipient_buffer.seek(SeekFrom::End(0))?;
+            if element_pointer as usize % alignment > 0 {
+                let pad = alignment - (element_pointer as usize % alignment);
+                recipient_buffer.seek(SeekFrom::Current(pad as i64))?;
+                element_pointer += pad as u64;
+            }
             recipient_buffer.write_all(exact_element)?;
             // Moving to the next free slot in the section id to write
             // the offset where the element was written.
             recipient_buffer.seek(SeekFrom::Start(id_section_cursor as u64))?;
             recipient_buffer.write_all(&element_pointer.to_le_bytes())?;
             id_section_cursor += POINTER_LEN;
             written_elements += 1;
@@ -259,15 +281,15 @@
 
     #[test]
     fn store_test() {
         let interpreter = TElem;
         let elems: [u32; 5] = [0, 1, 2, 3, 4];
         let expected: Vec<_> = elems.iter().map(|x| x.to_be_bytes()).collect();
         let mut buf = tempfile::tempfile().unwrap();
-        create_key_value(&mut buf, expected.clone()).unwrap();
+        create_key_value(&mut buf, expected.clone(), &VectorType::DenseF32Unaligned).unwrap();
 
         let buf_map = unsafe { memmap2::Mmap::map(&buf).unwrap() };
         let no_values = stored_elements(&buf_map);
         assert_eq!(no_values, expected.len());
         for (id, expected_value) in expected.iter().enumerate() {
             let actual_value = get_value(interpreter, &buf_map, id);
             let (head, tail) = interpreter.read_exact(actual_value);
@@ -284,26 +306,26 @@
         let v2: Vec<_> = [8u32, 9, 10, 11].iter().map(|x| x.to_be_bytes()).collect();
         let expected = [0u32, 1, 2, 4, 5, 7, 8, 9, 10, 11];
 
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let mut merge_store = tempfile::tempfile().unwrap();
         let elems = vec![(TElem, v0_map.as_ref()), (TElem, v1_map.as_ref()), (TElem, v2_map.as_ref())];
 
-        merge(&mut merge_store, &elems).unwrap();
+        merge(&mut merge_store, &elems, &VectorConfig::default()).unwrap();
         let merge_map = unsafe { memmap2::Mmap::map(&merge_store).unwrap() };
         let number_of_elements = stored_elements(&merge_map);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_map, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
 
@@ -318,17 +340,17 @@
         let v1: Vec<_> = [3u32, 4, 5, 11].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8, 9, 10].iter().map(|x| x.to_be_bytes()).collect();
 
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let interpreter = (GreaterThan(ONE), TElem);
         let mut merge_store = tempfile::tempfile().unwrap();
@@ -337,15 +359,15 @@
             (interpreter, v0_map.as_ref()),
             // no element is removed
             (interpreter, v1_map.as_ref()),
             // no element is removed
             (interpreter, v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
         let merge_map = unsafe { memmap2::Mmap::map(&merge_store).unwrap() };
         let number_of_elements = stored_elements(&merge_map);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_map, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
@@ -360,17 +382,17 @@
         let v0: Vec<_> = [0u32, 1, 2].iter().map(|x| x.to_be_bytes()).collect();
         let v1: Vec<_> = [3u32, 4, 5].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8].iter().map(|x| x.to_be_bytes()).collect();
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let interpreter = (GreaterThan(ONE), TElem);
         let mut merge_store = tempfile::tempfile().unwrap();
@@ -379,15 +401,15 @@
             (interpreter, v0_map.as_ref()),
             // no element is removed
             (interpreter, v1_map.as_ref()),
             // no element is removed
             (interpreter, v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![2, 3, 4, 5, 6, 7, 8];
         let merge_map = unsafe { memmap2::Mmap::map(&merge_store).unwrap() };
         let number_of_elements = stored_elements(&merge_map);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_map, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
@@ -402,17 +424,17 @@
         let v0: Vec<_> = [0u32, 1, 2].iter().map(|x| x.to_be_bytes()).collect();
         let v1: Vec<_> = [3u32, 4, 5].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8].iter().map(|x| x.to_be_bytes()).collect();
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let mut merge_store = tempfile::tempfile().unwrap();
         let elems = vec![
@@ -420,15 +442,15 @@
             ((GreaterThan(ZERO), TElem), v0_map.as_ref()),
             // The first element is deleted
             ((GreaterThan(THREE), TElem), v1_map.as_ref()),
             // The first element is deleted
             ((GreaterThan(SIX), TElem), v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut merge_store, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![1, 2, 4, 5, 7, 8];
         let merge_map = unsafe { memmap2::Mmap::map(&merge_store).unwrap() };
         let number_of_elements = stored_elements(&merge_map);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_map, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
@@ -443,17 +465,17 @@
         let v0: Vec<_> = [0u32, 1, 2].iter().map(|x| x.to_be_bytes()).collect();
         let v1: Vec<_> = [3u32, 4, 5].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8].iter().map(|x| x.to_be_bytes()).collect();
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let interpreter = (GreaterThan(TWO), TElem);
         let mut merge_storage = tempfile::tempfile().unwrap();
@@ -462,15 +484,15 @@
             (interpreter, v0_map.as_ref()),
             // no element is removed
             (interpreter, v1_map.as_ref()),
             // no element is removed
             (interpreter, v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut merge_storage, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut merge_storage, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![3, 4, 5, 6, 7, 8];
         let merge_store = unsafe { memmap2::Mmap::map(&merge_storage).unwrap() };
         let number_of_elements = stored_elements(&merge_store);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_store, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
@@ -485,17 +507,17 @@
         let v0: Vec<_> = [0u32, 1, 2].iter().map(|x| x.to_be_bytes()).collect();
         let v1: Vec<_> = [3u32, 4, 5].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8].iter().map(|x| x.to_be_bytes()).collect();
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let greater_than_2 = (GreaterThan(TWO), TElem);
         let greater_than_10 = (GreaterThan(TEN), TElem);
@@ -505,15 +527,15 @@
             (greater_than_2, v0_map.as_ref()),
             // no element are removed
             (greater_than_2, v1_map.as_ref()),
             // all the elements are removed
             (greater_than_10, v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut merge_storage, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut merge_storage, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![3, 4, 5];
         let merge_store = unsafe { memmap2::Mmap::map(&merge_storage).unwrap() };
         let number_of_elements = stored_elements(&merge_store);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_store, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
@@ -528,17 +550,17 @@
         let v0: Vec<_> = [0u32, 1, 2].iter().map(|x| x.to_be_bytes()).collect();
         let v1: Vec<_> = [3u32, 4, 5].iter().map(|x| x.to_be_bytes()).collect();
         let v2: Vec<_> = [6u32, 7, 8].iter().map(|x| x.to_be_bytes()).collect();
         let mut v0_store = tempfile::tempfile().unwrap();
         let mut v1_store = tempfile::tempfile().unwrap();
         let mut v2_store = tempfile::tempfile().unwrap();
 
-        create_key_value(&mut v0_store, v0).unwrap();
-        create_key_value(&mut v1_store, v1).unwrap();
-        create_key_value(&mut v2_store, v2).unwrap();
+        create_key_value(&mut v0_store, v0, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v1_store, v1, &VectorType::DenseF32Unaligned).unwrap();
+        create_key_value(&mut v2_store, v2, &VectorType::DenseF32Unaligned).unwrap();
 
         let v0_map = unsafe { memmap2::Mmap::map(&v0_store).unwrap() };
         let v1_map = unsafe { memmap2::Mmap::map(&v1_store).unwrap() };
         let v2_map = unsafe { memmap2::Mmap::map(&v2_store).unwrap() };
 
         let interpreter = (GreaterThan(TEN), TElem);
         let mut file = tempfile::tempfile().unwrap();
@@ -548,15 +570,15 @@
             (interpreter, v0_map.as_ref()),
             // all the elements are removed
             (interpreter, v1_map.as_ref()),
             // all the elements are removed
             (interpreter, v2_map.as_ref()),
         ];
 
-        merge::<(GreaterThan, TElem)>(&mut file, elems.as_slice()).unwrap();
+        merge::<(GreaterThan, TElem)>(&mut file, elems.as_slice(), &VectorConfig::default()).unwrap();
         let expected: Vec<u32> = vec![];
         let merge_store = unsafe { memmap2::Mmap::map(&file).unwrap() };
         let number_of_elements = stored_elements(&merge_store);
         let values: Vec<u32> = (0..number_of_elements)
             .map(|i| get_value(TElem, &merge_store, i))
             .map(|s| u32::from_be_bytes(s.try_into().unwrap()))
             .collect();
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,28 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 pub mod data_store;
 pub mod dtrie_ram;
 pub mod trie;
 pub mod trie_ram;
-pub mod vector;
 
 pub mod usize_utils {
     pub const USIZE_LEN: usize = (usize::BITS / 8) as usize;
     pub fn usize_from_slice_le(v: &[u8]) -> usize {
         let mut buff = [0; USIZE_LEN];
         buff.copy_from_slice(v);
         usize::from_le_bytes(buff)
     }
+    pub const U32_LEN: usize = (u32::BITS / 8) as usize;
+    pub fn u32_from_slice_le(v: &[u8]) -> u32 {
+        let mut buff = [0; U32_LEN];
+        buff.copy_from_slice(v);
+        u32::from_le_bytes(buff)
+    }
 }
 
 pub trait DeleteLog: std::marker::Sync {
     fn is_deleted(&self, _: &[u8]) -> bool;
 }
 
 impl<'a, D: DeleteLog> DeleteLog for &'a D {
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::io::{Read, Write};
+
 type Len = u64;
 type Unit = f32;
-type Dist = f32;
 
 fn encode_length(mut buff: Vec<u8>, vec: &[Unit]) -> Vec<u8> {
     let len = vec.len() as Len;
     buff.write_all(&len.to_le_bytes()).unwrap();
     buff.flush().unwrap();
     buff
 }
@@ -37,15 +37,15 @@
 
 pub fn vector_len(mut x: &[u8]) -> u64 {
     let mut buff_x = [0; 8];
     x.read_exact(&mut buff_x).unwrap();
     Len::from_le_bytes(buff_x)
 }
 
-pub fn cosine_similarity(mut x: &[u8], mut y: &[u8]) -> Dist {
+pub fn cosine_similarity(mut x: &[u8], mut y: &[u8]) -> f32 {
     let mut buff_x = [0; 8];
     let mut buff_y = [0; 8];
     x.read_exact(&mut buff_x).unwrap();
     y.read_exact(&mut buff_y).unwrap();
     let len_x = Len::from_le_bytes(buff_x);
     let len_y = Len::from_le_bytes(buff_y);
     assert_eq!(len_x, len_y);
@@ -63,15 +63,15 @@
         sum += x_value * y_value;
         dem_x += x_value * x_value;
         dem_y += y_value * y_value;
     }
     sum / (f32::sqrt(dem_x) * f32::sqrt(dem_y))
 }
 
-pub fn dot_similarity(mut x: &[u8], mut y: &[u8]) -> Dist {
+pub fn dot_similarity(mut x: &[u8], mut y: &[u8]) -> f32 {
     let mut buff_x = [0; 8];
     let mut buff_y = [0; 8];
     x.read_exact(&mut buff_x).unwrap();
     y.read_exact(&mut buff_y).unwrap();
     let len_x = Len::from_le_bytes(buff_x);
     let len_y = Len::from_le_bytes(buff_y);
     assert_eq!(len_x, len_y);
@@ -92,15 +92,15 @@
 pub fn encode_vector(vec: &[Unit]) -> Vec<u8> {
     vec.iter().cloned().fold(encode_length(vec![], vec), encode_unit)
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
-    fn naive_cosine_similatiry(a: &[f32], b: &[f32]) -> f32 {
+    fn naive_cosine_similarity(a: &[f32], b: &[f32]) -> f32 {
         let ab: f32 = a.iter().cloned().zip(b.iter().cloned()).map(|(a, b)| a * b).sum();
         let aa: f32 = a.iter().cloned().map(|a| a * a).sum();
         let bb: f32 = b.iter().cloned().map(|b| b * b).sum();
         ab / (f32::sqrt(aa) * f32::sqrt(bb))
     }
 
     fn naive_dot_similatiry(a: &[f32], b: &[f32]) -> f32 {
@@ -109,21 +109,21 @@
 
     #[test]
     fn cosine_test() {
         let v0: Vec<_> = (0..758).map(|i| (i * 2) as f32).collect();
         let v1: Vec<_> = (0..758).map(|i| ((i * 2) + 1) as f32).collect();
         let v0_r = encode_vector(&v0);
         let v1_r = encode_vector(&v1);
-        assert_eq!(naive_cosine_similatiry(&v0, &v1), cosine_similarity(&v0_r, &v1_r));
-        assert_eq!(naive_cosine_similatiry(&v0, &v0), cosine_similarity(&v0_r, &v0_r));
+        assert_eq!(naive_cosine_similarity(&v0, &v1), cosine_similarity(&v0_r, &v1_r));
+        assert_eq!(naive_cosine_similarity(&v0, &v0), cosine_similarity(&v0_r, &v0_r));
     }
 
     #[test]
     fn dot_test() {
         let v0: Vec<_> = (0..758).map(|i| (i * 2) as f32).collect();
         let v1: Vec<_> = (0..758).map(|i| ((i * 2) + 1) as f32).collect();
         let v0_r = encode_vector(&v0);
         let v1_r = encode_vector(&v1);
         assert_eq!(naive_dot_similatiry(&v0, &v1), dot_similarity(&v0_r, &v1_r));
-        assert_eq!(naive_dot_similatiry(&v0, &v1), dot_similarity(&v0_r, &v1_r));
+        assert_eq!(naive_dot_similatiry(&v0, &v0), dot_similarity(&v0_r, &v0_r));
     }
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 pub mod config;
 pub mod data_point;
 pub mod data_point_provider;
 mod data_types;
 pub mod formula;
 pub mod service;
 mod utils;
+mod vector_types;
 
 use thiserror::Error;
 #[derive(Debug, Error)]
 pub enum VectorErr {
     #[error("Error using bincode: {0}")]
     BincodeError(#[from] bincode::Error),
     #[error("Error using fst: {0}")]
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,16 @@
         if lengths.len() > 1 {
             return Ok(tracing::error!("{}", self.dimensions_report(lengths)));
         }
 
         if !elems.is_empty() {
             let location = self.index.location();
             let time = Some(temporal_mark);
-            let similarity = self.index.config().similarity;
             let data_point_pin = DataPointPin::create_pin(location)?;
-            data_point::create(&data_point_pin, elems, time, similarity)?;
+            data_point::create(&data_point_pin, elems, time, self.index.config())?;
             self.index.add_data_point(data_point_pin)?;
         }
 
         for to_delete in resource.sentences_to_delete() {
             let key_as_bytes = to_delete.as_bytes();
             self.index.record_delete(key_as_bytes, temporal_mark);
         }
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,27 @@
 }
 
 #[test]
 fn test_concurrent_merge_delete() -> NodeResult<()> {
     let workdir = tempdir()?;
     let index_path = workdir.path().join("vectors");
     let config = VectorConfig::default();
-    let similarity = config.similarity;
-    let mut writer = Writer::new(&index_path, config, "abc".into())?;
+    let mut writer = Writer::new(&index_path, config.clone(), "abc".into())?;
 
     let now = SystemTime::now();
     let past = now - Duration::from_secs(5);
 
     // Create two segments
     let data_point_pin = DataPointPin::create_pin(&index_path)?;
-    data_point::create(&data_point_pin, vec![elem(0)], Some(past), similarity)?;
+    data_point::create(&data_point_pin, vec![elem(0)], Some(past), &config)?;
     writer.add_data_point(data_point_pin)?;
     writer.commit()?;
 
     let data_point_pin = DataPointPin::create_pin(&index_path)?;
-    data_point::create(&data_point_pin, vec![elem(1)], Some(past), similarity)?;
+    data_point::create(&data_point_pin, vec![elem(1)], Some(past), &config)?;
     writer.add_data_point(data_point_pin)?;
     writer.commit()?;
 
     // Merge the two segments and simultaneously remove something
     let to_delete = elem(0);
     let mut merge = writer
         .prepare_merge(MergeParameters {
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 pub struct MergeContext {
     pub parameters: MergeParameters,
     pub source: MergeSource,
 }
 
 #[derive(Clone)]
-pub struct VectorConfig {
+pub struct VectorIndexConfig {
     pub similarity: utils::VectorSimilarity,
     pub path: PathBuf,
     pub channel: Channel,
     pub shard_id: String,
     pub normalize_vectors: bool,
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.1.post1380/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/Cargo.toml` & `nucliadb_node_binding-4.0.1.post1380/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "4.0.1-post1376"
+version = "4.0.1-post1380"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/.cargo/config.toml` & `nucliadb_node_binding-4.0.1.post1380/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/CHANGELOG.md` & `nucliadb_node_binding-4.0.1.post1380/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/Makefile` & `nucliadb_node_binding-4.0.1.post1380/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/cov.sh` & `nucliadb_node_binding-4.0.1.post1380/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/audit.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/audit.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/dataset.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/dataset.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/knowledgebox.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/knowledgebox.proto`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 syntax = "proto3";
 
 package knowledgebox;
 
 import public "nucliadb_protos/utils.proto";
+import public "nucliadb_protos/nodewriter.proto";
 
 
 enum KnowledgeBoxResponseStatus {
     OK = 0;
     CONFLICT = 1;
     NOTFOUND = 2;
     ERROR = 3;
@@ -176,14 +177,31 @@
 }
 
 message VectorSets {
     map<string, VectorSet> vectorsets = 1;
 }
 
 
+// Configuration values for a vectorset
+message VectorSetConfig {
+    string vectorset_id = 1;
+
+    nodewriter.VectorIndexConfig vectorset_index_config = 2;
+
+    // list of possible subdivisions of the matryoshka embeddings (if the model
+    // supports it)
+    repeated uint32 matryoshka_dimensions = 3;
+}
+
+// KB vectorsets and their configuration
+message KnowledgeBoxVectorSetsConfig {
+    repeated VectorSetConfig vectorsets = 1;
+}
+
+
 // Synonyms of a Knowledge Box
 
 message TermSynonyms {
     repeated string synonyms = 1;
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/nodereader.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/nodereader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/noderesources.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/noderesources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/nodewriter.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/nodewriter.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/audit_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,28 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from nucliadb_protos import utils_pb2 as nucliadb__protos_dot_utils__pb2
+from nucliadb_protos import nodewriter_pb2 as nucliadb__protos_dot_nodewriter__pb2
+try:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_nodewriter__pb2.nucliadb__protos_dot_noderesources__pb2
+except AttributeError:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_nodewriter__pb2.nucliadb_protos.noderesources_pb2
+try:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_nodewriter__pb2.nucliadb__protos_dot_utils__pb2
+except AttributeError:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_nodewriter__pb2.nucliadb_protos.utils_pb2
 
 from nucliadb_protos.utils_pb2 import *
+from nucliadb_protos.nodewriter_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"nucliadb_protos/knowledgebox.proto\x12\x0cknowledgebox\x1a\x1bnucliadb_protos/utils.proto\",\n\x0eKnowledgeBoxID\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\xed\x01\n\x12KnowledgeBoxConfig\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x0f\x65nabled_filters\x18\x03 \x03(\tB\x02\x18\x01\x12\x1c\n\x10\x65nabled_insights\x18\x04 \x03(\tB\x02\x18\x01\x12\x0c\n\x04slug\x18\x05 \x01(\t\x12\x1b\n\x0f\x64isable_vectors\x18\x06 \x01(\x08\x42\x02\x18\x01\x12\x19\n\x11migration_version\x18\x07 \x01(\x03\x12\x32\n\x0frelease_channel\x18\x08 \x01(\x0e\x32\x15.utils.ReleaseChannelB\x02\x18\x01\"\xe7\x02\n\x0fKnowledgeBoxNew\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x30\n\x06\x63onfig\x18\x02 \x01(\x0b\x32 .knowledgebox.KnowledgeBoxConfig\x12\x11\n\tforceuuid\x18\x03 \x01(\t\x12+\n\nsimilarity\x18\x04 \x01(\x0e\x32\x17.utils.VectorSimilarity\x12\x1d\n\x10vector_dimension\x18\x05 \x01(\x05H\x00\x88\x01\x01\x12\"\n\x11\x64\x65\x66\x61ult_min_score\x18\x06 \x01(\x02\x42\x02\x18\x01H\x01\x88\x01\x01\x12\x1d\n\x15matryoshka_dimensions\x18\t \x03(\r\x12\x17\n\x0flearning_config\x18\x08 \x01(\t\x12.\n\x0frelease_channel\x18\x07 \x01(\x0e\x32\x15.utils.ReleaseChannelB\x13\n\x11_vector_dimensionB\x14\n\x12_default_min_score\"a\n\x17NewKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"b\n\x12KnowledgeBoxUpdate\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x30\n\x06\x63onfig\x18\x03 \x01(\x0b\x32 .knowledgebox.KnowledgeBoxConfig\"d\n\x1aUpdateKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\x18\n\x16GCKnowledgeBoxResponse\"V\n\x1a\x44\x65leteKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\"B\n\x05Label\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07related\x18\x03 \x01(\t\x12\x0c\n\x04text\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\"\xe0\x01\n\x08LabelSet\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63olor\x18\x02 \x01(\t\x12#\n\x06labels\x18\x03 \x03(\x0b\x32\x13.knowledgebox.Label\x12\x10\n\x08multiple\x18\x04 \x01(\x08\x12\x31\n\x04kind\x18\x05 \x03(\x0e\x32#.knowledgebox.LabelSet.LabelSetKind\"L\n\x0cLabelSetKind\x12\r\n\tRESOURCES\x10\x00\x12\x0e\n\nPARAGRAPHS\x10\x01\x12\r\n\tSENTENCES\x10\x02\x12\x0e\n\nSELECTIONS\x10\x03\"\x87\x01\n\x06Labels\x12\x34\n\x08labelset\x18\x01 \x03(\x0b\x32\".knowledgebox.Labels.LabelsetEntry\x1aG\n\rLabelsetEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.knowledgebox.LabelSet:\x02\x38\x01\"L\n\x06\x45ntity\x12\r\n\x05value\x18\x02 \x01(\t\x12\x12\n\nrepresents\x18\x04 \x03(\t\x12\x0e\n\x06merged\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65leted\x18\x05 \x01(\x08\"D\n\x14\x45ntitiesGroupSummary\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x04 \x01(\x08\"\xc1\x01\n\rEntitiesGroup\x12;\n\x08\x65ntities\x18\x01 \x03(\x0b\x32).knowledgebox.EntitiesGroup.EntitiesEntry\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x04 \x01(\x08\x1a\x45\n\rEntitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\"0\n\x15\x44\x65letedEntitiesGroups\x12\x17\n\x0f\x65ntities_groups\x18\x01 \x03(\t\"\xaf\x01\n\x0e\x45ntitiesGroups\x12I\n\x0f\x65ntities_groups\x18\x01 \x03(\x0b\x32\x30.knowledgebox.EntitiesGroups.EntitiesGroupsEntry\x1aR\n\x13\x45ntitiesGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup:\x02\x38\x01\"\xf3\x03\n\x19\x45ntityGroupDuplicateIndex\x12T\n\x0f\x65ntities_groups\x18\x01 \x03(\x0b\x32;.knowledgebox.EntityGroupDuplicateIndex.EntitiesGroupsEntry\x1a&\n\x10\x45ntityDuplicates\x12\x12\n\nduplicates\x18\x01 \x03(\t\x1a\xe1\x01\n\x15\x45ntityGroupDuplicates\x12]\n\x08\x65ntities\x18\x01 \x03(\x0b\x32K.knowledgebox.EntityGroupDuplicateIndex.EntityGroupDuplicates.EntitiesEntry\x1ai\n\rEntitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x38.knowledgebox.EntityGroupDuplicateIndex.EntityDuplicates:\x02\x38\x01\x1at\n\x13\x45ntitiesGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12L\n\x05value\x18\x02 \x01(\x0b\x32=.knowledgebox.EntityGroupDuplicateIndex.EntityGroupDuplicates:\x02\x38\x01\"K\n\tVectorSet\x12\x11\n\tdimension\x18\x01 \x01(\x05\x12+\n\nsimilarity\x18\x02 \x01(\x0e\x32\x17.utils.VectorSimilarity\"\x96\x01\n\nVectorSets\x12<\n\nvectorsets\x18\x01 \x03(\x0b\x32(.knowledgebox.VectorSets.VectorsetsEntry\x1aJ\n\x0fVectorsetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.knowledgebox.VectorSet:\x02\x38\x01\" \n\x0cTermSynonyms\x12\x10\n\x08synonyms\x18\x01 \x03(\t\"\x86\x01\n\x08Synonyms\x12\x30\n\x05terms\x18\x01 \x03(\x0b\x32!.knowledgebox.Synonyms.TermsEntry\x1aH\n\nTermsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.knowledgebox.TermSynonyms:\x02\x38\x01\"\xda\x01\n\x15SemanticModelMetadata\x12\x34\n\x13similarity_function\x18\x01 \x01(\x0e\x32\x17.utils.VectorSimilarity\x12\x1d\n\x10vector_dimension\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\"\n\x11\x64\x65\x66\x61ult_min_score\x18\x03 \x01(\x02\x42\x02\x18\x01H\x01\x88\x01\x01\x12\x1d\n\x15matryoshka_dimensions\x18\x04 \x03(\rB\x13\n\x11_vector_dimensionB\x14\n\x12_default_min_score\"\x8c\x01\n\x0fKBConfiguration\x12\x16\n\x0esemantic_model\x18\x02 \x01(\t\x12\x18\n\x10generative_model\x18\x03 \x01(\t\x12\x11\n\tner_model\x18\x04 \x01(\t\x12\x1b\n\x13\x61nonymization_model\x18\x05 \x01(\t\x12\x17\n\x0fvisual_labeling\x18\x06 \x01(\t*K\n\x1aKnowledgeBoxResponseStatus\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08\x43ONFLICT\x10\x01\x12\x0c\n\x08NOTFOUND\x10\x02\x12\t\n\x05\x45RROR\x10\x03P\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"nucliadb_protos/knowledgebox.proto\x12\x0cknowledgebox\x1a\x1bnucliadb_protos/utils.proto\x1a nucliadb_protos/nodewriter.proto\",\n\x0eKnowledgeBoxID\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\xed\x01\n\x12KnowledgeBoxConfig\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x0f\x65nabled_filters\x18\x03 \x03(\tB\x02\x18\x01\x12\x1c\n\x10\x65nabled_insights\x18\x04 \x03(\tB\x02\x18\x01\x12\x0c\n\x04slug\x18\x05 \x01(\t\x12\x1b\n\x0f\x64isable_vectors\x18\x06 \x01(\x08\x42\x02\x18\x01\x12\x19\n\x11migration_version\x18\x07 \x01(\x03\x12\x32\n\x0frelease_channel\x18\x08 \x01(\x0e\x32\x15.utils.ReleaseChannelB\x02\x18\x01\"\xe7\x02\n\x0fKnowledgeBoxNew\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x30\n\x06\x63onfig\x18\x02 \x01(\x0b\x32 .knowledgebox.KnowledgeBoxConfig\x12\x11\n\tforceuuid\x18\x03 \x01(\t\x12+\n\nsimilarity\x18\x04 \x01(\x0e\x32\x17.utils.VectorSimilarity\x12\x1d\n\x10vector_dimension\x18\x05 \x01(\x05H\x00\x88\x01\x01\x12\"\n\x11\x64\x65\x66\x61ult_min_score\x18\x06 \x01(\x02\x42\x02\x18\x01H\x01\x88\x01\x01\x12\x1d\n\x15matryoshka_dimensions\x18\t \x03(\r\x12\x17\n\x0flearning_config\x18\x08 \x01(\t\x12.\n\x0frelease_channel\x18\x07 \x01(\x0e\x32\x15.utils.ReleaseChannelB\x13\n\x11_vector_dimensionB\x14\n\x12_default_min_score\"a\n\x17NewKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"b\n\x12KnowledgeBoxUpdate\x12\x0c\n\x04slug\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x30\n\x06\x63onfig\x18\x03 \x01(\x0b\x32 .knowledgebox.KnowledgeBoxConfig\"d\n\x1aUpdateKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\x18\n\x16GCKnowledgeBoxResponse\"V\n\x1a\x44\x65leteKnowledgeBoxResponse\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.knowledgebox.KnowledgeBoxResponseStatus\"B\n\x05Label\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07related\x18\x03 \x01(\t\x12\x0c\n\x04text\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\"\xe0\x01\n\x08LabelSet\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63olor\x18\x02 \x01(\t\x12#\n\x06labels\x18\x03 \x03(\x0b\x32\x13.knowledgebox.Label\x12\x10\n\x08multiple\x18\x04 \x01(\x08\x12\x31\n\x04kind\x18\x05 \x03(\x0e\x32#.knowledgebox.LabelSet.LabelSetKind\"L\n\x0cLabelSetKind\x12\r\n\tRESOURCES\x10\x00\x12\x0e\n\nPARAGRAPHS\x10\x01\x12\r\n\tSENTENCES\x10\x02\x12\x0e\n\nSELECTIONS\x10\x03\"\x87\x01\n\x06Labels\x12\x34\n\x08labelset\x18\x01 \x03(\x0b\x32\".knowledgebox.Labels.LabelsetEntry\x1aG\n\rLabelsetEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.knowledgebox.LabelSet:\x02\x38\x01\"L\n\x06\x45ntity\x12\r\n\x05value\x18\x02 \x01(\t\x12\x12\n\nrepresents\x18\x04 \x03(\t\x12\x0e\n\x06merged\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65leted\x18\x05 \x01(\x08\"D\n\x14\x45ntitiesGroupSummary\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x04 \x01(\x08\"\xc1\x01\n\rEntitiesGroup\x12;\n\x08\x65ntities\x18\x01 \x03(\x0b\x32).knowledgebox.EntitiesGroup.EntitiesEntry\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x04 \x01(\x08\x1a\x45\n\rEntitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\"0\n\x15\x44\x65letedEntitiesGroups\x12\x17\n\x0f\x65ntities_groups\x18\x01 \x03(\t\"\xaf\x01\n\x0e\x45ntitiesGroups\x12I\n\x0f\x65ntities_groups\x18\x01 \x03(\x0b\x32\x30.knowledgebox.EntitiesGroups.EntitiesGroupsEntry\x1aR\n\x13\x45ntitiesGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup:\x02\x38\x01\"\xf3\x03\n\x19\x45ntityGroupDuplicateIndex\x12T\n\x0f\x65ntities_groups\x18\x01 \x03(\x0b\x32;.knowledgebox.EntityGroupDuplicateIndex.EntitiesGroupsEntry\x1a&\n\x10\x45ntityDuplicates\x12\x12\n\nduplicates\x18\x01 \x03(\t\x1a\xe1\x01\n\x15\x45ntityGroupDuplicates\x12]\n\x08\x65ntities\x18\x01 \x03(\x0b\x32K.knowledgebox.EntityGroupDuplicateIndex.EntityGroupDuplicates.EntitiesEntry\x1ai\n\rEntitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x38.knowledgebox.EntityGroupDuplicateIndex.EntityDuplicates:\x02\x38\x01\x1at\n\x13\x45ntitiesGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12L\n\x05value\x18\x02 \x01(\x0b\x32=.knowledgebox.EntityGroupDuplicateIndex.EntityGroupDuplicates:\x02\x38\x01\"K\n\tVectorSet\x12\x11\n\tdimension\x18\x01 \x01(\x05\x12+\n\nsimilarity\x18\x02 \x01(\x0e\x32\x17.utils.VectorSimilarity\"\x96\x01\n\nVectorSets\x12<\n\nvectorsets\x18\x01 \x03(\x0b\x32(.knowledgebox.VectorSets.VectorsetsEntry\x1aJ\n\x0fVectorsetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.knowledgebox.VectorSet:\x02\x38\x01\"\x85\x01\n\x0fVectorSetConfig\x12\x14\n\x0cvectorset_id\x18\x01 \x01(\t\x12=\n\x16vectorset_index_config\x18\x02 \x01(\x0b\x32\x1d.nodewriter.VectorIndexConfig\x12\x1d\n\x15matryoshka_dimensions\x18\x03 \x03(\r\"Q\n\x1cKnowledgeBoxVectorSetsConfig\x12\x31\n\nvectorsets\x18\x01 \x03(\x0b\x32\x1d.knowledgebox.VectorSetConfig\" \n\x0cTermSynonyms\x12\x10\n\x08synonyms\x18\x01 \x03(\t\"\x86\x01\n\x08Synonyms\x12\x30\n\x05terms\x18\x01 \x03(\x0b\x32!.knowledgebox.Synonyms.TermsEntry\x1aH\n\nTermsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.knowledgebox.TermSynonyms:\x02\x38\x01\"\xda\x01\n\x15SemanticModelMetadata\x12\x34\n\x13similarity_function\x18\x01 \x01(\x0e\x32\x17.utils.VectorSimilarity\x12\x1d\n\x10vector_dimension\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\"\n\x11\x64\x65\x66\x61ult_min_score\x18\x03 \x01(\x02\x42\x02\x18\x01H\x01\x88\x01\x01\x12\x1d\n\x15matryoshka_dimensions\x18\x04 \x03(\rB\x13\n\x11_vector_dimensionB\x14\n\x12_default_min_score\"\x8c\x01\n\x0fKBConfiguration\x12\x16\n\x0esemantic_model\x18\x02 \x01(\t\x12\x18\n\x10generative_model\x18\x03 \x01(\t\x12\x11\n\tner_model\x18\x04 \x01(\t\x12\x1b\n\x13\x61nonymization_model\x18\x05 \x01(\t\x12\x17\n\x0fvisual_labeling\x18\x06 \x01(\t*K\n\x1aKnowledgeBoxResponseStatus\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08\x43ONFLICT\x10\x01\x12\x0c\n\x08NOTFOUND\x10\x02\x12\t\n\x05\x45RROR\x10\x03P\x00P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nucliadb_protos.knowledgebox_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_KNOWLEDGEBOXCONFIG'].fields_by_name['enabled_filters']._options = None
@@ -45,76 +55,80 @@
   _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITIESGROUPSENTRY']._serialized_options = b'8\001'
   _globals['_VECTORSETS_VECTORSETSENTRY']._options = None
   _globals['_VECTORSETS_VECTORSETSENTRY']._serialized_options = b'8\001'
   _globals['_SYNONYMS_TERMSENTRY']._options = None
   _globals['_SYNONYMS_TERMSENTRY']._serialized_options = b'8\001'
   _globals['_SEMANTICMODELMETADATA'].fields_by_name['default_min_score']._options = None
   _globals['_SEMANTICMODELMETADATA'].fields_by_name['default_min_score']._serialized_options = b'\030\001'
-  _globals['_KNOWLEDGEBOXRESPONSESTATUS']._serialized_start=3416
-  _globals['_KNOWLEDGEBOXRESPONSESTATUS']._serialized_end=3491
-  _globals['_KNOWLEDGEBOXID']._serialized_start=81
-  _globals['_KNOWLEDGEBOXID']._serialized_end=125
-  _globals['_KNOWLEDGEBOXCONFIG']._serialized_start=128
-  _globals['_KNOWLEDGEBOXCONFIG']._serialized_end=365
-  _globals['_KNOWLEDGEBOXNEW']._serialized_start=368
-  _globals['_KNOWLEDGEBOXNEW']._serialized_end=727
-  _globals['_NEWKNOWLEDGEBOXRESPONSE']._serialized_start=729
-  _globals['_NEWKNOWLEDGEBOXRESPONSE']._serialized_end=826
-  _globals['_KNOWLEDGEBOXUPDATE']._serialized_start=828
-  _globals['_KNOWLEDGEBOXUPDATE']._serialized_end=926
-  _globals['_UPDATEKNOWLEDGEBOXRESPONSE']._serialized_start=928
-  _globals['_UPDATEKNOWLEDGEBOXRESPONSE']._serialized_end=1028
-  _globals['_GCKNOWLEDGEBOXRESPONSE']._serialized_start=1030
-  _globals['_GCKNOWLEDGEBOXRESPONSE']._serialized_end=1054
-  _globals['_DELETEKNOWLEDGEBOXRESPONSE']._serialized_start=1056
-  _globals['_DELETEKNOWLEDGEBOXRESPONSE']._serialized_end=1142
-  _globals['_LABEL']._serialized_start=1144
-  _globals['_LABEL']._serialized_end=1210
-  _globals['_LABELSET']._serialized_start=1213
-  _globals['_LABELSET']._serialized_end=1437
-  _globals['_LABELSET_LABELSETKIND']._serialized_start=1361
-  _globals['_LABELSET_LABELSETKIND']._serialized_end=1437
-  _globals['_LABELS']._serialized_start=1440
-  _globals['_LABELS']._serialized_end=1575
-  _globals['_LABELS_LABELSETENTRY']._serialized_start=1504
-  _globals['_LABELS_LABELSETENTRY']._serialized_end=1575
-  _globals['_ENTITY']._serialized_start=1577
-  _globals['_ENTITY']._serialized_end=1653
-  _globals['_ENTITIESGROUPSUMMARY']._serialized_start=1655
-  _globals['_ENTITIESGROUPSUMMARY']._serialized_end=1723
-  _globals['_ENTITIESGROUP']._serialized_start=1726
-  _globals['_ENTITIESGROUP']._serialized_end=1919
-  _globals['_ENTITIESGROUP_ENTITIESENTRY']._serialized_start=1850
-  _globals['_ENTITIESGROUP_ENTITIESENTRY']._serialized_end=1919
-  _globals['_DELETEDENTITIESGROUPS']._serialized_start=1921
-  _globals['_DELETEDENTITIESGROUPS']._serialized_end=1969
-  _globals['_ENTITIESGROUPS']._serialized_start=1972
-  _globals['_ENTITIESGROUPS']._serialized_end=2147
-  _globals['_ENTITIESGROUPS_ENTITIESGROUPSENTRY']._serialized_start=2065
-  _globals['_ENTITIESGROUPS_ENTITIESGROUPSENTRY']._serialized_end=2147
-  _globals['_ENTITYGROUPDUPLICATEINDEX']._serialized_start=2150
-  _globals['_ENTITYGROUPDUPLICATEINDEX']._serialized_end=2649
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYDUPLICATES']._serialized_start=2265
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYDUPLICATES']._serialized_end=2303
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES']._serialized_start=2306
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES']._serialized_end=2531
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES_ENTITIESENTRY']._serialized_start=2426
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES_ENTITIESENTRY']._serialized_end=2531
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITIESGROUPSENTRY']._serialized_start=2533
-  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITIESGROUPSENTRY']._serialized_end=2649
-  _globals['_VECTORSET']._serialized_start=2651
-  _globals['_VECTORSET']._serialized_end=2726
-  _globals['_VECTORSETS']._serialized_start=2729
-  _globals['_VECTORSETS']._serialized_end=2879
-  _globals['_VECTORSETS_VECTORSETSENTRY']._serialized_start=2805
-  _globals['_VECTORSETS_VECTORSETSENTRY']._serialized_end=2879
-  _globals['_TERMSYNONYMS']._serialized_start=2881
-  _globals['_TERMSYNONYMS']._serialized_end=2913
-  _globals['_SYNONYMS']._serialized_start=2916
-  _globals['_SYNONYMS']._serialized_end=3050
-  _globals['_SYNONYMS_TERMSENTRY']._serialized_start=2978
-  _globals['_SYNONYMS_TERMSENTRY']._serialized_end=3050
-  _globals['_SEMANTICMODELMETADATA']._serialized_start=3053
-  _globals['_SEMANTICMODELMETADATA']._serialized_end=3271
-  _globals['_KBCONFIGURATION']._serialized_start=3274
-  _globals['_KBCONFIGURATION']._serialized_end=3414
+  _globals['_KNOWLEDGEBOXRESPONSESTATUS']._serialized_start=3669
+  _globals['_KNOWLEDGEBOXRESPONSESTATUS']._serialized_end=3744
+  _globals['_KNOWLEDGEBOXID']._serialized_start=115
+  _globals['_KNOWLEDGEBOXID']._serialized_end=159
+  _globals['_KNOWLEDGEBOXCONFIG']._serialized_start=162
+  _globals['_KNOWLEDGEBOXCONFIG']._serialized_end=399
+  _globals['_KNOWLEDGEBOXNEW']._serialized_start=402
+  _globals['_KNOWLEDGEBOXNEW']._serialized_end=761
+  _globals['_NEWKNOWLEDGEBOXRESPONSE']._serialized_start=763
+  _globals['_NEWKNOWLEDGEBOXRESPONSE']._serialized_end=860
+  _globals['_KNOWLEDGEBOXUPDATE']._serialized_start=862
+  _globals['_KNOWLEDGEBOXUPDATE']._serialized_end=960
+  _globals['_UPDATEKNOWLEDGEBOXRESPONSE']._serialized_start=962
+  _globals['_UPDATEKNOWLEDGEBOXRESPONSE']._serialized_end=1062
+  _globals['_GCKNOWLEDGEBOXRESPONSE']._serialized_start=1064
+  _globals['_GCKNOWLEDGEBOXRESPONSE']._serialized_end=1088
+  _globals['_DELETEKNOWLEDGEBOXRESPONSE']._serialized_start=1090
+  _globals['_DELETEKNOWLEDGEBOXRESPONSE']._serialized_end=1176
+  _globals['_LABEL']._serialized_start=1178
+  _globals['_LABEL']._serialized_end=1244
+  _globals['_LABELSET']._serialized_start=1247
+  _globals['_LABELSET']._serialized_end=1471
+  _globals['_LABELSET_LABELSETKIND']._serialized_start=1395
+  _globals['_LABELSET_LABELSETKIND']._serialized_end=1471
+  _globals['_LABELS']._serialized_start=1474
+  _globals['_LABELS']._serialized_end=1609
+  _globals['_LABELS_LABELSETENTRY']._serialized_start=1538
+  _globals['_LABELS_LABELSETENTRY']._serialized_end=1609
+  _globals['_ENTITY']._serialized_start=1611
+  _globals['_ENTITY']._serialized_end=1687
+  _globals['_ENTITIESGROUPSUMMARY']._serialized_start=1689
+  _globals['_ENTITIESGROUPSUMMARY']._serialized_end=1757
+  _globals['_ENTITIESGROUP']._serialized_start=1760
+  _globals['_ENTITIESGROUP']._serialized_end=1953
+  _globals['_ENTITIESGROUP_ENTITIESENTRY']._serialized_start=1884
+  _globals['_ENTITIESGROUP_ENTITIESENTRY']._serialized_end=1953
+  _globals['_DELETEDENTITIESGROUPS']._serialized_start=1955
+  _globals['_DELETEDENTITIESGROUPS']._serialized_end=2003
+  _globals['_ENTITIESGROUPS']._serialized_start=2006
+  _globals['_ENTITIESGROUPS']._serialized_end=2181
+  _globals['_ENTITIESGROUPS_ENTITIESGROUPSENTRY']._serialized_start=2099
+  _globals['_ENTITIESGROUPS_ENTITIESGROUPSENTRY']._serialized_end=2181
+  _globals['_ENTITYGROUPDUPLICATEINDEX']._serialized_start=2184
+  _globals['_ENTITYGROUPDUPLICATEINDEX']._serialized_end=2683
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYDUPLICATES']._serialized_start=2299
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYDUPLICATES']._serialized_end=2337
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES']._serialized_start=2340
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES']._serialized_end=2565
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES_ENTITIESENTRY']._serialized_start=2460
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITYGROUPDUPLICATES_ENTITIESENTRY']._serialized_end=2565
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITIESGROUPSENTRY']._serialized_start=2567
+  _globals['_ENTITYGROUPDUPLICATEINDEX_ENTITIESGROUPSENTRY']._serialized_end=2683
+  _globals['_VECTORSET']._serialized_start=2685
+  _globals['_VECTORSET']._serialized_end=2760
+  _globals['_VECTORSETS']._serialized_start=2763
+  _globals['_VECTORSETS']._serialized_end=2913
+  _globals['_VECTORSETS_VECTORSETSENTRY']._serialized_start=2839
+  _globals['_VECTORSETS_VECTORSETSENTRY']._serialized_end=2913
+  _globals['_VECTORSETCONFIG']._serialized_start=2916
+  _globals['_VECTORSETCONFIG']._serialized_end=3049
+  _globals['_KNOWLEDGEBOXVECTORSETSCONFIG']._serialized_start=3051
+  _globals['_KNOWLEDGEBOXVECTORSETSCONFIG']._serialized_end=3132
+  _globals['_TERMSYNONYMS']._serialized_start=3134
+  _globals['_TERMSYNONYMS']._serialized_end=3166
+  _globals['_SYNONYMS']._serialized_start=3169
+  _globals['_SYNONYMS']._serialized_end=3303
+  _globals['_SYNONYMS_TERMSENTRY']._serialized_start=3231
+  _globals['_SYNONYMS_TERMSENTRY']._serialized_end=3303
+  _globals['_SEMANTICMODELMETADATA']._serialized_start=3306
+  _globals['_SEMANTICMODELMETADATA']._serialized_end=3524
+  _globals['_KBCONFIGURATION']._serialized_start=3527
+  _globals['_KBCONFIGURATION']._serialized_end=3667
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,40 @@
 
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import nucliadb_protos.nodewriter_pb2
 import nucliadb_protos.utils_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
+from nucliadb_protos.nodewriter_pb2 import (
+    CREATION as CREATION,
+    DELETION as DELETION,
+    DENSE_F32 as DENSE_F32,
+    GarbageCollectorResponse as GarbageCollectorResponse,
+    IndexMessage as IndexMessage,
+    IndexMessageSource as IndexMessageSource,
+    MergeResponse as MergeResponse,
+    NewShardRequest as NewShardRequest,
+    NewVectorSetRequest as NewVectorSetRequest,
+    OpStatus as OpStatus,
+    PROCESSOR as PROCESSOR,
+    TypeMessage as TypeMessage,
+    VectorIndexConfig as VectorIndexConfig,
+    VectorType as VectorType,
+    WRITER as WRITER,
+)
 from nucliadb_protos.utils_pb2 import (
     COSINE as COSINE,
     DOT as DOT,
     EXPERIMENTAL as EXPERIMENTAL,
     ExtractedText as ExtractedText,
     Relation as Relation,
     RelationMetadata as RelationMetadata,
@@ -649,14 +667,62 @@
         vectorsets: collections.abc.Mapping[builtins.str, global___VectorSet] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["vectorsets", b"vectorsets"]) -> None: ...
 
 global___VectorSets = VectorSets
 
 @typing.final
+class VectorSetConfig(google.protobuf.message.Message):
+    """Configuration values for a vectorset"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VECTORSET_ID_FIELD_NUMBER: builtins.int
+    VECTORSET_INDEX_CONFIG_FIELD_NUMBER: builtins.int
+    MATRYOSHKA_DIMENSIONS_FIELD_NUMBER: builtins.int
+    vectorset_id: builtins.str
+    @property
+    def vectorset_index_config(self) -> nucliadb_protos.nodewriter_pb2.VectorIndexConfig: ...
+    @property
+    def matryoshka_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """list of possible subdivisions of the matryoshka embeddings (if the model
+        supports it)
+        """
+
+    def __init__(
+        self,
+        *,
+        vectorset_id: builtins.str = ...,
+        vectorset_index_config: nucliadb_protos.nodewriter_pb2.VectorIndexConfig | None = ...,
+        matryoshka_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing.Literal["vectorset_index_config", b"vectorset_index_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["matryoshka_dimensions", b"matryoshka_dimensions", "vectorset_id", b"vectorset_id", "vectorset_index_config", b"vectorset_index_config"]) -> None: ...
+
+global___VectorSetConfig = VectorSetConfig
+
+@typing.final
+class KnowledgeBoxVectorSetsConfig(google.protobuf.message.Message):
+    """KB vectorsets and their configuration"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VECTORSETS_FIELD_NUMBER: builtins.int
+    @property
+    def vectorsets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___VectorSetConfig]: ...
+    def __init__(
+        self,
+        *,
+        vectorsets: collections.abc.Iterable[global___VectorSetConfig] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["vectorsets", b"vectorsets"]) -> None: ...
+
+global___KnowledgeBoxVectorSetsConfig = KnowledgeBoxVectorSetsConfig
+
+@typing.final
 class TermSynonyms(google.protobuf.message.Message):
     """Synonyms of a Knowledge Box"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SYNONYMS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/resources_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from nucliadb_protos import knowledgebox_pb2 as nucliadb__protos_dot_knowledgebox__pb2
 try:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_utils__pb2
 except AttributeError:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.utils_pb2
+try:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_nodewriter__pb2
+except AttributeError:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.nodewriter_pb2
+try:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_noderesources__pb2
+except AttributeError:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.noderesources_pb2
+try:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_utils__pb2
+except AttributeError:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.utils_pb2
 from nucliadb_protos import resources_pb2 as nucliadb__protos_dot_resources__pb2
 try:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_resources__pb2.nucliadb__protos_dot_utils__pb2
 except AttributeError:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_resources__pb2.nucliadb_protos.utils_pb2
 from nucliadb_protos import writer_pb2 as nucliadb__protos_dot_writer__pb2
 try:
@@ -45,14 +57,26 @@
 except AttributeError:
   nucliadb__protos_dot_knowledgebox__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.knowledgebox_pb2
 try:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb__protos_dot_utils__pb2
 except AttributeError:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.utils_pb2
 try:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb__protos_dot_nodewriter__pb2
+except AttributeError:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.nodewriter_pb2
+try:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb__protos_dot_noderesources__pb2
+except AttributeError:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.noderesources_pb2
+try:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb__protos_dot_utils__pb2
+except AttributeError:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.utils_pb2
+try:
   nucliadb__protos_dot_audit__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb__protos_dot_audit__pb2
 except AttributeError:
   nucliadb__protos_dot_audit__pb2 = nucliadb__protos_dot_writer__pb2.nucliadb_protos.audit_pb2
 
 from nucliadb_protos.knowledgebox_pb2 import *
 from nucliadb_protos.resources_pb2 import *
 from nucliadb_protos.writer_pb2 import *
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,27 @@
     GCKnowledgeBoxResponse as GCKnowledgeBoxResponse,
     KBConfiguration as KBConfiguration,
     KnowledgeBoxConfig as KnowledgeBoxConfig,
     KnowledgeBoxID as KnowledgeBoxID,
     KnowledgeBoxNew as KnowledgeBoxNew,
     KnowledgeBoxResponseStatus as KnowledgeBoxResponseStatus,
     KnowledgeBoxUpdate as KnowledgeBoxUpdate,
+    KnowledgeBoxVectorSetsConfig as KnowledgeBoxVectorSetsConfig,
     Label as Label,
     LabelSet as LabelSet,
     Labels as Labels,
     NOTFOUND as NOTFOUND,
     NewKnowledgeBoxResponse as NewKnowledgeBoxResponse,
     OK as OK,
     SemanticModelMetadata as SemanticModelMetadata,
     Synonyms as Synonyms,
     TermSynonyms as TermSynonyms,
     UpdateKnowledgeBoxResponse as UpdateKnowledgeBoxResponse,
     VectorSet as VectorSet,
+    VectorSetConfig as VectorSetConfig,
     VectorSets as VectorSets,
 )
 from nucliadb_protos.resources_pb2 import (
     AllFieldIDs as AllFieldIDs,
     Answers as Answers,
     Basic as Basic,
     Block as Block,
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,27 @@
     GCKnowledgeBoxResponse as GCKnowledgeBoxResponse,
     KBConfiguration as KBConfiguration,
     KnowledgeBoxConfig as KnowledgeBoxConfig,
     KnowledgeBoxID as KnowledgeBoxID,
     KnowledgeBoxNew as KnowledgeBoxNew,
     KnowledgeBoxResponseStatus as KnowledgeBoxResponseStatus,
     KnowledgeBoxUpdate as KnowledgeBoxUpdate,
+    KnowledgeBoxVectorSetsConfig as KnowledgeBoxVectorSetsConfig,
     Label as Label,
     LabelSet as LabelSet,
     Labels as Labels,
     NOTFOUND as NOTFOUND,
     NewKnowledgeBoxResponse as NewKnowledgeBoxResponse,
     OK as OK,
     SemanticModelMetadata as SemanticModelMetadata,
     Synonyms as Synonyms,
     TermSynonyms as TermSynonyms,
     UpdateKnowledgeBoxResponse as UpdateKnowledgeBoxResponse,
     VectorSet as VectorSet,
+    VectorSetConfig as VectorSetConfig,
     VectorSets as VectorSets,
 )
 from nucliadb_protos.resources_pb2 import (
     AllFieldIDs as AllFieldIDs,
     Answers as Answers,
     Basic as Basic,
     Block as Block,
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/utils_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,26 @@
 except AttributeError:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_resources__pb2.nucliadb_protos.utils_pb2
 from nucliadb_protos import knowledgebox_pb2 as nucliadb__protos_dot_knowledgebox__pb2
 try:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_utils__pb2
 except AttributeError:
   nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.utils_pb2
+try:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_nodewriter__pb2
+except AttributeError:
+  nucliadb__protos_dot_nodewriter__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.nodewriter_pb2
+try:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_noderesources__pb2
+except AttributeError:
+  nucliadb__protos_dot_noderesources__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.noderesources_pb2
+try:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb__protos_dot_utils__pb2
+except AttributeError:
+  nucliadb__protos_dot_utils__pb2 = nucliadb__protos_dot_knowledgebox__pb2.nucliadb_protos.utils_pb2
 from nucliadb_protos import audit_pb2 as nucliadb__protos_dot_audit__pb2
 
 from nucliadb_protos.noderesources_pb2 import *
 from nucliadb_protos.resources_pb2 import *
 from nucliadb_protos.knowledgebox_pb2 import *
 from nucliadb_protos.audit_pb2 import *
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -103,4789 +103,4795 @@
 00000660: 426f 784e 6577 2c0a 2020 2020 4b6e 6f77  BoxNew,.    Know
 00000670: 6c65 6467 6542 6f78 5265 7370 6f6e 7365  ledgeBoxResponse
 00000680: 5374 6174 7573 2061 7320 4b6e 6f77 6c65  Status as Knowle
 00000690: 6467 6542 6f78 5265 7370 6f6e 7365 5374  dgeBoxResponseSt
 000006a0: 6174 7573 2c0a 2020 2020 4b6e 6f77 6c65  atus,.    Knowle
 000006b0: 6467 6542 6f78 5570 6461 7465 2061 7320  dgeBoxUpdate as 
 000006c0: 4b6e 6f77 6c65 6467 6542 6f78 5570 6461  KnowledgeBoxUpda
-000006d0: 7465 2c0a 2020 2020 4c61 6265 6c20 6173  te,.    Label as
-000006e0: 204c 6162 656c 2c0a 2020 2020 4c61 6265   Label,.    Labe
-000006f0: 6c53 6574 2061 7320 4c61 6265 6c53 6574  lSet as LabelSet
-00000700: 2c0a 2020 2020 4c61 6265 6c73 2061 7320  ,.    Labels as 
-00000710: 4c61 6265 6c73 2c0a 2020 2020 4e4f 5446  Labels,.    NOTF
-00000720: 4f55 4e44 2061 7320 4e4f 5446 4f55 4e44  OUND as NOTFOUND
-00000730: 2c0a 2020 2020 4e65 774b 6e6f 776c 6564  ,.    NewKnowled
-00000740: 6765 426f 7852 6573 706f 6e73 6520 6173  geBoxResponse as
-00000750: 204e 6577 4b6e 6f77 6c65 6467 6542 6f78   NewKnowledgeBox
-00000760: 5265 7370 6f6e 7365 2c0a 2020 2020 4f4b  Response,.    OK
-00000770: 2061 7320 4f4b 2c0a 2020 2020 5365 6d61   as OK,.    Sema
-00000780: 6e74 6963 4d6f 6465 6c4d 6574 6164 6174  nticModelMetadat
-00000790: 6120 6173 2053 656d 616e 7469 634d 6f64  a as SemanticMod
-000007a0: 656c 4d65 7461 6461 7461 2c0a 2020 2020  elMetadata,.    
-000007b0: 5379 6e6f 6e79 6d73 2061 7320 5379 6e6f  Synonyms as Syno
-000007c0: 6e79 6d73 2c0a 2020 2020 5465 726d 5379  nyms,.    TermSy
-000007d0: 6e6f 6e79 6d73 2061 7320 5465 726d 5379  nonyms as TermSy
-000007e0: 6e6f 6e79 6d73 2c0a 2020 2020 5570 6461  nonyms,.    Upda
-000007f0: 7465 4b6e 6f77 6c65 6467 6542 6f78 5265  teKnowledgeBoxRe
-00000800: 7370 6f6e 7365 2061 7320 5570 6461 7465  sponse as Update
-00000810: 4b6e 6f77 6c65 6467 6542 6f78 5265 7370  KnowledgeBoxResp
-00000820: 6f6e 7365 2c0a 2020 2020 5665 6374 6f72  onse,.    Vector
-00000830: 5365 7420 6173 2056 6563 746f 7253 6574  Set as VectorSet
-00000840: 2c0a 2020 2020 5665 6374 6f72 5365 7473  ,.    VectorSets
-00000850: 2061 7320 5665 6374 6f72 5365 7473 2c0a   as VectorSets,.
-00000860: 290a 6672 6f6d 206e 7563 6c69 6164 625f  ).from nucliadb_
-00000870: 7072 6f74 6f73 2e6e 6f64 6572 6573 6f75  protos.noderesou
-00000880: 7263 6573 5f70 6232 2069 6d70 6f72 7420  rces_pb2 import 
-00000890: 280a 2020 2020 456d 7074 7951 7565 7279  (.    EmptyQuery
-000008a0: 2061 7320 456d 7074 7951 7565 7279 2c0a   as EmptyQuery,.
-000008b0: 2020 2020 456d 7074 7952 6573 706f 6e73      EmptyRespons
-000008c0: 6520 6173 2045 6d70 7479 5265 7370 6f6e  e as EmptyRespon
-000008d0: 7365 2c0a 2020 2020 496e 6465 784d 6574  se,.    IndexMet
-000008e0: 6164 6174 6120 6173 2049 6e64 6578 4d65  adata as IndexMe
-000008f0: 7461 6461 7461 2c0a 2020 2020 496e 6465  tadata,.    Inde
-00000900: 7850 6172 6167 7261 7068 2061 7320 496e  xParagraph as In
-00000910: 6465 7850 6172 6167 7261 7068 2c0a 2020  dexParagraph,.  
-00000920: 2020 496e 6465 7850 6172 6167 7261 7068    IndexParagraph
-00000930: 7320 6173 2049 6e64 6578 5061 7261 6772  s as IndexParagr
-00000940: 6170 6873 2c0a 2020 2020 4e6f 6465 4d65  aphs,.    NodeMe
-00000950: 7461 6461 7461 2061 7320 4e6f 6465 4d65  tadata as NodeMe
-00000960: 7461 6461 7461 2c0a 2020 2020 5061 7261  tadata,.    Para
-00000970: 6772 6170 684d 6574 6164 6174 6120 6173  graphMetadata as
-00000980: 2050 6172 6167 7261 7068 4d65 7461 6461   ParagraphMetada
-00000990: 7461 2c0a 2020 2020 506f 7369 7469 6f6e  ta,.    Position
-000009a0: 2061 7320 506f 7369 7469 6f6e 2c0a 2020   as Position,.  
-000009b0: 2020 5265 7072 6573 656e 7461 7469 6f6e    Representation
-000009c0: 2061 7320 5265 7072 6573 656e 7461 7469   as Representati
-000009d0: 6f6e 2c0a 2020 2020 5265 736f 7572 6365  on,.    Resource
-000009e0: 2061 7320 5265 736f 7572 6365 2c0a 2020   as Resource,.  
-000009f0: 2020 5265 736f 7572 6365 4944 2061 7320    ResourceID as 
-00000a00: 5265 736f 7572 6365 4944 2c0a 2020 2020  ResourceID,.    
-00000a10: 5365 6e74 656e 6365 4d65 7461 6461 7461  SentenceMetadata
-00000a20: 2061 7320 5365 6e74 656e 6365 4d65 7461   as SentenceMeta
-00000a30: 6461 7461 2c0a 2020 2020 5368 6172 6420  data,.    Shard 
-00000a40: 6173 2053 6861 7264 2c0a 2020 2020 5368  as Shard,.    Sh
-00000a50: 6172 6443 7265 6174 6564 2061 7320 5368  ardCreated as Sh
-00000a60: 6172 6443 7265 6174 6564 2c0a 2020 2020  ardCreated,.    
-00000a70: 5368 6172 6449 6420 6173 2053 6861 7264  ShardId as Shard
-00000a80: 4964 2c0a 2020 2020 5368 6172 6449 6473  Id,.    ShardIds
-00000a90: 2061 7320 5368 6172 6449 6473 2c0a 2020   as ShardIds,.  
-00000aa0: 2020 5368 6172 644d 6574 6164 6174 6120    ShardMetadata 
-00000ab0: 6173 2053 6861 7264 4d65 7461 6461 7461  as ShardMetadata
-00000ac0: 2c0a 2020 2020 5465 7874 496e 666f 726d  ,.    TextInform
-00000ad0: 6174 696f 6e20 6173 2054 6578 7449 6e66  ation as TextInf
-00000ae0: 6f72 6d61 7469 6f6e 2c0a 2020 2020 5665  ormation,.    Ve
-00000af0: 6374 6f72 5365 6e74 656e 6365 2061 7320  ctorSentence as 
-00000b00: 5665 6374 6f72 5365 6e74 656e 6365 2c0a  VectorSentence,.
-00000b10: 2020 2020 5665 6374 6f72 5365 7449 4420      VectorSetID 
-00000b20: 6173 2056 6563 746f 7253 6574 4944 2c0a  as VectorSetID,.
-00000b30: 2020 2020 5665 6374 6f72 5365 744c 6973      VectorSetLis
-00000b40: 7420 6173 2056 6563 746f 7253 6574 4c69  t as VectorSetLi
-00000b50: 7374 2c0a 2020 2020 5665 6374 6f72 7365  st,.    Vectorse
-00000b60: 7453 656e 7465 6e63 6573 2061 7320 5665  tSentences as Ve
-00000b70: 6374 6f72 7365 7453 656e 7465 6e63 6573  ctorsetSentences
-00000b80: 2c0a 290a 6672 6f6d 206e 7563 6c69 6164  ,.).from nucliad
-00000b90: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00000ba0: 6573 5f70 6232 2069 6d70 6f72 7420 280a  es_pb2 import (.
-00000bb0: 2020 2020 416c 6c46 6965 6c64 4944 7320      AllFieldIDs 
-00000bc0: 6173 2041 6c6c 4669 656c 6449 4473 2c0a  as AllFieldIDs,.
-00000bd0: 2020 2020 416e 7377 6572 7320 6173 2041      Answers as A
-00000be0: 6e73 7765 7273 2c0a 2020 2020 4261 7369  nswers,.    Basi
-00000bf0: 6320 6173 2042 6173 6963 2c0a 2020 2020  c as Basic,.    
-00000c00: 426c 6f63 6b20 6173 2042 6c6f 636b 2c0a  Block as Block,.
-00000c10: 2020 2020 434f 4e56 4552 5341 5449 4f4e      CONVERSATION
-00000c20: 2061 7320 434f 4e56 4552 5341 5449 4f4e   as CONVERSATION
-00000c30: 2c0a 2020 2020 436c 6173 7369 6669 6361  ,.    Classifica
-00000c40: 7469 6f6e 2061 7320 436c 6173 7369 6669  tion as Classifi
-00000c50: 6361 7469 6f6e 2c0a 2020 2020 436c 6f75  cation,.    Clou
-00000c60: 6446 696c 6520 6173 2043 6c6f 7564 4669  dFile as CloudFi
-00000c70: 6c65 2c0a 2020 2020 436f 6d70 7574 6564  le,.    Computed
-00000c80: 4d65 7461 6461 7461 2061 7320 436f 6d70  Metadata as Comp
-00000c90: 7574 6564 4d65 7461 6461 7461 2c0a 2020  utedMetadata,.  
-00000ca0: 2020 436f 6e76 6572 7361 7469 6f6e 2061    Conversation a
-00000cb0: 7320 436f 6e76 6572 7361 7469 6f6e 2c0a  s Conversation,.
-00000cc0: 2020 2020 4441 5445 5449 4d45 2061 7320      DATETIME as 
-00000cd0: 4441 5445 5449 4d45 2c0a 2020 2020 456e  DATETIME,.    En
-00000ce0: 7469 7479 2061 7320 456e 7469 7479 2c0a  tity as Entity,.
-00000cf0: 2020 2020 4578 7472 6120 6173 2045 7874      Extra as Ext
-00000d00: 7261 2c0a 2020 2020 4578 7472 6163 7465  ra,.    Extracte
-00000d10: 6454 6578 7457 7261 7070 6572 2061 7320  dTextWrapper as 
-00000d20: 4578 7472 6163 7465 6454 6578 7457 7261  ExtractedTextWra
-00000d30: 7070 6572 2c0a 2020 2020 4578 7472 6163  pper,.    Extrac
-00000d40: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
-00000d50: 7220 6173 2045 7874 7261 6374 6564 5665  r as ExtractedVe
-00000d60: 6374 6f72 7357 7261 7070 6572 2c0a 2020  ctorsWrapper,.  
-00000d70: 2020 4649 4c45 2061 7320 4649 4c45 2c0a    FILE as FILE,.
-00000d80: 2020 2020 4669 656c 6443 6c61 7373 6966      FieldClassif
-00000d90: 6963 6174 696f 6e73 2061 7320 4669 656c  ications as Fiel
-00000da0: 6443 6c61 7373 6966 6963 6174 696f 6e73  dClassifications
-00000db0: 2c0a 2020 2020 4669 656c 6443 6f6d 7075  ,.    FieldCompu
-00000dc0: 7465 644d 6574 6164 6174 6120 6173 2046  tedMetadata as F
-00000dd0: 6965 6c64 436f 6d70 7574 6564 4d65 7461  ieldComputedMeta
-00000de0: 6461 7461 2c0a 2020 2020 4669 656c 6443  data,.    FieldC
-00000df0: 6f6d 7075 7465 644d 6574 6164 6174 6157  omputedMetadataW
-00000e00: 7261 7070 6572 2061 7320 4669 656c 6443  rapper as FieldC
-00000e10: 6f6d 7075 7465 644d 6574 6164 6174 6157  omputedMetadataW
-00000e20: 7261 7070 6572 2c0a 2020 2020 4669 656c  rapper,.    Fiel
-00000e30: 6443 6f6e 7665 7273 6174 696f 6e20 6173  dConversation as
-00000e40: 2046 6965 6c64 436f 6e76 6572 7361 7469   FieldConversati
-00000e50: 6f6e 2c0a 2020 2020 4669 656c 6444 6174  on,.    FieldDat
-00000e60: 6574 696d 6520 6173 2046 6965 6c64 4461  etime as FieldDa
-00000e70: 7465 7469 6d65 2c0a 2020 2020 4669 656c  tetime,.    Fiel
-00000e80: 6446 696c 6520 6173 2046 6965 6c64 4669  dFile as FieldFi
-00000e90: 6c65 2c0a 2020 2020 4669 656c 6449 4420  le,.    FieldID 
-00000ea0: 6173 2046 6965 6c64 4944 2c0a 2020 2020  as FieldID,.    
-00000eb0: 4669 656c 644b 6579 776f 7264 7365 7420  FieldKeywordset 
-00000ec0: 6173 2046 6965 6c64 4b65 7977 6f72 6473  as FieldKeywords
-00000ed0: 6574 2c0a 2020 2020 4669 656c 644c 6172  et,.    FieldLar
-00000ee0: 6765 4d65 7461 6461 7461 2061 7320 4669  geMetadata as Fi
-00000ef0: 656c 644c 6172 6765 4d65 7461 6461 7461  eldLargeMetadata
-00000f00: 2c0a 2020 2020 4669 656c 644c 6179 6f75  ,.    FieldLayou
-00000f10: 7420 6173 2046 6965 6c64 4c61 796f 7574  t as FieldLayout
-00000f20: 2c0a 2020 2020 4669 656c 644c 696e 6b20  ,.    FieldLink 
-00000f30: 6173 2046 6965 6c64 4c69 6e6b 2c0a 2020  as FieldLink,.  
-00000f40: 2020 4669 656c 644d 6574 6164 6174 6120    FieldMetadata 
-00000f50: 6173 2046 6965 6c64 4d65 7461 6461 7461  as FieldMetadata
-00000f60: 2c0a 2020 2020 4669 656c 6451 7565 7374  ,.    FieldQuest
-00000f70: 696f 6e41 6e73 7765 7257 7261 7070 6572  ionAnswerWrapper
-00000f80: 2061 7320 4669 656c 6451 7565 7374 696f   as FieldQuestio
-00000f90: 6e41 6e73 7765 7257 7261 7070 6572 2c0a  nAnswerWrapper,.
-00000fa0: 2020 2020 4669 656c 6454 6578 7420 6173      FieldText as
-00000fb0: 2046 6965 6c64 5465 7874 2c0a 2020 2020   FieldText,.    
-00000fc0: 4669 656c 6454 7970 6520 6173 2046 6965  FieldType as Fie
-00000fd0: 6c64 5479 7065 2c0a 2020 2020 4669 6c65  ldType,.    File
-00000fe0: 4578 7472 6163 7465 6444 6174 6120 6173  ExtractedData as
-00000ff0: 2046 696c 6545 7874 7261 6374 6564 4461   FileExtractedDa
-00001000: 7461 2c0a 2020 2020 4669 6c65 5061 6765  ta,.    FilePage
-00001010: 7320 6173 2046 696c 6550 6167 6573 2c0a  s as FilePages,.
-00001020: 2020 2020 4745 4e45 5249 4320 6173 2047      GENERIC as G
-00001030: 454e 4552 4943 2c0a 2020 2020 4b45 5957  ENERIC,.    KEYW
-00001040: 4f52 4453 4554 2061 7320 4b45 5957 4f52  ORDSET as KEYWOR
-00001050: 4453 4554 2c0a 2020 2020 4b65 7977 6f72  DSET,.    Keywor
-00001060: 6420 6173 204b 6579 776f 7264 2c0a 2020  d as Keyword,.  
-00001070: 2020 4c41 594f 5554 2061 7320 4c41 594f    LAYOUT as LAYO
-00001080: 5554 2c0a 2020 2020 4c49 4e4b 2061 7320  UT,.    LINK as 
-00001090: 4c49 4e4b 2c0a 2020 2020 4c61 7267 6543  LINK,.    LargeC
-000010a0: 6f6d 7075 7465 644d 6574 6164 6174 6120  omputedMetadata 
-000010b0: 6173 204c 6172 6765 436f 6d70 7574 6564  as LargeComputed
-000010c0: 4d65 7461 6461 7461 2c0a 2020 2020 4c61  Metadata,.    La
-000010d0: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
-000010e0: 6174 6157 7261 7070 6572 2061 7320 4c61  ataWrapper as La
-000010f0: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
-00001100: 6174 6157 7261 7070 6572 2c0a 2020 2020  ataWrapper,.    
-00001110: 4c61 796f 7574 436f 6e74 656e 7420 6173  LayoutContent as
-00001120: 204c 6179 6f75 7443 6f6e 7465 6e74 2c0a   LayoutContent,.
-00001130: 2020 2020 4c69 6e6b 4578 7472 6163 7465      LinkExtracte
-00001140: 6444 6174 6120 6173 204c 696e 6b45 7874  dData as LinkExt
-00001150: 7261 6374 6564 4461 7461 2c0a 2020 2020  ractedData,.    
-00001160: 4d65 7373 6167 6520 6173 204d 6573 7361  Message as Messa
-00001170: 6765 2c0a 2020 2020 4d65 7373 6167 6543  ge,.    MessageC
-00001180: 6f6e 7465 6e74 2061 7320 4d65 7373 6167  ontent as Messag
-00001190: 6543 6f6e 7465 6e74 2c0a 2020 2020 4d65  eContent,.    Me
-000011a0: 7461 6461 7461 2061 7320 4d65 7461 6461  tadata as Metada
-000011b0: 7461 2c0a 2020 2020 4e65 7374 6564 4c69  ta,.    NestedLi
-000011c0: 7374 506f 7369 7469 6f6e 2061 7320 4e65  stPosition as Ne
-000011d0: 7374 6564 4c69 7374 506f 7369 7469 6f6e  stedListPosition
-000011e0: 2c0a 2020 2020 4e65 7374 6564 506f 7369  ,.    NestedPosi
-000011f0: 7469 6f6e 2061 7320 4e65 7374 6564 506f  tion as NestedPo
-00001200: 7369 7469 6f6e 2c0a 2020 2020 4f72 6967  sition,.    Orig
-00001210: 696e 2061 7320 4f72 6967 696e 2c0a 2020  in as Origin,.  
-00001220: 2020 5061 6765 496e 666f 726d 6174 696f    PageInformatio
-00001230: 6e20 6173 2050 6167 6549 6e66 6f72 6d61  n as PageInforma
-00001240: 7469 6f6e 2c0a 2020 2020 5061 6765 506f  tion,.    PagePo
-00001250: 7369 7469 6f6e 7320 6173 2050 6167 6550  sitions as PageP
-00001260: 6f73 6974 696f 6e73 2c0a 2020 2020 5061  ositions,.    Pa
-00001270: 6765 5365 6c65 6374 696f 6e73 2061 7320  geSelections as 
-00001280: 5061 6765 5365 6c65 6374 696f 6e73 2c0a  PageSelections,.
-00001290: 2020 2020 5061 6765 5374 7275 6374 7572      PageStructur
-000012a0: 6520 6173 2050 6167 6553 7472 7563 7475  e as PageStructu
-000012b0: 7265 2c0a 2020 2020 5061 6765 5374 7275  re,.    PageStru
-000012c0: 6374 7572 6550 6167 6520 6173 2050 6167  cturePage as Pag
-000012d0: 6553 7472 7563 7475 7265 5061 6765 2c0a  eStructurePage,.
-000012e0: 2020 2020 5061 6765 5374 7275 6374 7572      PageStructur
-000012f0: 6554 6f6b 656e 2061 7320 5061 6765 5374  eToken as PageSt
-00001300: 7275 6374 7572 6554 6f6b 656e 2c0a 2020  ructureToken,.  
-00001310: 2020 5061 7261 6772 6170 6820 6173 2050    Paragraph as P
-00001320: 6172 6167 7261 7068 2c0a 2020 2020 5061  aragraph,.    Pa
-00001330: 7261 6772 6170 6841 6e6e 6f74 6174 696f  ragraphAnnotatio
-00001340: 6e20 6173 2050 6172 6167 7261 7068 416e  n as ParagraphAn
-00001350: 6e6f 7461 7469 6f6e 2c0a 2020 2020 5061  notation,.    Pa
-00001360: 7261 6772 6170 6852 656c 6174 696f 6e73  ragraphRelations
-00001370: 2061 7320 5061 7261 6772 6170 6852 656c   as ParagraphRel
-00001380: 6174 696f 6e73 2c0a 2020 2020 506f 7369  ations,.    Posi
-00001390: 7469 6f6e 2061 7320 506f 7369 7469 6f6e  tion as Position
-000013a0: 2c0a 2020 2020 506f 7369 7469 6f6e 7320  ,.    Positions 
-000013b0: 6173 2050 6f73 6974 696f 6e73 2c0a 2020  as Positions,.  
-000013c0: 2020 5175 6573 7469 6f6e 2061 7320 5175    Question as Qu
-000013d0: 6573 7469 6f6e 2c0a 2020 2020 5175 6573  estion,.    Ques
-000013e0: 7469 6f6e 416e 7377 6572 2061 7320 5175  tionAnswer as Qu
-000013f0: 6573 7469 6f6e 416e 7377 6572 2c0a 2020  estionAnswer,.  
-00001400: 2020 5175 6573 7469 6f6e 416e 7377 6572    QuestionAnswer
-00001410: 416e 6e6f 7461 7469 6f6e 2061 7320 5175  Annotation as Qu
-00001420: 6573 7469 6f6e 416e 7377 6572 416e 6e6f  estionAnswerAnno
-00001430: 7461 7469 6f6e 2c0a 2020 2020 5175 6573  tation,.    Ques
-00001440: 7469 6f6e 416e 7377 6572 7320 6173 2051  tionAnswers as Q
-00001450: 7565 7374 696f 6e41 6e73 7765 7273 2c0a  uestionAnswers,.
-00001460: 2020 2020 5265 6c61 7469 6f6e 7320 6173      Relations as
-00001470: 2052 656c 6174 696f 6e73 2c0a 2020 2020   Relations,.    
-00001480: 5265 7072 6573 656e 7461 7469 6f6e 2061  Representation a
-00001490: 7320 5265 7072 6573 656e 7461 7469 6f6e  s Representation
-000014a0: 2c0a 2020 2020 526f 7773 5072 6576 6965  ,.    RowsPrevie
-000014b0: 7720 6173 2052 6f77 7350 7265 7669 6577  w as RowsPreview
-000014c0: 2c0a 2020 2020 5365 6e74 656e 6365 2061  ,.    Sentence a
-000014d0: 7320 5365 6e74 656e 6365 2c0a 2020 2020  s Sentence,.    
-000014e0: 5445 5854 2061 7320 5445 5854 2c0a 2020  TEXT as TEXT,.  
-000014f0: 2020 546f 6b65 6e53 706c 6974 2061 7320    TokenSplit as 
-00001500: 546f 6b65 6e53 706c 6974 2c0a 2020 2020  TokenSplit,.    
-00001510: 5573 6572 4669 656c 644d 6574 6164 6174  UserFieldMetadat
-00001520: 6120 6173 2055 7365 7246 6965 6c64 4d65  a as UserFieldMe
-00001530: 7461 6461 7461 2c0a 2020 2020 5573 6572  tadata,.    User
-00001540: 4d65 7461 6461 7461 2061 7320 5573 6572  Metadata as User
-00001550: 4d65 7461 6461 7461 2c0a 2020 2020 5573  Metadata,.    Us
-00001560: 6572 5665 6374 6f72 7357 7261 7070 6572  erVectorsWrapper
-00001570: 2061 7320 5573 6572 5665 6374 6f72 7357   as UserVectorsW
-00001580: 7261 7070 6572 2c0a 2020 2020 5669 7375  rapper,.    Visu
-00001590: 616c 5365 6c65 6374 696f 6e20 6173 2056  alSelection as V
-000015a0: 6973 7561 6c53 656c 6563 7469 6f6e 2c0a  isualSelection,.
-000015b0: 290a 0a44 4553 4352 4950 544f 523a 2067  )..DESCRIPTOR: g
-000015c0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-000015d0: 6573 6372 6970 746f 722e 4669 6c65 4465  escriptor.FileDe
-000015e0: 7363 7269 7074 6f72 0a0a 636c 6173 7320  scriptor..class 
-000015f0: 5f4e 6f74 6966 6963 6174 696f 6e53 6f75  _NotificationSou
-00001600: 7263 653a 0a20 2020 2056 616c 7565 5479  rce:.    ValueTy
-00001610: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
-00001620: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
-00001630: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
-00001640: 2020 2056 3a20 7479 7069 6e67 5f65 7874     V: typing_ext
-00001650: 656e 7369 6f6e 732e 5479 7065 416c 6961  ensions.TypeAlia
-00001660: 7320 3d20 5661 6c75 6554 7970 650a 0a63  s = ValueType..c
-00001670: 6c61 7373 205f 4e6f 7469 6669 6361 7469  lass _Notificati
-00001680: 6f6e 536f 7572 6365 456e 756d 5479 7065  onSourceEnumType
-00001690: 5772 6170 7065 7228 676f 6f67 6c65 2e70  Wrapper(google.p
-000016a0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
-000016b0: 2e65 6e75 6d5f 7479 7065 5f77 7261 7070  .enum_type_wrapp
-000016c0: 6572 2e5f 456e 756d 5479 7065 5772 6170  er._EnumTypeWrap
-000016d0: 7065 725b 5f4e 6f74 6966 6963 6174 696f  per[_Notificatio
-000016e0: 6e53 6f75 7263 652e 5661 6c75 6554 7970  nSource.ValueTyp
-000016f0: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
-00001700: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-00001710: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00001720: 6275 662e 6465 7363 7269 7074 6f72 2e45  buf.descriptor.E
-00001730: 6e75 6d44 6573 6372 6970 746f 720a 2020  numDescriptor.  
-00001740: 2020 554e 5345 543a 205f 4e6f 7469 6669    UNSET: _Notifi
-00001750: 6361 7469 6f6e 536f 7572 6365 2e56 616c  cationSource.Val
-00001760: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
-00001770: 5752 4954 4552 3a20 5f4e 6f74 6966 6963  WRITER: _Notific
-00001780: 6174 696f 6e53 6f75 7263 652e 5661 6c75  ationSource.Valu
-00001790: 6554 7970 6520 2023 2031 0a20 2020 2050  eType  # 1.    P
-000017a0: 524f 4345 5353 4f52 3a20 5f4e 6f74 6966  ROCESSOR: _Notif
-000017b0: 6963 6174 696f 6e53 6f75 7263 652e 5661  icationSource.Va
-000017c0: 6c75 6554 7970 6520 2023 2032 0a0a 636c  lueType  # 2..cl
-000017d0: 6173 7320 4e6f 7469 6669 6361 7469 6f6e  ass Notification
-000017e0: 536f 7572 6365 285f 4e6f 7469 6669 6361  Source(_Notifica
-000017f0: 7469 6f6e 536f 7572 6365 2c20 6d65 7461  tionSource, meta
-00001800: 636c 6173 733d 5f4e 6f74 6966 6963 6174  class=_Notificat
-00001810: 696f 6e53 6f75 7263 6545 6e75 6d54 7970  ionSourceEnumTyp
-00001820: 6557 7261 7070 6572 293a 202e 2e2e 0a0a  eWrapper): .....
-00001830: 554e 5345 543a 204e 6f74 6966 6963 6174  UNSET: Notificat
-00001840: 696f 6e53 6f75 7263 652e 5661 6c75 6554  ionSource.ValueT
-00001850: 7970 6520 2023 2030 0a57 5249 5445 523a  ype  # 0.WRITER:
-00001860: 204e 6f74 6966 6963 6174 696f 6e53 6f75   NotificationSou
-00001870: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
-00001880: 2031 0a50 524f 4345 5353 4f52 3a20 4e6f   1.PROCESSOR: No
-00001890: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
-000018a0: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-000018b0: 676c 6f62 616c 5f5f 5f4e 6f74 6966 6963  global___Notific
-000018c0: 6174 696f 6e53 6f75 7263 6520 3d20 4e6f  ationSource = No
-000018d0: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
-000018e0: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-000018f0: 636c 6173 7320 4175 6469 7428 676f 6f67  class Audit(goog
-00001900: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-00001910: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-00001920: 2020 2222 2257 6520 7265 6365 6976 6520    """We receive 
-00001930: 7468 6973 2069 6e66 6f72 6d61 7469 6f6e  this information
-00001940: 2074 6872 6f77 2061 6e20 7374 7265 616d   throw an stream
-00001950: 2073 7973 7465 6d22 2222 0a0a 2020 2020   system"""..    
-00001960: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00001970: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00001980: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00001990: 720a 0a20 2020 2063 6c61 7373 205f 536f  r..    class _So
-000019a0: 7572 6365 3a0a 2020 2020 2020 2020 5661  urce:.        Va
-000019b0: 6c75 6554 7970 6520 3d20 7479 7069 6e67  lueType = typing
-000019c0: 2e4e 6577 5479 7065 2822 5661 6c75 6554  .NewType("ValueT
-000019d0: 7970 6522 2c20 6275 696c 7469 6e73 2e69  ype", builtins.i
-000019e0: 6e74 290a 2020 2020 2020 2020 563a 2074  nt).        V: t
-000019f0: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
-00001a00: 2e54 7970 6541 6c69 6173 203d 2056 616c  .TypeAlias = Val
-00001a10: 7565 5479 7065 0a0a 2020 2020 636c 6173  ueType..    clas
-00001a20: 7320 5f53 6f75 7263 6545 6e75 6d54 7970  s _SourceEnumTyp
-00001a30: 6557 7261 7070 6572 2867 6f6f 676c 652e  eWrapper(google.
-00001a40: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
-00001a50: 6c2e 656e 756d 5f74 7970 655f 7772 6170  l.enum_type_wrap
-00001a60: 7065 722e 5f45 6e75 6d54 7970 6557 7261  per._EnumTypeWra
-00001a70: 7070 6572 5b41 7564 6974 2e5f 536f 7572  pper[Audit._Sour
-00001a80: 6365 2e56 616c 7565 5479 7065 5d2c 2062  ce.ValueType], b
-00001a90: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
-00001aa0: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
-00001ab0: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-00001ac0: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
-00001ad0: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
-00001ae0: 2020 2020 2048 5454 503a 2041 7564 6974       HTTP: Audit
-00001af0: 2e5f 536f 7572 6365 2e56 616c 7565 5479  ._Source.ValueTy
-00001b00: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
-00001b10: 4441 5348 424f 4152 443a 2041 7564 6974  DASHBOARD: Audit
-00001b20: 2e5f 536f 7572 6365 2e56 616c 7565 5479  ._Source.ValueTy
-00001b30: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
-00001b40: 4445 534b 544f 503a 2041 7564 6974 2e5f  DESKTOP: Audit._
-00001b50: 536f 7572 6365 2e56 616c 7565 5479 7065  Source.ValueType
-00001b60: 2020 2320 320a 0a20 2020 2063 6c61 7373    # 2..    class
-00001b70: 2053 6f75 7263 6528 5f53 6f75 7263 652c   Source(_Source,
-00001b80: 206d 6574 6163 6c61 7373 3d5f 536f 7572   metaclass=_Sour
-00001b90: 6365 456e 756d 5479 7065 5772 6170 7065  ceEnumTypeWrappe
-00001ba0: 7229 3a20 2e2e 2e0a 2020 2020 4854 5450  r): ....    HTTP
-00001bb0: 3a20 4175 6469 742e 536f 7572 6365 2e56  : Audit.Source.V
-00001bc0: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
-00001bd0: 2020 4441 5348 424f 4152 443a 2041 7564    DASHBOARD: Aud
-00001be0: 6974 2e53 6f75 7263 652e 5661 6c75 6554  it.Source.ValueT
-00001bf0: 7970 6520 2023 2031 0a20 2020 2044 4553  ype  # 1.    DES
-00001c00: 4b54 4f50 3a20 4175 6469 742e 536f 7572  KTOP: Audit.Sour
-00001c10: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
-00001c20: 320a 0a20 2020 2055 5345 525f 4649 454c  2..    USER_FIEL
-00001c30: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00001c40: 6e73 2e69 6e74 0a20 2020 2057 4845 4e5f  ns.int.    WHEN_
-00001c50: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00001c60: 696c 7469 6e73 2e69 6e74 0a20 2020 204f  iltins.int.    O
-00001c70: 5249 4749 4e5f 4649 454c 445f 4e55 4d42  RIGIN_FIELD_NUMB
-00001c80: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00001c90: 0a20 2020 2053 4f55 5243 455f 4649 454c  .    SOURCE_FIEL
-00001ca0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00001cb0: 6e73 2e69 6e74 0a20 2020 204b 4249 445f  ns.int.    KBID_
-00001cc0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00001cd0: 696c 7469 6e73 2e69 6e74 0a20 2020 2055  iltins.int.    U
-00001ce0: 5549 445f 4649 454c 445f 4e55 4d42 4552  UID_FIELD_NUMBER
-00001cf0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00001d00: 2020 204d 4553 5341 4745 5f53 4f55 5243     MESSAGE_SOURC
-00001d10: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
-00001d20: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00001d30: 2046 4945 4c44 5f4d 4554 4144 4154 415f   FIELD_METADATA_
-00001d40: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00001d50: 696c 7469 6e73 2e69 6e74 0a20 2020 2041  iltins.int.    A
-00001d60: 5544 4954 5f46 4945 4c44 535f 4649 454c  UDIT_FIELDS_FIEL
-00001d70: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00001d80: 6e73 2e69 6e74 0a20 2020 2075 7365 723a  ns.int.    user:
-00001d90: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00001da0: 2020 6f72 6967 696e 3a20 6275 696c 7469    origin: builti
-00001db0: 6e73 2e73 7472 0a20 2020 2073 6f75 7263  ns.str.    sourc
-00001dc0: 653a 2067 6c6f 6261 6c5f 5f5f 4175 6469  e: global___Audi
-00001dd0: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
-00001de0: 7065 0a20 2020 206b 6269 643a 2062 7569  pe.    kbid: bui
-00001df0: 6c74 696e 732e 7374 720a 2020 2020 7575  ltins.str.    uu
-00001e00: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
-00001e10: 0a20 2020 206d 6573 7361 6765 5f73 6f75  .    message_sou
-00001e20: 7263 653a 2067 6c6f 6261 6c5f 5f5f 4272  rce: global___Br
-00001e30: 6f6b 6572 4d65 7373 6167 652e 4d65 7373  okerMessage.Mess
-00001e40: 6167 6553 6f75 7263 652e 5661 6c75 6554  ageSource.ValueT
-00001e50: 7970 650a 2020 2020 4070 726f 7065 7274  ype.    @propert
-00001e60: 790a 2020 2020 6465 6620 7768 656e 2873  y.    def when(s
-00001e70: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
-00001e80: 726f 746f 6275 662e 7469 6d65 7374 616d  rotobuf.timestam
-00001e90: 705f 7062 322e 5469 6d65 7374 616d 703a  p_pb2.Timestamp:
-00001ea0: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
-00001eb0: 7479 0a20 2020 2064 6566 2066 6965 6c64  ty.    def field
-00001ec0: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
-00001ed0: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
-00001ee0: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
-00001ef0: 6169 6e65 7273 2e52 6570 6561 7465 6443  ainers.RepeatedC
-00001f00: 6f6d 706f 7369 7465 4669 656c 6443 6f6e  ompositeFieldCon
-00001f10: 7461 696e 6572 5b6e 7563 6c69 6164 625f  tainer[nucliadb_
-00001f20: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00001f30: 5f70 6232 2e46 6965 6c64 4944 5d3a 202e  _pb2.FieldID]: .
-00001f40: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00001f50: 0a20 2020 2064 6566 2061 7564 6974 5f66  .    def audit_f
-00001f60: 6965 6c64 7328 7365 6c66 2920 2d3e 2067  ields(self) -> g
-00001f70: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
-00001f80: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
-00001f90: 7273 2e52 6570 6561 7465 6443 6f6d 706f  rs.RepeatedCompo
-00001fa0: 7369 7465 4669 656c 6443 6f6e 7461 696e  siteFieldContain
-00001fb0: 6572 5b6e 7563 6c69 6164 625f 7072 6f74  er[nucliadb_prot
-00001fc0: 6f73 2e61 7564 6974 5f70 6232 2e41 7564  os.audit_pb2.Aud
-00001fd0: 6974 4669 656c 645d 3a20 2e2e 2e0a 2020  itField]: ....  
-00001fe0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00001ff0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00002000: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00002010: 2075 7365 723a 2062 7569 6c74 696e 732e   user: builtins.
-00002020: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-00002030: 2020 2077 6865 6e3a 2067 6f6f 676c 652e     when: google.
-00002040: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
-00002050: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
-00002060: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00002070: 2020 2020 2020 206f 7269 6769 6e3a 2062         origin: b
-00002080: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00002090: 2e2c 0a20 2020 2020 2020 2073 6f75 7263  .,.        sourc
-000020a0: 653a 2067 6c6f 6261 6c5f 5f5f 4175 6469  e: global___Audi
-000020b0: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
-000020c0: 7065 203d 202e 2e2e 2c0a 2020 2020 2020  pe = ...,.      
-000020d0: 2020 6b62 6964 3a20 6275 696c 7469 6e73    kbid: builtins
-000020e0: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-000020f0: 2020 2020 7575 6964 3a20 6275 696c 7469      uuid: builti
-00002100: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00002110: 2020 2020 2020 6d65 7373 6167 655f 736f        message_so
-00002120: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
-00002130: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
-00002140: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
-00002150: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-00002160: 2020 2020 6669 656c 645f 6d65 7461 6461      field_metada
-00002170: 7461 3a20 636f 6c6c 6563 7469 6f6e 732e  ta: collections.
-00002180: 6162 632e 4974 6572 6162 6c65 5b6e 7563  abc.Iterable[nuc
-00002190: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
-000021a0: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
-000021b0: 4944 5d20 7c20 4e6f 6e65 203d 202e 2e2e  ID] | None = ...
-000021c0: 2c0a 2020 2020 2020 2020 6175 6469 745f  ,.        audit_
-000021d0: 6669 656c 6473 3a20 636f 6c6c 6563 7469  fields: collecti
-000021e0: 6f6e 732e 6162 632e 4974 6572 6162 6c65  ons.abc.Iterable
-000021f0: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
-00002200: 2e61 7564 6974 5f70 6232 2e41 7564 6974  .audit_pb2.Audit
-00002210: 4669 656c 645d 207c 204e 6f6e 6520 3d20  Field] | None = 
-00002220: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
-00002230: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00002240: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
-00002250: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00002260: 672e 4c69 7465 7261 6c5b 2277 6865 6e22  g.Literal["when"
-00002270: 2c20 6222 7768 656e 225d 2920 2d3e 2062  , b"when"]) -> b
-00002280: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-00002290: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-000022a0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-000022b0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-000022c0: 7465 7261 6c5b 2261 7564 6974 5f66 6965  teral["audit_fie
-000022d0: 6c64 7322 2c20 6222 6175 6469 745f 6669  lds", b"audit_fi
-000022e0: 656c 6473 222c 2022 6669 656c 645f 6d65  elds", "field_me
-000022f0: 7461 6461 7461 222c 2062 2266 6965 6c64  tadata", b"field
-00002300: 5f6d 6574 6164 6174 6122 2c20 226b 6269  _metadata", "kbi
-00002310: 6422 2c20 6222 6b62 6964 222c 2022 6d65  d", b"kbid", "me
-00002320: 7373 6167 655f 736f 7572 6365 222c 2062  ssage_source", b
-00002330: 226d 6573 7361 6765 5f73 6f75 7263 6522  "message_source"
-00002340: 2c20 226f 7269 6769 6e22 2c20 6222 6f72  , "origin", b"or
-00002350: 6967 696e 222c 2022 736f 7572 6365 222c  igin", "source",
-00002360: 2062 2273 6f75 7263 6522 2c20 2275 7365   b"source", "use
-00002370: 7222 2c20 6222 7573 6572 222c 2022 7575  r", b"user", "uu
-00002380: 6964 222c 2062 2275 7569 6422 2c20 2277  id", b"uuid", "w
-00002390: 6865 6e22 2c20 6222 7768 656e 225d 2920  hen", b"when"]) 
-000023a0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-000023b0: 6f62 616c 5f5f 5f41 7564 6974 203d 2041  obal___Audit = A
-000023c0: 7564 6974 0a0a 4074 7970 696e 672e 6669  udit..@typing.fi
-000023d0: 6e61 6c0a 636c 6173 7320 4572 726f 7228  nal.class Error(
-000023e0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000023f0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-00002400: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
-00002410: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-00002420: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
-00002430: 6372 6970 746f 720a 0a20 2020 2063 6c61  criptor..    cla
-00002440: 7373 205f 4572 726f 7243 6f64 653a 0a20  ss _ErrorCode:. 
-00002450: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
-00002460: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
-00002470: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
-00002480: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
-00002490: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
-000024a0: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
-000024b0: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
-000024c0: 0a20 2020 2063 6c61 7373 205f 4572 726f  .    class _Erro
-000024d0: 7243 6f64 6545 6e75 6d54 7970 6557 7261  rCodeEnumTypeWra
-000024e0: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
-000024f0: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
-00002500: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
-00002510: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
-00002520: 5b45 7272 6f72 2e5f 4572 726f 7243 6f64  [Error._ErrorCod
-00002530: 652e 5661 6c75 6554 7970 655d 2c20 6275  e.ValueType], bu
-00002540: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
-00002550: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
-00002560: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-00002570: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
-00002580: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
-00002590: 2020 2020 4745 4e45 5249 433a 2045 7272      GENERIC: Err
-000025a0: 6f72 2e5f 4572 726f 7243 6f64 652e 5661  or._ErrorCode.Va
-000025b0: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
-000025c0: 2020 2020 2045 5854 5241 4354 3a20 4572       EXTRACT: Er
-000025d0: 726f 722e 5f45 7272 6f72 436f 6465 2e56  ror._ErrorCode.V
-000025e0: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
-000025f0: 2020 2020 2020 5052 4f43 4553 533a 2045        PROCESS: E
-00002600: 7272 6f72 2e5f 4572 726f 7243 6f64 652e  rror._ErrorCode.
-00002610: 5661 6c75 6554 7970 6520 2023 2032 0a0a  ValueType  # 2..
-00002620: 2020 2020 636c 6173 7320 4572 726f 7243      class ErrorC
-00002630: 6f64 6528 5f45 7272 6f72 436f 6465 2c20  ode(_ErrorCode, 
-00002640: 6d65 7461 636c 6173 733d 5f45 7272 6f72  metaclass=_Error
-00002650: 436f 6465 456e 756d 5479 7065 5772 6170  CodeEnumTypeWrap
-00002660: 7065 7229 3a20 2e2e 2e0a 2020 2020 4745  per): ....    GE
-00002670: 4e45 5249 433a 2045 7272 6f72 2e45 7272  NERIC: Error.Err
-00002680: 6f72 436f 6465 2e56 616c 7565 5479 7065  orCode.ValueType
-00002690: 2020 2320 300a 2020 2020 4558 5452 4143    # 0.    EXTRAC
-000026a0: 543a 2045 7272 6f72 2e45 7272 6f72 436f  T: Error.ErrorCo
-000026b0: 6465 2e56 616c 7565 5479 7065 2020 2320  de.ValueType  # 
-000026c0: 310a 2020 2020 5052 4f43 4553 533a 2045  1.    PROCESS: E
-000026d0: 7272 6f72 2e45 7272 6f72 436f 6465 2e56  rror.ErrorCode.V
-000026e0: 616c 7565 5479 7065 2020 2320 320a 0a20  alueType  # 2.. 
-000026f0: 2020 2046 4945 4c44 5f46 4945 4c44 5f4e     FIELD_FIELD_N
-00002700: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00002710: 696e 740a 2020 2020 4649 454c 445f 5459  int.    FIELD_TY
-00002720: 5045 5f46 4945 4c44 5f4e 554d 4245 523a  PE_FIELD_NUMBER:
-00002730: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00002740: 2020 4552 524f 525f 4649 454c 445f 4e55    ERROR_FIELD_NU
-00002750: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00002760: 6e74 0a20 2020 2043 4f44 455f 4649 454c  nt.    CODE_FIEL
-00002770: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00002780: 6e73 2e69 6e74 0a20 2020 2066 6965 6c64  ns.int.    field
-00002790: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-000027a0: 2020 2066 6965 6c64 5f74 7970 653a 206e     field_type: n
-000027b0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-000027c0: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
-000027d0: 6c64 5479 7065 2e56 616c 7565 5479 7065  ldType.ValueType
-000027e0: 0a20 2020 2065 7272 6f72 3a20 6275 696c  .    error: buil
-000027f0: 7469 6e73 2e73 7472 0a20 2020 2063 6f64  tins.str.    cod
-00002800: 653a 2067 6c6f 6261 6c5f 5f5f 4572 726f  e: global___Erro
-00002810: 722e 4572 726f 7243 6f64 652e 5661 6c75  r.ErrorCode.Valu
-00002820: 6554 7970 650a 2020 2020 6465 6620 5f5f  eType.    def __
-00002830: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00002840: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00002850: 0a20 2020 2020 2020 2066 6965 6c64 3a20  .        field: 
-00002860: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-00002870: 2e2e 2c0a 2020 2020 2020 2020 6669 656c  ..,.        fiel
-00002880: 645f 7479 7065 3a20 6e75 636c 6961 6462  d_type: nucliadb
-00002890: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-000028a0: 735f 7062 322e 4669 656c 6454 7970 652e  s_pb2.FieldType.
-000028b0: 5661 6c75 6554 7970 6520 3d20 2e2e 2e2c  ValueType = ...,
-000028c0: 0a20 2020 2020 2020 2065 7272 6f72 3a20  .        error: 
-000028d0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-000028e0: 2e2e 2c0a 2020 2020 2020 2020 636f 6465  ..,.        code
-000028f0: 3a20 676c 6f62 616c 5f5f 5f45 7272 6f72  : global___Error
-00002900: 2e45 7272 6f72 436f 6465 2e56 616c 7565  .ErrorCode.Value
-00002910: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-00002920: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00002930: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-00002940: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00002950: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00002960: 616c 5b22 636f 6465 222c 2062 2263 6f64  al["code", b"cod
-00002970: 6522 2c20 2265 7272 6f72 222c 2062 2265  e", "error", b"e
-00002980: 7272 6f72 222c 2022 6669 656c 6422 2c20  rror", "field", 
-00002990: 6222 6669 656c 6422 2c20 2266 6965 6c64  b"field", "field
-000029a0: 5f74 7970 6522 2c20 6222 6669 656c 645f  _type", b"field_
-000029b0: 7479 7065 225d 2920 2d3e 204e 6f6e 653a  type"]) -> None:
-000029c0: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f45   .....global___E
-000029d0: 7272 6f72 203d 2045 7272 6f72 0a0a 4074  rror = Error..@t
-000029e0: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
-000029f0: 7320 4272 6f6b 6572 4d65 7373 6167 6528  s BrokerMessage(
-00002a00: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00002a10: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-00002a20: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
-00002a30: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-00002a40: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
-00002a50: 6372 6970 746f 720a 0a20 2020 2063 6c61  criptor..    cla
-00002a60: 7373 205f 4d65 7373 6167 6554 7970 653a  ss _MessageType:
-00002a70: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
-00002a80: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
-00002a90: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
-00002aa0: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
-00002ab0: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
-00002ac0: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
-00002ad0: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
-00002ae0: 650a 0a20 2020 2063 6c61 7373 205f 4d65  e..    class _Me
-00002af0: 7373 6167 6554 7970 6545 6e75 6d54 7970  ssageTypeEnumTyp
-00002b00: 6557 7261 7070 6572 2867 6f6f 676c 652e  eWrapper(google.
-00002b10: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
-00002b20: 6c2e 656e 756d 5f74 7970 655f 7772 6170  l.enum_type_wrap
-00002b30: 7065 722e 5f45 6e75 6d54 7970 6557 7261  per._EnumTypeWra
-00002b40: 7070 6572 5b42 726f 6b65 724d 6573 7361  pper[BrokerMessa
-00002b50: 6765 2e5f 4d65 7373 6167 6554 7970 652e  ge._MessageType.
-00002b60: 5661 6c75 6554 7970 655d 2c20 6275 696c  ValueType], buil
-00002b70: 7469 6e73 2e74 7970 6529 3a0a 2020 2020  tins.type):.    
-00002b80: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00002b90: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00002ba0: 6465 7363 7269 7074 6f72 2e45 6e75 6d44  descriptor.EnumD
-00002bb0: 6573 6372 6970 746f 720a 2020 2020 2020  escriptor.      
-00002bc0: 2020 4155 544f 434f 4d4d 4954 3a20 4272    AUTOCOMMIT: Br
-00002bd0: 6f6b 6572 4d65 7373 6167 652e 5f4d 6573  okerMessage._Mes
-00002be0: 7361 6765 5479 7065 2e56 616c 7565 5479  sageType.ValueTy
-00002bf0: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
-00002c00: 4d55 4c54 493a 2042 726f 6b65 724d 6573  MULTI: BrokerMes
-00002c10: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
-00002c20: 652e 5661 6c75 6554 7970 6520 2023 2031  e.ValueType  # 1
-00002c30: 0a20 2020 2020 2020 2043 4f4d 4d49 543a  .        COMMIT:
-00002c40: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
-00002c50: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
-00002c60: 6554 7970 6520 2023 2032 0a20 2020 2020  eType  # 2.     
-00002c70: 2020 2052 4f4c 4c42 4143 4b3a 2042 726f     ROLLBACK: Bro
-00002c80: 6b65 724d 6573 7361 6765 2e5f 4d65 7373  kerMessage._Mess
-00002c90: 6167 6554 7970 652e 5661 6c75 6554 7970  ageType.ValueTyp
-00002ca0: 6520 2023 2033 0a20 2020 2020 2020 2044  e  # 3.        D
-00002cb0: 454c 4554 453a 2042 726f 6b65 724d 6573  ELETE: BrokerMes
-00002cc0: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
-00002cd0: 652e 5661 6c75 6554 7970 6520 2023 2034  e.ValueType  # 4
-00002ce0: 0a0a 2020 2020 636c 6173 7320 4d65 7373  ..    class Mess
-00002cf0: 6167 6554 7970 6528 5f4d 6573 7361 6765  ageType(_Message
-00002d00: 5479 7065 2c20 6d65 7461 636c 6173 733d  Type, metaclass=
-00002d10: 5f4d 6573 7361 6765 5479 7065 456e 756d  _MessageTypeEnum
-00002d20: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
-00002d30: 2e0a 2020 2020 4155 544f 434f 4d4d 4954  ..    AUTOCOMMIT
-00002d40: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
-00002d50: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
-00002d60: 6554 7970 6520 2023 2030 0a20 2020 204d  eType  # 0.    M
-00002d70: 554c 5449 3a20 4272 6f6b 6572 4d65 7373  ULTI: BrokerMess
-00002d80: 6167 652e 4d65 7373 6167 6554 7970 652e  age.MessageType.
-00002d90: 5661 6c75 6554 7970 6520 2023 2031 0a20  ValueType  # 1. 
-00002da0: 2020 2043 4f4d 4d49 543a 2042 726f 6b65     COMMIT: Broke
-00002db0: 724d 6573 7361 6765 2e4d 6573 7361 6765  rMessage.Message
-00002dc0: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
-00002dd0: 2320 320a 2020 2020 524f 4c4c 4241 434b  # 2.    ROLLBACK
-00002de0: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
-00002df0: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
-00002e00: 6554 7970 6520 2023 2033 0a20 2020 2044  eType  # 3.    D
-00002e10: 454c 4554 453a 2042 726f 6b65 724d 6573  ELETE: BrokerMes
-00002e20: 7361 6765 2e4d 6573 7361 6765 5479 7065  sage.MessageType
-00002e30: 2e56 616c 7565 5479 7065 2020 2320 340a  .ValueType  # 4.
-00002e40: 0a20 2020 2063 6c61 7373 205f 4d65 7373  .    class _Mess
-00002e50: 6167 6553 6f75 7263 653a 0a20 2020 2020  ageSource:.     
-00002e60: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
-00002e70: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
-00002e80: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
-00002e90: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
-00002ea0: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
-00002eb0: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
-00002ec0: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
-00002ed0: 2063 6c61 7373 205f 4d65 7373 6167 6553   class _MessageS
-00002ee0: 6f75 7263 6545 6e75 6d54 7970 6557 7261  ourceEnumTypeWra
-00002ef0: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
-00002f00: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
-00002f10: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
-00002f20: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
-00002f30: 5b42 726f 6b65 724d 6573 7361 6765 2e5f  [BrokerMessage._
-00002f40: 4d65 7373 6167 6553 6f75 7263 652e 5661  MessageSource.Va
-00002f50: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
-00002f60: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
-00002f70: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00002f80: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00002f90: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
-00002fa0: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
-00002fb0: 5752 4954 4552 3a20 4272 6f6b 6572 4d65  WRITER: BrokerMe
-00002fc0: 7373 6167 652e 5f4d 6573 7361 6765 536f  ssage._MessageSo
-00002fd0: 7572 6365 2e56 616c 7565 5479 7065 2020  urce.ValueType  
-00002fe0: 2320 300a 2020 2020 2020 2020 5052 4f43  # 0.        PROC
-00002ff0: 4553 534f 523a 2042 726f 6b65 724d 6573  ESSOR: BrokerMes
-00003000: 7361 6765 2e5f 4d65 7373 6167 6553 6f75  sage._MessageSou
-00003010: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
-00003020: 2031 0a0a 2020 2020 636c 6173 7320 4d65   1..    class Me
-00003030: 7373 6167 6553 6f75 7263 6528 5f4d 6573  ssageSource(_Mes
-00003040: 7361 6765 536f 7572 6365 2c20 6d65 7461  sageSource, meta
-00003050: 636c 6173 733d 5f4d 6573 7361 6765 536f  class=_MessageSo
-00003060: 7572 6365 456e 756d 5479 7065 5772 6170  urceEnumTypeWrap
-00003070: 7065 7229 3a20 2e2e 2e0a 2020 2020 5752  per): ....    WR
-00003080: 4954 4552 3a20 4272 6f6b 6572 4d65 7373  ITER: BrokerMess
-00003090: 6167 652e 4d65 7373 6167 6553 6f75 7263  age.MessageSourc
-000030a0: 652e 5661 6c75 6554 7970 6520 2023 2030  e.ValueType  # 0
-000030b0: 0a20 2020 2050 524f 4345 5353 4f52 3a20  .    PROCESSOR: 
-000030c0: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
-000030d0: 7373 6167 6553 6f75 7263 652e 5661 6c75  ssageSource.Valu
-000030e0: 6554 7970 6520 2023 2031 0a0a 2020 2020  eType  # 1..    
-000030f0: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
-00003100: 2020 636c 6173 7320 436f 6e76 6572 7361    class Conversa
-00003110: 7469 6f6e 7345 6e74 7279 2867 6f6f 676c  tionsEntry(googl
-00003120: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00003130: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00003140: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
-00003150: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00003160: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-00003170: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
-00003180: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-00003190: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-000031a0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
-000031b0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000031c0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-000031d0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-000031e0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
-000031f0: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
-00003200: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
-00003210: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00003220: 6573 6f75 7263 6573 5f70 6232 2e43 6f6e  esources_pb2.Con
-00003230: 7665 7273 6174 696f 6e3a 202e 2e2e 0a20  versation: .... 
-00003240: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
-00003250: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
-00003260: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-00003270: 2020 202a 2c0a 2020 2020 2020 2020 2020     *,.          
-00003280: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
-00003290: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-000032a0: 2020 2020 2020 2076 616c 7565 3a20 6e75         value: nu
-000032b0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-000032c0: 736f 7572 6365 735f 7062 322e 436f 6e76  sources_pb2.Conv
-000032d0: 6572 7361 7469 6f6e 207c 204e 6f6e 6520  ersation | None 
-000032e0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
-000032f0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00003300: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
-00003310: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-00003320: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-00003330: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
-00003340: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
-00003350: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-00003360: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
-00003370: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00003380: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00003390: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
-000033a0: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
-000033b0: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
-000033c0: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
-000033d0: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
-000033e0: 7373 204c 6179 6f75 7473 456e 7472 7928  ss LayoutsEntry(
-000033f0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00003400: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-00003410: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
-00003420: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-00003430: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-00003440: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-00003450: 2020 2020 204b 4559 5f46 4945 4c44 5f4e       KEY_FIELD_N
-00003460: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00003470: 696e 740a 2020 2020 2020 2020 5641 4c55  int.        VALU
-00003480: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
-00003490: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000034a0: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
-000034b0: 6e73 2e73 7472 0a20 2020 2020 2020 2040  ns.str.        @
-000034c0: 7072 6f70 6572 7479 0a20 2020 2020 2020  property.       
-000034d0: 2064 6566 2076 616c 7565 2873 656c 6629   def value(self)
-000034e0: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-000034f0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00003500: 322e 4669 656c 644c 6179 6f75 743a 202e  2.FieldLayout: .
-00003510: 2e2e 0a20 2020 2020 2020 2064 6566 205f  ...        def _
-00003520: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00003530: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00003540: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00003550: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
-00003560: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-00003570: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00003580: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-00003590: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-000035a0: 4669 656c 644c 6179 6f75 7420 7c20 4e6f  FieldLayout | No
-000035b0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-000035c0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-000035d0: 0a20 2020 2020 2020 2064 6566 2048 6173  .        def Has
-000035e0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-000035f0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-00003600: 6974 6572 616c 5b22 7661 6c75 6522 2c20  iteral["value", 
-00003610: 6222 7661 6c75 6522 5d29 202d 3e20 6275  b"value"]) -> bu
-00003620: 696c 7469 6e73 2e62 6f6f 6c3a 202e 2e2e  iltins.bool: ...
-00003630: 0a20 2020 2020 2020 2064 6566 2043 6c65  .        def Cle
-00003640: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-00003650: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00003660: 2e4c 6974 6572 616c 5b22 6b65 7922 2c20  .Literal["key", 
-00003670: 6222 6b65 7922 2c20 2276 616c 7565 222c  b"key", "value",
-00003680: 2062 2276 616c 7565 225d 2920 2d3e 204e   b"value"]) -> N
-00003690: 6f6e 653a 202e 2e2e 0a0a 2020 2020 4074  one: .....    @t
-000036a0: 7970 696e 672e 6669 6e61 6c0a 2020 2020  yping.final.    
-000036b0: 636c 6173 7320 5465 7874 7345 6e74 7279  class TextsEntry
-000036c0: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-000036d0: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-000036e0: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
-000036f0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-00003700: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00003710: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00003720: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
-00003730: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00003740: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
-00003750: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
-00003760: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00003770: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
-00003780: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
-00003790: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
-000037a0: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
-000037b0: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-000037c0: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-000037d0: 6232 2e46 6965 6c64 5465 7874 3a20 2e2e  b2.FieldText: ..
-000037e0: 2e0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
-000037f0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00003800: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00003810: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00003820: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
-00003830: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00003840: 2020 2020 2020 2020 2020 7661 6c75 653a            value:
-00003850: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00003860: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00003870: 6965 6c64 5465 7874 207c 204e 6f6e 6520  ieldText | None 
-00003880: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
-00003890: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-000038a0: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
-000038b0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-000038c0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-000038d0: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
-000038e0: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
-000038f0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-00003900: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
-00003910: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00003920: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00003930: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
-00003940: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
-00003950: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
-00003960: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
-00003970: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
-00003980: 7373 204b 6579 776f 7264 7365 7473 456e  ss KeywordsetsEn
-00003990: 7472 7928 676f 6f67 6c65 2e70 726f 746f  try(google.proto
-000039a0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
-000039b0: 6167 6529 3a0a 2020 2020 2020 2020 4445  age):.        DE
-000039c0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-000039d0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-000039e0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-000039f0: 0a20 2020 2020 2020 204b 4559 5f46 4945  .        KEY_FIE
-00003a00: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00003a10: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-00003a20: 5641 4c55 455f 4649 454c 445f 4e55 4d42  VALUE_FIELD_NUMB
-00003a30: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00003a40: 0a20 2020 2020 2020 206b 6579 3a20 6275  .        key: bu
-00003a50: 696c 7469 6e73 2e73 7472 0a20 2020 2020  iltins.str.     
-00003a60: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00003a70: 2020 2020 2064 6566 2076 616c 7565 2873       def value(s
-00003a80: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
-00003a90: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00003aa0: 735f 7062 322e 4669 656c 644b 6579 776f  s_pb2.FieldKeywo
-00003ab0: 7264 7365 743a 202e 2e2e 0a20 2020 2020  rdset: ....     
-00003ac0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00003ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003ae0: 662c 0a20 2020 2020 2020 2020 2020 202a  f,.            *
-00003af0: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
-00003b00: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
-00003b10: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2020  = ...,.         
-00003b20: 2020 2076 616c 7565 3a20 6e75 636c 6961     value: nuclia
-00003b30: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00003b40: 6365 735f 7062 322e 4669 656c 644b 6579  ces_pb2.FieldKey
-00003b50: 776f 7264 7365 7420 7c20 4e6f 6e65 203d  wordset | None =
-00003b60: 202e 2e2e 2c0a 2020 2020 2020 2020 2920   ...,.        ) 
-00003b70: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-00003b80: 2020 2020 2064 6566 2048 6173 4669 656c       def HasFiel
-00003b90: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00003ba0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00003bb0: 616c 5b22 7661 6c75 6522 2c20 6222 7661  al["value", b"va
-00003bc0: 6c75 6522 5d29 202d 3e20 6275 696c 7469  lue"]) -> builti
-00003bd0: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
-00003be0: 2020 2020 2064 6566 2043 6c65 6172 4669       def ClearFi
-00003bf0: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-00003c00: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-00003c10: 6572 616c 5b22 6b65 7922 2c20 6222 6b65  eral["key", b"ke
-00003c20: 7922 2c20 2276 616c 7565 222c 2062 2276  y", "value", b"v
-00003c30: 616c 7565 225d 2920 2d3e 204e 6f6e 653a  alue"]) -> None:
-00003c40: 202e 2e2e 0a0a 2020 2020 4074 7970 696e   .....    @typin
-00003c50: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
-00003c60: 7320 4461 7465 7469 6d65 7345 6e74 7279  s DatetimesEntry
-00003c70: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-00003c80: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-00003c90: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
-00003ca0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-00003cb0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00003cc0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00003cd0: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
-00003ce0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00003cf0: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
-00003d00: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
-00003d10: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00003d20: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
-00003d30: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
-00003d40: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
-00003d50: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
-00003d60: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-00003d70: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00003d80: 6232 2e46 6965 6c64 4461 7465 7469 6d65  b2.FieldDatetime
-00003d90: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-00003da0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00003db0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00003dc0: 2020 2020 2020 2020 2020 2a2c 0a20 2020            *,.   
-00003dd0: 2020 2020 2020 2020 206b 6579 3a20 6275           key: bu
-00003de0: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
-00003df0: 2c0a 2020 2020 2020 2020 2020 2020 7661  ,.            va
-00003e00: 6c75 653a 206e 7563 6c69 6164 625f 7072  lue: nucliadb_pr
-00003e10: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00003e20: 6232 2e46 6965 6c64 4461 7465 7469 6d65  b2.FieldDatetime
-00003e30: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00003e40: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
-00003e50: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-00003e60: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
-00003e70: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-00003e80: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
-00003e90: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
-00003ea0: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-00003eb0: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-00003ec0: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-00003ed0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00003ee0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-00003ef0: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
-00003f00: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
-00003f10: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
-00003f20: 2020 2040 7479 7069 6e67 2e66 696e 616c     @typing.final
-00003f30: 0a20 2020 2063 6c61 7373 204c 696e 6b73  .    class Links
-00003f40: 456e 7472 7928 676f 6f67 6c65 2e70 726f  Entry(google.pro
-00003f50: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
-00003f60: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
-00003f70: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00003f80: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00003f90: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00003fa0: 720a 0a20 2020 2020 2020 204b 4559 5f46  r..        KEY_F
-00003fb0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00003fc0: 6c74 696e 732e 696e 740a 2020 2020 2020  ltins.int.      
-00003fd0: 2020 5641 4c55 455f 4649 454c 445f 4e55    VALUE_FIELD_NU
-00003fe0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00003ff0: 6e74 0a20 2020 2020 2020 206b 6579 3a20  nt.        key: 
-00004000: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
-00004010: 2020 2020 2040 7072 6f70 6572 7479 0a20       @property. 
-00004020: 2020 2020 2020 2064 6566 2076 616c 7565         def value
-00004030: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-00004040: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00004050: 6365 735f 7062 322e 4669 656c 644c 696e  ces_pb2.FieldLin
-00004060: 6b3a 202e 2e2e 0a20 2020 2020 2020 2064  k: ....        d
-00004070: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00004080: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00004090: 2020 2020 2020 2020 2020 202a 2c0a 2020             *,.  
-000040a0: 2020 2020 2020 2020 2020 6b65 793a 2062            key: b
-000040b0: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-000040c0: 2e2c 0a20 2020 2020 2020 2020 2020 2076  .,.            v
-000040d0: 616c 7565 3a20 6e75 636c 6961 6462 5f70  alue: nucliadb_p
-000040e0: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
-000040f0: 7062 322e 4669 656c 644c 696e 6b20 7c20  pb2.FieldLink | 
-00004100: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00004110: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-00004120: 2e2e 0a20 2020 2020 2020 2064 6566 2048  ...        def H
-00004130: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
-00004140: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00004150: 2e4c 6974 6572 616c 5b22 7661 6c75 6522  .Literal["value"
-00004160: 2c20 6222 7661 6c75 6522 5d29 202d 3e20  , b"value"]) -> 
-00004170: 6275 696c 7469 6e73 2e62 6f6f 6c3a 202e  builtins.bool: .
-00004180: 2e2e 0a20 2020 2020 2020 2064 6566 2043  ...        def C
-00004190: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-000041a0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-000041b0: 6e67 2e4c 6974 6572 616c 5b22 6b65 7922  ng.Literal["key"
-000041c0: 2c20 6222 6b65 7922 2c20 2276 616c 7565  , b"key", "value
-000041d0: 222c 2062 2276 616c 7565 225d 2920 2d3e  ", b"value"]) ->
-000041e0: 204e 6f6e 653a 202e 2e2e 0a0a 2020 2020   None: .....    
-000041f0: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
-00004200: 2020 636c 6173 7320 4669 6c65 7345 6e74    class FilesEnt
-00004210: 7279 2867 6f6f 676c 652e 7072 6f74 6f62  ry(google.protob
-00004220: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00004230: 6765 293a 0a20 2020 2020 2020 2044 4553  ge):.        DES
-00004240: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
-00004250: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
-00004260: 746f 722e 4465 7363 7269 7074 6f72 0a0a  tor.Descriptor..
-00004270: 2020 2020 2020 2020 4b45 595f 4649 454c          KEY_FIEL
-00004280: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004290: 6e73 2e69 6e74 0a20 2020 2020 2020 2056  ns.int.        V
-000042a0: 414c 5545 5f46 4945 4c44 5f4e 554d 4245  ALUE_FIELD_NUMBE
-000042b0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000042c0: 2020 2020 2020 2020 6b65 793a 2062 7569          key: bui
-000042d0: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
-000042e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-000042f0: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
-00004300: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-00004310: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00004320: 5f70 6232 2e46 6965 6c64 4669 6c65 3a20  _pb2.FieldFile: 
-00004330: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
-00004340: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00004350: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00004360: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00004370: 2020 2020 2020 206b 6579 3a20 6275 696c         key: buil
-00004380: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
-00004390: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-000043a0: 653a 206e 7563 6c69 6164 625f 7072 6f74  e: nucliadb_prot
-000043b0: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
-000043c0: 2e46 6965 6c64 4669 6c65 207c 204e 6f6e  .FieldFile | Non
-000043d0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-000043e0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-000043f0: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
-00004400: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00004410: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00004420: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
-00004430: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
-00004440: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
-00004450: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
-00004460: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-00004470: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00004480: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
-00004490: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
-000044a0: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
-000044b0: 6e65 3a20 2e2e 2e0a 0a20 2020 204b 4249  ne: .....    KBI
-000044c0: 445f 4649 454c 445f 4e55 4d42 4552 3a20  D_FIELD_NUMBER: 
-000044d0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000044e0: 2055 5549 445f 4649 454c 445f 4e55 4d42   UUID_FIELD_NUMB
-000044f0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00004500: 0a20 2020 2053 4c55 475f 4649 454c 445f  .    SLUG_FIELD_
-00004510: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00004520: 2e69 6e74 0a20 2020 2041 5544 4954 5f46  .int.    AUDIT_F
-00004530: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004540: 6c74 696e 732e 696e 740a 2020 2020 5459  ltins.int.    TY
-00004550: 5045 5f46 4945 4c44 5f4e 554d 4245 523a  PE_FIELD_NUMBER:
-00004560: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00004570: 2020 4d55 4c54 4949 445f 4649 454c 445f    MULTIID_FIELD_
-00004580: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00004590: 2e69 6e74 0a20 2020 2042 4153 4943 5f46  .int.    BASIC_F
-000045a0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-000045b0: 6c74 696e 732e 696e 740a 2020 2020 4f52  ltins.int.    OR
-000045c0: 4947 494e 5f46 4945 4c44 5f4e 554d 4245  IGIN_FIELD_NUMBE
-000045d0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000045e0: 2020 2020 5245 4c41 5449 4f4e 535f 4649      RELATIONS_FI
-000045f0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00004600: 7469 6e73 2e69 6e74 0a20 2020 2043 4f4e  tins.int.    CON
-00004610: 5645 5253 4154 494f 4e53 5f46 4945 4c44  VERSATIONS_FIELD
-00004620: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00004630: 732e 696e 740a 2020 2020 4c41 594f 5554  s.int.    LAYOUT
-00004640: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-00004650: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00004660: 2054 4558 5453 5f46 4945 4c44 5f4e 554d   TEXTS_FIELD_NUM
-00004670: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00004680: 740a 2020 2020 4b45 5957 4f52 4453 4554  t.    KEYWORDSET
-00004690: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-000046a0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000046b0: 2044 4154 4554 494d 4553 5f46 4945 4c44   DATETIMES_FIELD
-000046c0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-000046d0: 732e 696e 740a 2020 2020 4c49 4e4b 535f  s.int.    LINKS_
-000046e0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-000046f0: 696c 7469 6e73 2e69 6e74 0a20 2020 2046  iltins.int.    F
-00004700: 494c 4553 5f46 4945 4c44 5f4e 554d 4245  ILES_FIELD_NUMBE
-00004710: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00004720: 2020 2020 4c49 4e4b 5f45 5854 5241 4354      LINK_EXTRACT
-00004730: 4544 5f44 4154 415f 4649 454c 445f 4e55  ED_DATA_FIELD_NU
-00004740: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00004750: 6e74 0a20 2020 2046 494c 455f 4558 5452  nt.    FILE_EXTR
-00004760: 4143 5445 445f 4441 5441 5f46 4945 4c44  ACTED_DATA_FIELD
-00004770: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00004780: 732e 696e 740a 2020 2020 4558 5452 4143  s.int.    EXTRAC
-00004790: 5445 445f 5445 5854 5f46 4945 4c44 5f4e  TED_TEXT_FIELD_N
-000047a0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-000047b0: 696e 740a 2020 2020 4649 454c 445f 4d45  int.    FIELD_ME
-000047c0: 5441 4441 5441 5f46 4945 4c44 5f4e 554d  TADATA_FIELD_NUM
-000047d0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-000047e0: 740a 2020 2020 4649 454c 445f 5645 4354  t.    FIELD_VECT
-000047f0: 4f52 535f 4649 454c 445f 4e55 4d42 4552  ORS_FIELD_NUMBER
-00004800: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00004810: 2020 2046 4945 4c44 5f4c 4152 4745 5f4d     FIELD_LARGE_M
-00004820: 4554 4144 4154 415f 4649 454c 445f 4e55  ETADATA_FIELD_NU
-00004830: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00004840: 6e74 0a20 2020 2044 454c 4554 455f 4649  nt.    DELETE_FI
-00004850: 454c 4453 5f46 4945 4c44 5f4e 554d 4245  ELDS_FIELD_NUMBE
-00004860: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00004870: 2020 2020 4f52 4947 494e 5f53 4551 5f46      ORIGIN_SEQ_F
-00004880: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004890: 6c74 696e 732e 696e 740a 2020 2020 534c  ltins.int.    SL
-000048a0: 4f57 5f50 524f 4345 5353 494e 475f 5449  OW_PROCESSING_TI
-000048b0: 4d45 5f46 4945 4c44 5f4e 554d 4245 523a  ME_FIELD_NUMBER:
-000048c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000048d0: 2020 5052 455f 5052 4f43 4553 5349 4e47    PRE_PROCESSING
-000048e0: 5f54 494d 455f 4649 454c 445f 4e55 4d42  _TIME_FIELD_NUMB
-000048f0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00004900: 0a20 2020 2044 4f4e 455f 5449 4d45 5f46  .    DONE_TIME_F
-00004910: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004920: 6c74 696e 732e 696e 740a 2020 2020 5458  ltins.int.    TX
-00004930: 5345 5149 445f 4649 454c 445f 4e55 4d42  SEQID_FIELD_NUMB
-00004940: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00004950: 0a20 2020 2045 5252 4f52 535f 4649 454c  .    ERRORS_FIEL
-00004960: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004970: 6e73 2e69 6e74 0a20 2020 2050 524f 4345  ns.int.    PROCE
-00004980: 5353 494e 475f 4944 5f46 4945 4c44 5f4e  SSING_ID_FIELD_N
-00004990: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-000049a0: 696e 740a 2020 2020 534f 5552 4345 5f46  int.    SOURCE_F
-000049b0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-000049c0: 6c74 696e 732e 696e 740a 2020 2020 4143  ltins.int.    AC
-000049d0: 434f 554e 545f 5345 515f 4649 454c 445f  COUNT_SEQ_FIELD_
-000049e0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-000049f0: 2e69 6e74 0a20 2020 2055 5345 525f 5645  .int.    USER_VE
-00004a00: 4354 4f52 535f 4649 454c 445f 4e55 4d42  CTORS_FIELD_NUMB
-00004a10: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00004a20: 0a20 2020 2052 4549 4e44 4558 5f46 4945  .    REINDEX_FIE
-00004a30: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00004a40: 696e 732e 696e 740a 2020 2020 4558 5452  ins.int.    EXTR
-00004a50: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
-00004a60: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00004a70: 2051 5545 5354 494f 4e5f 414e 5357 4552   QUESTION_ANSWER
-00004a80: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-00004a90: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00004aa0: 2053 4543 5552 4954 595f 4649 454c 445f   SECURITY_FIELD_
-00004ab0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00004ac0: 2e69 6e74 0a20 2020 206b 6269 643a 2062  .int.    kbid: b
-00004ad0: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
-00004ae0: 7575 6964 3a20 6275 696c 7469 6e73 2e73  uuid: builtins.s
-00004af0: 7472 0a20 2020 2073 6c75 673a 2062 7569  tr.    slug: bui
-00004b00: 6c74 696e 732e 7374 720a 2020 2020 7479  ltins.str.    ty
-00004b10: 7065 3a20 676c 6f62 616c 5f5f 5f42 726f  pe: global___Bro
-00004b20: 6b65 724d 6573 7361 6765 2e4d 6573 7361  kerMessage.Messa
-00004b30: 6765 5479 7065 2e56 616c 7565 5479 7065  geType.ValueType
-00004b40: 0a20 2020 206d 756c 7469 6964 3a20 6275  .    multiid: bu
-00004b50: 696c 7469 6e73 2e73 7472 0a20 2020 206f  iltins.str.    o
-00004b60: 7269 6769 6e5f 7365 713a 2062 7569 6c74  rigin_seq: built
-00004b70: 696e 732e 696e 740a 2020 2020 736c 6f77  ins.int.    slow
-00004b80: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
-00004b90: 3a20 6275 696c 7469 6e73 2e66 6c6f 6174  : builtins.float
-00004ba0: 0a20 2020 2070 7265 5f70 726f 6365 7373  .    pre_process
-00004bb0: 696e 675f 7469 6d65 3a20 6275 696c 7469  ing_time: builti
-00004bc0: 6e73 2e66 6c6f 6174 0a20 2020 2074 7873  ns.float.    txs
-00004bd0: 6571 6964 3a20 6275 696c 7469 6e73 2e69  eqid: builtins.i
-00004be0: 6e74 0a20 2020 2022 2222 4e6f 7420 6e65  nt.    """Not ne
-00004bf0: 6564 6564 2061 6e79 6d6f 7265 2222 220a  eded anymore""".
-00004c00: 2020 2020 7072 6f63 6573 7369 6e67 5f69      processing_i
-00004c10: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
-00004c20: 2020 2020 736f 7572 6365 3a20 676c 6f62      source: glob
-00004c30: 616c 5f5f 5f42 726f 6b65 724d 6573 7361  al___BrokerMessa
-00004c40: 6765 2e4d 6573 7361 6765 536f 7572 6365  ge.MessageSource
-00004c50: 2e56 616c 7565 5479 7065 0a20 2020 2061  .ValueType.    a
-00004c60: 6363 6f75 6e74 5f73 6571 3a20 6275 696c  ccount_seq: buil
-00004c70: 7469 6e73 2e69 6e74 0a20 2020 2072 6569  tins.int.    rei
-00004c80: 6e64 6578 3a20 6275 696c 7469 6e73 2e62  ndex: builtins.b
-00004c90: 6f6f 6c0a 2020 2020 2222 2249 6620 7472  ool.    """If tr
-00004ca0: 7565 2c20 666f 7263 6520 7265 696e 6465  ue, force reinde
-00004cb0: 7820 616c 6c20 7061 7261 6772 6170 6873  x all paragraphs
-00004cc0: 2069 6e20 6120 7265 736f 7572 6365 2222   in a resource""
-00004cd0: 220a 2020 2020 4070 726f 7065 7274 790a  ".    @property.
-00004ce0: 2020 2020 6465 6620 6175 6469 7428 7365      def audit(se
-00004cf0: 6c66 2920 2d3e 2067 6c6f 6261 6c5f 5f5f  lf) -> global___
-00004d00: 4175 6469 743a 202e 2e2e 0a20 2020 2040  Audit: ....    @
-00004d10: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00004d20: 2062 6173 6963 2873 656c 6629 202d 3e20   basic(self) -> 
-00004d30: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00004d40: 7265 736f 7572 6365 735f 7062 322e 4261  resources_pb2.Ba
-00004d50: 7369 633a 202e 2e2e 0a20 2020 2040 7072  sic: ....    @pr
-00004d60: 6f70 6572 7479 0a20 2020 2064 6566 206f  operty.    def o
-00004d70: 7269 6769 6e28 7365 6c66 2920 2d3e 206e  rigin(self) -> n
-00004d80: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00004d90: 6573 6f75 7263 6573 5f70 6232 2e4f 7269  esources_pb2.Ori
-00004da0: 6769 6e3a 202e 2e2e 0a20 2020 2040 7072  gin: ....    @pr
-00004db0: 6f70 6572 7479 0a20 2020 2064 6566 2072  operty.    def r
-00004dc0: 656c 6174 696f 6e73 2873 656c 6629 202d  elations(self) -
-00004dd0: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
-00004de0: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
-00004df0: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
-00004e00: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
-00004e10: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
-00004e20: 726f 746f 732e 7574 696c 735f 7062 322e  rotos.utils_pb2.
-00004e30: 5265 6c61 7469 6f6e 5d3a 202e 2e2e 0a20  Relation]: .... 
-00004e40: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00004e50: 2064 6566 2063 6f6e 7665 7273 6174 696f   def conversatio
-00004e60: 6e73 2873 656c 6629 202d 3e20 676f 6f67  ns(self) -> goog
-00004e70: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-00004e80: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-00004e90: 4d65 7373 6167 654d 6170 5b62 7569 6c74  MessageMap[built
-00004ea0: 696e 732e 7374 722c 206e 7563 6c69 6164  ins.str, nucliad
-00004eb0: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00004ec0: 6573 5f70 6232 2e43 6f6e 7665 7273 6174  es_pb2.Conversat
-00004ed0: 696f 6e5d 3a0a 2020 2020 2020 2020 2222  ion]:.        ""
-00004ee0: 2246 6965 6c64 2043 6f6e 7665 7273 6174  "Field Conversat
-00004ef0: 696f 6e73 2222 220a 0a20 2020 2040 7072  ions"""..    @pr
-00004f00: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
-00004f10: 6179 6f75 7473 2873 656c 6629 202d 3e20  ayouts(self) -> 
-00004f20: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00004f30: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
-00004f40: 6572 732e 4d65 7373 6167 654d 6170 5b62  ers.MessageMap[b
-00004f50: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
-00004f60: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
-00004f70: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
-00004f80: 4c61 796f 7574 5d3a 0a20 2020 2020 2020  Layout]:.       
-00004f90: 2022 2222 4669 656c 6420 4c61 796f 7574   """Field Layout
-00004fa0: 2222 220a 0a20 2020 2040 7072 6f70 6572  """..    @proper
-00004fb0: 7479 0a20 2020 2064 6566 2074 6578 7473  ty.    def texts
-00004fc0: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
-00004fd0: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-00004fe0: 616c 2e63 6f6e 7461 696e 6572 732e 4d65  al.containers.Me
-00004ff0: 7373 6167 654d 6170 5b62 7569 6c74 696e  ssageMap[builtin
-00005000: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
-00005010: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00005020: 5f70 6232 2e46 6965 6c64 5465 7874 5d3a  _pb2.FieldText]:
-00005030: 0a20 2020 2020 2020 2022 2222 4669 656c  .        """Fiel
-00005040: 6420 5465 7874 2222 220a 0a20 2020 2040  d Text"""..    @
-00005050: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00005060: 206b 6579 776f 7264 7365 7473 2873 656c   keywordsets(sel
-00005070: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00005080: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
-00005090: 6f6e 7461 696e 6572 732e 4d65 7373 6167  ontainers.Messag
-000050a0: 654d 6170 5b62 7569 6c74 696e 732e 7374  eMap[builtins.st
-000050b0: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
-000050c0: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
-000050d0: 2e46 6965 6c64 4b65 7977 6f72 6473 6574  .FieldKeywordset
-000050e0: 5d3a 0a20 2020 2020 2020 2022 2222 4669  ]:.        """Fi
-000050f0: 656c 6420 6b65 7977 6f72 6422 2222 0a0a  eld keyword"""..
-00005100: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00005110: 2020 6465 6620 6461 7465 7469 6d65 7328    def datetimes(
-00005120: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
-00005130: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
-00005140: 6c2e 636f 6e74 6169 6e65 7273 2e4d 6573  l.containers.Mes
-00005150: 7361 6765 4d61 705b 6275 696c 7469 6e73  sageMap[builtins
-00005160: 2e73 7472 2c20 6e75 636c 6961 6462 5f70  .str, nucliadb_p
-00005170: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
-00005180: 7062 322e 4669 656c 6444 6174 6574 696d  pb2.FieldDatetim
-00005190: 655d 3a0a 2020 2020 2020 2020 2222 2246  e]:.        """F
-000051a0: 6965 6c64 2044 6174 6574 696d 6522 2222  ield Datetime"""
-000051b0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000051c0: 2020 2020 6465 6620 6c69 6e6b 7328 7365      def links(se
-000051d0: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
-000051e0: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-000051f0: 636f 6e74 6169 6e65 7273 2e4d 6573 7361  containers.Messa
-00005200: 6765 4d61 705b 6275 696c 7469 6e73 2e73  geMap[builtins.s
-00005210: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
-00005220: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00005230: 322e 4669 656c 644c 696e 6b5d 3a0a 2020  2.FieldLink]:.  
-00005240: 2020 2020 2020 2222 2246 6965 6c64 204c        """Field L
-00005250: 696e 6b73 2222 220a 0a20 2020 2040 7072  inks"""..    @pr
-00005260: 6f70 6572 7479 0a20 2020 2064 6566 2066  operty.    def f
-00005270: 696c 6573 2873 656c 6629 202d 3e20 676f  iles(self) -> go
-00005280: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-00005290: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-000052a0: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
-000052b0: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-000052c0: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
-000052d0: 7263 6573 5f70 6232 2e46 6965 6c64 4669  rces_pb2.FieldFi
-000052e0: 6c65 5d3a 0a20 2020 2020 2020 2022 2222  le]:.        """
-000052f0: 4669 656c 6420 4669 6c65 2222 220a 0a20  Field File""".. 
-00005300: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00005310: 2064 6566 206c 696e 6b5f 6578 7472 6163   def link_extrac
-00005320: 7465 645f 6461 7461 2873 656c 6629 202d  ted_data(self) -
-00005330: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
-00005340: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
-00005350: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
-00005360: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
-00005370: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
-00005380: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
-00005390: 7062 322e 4c69 6e6b 4578 7472 6163 7465  pb2.LinkExtracte
-000053a0: 6444 6174 615d 3a0a 2020 2020 2020 2020  dData]:.        
-000053b0: 2222 224c 696e 6b20 6578 7472 6163 7465  """Link extracte
-000053c0: 6420 6578 7472 6120 696e 666f 2222 220a  d extra info""".
-000053d0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000053e0: 2020 2064 6566 2066 696c 655f 6578 7472     def file_extr
-000053f0: 6163 7465 645f 6461 7461 2873 656c 6629  acted_data(self)
-00005400: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
-00005410: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
-00005420: 7461 696e 6572 732e 5265 7065 6174 6564  tainers.Repeated
-00005430: 436f 6d70 6f73 6974 6546 6965 6c64 436f  CompositeFieldCo
-00005440: 6e74 6169 6e65 725b 6e75 636c 6961 6462  ntainer[nucliadb
-00005450: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00005460: 735f 7062 322e 4669 6c65 4578 7472 6163  s_pb2.FileExtrac
-00005470: 7465 6444 6174 615d 3a0a 2020 2020 2020  tedData]:.      
-00005480: 2020 2222 2246 696c 6520 6578 7472 6163    """File extrac
-00005490: 7465 6420 6578 7472 6120 696e 666f 2222  ted extra info""
-000054a0: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-000054b0: 0a20 2020 2064 6566 2065 7874 7261 6374  .    def extract
-000054c0: 6564 5f74 6578 7428 7365 6c66 2920 2d3e  ed_text(self) ->
-000054d0: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-000054e0: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-000054f0: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
-00005500: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
-00005510: 696e 6572 5b6e 7563 6c69 6164 625f 7072  iner[nucliadb_pr
-00005520: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00005530: 6232 2e45 7874 7261 6374 6564 5465 7874  b2.ExtractedText
-00005540: 5772 6170 7065 725d 3a0a 2020 2020 2020  Wrapper]:.      
-00005550: 2020 2222 2246 6965 6c64 2045 7874 7261    """Field Extra
-00005560: 6374 6564 2f43 6f6d 7075 7465 6420 696e  cted/Computed in
-00005570: 666f 726d 6174 696f 6e22 2222 0a0a 2020  formation"""..  
-00005580: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00005590: 6465 6620 6669 656c 645f 6d65 7461 6461  def field_metada
-000055a0: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
-000055b0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-000055c0: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-000055d0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
-000055e0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
-000055f0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00005600: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
-00005610: 656c 6443 6f6d 7075 7465 644d 6574 6164  eldComputedMetad
-00005620: 6174 6157 7261 7070 6572 5d3a 202e 2e2e  ataWrapper]: ...
-00005630: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00005640: 2020 2064 6566 2066 6965 6c64 5f76 6563     def field_vec
-00005650: 746f 7273 2873 656c 6629 202d 3e20 676f  tors(self) -> go
-00005660: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-00005670: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-00005680: 732e 5265 7065 6174 6564 436f 6d70 6f73  s.RepeatedCompos
-00005690: 6974 6546 6965 6c64 436f 6e74 6169 6e65  iteFieldContaine
-000056a0: 725b 6e75 636c 6961 6462 5f70 726f 746f  r[nucliadb_proto
-000056b0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-000056c0: 4578 7472 6163 7465 6456 6563 746f 7273  ExtractedVectors
-000056d0: 5772 6170 7065 725d 3a20 2e2e 2e0a 2020  Wrapper]: ....  
-000056e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-000056f0: 6465 6620 6669 656c 645f 6c61 7267 655f  def field_large_
-00005700: 6d65 7461 6461 7461 2873 656c 6629 202d  metadata(self) -
-00005710: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
-00005720: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
-00005730: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
-00005740: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
-00005750: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
-00005760: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
-00005770: 7062 322e 4c61 7267 6543 6f6d 7075 7465  pb2.LargeCompute
-00005780: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
-00005790: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
-000057a0: 736f 7572 6365 204c 6172 6765 2043 6f6d  source Large Com
-000057b0: 7075 7465 6420 4d65 7461 6461 7461 2222  puted Metadata""
-000057c0: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-000057d0: 0a20 2020 2064 6566 2064 656c 6574 655f  .    def delete_
-000057e0: 6669 656c 6473 2873 656c 6629 202d 3e20  fields(self) -> 
-000057f0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00005800: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
-00005810: 6572 732e 5265 7065 6174 6564 436f 6d70  ers.RepeatedComp
-00005820: 6f73 6974 6546 6965 6c64 436f 6e74 6169  ositeFieldContai
-00005830: 6e65 725b 6e75 636c 6961 6462 5f70 726f  ner[nucliadb_pro
-00005840: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00005850: 322e 4669 656c 6449 445d 3a20 2e2e 2e0a  2.FieldID]: ....
-00005860: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00005870: 2020 6465 6620 646f 6e65 5f74 696d 6528    def done_time(
-00005880: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
-00005890: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
-000058a0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
-000058b0: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
-000058c0: 7274 790a 2020 2020 6465 6620 6572 726f  rty.    def erro
-000058d0: 7273 2873 656c 6629 202d 3e20 676f 6f67  rs(self) -> goog
-000058e0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-000058f0: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-00005900: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
-00005910: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
-00005920: 676c 6f62 616c 5f5f 5f45 7272 6f72 5d3a  global___Error]:
-00005930: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
-00005940: 7479 0a20 2020 2064 6566 2075 7365 725f  ty.    def user_
-00005950: 7665 6374 6f72 7328 7365 6c66 2920 2d3e  vectors(self) ->
-00005960: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00005970: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-00005980: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
-00005990: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
-000059a0: 696e 6572 5b6e 7563 6c69 6164 625f 7072  iner[nucliadb_pr
-000059b0: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-000059c0: 6232 2e55 7365 7256 6563 746f 7273 5772  b2.UserVectorsWr
-000059d0: 6170 7065 725d 3a20 2e2e 2e0a 2020 2020  apper]: ....    
-000059e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-000059f0: 6620 6578 7472 6128 7365 6c66 2920 2d3e  f extra(self) ->
-00005a00: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00005a10: 2e72 6573 6f75 7263 6573 5f70 6232 2e45  .resources_pb2.E
-00005a20: 7874 7261 3a20 2e2e 2e0a 2020 2020 4070  xtra: ....    @p
-00005a30: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00005a40: 7175 6573 7469 6f6e 5f61 6e73 7765 7273  question_answers
-00005a50: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
-00005a60: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-00005a70: 616c 2e63 6f6e 7461 696e 6572 732e 5265  al.containers.Re
-00005a80: 7065 6174 6564 436f 6d70 6f73 6974 6546  peatedCompositeF
-00005a90: 6965 6c64 436f 6e74 6169 6e65 725b 6e75  ieldContainer[nu
-00005aa0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-00005ab0: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-00005ac0: 6451 7565 7374 696f 6e41 6e73 7765 7257  dQuestionAnswerW
-00005ad0: 7261 7070 6572 5d3a 202e 2e2e 0a20 2020  rapper]: ....   
-00005ae0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00005af0: 6566 2073 6563 7572 6974 7928 7365 6c66  ef security(self
-00005b00: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-00005b10: 6f74 6f73 2e75 7469 6c73 5f70 6232 2e53  otos.utils_pb2.S
-00005b20: 6563 7572 6974 793a 202e 2e2e 0a20 2020  ecurity: ....   
-00005b30: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00005b40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00005b50: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00005b60: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
-00005b70: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
-00005b80: 2020 7575 6964 3a20 6275 696c 7469 6e73    uuid: builtins
-00005b90: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00005ba0: 2020 2020 736c 7567 3a20 6275 696c 7469      slug: builti
-00005bb0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00005bc0: 2020 2020 2020 6175 6469 743a 2067 6c6f        audit: glo
-00005bd0: 6261 6c5f 5f5f 4175 6469 7420 7c20 4e6f  bal___Audit | No
-00005be0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00005bf0: 2020 7479 7065 3a20 676c 6f62 616c 5f5f    type: global__
-00005c00: 5f42 726f 6b65 724d 6573 7361 6765 2e4d  _BrokerMessage.M
-00005c10: 6573 7361 6765 5479 7065 2e56 616c 7565  essageType.Value
-00005c20: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-00005c30: 2020 2020 6d75 6c74 6969 643a 2062 7569      multiid: bui
-00005c40: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00005c50: 0a20 2020 2020 2020 2062 6173 6963 3a20  .        basic: 
-00005c60: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00005c70: 7265 736f 7572 6365 735f 7062 322e 4261  resources_pb2.Ba
-00005c80: 7369 6320 7c20 4e6f 6e65 203d 202e 2e2e  sic | None = ...
-00005c90: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
-00005ca0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-00005cb0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-00005cc0: 4f72 6967 696e 207c 204e 6f6e 6520 3d20  Origin | None = 
-00005cd0: 2e2e 2e2c 0a20 2020 2020 2020 2072 656c  ...,.        rel
-00005ce0: 6174 696f 6e73 3a20 636f 6c6c 6563 7469  ations: collecti
-00005cf0: 6f6e 732e 6162 632e 4974 6572 6162 6c65  ons.abc.Iterable
-00005d00: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
-00005d10: 2e75 7469 6c73 5f70 6232 2e52 656c 6174  .utils_pb2.Relat
-00005d20: 696f 6e5d 207c 204e 6f6e 6520 3d20 2e2e  ion] | None = ..
-00005d30: 2e2c 0a20 2020 2020 2020 2063 6f6e 7665  .,.        conve
-00005d40: 7273 6174 696f 6e73 3a20 636f 6c6c 6563  rsations: collec
-00005d50: 7469 6f6e 732e 6162 632e 4d61 7070 696e  tions.abc.Mappin
-00005d60: 675b 6275 696c 7469 6e73 2e73 7472 2c20  g[builtins.str, 
-00005d70: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00005d80: 7265 736f 7572 6365 735f 7062 322e 436f  resources_pb2.Co
-00005d90: 6e76 6572 7361 7469 6f6e 5d20 7c20 4e6f  nversation] | No
-00005da0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00005db0: 2020 6c61 796f 7574 733a 2063 6f6c 6c65    layouts: colle
-00005dc0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-00005dd0: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-00005de0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00005df0: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00005e00: 6965 6c64 4c61 796f 7574 5d20 7c20 4e6f  ieldLayout] | No
-00005e10: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00005e20: 2020 7465 7874 733a 2063 6f6c 6c65 6374    texts: collect
-00005e30: 696f 6e73 2e61 6263 2e4d 6170 7069 6e67  ions.abc.Mapping
-00005e40: 5b62 7569 6c74 696e 732e 7374 722c 206e  [builtins.str, n
-00005e50: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00005e60: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
-00005e70: 6c64 5465 7874 5d20 7c20 4e6f 6e65 203d  ldText] | None =
-00005e80: 202e 2e2e 2c0a 2020 2020 2020 2020 6b65   ...,.        ke
-00005e90: 7977 6f72 6473 6574 733a 2063 6f6c 6c65  ywordsets: colle
-00005ea0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-00005eb0: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-00005ec0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00005ed0: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00005ee0: 6965 6c64 4b65 7977 6f72 6473 6574 5d20  ieldKeywordset] 
-00005ef0: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00005f00: 2020 2020 2020 6461 7465 7469 6d65 733a        datetimes:
-00005f10: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00005f20: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
-00005f30: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
-00005f40: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00005f50: 5f70 6232 2e46 6965 6c64 4461 7465 7469  _pb2.FieldDateti
-00005f60: 6d65 5d20 7c20 4e6f 6e65 203d 202e 2e2e  me] | None = ...
-00005f70: 2c0a 2020 2020 2020 2020 6c69 6e6b 733a  ,.        links:
-00005f80: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00005f90: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
-00005fa0: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
-00005fb0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00005fc0: 5f70 6232 2e46 6965 6c64 4c69 6e6b 5d20  _pb2.FieldLink] 
-00005fd0: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00005fe0: 2020 2020 2020 6669 6c65 733a 2063 6f6c        files: col
-00005ff0: 6c65 6374 696f 6e73 2e61 6263 2e4d 6170  lections.abc.Map
-00006000: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
-00006010: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
-00006020: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
-00006030: 2e46 6965 6c64 4669 6c65 5d20 7c20 4e6f  .FieldFile] | No
-00006040: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00006050: 2020 6c69 6e6b 5f65 7874 7261 6374 6564    link_extracted
-00006060: 5f64 6174 613a 2063 6f6c 6c65 6374 696f  _data: collectio
-00006070: 6e73 2e61 6263 2e49 7465 7261 626c 655b  ns.abc.Iterable[
-00006080: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00006090: 7265 736f 7572 6365 735f 7062 322e 4c69  resources_pb2.Li
-000060a0: 6e6b 4578 7472 6163 7465 6444 6174 615d  nkExtractedData]
-000060b0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-000060c0: 2020 2020 2020 2066 696c 655f 6578 7472         file_extr
-000060d0: 6163 7465 645f 6461 7461 3a20 636f 6c6c  acted_data: coll
-000060e0: 6563 7469 6f6e 732e 6162 632e 4974 6572  ections.abc.Iter
-000060f0: 6162 6c65 5b6e 7563 6c69 6164 625f 7072  able[nucliadb_pr
-00006100: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00006110: 6232 2e46 696c 6545 7874 7261 6374 6564  b2.FileExtracted
-00006120: 4461 7461 5d20 7c20 4e6f 6e65 203d 202e  Data] | None = .
-00006130: 2e2e 2c0a 2020 2020 2020 2020 6578 7472  ..,.        extr
-00006140: 6163 7465 645f 7465 7874 3a20 636f 6c6c  acted_text: coll
-00006150: 6563 7469 6f6e 732e 6162 632e 4974 6572  ections.abc.Iter
-00006160: 6162 6c65 5b6e 7563 6c69 6164 625f 7072  able[nucliadb_pr
-00006170: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00006180: 6232 2e45 7874 7261 6374 6564 5465 7874  b2.ExtractedText
-00006190: 5772 6170 7065 725d 207c 204e 6f6e 6520  Wrapper] | None 
-000061a0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2066  = ...,.        f
-000061b0: 6965 6c64 5f6d 6574 6164 6174 613a 2063  ield_metadata: c
-000061c0: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
-000061d0: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
-000061e0: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-000061f0: 735f 7062 322e 4669 656c 6443 6f6d 7075  s_pb2.FieldCompu
-00006200: 7465 644d 6574 6164 6174 6157 7261 7070  tedMetadataWrapp
-00006210: 6572 5d20 7c20 4e6f 6e65 203d 202e 2e2e  er] | None = ...
-00006220: 2c0a 2020 2020 2020 2020 6669 656c 645f  ,.        field_
-00006230: 7665 6374 6f72 733a 2063 6f6c 6c65 6374  vectors: collect
-00006240: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
-00006250: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
-00006260: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-00006270: 4578 7472 6163 7465 6456 6563 746f 7273  ExtractedVectors
-00006280: 5772 6170 7065 725d 207c 204e 6f6e 6520  Wrapper] | None 
-00006290: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2066  = ...,.        f
-000062a0: 6965 6c64 5f6c 6172 6765 5f6d 6574 6164  ield_large_metad
-000062b0: 6174 613a 2063 6f6c 6c65 6374 696f 6e73  ata: collections
-000062c0: 2e61 6263 2e49 7465 7261 626c 655b 6e75  .abc.Iterable[nu
-000062d0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-000062e0: 736f 7572 6365 735f 7062 322e 4c61 7267  sources_pb2.Larg
-000062f0: 6543 6f6d 7075 7465 644d 6574 6164 6174  eComputedMetadat
-00006300: 6157 7261 7070 6572 5d20 7c20 4e6f 6e65  aWrapper] | None
-00006310: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00006320: 6465 6c65 7465 5f66 6965 6c64 733a 2063  delete_fields: c
-00006330: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
-00006340: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
-00006350: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00006360: 735f 7062 322e 4669 656c 6449 445d 207c  s_pb2.FieldID] |
-00006370: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-00006380: 2020 2020 206f 7269 6769 6e5f 7365 713a       origin_seq:
-00006390: 2062 7569 6c74 696e 732e 696e 7420 3d20   builtins.int = 
-000063a0: 2e2e 2e2c 0a20 2020 2020 2020 2073 6c6f  ...,.        slo
-000063b0: 775f 7072 6f63 6573 7369 6e67 5f74 696d  w_processing_tim
-000063c0: 653a 2062 7569 6c74 696e 732e 666c 6f61  e: builtins.floa
-000063d0: 7420 3d20 2e2e 2e2c 0a20 2020 2020 2020  t = ...,.       
-000063e0: 2070 7265 5f70 726f 6365 7373 696e 675f   pre_processing_
-000063f0: 7469 6d65 3a20 6275 696c 7469 6e73 2e66  time: builtins.f
-00006400: 6c6f 6174 203d 202e 2e2e 2c0a 2020 2020  loat = ...,.    
-00006410: 2020 2020 646f 6e65 5f74 696d 653a 2067      done_time: g
-00006420: 6f6f 676c 652e 7072 6f74 6f62 7566 2e74  oogle.protobuf.t
-00006430: 696d 6573 7461 6d70 5f70 6232 2e54 696d  imestamp_pb2.Tim
-00006440: 6573 7461 6d70 207c 204e 6f6e 6520 3d20  estamp | None = 
-00006450: 2e2e 2e2c 0a20 2020 2020 2020 2074 7873  ...,.        txs
-00006460: 6571 6964 3a20 6275 696c 7469 6e73 2e69  eqid: builtins.i
-00006470: 6e74 203d 202e 2e2e 2c0a 2020 2020 2020  nt = ...,.      
-00006480: 2020 6572 726f 7273 3a20 636f 6c6c 6563    errors: collec
-00006490: 7469 6f6e 732e 6162 632e 4974 6572 6162  tions.abc.Iterab
-000064a0: 6c65 5b67 6c6f 6261 6c5f 5f5f 4572 726f  le[global___Erro
-000064b0: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
-000064c0: 0a20 2020 2020 2020 2070 726f 6365 7373  .        process
-000064d0: 696e 675f 6964 3a20 6275 696c 7469 6e73  ing_id: builtins
-000064e0: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-000064f0: 2020 2020 736f 7572 6365 3a20 676c 6f62      source: glob
-00006500: 616c 5f5f 5f42 726f 6b65 724d 6573 7361  al___BrokerMessa
-00006510: 6765 2e4d 6573 7361 6765 536f 7572 6365  ge.MessageSource
-00006520: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
-00006530: 2c0a 2020 2020 2020 2020 6163 636f 756e  ,.        accoun
-00006540: 745f 7365 713a 2062 7569 6c74 696e 732e  t_seq: builtins.
-00006550: 696e 7420 3d20 2e2e 2e2c 0a20 2020 2020  int = ...,.     
-00006560: 2020 2075 7365 725f 7665 6374 6f72 733a     user_vectors:
-00006570: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00006580: 2e49 7465 7261 626c 655b 6e75 636c 6961  .Iterable[nuclia
-00006590: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-000065a0: 6365 735f 7062 322e 5573 6572 5665 6374  ces_pb2.UserVect
-000065b0: 6f72 7357 7261 7070 6572 5d20 7c20 4e6f  orsWrapper] | No
-000065c0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-000065d0: 2020 7265 696e 6465 783a 2062 7569 6c74    reindex: built
-000065e0: 696e 732e 626f 6f6c 203d 202e 2e2e 2c0a  ins.bool = ...,.
-000065f0: 2020 2020 2020 2020 6578 7472 613a 206e          extra: n
-00006600: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00006610: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
-00006620: 7261 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ra | None = ...,
-00006630: 0a20 2020 2020 2020 2071 7565 7374 696f  .        questio
-00006640: 6e5f 616e 7377 6572 733a 2063 6f6c 6c65  n_answers: colle
-00006650: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
-00006660: 626c 655b 6e75 636c 6961 6462 5f70 726f  ble[nucliadb_pro
-00006670: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00006680: 322e 4669 656c 6451 7565 7374 696f 6e41  2.FieldQuestionA
-00006690: 6e73 7765 7257 7261 7070 6572 5d20 7c20  nswerWrapper] | 
-000066a0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-000066b0: 2020 2020 7365 6375 7269 7479 3a20 6e75      security: nu
-000066c0: 636c 6961 6462 5f70 726f 746f 732e 7574  cliadb_protos.ut
-000066d0: 696c 735f 7062 322e 5365 6375 7269 7479  ils_pb2.Security
-000066e0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-000066f0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-00006700: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
-00006710: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-00006720: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-00006730: 7261 6c5b 2261 7564 6974 222c 2062 2261  ral["audit", b"a
-00006740: 7564 6974 222c 2022 6261 7369 6322 2c20  udit", "basic", 
-00006750: 6222 6261 7369 6322 2c20 2264 6f6e 655f  b"basic", "done_
-00006760: 7469 6d65 222c 2062 2264 6f6e 655f 7469  time", b"done_ti
-00006770: 6d65 222c 2022 6578 7472 6122 2c20 6222  me", "extra", b"
-00006780: 6578 7472 6122 2c20 226f 7269 6769 6e22  extra", "origin"
-00006790: 2c20 6222 6f72 6967 696e 222c 2022 7365  , b"origin", "se
-000067a0: 6375 7269 7479 222c 2062 2273 6563 7572  curity", b"secur
-000067b0: 6974 7922 5d29 202d 3e20 6275 696c 7469  ity"]) -> builti
-000067c0: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
-000067d0: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
-000067e0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-000067f0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-00006800: 5b22 6163 636f 756e 745f 7365 7122 2c20  ["account_seq", 
-00006810: 6222 6163 636f 756e 745f 7365 7122 2c20  b"account_seq", 
-00006820: 2261 7564 6974 222c 2062 2261 7564 6974  "audit", b"audit
-00006830: 222c 2022 6261 7369 6322 2c20 6222 6261  ", "basic", b"ba
-00006840: 7369 6322 2c20 2263 6f6e 7665 7273 6174  sic", "conversat
-00006850: 696f 6e73 222c 2062 2263 6f6e 7665 7273  ions", b"convers
-00006860: 6174 696f 6e73 222c 2022 6461 7465 7469  ations", "dateti
-00006870: 6d65 7322 2c20 6222 6461 7465 7469 6d65  mes", b"datetime
-00006880: 7322 2c20 2264 656c 6574 655f 6669 656c  s", "delete_fiel
-00006890: 6473 222c 2062 2264 656c 6574 655f 6669  ds", b"delete_fi
-000068a0: 656c 6473 222c 2022 646f 6e65 5f74 696d  elds", "done_tim
-000068b0: 6522 2c20 6222 646f 6e65 5f74 696d 6522  e", b"done_time"
-000068c0: 2c20 2265 7272 6f72 7322 2c20 6222 6572  , "errors", b"er
-000068d0: 726f 7273 222c 2022 6578 7472 6122 2c20  rors", "extra", 
-000068e0: 6222 6578 7472 6122 2c20 2265 7874 7261  b"extra", "extra
-000068f0: 6374 6564 5f74 6578 7422 2c20 6222 6578  cted_text", b"ex
-00006900: 7472 6163 7465 645f 7465 7874 222c 2022  tracted_text", "
-00006910: 6669 656c 645f 6c61 7267 655f 6d65 7461  field_large_meta
-00006920: 6461 7461 222c 2062 2266 6965 6c64 5f6c  data", b"field_l
-00006930: 6172 6765 5f6d 6574 6164 6174 6122 2c20  arge_metadata", 
-00006940: 2266 6965 6c64 5f6d 6574 6164 6174 6122  "field_metadata"
-00006950: 2c20 6222 6669 656c 645f 6d65 7461 6461  , b"field_metada
-00006960: 7461 222c 2022 6669 656c 645f 7665 6374  ta", "field_vect
-00006970: 6f72 7322 2c20 6222 6669 656c 645f 7665  ors", b"field_ve
-00006980: 6374 6f72 7322 2c20 2266 696c 655f 6578  ctors", "file_ex
-00006990: 7472 6163 7465 645f 6461 7461 222c 2062  tracted_data", b
-000069a0: 2266 696c 655f 6578 7472 6163 7465 645f  "file_extracted_
-000069b0: 6461 7461 222c 2022 6669 6c65 7322 2c20  data", "files", 
-000069c0: 6222 6669 6c65 7322 2c20 226b 6269 6422  b"files", "kbid"
-000069d0: 2c20 6222 6b62 6964 222c 2022 6b65 7977  , b"kbid", "keyw
-000069e0: 6f72 6473 6574 7322 2c20 6222 6b65 7977  ordsets", b"keyw
-000069f0: 6f72 6473 6574 7322 2c20 226c 6179 6f75  ordsets", "layou
-00006a00: 7473 222c 2062 226c 6179 6f75 7473 222c  ts", b"layouts",
-00006a10: 2022 6c69 6e6b 5f65 7874 7261 6374 6564   "link_extracted
-00006a20: 5f64 6174 6122 2c20 6222 6c69 6e6b 5f65  _data", b"link_e
-00006a30: 7874 7261 6374 6564 5f64 6174 6122 2c20  xtracted_data", 
-00006a40: 226c 696e 6b73 222c 2062 226c 696e 6b73  "links", b"links
-00006a50: 222c 2022 6d75 6c74 6969 6422 2c20 6222  ", "multiid", b"
-00006a60: 6d75 6c74 6969 6422 2c20 226f 7269 6769  multiid", "origi
-00006a70: 6e22 2c20 6222 6f72 6967 696e 222c 2022  n", b"origin", "
-00006a80: 6f72 6967 696e 5f73 6571 222c 2062 226f  origin_seq", b"o
-00006a90: 7269 6769 6e5f 7365 7122 2c20 2270 7265  rigin_seq", "pre
-00006aa0: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
-00006ab0: 222c 2062 2270 7265 5f70 726f 6365 7373  ", b"pre_process
-00006ac0: 696e 675f 7469 6d65 222c 2022 7072 6f63  ing_time", "proc
-00006ad0: 6573 7369 6e67 5f69 6422 2c20 6222 7072  essing_id", b"pr
-00006ae0: 6f63 6573 7369 6e67 5f69 6422 2c20 2271  ocessing_id", "q
-00006af0: 7565 7374 696f 6e5f 616e 7377 6572 7322  uestion_answers"
-00006b00: 2c20 6222 7175 6573 7469 6f6e 5f61 6e73  , b"question_ans
-00006b10: 7765 7273 222c 2022 7265 696e 6465 7822  wers", "reindex"
-00006b20: 2c20 6222 7265 696e 6465 7822 2c20 2272  , b"reindex", "r
-00006b30: 656c 6174 696f 6e73 222c 2062 2272 656c  elations", b"rel
-00006b40: 6174 696f 6e73 222c 2022 7365 6375 7269  ations", "securi
-00006b50: 7479 222c 2062 2273 6563 7572 6974 7922  ty", b"security"
-00006b60: 2c20 2273 6c6f 775f 7072 6f63 6573 7369  , "slow_processi
-00006b70: 6e67 5f74 696d 6522 2c20 6222 736c 6f77  ng_time", b"slow
-00006b80: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
-00006b90: 222c 2022 736c 7567 222c 2062 2273 6c75  ", "slug", b"slu
-00006ba0: 6722 2c20 2273 6f75 7263 6522 2c20 6222  g", "source", b"
-00006bb0: 736f 7572 6365 222c 2022 7465 7874 7322  source", "texts"
-00006bc0: 2c20 6222 7465 7874 7322 2c20 2274 7873  , b"texts", "txs
-00006bd0: 6571 6964 222c 2062 2274 7873 6571 6964  eqid", b"txseqid
-00006be0: 222c 2022 7479 7065 222c 2062 2274 7970  ", "type", b"typ
-00006bf0: 6522 2c20 2275 7365 725f 7665 6374 6f72  e", "user_vector
-00006c00: 7322 2c20 6222 7573 6572 5f76 6563 746f  s", b"user_vecto
-00006c10: 7273 222c 2022 7575 6964 222c 2062 2275  rs", "uuid", b"u
-00006c20: 7569 6422 5d29 202d 3e20 4e6f 6e65 3a20  uid"]) -> None: 
-00006c30: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4272  .....global___Br
-00006c40: 6f6b 6572 4d65 7373 6167 6520 3d20 4272  okerMessage = Br
-00006c50: 6f6b 6572 4d65 7373 6167 650a 0a40 7479  okerMessage..@ty
-00006c60: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00006c70: 2042 726f 6b65 724d 6573 7361 6765 426c   BrokerMessageBl
-00006c80: 6f62 5265 6665 7265 6e63 6528 676f 6f67  obReference(goog
-00006c90: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-00006ca0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-00006cb0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00006cc0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00006cd0: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-00006ce0: 746f 720a 0a20 2020 204b 4249 445f 4649  tor..    KBID_FI
-00006cf0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00006d00: 7469 6e73 2e69 6e74 0a20 2020 2055 5549  tins.int.    UUI
-00006d10: 445f 4649 454c 445f 4e55 4d42 4552 3a20  D_FIELD_NUMBER: 
-00006d20: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00006d30: 2053 544f 5241 4745 5f4b 4559 5f46 4945   STORAGE_KEY_FIE
-00006d40: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00006d50: 696e 732e 696e 740a 2020 2020 6b62 6964  ins.int.    kbid
-00006d60: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-00006d70: 2020 2075 7569 643a 2062 7569 6c74 696e     uuid: builtin
-00006d80: 732e 7374 720a 2020 2020 7374 6f72 6167  s.str.    storag
-00006d90: 655f 6b65 793a 2062 7569 6c74 696e 732e  e_key: builtins.
-00006da0: 7374 720a 2020 2020 6465 6620 5f5f 696e  str.    def __in
-00006db0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00006dc0: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
-00006dd0: 2020 2020 2020 206b 6269 643a 2062 7569         kbid: bui
-00006de0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00006df0: 0a20 2020 2020 2020 2075 7569 643a 2062  .        uuid: b
-00006e00: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00006e10: 2e2c 0a20 2020 2020 2020 2073 746f 7261  .,.        stora
-00006e20: 6765 5f6b 6579 3a20 6275 696c 7469 6e73  ge_key: builtins
-00006e30: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00006e40: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00006e50: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-00006e60: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00006e70: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00006e80: 616c 5b22 6b62 6964 222c 2062 226b 6269  al["kbid", b"kbi
-00006e90: 6422 2c20 2273 746f 7261 6765 5f6b 6579  d", "storage_key
-00006ea0: 222c 2062 2273 746f 7261 6765 5f6b 6579  ", b"storage_key
-00006eb0: 222c 2022 7575 6964 222c 2062 2275 7569  ", "uuid", b"uui
-00006ec0: 6422 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  d"]) -> None: ..
-00006ed0: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4272 6f6b  ...global___Brok
-00006ee0: 6572 4d65 7373 6167 6542 6c6f 6252 6566  erMessageBlobRef
-00006ef0: 6572 656e 6365 203d 2042 726f 6b65 724d  erence = BrokerM
-00006f00: 6573 7361 6765 426c 6f62 5265 6665 7265  essageBlobRefere
-00006f10: 6e63 650a 0a40 7479 7069 6e67 2e66 696e  nce..@typing.fin
-00006f20: 616c 0a63 6c61 7373 2057 7269 7465 7253  al.class WriterS
-00006f30: 7461 7475 7352 6573 706f 6e73 6528 676f  tatusResponse(go
-00006f40: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00006f50: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-00006f60: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00006f70: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00006f80: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-00006f90: 6970 746f 720a 0a20 2020 2040 7479 7069  iptor..    @typi
-00006fa0: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
-00006fb0: 7373 204d 7367 6964 456e 7472 7928 676f  ss MsgidEntry(go
-00006fc0: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00006fd0: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-00006fe0: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-00006ff0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00007000: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00007010: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
-00007020: 2020 204b 4559 5f46 4945 4c44 5f4e 554d     KEY_FIELD_NUM
-00007030: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00007040: 740a 2020 2020 2020 2020 5641 4c55 455f  t.        VALUE_
-00007050: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00007060: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
-00007070: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
-00007080: 2e73 7472 0a20 2020 2020 2020 2076 616c  .str.        val
-00007090: 7565 3a20 6275 696c 7469 6e73 2e69 6e74  ue: builtins.int
-000070a0: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
-000070b0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-000070c0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000070d0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-000070e0: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
-000070f0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00007100: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
-00007110: 6275 696c 7469 6e73 2e69 6e74 203d 202e  builtins.int = .
-00007120: 2e2e 2c0a 2020 2020 2020 2020 2920 2d3e  ..,.        ) ->
-00007130: 204e 6f6e 653a 202e 2e2e 0a20 2020 2020   None: ....     
-00007140: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-00007150: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00007160: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00007170: 616c 5b22 6b65 7922 2c20 6222 6b65 7922  al["key", b"key"
-00007180: 2c20 2276 616c 7565 222c 2062 2276 616c  , "value", b"val
-00007190: 7565 225d 2920 2d3e 204e 6f6e 653a 202e  ue"]) -> None: .
-000071a0: 2e2e 0a0a 2020 2020 4b4e 4f57 4c45 4447  ....    KNOWLEDG
-000071b0: 4542 4f58 4553 5f46 4945 4c44 5f4e 554d  EBOXES_FIELD_NUM
-000071c0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-000071d0: 740a 2020 2020 4d53 4749 445f 4649 454c  t.    MSGID_FIEL
-000071e0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-000071f0: 6e73 2e69 6e74 0a20 2020 2040 7072 6f70  ns.int.    @prop
-00007200: 6572 7479 0a20 2020 2064 6566 206b 6e6f  erty.    def kno
-00007210: 776c 6564 6765 626f 7865 7328 7365 6c66  wledgeboxes(self
-00007220: 2920 2d3e 2067 6f6f 676c 652e 7072 6f74  ) -> google.prot
-00007230: 6f62 7566 2e69 6e74 6572 6e61 6c2e 636f  obuf.internal.co
-00007240: 6e74 6169 6e65 7273 2e52 6570 6561 7465  ntainers.Repeate
-00007250: 6453 6361 6c61 7246 6965 6c64 436f 6e74  dScalarFieldCont
-00007260: 6169 6e65 725b 6275 696c 7469 6e73 2e73  ainer[builtins.s
-00007270: 7472 5d3a 202e 2e2e 0a20 2020 2040 7072  tr]: ....    @pr
-00007280: 6f70 6572 7479 0a20 2020 2064 6566 206d  operty.    def m
-00007290: 7367 6964 2873 656c 6629 202d 3e20 676f  sgid(self) -> go
-000072a0: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-000072b0: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-000072c0: 732e 5363 616c 6172 4d61 705b 6275 696c  s.ScalarMap[buil
-000072d0: 7469 6e73 2e73 7472 2c20 6275 696c 7469  tins.str, builti
-000072e0: 6e73 2e69 6e74 5d3a 0a20 2020 2020 2020  ns.int]:.       
-000072f0: 2022 2222 6d61 7020 6f66 206c 6173 7420   """map of last 
-00007300: 6d65 7373 6167 6520 7072 6f63 6573 7365  message processe
-00007310: 6422 2222 0a0a 2020 2020 6465 6620 5f5f  d"""..    def __
-00007320: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00007330: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00007340: 0a20 2020 2020 2020 206b 6e6f 776c 6564  .        knowled
-00007350: 6765 626f 7865 733a 2063 6f6c 6c65 6374  geboxes: collect
-00007360: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
-00007370: 655b 6275 696c 7469 6e73 2e73 7472 5d20  e[builtins.str] 
-00007380: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00007390: 2020 2020 2020 6d73 6769 643a 2063 6f6c        msgid: col
-000073a0: 6c65 6374 696f 6e73 2e61 6263 2e4d 6170  lections.abc.Map
-000073b0: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
-000073c0: 722c 2062 7569 6c74 696e 732e 696e 745d  r, builtins.int]
-000073d0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-000073e0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-000073f0: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-00007400: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00007410: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00007420: 7465 7261 6c5b 226b 6e6f 776c 6564 6765  teral["knowledge
-00007430: 626f 7865 7322 2c20 6222 6b6e 6f77 6c65  boxes", b"knowle
-00007440: 6467 6562 6f78 6573 222c 2022 6d73 6769  dgeboxes", "msgi
-00007450: 6422 2c20 6222 6d73 6769 6422 5d29 202d  d", b"msgid"]) -
-00007460: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
-00007470: 6261 6c5f 5f5f 5772 6974 6572 5374 6174  bal___WriterStat
-00007480: 7573 5265 7370 6f6e 7365 203d 2057 7269  usResponse = Wri
-00007490: 7465 7253 7461 7475 7352 6573 706f 6e73  terStatusRespons
-000074a0: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
-000074b0: 0a63 6c61 7373 2057 7269 7465 7253 7461  .class WriterSta
-000074c0: 7475 7352 6571 7565 7374 2867 6f6f 676c  tusRequest(googl
-000074d0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-000074e0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-000074f0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00007500: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00007510: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00007520: 6f72 0a0a 2020 2020 6465 6620 5f5f 696e  or..    def __in
-00007530: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00007540: 6c66 2c0a 2020 2020 2920 2d3e 204e 6f6e  lf,.    ) -> Non
-00007550: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-00007560: 5f57 7269 7465 7253 7461 7475 7352 6571  _WriterStatusReq
-00007570: 7565 7374 203d 2057 7269 7465 7253 7461  uest = WriterSta
-00007580: 7475 7352 6571 7565 7374 0a0a 4074 7970  tusRequest..@typ
-00007590: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000075a0: 5365 744c 6162 656c 7352 6571 7565 7374  SetLabelsRequest
-000075b0: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-000075c0: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-000075d0: 293a 0a20 2020 2044 4553 4352 4950 544f  ):.    DESCRIPTO
-000075e0: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-000075f0: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-00007600: 7363 7269 7074 6f72 0a0a 2020 2020 4b42  scriptor..    KB
-00007610: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00007620: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00007630: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
-00007640: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00007650: 2020 4c41 4245 4c53 4554 5f46 4945 4c44    LABELSET_FIELD
-00007660: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00007670: 732e 696e 740a 2020 2020 6964 3a20 6275  s.int.    id: bu
-00007680: 696c 7469 6e73 2e73 7472 0a20 2020 2040  iltins.str.    @
-00007690: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000076a0: 206b 6228 7365 6c66 2920 2d3e 206e 7563   kb(self) -> nuc
-000076b0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-000076c0: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-000076d0: 6f77 6c65 6467 6542 6f78 4944 3a20 2e2e  owledgeBoxID: ..
-000076e0: 2e0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000076f0: 2020 2020 6465 6620 6c61 6265 6c73 6574      def labelset
-00007700: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-00007710: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-00007720: 6467 6562 6f78 5f70 6232 2e4c 6162 656c  dgebox_pb2.Label
-00007730: 5365 743a 202e 2e2e 0a20 2020 2064 6566  Set: ....    def
-00007740: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00007750: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00007760: 202a 2c0a 2020 2020 2020 2020 6b62 3a20   *,.        kb: 
-00007770: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00007780: 6b6e 6f77 6c65 6467 6562 6f78 5f70 6232  knowledgebox_pb2
-00007790: 2e4b 6e6f 776c 6564 6765 426f 7849 4420  .KnowledgeBoxID 
-000077a0: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-000077b0: 2020 2020 2020 6964 3a20 6275 696c 7469        id: builti
-000077c0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-000077d0: 2020 2020 2020 6c61 6265 6c73 6574 3a20        labelset: 
-000077e0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000077f0: 6b6e 6f77 6c65 6467 6562 6f78 5f70 6232  knowledgebox_pb2
-00007800: 2e4c 6162 656c 5365 7420 7c20 4e6f 6e65  .LabelSet | None
-00007810: 203d 202e 2e2e 2c0a 2020 2020 2920 2d3e   = ...,.    ) ->
-00007820: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
-00007830: 6566 2048 6173 4669 656c 6428 7365 6c66  ef HasField(self
-00007840: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00007850: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
-00007860: 222c 2062 226b 6222 2c20 226c 6162 656c  ", b"kb", "label
-00007870: 7365 7422 2c20 6222 6c61 6265 6c73 6574  set", b"labelset
-00007880: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
-00007890: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 6465  bool: ....    de
-000078a0: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-000078b0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-000078c0: 7970 696e 672e 4c69 7465 7261 6c5b 2269  yping.Literal["i
-000078d0: 6422 2c20 6222 6964 222c 2022 6b62 222c  d", b"id", "kb",
-000078e0: 2062 226b 6222 2c20 226c 6162 656c 7365   b"kb", "labelse
-000078f0: 7422 2c20 6222 6c61 6265 6c73 6574 225d  t", b"labelset"]
-00007900: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00007910: 676c 6f62 616c 5f5f 5f53 6574 4c61 6265  global___SetLabe
-00007920: 6c73 5265 7175 6573 7420 3d20 5365 744c  lsRequest = SetL
-00007930: 6162 656c 7352 6571 7565 7374 0a0a 4074  abelsRequest..@t
-00007940: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
-00007950: 7320 4465 6c4c 6162 656c 7352 6571 7565  s DelLabelsReque
-00007960: 7374 2867 6f6f 676c 652e 7072 6f74 6f62  st(google.protob
-00007970: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00007980: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00007990: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-000079a0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-000079b0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-000079c0: 4b42 5f46 4945 4c44 5f4e 554d 4245 523a  KB_FIELD_NUMBER:
-000079d0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000079e0: 2020 4944 5f46 4945 4c44 5f4e 554d 4245    ID_FIELD_NUMBE
-000079f0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00007a00: 2020 2020 6964 3a20 6275 696c 7469 6e73      id: builtins
-00007a10: 2e73 7472 0a20 2020 2040 7072 6f70 6572  .str.    @proper
-00007a20: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
-00007a30: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-00007a40: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-00007a50: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-00007a60: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
-00007a70: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00007a80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00007a90: 2020 2020 2a2c 0a20 2020 2020 2020 206b      *,.        k
-00007aa0: 623a 206e 7563 6c69 6164 625f 7072 6f74  b: nucliadb_prot
-00007ab0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-00007ac0: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
-00007ad0: 4944 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ID | None = ...,
-00007ae0: 0a20 2020 2020 2020 2069 643a 2062 7569  .        id: bui
-00007af0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00007b00: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
-00007b10: 2e2e 2e0a 2020 2020 6465 6620 4861 7346  ....    def HasF
-00007b20: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00007b30: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00007b40: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
-00007b50: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
-00007b60: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 6465  bool: ....    de
-00007b70: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-00007b80: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00007b90: 7970 696e 672e 4c69 7465 7261 6c5b 2269  yping.Literal["i
-00007ba0: 6422 2c20 6222 6964 222c 2022 6b62 222c  d", b"id", "kb",
-00007bb0: 2062 226b 6222 5d29 202d 3e20 4e6f 6e65   b"kb"]) -> None
-00007bc0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-00007bd0: 4465 6c4c 6162 656c 7352 6571 7565 7374  DelLabelsRequest
-00007be0: 203d 2044 656c 4c61 6265 6c73 5265 7175   = DelLabelsRequ
-00007bf0: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
-00007c00: 616c 0a63 6c61 7373 2047 6574 4c61 6265  al.class GetLabe
-00007c10: 6c73 5265 7370 6f6e 7365 2867 6f6f 676c  lsResponse(googl
-00007c20: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00007c30: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00007c40: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00007c50: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00007c60: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00007c70: 6f72 0a0a 2020 2020 636c 6173 7320 5f53  or..    class _S
-00007c80: 7461 7475 733a 0a20 2020 2020 2020 2056  tatus:.        V
-00007c90: 616c 7565 5479 7065 203d 2074 7970 696e  alueType = typin
-00007ca0: 672e 4e65 7754 7970 6528 2256 616c 7565  g.NewType("Value
-00007cb0: 5479 7065 222c 2062 7569 6c74 696e 732e  Type", builtins.
-00007cc0: 696e 7429 0a20 2020 2020 2020 2056 3a20  int).        V: 
-00007cd0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
-00007ce0: 732e 5479 7065 416c 6961 7320 3d20 5661  s.TypeAlias = Va
-00007cf0: 6c75 6554 7970 650a 0a20 2020 2063 6c61  lueType..    cla
-00007d00: 7373 205f 5374 6174 7573 456e 756d 5479  ss _StatusEnumTy
-00007d10: 7065 5772 6170 7065 7228 676f 6f67 6c65  peWrapper(google
-00007d20: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-00007d30: 616c 2e65 6e75 6d5f 7479 7065 5f77 7261  al.enum_type_wra
-00007d40: 7070 6572 2e5f 456e 756d 5479 7065 5772  pper._EnumTypeWr
-00007d50: 6170 7065 725b 4765 744c 6162 656c 7352  apper[GetLabelsR
-00007d60: 6573 706f 6e73 652e 5f53 7461 7475 732e  esponse._Status.
-00007d70: 5661 6c75 6554 7970 655d 2c20 6275 696c  ValueType], buil
-00007d80: 7469 6e73 2e74 7970 6529 3a0a 2020 2020  tins.type):.    
-00007d90: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00007da0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00007db0: 6465 7363 7269 7074 6f72 2e45 6e75 6d44  descriptor.EnumD
-00007dc0: 6573 6372 6970 746f 720a 2020 2020 2020  escriptor.      
-00007dd0: 2020 4f4b 3a20 4765 744c 6162 656c 7352    OK: GetLabelsR
-00007de0: 6573 706f 6e73 652e 5f53 7461 7475 732e  esponse._Status.
-00007df0: 5661 6c75 6554 7970 6520 2023 2030 0a20  ValueType  # 0. 
-00007e00: 2020 2020 2020 204e 4f54 464f 554e 443a         NOTFOUND:
-00007e10: 2047 6574 4c61 6265 6c73 5265 7370 6f6e   GetLabelsRespon
-00007e20: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-00007e30: 5479 7065 2020 2320 310a 0a20 2020 2063  Type  # 1..    c
-00007e40: 6c61 7373 2053 7461 7475 7328 5f53 7461  lass Status(_Sta
-00007e50: 7475 732c 206d 6574 6163 6c61 7373 3d5f  tus, metaclass=_
-00007e60: 5374 6174 7573 456e 756d 5479 7065 5772  StatusEnumTypeWr
-00007e70: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
-00007e80: 4f4b 3a20 4765 744c 6162 656c 7352 6573  OK: GetLabelsRes
-00007e90: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-00007ea0: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
-00007eb0: 4e4f 5446 4f55 4e44 3a20 4765 744c 6162  NOTFOUND: GetLab
-00007ec0: 656c 7352 6573 706f 6e73 652e 5374 6174  elsResponse.Stat
-00007ed0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-00007ee0: 310a 0a20 2020 204b 425f 4649 454c 445f  1..    KB_FIELD_
-00007ef0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00007f00: 2e69 6e74 0a20 2020 204c 4142 454c 535f  .int.    LABELS_
-00007f10: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00007f20: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
-00007f30: 5441 5455 535f 4649 454c 445f 4e55 4d42  TATUS_FIELD_NUMB
-00007f40: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00007f50: 0a20 2020 2073 7461 7475 733a 2067 6c6f  .    status: glo
-00007f60: 6261 6c5f 5f5f 4765 744c 6162 656c 7352  bal___GetLabelsR
-00007f70: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
-00007f80: 616c 7565 5479 7065 0a20 2020 2040 7072  alueType.    @pr
-00007f90: 6f70 6572 7479 0a20 2020 2064 6566 206b  operty.    def k
-00007fa0: 6228 7365 6c66 2920 2d3e 206e 7563 6c69  b(self) -> nucli
-00007fb0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-00007fc0: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
-00007fd0: 6c65 6467 6542 6f78 4944 3a20 2e2e 2e0a  ledgeBoxID: ....
-00007fe0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00007ff0: 2020 6465 6620 6c61 6265 6c73 2873 656c    def labels(sel
-00008000: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-00008010: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-00008020: 6f78 5f70 6232 2e4c 6162 656c 733a 202e  ox_pb2.Labels: .
-00008030: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00008040: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00008050: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-00008060: 2020 2020 2020 6b62 3a20 6e75 636c 6961        kb: nuclia
-00008070: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-00008080: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
-00008090: 6564 6765 426f 7849 4420 7c20 4e6f 6e65  edgeBoxID | None
-000080a0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-000080b0: 6c61 6265 6c73 3a20 6e75 636c 6961 6462  labels: nucliadb
-000080c0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-000080d0: 6562 6f78 5f70 6232 2e4c 6162 656c 7320  ebox_pb2.Labels 
-000080e0: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-000080f0: 2020 2020 2020 7374 6174 7573 3a20 676c        status: gl
-00008100: 6f62 616c 5f5f 5f47 6574 4c61 6265 6c73  obal___GetLabels
-00008110: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
-00008120: 5661 6c75 6554 7970 6520 3d20 2e2e 2e2c  ValueType = ...,
-00008130: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
-00008140: 2e2e 2e0a 2020 2020 6465 6620 4861 7346  ....    def HasF
-00008150: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00008160: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00008170: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
-00008180: 222c 2022 6c61 6265 6c73 222c 2062 226c  ", "labels", b"l
-00008190: 6162 656c 7322 5d29 202d 3e20 6275 696c  abels"]) -> buil
-000081a0: 7469 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20  tins.bool: .... 
-000081b0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-000081c0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-000081d0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-000081e0: 616c 5b22 6b62 222c 2062 226b 6222 2c20  al["kb", b"kb", 
-000081f0: 226c 6162 656c 7322 2c20 6222 6c61 6265  "labels", b"labe
-00008200: 6c73 222c 2022 7374 6174 7573 222c 2062  ls", "status", b
-00008210: 2273 7461 7475 7322 5d29 202d 3e20 4e6f  "status"]) -> No
-00008220: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
-00008230: 5f5f 4765 744c 6162 656c 7352 6573 706f  __GetLabelsRespo
-00008240: 6e73 6520 3d20 4765 744c 6162 656c 7352  nse = GetLabelsR
-00008250: 6573 706f 6e73 650a 0a40 7479 7069 6e67  esponse..@typing
-00008260: 2e66 696e 616c 0a63 6c61 7373 2047 6574  .final.class Get
-00008270: 4c61 6265 6c73 5265 7175 6573 7428 676f  LabelsRequest(go
-00008280: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00008290: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-000082a0: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-000082b0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000082c0: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-000082d0: 6970 746f 720a 0a20 2020 204b 425f 4649  iptor..    KB_FI
-000082e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000082f0: 7469 6e73 2e69 6e74 0a20 2020 2040 7072  tins.int.    @pr
-00008300: 6f70 6572 7479 0a20 2020 2064 6566 206b  operty.    def k
-00008310: 6228 7365 6c66 2920 2d3e 206e 7563 6c69  b(self) -> nucli
-00008320: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-00008330: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
-00008340: 6c65 6467 6542 6f78 4944 3a20 2e2e 2e0a  ledgeBoxID: ....
-00008350: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00008360: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00008370: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00008380: 2020 206b 623a 206e 7563 6c69 6164 625f     kb: nucliadb_
-00008390: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-000083a0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-000083b0: 6542 6f78 4944 207c 204e 6f6e 6520 3d20  eBoxID | None = 
-000083c0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
-000083d0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-000083e0: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
-000083f0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00008400: 672e 4c69 7465 7261 6c5b 226b 6222 2c20  g.Literal["kb", 
-00008410: 6222 6b62 225d 2920 2d3e 2062 7569 6c74  b"kb"]) -> built
-00008420: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-00008430: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-00008440: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-00008450: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-00008460: 6c5b 226b 6222 2c20 6222 6b62 225d 2920  l["kb", b"kb"]) 
-00008470: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-00008480: 6f62 616c 5f5f 5f47 6574 4c61 6265 6c73  obal___GetLabels
-00008490: 5265 7175 6573 7420 3d20 4765 744c 6162  Request = GetLab
-000084a0: 656c 7352 6571 7565 7374 0a0a 4074 7970  elsRequest..@typ
-000084b0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000084c0: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
-000084d0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
-000084e0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-000084f0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00008500: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00008510: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00008520: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00008530: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
-00008540: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00008550: 6e74 0a20 2020 2047 524f 5550 5f46 4945  nt.    GROUP_FIE
-00008560: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00008570: 696e 732e 696e 740a 2020 2020 454e 5449  ins.int.    ENTI
-00008580: 5449 4553 5f46 4945 4c44 5f4e 554d 4245  TIES_FIELD_NUMBE
-00008590: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000085a0: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
-000085b0: 696e 732e 7374 720a 2020 2020 4070 726f  ins.str.    @pro
-000085c0: 7065 7274 790a 2020 2020 6465 6620 6b62  perty.    def kb
-000085d0: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-000085e0: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-000085f0: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
-00008600: 6564 6765 426f 7849 443a 202e 2e2e 0a20  edgeBoxID: .... 
-00008610: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00008620: 2064 6566 2065 6e74 6974 6965 7328 7365   def entities(se
-00008630: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-00008640: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-00008650: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
-00008660: 4772 6f75 703a 202e 2e2e 0a20 2020 2064  Group: ....    d
-00008670: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00008680: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00008690: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
-000086a0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-000086b0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-000086c0: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-000086d0: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
-000086e0: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
-000086f0: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00008700: 2e2c 0a20 2020 2020 2020 2065 6e74 6974  .,.        entit
-00008710: 6965 733a 206e 7563 6c69 6164 625f 7072  ies: nucliadb_pr
-00008720: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-00008730: 785f 7062 322e 456e 7469 7469 6573 4772  x_pb2.EntitiesGr
-00008740: 6f75 7020 7c20 4e6f 6e65 203d 202e 2e2e  oup | None = ...
-00008750: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00008760: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-00008770: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-00008780: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-00008790: 6974 6572 616c 5b22 656e 7469 7469 6573  iteral["entities
-000087a0: 222c 2062 2265 6e74 6974 6965 7322 2c20  ", b"entities", 
-000087b0: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
-000087c0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-000087d0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-000087e0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-000087f0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00008800: 4c69 7465 7261 6c5b 2265 6e74 6974 6965  Literal["entitie
-00008810: 7322 2c20 6222 656e 7469 7469 6573 222c  s", b"entities",
-00008820: 2022 6772 6f75 7022 2c20 6222 6772 6f75   "group", b"grou
-00008830: 7022 2c20 226b 6222 2c20 6222 6b62 225d  p", "kb", b"kb"]
-00008840: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00008850: 676c 6f62 616c 5f5f 5f4e 6577 456e 7469  global___NewEnti
-00008860: 7469 6573 4772 6f75 7052 6571 7565 7374  tiesGroupRequest
-00008870: 203d 204e 6577 456e 7469 7469 6573 4772   = NewEntitiesGr
-00008880: 6f75 7052 6571 7565 7374 0a0a 4074 7970  oupRequest..@typ
-00008890: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000088a0: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
-000088b0: 5265 7370 6f6e 7365 2867 6f6f 676c 652e  Response(google.
-000088c0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
-000088d0: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
-000088e0: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
-000088f0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
-00008900: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
-00008910: 0a0a 2020 2020 636c 6173 7320 5f53 7461  ..    class _Sta
-00008920: 7475 733a 0a20 2020 2020 2020 2056 616c  tus:.        Val
-00008930: 7565 5479 7065 203d 2074 7970 696e 672e  ueType = typing.
-00008940: 4e65 7754 7970 6528 2256 616c 7565 5479  NewType("ValueTy
-00008950: 7065 222c 2062 7569 6c74 696e 732e 696e  pe", builtins.in
-00008960: 7429 0a20 2020 2020 2020 2056 3a20 7479  t).        V: ty
-00008970: 7069 6e67 5f65 7874 656e 7369 6f6e 732e  ping_extensions.
-00008980: 5479 7065 416c 6961 7320 3d20 5661 6c75  TypeAlias = Valu
-00008990: 6554 7970 650a 0a20 2020 2063 6c61 7373  eType..    class
-000089a0: 205f 5374 6174 7573 456e 756d 5479 7065   _StatusEnumType
-000089b0: 5772 6170 7065 7228 676f 6f67 6c65 2e70  Wrapper(google.p
-000089c0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
-000089d0: 2e65 6e75 6d5f 7479 7065 5f77 7261 7070  .enum_type_wrapp
-000089e0: 6572 2e5f 456e 756d 5479 7065 5772 6170  er._EnumTypeWrap
-000089f0: 7065 725b 4e65 7745 6e74 6974 6965 7347  per[NewEntitiesG
-00008a00: 726f 7570 5265 7370 6f6e 7365 2e5f 5374  roupResponse._St
-00008a10: 6174 7573 2e56 616c 7565 5479 7065 5d2c  atus.ValueType],
-00008a20: 2062 7569 6c74 696e 732e 7479 7065 293a   builtins.type):
-00008a30: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
-00008a40: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00008a50: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-00008a60: 456e 756d 4465 7363 7269 7074 6f72 0a20  EnumDescriptor. 
-00008a70: 2020 2020 2020 204f 4b3a 204e 6577 456e         OK: NewEn
-00008a80: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-00008a90: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-00008aa0: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
-00008ab0: 2020 2045 5252 4f52 3a20 4e65 7745 6e74     ERROR: NewEnt
-00008ac0: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-00008ad0: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-00008ae0: 5479 7065 2020 2320 310a 2020 2020 2020  Type  # 1.      
-00008af0: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
-00008b00: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
-00008b10: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-00008b20: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-00008b30: 2020 2020 2020 2020 414c 5245 4144 595f          ALREADY_
-00008b40: 4558 4953 5453 3a20 4e65 7745 6e74 6974  EXISTS: NewEntit
-00008b50: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-00008b60: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
-00008b70: 7065 2020 2320 330a 0a20 2020 2063 6c61  pe  # 3..    cla
-00008b80: 7373 2053 7461 7475 7328 5f53 7461 7475  ss Status(_Statu
-00008b90: 732c 206d 6574 6163 6c61 7373 3d5f 5374  s, metaclass=_St
-00008ba0: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
-00008bb0: 7065 7229 3a20 2e2e 2e0a 2020 2020 4f4b  per): ....    OK
-00008bc0: 3a20 4e65 7745 6e74 6974 6965 7347 726f  : NewEntitiesGro
-00008bd0: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
-00008be0: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
-00008bf0: 0a20 2020 2045 5252 4f52 3a20 4e65 7745  .    ERROR: NewE
-00008c00: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
-00008c10: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
-00008c20: 6554 7970 6520 2023 2031 0a20 2020 204b  eType  # 1.    K
-00008c30: 425f 4e4f 545f 464f 554e 443a 204e 6577  B_NOT_FOUND: New
-00008c40: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
-00008c50: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-00008c60: 7565 5479 7065 2020 2320 320a 2020 2020  ueType  # 2.    
-00008c70: 414c 5245 4144 595f 4558 4953 5453 3a20  ALREADY_EXISTS: 
-00008c80: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
-00008c90: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
-00008ca0: 5661 6c75 6554 7970 6520 2023 2033 0a0a  ValueType  # 3..
-00008cb0: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
-00008cc0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00008cd0: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
-00008ce0: 3a20 676c 6f62 616c 5f5f 5f4e 6577 456e  : global___NewEn
-00008cf0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-00008d00: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
-00008d10: 5479 7065 0a20 2020 2064 6566 205f 5f69  Type.    def __i
-00008d20: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00008d30: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-00008d40: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
-00008d50: 676c 6f62 616c 5f5f 5f4e 6577 456e 7469  global___NewEnti
-00008d60: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-00008d70: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-00008d80: 7065 203d 202e 2e2e 2c0a 2020 2020 2920  pe = ...,.    ) 
-00008d90: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-00008da0: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
-00008db0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-00008dc0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-00008dd0: 5b22 7374 6174 7573 222c 2062 2273 7461  ["status", b"sta
-00008de0: 7475 7322 5d29 202d 3e20 4e6f 6e65 3a20  tus"]) -> None: 
-00008df0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4e65  .....global___Ne
-00008e00: 7745 6e74 6974 6965 7347 726f 7570 5265  wEntitiesGroupRe
-00008e10: 7370 6f6e 7365 203d 204e 6577 456e 7469  sponse = NewEnti
-00008e20: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-00008e30: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
-00008e40: 0a63 6c61 7373 2053 6574 456e 7469 7469  .class SetEntiti
-00008e50: 6573 5265 7175 6573 7428 676f 6f67 6c65  esRequest(google
-00008e60: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-00008e70: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00008e80: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00008e90: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00008ea0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00008eb0: 720a 0a20 2020 204b 425f 4649 454c 445f  r..    KB_FIELD_
-00008ec0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00008ed0: 2e69 6e74 0a20 2020 2047 524f 5550 5f46  .int.    GROUP_F
-00008ee0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00008ef0: 6c74 696e 732e 696e 740a 2020 2020 454e  ltins.int.    EN
-00008f00: 5449 5449 4553 5f46 4945 4c44 5f4e 554d  TITIES_FIELD_NUM
-00008f10: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00008f20: 740a 2020 2020 6772 6f75 703a 2062 7569  t.    group: bui
-00008f30: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
-00008f40: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00008f50: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
-00008f60: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-00008f70: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-00008f80: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
-00008f90: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00008fa0: 2020 2064 6566 2065 6e74 6974 6965 7328     def entities(
-00008fb0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-00008fc0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-00008fd0: 6765 626f 785f 7062 322e 456e 7469 7469  gebox_pb2.Entiti
-00008fe0: 6573 4772 6f75 703a 202e 2e2e 0a20 2020  esGroup: ....   
-00008ff0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00009000: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00009010: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00009020: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
-00009030: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-00009040: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-00009050: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
-00009060: 2c0a 2020 2020 2020 2020 6772 6f75 703a  ,.        group:
-00009070: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-00009080: 2e2e 2e2c 0a20 2020 2020 2020 2065 6e74  ...,.        ent
-00009090: 6974 6965 733a 206e 7563 6c69 6164 625f  ities: nucliadb_
-000090a0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-000090b0: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
-000090c0: 4772 6f75 7020 7c20 4e6f 6e65 203d 202e  Group | None = .
-000090d0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
-000090e0: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
-000090f0: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
-00009100: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00009110: 2e4c 6974 6572 616c 5b22 656e 7469 7469  .Literal["entiti
-00009120: 6573 222c 2062 2265 6e74 6974 6965 7322  es", b"entities"
-00009130: 2c20 226b 6222 2c20 6222 6b62 225d 2920  , "kb", b"kb"]) 
-00009140: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-00009150: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
-00009160: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-00009170: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00009180: 672e 4c69 7465 7261 6c5b 2265 6e74 6974  g.Literal["entit
-00009190: 6965 7322 2c20 6222 656e 7469 7469 6573  ies", b"entities
-000091a0: 222c 2022 6772 6f75 7022 2c20 6222 6772  ", "group", b"gr
-000091b0: 6f75 7022 2c20 226b 6222 2c20 6222 6b62  oup", "kb", b"kb
-000091c0: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-000091d0: 0a0a 676c 6f62 616c 5f5f 5f53 6574 456e  ..global___SetEn
-000091e0: 7469 7469 6573 5265 7175 6573 7420 3d20  titiesRequest = 
-000091f0: 5365 7445 6e74 6974 6965 7352 6571 7565  SetEntitiesReque
-00009200: 7374 0a0a 4074 7970 696e 672e 6669 6e61  st..@typing.fina
-00009210: 6c0a 636c 6173 7320 5570 6461 7465 456e  l.class UpdateEn
-00009220: 7469 7469 6573 4772 6f75 7052 6571 7565  titiesGroupReque
-00009230: 7374 2867 6f6f 676c 652e 7072 6f74 6f62  st(google.protob
-00009240: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00009250: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00009260: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00009270: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-00009280: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-00009290: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
-000092a0: 2020 636c 6173 7320 4164 6445 6e74 7279    class AddEntry
-000092b0: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-000092c0: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-000092d0: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
-000092e0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-000092f0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00009300: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00009310: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
-00009320: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00009330: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
-00009340: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
-00009350: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00009360: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
-00009370: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
-00009380: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
-00009390: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
-000093a0: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-000093b0: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-000093c0: 785f 7062 322e 456e 7469 7479 3a20 2e2e  x_pb2.Entity: ..
-000093d0: 2e0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
-000093e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000093f0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00009400: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00009410: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
-00009420: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00009430: 2020 2020 2020 2020 2020 7661 6c75 653a            value:
-00009440: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00009450: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-00009460: 322e 456e 7469 7479 207c 204e 6f6e 6520  2.Entity | None 
-00009470: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
-00009480: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00009490: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
-000094a0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-000094b0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-000094c0: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
-000094d0: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
-000094e0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-000094f0: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
-00009500: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00009510: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00009520: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
-00009530: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
-00009540: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
-00009550: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
-00009560: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
-00009570: 7373 2055 7064 6174 6545 6e74 7279 2867  ss UpdateEntry(g
-00009580: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-00009590: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-000095a0: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
-000095b0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-000095c0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-000095d0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-000095e0: 2020 2020 4b45 595f 4649 454c 445f 4e55      KEY_FIELD_NU
-000095f0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00009600: 6e74 0a20 2020 2020 2020 2056 414c 5545  nt.        VALUE
-00009610: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00009620: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00009630: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
-00009640: 732e 7374 720a 2020 2020 2020 2020 4070  s.str.        @p
-00009650: 726f 7065 7274 790a 2020 2020 2020 2020  roperty.        
-00009660: 6465 6620 7661 6c75 6528 7365 6c66 2920  def value(self) 
-00009670: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-00009680: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-00009690: 7062 322e 456e 7469 7479 3a20 2e2e 2e0a  pb2.Entity: ....
-000096a0: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
-000096b0: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
-000096c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000096d0: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
-000096e0: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
-000096f0: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00009700: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
-00009710: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-00009720: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-00009730: 456e 7469 7479 207c 204e 6f6e 6520 3d20  Entity | None = 
-00009740: 2e2e 2e2c 0a20 2020 2020 2020 2029 202d  ...,.        ) -
-00009750: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00009760: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
-00009770: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-00009780: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-00009790: 6c5b 2276 616c 7565 222c 2062 2276 616c  l["value", b"val
-000097a0: 7565 225d 2920 2d3e 2062 7569 6c74 696e  ue"]) -> builtin
-000097b0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-000097c0: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
-000097d0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-000097e0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-000097f0: 7261 6c5b 226b 6579 222c 2062 226b 6579  ral["key", b"key
-00009800: 222c 2022 7661 6c75 6522 2c20 6222 7661  ", "value", b"va
-00009810: 6c75 6522 5d29 202d 3e20 4e6f 6e65 3a20  lue"]) -> None: 
-00009820: 2e2e 2e0a 0a20 2020 204b 425f 4649 454c  .....    KB_FIEL
-00009830: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00009840: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
-00009850: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00009860: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00009870: 4144 445f 4649 454c 445f 4e55 4d42 4552  ADD_FIELD_NUMBER
-00009880: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00009890: 2020 2055 5044 4154 455f 4649 454c 445f     UPDATE_FIELD_
-000098a0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-000098b0: 2e69 6e74 0a20 2020 2044 454c 4554 455f  .int.    DELETE_
-000098c0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-000098d0: 696c 7469 6e73 2e69 6e74 0a20 2020 2054  iltins.int.    T
-000098e0: 4954 4c45 5f46 4945 4c44 5f4e 554d 4245  ITLE_FIELD_NUMBE
-000098f0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00009900: 2020 2020 434f 4c4f 525f 4649 454c 445f      COLOR_FIELD_
-00009910: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00009920: 2e69 6e74 0a20 2020 2067 726f 7570 3a20  .int.    group: 
-00009930: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
-00009940: 2074 6974 6c65 3a20 6275 696c 7469 6e73   title: builtins
-00009950: 2e73 7472 0a20 2020 2063 6f6c 6f72 3a20  .str.    color: 
-00009960: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
-00009970: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00009980: 6566 206b 6228 7365 6c66 2920 2d3e 206e  ef kb(self) -> n
-00009990: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-000099a0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-000099b0: 4b6e 6f77 6c65 6467 6542 6f78 4944 3a20  KnowledgeBoxID: 
-000099c0: 2e2e 2e0a 2020 2020 4070 726f 7065 7274  ....    @propert
-000099d0: 790a 2020 2020 6465 6620 6164 6428 7365  y.    def add(se
-000099e0: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
-000099f0: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-00009a00: 636f 6e74 6169 6e65 7273 2e4d 6573 7361  containers.Messa
-00009a10: 6765 4d61 705b 6275 696c 7469 6e73 2e73  geMap[builtins.s
-00009a20: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
-00009a30: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-00009a40: 5f70 6232 2e45 6e74 6974 795d 3a0a 2020  _pb2.Entity]:.  
-00009a50: 2020 2020 2020 2222 2265 6e74 6974 795f        """entity_
-00009a60: 6964 3a20 456e 7469 7479 2222 220a 0a20  id: Entity""".. 
-00009a70: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00009a80: 2064 6566 2075 7064 6174 6528 7365 6c66   def update(self
-00009a90: 2920 2d3e 2067 6f6f 676c 652e 7072 6f74  ) -> google.prot
-00009aa0: 6f62 7566 2e69 6e74 6572 6e61 6c2e 636f  obuf.internal.co
-00009ab0: 6e74 6169 6e65 7273 2e4d 6573 7361 6765  ntainers.Message
-00009ac0: 4d61 705b 6275 696c 7469 6e73 2e73 7472  Map[builtins.str
-00009ad0: 2c20 6e75 636c 6961 6462 5f70 726f 746f  , nucliadb_proto
-00009ae0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-00009af0: 6232 2e45 6e74 6974 795d 3a0a 2020 2020  b2.Entity]:.    
-00009b00: 2020 2020 2222 2265 6e74 6974 795f 6964      """entity_id
-00009b10: 3a20 456e 7469 7479 2222 220a 0a20 2020  : Entity"""..   
-00009b20: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00009b30: 6566 2064 656c 6574 6528 7365 6c66 2920  ef delete(self) 
-00009b40: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
-00009b50: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
-00009b60: 6169 6e65 7273 2e52 6570 6561 7465 6453  ainers.RepeatedS
-00009b70: 6361 6c61 7246 6965 6c64 436f 6e74 6169  calarFieldContai
-00009b80: 6e65 725b 6275 696c 7469 6e73 2e73 7472  ner[builtins.str
-00009b90: 5d3a 0a20 2020 2020 2020 2022 2222 656e  ]:.        """en
-00009ba0: 7469 7479 5f69 6422 2222 0a0a 2020 2020  tity_id"""..    
-00009bb0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00009bc0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00009bd0: 2020 2020 2a2c 0a20 2020 2020 2020 206b      *,.        k
-00009be0: 623a 206e 7563 6c69 6164 625f 7072 6f74  b: nucliadb_prot
-00009bf0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-00009c00: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
-00009c10: 4944 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ID | None = ...,
-00009c20: 0a20 2020 2020 2020 2067 726f 7570 3a20  .        group: 
-00009c30: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-00009c40: 2e2e 2c0a 2020 2020 2020 2020 6164 643a  ..,.        add:
-00009c50: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00009c60: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
-00009c70: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
-00009c80: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-00009c90: 626f 785f 7062 322e 456e 7469 7479 5d20  box_pb2.Entity] 
-00009ca0: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00009cb0: 2020 2020 2020 7570 6461 7465 3a20 636f        update: co
-00009cc0: 6c6c 6563 7469 6f6e 732e 6162 632e 4d61  llections.abc.Ma
-00009cd0: 7070 696e 675b 6275 696c 7469 6e73 2e73  pping[builtins.s
-00009ce0: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
-00009cf0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-00009d00: 5f70 6232 2e45 6e74 6974 795d 207c 204e  _pb2.Entity] | N
-00009d10: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-00009d20: 2020 2064 656c 6574 653a 2063 6f6c 6c65     delete: colle
-00009d30: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
-00009d40: 626c 655b 6275 696c 7469 6e73 2e73 7472  ble[builtins.str
-00009d50: 5d20 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  ] | None = ...,.
-00009d60: 2020 2020 2020 2020 7469 746c 653a 2062          title: b
-00009d70: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00009d80: 2e2c 0a20 2020 2020 2020 2063 6f6c 6f72  .,.        color
-00009d90: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00009da0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-00009db0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-00009dc0: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
-00009dd0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-00009de0: 6e67 2e4c 6974 6572 616c 5b22 6b62 222c  ng.Literal["kb",
-00009df0: 2062 226b 6222 5d29 202d 3e20 6275 696c   b"kb"]) -> buil
-00009e00: 7469 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20  tins.bool: .... 
-00009e10: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-00009e20: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00009e30: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00009e40: 616c 5b22 6164 6422 2c20 6222 6164 6422  al["add", b"add"
-00009e50: 2c20 2263 6f6c 6f72 222c 2062 2263 6f6c  , "color", b"col
-00009e60: 6f72 222c 2022 6465 6c65 7465 222c 2062  or", "delete", b
-00009e70: 2264 656c 6574 6522 2c20 2267 726f 7570  "delete", "group
-00009e80: 222c 2062 2267 726f 7570 222c 2022 6b62  ", b"group", "kb
-00009e90: 222c 2062 226b 6222 2c20 2274 6974 6c65  ", b"kb", "title
-00009ea0: 222c 2062 2274 6974 6c65 222c 2022 7570  ", b"title", "up
-00009eb0: 6461 7465 222c 2062 2275 7064 6174 6522  date", b"update"
-00009ec0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-00009ed0: 0a67 6c6f 6261 6c5f 5f5f 5570 6461 7465  .global___Update
-00009ee0: 456e 7469 7469 6573 4772 6f75 7052 6571  EntitiesGroupReq
-00009ef0: 7565 7374 203d 2055 7064 6174 6545 6e74  uest = UpdateEnt
-00009f00: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
-00009f10: 740a 0a40 7479 7069 6e67 2e66 696e 616c  t..@typing.final
-00009f20: 0a63 6c61 7373 2055 7064 6174 6545 6e74  .class UpdateEnt
-00009f30: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-00009f40: 7365 2867 6f6f 676c 652e 7072 6f74 6f62  se(google.protob
-00009f50: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00009f60: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00009f70: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00009f80: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-00009f90: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-00009fa0: 636c 6173 7320 5f53 7461 7475 733a 0a20  class _Status:. 
-00009fb0: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
-00009fc0: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
-00009fd0: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
-00009fe0: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
-00009ff0: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
-0000a000: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
-0000a010: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
-0000a020: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
-0000a030: 7573 456e 756d 5479 7065 5772 6170 7065  usEnumTypeWrappe
-0000a040: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
-0000a050: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
-0000a060: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
-0000a070: 756d 5479 7065 5772 6170 7065 725b 5570  umTypeWrapper[Up
-0000a080: 6461 7465 456e 7469 7469 6573 4772 6f75  dateEntitiesGrou
-0000a090: 7052 6573 706f 6e73 652e 5f53 7461 7475  pResponse._Statu
-0000a0a0: 732e 5661 6c75 6554 7970 655d 2c20 6275  s.ValueType], bu
-0000a0b0: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
-0000a0c0: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
-0000a0d0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-0000a0e0: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
-0000a0f0: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
-0000a100: 2020 2020 4f4b 3a20 5570 6461 7465 456e      OK: UpdateEn
-0000a110: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-0000a120: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-0000a130: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
-0000a140: 2020 2045 5252 4f52 3a20 5570 6461 7465     ERROR: Update
-0000a150: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
-0000a160: 706f 6e73 652e 5f53 7461 7475 732e 5661  ponse._Status.Va
-0000a170: 6c75 6554 7970 6520 2023 2031 0a20 2020  lueType  # 1.   
-0000a180: 2020 2020 204b 425f 4e4f 545f 464f 554e       KB_NOT_FOUN
-0000a190: 443a 2055 7064 6174 6545 6e74 6974 6965  D: UpdateEntitie
-0000a1a0: 7347 726f 7570 5265 7370 6f6e 7365 2e5f  sGroupResponse._
-0000a1b0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000a1c0: 2020 2320 320a 2020 2020 2020 2020 454e    # 2.        EN
-0000a1d0: 5449 5449 4553 5f47 524f 5550 5f4e 4f54  TITIES_GROUP_NOT
-0000a1e0: 5f46 4f55 4e44 3a20 5570 6461 7465 456e  _FOUND: UpdateEn
-0000a1f0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-0000a200: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-0000a210: 6554 7970 6520 2023 2033 0a0a 2020 2020  eType  # 3..    
-0000a220: 636c 6173 7320 5374 6174 7573 285f 5374  class Status(_St
-0000a230: 6174 7573 2c20 6d65 7461 636c 6173 733d  atus, metaclass=
-0000a240: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
-0000a250: 7261 7070 6572 293a 202e 2e2e 0a20 2020  rapper): ....   
-0000a260: 204f 4b3a 2055 7064 6174 6545 6e74 6974   OK: UpdateEntit
-0000a270: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-0000a280: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000a290: 6520 2023 2030 0a20 2020 2045 5252 4f52  e  # 0.    ERROR
-0000a2a0: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
-0000a2b0: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
-0000a2c0: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
-0000a2d0: 2320 310a 2020 2020 4b42 5f4e 4f54 5f46  # 1.    KB_NOT_F
-0000a2e0: 4f55 4e44 3a20 5570 6461 7465 456e 7469  OUND: UpdateEnti
-0000a2f0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000a300: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000a310: 7065 2020 2320 320a 2020 2020 454e 5449  pe  # 2.    ENTI
-0000a320: 5449 4553 5f47 524f 5550 5f4e 4f54 5f46  TIES_GROUP_NOT_F
-0000a330: 4f55 4e44 3a20 5570 6461 7465 456e 7469  OUND: UpdateEnti
-0000a340: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000a350: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000a360: 7065 2020 2320 330a 0a20 2020 2053 5441  pe  # 3..    STA
-0000a370: 5455 535f 4649 454c 445f 4e55 4d42 4552  TUS_FIELD_NUMBER
-0000a380: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-0000a390: 2020 2073 7461 7475 733a 2067 6c6f 6261     status: globa
-0000a3a0: 6c5f 5f5f 5570 6461 7465 456e 7469 7469  l___UpdateEntiti
-0000a3b0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
-0000a3c0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000a3d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000a3e0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000a3f0: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000a400: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
-0000a410: 616c 5f5f 5f55 7064 6174 6545 6e74 6974  al___UpdateEntit
-0000a420: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-0000a430: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000a440: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-0000a450: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000a460: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000a470: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000a480: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000a490: 2273 7461 7475 7322 2c20 6222 7374 6174  "status", b"stat
-0000a4a0: 7573 225d 2920 2d3e 204e 6f6e 653a 202e  us"]) -> None: .
-0000a4b0: 2e2e 0a0a 676c 6f62 616c 5f5f 5f55 7064  ....global___Upd
-0000a4c0: 6174 6545 6e74 6974 6965 7347 726f 7570  ateEntitiesGroup
-0000a4d0: 5265 7370 6f6e 7365 203d 2055 7064 6174  Response = Updat
-0000a4e0: 6545 6e74 6974 6965 7347 726f 7570 5265  eEntitiesGroupRe
-0000a4f0: 7370 6f6e 7365 0a0a 4074 7970 696e 672e  sponse..@typing.
-0000a500: 6669 6e61 6c0a 636c 6173 7320 4c69 7374  final.class List
-0000a510: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
-0000a520: 7175 6573 7428 676f 6f67 6c65 2e70 726f  quest(google.pro
-0000a530: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
-0000a540: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
-0000a550: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-0000a560: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-0000a570: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
-0000a580: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
-0000a590: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000a5a0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a5b0: 2020 2064 6566 206b 6228 7365 6c66 2920     def kb(self) 
-0000a5c0: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-0000a5d0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000a5e0: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
-0000a5f0: 4944 3a20 2e2e 2e0a 2020 2020 6465 6620  ID: ....    def 
-0000a600: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0000a610: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000a620: 2a2c 0a20 2020 2020 2020 206b 623a 206e  *,.        kb: n
-0000a630: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000a640: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000a650: 4b6e 6f77 6c65 6467 6542 6f78 4944 207c  KnowledgeBoxID |
-0000a660: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-0000a670: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-0000a680: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
-0000a690: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-0000a6a0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-0000a6b0: 6c5b 226b 6222 2c20 6222 6b62 225d 2920  l["kb", b"kb"]) 
-0000a6c0: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-0000a6d0: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
-0000a6e0: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-0000a6f0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-0000a700: 672e 4c69 7465 7261 6c5b 226b 6222 2c20  g.Literal["kb", 
-0000a710: 6222 6b62 225d 2920 2d3e 204e 6f6e 653a  b"kb"]) -> None:
-0000a720: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f4c   .....global___L
-0000a730: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
-0000a740: 7352 6571 7565 7374 203d 204c 6973 7445  sRequest = ListE
-0000a750: 6e74 6974 6965 7347 726f 7570 7352 6571  ntitiesGroupsReq
-0000a760: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
-0000a770: 6e61 6c0a 636c 6173 7320 4c69 7374 456e  nal.class ListEn
-0000a780: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
-0000a790: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
-0000a7a0: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-0000a7b0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-0000a7c0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-0000a7d0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-0000a7e0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-0000a7f0: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
-0000a800: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
-0000a810: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
-0000a820: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
-0000a830: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
-0000a840: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
-0000a850: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
-0000a860: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
-0000a870: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
-0000a880: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
-0000a890: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
-0000a8a0: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
-0000a8b0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
-0000a8c0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
-0000a8d0: 4c69 7374 456e 7469 7469 6573 4772 6f75  ListEntitiesGrou
-0000a8e0: 7073 5265 7370 6f6e 7365 2e5f 5374 6174  psResponse._Stat
-0000a8f0: 7573 2e56 616c 7565 5479 7065 5d2c 2062  us.ValueType], b
-0000a900: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
-0000a910: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
-0000a920: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-0000a930: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
-0000a940: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
-0000a950: 2020 2020 204f 4b3a 204c 6973 7445 6e74       OK: ListEnt
-0000a960: 6974 6965 7347 726f 7570 7352 6573 706f  itiesGroupsRespo
-0000a970: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-0000a980: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
-0000a990: 2020 204e 4f54 464f 554e 443a 204c 6973     NOTFOUND: Lis
-0000a9a0: 7445 6e74 6974 6965 7347 726f 7570 7352  tEntitiesGroupsR
-0000a9b0: 6573 706f 6e73 652e 5f53 7461 7475 732e  esponse._Status.
-0000a9c0: 5661 6c75 6554 7970 6520 2023 2031 0a20  ValueType  # 1. 
-0000a9d0: 2020 2020 2020 2045 5252 4f52 3a20 4c69         ERROR: Li
-0000a9e0: 7374 456e 7469 7469 6573 4772 6f75 7073  stEntitiesGroups
-0000a9f0: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-0000aa00: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-0000aa10: 0a20 2020 2063 6c61 7373 2053 7461 7475  .    class Statu
-0000aa20: 7328 5f53 7461 7475 732c 206d 6574 6163  s(_Status, metac
-0000aa30: 6c61 7373 3d5f 5374 6174 7573 456e 756d  lass=_StatusEnum
-0000aa40: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
-0000aa50: 2e0a 2020 2020 4f4b 3a20 4c69 7374 456e  ..    OK: ListEn
-0000aa60: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
-0000aa70: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
-0000aa80: 6554 7970 6520 2023 2030 0a20 2020 204e  eType  # 0.    N
-0000aa90: 4f54 464f 554e 443a 204c 6973 7445 6e74  OTFOUND: ListEnt
-0000aaa0: 6974 6965 7347 726f 7570 7352 6573 706f  itiesGroupsRespo
-0000aab0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
-0000aac0: 5479 7065 2020 2320 310a 2020 2020 4552  Type  # 1.    ER
-0000aad0: 524f 523a 204c 6973 7445 6e74 6974 6965  ROR: ListEntitie
-0000aae0: 7347 726f 7570 7352 6573 706f 6e73 652e  sGroupsResponse.
-0000aaf0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000ab00: 2020 2320 320a 0a20 2020 2040 7479 7069    # 2..    @typi
-0000ab10: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
-0000ab20: 7373 2047 726f 7570 7345 6e74 7279 2867  ss GroupsEntry(g
-0000ab30: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-0000ab40: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-0000ab50: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
-0000ab60: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-0000ab70: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-0000ab80: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-0000ab90: 2020 2020 4b45 595f 4649 454c 445f 4e55      KEY_FIELD_NU
-0000aba0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000abb0: 6e74 0a20 2020 2020 2020 2056 414c 5545  nt.        VALUE
-0000abc0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000abd0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000abe0: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
-0000abf0: 732e 7374 720a 2020 2020 2020 2020 4070  s.str.        @p
-0000ac00: 726f 7065 7274 790a 2020 2020 2020 2020  roperty.        
-0000ac10: 6465 6620 7661 6c75 6528 7365 6c66 2920  def value(self) 
-0000ac20: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-0000ac30: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000ac40: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
-0000ac50: 7053 756d 6d61 7279 3a20 2e2e 2e0a 2020  pSummary: ....  
-0000ac60: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
-0000ac70: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
-0000ac80: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000ac90: 2020 2a2c 0a20 2020 2020 2020 2020 2020    *,.           
-0000aca0: 206b 6579 3a20 6275 696c 7469 6e73 2e73   key: builtins.s
-0000acb0: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
-0000acc0: 2020 2020 2020 7661 6c75 653a 206e 7563        value: nuc
-0000acd0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000ace0: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
-0000acf0: 7469 7469 6573 4772 6f75 7053 756d 6d61  titiesGroupSumma
-0000ad00: 7279 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ry | None = ...,
-0000ad10: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
-0000ad20: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
-0000ad30: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-0000ad40: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000ad50: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
-0000ad60: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
-0000ad70: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-0000ad80: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
-0000ad90: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000ada0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000adb0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000adc0: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
-0000add0: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
-0000ade0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-0000adf0: 0a20 2020 2047 524f 5550 535f 4649 454c  .    GROUPS_FIEL
-0000ae00: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000ae10: 6e73 2e69 6e74 0a20 2020 2053 5441 5455  ns.int.    STATU
-0000ae20: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-0000ae30: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000ae40: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
-0000ae50: 5f5f 4c69 7374 456e 7469 7469 6573 4772  __ListEntitiesGr
-0000ae60: 6f75 7073 5265 7370 6f6e 7365 2e53 7461  oupsResponse.Sta
-0000ae70: 7475 732e 5661 6c75 6554 7970 650a 2020  tus.ValueType.  
-0000ae80: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000ae90: 6465 6620 6772 6f75 7073 2873 656c 6629  def groups(self)
-0000aea0: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
-0000aeb0: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
-0000aec0: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
-0000aed0: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
-0000aee0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000aef0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000af00: 322e 456e 7469 7469 6573 4772 6f75 7053  2.EntitiesGroupS
-0000af10: 756d 6d61 7279 5d3a 202e 2e2e 0a20 2020  ummary]: ....   
-0000af20: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0000af30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000af40: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-0000af50: 6772 6f75 7073 3a20 636f 6c6c 6563 7469  groups: collecti
-0000af60: 6f6e 732e 6162 632e 4d61 7070 696e 675b  ons.abc.Mapping[
-0000af70: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
-0000af80: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-0000af90: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
-0000afa0: 6e74 6974 6965 7347 726f 7570 5375 6d6d  ntitiesGroupSumm
-0000afb0: 6172 795d 207c 204e 6f6e 6520 3d20 2e2e  ary] | None = ..
-0000afc0: 2e2c 0a20 2020 2020 2020 2073 7461 7475  .,.        statu
-0000afd0: 733a 2067 6c6f 6261 6c5f 5f5f 4c69 7374  s: global___List
-0000afe0: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
-0000aff0: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
-0000b000: 6c75 6554 7970 6520 3d20 2e2e 2e2c 0a20  lueType = ...,. 
-0000b010: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-0000b020: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000b030: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000b040: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000b050: 7465 7261 6c5b 2267 726f 7570 7322 2c20  teral["groups", 
-0000b060: 6222 6772 6f75 7073 222c 2022 7374 6174  b"groups", "stat
-0000b070: 7573 222c 2062 2273 7461 7475 7322 5d29  us", b"status"])
-0000b080: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
-0000b090: 6c6f 6261 6c5f 5f5f 4c69 7374 456e 7469  lobal___ListEnti
-0000b0a0: 7469 6573 4772 6f75 7073 5265 7370 6f6e  tiesGroupsRespon
-0000b0b0: 7365 203d 204c 6973 7445 6e74 6974 6965  se = ListEntitie
-0000b0c0: 7347 726f 7570 7352 6573 706f 6e73 650a  sGroupsResponse.
-0000b0d0: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000b0e0: 6c61 7373 2047 6574 456e 7469 7469 6573  lass GetEntities
-0000b0f0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
-0000b100: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000b110: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-0000b120: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000b130: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000b140: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000b150: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
-0000b160: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000b170: 6e74 0a20 2020 2040 7072 6f70 6572 7479  nt.    @property
-0000b180: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
-0000b190: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-0000b1a0: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-0000b1b0: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
-0000b1c0: 6f78 4944 3a20 2e2e 2e0a 2020 2020 6465  oxID: ....    de
-0000b1d0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0000b1e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000b1f0: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
-0000b200: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000b210: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000b220: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-0000b230: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000b240: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-0000b250: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
-0000b260: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-0000b270: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-0000b280: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
-0000b290: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-0000b2a0: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
-0000b2b0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-0000b2c0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-0000b2d0: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
-0000b2e0: 2c20 6222 6b62 225d 2920 2d3e 204e 6f6e  , b"kb"]) -> Non
-0000b2f0: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-0000b300: 5f47 6574 456e 7469 7469 6573 5265 7175  _GetEntitiesRequ
-0000b310: 6573 7420 3d20 4765 7445 6e74 6974 6965  est = GetEntitie
-0000b320: 7352 6571 7565 7374 0a0a 4074 7970 696e  sRequest..@typin
-0000b330: 672e 6669 6e61 6c0a 636c 6173 7320 4765  g.final.class Ge
-0000b340: 7445 6e74 6974 6965 7352 6573 706f 6e73  tEntitiesRespons
-0000b350: 6528 676f 6f67 6c65 2e70 726f 746f 6275  e(google.protobu
-0000b360: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000b370: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000b380: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000b390: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000b3a0: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
-0000b3b0: 6c61 7373 205f 5374 6174 7573 3a0a 2020  lass _Status:.  
-0000b3c0: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
-0000b3d0: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
-0000b3e0: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
-0000b3f0: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
-0000b400: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
-0000b410: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
-0000b420: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
-0000b430: 2020 2020 636c 6173 7320 5f53 7461 7475      class _Statu
-0000b440: 7345 6e75 6d54 7970 6557 7261 7070 6572  sEnumTypeWrapper
-0000b450: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-0000b460: 2e69 6e74 6572 6e61 6c2e 656e 756d 5f74  .internal.enum_t
-0000b470: 7970 655f 7772 6170 7065 722e 5f45 6e75  ype_wrapper._Enu
-0000b480: 6d54 7970 6557 7261 7070 6572 5b47 6574  mTypeWrapper[Get
-0000b490: 456e 7469 7469 6573 5265 7370 6f6e 7365  EntitiesResponse
-0000b4a0: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
-0000b4b0: 7065 5d2c 2062 7569 6c74 696e 732e 7479  pe], builtins.ty
-0000b4c0: 7065 293a 0a20 2020 2020 2020 2044 4553  pe):.        DES
-0000b4d0: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
-0000b4e0: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
-0000b4f0: 746f 722e 456e 756d 4465 7363 7269 7074  tor.EnumDescript
-0000b500: 6f72 0a20 2020 2020 2020 204f 4b3a 2047  or.        OK: G
-0000b510: 6574 456e 7469 7469 6573 5265 7370 6f6e  etEntitiesRespon
-0000b520: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-0000b530: 5479 7065 2020 2320 300a 2020 2020 2020  Type  # 0.      
-0000b540: 2020 4e4f 5446 4f55 4e44 3a20 4765 7445    NOTFOUND: GetE
-0000b550: 6e74 6974 6965 7352 6573 706f 6e73 652e  ntitiesResponse.
-0000b560: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
-0000b570: 6520 2023 2031 0a20 2020 2020 2020 2045  e  # 1.        E
-0000b580: 5252 4f52 3a20 4765 7445 6e74 6974 6965  RROR: GetEntitie
-0000b590: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
-0000b5a0: 732e 5661 6c75 6554 7970 6520 2023 2032  s.ValueType  # 2
-0000b5b0: 0a0a 2020 2020 636c 6173 7320 5374 6174  ..    class Stat
-0000b5c0: 7573 285f 5374 6174 7573 2c20 6d65 7461  us(_Status, meta
-0000b5d0: 636c 6173 733d 5f53 7461 7475 7345 6e75  class=_StatusEnu
-0000b5e0: 6d54 7970 6557 7261 7070 6572 293a 202e  mTypeWrapper): .
-0000b5f0: 2e2e 0a20 2020 204f 4b3a 2047 6574 456e  ...    OK: GetEn
-0000b600: 7469 7469 6573 5265 7370 6f6e 7365 2e53  titiesResponse.S
-0000b610: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000b620: 2023 2030 0a20 2020 204e 4f54 464f 554e   # 0.    NOTFOUN
-0000b630: 443a 2047 6574 456e 7469 7469 6573 5265  D: GetEntitiesRe
-0000b640: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
-0000b650: 6c75 6554 7970 6520 2023 2031 0a20 2020  lueType  # 1.   
-0000b660: 2045 5252 4f52 3a20 4765 7445 6e74 6974   ERROR: GetEntit
-0000b670: 6965 7352 6573 706f 6e73 652e 5374 6174  iesResponse.Stat
-0000b680: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000b690: 320a 0a20 2020 2040 7479 7069 6e67 2e66  2..    @typing.f
-0000b6a0: 696e 616c 0a20 2020 2063 6c61 7373 2047  inal.    class G
-0000b6b0: 726f 7570 7345 6e74 7279 2867 6f6f 676c  roupsEntry(googl
-0000b6c0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-0000b6d0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-0000b6e0: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
-0000b6f0: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-0000b700: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-0000b710: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
-0000b720: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-0000b730: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-0000b740: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
-0000b750: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-0000b760: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-0000b770: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-0000b780: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
-0000b790: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
-0000b7a0: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
-0000b7b0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000b7c0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000b7d0: 456e 7469 7469 6573 4772 6f75 703a 202e  EntitiesGroup: .
-0000b7e0: 2e2e 0a20 2020 2020 2020 2064 6566 205f  ...        def _
-0000b7f0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000b800: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000b810: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-0000b820: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
-0000b830: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-0000b840: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0000b850: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-0000b860: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000b870: 6232 2e45 6e74 6974 6965 7347 726f 7570  b2.EntitiesGroup
-0000b880: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000b890: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
-0000b8a0: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-0000b8b0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
-0000b8c0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-0000b8d0: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
-0000b8e0: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
-0000b8f0: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-0000b900: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-0000b910: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-0000b920: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000b930: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000b940: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
-0000b950: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
-0000b960: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
-0000b970: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
-0000b980: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000b990: 0a20 2020 2047 524f 5550 535f 4649 454c  .    GROUPS_FIEL
-0000b9a0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000b9b0: 6e73 2e69 6e74 0a20 2020 2053 5441 5455  ns.int.    STATU
-0000b9c0: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-0000b9d0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000b9e0: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
-0000b9f0: 5f5f 4765 7445 6e74 6974 6965 7352 6573  __GetEntitiesRes
-0000ba00: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-0000ba10: 7565 5479 7065 0a20 2020 2040 7072 6f70  ueType.    @prop
-0000ba20: 6572 7479 0a20 2020 2064 6566 206b 6228  erty.    def kb(
-0000ba30: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-0000ba40: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000ba50: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
-0000ba60: 6467 6542 6f78 4944 3a20 2e2e 2e0a 2020  dgeBoxID: ....  
-0000ba70: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000ba80: 6465 6620 6772 6f75 7073 2873 656c 6629  def groups(self)
-0000ba90: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
-0000baa0: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
-0000bab0: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
-0000bac0: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
-0000bad0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000bae0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000baf0: 322e 456e 7469 7469 6573 4772 6f75 705d  2.EntitiesGroup]
-0000bb00: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
-0000bb10: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0000bb20: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-0000bb30: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
-0000bb40: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000bb50: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-0000bb60: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
-0000bb70: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-0000bb80: 2020 2067 726f 7570 733a 2063 6f6c 6c65     groups: colle
-0000bb90: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-0000bba0: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-0000bbb0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000bbc0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000bbd0: 322e 456e 7469 7469 6573 4772 6f75 705d  2.EntitiesGroup]
-0000bbe0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000bbf0: 2020 2020 2020 2073 7461 7475 733a 2067         status: g
-0000bc00: 6c6f 6261 6c5f 5f5f 4765 7445 6e74 6974  lobal___GetEntit
-0000bc10: 6965 7352 6573 706f 6e73 652e 5374 6174  iesResponse.Stat
-0000bc20: 7573 2e56 616c 7565 5479 7065 203d 202e  us.ValueType = .
-0000bc30: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
-0000bc40: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
-0000bc50: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
-0000bc60: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-0000bc70: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
-0000bc80: 226b 6222 5d29 202d 3e20 6275 696c 7469  "kb"]) -> builti
-0000bc90: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
-0000bca0: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
-0000bcb0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-0000bcc0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-0000bcd0: 5b22 6772 6f75 7073 222c 2062 2267 726f  ["groups", b"gro
-0000bce0: 7570 7322 2c20 226b 6222 2c20 6222 6b62  ups", "kb", b"kb
-0000bcf0: 222c 2022 7374 6174 7573 222c 2062 2273  ", "status", b"s
-0000bd00: 7461 7475 7322 5d29 202d 3e20 4e6f 6e65  tatus"]) -> None
-0000bd10: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-0000bd20: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
-0000bd30: 6e73 6520 3d20 4765 7445 6e74 6974 6965  nse = GetEntitie
-0000bd40: 7352 6573 706f 6e73 650a 0a40 7479 7069  sResponse..@typi
-0000bd50: 6e67 2e66 696e 616c 0a63 6c61 7373 2044  ng.final.class D
-0000bd60: 656c 456e 7469 7469 6573 5265 7175 6573  elEntitiesReques
-0000bd70: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-0000bd80: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000bd90: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000bda0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000bdb0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000bdc0: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-0000bdd0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
-0000bde0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000bdf0: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
-0000be00: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-0000be10: 740a 2020 2020 6772 6f75 703a 2062 7569  t.    group: bui
-0000be20: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
-0000be30: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000be40: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
-0000be50: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000be60: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-0000be70: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
-0000be80: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000be90: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000bea0: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000beb0: 2020 2020 6b62 3a20 6e75 636c 6961 6462      kb: nucliadb
-0000bec0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000bed0: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
-0000bee0: 6765 426f 7849 4420 7c20 4e6f 6e65 203d  geBoxID | None =
-0000bef0: 202e 2e2e 2c0a 2020 2020 2020 2020 6772   ...,.        gr
-0000bf00: 6f75 703a 2062 7569 6c74 696e 732e 7374  oup: builtins.st
-0000bf10: 7220 3d20 2e2e 2e2c 0a20 2020 2029 202d  r = ...,.    ) -
-0000bf20: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000bf30: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-0000bf40: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000bf50: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000bf60: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
-0000bf70: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000bf80: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000bf90: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000bfa0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000bfb0: 7465 7261 6c5b 2267 726f 7570 222c 2062  teral["group", b
-0000bfc0: 2267 726f 7570 222c 2022 6b62 222c 2062  "group", "kb", b
-0000bfd0: 226b 6222 5d29 202d 3e20 4e6f 6e65 3a20  "kb"]) -> None: 
-0000bfe0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4465  .....global___De
-0000bff0: 6c45 6e74 6974 6965 7352 6571 7565 7374  lEntitiesRequest
-0000c000: 203d 2044 656c 456e 7469 7469 6573 5265   = DelEntitiesRe
-0000c010: 7175 6573 740a 0a40 7479 7069 6e67 2e66  quest..@typing.f
-0000c020: 696e 616c 0a63 6c61 7373 204d 6572 6765  inal.class Merge
-0000c030: 456e 7469 7469 6573 5265 7175 6573 7428  EntitiesRequest(
-0000c040: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000c050: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-0000c060: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
-0000c070: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-0000c080: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
-0000c090: 6372 6970 746f 720a 0a20 2020 2040 7479  criptor..    @ty
-0000c0a0: 7069 6e67 2e66 696e 616c 0a20 2020 2063  ping.final.    c
-0000c0b0: 6c61 7373 2045 6e74 6974 7949 4428 676f  lass EntityID(go
-0000c0c0: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-0000c0d0: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-0000c0e0: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-0000c0f0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000c100: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000c110: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
-0000c120: 2020 2047 524f 5550 5f46 4945 4c44 5f4e     GROUP_FIELD_N
-0000c130: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-0000c140: 696e 740a 2020 2020 2020 2020 454e 5449  int.        ENTI
-0000c150: 5459 5f46 4945 4c44 5f4e 554d 4245 523a  TY_FIELD_NUMBER:
-0000c160: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-0000c170: 2020 2020 2020 6772 6f75 703a 2062 7569        group: bui
-0000c180: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
-0000c190: 2020 656e 7469 7479 3a20 6275 696c 7469    entity: builti
-0000c1a0: 6e73 2e73 7472 0a20 2020 2020 2020 2064  ns.str.        d
-0000c1b0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000c1c0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-0000c1d0: 2020 2020 2020 2020 2020 202a 2c0a 2020             *,.  
-0000c1e0: 2020 2020 2020 2020 2020 6772 6f75 703a            group:
-0000c1f0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-0000c200: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
-0000c210: 2065 6e74 6974 793a 2062 7569 6c74 696e   entity: builtin
-0000c220: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-0000c230: 2020 2020 2029 202d 3e20 4e6f 6e65 3a20       ) -> None: 
-0000c240: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
-0000c250: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-0000c260: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-0000c270: 696e 672e 4c69 7465 7261 6c5b 2265 6e74  ing.Literal["ent
-0000c280: 6974 7922 2c20 6222 656e 7469 7479 222c  ity", b"entity",
-0000c290: 2022 6772 6f75 7022 2c20 6222 6772 6f75   "group", b"grou
-0000c2a0: 7022 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  p"]) -> None: ..
-0000c2b0: 2e0a 0a20 2020 204b 425f 4649 454c 445f  ...    KB_FIELD_
-0000c2c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-0000c2d0: 2e69 6e74 0a20 2020 2046 524f 4d5f 4649  .int.    FROM_FI
-0000c2e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000c2f0: 7469 6e73 2e69 6e74 0a20 2020 2054 4f5f  tins.int.    TO_
-0000c300: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-0000c310: 696c 7469 6e73 2e69 6e74 0a20 2020 2040  iltins.int.    @
-0000c320: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000c330: 206b 6228 7365 6c66 2920 2d3e 206e 7563   kb(self) -> nuc
-0000c340: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000c350: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-0000c360: 6f77 6c65 6467 6542 6f78 4944 3a20 2e2e  owledgeBoxID: ..
-0000c370: 2e0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000c380: 2020 2020 6465 6620 746f 2873 656c 6629      def to(self)
-0000c390: 202d 3e20 676c 6f62 616c 5f5f 5f4d 6572   -> global___Mer
-0000c3a0: 6765 456e 7469 7469 6573 5265 7175 6573  geEntitiesReques
-0000c3b0: 742e 456e 7469 7479 4944 3a20 2e2e 2e0a  t.EntityID: ....
-0000c3c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000c3d0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000c3e0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0000c3f0: 2020 206b 623a 206e 7563 6c69 6164 625f     kb: nucliadb_
-0000c400: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-0000c410: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-0000c420: 6542 6f78 4944 207c 204e 6f6e 6520 3d20  eBoxID | None = 
-0000c430: 2e2e 2e2c 0a20 2020 2020 2020 2074 6f3a  ...,.        to:
-0000c440: 2067 6c6f 6261 6c5f 5f5f 4d65 7267 6545   global___MergeE
-0000c450: 6e74 6974 6965 7352 6571 7565 7374 2e45  ntitiesRequest.E
-0000c460: 6e74 6974 7949 4420 7c20 4e6f 6e65 203d  ntityID | None =
-0000c470: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-0000c480: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-0000c490: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
-0000c4a0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-0000c4b0: 6e67 2e4c 6974 6572 616c 5b22 6672 6f6d  ng.Literal["from
-0000c4c0: 222c 2062 2266 726f 6d22 2c20 226b 6222  ", b"from", "kb"
-0000c4d0: 2c20 6222 6b62 222c 2022 746f 222c 2062  , b"kb", "to", b
-0000c4e0: 2274 6f22 5d29 202d 3e20 6275 696c 7469  "to"]) -> builti
-0000c4f0: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
-0000c500: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
-0000c510: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-0000c520: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-0000c530: 5b22 6672 6f6d 222c 2062 2266 726f 6d22  ["from", b"from"
-0000c540: 2c20 226b 6222 2c20 6222 6b62 222c 2022  , "kb", b"kb", "
-0000c550: 746f 222c 2062 2274 6f22 5d29 202d 3e20  to", b"to"]) -> 
-0000c560: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-0000c570: 6c5f 5f5f 4d65 7267 6545 6e74 6974 6965  l___MergeEntitie
-0000c580: 7352 6571 7565 7374 203d 204d 6572 6765  sRequest = Merge
-0000c590: 456e 7469 7469 6573 5265 7175 6573 740a  EntitiesRequest.
-0000c5a0: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000c5b0: 6c61 7373 2047 6574 4c61 6265 6c53 6574  lass GetLabelSet
-0000c5c0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
-0000c5d0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000c5e0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-0000c5f0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000c600: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000c610: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000c620: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
-0000c630: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000c640: 6e74 0a20 2020 204c 4142 454c 5345 545f  nt.    LABELSET_
-0000c650: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-0000c660: 696c 7469 6e73 2e69 6e74 0a20 2020 206c  iltins.int.    l
-0000c670: 6162 656c 7365 743a 2062 7569 6c74 696e  abelset: builtin
-0000c680: 732e 7374 720a 2020 2020 4070 726f 7065  s.str.    @prope
-0000c690: 7274 790a 2020 2020 6465 6620 6b62 2873  rty.    def kb(s
-0000c6a0: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
-0000c6b0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000c6c0: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
-0000c6d0: 6765 426f 7849 443a 202e 2e2e 0a20 2020  geBoxID: ....   
-0000c6e0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0000c6f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000c700: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-0000c710: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
-0000c720: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-0000c730: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-0000c740: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
-0000c750: 2c0a 2020 2020 2020 2020 6c61 6265 6c73  ,.        labels
-0000c760: 6574 3a20 6275 696c 7469 6e73 2e73 7472  et: builtins.str
-0000c770: 203d 202e 2e2e 2c0a 2020 2020 2920 2d3e   = ...,.    ) ->
-0000c780: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
-0000c790: 6566 2048 6173 4669 656c 6428 7365 6c66  ef HasField(self
-0000c7a0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-0000c7b0: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
-0000c7c0: 222c 2062 226b 6222 5d29 202d 3e20 6275  ", b"kb"]) -> bu
-0000c7d0: 696c 7469 6e73 2e62 6f6f 6c3a 202e 2e2e  iltins.bool: ...
-0000c7e0: 0a20 2020 2064 6566 2043 6c65 6172 4669  .    def ClearFi
-0000c7f0: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-0000c800: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-0000c810: 6572 616c 5b22 6b62 222c 2062 226b 6222  eral["kb", b"kb"
-0000c820: 2c20 226c 6162 656c 7365 7422 2c20 6222  , "labelset", b"
-0000c830: 6c61 6265 6c73 6574 225d 2920 2d3e 204e  labelset"]) -> N
-0000c840: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
-0000c850: 5f5f 5f47 6574 4c61 6265 6c53 6574 5265  ___GetLabelSetRe
-0000c860: 7175 6573 7420 3d20 4765 744c 6162 656c  quest = GetLabel
-0000c870: 5365 7452 6571 7565 7374 0a0a 4074 7970  SetRequest..@typ
-0000c880: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-0000c890: 4765 744c 6162 656c 5365 7452 6573 706f  GetLabelSetRespo
-0000c8a0: 6e73 6528 676f 6f67 6c65 2e70 726f 746f  nse(google.proto
-0000c8b0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
-0000c8c0: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
-0000c8d0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-0000c8e0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-0000c8f0: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-0000c900: 2063 6c61 7373 205f 5374 6174 7573 3a0a   class _Status:.
-0000c910: 2020 2020 2020 2020 5661 6c75 6554 7970          ValueTyp
-0000c920: 6520 3d20 7479 7069 6e67 2e4e 6577 5479  e = typing.NewTy
-0000c930: 7065 2822 5661 6c75 6554 7970 6522 2c20  pe("ValueType", 
-0000c940: 6275 696c 7469 6e73 2e69 6e74 290a 2020  builtins.int).  
-0000c950: 2020 2020 2020 563a 2074 7970 696e 675f        V: typing_
-0000c960: 6578 7465 6e73 696f 6e73 2e54 7970 6541  extensions.TypeA
-0000c970: 6c69 6173 203d 2056 616c 7565 5479 7065  lias = ValueType
-0000c980: 0a0a 2020 2020 636c 6173 7320 5f53 7461  ..    class _Sta
-0000c990: 7475 7345 6e75 6d54 7970 6557 7261 7070  tusEnumTypeWrapp
-0000c9a0: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
-0000c9b0: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
-0000c9c0: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
-0000c9d0: 6e75 6d54 7970 6557 7261 7070 6572 5b47  numTypeWrapper[G
-0000c9e0: 6574 4c61 6265 6c53 6574 5265 7370 6f6e  etLabelSetRespon
-0000c9f0: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-0000ca00: 5479 7065 5d2c 2062 7569 6c74 696e 732e  Type], builtins.
-0000ca10: 7479 7065 293a 0a20 2020 2020 2020 2044  type):.        D
-0000ca20: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
-0000ca30: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
-0000ca40: 6970 746f 722e 456e 756d 4465 7363 7269  iptor.EnumDescri
-0000ca50: 7074 6f72 0a20 2020 2020 2020 204f 4b3a  ptor.        OK:
-0000ca60: 2047 6574 4c61 6265 6c53 6574 5265 7370   GetLabelSetResp
-0000ca70: 6f6e 7365 2e5f 5374 6174 7573 2e56 616c  onse._Status.Val
-0000ca80: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
-0000ca90: 2020 2020 4e4f 5446 4f55 4e44 3a20 4765      NOTFOUND: Ge
-0000caa0: 744c 6162 656c 5365 7452 6573 706f 6e73  tLabelSetRespons
-0000cab0: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
-0000cac0: 7970 6520 2023 2031 0a0a 2020 2020 636c  ype  # 1..    cl
-0000cad0: 6173 7320 5374 6174 7573 285f 5374 6174  ass Status(_Stat
-0000cae0: 7573 2c20 6d65 7461 636c 6173 733d 5f53  us, metaclass=_S
-0000caf0: 7461 7475 7345 6e75 6d54 7970 6557 7261  tatusEnumTypeWra
-0000cb00: 7070 6572 293a 202e 2e2e 0a20 2020 204f  pper): ....    O
-0000cb10: 4b3a 2047 6574 4c61 6265 6c53 6574 5265  K: GetLabelSetRe
-0000cb20: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
-0000cb30: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
-0000cb40: 204e 4f54 464f 554e 443a 2047 6574 4c61   NOTFOUND: GetLa
-0000cb50: 6265 6c53 6574 5265 7370 6f6e 7365 2e53  belSetResponse.S
-0000cb60: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000cb70: 2023 2031 0a0a 2020 2020 4b42 5f46 4945   # 1..    KB_FIE
-0000cb80: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-0000cb90: 696e 732e 696e 740a 2020 2020 4c41 4245  ins.int.    LABE
-0000cba0: 4c53 4554 5f46 4945 4c44 5f4e 554d 4245  LSET_FIELD_NUMBE
-0000cbb0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000cbc0: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
-0000cbd0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000cbe0: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
-0000cbf0: 3a20 676c 6f62 616c 5f5f 5f47 6574 4c61  : global___GetLa
-0000cc00: 6265 6c53 6574 5265 7370 6f6e 7365 2e53  belSetResponse.S
-0000cc10: 7461 7475 732e 5661 6c75 6554 7970 650a  tatus.ValueType.
-0000cc20: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000cc30: 2020 6465 6620 6b62 2873 656c 6629 202d    def kb(self) -
-0000cc40: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
-0000cc50: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000cc60: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-0000cc70: 443a 202e 2e2e 0a20 2020 2040 7072 6f70  D: ....    @prop
-0000cc80: 6572 7479 0a20 2020 2064 6566 206c 6162  erty.    def lab
-0000cc90: 656c 7365 7428 7365 6c66 2920 2d3e 206e  elset(self) -> n
-0000cca0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000ccb0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000ccc0: 4c61 6265 6c53 6574 3a20 2e2e 2e0a 2020  LabelSet: ....  
-0000ccd0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-0000cce0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000ccf0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-0000cd00: 206b 623a 206e 7563 6c69 6164 625f 7072   kb: nucliadb_pr
-0000cd10: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-0000cd20: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
-0000cd30: 6f78 4944 207c 204e 6f6e 6520 3d20 2e2e  oxID | None = ..
-0000cd40: 2e2c 0a20 2020 2020 2020 206c 6162 656c  .,.        label
-0000cd50: 7365 743a 206e 7563 6c69 6164 625f 7072  set: nucliadb_pr
-0000cd60: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-0000cd70: 785f 7062 322e 4c61 6265 6c53 6574 207c  x_pb2.LabelSet |
-0000cd80: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-0000cd90: 2020 2020 2073 7461 7475 733a 2067 6c6f       status: glo
-0000cda0: 6261 6c5f 5f5f 4765 744c 6162 656c 5365  bal___GetLabelSe
-0000cdb0: 7452 6573 706f 6e73 652e 5374 6174 7573  tResponse.Status
-0000cdc0: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
-0000cdd0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0000cde0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-0000cdf0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-0000ce00: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-0000ce10: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
-0000ce20: 6222 2c20 226c 6162 656c 7365 7422 2c20  b", "labelset", 
-0000ce30: 6222 6c61 6265 6c73 6574 225d 2920 2d3e  b"labelset"]) ->
-0000ce40: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-0000ce50: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-0000ce60: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-0000ce70: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000ce80: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
-0000ce90: 6b62 222c 2022 6c61 6265 6c73 6574 222c  kb", "labelset",
-0000cea0: 2062 226c 6162 656c 7365 7422 2c20 2273   b"labelset", "s
-0000ceb0: 7461 7475 7322 2c20 6222 7374 6174 7573  tatus", b"status
-0000cec0: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-0000ced0: 0a0a 676c 6f62 616c 5f5f 5f47 6574 4c61  ..global___GetLa
-0000cee0: 6265 6c53 6574 5265 7370 6f6e 7365 203d  belSetResponse =
-0000cef0: 2047 6574 4c61 6265 6c53 6574 5265 7370   GetLabelSetResp
-0000cf00: 6f6e 7365 0a0a 4074 7970 696e 672e 6669  onse..@typing.fi
-0000cf10: 6e61 6c0a 636c 6173 7320 4765 7445 6e74  nal.class GetEnt
-0000cf20: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
-0000cf30: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-0000cf40: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000cf50: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000cf60: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000cf70: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000cf80: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-0000cf90: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
-0000cfa0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000cfb0: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
-0000cfc0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-0000cfd0: 740a 2020 2020 6772 6f75 703a 2062 7569  t.    group: bui
-0000cfe0: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
-0000cff0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000d000: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
-0000d010: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000d020: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-0000d030: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
-0000d040: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000d050: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000d060: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000d070: 2020 2020 6b62 3a20 6e75 636c 6961 6462      kb: nucliadb
-0000d080: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000d090: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
-0000d0a0: 6765 426f 7849 4420 7c20 4e6f 6e65 203d  geBoxID | None =
-0000d0b0: 202e 2e2e 2c0a 2020 2020 2020 2020 6772   ...,.        gr
-0000d0c0: 6f75 703a 2062 7569 6c74 696e 732e 7374  oup: builtins.st
-0000d0d0: 7220 3d20 2e2e 2e2c 0a20 2020 2029 202d  r = ...,.    ) -
-0000d0e0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000d0f0: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-0000d100: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000d110: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000d120: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
-0000d130: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000d140: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000d150: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000d160: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000d170: 7465 7261 6c5b 2267 726f 7570 222c 2062  teral["group", b
-0000d180: 2267 726f 7570 222c 2022 6b62 222c 2062  "group", "kb", b
-0000d190: 226b 6222 5d29 202d 3e20 4e6f 6e65 3a20  "kb"]) -> None: 
-0000d1a0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765  .....global___Ge
-0000d1b0: 7445 6e74 6974 6965 7347 726f 7570 5265  tEntitiesGroupRe
-0000d1c0: 7175 6573 7420 3d20 4765 7445 6e74 6974  quest = GetEntit
-0000d1d0: 6965 7347 726f 7570 5265 7175 6573 740a  iesGroupRequest.
-0000d1e0: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000d1f0: 6c61 7373 2047 6574 456e 7469 7469 6573  lass GetEntities
-0000d200: 4772 6f75 7052 6573 706f 6e73 6528 676f  GroupResponse(go
-0000d210: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-0000d220: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-0000d230: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-0000d240: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000d250: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-0000d260: 6970 746f 720a 0a20 2020 2063 6c61 7373  iptor..    class
-0000d270: 205f 5374 6174 7573 3a0a 2020 2020 2020   _Status:.      
-0000d280: 2020 5661 6c75 6554 7970 6520 3d20 7479    ValueType = ty
-0000d290: 7069 6e67 2e4e 6577 5479 7065 2822 5661  ping.NewType("Va
-0000d2a0: 6c75 6554 7970 6522 2c20 6275 696c 7469  lueType", builti
-0000d2b0: 6e73 2e69 6e74 290a 2020 2020 2020 2020  ns.int).        
-0000d2c0: 563a 2074 7970 696e 675f 6578 7465 6e73  V: typing_extens
-0000d2d0: 696f 6e73 2e54 7970 6541 6c69 6173 203d  ions.TypeAlias =
-0000d2e0: 2056 616c 7565 5479 7065 0a0a 2020 2020   ValueType..    
-0000d2f0: 636c 6173 7320 5f53 7461 7475 7345 6e75  class _StatusEnu
-0000d300: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
-0000d310: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-0000d320: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
-0000d330: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
-0000d340: 6557 7261 7070 6572 5b47 6574 456e 7469  eWrapper[GetEnti
-0000d350: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000d360: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
-0000d370: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
-0000d380: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
-0000d390: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000d3a0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000d3b0: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
-0000d3c0: 746f 720a 2020 2020 2020 2020 4f4b 3a20  tor.        OK: 
-0000d3d0: 4765 7445 6e74 6974 6965 7347 726f 7570  GetEntitiesGroup
-0000d3e0: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-0000d3f0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
-0000d400: 2020 2020 2020 2020 4b42 5f4e 4f54 5f46          KB_NOT_F
-0000d410: 4f55 4e44 3a20 4765 7445 6e74 6974 6965  OUND: GetEntitie
-0000d420: 7347 726f 7570 5265 7370 6f6e 7365 2e5f  sGroupResponse._
-0000d430: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000d440: 2020 2320 310a 2020 2020 2020 2020 454e    # 1.        EN
-0000d450: 5449 5449 4553 5f47 524f 5550 5f4e 4f54  TITIES_GROUP_NOT
-0000d460: 5f46 4f55 4e44 3a20 4765 7445 6e74 6974  _FOUND: GetEntit
-0000d470: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-0000d480: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
-0000d490: 7065 2020 2320 320a 2020 2020 2020 2020  pe  # 2.        
-0000d4a0: 4552 524f 523a 2047 6574 456e 7469 7469  ERROR: GetEntiti
-0000d4b0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
-0000d4c0: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
-0000d4d0: 6520 2023 2033 0a0a 2020 2020 636c 6173  e  # 3..    clas
-0000d4e0: 7320 5374 6174 7573 285f 5374 6174 7573  s Status(_Status
-0000d4f0: 2c20 6d65 7461 636c 6173 733d 5f53 7461  , metaclass=_Sta
-0000d500: 7475 7345 6e75 6d54 7970 6557 7261 7070  tusEnumTypeWrapp
-0000d510: 6572 293a 202e 2e2e 0a20 2020 204f 4b3a  er): ....    OK:
-0000d520: 2047 6574 456e 7469 7469 6573 4772 6f75   GetEntitiesGrou
-0000d530: 7052 6573 706f 6e73 652e 5374 6174 7573  pResponse.Status
-0000d540: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
-0000d550: 2020 2020 4b42 5f4e 4f54 5f46 4f55 4e44      KB_NOT_FOUND
-0000d560: 3a20 4765 7445 6e74 6974 6965 7347 726f  : GetEntitiesGro
-0000d570: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
-0000d580: 732e 5661 6c75 6554 7970 6520 2023 2031  s.ValueType  # 1
-0000d590: 0a20 2020 2045 4e54 4954 4945 535f 4752  .    ENTITIES_GR
-0000d5a0: 4f55 505f 4e4f 545f 464f 554e 443a 2047  OUP_NOT_FOUND: G
-0000d5b0: 6574 456e 7469 7469 6573 4772 6f75 7052  etEntitiesGroupR
-0000d5c0: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
-0000d5d0: 616c 7565 5479 7065 2020 2320 320a 2020  alueType  # 2.  
-0000d5e0: 2020 4552 524f 523a 2047 6574 456e 7469    ERROR: GetEnti
-0000d5f0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000d600: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000d610: 7065 2020 2320 330a 0a20 2020 204b 425f  pe  # 3..    KB_
-0000d620: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-0000d630: 696c 7469 6e73 2e69 6e74 0a20 2020 2047  iltins.int.    G
-0000d640: 524f 5550 5f46 4945 4c44 5f4e 554d 4245  ROUP_FIELD_NUMBE
-0000d650: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000d660: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
-0000d670: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000d680: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
-0000d690: 3a20 676c 6f62 616c 5f5f 5f47 6574 456e  : global___GetEn
-0000d6a0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-0000d6b0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
-0000d6c0: 5479 7065 0a20 2020 2040 7072 6f70 6572  Type.    @proper
-0000d6d0: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
-0000d6e0: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-0000d6f0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-0000d700: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-0000d710: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
-0000d720: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000d730: 6620 6772 6f75 7028 7365 6c66 2920 2d3e  f group(self) ->
-0000d740: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000d750: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000d760: 322e 456e 7469 7469 6573 4772 6f75 703a  2.EntitiesGroup:
-0000d770: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
-0000d780: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0000d790: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-0000d7a0: 2020 2020 2020 2020 6b62 3a20 6e75 636c          kb: nucl
-0000d7b0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000d7c0: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-0000d7d0: 776c 6564 6765 426f 7849 4420 7c20 4e6f  wledgeBoxID | No
-0000d7e0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-0000d7f0: 2020 6772 6f75 703a 206e 7563 6c69 6164    group: nucliad
-0000d800: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000d810: 6765 626f 785f 7062 322e 456e 7469 7469  gebox_pb2.Entiti
-0000d820: 6573 4772 6f75 7020 7c20 4e6f 6e65 203d  esGroup | None =
-0000d830: 202e 2e2e 2c0a 2020 2020 2020 2020 7374   ...,.        st
-0000d840: 6174 7573 3a20 676c 6f62 616c 5f5f 5f47  atus: global___G
-0000d850: 6574 456e 7469 7469 6573 4772 6f75 7052  etEntitiesGroupR
-0000d860: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
-0000d870: 616c 7565 5479 7065 203d 202e 2e2e 2c0a  alueType = ...,.
-0000d880: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-0000d890: 2e2e 0a20 2020 2064 6566 2048 6173 4669  ...    def HasFi
-0000d8a0: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-0000d8b0: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-0000d8c0: 6572 616c 5b22 6772 6f75 7022 2c20 6222  eral["group", b"
-0000d8d0: 6772 6f75 7022 2c20 226b 6222 2c20 6222  group", "kb", b"
-0000d8e0: 6b62 225d 2920 2d3e 2062 7569 6c74 696e  kb"]) -> builtin
-0000d8f0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-0000d900: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000d910: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000d920: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000d930: 2267 726f 7570 222c 2062 2267 726f 7570  "group", b"group
-0000d940: 222c 2022 6b62 222c 2062 226b 6222 2c20  ", "kb", b"kb", 
-0000d950: 2273 7461 7475 7322 2c20 6222 7374 6174  "status", b"stat
-0000d960: 7573 225d 2920 2d3e 204e 6f6e 653a 202e  us"]) -> None: .
-0000d970: 2e2e 0a0a 676c 6f62 616c 5f5f 5f47 6574  ....global___Get
-0000d980: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
-0000d990: 706f 6e73 6520 3d20 4765 7445 6e74 6974  ponse = GetEntit
-0000d9a0: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-0000d9b0: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-0000d9c0: 636c 6173 7320 4765 7456 6563 746f 7253  class GetVectorS
-0000d9d0: 6574 7352 6571 7565 7374 2867 6f6f 676c  etsRequest(googl
-0000d9e0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-0000d9f0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-0000da00: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-0000da10: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-0000da20: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-0000da30: 6f72 0a0a 2020 2020 4b42 5f46 4945 4c44  or..    KB_FIELD
-0000da40: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000da50: 732e 696e 740a 2020 2020 4070 726f 7065  s.int.    @prope
-0000da60: 7274 790a 2020 2020 6465 6620 6b62 2873  rty.    def kb(s
-0000da70: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
-0000da80: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000da90: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
-0000daa0: 6765 426f 7849 443a 202e 2e2e 0a20 2020  geBoxID: ....   
-0000dab0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0000dac0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000dad0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-0000dae0: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
-0000daf0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-0000db00: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-0000db10: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
-0000db20: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0000db30: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-0000db40: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-0000db50: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-0000db60: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
-0000db70: 6222 5d29 202d 3e20 6275 696c 7469 6e73  b"]) -> builtins
-0000db80: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2064  .bool: ....    d
-0000db90: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-0000dba0: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-0000dbb0: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-0000dbc0: 6b62 222c 2062 226b 6222 5d29 202d 3e20  kb", b"kb"]) -> 
-0000dbd0: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-0000dbe0: 6c5f 5f5f 4765 7456 6563 746f 7253 6574  l___GetVectorSet
-0000dbf0: 7352 6571 7565 7374 203d 2047 6574 5665  sRequest = GetVe
-0000dc00: 6374 6f72 5365 7473 5265 7175 6573 740a  ctorSetsRequest.
-0000dc10: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000dc20: 6c61 7373 2047 6574 5665 6374 6f72 5365  lass GetVectorSe
-0000dc30: 7473 5265 7370 6f6e 7365 2867 6f6f 676c  tsResponse(googl
-0000dc40: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-0000dc50: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-0000dc60: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-0000dc70: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-0000dc80: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-0000dc90: 6f72 0a0a 2020 2020 636c 6173 7320 5f53  or..    class _S
-0000dca0: 7461 7475 733a 0a20 2020 2020 2020 2056  tatus:.        V
-0000dcb0: 616c 7565 5479 7065 203d 2074 7970 696e  alueType = typin
-0000dcc0: 672e 4e65 7754 7970 6528 2256 616c 7565  g.NewType("Value
-0000dcd0: 5479 7065 222c 2062 7569 6c74 696e 732e  Type", builtins.
-0000dce0: 696e 7429 0a20 2020 2020 2020 2056 3a20  int).        V: 
-0000dcf0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
-0000dd00: 732e 5479 7065 416c 6961 7320 3d20 5661  s.TypeAlias = Va
-0000dd10: 6c75 6554 7970 650a 0a20 2020 2063 6c61  lueType..    cla
-0000dd20: 7373 205f 5374 6174 7573 456e 756d 5479  ss _StatusEnumTy
-0000dd30: 7065 5772 6170 7065 7228 676f 6f67 6c65  peWrapper(google
-0000dd40: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-0000dd50: 616c 2e65 6e75 6d5f 7479 7065 5f77 7261  al.enum_type_wra
-0000dd60: 7070 6572 2e5f 456e 756d 5479 7065 5772  pper._EnumTypeWr
-0000dd70: 6170 7065 725b 4765 7456 6563 746f 7253  apper[GetVectorS
-0000dd80: 6574 7352 6573 706f 6e73 652e 5f53 7461  etsResponse._Sta
-0000dd90: 7475 732e 5661 6c75 6554 7970 655d 2c20  tus.ValueType], 
-0000dda0: 6275 696c 7469 6e73 2e74 7970 6529 3a0a  builtins.type):.
-0000ddb0: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-0000ddc0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000ddd0: 6275 662e 6465 7363 7269 7074 6f72 2e45  buf.descriptor.E
-0000dde0: 6e75 6d44 6573 6372 6970 746f 720a 2020  numDescriptor.  
-0000ddf0: 2020 2020 2020 4f4b 3a20 4765 7456 6563        OK: GetVec
-0000de00: 746f 7253 6574 7352 6573 706f 6e73 652e  torSetsResponse.
-0000de10: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
-0000de20: 6520 2023 2030 0a20 2020 2020 2020 204e  e  # 0.        N
-0000de30: 4f54 464f 554e 443a 2047 6574 5665 6374  OTFOUND: GetVect
-0000de40: 6f72 5365 7473 5265 7370 6f6e 7365 2e5f  orSetsResponse._
-0000de50: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000de60: 2020 2320 310a 2020 2020 2020 2020 4552    # 1.        ER
-0000de70: 524f 523a 2047 6574 5665 6374 6f72 5365  ROR: GetVectorSe
-0000de80: 7473 5265 7370 6f6e 7365 2e5f 5374 6174  tsResponse._Stat
-0000de90: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000dea0: 320a 0a20 2020 2063 6c61 7373 2053 7461  2..    class Sta
-0000deb0: 7475 7328 5f53 7461 7475 732c 206d 6574  tus(_Status, met
-0000dec0: 6163 6c61 7373 3d5f 5374 6174 7573 456e  aclass=_StatusEn
-0000ded0: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
-0000dee0: 2e2e 2e0a 2020 2020 4f4b 3a20 4765 7456  ....    OK: GetV
-0000def0: 6563 746f 7253 6574 7352 6573 706f 6e73  ectorSetsRespons
-0000df00: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000df10: 7065 2020 2320 300a 2020 2020 4e4f 5446  pe  # 0.    NOTF
-0000df20: 4f55 4e44 3a20 4765 7456 6563 746f 7253  OUND: GetVectorS
-0000df30: 6574 7352 6573 706f 6e73 652e 5374 6174  etsResponse.Stat
-0000df40: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000df50: 310a 2020 2020 4552 524f 523a 2047 6574  1.    ERROR: Get
-0000df60: 5665 6374 6f72 5365 7473 5265 7370 6f6e  VectorSetsRespon
-0000df70: 7365 2e53 7461 7475 732e 5661 6c75 6554  se.Status.ValueT
-0000df80: 7970 6520 2023 2032 0a0a 2020 2020 4b42  ype  # 2..    KB
-0000df90: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000dfa0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000dfb0: 5645 4354 4f52 5345 5453 5f46 4945 4c44  VECTORSETS_FIELD
-0000dfc0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000dfd0: 732e 696e 740a 2020 2020 5354 4154 5553  s.int.    STATUS
-0000dfe0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000dff0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000e000: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
-0000e010: 5f47 6574 5665 6374 6f72 5365 7473 5265  _GetVectorSetsRe
-0000e020: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
-0000e030: 6c75 6554 7970 650a 2020 2020 4070 726f  lueType.    @pro
-0000e040: 7065 7274 790a 2020 2020 6465 6620 6b62  perty.    def kb
-0000e050: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-0000e060: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-0000e070: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
-0000e080: 6564 6765 426f 7849 443a 202e 2e2e 0a20  edgeBoxID: .... 
-0000e090: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000e0a0: 2064 6566 2076 6563 746f 7273 6574 7328   def vectorsets(
-0000e0b0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-0000e0c0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000e0d0: 6765 626f 785f 7062 322e 5665 6374 6f72  gebox_pb2.Vector
-0000e0e0: 5365 7473 3a20 2e2e 2e0a 2020 2020 6465  Sets: ....    de
-0000e0f0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0000e100: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000e110: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
-0000e120: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000e130: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000e140: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-0000e150: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000e160: 2020 2020 2020 2076 6563 746f 7273 6574         vectorset
-0000e170: 733a 206e 7563 6c69 6164 625f 7072 6f74  s: nucliadb_prot
-0000e180: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000e190: 7062 322e 5665 6374 6f72 5365 7473 207c  pb2.VectorSets |
-0000e1a0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-0000e1b0: 2020 2020 2073 7461 7475 733a 2067 6c6f       status: glo
-0000e1c0: 6261 6c5f 5f5f 4765 7456 6563 746f 7253  bal___GetVectorS
-0000e1d0: 6574 7352 6573 706f 6e73 652e 5374 6174  etsResponse.Stat
-0000e1e0: 7573 2e56 616c 7565 5479 7065 203d 202e  us.ValueType = .
-0000e1f0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
-0000e200: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
-0000e210: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
-0000e220: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-0000e230: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
-0000e240: 226b 6222 2c20 2276 6563 746f 7273 6574  "kb", "vectorset
-0000e250: 7322 2c20 6222 7665 6374 6f72 7365 7473  s", b"vectorsets
-0000e260: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
-0000e270: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 6465  bool: ....    de
-0000e280: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-0000e290: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000e2a0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000e2b0: 6222 2c20 6222 6b62 222c 2022 7374 6174  b", b"kb", "stat
-0000e2c0: 7573 222c 2062 2273 7461 7475 7322 2c20  us", b"status", 
-0000e2d0: 2276 6563 746f 7273 6574 7322 2c20 6222  "vectorsets", b"
-0000e2e0: 7665 6374 6f72 7365 7473 225d 2920 2d3e  vectorsets"]) ->
-0000e2f0: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-0000e300: 616c 5f5f 5f47 6574 5665 6374 6f72 5365  al___GetVectorSe
-0000e310: 7473 5265 7370 6f6e 7365 203d 2047 6574  tsResponse = Get
-0000e320: 5665 6374 6f72 5365 7473 5265 7370 6f6e  VectorSetsRespon
-0000e330: 7365 0a0a 4074 7970 696e 672e 6669 6e61  se..@typing.fina
-0000e340: 6c0a 636c 6173 7320 4465 6c56 6563 746f  l.class DelVecto
-0000e350: 7253 6574 5265 7175 6573 7428 676f 6f67  rSetRequest(goog
-0000e360: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-0000e370: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-0000e380: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000e390: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000e3a0: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-0000e3b0: 746f 720a 0a20 2020 204b 425f 4649 454c  tor..    KB_FIEL
-0000e3c0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000e3d0: 6e73 2e69 6e74 0a20 2020 2056 4543 544f  ns.int.    VECTO
-0000e3e0: 5253 4554 5f46 4945 4c44 5f4e 554d 4245  RSET_FIELD_NUMBE
-0000e3f0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000e400: 2020 2020 7665 6374 6f72 7365 743a 2062      vectorset: b
-0000e410: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
-0000e420: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000e430: 6620 6b62 2873 656c 6629 202d 3e20 6e75  f kb(self) -> nu
-0000e440: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-0000e450: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
-0000e460: 6e6f 776c 6564 6765 426f 7849 443a 202e  nowledgeBoxID: .
-0000e470: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-0000e480: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0000e490: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-0000e4a0: 2020 2020 2020 6b62 3a20 6e75 636c 6961        kb: nuclia
-0000e4b0: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-0000e4c0: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
-0000e4d0: 6564 6765 426f 7849 4420 7c20 4e6f 6e65  edgeBoxID | None
-0000e4e0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-0000e4f0: 7665 6374 6f72 7365 743a 2062 7569 6c74  vectorset: built
-0000e500: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-0000e510: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-0000e520: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
-0000e530: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-0000e540: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-0000e550: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
-0000e560: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-0000e570: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
-0000e580: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-0000e590: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-0000e5a0: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
-0000e5b0: 2c20 6222 6b62 222c 2022 7665 6374 6f72  , b"kb", "vector
-0000e5c0: 7365 7422 2c20 6222 7665 6374 6f72 7365  set", b"vectorse
-0000e5d0: 7422 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  t"]) -> None: ..
-0000e5e0: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4465 6c56  ...global___DelV
-0000e5f0: 6563 746f 7253 6574 5265 7175 6573 7420  ectorSetRequest 
-0000e600: 3d20 4465 6c56 6563 746f 7253 6574 5265  = DelVectorSetRe
-0000e610: 7175 6573 740a 0a40 7479 7069 6e67 2e66  quest..@typing.f
-0000e620: 696e 616c 0a63 6c61 7373 2053 6574 5665  inal.class SetVe
-0000e630: 6374 6f72 5365 7452 6571 7565 7374 2867  ctorSetRequest(g
-0000e640: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-0000e650: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-0000e660: 0a20 2020 2044 4553 4352 4950 544f 523a  .    DESCRIPTOR:
-0000e670: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-0000e680: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-0000e690: 7269 7074 6f72 0a0a 2020 2020 4b42 5f46  riptor..    KB_F
-0000e6a0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000e6b0: 6c74 696e 732e 696e 740a 2020 2020 4944  ltins.int.    ID
-0000e6c0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000e6d0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000e6e0: 5645 4354 4f52 5345 545f 4649 454c 445f  VECTORSET_FIELD_
-0000e6f0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-0000e700: 2e69 6e74 0a20 2020 2069 643a 2062 7569  .int.    id: bui
-0000e710: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
-0000e720: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e730: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
-0000e740: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000e750: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-0000e760: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
-0000e770: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000e780: 2020 2064 6566 2076 6563 746f 7273 6574     def vectorset
-0000e790: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-0000e7a0: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-0000e7b0: 6467 6562 6f78 5f70 6232 2e56 6563 746f  dgebox_pb2.Vecto
-0000e7c0: 7253 6574 3a20 2e2e 2e0a 2020 2020 6465  rSet: ....    de
-0000e7d0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0000e7e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000e7f0: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
-0000e800: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000e810: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000e820: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-0000e830: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000e840: 2020 2020 2020 2069 643a 2062 7569 6c74         id: built
-0000e850: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-0000e860: 2020 2020 2020 2076 6563 746f 7273 6574         vectorset
-0000e870: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-0000e880: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000e890: 6232 2e56 6563 746f 7253 6574 207c 204e  b2.VectorSet | N
-0000e8a0: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2029  one = ...,.    )
-0000e8b0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-0000e8c0: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-0000e8d0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000e8e0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000e8f0: 226b 6222 2c20 6222 6b62 222c 2022 7665  "kb", b"kb", "ve
-0000e900: 6374 6f72 7365 7422 2c20 6222 7665 6374  ctorset", b"vect
-0000e910: 6f72 7365 7422 5d29 202d 3e20 6275 696c  orset"]) -> buil
-0000e920: 7469 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20  tins.bool: .... 
-0000e930: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-0000e940: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-0000e950: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-0000e960: 616c 5b22 6964 222c 2062 2269 6422 2c20  al["id", b"id", 
-0000e970: 226b 6222 2c20 6222 6b62 222c 2022 7665  "kb", b"kb", "ve
-0000e980: 6374 6f72 7365 7422 2c20 6222 7665 6374  ctorset", b"vect
-0000e990: 6f72 7365 7422 5d29 202d 3e20 4e6f 6e65  orset"]) -> None
-0000e9a0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-0000e9b0: 5365 7456 6563 746f 7253 6574 5265 7175  SetVectorSetRequ
-0000e9c0: 6573 7420 3d20 5365 7456 6563 746f 7253  est = SetVectorS
-0000e9d0: 6574 5265 7175 6573 740a 0a40 7479 7069  etRequest..@typi
-0000e9e0: 6e67 2e66 696e 616c 0a63 6c61 7373 204f  ng.final.class O
-0000e9f0: 7053 7461 7475 7357 7269 7465 7228 676f  pStatusWriter(go
-0000ea00: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-0000ea10: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-0000ea20: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-0000ea30: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000ea40: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-0000ea50: 6970 746f 720a 0a20 2020 2063 6c61 7373  iptor..    class
-0000ea60: 205f 5374 6174 7573 3a0a 2020 2020 2020   _Status:.      
-0000ea70: 2020 5661 6c75 6554 7970 6520 3d20 7479    ValueType = ty
-0000ea80: 7069 6e67 2e4e 6577 5479 7065 2822 5661  ping.NewType("Va
-0000ea90: 6c75 6554 7970 6522 2c20 6275 696c 7469  lueType", builti
-0000eaa0: 6e73 2e69 6e74 290a 2020 2020 2020 2020  ns.int).        
-0000eab0: 563a 2074 7970 696e 675f 6578 7465 6e73  V: typing_extens
-0000eac0: 696f 6e73 2e54 7970 6541 6c69 6173 203d  ions.TypeAlias =
-0000ead0: 2056 616c 7565 5479 7065 0a0a 2020 2020   ValueType..    
-0000eae0: 636c 6173 7320 5f53 7461 7475 7345 6e75  class _StatusEnu
-0000eaf0: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
-0000eb00: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-0000eb10: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
-0000eb20: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
-0000eb30: 6557 7261 7070 6572 5b4f 7053 7461 7475  eWrapper[OpStatu
-0000eb40: 7357 7269 7465 722e 5f53 7461 7475 732e  sWriter._Status.
-0000eb50: 5661 6c75 6554 7970 655d 2c20 6275 696c  ValueType], buil
-0000eb60: 7469 6e73 2e74 7970 6529 3a0a 2020 2020  tins.type):.    
-0000eb70: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-0000eb80: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000eb90: 6465 7363 7269 7074 6f72 2e45 6e75 6d44  descriptor.EnumD
-0000eba0: 6573 6372 6970 746f 720a 2020 2020 2020  escriptor.      
-0000ebb0: 2020 4f4b 3a20 4f70 5374 6174 7573 5772    OK: OpStatusWr
-0000ebc0: 6974 6572 2e5f 5374 6174 7573 2e56 616c  iter._Status.Val
-0000ebd0: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
-0000ebe0: 2020 2020 4552 524f 523a 204f 7053 7461      ERROR: OpSta
-0000ebf0: 7475 7357 7269 7465 722e 5f53 7461 7475  tusWriter._Statu
-0000ec00: 732e 5661 6c75 6554 7970 6520 2023 2031  s.ValueType  # 1
-0000ec10: 0a20 2020 2020 2020 204e 4f54 464f 554e  .        NOTFOUN
-0000ec20: 443a 204f 7053 7461 7475 7357 7269 7465  D: OpStatusWrite
-0000ec30: 722e 5f53 7461 7475 732e 5661 6c75 6554  r._Status.ValueT
-0000ec40: 7970 6520 2023 2032 0a0a 2020 2020 636c  ype  # 2..    cl
-0000ec50: 6173 7320 5374 6174 7573 285f 5374 6174  ass Status(_Stat
-0000ec60: 7573 2c20 6d65 7461 636c 6173 733d 5f53  us, metaclass=_S
-0000ec70: 7461 7475 7345 6e75 6d54 7970 6557 7261  tatusEnumTypeWra
-0000ec80: 7070 6572 293a 202e 2e2e 0a20 2020 204f  pper): ....    O
-0000ec90: 4b3a 204f 7053 7461 7475 7357 7269 7465  K: OpStatusWrite
-0000eca0: 722e 5374 6174 7573 2e56 616c 7565 5479  r.Status.ValueTy
-0000ecb0: 7065 2020 2320 300a 2020 2020 4552 524f  pe  # 0.    ERRO
-0000ecc0: 523a 204f 7053 7461 7475 7357 7269 7465  R: OpStatusWrite
-0000ecd0: 722e 5374 6174 7573 2e56 616c 7565 5479  r.Status.ValueTy
-0000ece0: 7065 2020 2320 310a 2020 2020 4e4f 5446  pe  # 1.    NOTF
-0000ecf0: 4f55 4e44 3a20 4f70 5374 6174 7573 5772  OUND: OpStatusWr
-0000ed00: 6974 6572 2e53 7461 7475 732e 5661 6c75  iter.Status.Valu
-0000ed10: 6554 7970 6520 2023 2032 0a0a 2020 2020  eType  # 2..    
-0000ed20: 5354 4154 5553 5f46 4945 4c44 5f4e 554d  STATUS_FIELD_NUM
-0000ed30: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-0000ed40: 740a 2020 2020 7374 6174 7573 3a20 676c  t.    status: gl
-0000ed50: 6f62 616c 5f5f 5f4f 7053 7461 7475 7357  obal___OpStatusW
-0000ed60: 7269 7465 722e 5374 6174 7573 2e56 616c  riter.Status.Val
-0000ed70: 7565 5479 7065 0a20 2020 2064 6566 205f  ueType.    def _
-0000ed80: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000ed90: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-0000eda0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-0000edb0: 3a20 676c 6f62 616c 5f5f 5f4f 7053 7461  : global___OpSta
-0000edc0: 7475 7357 7269 7465 722e 5374 6174 7573  tusWriter.Status
-0000edd0: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
-0000ede0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0000edf0: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-0000ee00: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-0000ee10: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-0000ee20: 2e4c 6974 6572 616c 5b22 7374 6174 7573  .Literal["status
-0000ee30: 222c 2062 2273 7461 7475 7322 5d29 202d  ", b"status"]) -
-0000ee40: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
-0000ee50: 6261 6c5f 5f5f 4f70 5374 6174 7573 5772  bal___OpStatusWr
-0000ee60: 6974 6572 203d 204f 7053 7461 7475 7357  iter = OpStatusW
-0000ee70: 7269 7465 720a 0a40 7479 7069 6e67 2e66  riter..@typing.f
-0000ee80: 696e 616c 0a63 6c61 7373 204e 6f74 6966  inal.class Notif
-0000ee90: 6963 6174 696f 6e28 676f 6f67 6c65 2e70  ication(google.p
-0000eea0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000eeb0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-0000eec0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000eed0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000eee0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000eef0: 0a20 2020 2063 6c61 7373 205f 4163 7469  .    class _Acti
-0000ef00: 6f6e 3a0a 2020 2020 2020 2020 5661 6c75  on:.        Valu
-0000ef10: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
-0000ef20: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
-0000ef30: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
-0000ef40: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
-0000ef50: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
-0000ef60: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
-0000ef70: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
-0000ef80: 5f41 6374 696f 6e45 6e75 6d54 7970 6557  _ActionEnumTypeW
-0000ef90: 7261 7070 6572 2867 6f6f 676c 652e 7072  rapper(google.pr
-0000efa0: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-0000efb0: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
-0000efc0: 722e 5f45 6e75 6d54 7970 6557 7261 7070  r._EnumTypeWrapp
-0000efd0: 6572 5b4e 6f74 6966 6963 6174 696f 6e2e  er[Notification.
-0000efe0: 5f41 6374 696f 6e2e 5661 6c75 6554 7970  _Action.ValueTyp
-0000eff0: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
-0000f000: 6529 3a0a 2020 2020 2020 2020 4445 5343  e):.        DESC
-0000f010: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-0000f020: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-0000f030: 6f72 2e45 6e75 6d44 6573 6372 6970 746f  or.EnumDescripto
-0000f040: 720a 2020 2020 2020 2020 434f 4d4d 4954  r.        COMMIT
-0000f050: 3a20 4e6f 7469 6669 6361 7469 6f6e 2e5f  : Notification._
-0000f060: 4163 7469 6f6e 2e56 616c 7565 5479 7065  Action.ValueType
-0000f070: 2020 2320 300a 2020 2020 2020 2020 4142    # 0.        AB
-0000f080: 4f52 543a 204e 6f74 6966 6963 6174 696f  ORT: Notificatio
-0000f090: 6e2e 5f41 6374 696f 6e2e 5661 6c75 6554  n._Action.ValueT
-0000f0a0: 7970 6520 2023 2031 0a20 2020 2020 2020  ype  # 1.       
-0000f0b0: 2049 4e44 4558 4544 3a20 4e6f 7469 6669   INDEXED: Notifi
-0000f0c0: 6361 7469 6f6e 2e5f 4163 7469 6f6e 2e56  cation._Action.V
-0000f0d0: 616c 7565 5479 7065 2020 2320 320a 0a20  alueType  # 2.. 
-0000f0e0: 2020 2063 6c61 7373 2041 6374 696f 6e28     class Action(
-0000f0f0: 5f41 6374 696f 6e2c 206d 6574 6163 6c61  _Action, metacla
-0000f100: 7373 3d5f 4163 7469 6f6e 456e 756d 5479  ss=_ActionEnumTy
-0000f110: 7065 5772 6170 7065 7229 3a20 2e2e 2e0a  peWrapper): ....
-0000f120: 2020 2020 434f 4d4d 4954 3a20 4e6f 7469      COMMIT: Noti
-0000f130: 6669 6361 7469 6f6e 2e41 6374 696f 6e2e  fication.Action.
-0000f140: 5661 6c75 6554 7970 6520 2023 2030 0a20  ValueType  # 0. 
-0000f150: 2020 2041 424f 5254 3a20 4e6f 7469 6669     ABORT: Notifi
-0000f160: 6361 7469 6f6e 2e41 6374 696f 6e2e 5661  cation.Action.Va
-0000f170: 6c75 6554 7970 6520 2023 2031 0a20 2020  lueType  # 1.   
-0000f180: 2049 4e44 4558 4544 3a20 4e6f 7469 6669   INDEXED: Notifi
-0000f190: 6361 7469 6f6e 2e41 6374 696f 6e2e 5661  cation.Action.Va
-0000f1a0: 6c75 6554 7970 6520 2023 2032 0a0a 2020  lueType  # 2..  
-0000f1b0: 2020 636c 6173 7320 5f57 7269 7465 5479    class _WriteTy
-0000f1c0: 7065 3a0a 2020 2020 2020 2020 5661 6c75  pe:.        Valu
-0000f1d0: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
-0000f1e0: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
-0000f1f0: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
-0000f200: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
-0000f210: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
-0000f220: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
-0000f230: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
-0000f240: 5f57 7269 7465 5479 7065 456e 756d 5479  _WriteTypeEnumTy
-0000f250: 7065 5772 6170 7065 7228 676f 6f67 6c65  peWrapper(google
-0000f260: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-0000f270: 616c 2e65 6e75 6d5f 7479 7065 5f77 7261  al.enum_type_wra
-0000f280: 7070 6572 2e5f 456e 756d 5479 7065 5772  pper._EnumTypeWr
-0000f290: 6170 7065 725b 4e6f 7469 6669 6361 7469  apper[Notificati
-0000f2a0: 6f6e 2e5f 5772 6974 6554 7970 652e 5661  on._WriteType.Va
-0000f2b0: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
-0000f2c0: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
-0000f2d0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000f2e0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000f2f0: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
-0000f300: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
-0000f310: 554e 5345 543a 204e 6f74 6966 6963 6174  UNSET: Notificat
-0000f320: 696f 6e2e 5f57 7269 7465 5479 7065 2e56  ion._WriteType.V
-0000f330: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
-0000f340: 2020 2020 2020 4352 4541 5445 443a 204e        CREATED: N
-0000f350: 6f74 6966 6963 6174 696f 6e2e 5f57 7269  otification._Wri
-0000f360: 7465 5479 7065 2e56 616c 7565 5479 7065  teType.ValueType
-0000f370: 2020 2320 310a 2020 2020 2020 2020 4d4f    # 1.        MO
-0000f380: 4449 4649 4544 3a20 4e6f 7469 6669 6361  DIFIED: Notifica
-0000f390: 7469 6f6e 2e5f 5772 6974 6554 7970 652e  tion._WriteType.
-0000f3a0: 5661 6c75 6554 7970 6520 2023 2032 0a20  ValueType  # 2. 
-0000f3b0: 2020 2020 2020 2044 454c 4554 4544 3a20         DELETED: 
-0000f3c0: 4e6f 7469 6669 6361 7469 6f6e 2e5f 5772  Notification._Wr
-0000f3d0: 6974 6554 7970 652e 5661 6c75 6554 7970  iteType.ValueTyp
-0000f3e0: 6520 2023 2033 0a0a 2020 2020 636c 6173  e  # 3..    clas
-0000f3f0: 7320 5772 6974 6554 7970 6528 5f57 7269  s WriteType(_Wri
-0000f400: 7465 5479 7065 2c20 6d65 7461 636c 6173  teType, metaclas
-0000f410: 733d 5f57 7269 7465 5479 7065 456e 756d  s=_WriteTypeEnum
-0000f420: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
-0000f430: 2e0a 2020 2020 554e 5345 543a 204e 6f74  ..    UNSET: Not
-0000f440: 6966 6963 6174 696f 6e2e 5772 6974 6554  ification.WriteT
-0000f450: 7970 652e 5661 6c75 6554 7970 6520 2023  ype.ValueType  #
-0000f460: 2030 0a20 2020 2043 5245 4154 4544 3a20   0.    CREATED: 
-0000f470: 4e6f 7469 6669 6361 7469 6f6e 2e57 7269  Notification.Wri
-0000f480: 7465 5479 7065 2e56 616c 7565 5479 7065  teType.ValueType
-0000f490: 2020 2320 310a 2020 2020 4d4f 4449 4649    # 1.    MODIFI
-0000f4a0: 4544 3a20 4e6f 7469 6669 6361 7469 6f6e  ED: Notification
-0000f4b0: 2e57 7269 7465 5479 7065 2e56 616c 7565  .WriteType.Value
-0000f4c0: 5479 7065 2020 2320 320a 2020 2020 4445  Type  # 2.    DE
-0000f4d0: 4c45 5445 443a 204e 6f74 6966 6963 6174  LETED: Notificat
-0000f4e0: 696f 6e2e 5772 6974 6554 7970 652e 5661  ion.WriteType.Va
-0000f4f0: 6c75 6554 7970 6520 2023 2033 0a0a 2020  lueType  # 3..  
-0000f500: 2020 5041 5254 4954 494f 4e5f 4649 454c    PARTITION_FIEL
-0000f510: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000f520: 6e73 2e69 6e74 0a20 2020 204d 554c 5449  ns.int.    MULTI
-0000f530: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000f540: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000f550: 5555 4944 5f46 4945 4c44 5f4e 554d 4245  UUID_FIELD_NUMBE
-0000f560: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000f570: 2020 2020 4b42 4944 5f46 4945 4c44 5f4e      KBID_FIELD_N
-0000f580: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-0000f590: 696e 740a 2020 2020 5345 5149 445f 4649  int.    SEQID_FI
-0000f5a0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000f5b0: 7469 6e73 2e69 6e74 0a20 2020 2041 4354  tins.int.    ACT
-0000f5c0: 494f 4e5f 4649 454c 445f 4e55 4d42 4552  ION_FIELD_NUMBER
-0000f5d0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-0000f5e0: 2020 2057 5249 5445 5f54 5950 455f 4649     WRITE_TYPE_FI
-0000f5f0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000f600: 7469 6e73 2e69 6e74 0a20 2020 204d 4553  tins.int.    MES
-0000f610: 5341 4745 5f46 4945 4c44 5f4e 554d 4245  SAGE_FIELD_NUMBE
-0000f620: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000f630: 2020 2020 534f 5552 4345 5f46 4945 4c44      SOURCE_FIELD
-0000f640: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000f650: 732e 696e 740a 2020 2020 5052 4f43 4553  s.int.    PROCES
-0000f660: 5349 4e47 5f45 5252 4f52 535f 4649 454c  SING_ERRORS_FIEL
-0000f670: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000f680: 6e73 2e69 6e74 0a20 2020 204d 4553 5341  ns.int.    MESSA
-0000f690: 4745 5f41 5544 4954 5f46 4945 4c44 5f4e  GE_AUDIT_FIELD_N
-0000f6a0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-0000f6b0: 696e 740a 2020 2020 7061 7274 6974 696f  int.    partitio
-0000f6c0: 6e3a 2062 7569 6c74 696e 732e 696e 740a  n: builtins.int.
-0000f6d0: 2020 2020 6d75 6c74 693a 2062 7569 6c74      multi: built
-0000f6e0: 696e 732e 7374 720a 2020 2020 7575 6964  ins.str.    uuid
-0000f6f0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-0000f700: 2020 206b 6269 643a 2062 7569 6c74 696e     kbid: builtin
-0000f710: 732e 7374 720a 2020 2020 7365 7169 643a  s.str.    seqid:
-0000f720: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-0000f730: 2020 6163 7469 6f6e 3a20 676c 6f62 616c    action: global
-0000f740: 5f5f 5f4e 6f74 6966 6963 6174 696f 6e2e  ___Notification.
-0000f750: 4163 7469 6f6e 2e56 616c 7565 5479 7065  Action.ValueType
-0000f760: 0a20 2020 2077 7269 7465 5f74 7970 653a  .    write_type:
-0000f770: 2067 6c6f 6261 6c5f 5f5f 4e6f 7469 6669   global___Notifi
-0000f780: 6361 7469 6f6e 2e57 7269 7465 5479 7065  cation.WriteType
-0000f790: 2e56 616c 7565 5479 7065 0a20 2020 2073  .ValueType.    s
-0000f7a0: 6f75 7263 653a 2067 6c6f 6261 6c5f 5f5f  ource: global___
-0000f7b0: 4e6f 7469 6669 6361 7469 6f6e 536f 7572  NotificationSour
-0000f7c0: 6365 2e56 616c 7565 5479 7065 0a20 2020  ce.ValueType.   
-0000f7d0: 2070 726f 6365 7373 696e 675f 6572 726f   processing_erro
-0000f7e0: 7273 3a20 6275 696c 7469 6e73 2e62 6f6f  rs: builtins.boo
-0000f7f0: 6c0a 2020 2020 4070 726f 7065 7274 790a  l.    @property.
-0000f800: 2020 2020 6465 6620 6d65 7373 6167 6528      def message(
-0000f810: 7365 6c66 2920 2d3e 2067 6c6f 6261 6c5f  self) -> global_
-0000f820: 5f5f 4272 6f6b 6572 4d65 7373 6167 653a  __BrokerMessage:
-0000f830: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
-0000f840: 7479 0a20 2020 2064 6566 206d 6573 7361  ty.    def messa
-0000f850: 6765 5f61 7564 6974 2873 656c 6629 202d  ge_audit(self) -
-0000f860: 3e20 676c 6f62 616c 5f5f 5f41 7564 6974  > global___Audit
-0000f870: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
-0000f880: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0000f890: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-0000f8a0: 0a20 2020 2020 2020 2070 6172 7469 7469  .        partiti
-0000f8b0: 6f6e 3a20 6275 696c 7469 6e73 2e69 6e74  on: builtins.int
-0000f8c0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-0000f8d0: 6d75 6c74 693a 2062 7569 6c74 696e 732e  multi: builtins.
-0000f8e0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-0000f8f0: 2020 2075 7569 643a 2062 7569 6c74 696e     uuid: builtin
-0000f900: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-0000f910: 2020 2020 206b 6269 643a 2062 7569 6c74       kbid: built
-0000f920: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-0000f930: 2020 2020 2020 2073 6571 6964 3a20 6275         seqid: bu
-0000f940: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
-0000f950: 2c0a 2020 2020 2020 2020 6163 7469 6f6e  ,.        action
-0000f960: 3a20 676c 6f62 616c 5f5f 5f4e 6f74 6966  : global___Notif
-0000f970: 6963 6174 696f 6e2e 4163 7469 6f6e 2e56  ication.Action.V
-0000f980: 616c 7565 5479 7065 203d 202e 2e2e 2c0a  alueType = ...,.
-0000f990: 2020 2020 2020 2020 7772 6974 655f 7479          write_ty
-0000f9a0: 7065 3a20 676c 6f62 616c 5f5f 5f4e 6f74  pe: global___Not
-0000f9b0: 6966 6963 6174 696f 6e2e 5772 6974 6554  ification.WriteT
-0000f9c0: 7970 652e 5661 6c75 6554 7970 6520 3d20  ype.ValueType = 
-0000f9d0: 2e2e 2e2c 0a20 2020 2020 2020 206d 6573  ...,.        mes
-0000f9e0: 7361 6765 3a20 676c 6f62 616c 5f5f 5f42  sage: global___B
-0000f9f0: 726f 6b65 724d 6573 7361 6765 207c 204e  rokerMessage | N
-0000fa00: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-0000fa10: 2020 2073 6f75 7263 653a 2067 6c6f 6261     source: globa
-0000fa20: 6c5f 5f5f 4e6f 7469 6669 6361 7469 6f6e  l___Notification
-0000fa30: 536f 7572 6365 2e56 616c 7565 5479 7065  Source.ValueType
-0000fa40: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-0000fa50: 7072 6f63 6573 7369 6e67 5f65 7272 6f72  processing_error
-0000fa60: 733a 2062 7569 6c74 696e 732e 626f 6f6c  s: builtins.bool
-0000fa70: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-0000fa80: 6d65 7373 6167 655f 6175 6469 743a 2067  message_audit: g
-0000fa90: 6c6f 6261 6c5f 5f5f 4175 6469 7420 7c20  lobal___Audit | 
-0000faa0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-0000fab0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000fac0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-0000fad0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-0000fae0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-0000faf0: 5b22 6d65 7373 6167 6522 2c20 6222 6d65  ["message", b"me
-0000fb00: 7373 6167 6522 2c20 226d 6573 7361 6765  ssage", "message
-0000fb10: 5f61 7564 6974 222c 2062 226d 6573 7361  _audit", b"messa
-0000fb20: 6765 5f61 7564 6974 225d 2920 2d3e 2062  ge_audit"]) -> b
-0000fb30: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000fb40: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000fb50: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000fb60: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000fb70: 7465 7261 6c5b 2261 6374 696f 6e22 2c20  teral["action", 
-0000fb80: 6222 6163 7469 6f6e 222c 2022 6b62 6964  b"action", "kbid
-0000fb90: 222c 2062 226b 6269 6422 2c20 226d 6573  ", b"kbid", "mes
-0000fba0: 7361 6765 222c 2062 226d 6573 7361 6765  sage", b"message
-0000fbb0: 222c 2022 6d65 7373 6167 655f 6175 6469  ", "message_audi
-0000fbc0: 7422 2c20 6222 6d65 7373 6167 655f 6175  t", b"message_au
-0000fbd0: 6469 7422 2c20 226d 756c 7469 222c 2062  dit", "multi", b
-0000fbe0: 226d 756c 7469 222c 2022 7061 7274 6974  "multi", "partit
-0000fbf0: 696f 6e22 2c20 6222 7061 7274 6974 696f  ion", b"partitio
-0000fc00: 6e22 2c20 2270 726f 6365 7373 696e 675f  n", "processing_
-0000fc10: 6572 726f 7273 222c 2062 2270 726f 6365  errors", b"proce
-0000fc20: 7373 696e 675f 6572 726f 7273 222c 2022  ssing_errors", "
-0000fc30: 7365 7169 6422 2c20 6222 7365 7169 6422  seqid", b"seqid"
-0000fc40: 2c20 2273 6f75 7263 6522 2c20 6222 736f  , "source", b"so
-0000fc50: 7572 6365 222c 2022 7575 6964 222c 2062  urce", "uuid", b
-0000fc60: 2275 7569 6422 2c20 2277 7269 7465 5f74  "uuid", "write_t
-0000fc70: 7970 6522 2c20 6222 7772 6974 655f 7479  ype", b"write_ty
-0000fc80: 7065 225d 2920 2d3e 204e 6f6e 653a 202e  pe"]) -> None: .
-0000fc90: 2e2e 0a0a 676c 6f62 616c 5f5f 5f4e 6f74  ....global___Not
-0000fca0: 6966 6963 6174 696f 6e20 3d20 4e6f 7469  ification = Noti
-0000fcb0: 6669 6361 7469 6f6e 0a0a 4074 7970 696e  fication..@typin
-0000fcc0: 672e 6669 6e61 6c0a 636c 6173 7320 4d65  g.final.class Me
-0000fcd0: 6d62 6572 2867 6f6f 676c 652e 7072 6f74  mber(google.prot
-0000fce0: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-0000fcf0: 7361 6765 293a 0a20 2020 2022 2222 5468  sage):.    """Th
-0000fd00: 6520 6d65 6d62 6572 2069 6e66 6f72 6d61  e member informa
-0000fd10: 7469 6f6e 2e22 2222 0a0a 2020 2020 4445  tion."""..    DE
-0000fd20: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000fd30: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000fd40: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000fd50: 0a20 2020 2063 6c61 7373 205f 5479 7065  .    class _Type
-0000fd60: 3a0a 2020 2020 2020 2020 5661 6c75 6554  :.        ValueT
-0000fd70: 7970 6520 3d20 7479 7069 6e67 2e4e 6577  ype = typing.New
-0000fd80: 5479 7065 2822 5661 6c75 6554 7970 6522  Type("ValueType"
-0000fd90: 2c20 6275 696c 7469 6e73 2e69 6e74 290a  , builtins.int).
-0000fda0: 2020 2020 2020 2020 563a 2074 7970 696e          V: typin
-0000fdb0: 675f 6578 7465 6e73 696f 6e73 2e54 7970  g_extensions.Typ
-0000fdc0: 6541 6c69 6173 203d 2056 616c 7565 5479  eAlias = ValueTy
-0000fdd0: 7065 0a0a 2020 2020 636c 6173 7320 5f54  pe..    class _T
-0000fde0: 7970 6545 6e75 6d54 7970 6557 7261 7070  ypeEnumTypeWrapp
-0000fdf0: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
-0000fe00: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
-0000fe10: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
-0000fe20: 6e75 6d54 7970 6557 7261 7070 6572 5b4d  numTypeWrapper[M
-0000fe30: 656d 6265 722e 5f54 7970 652e 5661 6c75  ember._Type.Valu
-0000fe40: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
-0000fe50: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
-0000fe60: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-0000fe70: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-0000fe80: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
-0000fe90: 6970 746f 720a 2020 2020 2020 2020 494f  iptor.        IO
-0000fea0: 3a20 4d65 6d62 6572 2e5f 5479 7065 2e56  : Member._Type.V
-0000feb0: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
-0000fec0: 2020 2020 2020 5345 4152 4348 3a20 4d65        SEARCH: Me
-0000fed0: 6d62 6572 2e5f 5479 7065 2e56 616c 7565  mber._Type.Value
-0000fee0: 5479 7065 2020 2320 310a 2020 2020 2020  Type  # 1.      
-0000fef0: 2020 494e 4745 5354 3a20 4d65 6d62 6572    INGEST: Member
-0000ff00: 2e5f 5479 7065 2e56 616c 7565 5479 7065  ._Type.ValueType
-0000ff10: 2020 2320 320a 2020 2020 2020 2020 5452    # 2.        TR
-0000ff20: 4149 4e3a 204d 656d 6265 722e 5f54 7970  AIN: Member._Typ
-0000ff30: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
-0000ff40: 0a20 2020 2020 2020 2055 4e4b 4e4f 574e  .        UNKNOWN
-0000ff50: 3a20 4d65 6d62 6572 2e5f 5479 7065 2e56  : Member._Type.V
-0000ff60: 616c 7565 5479 7065 2020 2320 340a 0a20  alueType  # 4.. 
-0000ff70: 2020 2063 6c61 7373 2054 7970 6528 5f54     class Type(_T
-0000ff80: 7970 652c 206d 6574 6163 6c61 7373 3d5f  ype, metaclass=_
-0000ff90: 5479 7065 456e 756d 5479 7065 5772 6170  TypeEnumTypeWrap
-0000ffa0: 7065 7229 3a20 2e2e 2e0a 2020 2020 494f  per): ....    IO
-0000ffb0: 3a20 4d65 6d62 6572 2e54 7970 652e 5661  : Member.Type.Va
-0000ffc0: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
-0000ffd0: 2053 4541 5243 483a 204d 656d 6265 722e   SEARCH: Member.
-0000ffe0: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
-0000fff0: 2320 310a 2020 2020 494e 4745 5354 3a20  # 1.    INGEST: 
-00010000: 4d65 6d62 6572 2e54 7970 652e 5661 6c75  Member.Type.Valu
-00010010: 6554 7970 6520 2023 2032 0a20 2020 2054  eType  # 2.    T
-00010020: 5241 494e 3a20 4d65 6d62 6572 2e54 7970  RAIN: Member.Typ
-00010030: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
-00010040: 0a20 2020 2055 4e4b 4e4f 574e 3a20 4d65  .    UNKNOWN: Me
-00010050: 6d62 6572 2e54 7970 652e 5661 6c75 6554  mber.Type.ValueT
-00010060: 7970 6520 2023 2034 0a0a 2020 2020 4944  ype  # 4..    ID
-00010070: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00010080: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00010090: 4c49 5354 454e 5f41 4444 5245 5353 5f46  LISTEN_ADDRESS_F
-000100a0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-000100b0: 6c74 696e 732e 696e 740a 2020 2020 4953  ltins.int.    IS
-000100c0: 5f53 454c 465f 4649 454c 445f 4e55 4d42  _SELF_FIELD_NUMB
-000100d0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-000100e0: 0a20 2020 2054 5950 455f 4649 454c 445f  .    TYPE_FIELD_
-000100f0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00010100: 2e69 6e74 0a20 2020 2044 554d 4d59 5f46  .int.    DUMMY_F
-00010110: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00010120: 6c74 696e 732e 696e 740a 2020 2020 4c4f  ltins.int.    LO
-00010130: 4144 5f53 434f 5245 5f46 4945 4c44 5f4e  AD_SCORE_FIELD_N
-00010140: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00010150: 696e 740a 2020 2020 5348 4152 445f 434f  int.    SHARD_CO
-00010160: 554e 545f 4649 454c 445f 4e55 4d42 4552  UNT_FIELD_NUMBER
-00010170: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00010180: 2020 2050 5249 4d41 5259 5f49 445f 4649     PRIMARY_ID_FI
-00010190: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000101a0: 7469 6e73 2e69 6e74 0a20 2020 2069 643a  tins.int.    id:
-000101b0: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-000101c0: 2020 2222 222f 204d 656d 6265 7220 4944    """/ Member ID
-000101d0: 2ee3 8080 4120 7374 7269 6e67 206f 6620  ....A string of 
-000101e0: 7468 6520 5555 4944 2e22 2222 0a20 2020  the UUID.""".   
-000101f0: 206c 6973 7465 6e5f 6164 6472 6573 733a   listen_address:
-00010200: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00010210: 2020 2222 222f 2043 6c75 7374 6572 206c    """/ Cluster l
-00010220: 6973 7465 6e20 6164 6472 6573 732e 2073  isten address. s
-00010230: 7472 696e 6720 6f66 2049 5020 616e 6420  tring of IP and 
-00010240: 706f 7274 206e 756d 6265 722e 0a20 2020  port number..   
-00010250: 202f 2045 2e67 2e20 3132 372e 302e 302e   / E.g. 127.0.0.
-00010260: 313a 3530 3030 0a20 2020 2022 2222 0a20  1:5000.    """. 
-00010270: 2020 2069 735f 7365 6c66 3a20 6275 696c     is_self: buil
-00010280: 7469 6e73 2e62 6f6f 6c0a 2020 2020 2222  tins.bool.    ""
-00010290: 222f 2049 6620 7472 7565 2c20 6974 206d  "/ If true, it m
-000102a0: 6561 6e73 2073 656c 662e 2222 220a 2020  eans self.""".  
-000102b0: 2020 7479 7065 3a20 676c 6f62 616c 5f5f    type: global__
-000102c0: 5f4d 656d 6265 722e 5479 7065 2e56 616c  _Member.Type.Val
-000102d0: 7565 5479 7065 0a20 2020 2022 2222 2f20  ueType.    """/ 
-000102e0: 496f 2c20 496e 6765 7374 2c20 5365 6172  Io, Ingest, Sear
-000102f0: 6368 2c20 5472 6169 6e2e 2222 220a 2020  ch, Train.""".  
-00010300: 2020 6475 6d6d 793a 2062 7569 6c74 696e    dummy: builtin
-00010310: 732e 626f 6f6c 0a20 2020 2022 2222 2f20  s.bool.    """/ 
-00010320: 4475 6d6d 7920 4d65 6d62 6572 2222 220a  Dummy Member""".
-00010330: 2020 2020 6c6f 6164 5f73 636f 7265 3a20      load_score: 
-00010340: 6275 696c 7469 6e73 2e66 6c6f 6174 0a20  builtins.float. 
-00010350: 2020 2022 2222 2f20 5468 6520 6c6f 6164     """/ The load
-00010360: 2073 636f 7265 206f 6620 7468 6520 6d65   score of the me
-00010370: 6d62 6572 2e22 2222 0a20 2020 2073 6861  mber.""".    sha
-00010380: 7264 5f63 6f75 6e74 3a20 6275 696c 7469  rd_count: builti
-00010390: 6e73 2e69 6e74 0a20 2020 2022 2222 2f20  ns.int.    """/ 
-000103a0: 5468 6520 6e75 6d62 6572 206f 6620 7368  The number of sh
-000103b0: 6172 6473 2069 6e20 7468 6520 6e6f 6465  ards in the node
-000103c0: 2e22 2222 0a20 2020 2070 7269 6d61 7279  .""".    primary
-000103d0: 5f69 643a 2062 7569 6c74 696e 732e 7374  _id: builtins.st
-000103e0: 720a 2020 2020 2222 222f 2054 6865 2069  r.    """/ The i
-000103f0: 6420 6f66 2074 6865 2070 7269 6d61 7279  d of the primary
-00010400: 206e 6f64 6520 2869 6620 6974 2069 7320   node (if it is 
-00010410: 6120 7365 636f 6e64 6172 7920 6e6f 6465  a secondary node
-00010420: 292e 2222 220a 2020 2020 6465 6620 5f5f  ).""".    def __
-00010430: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00010440: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00010450: 0a20 2020 2020 2020 2069 643a 2062 7569  .        id: bui
-00010460: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00010470: 0a20 2020 2020 2020 206c 6973 7465 6e5f  .        listen_
-00010480: 6164 6472 6573 733a 2062 7569 6c74 696e  address: builtin
-00010490: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-000104a0: 2020 2020 2069 735f 7365 6c66 3a20 6275       is_self: bu
-000104b0: 696c 7469 6e73 2e62 6f6f 6c20 3d20 2e2e  iltins.bool = ..
-000104c0: 2e2c 0a20 2020 2020 2020 2074 7970 653a  .,.        type:
-000104d0: 2067 6c6f 6261 6c5f 5f5f 4d65 6d62 6572   global___Member
-000104e0: 2e54 7970 652e 5661 6c75 6554 7970 6520  .Type.ValueType 
-000104f0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2064  = ...,.        d
-00010500: 756d 6d79 3a20 6275 696c 7469 6e73 2e62  ummy: builtins.b
-00010510: 6f6f 6c20 3d20 2e2e 2e2c 0a20 2020 2020  ool = ...,.     
-00010520: 2020 206c 6f61 645f 7363 6f72 653a 2062     load_score: b
-00010530: 7569 6c74 696e 732e 666c 6f61 7420 3d20  uiltins.float = 
-00010540: 2e2e 2e2c 0a20 2020 2020 2020 2073 6861  ...,.        sha
-00010550: 7264 5f63 6f75 6e74 3a20 6275 696c 7469  rd_count: builti
-00010560: 6e73 2e69 6e74 203d 202e 2e2e 2c0a 2020  ns.int = ...,.  
-00010570: 2020 2020 2020 7072 696d 6172 795f 6964        primary_id
-00010580: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00010590: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-000105a0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-000105b0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-000105c0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-000105d0: 7069 6e67 2e4c 6974 6572 616c 5b22 6475  ping.Literal["du
-000105e0: 6d6d 7922 2c20 6222 6475 6d6d 7922 2c20  mmy", b"dummy", 
-000105f0: 2269 6422 2c20 6222 6964 222c 2022 6973  "id", b"id", "is
-00010600: 5f73 656c 6622 2c20 6222 6973 5f73 656c  _self", b"is_sel
-00010610: 6622 2c20 226c 6973 7465 6e5f 6164 6472  f", "listen_addr
-00010620: 6573 7322 2c20 6222 6c69 7374 656e 5f61  ess", b"listen_a
-00010630: 6464 7265 7373 222c 2022 6c6f 6164 5f73  ddress", "load_s
-00010640: 636f 7265 222c 2062 226c 6f61 645f 7363  core", b"load_sc
-00010650: 6f72 6522 2c20 2270 7269 6d61 7279 5f69  ore", "primary_i
-00010660: 6422 2c20 6222 7072 696d 6172 795f 6964  d", b"primary_id
-00010670: 222c 2022 7368 6172 645f 636f 756e 7422  ", "shard_count"
-00010680: 2c20 6222 7368 6172 645f 636f 756e 7422  , b"shard_count"
-00010690: 2c20 2274 7970 6522 2c20 6222 7479 7065  , "type", b"type
-000106a0: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-000106b0: 0a0a 676c 6f62 616c 5f5f 5f4d 656d 6265  ..global___Membe
-000106c0: 7220 3d20 4d65 6d62 6572 0a0a 4074 7970  r = Member..@typ
-000106d0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000106e0: 4c69 7374 4d65 6d62 6572 7352 6571 7565  ListMembersReque
-000106f0: 7374 2867 6f6f 676c 652e 7072 6f74 6f62  st(google.protob
-00010700: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00010710: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00010720: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00010730: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-00010740: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-00010750: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00010760: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00010770: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00010780: 676c 6f62 616c 5f5f 5f4c 6973 744d 656d  global___ListMem
-00010790: 6265 7273 5265 7175 6573 7420 3d20 4c69  bersRequest = Li
-000107a0: 7374 4d65 6d62 6572 7352 6571 7565 7374  stMembersRequest
-000107b0: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-000107c0: 636c 6173 7320 4c69 7374 4d65 6d62 6572  class ListMember
-000107d0: 7352 6573 706f 6e73 6528 676f 6f67 6c65  sResponse(google
-000107e0: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-000107f0: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00010800: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00010810: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00010820: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00010830: 720a 0a20 2020 204d 454d 4245 5253 5f46  r..    MEMBERS_F
-00010840: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00010850: 6c74 696e 732e 696e 740a 2020 2020 4070  ltins.int.    @p
-00010860: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00010870: 6d65 6d62 6572 7328 7365 6c66 2920 2d3e  members(self) ->
-00010880: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00010890: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-000108a0: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
-000108b0: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
-000108c0: 696e 6572 5b67 6c6f 6261 6c5f 5f5f 4d65  iner[global___Me
-000108d0: 6d62 6572 5d3a 202e 2e2e 0a20 2020 2064  mber]: ....    d
-000108e0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000108f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00010900: 2020 202a 2c0a 2020 2020 2020 2020 6d65     *,.        me
-00010910: 6d62 6572 733a 2063 6f6c 6c65 6374 696f  mbers: collectio
-00010920: 6e73 2e61 6263 2e49 7465 7261 626c 655b  ns.abc.Iterable[
-00010930: 676c 6f62 616c 5f5f 5f4d 656d 6265 725d  global___Member]
-00010940: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00010950: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-00010960: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-00010970: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00010980: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00010990: 7465 7261 6c5b 226d 656d 6265 7273 222c  teral["members",
-000109a0: 2062 226d 656d 6265 7273 225d 2920 2d3e   b"members"]) ->
-000109b0: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-000109c0: 616c 5f5f 5f4c 6973 744d 656d 6265 7273  al___ListMembers
-000109d0: 5265 7370 6f6e 7365 203d 204c 6973 744d  Response = ListM
-000109e0: 656d 6265 7273 5265 7370 6f6e 7365 0a0a  embersResponse..
-000109f0: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
-00010a00: 6173 7320 5368 6172 6452 6570 6c69 6361  ass ShardReplica
-00010a10: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-00010a20: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-00010a30: 293a 0a20 2020 2044 4553 4352 4950 544f  ):.    DESCRIPTO
-00010a40: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-00010a50: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-00010a60: 7363 7269 7074 6f72 0a0a 2020 2020 5348  scriptor..    SH
-00010a70: 4152 445f 4649 454c 445f 4e55 4d42 4552  ARD_FIELD_NUMBER
-00010a80: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00010a90: 2020 204e 4f44 455f 4649 454c 445f 4e55     NODE_FIELD_NU
-00010aa0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00010ab0: 6e74 0a20 2020 206e 6f64 653a 2062 7569  nt.    node: bui
-00010ac0: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
-00010ad0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00010ae0: 7368 6172 6428 7365 6c66 2920 2d3e 206e  shard(self) -> n
-00010af0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6e  ucliadb_protos.n
-00010b00: 6f64 6572 6573 6f75 7263 6573 5f70 6232  oderesources_pb2
-00010b10: 2e53 6861 7264 4372 6561 7465 643a 202e  .ShardCreated: .
-00010b20: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00010b30: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00010b40: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-00010b50: 2020 2020 2020 7368 6172 643a 206e 7563        shard: nuc
-00010b60: 6c69 6164 625f 7072 6f74 6f73 2e6e 6f64  liadb_protos.nod
-00010b70: 6572 6573 6f75 7263 6573 5f70 6232 2e53  eresources_pb2.S
-00010b80: 6861 7264 4372 6561 7465 6420 7c20 4e6f  hardCreated | No
-00010b90: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00010ba0: 2020 6e6f 6465 3a20 6275 696c 7469 6e73    node: builtins
-00010bb0: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00010bc0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00010bd0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-00010be0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-00010bf0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-00010c00: 5b22 7368 6172 6422 2c20 6222 7368 6172  ["shard", b"shar
-00010c10: 6422 5d29 202d 3e20 6275 696c 7469 6e73  d"]) -> builtins
-00010c20: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2064  .bool: ....    d
-00010c30: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-00010c40: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-00010c50: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-00010c60: 6e6f 6465 222c 2062 226e 6f64 6522 2c20  node", b"node", 
-00010c70: 2273 6861 7264 222c 2062 2273 6861 7264  "shard", b"shard
-00010c80: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-00010c90: 0a0a 676c 6f62 616c 5f5f 5f53 6861 7264  ..global___Shard
-00010ca0: 5265 706c 6963 6120 3d20 5368 6172 6452  Replica = ShardR
-00010cb0: 6570 6c69 6361 0a0a 4074 7970 696e 672e  eplica..@typing.
-00010cc0: 6669 6e61 6c0a 636c 6173 7320 5368 6172  final.class Shar
-00010cd0: 644f 626a 6563 7428 676f 6f67 6c65 2e70  dObject(google.p
-00010ce0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00010cf0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00010d00: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00010d10: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00010d20: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00010d30: 0a20 2020 2053 4841 5244 5f46 4945 4c44  .    SHARD_FIELD
-00010d40: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00010d50: 732e 696e 740a 2020 2020 5245 504c 4943  s.int.    REPLIC
-00010d60: 4153 5f46 4945 4c44 5f4e 554d 4245 523a  AS_FIELD_NUMBER:
-00010d70: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00010d80: 2020 5449 4d45 5354 414d 505f 4649 454c    TIMESTAMP_FIEL
-00010d90: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00010da0: 6e73 2e69 6e74 0a20 2020 2052 4541 445f  ns.int.    READ_
-00010db0: 4f4e 4c59 5f46 4945 4c44 5f4e 554d 4245  ONLY_FIELD_NUMBE
-00010dc0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00010dd0: 2020 2020 7368 6172 643a 2062 7569 6c74      shard: built
-00010de0: 696e 732e 7374 720a 2020 2020 7265 6164  ins.str.    read
-00010df0: 5f6f 6e6c 793a 2062 7569 6c74 696e 732e  _only: builtins.
-00010e00: 626f 6f6c 0a20 2020 2040 7072 6f70 6572  bool.    @proper
-00010e10: 7479 0a20 2020 2064 6566 2072 6570 6c69  ty.    def repli
-00010e20: 6361 7328 7365 6c66 2920 2d3e 2067 6f6f  cas(self) -> goo
-00010e30: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-00010e40: 6572 6e61 6c2e 636f 6e74 6169 6e65 7273  ernal.containers
-00010e50: 2e52 6570 6561 7465 6443 6f6d 706f 7369  .RepeatedComposi
-00010e60: 7465 4669 656c 6443 6f6e 7461 696e 6572  teFieldContainer
-00010e70: 5b67 6c6f 6261 6c5f 5f5f 5368 6172 6452  [global___ShardR
-00010e80: 6570 6c69 6361 5d3a 202e 2e2e 0a20 2020  eplica]: ....   
-00010e90: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00010ea0: 6566 2074 696d 6573 7461 6d70 2873 656c  ef timestamp(sel
-00010eb0: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00010ec0: 746f 6275 662e 7469 6d65 7374 616d 705f  tobuf.timestamp_
-00010ed0: 7062 322e 5469 6d65 7374 616d 703a 202e  pb2.Timestamp: .
-00010ee0: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00010ef0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00010f00: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-00010f10: 2020 2020 2020 7368 6172 643a 2062 7569        shard: bui
-00010f20: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00010f30: 0a20 2020 2020 2020 2072 6570 6c69 6361  .        replica
-00010f40: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
-00010f50: 6263 2e49 7465 7261 626c 655b 676c 6f62  bc.Iterable[glob
-00010f60: 616c 5f5f 5f53 6861 7264 5265 706c 6963  al___ShardReplic
-00010f70: 615d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  a] | None = ...,
-00010f80: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-00010f90: 6d70 3a20 676f 6f67 6c65 2e70 726f 746f  mp: google.proto
-00010fa0: 6275 662e 7469 6d65 7374 616d 705f 7062  buf.timestamp_pb
-00010fb0: 322e 5469 6d65 7374 616d 7020 7c20 4e6f  2.Timestamp | No
-00010fc0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00010fd0: 2020 7265 6164 5f6f 6e6c 793a 2062 7569    read_only: bui
-00010fe0: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
-00010ff0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00011000: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-00011010: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-00011020: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-00011030: 6974 6572 616c 5b22 7469 6d65 7374 616d  iteral["timestam
-00011040: 7022 2c20 6222 7469 6d65 7374 616d 7022  p", b"timestamp"
-00011050: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
-00011060: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
-00011070: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-00011080: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00011090: 7069 6e67 2e4c 6974 6572 616c 5b22 7265  ping.Literal["re
-000110a0: 6164 5f6f 6e6c 7922 2c20 6222 7265 6164  ad_only", b"read
-000110b0: 5f6f 6e6c 7922 2c20 2272 6570 6c69 6361  _only", "replica
-000110c0: 7322 2c20 6222 7265 706c 6963 6173 222c  s", b"replicas",
-000110d0: 2022 7368 6172 6422 2c20 6222 7368 6172   "shard", b"shar
-000110e0: 6422 2c20 2274 696d 6573 7461 6d70 222c  d", "timestamp",
-000110f0: 2062 2274 696d 6573 7461 6d70 225d 2920   b"timestamp"]) 
-00011100: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-00011110: 6f62 616c 5f5f 5f53 6861 7264 4f62 6a65  obal___ShardObje
-00011120: 6374 203d 2053 6861 7264 4f62 6a65 6374  ct = ShardObject
-00011130: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-00011140: 636c 6173 7320 5368 6172 6473 2867 6f6f  class Shards(goo
-00011150: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-00011160: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-00011170: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00011180: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00011190: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-000111a0: 7074 6f72 0a0a 2020 2020 4074 7970 696e  ptor..    @typin
-000111b0: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
-000111c0: 7320 4578 7472 6145 6e74 7279 2867 6f6f  s ExtraEntry(goo
-000111d0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-000111e0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-000111f0: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
-00011200: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-00011210: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-00011220: 7363 7269 7074 6f72 0a0a 2020 2020 2020  scriptor..      
-00011230: 2020 4b45 595f 4649 454c 445f 4e55 4d42    KEY_FIELD_NUMB
-00011240: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00011250: 0a20 2020 2020 2020 2056 414c 5545 5f46  .        VALUE_F
-00011260: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00011270: 6c74 696e 732e 696e 740a 2020 2020 2020  ltins.int.      
-00011280: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
-00011290: 7374 720a 2020 2020 2020 2020 7661 6c75  str.        valu
-000112a0: 653a 2062 7569 6c74 696e 732e 7374 720a  e: builtins.str.
-000112b0: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
-000112c0: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
-000112d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000112e0: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
-000112f0: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
-00011300: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00011310: 2020 2020 2020 2020 7661 6c75 653a 2062          value: b
-00011320: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00011330: 2e2c 0a20 2020 2020 2020 2029 202d 3e20  .,.        ) -> 
-00011340: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 2020  None: ....      
-00011350: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-00011360: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-00011370: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-00011380: 6c5b 226b 6579 222c 2062 226b 6579 222c  l["key", b"key",
-00011390: 2022 7661 6c75 6522 2c20 6222 7661 6c75   "value", b"valu
-000113a0: 6522 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  e"]) -> None: ..
-000113b0: 2e0a 0a20 2020 2053 4841 5244 535f 4649  ...    SHARDS_FI
-000113c0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000113d0: 7469 6e73 2e69 6e74 0a20 2020 204b 4249  tins.int.    KBI
-000113e0: 445f 4649 454c 445f 4e55 4d42 4552 3a20  D_FIELD_NUMBER: 
-000113f0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00011400: 2041 4354 5541 4c5f 4649 454c 445f 4e55   ACTUAL_FIELD_NU
-00011410: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00011420: 6e74 0a20 2020 2053 494d 494c 4152 4954  nt.    SIMILARIT
-00011430: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
-00011440: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00011450: 204d 4f44 454c 5f46 4945 4c44 5f4e 554d   MODEL_FIELD_NUM
-00011460: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00011470: 740a 2020 2020 5245 4c45 4153 455f 4348  t.    RELEASE_CH
-00011480: 414e 4e45 4c5f 4649 454c 445f 4e55 4d42  ANNEL_FIELD_NUMB
-00011490: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-000114a0: 0a20 2020 2045 5854 5241 5f46 4945 4c44  .    EXTRA_FIELD
-000114b0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-000114c0: 732e 696e 740a 2020 2020 6b62 6964 3a20  s.int.    kbid: 
-000114d0: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
-000114e0: 2061 6374 7561 6c3a 2062 7569 6c74 696e   actual: builtin
-000114f0: 732e 696e 740a 2020 2020 2222 2244 4550  s.int.    """DEP
-00011500: 5245 4341 5445 4420 6120 4b42 206b 6e6f  RECATED a KB kno
-00011510: 7720 6361 6e20 6861 7665 206d 756c 7469  w can have multi
-00011520: 706c 6520 616c 6976 6520 7368 6172 6473  ple alive shards
-00011530: 2061 6e64 2069 7320 7472 6163 6b65 6420   and is tracked 
-00011540: 696e 0a20 2020 2065 6163 6820 5368 6172  in.    each Shar
-00011550: 644f 626a 6563 740a 2020 2020 2222 220a  dObject.    """.
-00011560: 2020 2020 7369 6d69 6c61 7269 7479 3a20      similarity: 
-00011570: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00011580: 7574 696c 735f 7062 322e 5665 6374 6f72  utils_pb2.Vector
-00011590: 5369 6d69 6c61 7269 7479 2e56 616c 7565  Similarity.Value
-000115a0: 5479 7065 0a20 2020 2022 2222 4445 5052  Type.    """DEPR
-000115b0: 4543 4154 4544 2069 6e20 6661 766f 7220  ECATED in favor 
-000115c0: 6f66 2060 6d6f 6465 6c60 2074 6f20 696e  of `model` to in
-000115d0: 636c 7564 6520 6d6f 7265 2064 6174 6122  clude more data"
-000115e0: 2222 0a20 2020 2072 656c 6561 7365 5f63  "".    release_c
-000115f0: 6861 6e6e 656c 3a20 6e75 636c 6961 6462  hannel: nucliadb
-00011600: 5f70 726f 746f 732e 7574 696c 735f 7062  _protos.utils_pb
-00011610: 322e 5265 6c65 6173 6543 6861 6e6e 656c  2.ReleaseChannel
-00011620: 2e56 616c 7565 5479 7065 0a20 2020 2040  .ValueType.    @
-00011630: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00011640: 2073 6861 7264 7328 7365 6c66 2920 2d3e   shards(self) ->
-00011650: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00011660: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-00011670: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
-00011680: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
-00011690: 696e 6572 5b67 6c6f 6261 6c5f 5f5f 5368  iner[global___Sh
-000116a0: 6172 644f 626a 6563 745d 3a20 2e2e 2e0a  ardObject]: ....
-000116b0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-000116c0: 2020 6465 6620 6d6f 6465 6c28 7365 6c66    def model(self
-000116d0: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-000116e0: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-000116f0: 785f 7062 322e 5365 6d61 6e74 6963 4d6f  x_pb2.SemanticMo
-00011700: 6465 6c4d 6574 6164 6174 613a 202e 2e2e  delMetadata: ...
-00011710: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00011720: 2020 2064 6566 2065 7874 7261 2873 656c     def extra(sel
-00011730: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00011740: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
-00011750: 6f6e 7461 696e 6572 732e 5363 616c 6172  ontainers.Scalar
-00011760: 4d61 705b 6275 696c 7469 6e73 2e73 7472  Map[builtins.str
-00011770: 2c20 6275 696c 7469 6e73 2e73 7472 5d3a  , builtins.str]:
-00011780: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
-00011790: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000117a0: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-000117b0: 2020 2020 2020 2020 7368 6172 6473 3a20          shards: 
-000117c0: 636f 6c6c 6563 7469 6f6e 732e 6162 632e  collections.abc.
-000117d0: 4974 6572 6162 6c65 5b67 6c6f 6261 6c5f  Iterable[global_
-000117e0: 5f5f 5368 6172 644f 626a 6563 745d 207c  __ShardObject] |
-000117f0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-00011800: 2020 2020 206b 6269 643a 2062 7569 6c74       kbid: built
-00011810: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-00011820: 2020 2020 2020 2061 6374 7561 6c3a 2062         actual: b
-00011830: 7569 6c74 696e 732e 696e 7420 3d20 2e2e  uiltins.int = ..
-00011840: 2e2c 0a20 2020 2020 2020 2073 696d 696c  .,.        simil
-00011850: 6172 6974 793a 206e 7563 6c69 6164 625f  arity: nucliadb_
-00011860: 7072 6f74 6f73 2e75 7469 6c73 5f70 6232  protos.utils_pb2
-00011870: 2e56 6563 746f 7253 696d 696c 6172 6974  .VectorSimilarit
-00011880: 792e 5661 6c75 6554 7970 6520 3d20 2e2e  y.ValueType = ..
-00011890: 2e2c 0a20 2020 2020 2020 206d 6f64 656c  .,.        model
-000118a0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-000118b0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-000118c0: 6232 2e53 656d 616e 7469 634d 6f64 656c  b2.SemanticModel
-000118d0: 4d65 7461 6461 7461 207c 204e 6f6e 6520  Metadata | None 
-000118e0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2072  = ...,.        r
-000118f0: 656c 6561 7365 5f63 6861 6e6e 656c 3a20  elease_channel: 
-00011900: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00011910: 7574 696c 735f 7062 322e 5265 6c65 6173  utils_pb2.Releas
-00011920: 6543 6861 6e6e 656c 2e56 616c 7565 5479  eChannel.ValueTy
-00011930: 7065 203d 202e 2e2e 2c0a 2020 2020 2020  pe = ...,.      
-00011940: 2020 6578 7472 613a 2063 6f6c 6c65 6374    extra: collect
-00011950: 696f 6e73 2e61 6263 2e4d 6170 7069 6e67  ions.abc.Mapping
-00011960: 5b62 7569 6c74 696e 732e 7374 722c 2062  [builtins.str, b
-00011970: 7569 6c74 696e 732e 7374 725d 207c 204e  uiltins.str] | N
-00011980: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2029  one = ...,.    )
-00011990: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-000119a0: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-000119b0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-000119c0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-000119d0: 226d 6f64 656c 222c 2062 226d 6f64 656c  "model", b"model
-000119e0: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
-000119f0: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 6465  bool: ....    de
-00011a00: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-00011a10: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00011a20: 7970 696e 672e 4c69 7465 7261 6c5b 2261  yping.Literal["a
-00011a30: 6374 7561 6c22 2c20 6222 6163 7475 616c  ctual", b"actual
-00011a40: 222c 2022 6578 7472 6122 2c20 6222 6578  ", "extra", b"ex
-00011a50: 7472 6122 2c20 226b 6269 6422 2c20 6222  tra", "kbid", b"
-00011a60: 6b62 6964 222c 2022 6d6f 6465 6c22 2c20  kbid", "model", 
-00011a70: 6222 6d6f 6465 6c22 2c20 2272 656c 6561  b"model", "relea
-00011a80: 7365 5f63 6861 6e6e 656c 222c 2062 2272  se_channel", b"r
-00011a90: 656c 6561 7365 5f63 6861 6e6e 656c 222c  elease_channel",
-00011aa0: 2022 7368 6172 6473 222c 2062 2273 6861   "shards", b"sha
-00011ab0: 7264 7322 2c20 2273 696d 696c 6172 6974  rds", "similarit
-00011ac0: 7922 2c20 6222 7369 6d69 6c61 7269 7479  y", b"similarity
-00011ad0: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-00011ae0: 0a0a 676c 6f62 616c 5f5f 5f53 6861 7264  ..global___Shard
-00011af0: 7320 3d20 5368 6172 6473 0a0a 4074 7970  s = Shards..@typ
-00011b00: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-00011b10: 496e 6465 7852 6573 6f75 7263 6528 676f  IndexResource(go
-00011b20: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00011b30: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-00011b40: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00011b50: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00011b60: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-00011b70: 6970 746f 720a 0a20 2020 204b 4249 445f  iptor..    KBID_
-00011b80: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00011b90: 696c 7469 6e73 2e69 6e74 0a20 2020 2052  iltins.int.    R
-00011ba0: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
-00011bb0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00011bc0: 2020 5245 494e 4445 585f 5645 4354 4f52    REINDEX_VECTOR
-00011bd0: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
-00011be0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00011bf0: 206b 6269 643a 2062 7569 6c74 696e 732e   kbid: builtins.
-00011c00: 7374 720a 2020 2020 7269 643a 2062 7569  str.    rid: bui
-00011c10: 6c74 696e 732e 7374 720a 2020 2020 7265  ltins.str.    re
-00011c20: 696e 6465 785f 7665 6374 6f72 733a 2062  index_vectors: b
-00011c30: 7569 6c74 696e 732e 626f 6f6c 0a20 2020  uiltins.bool.   
-00011c40: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00011c50: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00011c60: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00011c70: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
-00011c80: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
-00011c90: 2020 7269 643a 2062 7569 6c74 696e 732e    rid: builtins.
-00011ca0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-00011cb0: 2020 2072 6569 6e64 6578 5f76 6563 746f     reindex_vecto
-00011cc0: 7273 3a20 6275 696c 7469 6e73 2e62 6f6f  rs: builtins.boo
-00011cd0: 6c20 3d20 2e2e 2e2c 0a20 2020 2029 202d  l = ...,.    ) -
-00011ce0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00011cf0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-00011d00: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00011d10: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00011d20: 226b 6269 6422 2c20 6222 6b62 6964 222c  "kbid", b"kbid",
-00011d30: 2022 7265 696e 6465 785f 7665 6374 6f72   "reindex_vector
-00011d40: 7322 2c20 6222 7265 696e 6465 785f 7665  s", b"reindex_ve
-00011d50: 6374 6f72 7322 2c20 2272 6964 222c 2062  ctors", "rid", b
-00011d60: 2272 6964 225d 2920 2d3e 204e 6f6e 653a  "rid"]) -> None:
-00011d70: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f49   .....global___I
-00011d80: 6e64 6578 5265 736f 7572 6365 203d 2049  ndexResource = I
-00011d90: 6e64 6578 5265 736f 7572 6365 0a0a 4074  ndexResource..@t
-00011da0: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
-00011db0: 7320 496e 6465 7853 7461 7475 7328 676f  s IndexStatus(go
-00011dc0: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00011dd0: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-00011de0: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00011df0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00011e00: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-00011e10: 6970 746f 720a 0a20 2020 2064 6566 205f  iptor..    def _
-00011e20: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00011e30: 2073 656c 662c 0a20 2020 2029 202d 3e20   self,.    ) -> 
-00011e40: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-00011e50: 6c5f 5f5f 496e 6465 7853 7461 7475 7320  l___IndexStatus 
-00011e60: 3d20 496e 6465 7853 7461 7475 730a 0a40  = IndexStatus..@
-00011e70: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
-00011e80: 7373 2053 6574 5665 6374 6f72 7352 6571  ss SetVectorsReq
-00011e90: 7565 7374 2867 6f6f 676c 652e 7072 6f74  uest(google.prot
-00011ea0: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-00011eb0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-00011ec0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-00011ed0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00011ee0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00011ef0: 2020 5645 4354 4f52 535f 4649 454c 445f    VECTORS_FIELD_
-00011f00: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00011f10: 2e69 6e74 0a20 2020 204b 4249 445f 4649  .int.    KBID_FI
-00011f20: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00011f30: 7469 6e73 2e69 6e74 0a20 2020 2052 4944  tins.int.    RID
-00011f40: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00011f50: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00011f60: 4649 454c 445f 4649 454c 445f 4e55 4d42  FIELD_FIELD_NUMB
-00011f70: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00011f80: 0a20 2020 206b 6269 643a 2062 7569 6c74  .    kbid: built
-00011f90: 696e 732e 7374 720a 2020 2020 7269 643a  ins.str.    rid:
-00011fa0: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00011fb0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00011fc0: 6465 6620 7665 6374 6f72 7328 7365 6c66  def vectors(self
-00011fd0: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-00011fe0: 6f74 6f73 2e75 7469 6c73 5f70 6232 2e56  otos.utils_pb2.V
-00011ff0: 6563 746f 724f 626a 6563 743a 202e 2e2e  ectorObject: ...
-00012000: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00012010: 2020 2064 6566 2066 6965 6c64 2873 656c     def field(sel
-00012020: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-00012030: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
-00012040: 7062 322e 4669 656c 6449 443a 202e 2e2e  pb2.FieldID: ...
-00012050: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00012060: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00012070: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00012080: 2020 2020 7665 6374 6f72 733a 206e 7563      vectors: nuc
-00012090: 6c69 6164 625f 7072 6f74 6f73 2e75 7469  liadb_protos.uti
-000120a0: 6c73 5f70 6232 2e56 6563 746f 724f 626a  ls_pb2.VectorObj
-000120b0: 6563 7420 7c20 4e6f 6e65 203d 202e 2e2e  ect | None = ...
-000120c0: 2c0a 2020 2020 2020 2020 6b62 6964 3a20  ,.        kbid: 
-000120d0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-000120e0: 2e2e 2c0a 2020 2020 2020 2020 7269 643a  ..,.        rid:
-000120f0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-00012100: 2e2e 2e2c 0a20 2020 2020 2020 2066 6965  ...,.        fie
-00012110: 6c64 3a20 6e75 636c 6961 6462 5f70 726f  ld: nucliadb_pro
-00012120: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00012130: 322e 4669 656c 6449 4420 7c20 4e6f 6e65  2.FieldID | None
-00012140: 203d 202e 2e2e 2c0a 2020 2020 2920 2d3e   = ...,.    ) ->
-00012150: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
-00012160: 6566 2048 6173 4669 656c 6428 7365 6c66  ef HasField(self
-00012170: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00012180: 7069 6e67 2e4c 6974 6572 616c 5b22 6669  ping.Literal["fi
-00012190: 656c 6422 2c20 6222 6669 656c 6422 2c20  eld", b"field", 
-000121a0: 2276 6563 746f 7273 222c 2062 2276 6563  "vectors", b"vec
-000121b0: 746f 7273 225d 2920 2d3e 2062 7569 6c74  tors"]) -> built
-000121c0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-000121d0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-000121e0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-000121f0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-00012200: 6c5b 2266 6965 6c64 222c 2062 2266 6965  l["field", b"fie
-00012210: 6c64 222c 2022 6b62 6964 222c 2062 226b  ld", "kbid", b"k
-00012220: 6269 6422 2c20 2272 6964 222c 2062 2272  bid", "rid", b"r
-00012230: 6964 222c 2022 7665 6374 6f72 7322 2c20  id", "vectors", 
-00012240: 6222 7665 6374 6f72 7322 5d29 202d 3e20  b"vectors"]) -> 
-00012250: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-00012260: 6c5f 5f5f 5365 7456 6563 746f 7273 5265  l___SetVectorsRe
-00012270: 7175 6573 7420 3d20 5365 7456 6563 746f  quest = SetVecto
-00012280: 7273 5265 7175 6573 740a 0a40 7479 7069  rsRequest..@typi
-00012290: 6e67 2e66 696e 616c 0a63 6c61 7373 2053  ng.final.class S
-000122a0: 6574 5665 6374 6f72 7352 6573 706f 6e73  etVectorsRespons
-000122b0: 6528 676f 6f67 6c65 2e70 726f 746f 6275  e(google.protobu
-000122c0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-000122d0: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-000122e0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-000122f0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00012300: 6573 6372 6970 746f 720a 0a20 2020 2046  escriptor..    F
-00012310: 4f55 4e44 5f46 4945 4c44 5f4e 554d 4245  OUND_FIELD_NUMBE
-00012320: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00012330: 2020 2020 666f 756e 643a 2062 7569 6c74      found: built
-00012340: 696e 732e 626f 6f6c 0a20 2020 2064 6566  ins.bool.    def
-00012350: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00012360: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00012370: 202a 2c0a 2020 2020 2020 2020 666f 756e   *,.        foun
-00012380: 643a 2062 7569 6c74 696e 732e 626f 6f6c  d: builtins.bool
-00012390: 203d 202e 2e2e 2c0a 2020 2020 2920 2d3e   = ...,.    ) ->
-000123a0: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
-000123b0: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-000123c0: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-000123d0: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-000123e0: 666f 756e 6422 2c20 6222 666f 756e 6422  found", b"found"
-000123f0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-00012400: 0a67 6c6f 6261 6c5f 5f5f 5365 7456 6563  .global___SetVec
-00012410: 746f 7273 5265 7370 6f6e 7365 203d 2053  torsResponse = S
-00012420: 6574 5665 6374 6f72 7352 6573 706f 6e73  etVectorsRespons
-00012430: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
-00012440: 0a63 6c61 7373 2046 696c 6552 6571 7565  .class FileReque
-00012450: 7374 2867 6f6f 676c 652e 7072 6f74 6f62  st(google.protob
-00012460: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00012470: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00012480: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00012490: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-000124a0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-000124b0: 4255 434b 4554 5f46 4945 4c44 5f4e 554d  BUCKET_FIELD_NUM
-000124c0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-000124d0: 740a 2020 2020 4b45 595f 4649 454c 445f  t.    KEY_FIELD_
-000124e0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-000124f0: 2e69 6e74 0a20 2020 2062 7563 6b65 743a  .int.    bucket:
-00012500: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00012510: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
-00012520: 7374 720a 2020 2020 6465 6620 5f5f 696e  str.    def __in
-00012530: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00012540: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
-00012550: 2020 2020 2020 2062 7563 6b65 743a 2062         bucket: b
-00012560: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-00012570: 2e2c 0a20 2020 2020 2020 206b 6579 3a20  .,.        key: 
-00012580: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-00012590: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
-000125a0: 653a 202e 2e2e 0a20 2020 2064 6566 2043  e: ....    def C
-000125b0: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-000125c0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-000125d0: 6e67 2e4c 6974 6572 616c 5b22 6275 636b  ng.Literal["buck
-000125e0: 6574 222c 2062 2262 7563 6b65 7422 2c20  et", b"bucket", 
-000125f0: 226b 6579 222c 2062 226b 6579 225d 2920  "key", b"key"]) 
-00012600: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-00012610: 6f62 616c 5f5f 5f46 696c 6552 6571 7565  obal___FileReque
-00012620: 7374 203d 2046 696c 6552 6571 7565 7374  st = FileRequest
-00012630: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-00012640: 636c 6173 7320 4269 6e61 7279 4461 7461  class BinaryData
-00012650: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-00012660: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-00012670: 293a 0a20 2020 2044 4553 4352 4950 544f  ):.    DESCRIPTO
-00012680: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-00012690: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-000126a0: 7363 7269 7074 6f72 0a0a 2020 2020 4441  scriptor..    DA
-000126b0: 5441 5f46 4945 4c44 5f4e 554d 4245 523a  TA_FIELD_NUMBER:
-000126c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000126d0: 2020 6461 7461 3a20 6275 696c 7469 6e73    data: builtins
-000126e0: 2e62 7974 6573 0a20 2020 2064 6566 205f  .bytes.    def _
-000126f0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00012700: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00012710: 2c0a 2020 2020 2020 2020 6461 7461 3a20  ,.        data: 
-00012720: 6275 696c 7469 6e73 2e62 7974 6573 203d  builtins.bytes =
-00012730: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-00012740: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-00012750: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-00012760: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00012770: 7069 6e67 2e4c 6974 6572 616c 5b22 6461  ping.Literal["da
-00012780: 7461 222c 2062 2264 6174 6122 5d29 202d  ta", b"data"]) -
-00012790: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
-000127a0: 6261 6c5f 5f5f 4269 6e61 7279 4461 7461  bal___BinaryData
-000127b0: 203d 2042 696e 6172 7944 6174 610a 0a40   = BinaryData..@
-000127c0: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
-000127d0: 7373 2042 696e 6172 794d 6574 6164 6174  ss BinaryMetadat
-000127e0: 6128 676f 6f67 6c65 2e70 726f 746f 6275  a(google.protobu
-000127f0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-00012800: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-00012810: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00012820: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00012830: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-00012840: 4249 445f 4649 454c 445f 4e55 4d42 4552  BID_FIELD_NUMBER
-00012850: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00012860: 2020 204b 4559 5f46 4945 4c44 5f4e 554d     KEY_FIELD_NUM
-00012870: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00012880: 740a 2020 2020 5349 5a45 5f46 4945 4c44  t.    SIZE_FIELD
-00012890: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-000128a0: 732e 696e 740a 2020 2020 4649 4c45 4e41  s.int.    FILENA
-000128b0: 4d45 5f46 4945 4c44 5f4e 554d 4245 523a  ME_FIELD_NUMBER:
-000128c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000128d0: 2020 434f 4e54 454e 545f 5459 5045 5f46    CONTENT_TYPE_F
-000128e0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-000128f0: 6c74 696e 732e 696e 740a 2020 2020 6b62  ltins.int.    kb
-00012900: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
-00012910: 0a20 2020 206b 6579 3a20 6275 696c 7469  .    key: builti
-00012920: 6e73 2e73 7472 0a20 2020 2073 697a 653a  ns.str.    size:
-00012930: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00012940: 2020 6669 6c65 6e61 6d65 3a20 6275 696c    filename: buil
-00012950: 7469 6e73 2e73 7472 0a20 2020 2063 6f6e  tins.str.    con
-00012960: 7465 6e74 5f74 7970 653a 2062 7569 6c74  tent_type: built
-00012970: 696e 732e 7374 720a 2020 2020 6465 6620  ins.str.    def 
-00012980: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00012990: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000129a0: 2a2c 0a20 2020 2020 2020 206b 6269 643a  *,.        kbid:
-000129b0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-000129c0: 2e2e 2e2c 0a20 2020 2020 2020 206b 6579  ...,.        key
-000129d0: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-000129e0: 202e 2e2e 2c0a 2020 2020 2020 2020 7369   ...,.        si
-000129f0: 7a65 3a20 6275 696c 7469 6e73 2e69 6e74  ze: builtins.int
-00012a00: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00012a10: 6669 6c65 6e61 6d65 3a20 6275 696c 7469  filename: builti
-00012a20: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00012a30: 2020 2020 2020 636f 6e74 656e 745f 7479        content_ty
-00012a40: 7065 3a20 6275 696c 7469 6e73 2e73 7472  pe: builtins.str
-00012a50: 203d 202e 2e2e 2c0a 2020 2020 2920 2d3e   = ...,.    ) ->
-00012a60: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
-00012a70: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-00012a80: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-00012a90: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-00012aa0: 636f 6e74 656e 745f 7479 7065 222c 2062  content_type", b
-00012ab0: 2263 6f6e 7465 6e74 5f74 7970 6522 2c20  "content_type", 
-00012ac0: 2266 696c 656e 616d 6522 2c20 6222 6669  "filename", b"fi
-00012ad0: 6c65 6e61 6d65 222c 2022 6b62 6964 222c  lename", "kbid",
-00012ae0: 2062 226b 6269 6422 2c20 226b 6579 222c   b"kbid", "key",
-00012af0: 2062 226b 6579 222c 2022 7369 7a65 222c   b"key", "size",
-00012b00: 2062 2273 697a 6522 5d29 202d 3e20 4e6f   b"size"]) -> No
-00012b10: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
-00012b20: 5f5f 4269 6e61 7279 4d65 7461 6461 7461  __BinaryMetadata
-00012b30: 203d 2042 696e 6172 794d 6574 6164 6174   = BinaryMetadat
-00012b40: 610a 0a40 7479 7069 6e67 2e66 696e 616c  a..@typing.final
-00012b50: 0a63 6c61 7373 2055 706c 6f61 6442 696e  .class UploadBin
-00012b60: 6172 7944 6174 6128 676f 6f67 6c65 2e70  aryData(google.p
-00012b70: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00012b80: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00012b90: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00012ba0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00012bb0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00012bc0: 0a20 2020 2043 4f55 4e54 5f46 4945 4c44  .    COUNT_FIELD
-00012bd0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00012be0: 732e 696e 740a 2020 2020 4d45 5441 4441  s.int.    METADA
-00012bf0: 5441 5f46 4945 4c44 5f4e 554d 4245 523a  TA_FIELD_NUMBER:
-00012c00: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00012c10: 2020 5041 594c 4f41 445f 4649 454c 445f    PAYLOAD_FIELD_
-00012c20: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00012c30: 2e69 6e74 0a20 2020 2063 6f75 6e74 3a20  .int.    count: 
-00012c40: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00012c50: 2070 6179 6c6f 6164 3a20 6275 696c 7469   payload: builti
-00012c60: 6e73 2e62 7974 6573 0a20 2020 2040 7072  ns.bytes.    @pr
-00012c70: 6f70 6572 7479 0a20 2020 2064 6566 206d  operty.    def m
-00012c80: 6574 6164 6174 6128 7365 6c66 2920 2d3e  etadata(self) ->
-00012c90: 2067 6c6f 6261 6c5f 5f5f 4269 6e61 7279   global___Binary
-00012ca0: 4d65 7461 6461 7461 3a20 2e2e 2e0a 2020  Metadata: ....  
-00012cb0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00012cc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00012cd0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00012ce0: 2063 6f75 6e74 3a20 6275 696c 7469 6e73   count: builtins
-00012cf0: 2e69 6e74 203d 202e 2e2e 2c0a 2020 2020  .int = ...,.    
-00012d00: 2020 2020 6d65 7461 6461 7461 3a20 676c      metadata: gl
-00012d10: 6f62 616c 5f5f 5f42 696e 6172 794d 6574  obal___BinaryMet
-00012d20: 6164 6174 6120 7c20 4e6f 6e65 203d 202e  adata | None = .
-00012d30: 2e2e 2c0a 2020 2020 2020 2020 7061 796c  ..,.        payl
-00012d40: 6f61 643a 2062 7569 6c74 696e 732e 6279  oad: builtins.by
-00012d50: 7465 7320 3d20 2e2e 2e2c 0a20 2020 2029  tes = ...,.    )
-00012d60: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00012d70: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-00012d80: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00012d90: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00012da0: 2264 6174 6122 2c20 6222 6461 7461 222c  "data", b"data",
-00012db0: 2022 6d65 7461 6461 7461 222c 2062 226d   "metadata", b"m
-00012dc0: 6574 6164 6174 6122 2c20 2270 6179 6c6f  etadata", "paylo
-00012dd0: 6164 222c 2062 2270 6179 6c6f 6164 225d  ad", b"payload"]
-00012de0: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-00012df0: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
-00012e00: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-00012e10: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-00012e20: 696e 672e 4c69 7465 7261 6c5b 2263 6f75  ing.Literal["cou
-00012e30: 6e74 222c 2062 2263 6f75 6e74 222c 2022  nt", b"count", "
-00012e40: 6461 7461 222c 2062 2264 6174 6122 2c20  data", b"data", 
-00012e50: 226d 6574 6164 6174 6122 2c20 6222 6d65  "metadata", b"me
-00012e60: 7461 6461 7461 222c 2022 7061 796c 6f61  tadata", "payloa
-00012e70: 6422 2c20 6222 7061 796c 6f61 6422 5d29  d", b"payload"])
-00012e80: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00012e90: 2020 6465 6620 5768 6963 684f 6e65 6f66    def WhichOneof
-00012ea0: 2873 656c 662c 206f 6e65 6f66 5f67 726f  (self, oneof_gro
-00012eb0: 7570 3a20 7479 7069 6e67 2e4c 6974 6572  up: typing.Liter
-00012ec0: 616c 5b22 6461 7461 222c 2062 2264 6174  al["data", b"dat
-00012ed0: 6122 5d29 202d 3e20 7479 7069 6e67 2e4c  a"]) -> typing.L
-00012ee0: 6974 6572 616c 5b22 6d65 7461 6461 7461  iteral["metadata
-00012ef0: 222c 2022 7061 796c 6f61 6422 5d20 7c20  ", "payload"] | 
-00012f00: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-00012f10: 6c5f 5f5f 5570 6c6f 6164 4269 6e61 7279  l___UploadBinary
-00012f20: 4461 7461 203d 2055 706c 6f61 6442 696e  Data = UploadBin
-00012f30: 6172 7944 6174 610a 0a40 7479 7069 6e67  aryData..@typing
-00012f40: 2e66 696e 616c 0a63 6c61 7373 2046 696c  .final.class Fil
-00012f50: 6555 706c 6f61 6465 6428 676f 6f67 6c65  eUploaded(google
-00012f60: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-00012f70: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00012f80: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00012f90: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00012fa0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00012fb0: 720a 0a20 2020 2064 6566 205f 5f69 6e69  r..    def __ini
-00012fc0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00012fd0: 662c 0a20 2020 2029 202d 3e20 4e6f 6e65  f,.    ) -> None
-00012fe0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-00012ff0: 4669 6c65 5570 6c6f 6164 6564 203d 2046  FileUploaded = F
-00013000: 696c 6555 706c 6f61 6465 640a 0a40 7479  ileUploaded..@ty
-00013010: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00013020: 2053 796e 6f6e 796d 7352 6571 7565 7374   SynonymsRequest
-00013030: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-00013040: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
-00013050: 293a 0a20 2020 2044 4553 4352 4950 544f  ):.    DESCRIPTO
-00013060: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-00013070: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-00013080: 7363 7269 7074 6f72 0a0a 2020 2020 4b42  scriptor..    KB
-00013090: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
-000130a0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000130b0: 2020 6b62 6964 3a20 6275 696c 7469 6e73    kbid: builtins
-000130c0: 2e73 7472 0a20 2020 2064 6566 205f 5f69  .str.    def __i
-000130d0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000130e0: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-000130f0: 2020 2020 2020 2020 6b62 6964 3a20 6275          kbid: bu
-00013100: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
-00013110: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00013120: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-00013130: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-00013140: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00013150: 2e4c 6974 6572 616c 5b22 6b62 6964 222c  .Literal["kbid",
-00013160: 2062 226b 6269 6422 5d29 202d 3e20 4e6f   b"kbid"]) -> No
-00013170: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
-00013180: 5f5f 5379 6e6f 6e79 6d73 5265 7175 6573  __SynonymsReques
-00013190: 7420 3d20 5379 6e6f 6e79 6d73 5265 7175  t = SynonymsRequ
-000131a0: 6573 740a                                est.
+000006d0: 7465 2c0a 2020 2020 4b6e 6f77 6c65 6467  te,.    Knowledg
+000006e0: 6542 6f78 5665 6374 6f72 5365 7473 436f  eBoxVectorSetsCo
+000006f0: 6e66 6967 2061 7320 4b6e 6f77 6c65 6467  nfig as Knowledg
+00000700: 6542 6f78 5665 6374 6f72 5365 7473 436f  eBoxVectorSetsCo
+00000710: 6e66 6967 2c0a 2020 2020 4c61 6265 6c20  nfig,.    Label 
+00000720: 6173 204c 6162 656c 2c0a 2020 2020 4c61  as Label,.    La
+00000730: 6265 6c53 6574 2061 7320 4c61 6265 6c53  belSet as LabelS
+00000740: 6574 2c0a 2020 2020 4c61 6265 6c73 2061  et,.    Labels a
+00000750: 7320 4c61 6265 6c73 2c0a 2020 2020 4e4f  s Labels,.    NO
+00000760: 5446 4f55 4e44 2061 7320 4e4f 5446 4f55  TFOUND as NOTFOU
+00000770: 4e44 2c0a 2020 2020 4e65 774b 6e6f 776c  ND,.    NewKnowl
+00000780: 6564 6765 426f 7852 6573 706f 6e73 6520  edgeBoxResponse 
+00000790: 6173 204e 6577 4b6e 6f77 6c65 6467 6542  as NewKnowledgeB
+000007a0: 6f78 5265 7370 6f6e 7365 2c0a 2020 2020  oxResponse,.    
+000007b0: 4f4b 2061 7320 4f4b 2c0a 2020 2020 5365  OK as OK,.    Se
+000007c0: 6d61 6e74 6963 4d6f 6465 6c4d 6574 6164  manticModelMetad
+000007d0: 6174 6120 6173 2053 656d 616e 7469 634d  ata as SemanticM
+000007e0: 6f64 656c 4d65 7461 6461 7461 2c0a 2020  odelMetadata,.  
+000007f0: 2020 5379 6e6f 6e79 6d73 2061 7320 5379    Synonyms as Sy
+00000800: 6e6f 6e79 6d73 2c0a 2020 2020 5465 726d  nonyms,.    Term
+00000810: 5379 6e6f 6e79 6d73 2061 7320 5465 726d  Synonyms as Term
+00000820: 5379 6e6f 6e79 6d73 2c0a 2020 2020 5570  Synonyms,.    Up
+00000830: 6461 7465 4b6e 6f77 6c65 6467 6542 6f78  dateKnowledgeBox
+00000840: 5265 7370 6f6e 7365 2061 7320 5570 6461  Response as Upda
+00000850: 7465 4b6e 6f77 6c65 6467 6542 6f78 5265  teKnowledgeBoxRe
+00000860: 7370 6f6e 7365 2c0a 2020 2020 5665 6374  sponse,.    Vect
+00000870: 6f72 5365 7420 6173 2056 6563 746f 7253  orSet as VectorS
+00000880: 6574 2c0a 2020 2020 5665 6374 6f72 5365  et,.    VectorSe
+00000890: 7443 6f6e 6669 6720 6173 2056 6563 746f  tConfig as Vecto
+000008a0: 7253 6574 436f 6e66 6967 2c0a 2020 2020  rSetConfig,.    
+000008b0: 5665 6374 6f72 5365 7473 2061 7320 5665  VectorSets as Ve
+000008c0: 6374 6f72 5365 7473 2c0a 290a 6672 6f6d  ctorSets,.).from
+000008d0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+000008e0: 2e6e 6f64 6572 6573 6f75 7263 6573 5f70  .noderesources_p
+000008f0: 6232 2069 6d70 6f72 7420 280a 2020 2020  b2 import (.    
+00000900: 456d 7074 7951 7565 7279 2061 7320 456d  EmptyQuery as Em
+00000910: 7074 7951 7565 7279 2c0a 2020 2020 456d  ptyQuery,.    Em
+00000920: 7074 7952 6573 706f 6e73 6520 6173 2045  ptyResponse as E
+00000930: 6d70 7479 5265 7370 6f6e 7365 2c0a 2020  mptyResponse,.  
+00000940: 2020 496e 6465 784d 6574 6164 6174 6120    IndexMetadata 
+00000950: 6173 2049 6e64 6578 4d65 7461 6461 7461  as IndexMetadata
+00000960: 2c0a 2020 2020 496e 6465 7850 6172 6167  ,.    IndexParag
+00000970: 7261 7068 2061 7320 496e 6465 7850 6172  raph as IndexPar
+00000980: 6167 7261 7068 2c0a 2020 2020 496e 6465  agraph,.    Inde
+00000990: 7850 6172 6167 7261 7068 7320 6173 2049  xParagraphs as I
+000009a0: 6e64 6578 5061 7261 6772 6170 6873 2c0a  ndexParagraphs,.
+000009b0: 2020 2020 4e6f 6465 4d65 7461 6461 7461      NodeMetadata
+000009c0: 2061 7320 4e6f 6465 4d65 7461 6461 7461   as NodeMetadata
+000009d0: 2c0a 2020 2020 5061 7261 6772 6170 684d  ,.    ParagraphM
+000009e0: 6574 6164 6174 6120 6173 2050 6172 6167  etadata as Parag
+000009f0: 7261 7068 4d65 7461 6461 7461 2c0a 2020  raphMetadata,.  
+00000a00: 2020 506f 7369 7469 6f6e 2061 7320 506f    Position as Po
+00000a10: 7369 7469 6f6e 2c0a 2020 2020 5265 7072  sition,.    Repr
+00000a20: 6573 656e 7461 7469 6f6e 2061 7320 5265  esentation as Re
+00000a30: 7072 6573 656e 7461 7469 6f6e 2c0a 2020  presentation,.  
+00000a40: 2020 5265 736f 7572 6365 2061 7320 5265    Resource as Re
+00000a50: 736f 7572 6365 2c0a 2020 2020 5265 736f  source,.    Reso
+00000a60: 7572 6365 4944 2061 7320 5265 736f 7572  urceID as Resour
+00000a70: 6365 4944 2c0a 2020 2020 5365 6e74 656e  ceID,.    Senten
+00000a80: 6365 4d65 7461 6461 7461 2061 7320 5365  ceMetadata as Se
+00000a90: 6e74 656e 6365 4d65 7461 6461 7461 2c0a  ntenceMetadata,.
+00000aa0: 2020 2020 5368 6172 6420 6173 2053 6861      Shard as Sha
+00000ab0: 7264 2c0a 2020 2020 5368 6172 6443 7265  rd,.    ShardCre
+00000ac0: 6174 6564 2061 7320 5368 6172 6443 7265  ated as ShardCre
+00000ad0: 6174 6564 2c0a 2020 2020 5368 6172 6449  ated,.    ShardI
+00000ae0: 6420 6173 2053 6861 7264 4964 2c0a 2020  d as ShardId,.  
+00000af0: 2020 5368 6172 6449 6473 2061 7320 5368    ShardIds as Sh
+00000b00: 6172 6449 6473 2c0a 2020 2020 5368 6172  ardIds,.    Shar
+00000b10: 644d 6574 6164 6174 6120 6173 2053 6861  dMetadata as Sha
+00000b20: 7264 4d65 7461 6461 7461 2c0a 2020 2020  rdMetadata,.    
+00000b30: 5465 7874 496e 666f 726d 6174 696f 6e20  TextInformation 
+00000b40: 6173 2054 6578 7449 6e66 6f72 6d61 7469  as TextInformati
+00000b50: 6f6e 2c0a 2020 2020 5665 6374 6f72 5365  on,.    VectorSe
+00000b60: 6e74 656e 6365 2061 7320 5665 6374 6f72  ntence as Vector
+00000b70: 5365 6e74 656e 6365 2c0a 2020 2020 5665  Sentence,.    Ve
+00000b80: 6374 6f72 5365 7449 4420 6173 2056 6563  ctorSetID as Vec
+00000b90: 746f 7253 6574 4944 2c0a 2020 2020 5665  torSetID,.    Ve
+00000ba0: 6374 6f72 5365 744c 6973 7420 6173 2056  ctorSetList as V
+00000bb0: 6563 746f 7253 6574 4c69 7374 2c0a 2020  ectorSetList,.  
+00000bc0: 2020 5665 6374 6f72 7365 7453 656e 7465    VectorsetSente
+00000bd0: 6e63 6573 2061 7320 5665 6374 6f72 7365  nces as Vectorse
+00000be0: 7453 656e 7465 6e63 6573 2c0a 290a 6672  tSentences,.).fr
+00000bf0: 6f6d 206e 7563 6c69 6164 625f 7072 6f74  om nucliadb_prot
+00000c00: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
+00000c10: 2069 6d70 6f72 7420 280a 2020 2020 416c   import (.    Al
+00000c20: 6c46 6965 6c64 4944 7320 6173 2041 6c6c  lFieldIDs as All
+00000c30: 4669 656c 6449 4473 2c0a 2020 2020 416e  FieldIDs,.    An
+00000c40: 7377 6572 7320 6173 2041 6e73 7765 7273  swers as Answers
+00000c50: 2c0a 2020 2020 4261 7369 6320 6173 2042  ,.    Basic as B
+00000c60: 6173 6963 2c0a 2020 2020 426c 6f63 6b20  asic,.    Block 
+00000c70: 6173 2042 6c6f 636b 2c0a 2020 2020 434f  as Block,.    CO
+00000c80: 4e56 4552 5341 5449 4f4e 2061 7320 434f  NVERSATION as CO
+00000c90: 4e56 4552 5341 5449 4f4e 2c0a 2020 2020  NVERSATION,.    
+00000ca0: 436c 6173 7369 6669 6361 7469 6f6e 2061  Classification a
+00000cb0: 7320 436c 6173 7369 6669 6361 7469 6f6e  s Classification
+00000cc0: 2c0a 2020 2020 436c 6f75 6446 696c 6520  ,.    CloudFile 
+00000cd0: 6173 2043 6c6f 7564 4669 6c65 2c0a 2020  as CloudFile,.  
+00000ce0: 2020 436f 6d70 7574 6564 4d65 7461 6461    ComputedMetada
+00000cf0: 7461 2061 7320 436f 6d70 7574 6564 4d65  ta as ComputedMe
+00000d00: 7461 6461 7461 2c0a 2020 2020 436f 6e76  tadata,.    Conv
+00000d10: 6572 7361 7469 6f6e 2061 7320 436f 6e76  ersation as Conv
+00000d20: 6572 7361 7469 6f6e 2c0a 2020 2020 4441  ersation,.    DA
+00000d30: 5445 5449 4d45 2061 7320 4441 5445 5449  TETIME as DATETI
+00000d40: 4d45 2c0a 2020 2020 456e 7469 7479 2061  ME,.    Entity a
+00000d50: 7320 456e 7469 7479 2c0a 2020 2020 4578  s Entity,.    Ex
+00000d60: 7472 6120 6173 2045 7874 7261 2c0a 2020  tra as Extra,.  
+00000d70: 2020 4578 7472 6163 7465 6454 6578 7457    ExtractedTextW
+00000d80: 7261 7070 6572 2061 7320 4578 7472 6163  rapper as Extrac
+00000d90: 7465 6454 6578 7457 7261 7070 6572 2c0a  tedTextWrapper,.
+00000da0: 2020 2020 4578 7472 6163 7465 6456 6563      ExtractedVec
+00000db0: 746f 7273 5772 6170 7065 7220 6173 2045  torsWrapper as E
+00000dc0: 7874 7261 6374 6564 5665 6374 6f72 7357  xtractedVectorsW
+00000dd0: 7261 7070 6572 2c0a 2020 2020 4649 4c45  rapper,.    FILE
+00000de0: 2061 7320 4649 4c45 2c0a 2020 2020 4669   as FILE,.    Fi
+00000df0: 656c 6443 6c61 7373 6966 6963 6174 696f  eldClassificatio
+00000e00: 6e73 2061 7320 4669 656c 6443 6c61 7373  ns as FieldClass
+00000e10: 6966 6963 6174 696f 6e73 2c0a 2020 2020  ifications,.    
+00000e20: 4669 656c 6443 6f6d 7075 7465 644d 6574  FieldComputedMet
+00000e30: 6164 6174 6120 6173 2046 6965 6c64 436f  adata as FieldCo
+00000e40: 6d70 7574 6564 4d65 7461 6461 7461 2c0a  mputedMetadata,.
+00000e50: 2020 2020 4669 656c 6443 6f6d 7075 7465      FieldCompute
+00000e60: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
+00000e70: 2061 7320 4669 656c 6443 6f6d 7075 7465   as FieldCompute
+00000e80: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
+00000e90: 2c0a 2020 2020 4669 656c 6443 6f6e 7665  ,.    FieldConve
+00000ea0: 7273 6174 696f 6e20 6173 2046 6965 6c64  rsation as Field
+00000eb0: 436f 6e76 6572 7361 7469 6f6e 2c0a 2020  Conversation,.  
+00000ec0: 2020 4669 656c 6444 6174 6574 696d 6520    FieldDatetime 
+00000ed0: 6173 2046 6965 6c64 4461 7465 7469 6d65  as FieldDatetime
+00000ee0: 2c0a 2020 2020 4669 656c 6446 696c 6520  ,.    FieldFile 
+00000ef0: 6173 2046 6965 6c64 4669 6c65 2c0a 2020  as FieldFile,.  
+00000f00: 2020 4669 656c 6449 4420 6173 2046 6965    FieldID as Fie
+00000f10: 6c64 4944 2c0a 2020 2020 4669 656c 644b  ldID,.    FieldK
+00000f20: 6579 776f 7264 7365 7420 6173 2046 6965  eywordset as Fie
+00000f30: 6c64 4b65 7977 6f72 6473 6574 2c0a 2020  ldKeywordset,.  
+00000f40: 2020 4669 656c 644c 6172 6765 4d65 7461    FieldLargeMeta
+00000f50: 6461 7461 2061 7320 4669 656c 644c 6172  data as FieldLar
+00000f60: 6765 4d65 7461 6461 7461 2c0a 2020 2020  geMetadata,.    
+00000f70: 4669 656c 644c 6179 6f75 7420 6173 2046  FieldLayout as F
+00000f80: 6965 6c64 4c61 796f 7574 2c0a 2020 2020  ieldLayout,.    
+00000f90: 4669 656c 644c 696e 6b20 6173 2046 6965  FieldLink as Fie
+00000fa0: 6c64 4c69 6e6b 2c0a 2020 2020 4669 656c  ldLink,.    Fiel
+00000fb0: 644d 6574 6164 6174 6120 6173 2046 6965  dMetadata as Fie
+00000fc0: 6c64 4d65 7461 6461 7461 2c0a 2020 2020  ldMetadata,.    
+00000fd0: 4669 656c 6451 7565 7374 696f 6e41 6e73  FieldQuestionAns
+00000fe0: 7765 7257 7261 7070 6572 2061 7320 4669  werWrapper as Fi
+00000ff0: 656c 6451 7565 7374 696f 6e41 6e73 7765  eldQuestionAnswe
+00001000: 7257 7261 7070 6572 2c0a 2020 2020 4669  rWrapper,.    Fi
+00001010: 656c 6454 6578 7420 6173 2046 6965 6c64  eldText as Field
+00001020: 5465 7874 2c0a 2020 2020 4669 656c 6454  Text,.    FieldT
+00001030: 7970 6520 6173 2046 6965 6c64 5479 7065  ype as FieldType
+00001040: 2c0a 2020 2020 4669 6c65 4578 7472 6163  ,.    FileExtrac
+00001050: 7465 6444 6174 6120 6173 2046 696c 6545  tedData as FileE
+00001060: 7874 7261 6374 6564 4461 7461 2c0a 2020  xtractedData,.  
+00001070: 2020 4669 6c65 5061 6765 7320 6173 2046    FilePages as F
+00001080: 696c 6550 6167 6573 2c0a 2020 2020 4745  ilePages,.    GE
+00001090: 4e45 5249 4320 6173 2047 454e 4552 4943  NERIC as GENERIC
+000010a0: 2c0a 2020 2020 4b45 5957 4f52 4453 4554  ,.    KEYWORDSET
+000010b0: 2061 7320 4b45 5957 4f52 4453 4554 2c0a   as KEYWORDSET,.
+000010c0: 2020 2020 4b65 7977 6f72 6420 6173 204b      Keyword as K
+000010d0: 6579 776f 7264 2c0a 2020 2020 4c41 594f  eyword,.    LAYO
+000010e0: 5554 2061 7320 4c41 594f 5554 2c0a 2020  UT as LAYOUT,.  
+000010f0: 2020 4c49 4e4b 2061 7320 4c49 4e4b 2c0a    LINK as LINK,.
+00001100: 2020 2020 4c61 7267 6543 6f6d 7075 7465      LargeCompute
+00001110: 644d 6574 6164 6174 6120 6173 204c 6172  dMetadata as Lar
+00001120: 6765 436f 6d70 7574 6564 4d65 7461 6461  geComputedMetada
+00001130: 7461 2c0a 2020 2020 4c61 7267 6543 6f6d  ta,.    LargeCom
+00001140: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
+00001150: 7070 6572 2061 7320 4c61 7267 6543 6f6d  pper as LargeCom
+00001160: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
+00001170: 7070 6572 2c0a 2020 2020 4c61 796f 7574  pper,.    Layout
+00001180: 436f 6e74 656e 7420 6173 204c 6179 6f75  Content as Layou
+00001190: 7443 6f6e 7465 6e74 2c0a 2020 2020 4c69  tContent,.    Li
+000011a0: 6e6b 4578 7472 6163 7465 6444 6174 6120  nkExtractedData 
+000011b0: 6173 204c 696e 6b45 7874 7261 6374 6564  as LinkExtracted
+000011c0: 4461 7461 2c0a 2020 2020 4d65 7373 6167  Data,.    Messag
+000011d0: 6520 6173 204d 6573 7361 6765 2c0a 2020  e as Message,.  
+000011e0: 2020 4d65 7373 6167 6543 6f6e 7465 6e74    MessageContent
+000011f0: 2061 7320 4d65 7373 6167 6543 6f6e 7465   as MessageConte
+00001200: 6e74 2c0a 2020 2020 4d65 7461 6461 7461  nt,.    Metadata
+00001210: 2061 7320 4d65 7461 6461 7461 2c0a 2020   as Metadata,.  
+00001220: 2020 4e65 7374 6564 4c69 7374 506f 7369    NestedListPosi
+00001230: 7469 6f6e 2061 7320 4e65 7374 6564 4c69  tion as NestedLi
+00001240: 7374 506f 7369 7469 6f6e 2c0a 2020 2020  stPosition,.    
+00001250: 4e65 7374 6564 506f 7369 7469 6f6e 2061  NestedPosition a
+00001260: 7320 4e65 7374 6564 506f 7369 7469 6f6e  s NestedPosition
+00001270: 2c0a 2020 2020 4f72 6967 696e 2061 7320  ,.    Origin as 
+00001280: 4f72 6967 696e 2c0a 2020 2020 5061 6765  Origin,.    Page
+00001290: 496e 666f 726d 6174 696f 6e20 6173 2050  Information as P
+000012a0: 6167 6549 6e66 6f72 6d61 7469 6f6e 2c0a  ageInformation,.
+000012b0: 2020 2020 5061 6765 506f 7369 7469 6f6e      PagePosition
+000012c0: 7320 6173 2050 6167 6550 6f73 6974 696f  s as PagePositio
+000012d0: 6e73 2c0a 2020 2020 5061 6765 5365 6c65  ns,.    PageSele
+000012e0: 6374 696f 6e73 2061 7320 5061 6765 5365  ctions as PageSe
+000012f0: 6c65 6374 696f 6e73 2c0a 2020 2020 5061  lections,.    Pa
+00001300: 6765 5374 7275 6374 7572 6520 6173 2050  geStructure as P
+00001310: 6167 6553 7472 7563 7475 7265 2c0a 2020  ageStructure,.  
+00001320: 2020 5061 6765 5374 7275 6374 7572 6550    PageStructureP
+00001330: 6167 6520 6173 2050 6167 6553 7472 7563  age as PageStruc
+00001340: 7475 7265 5061 6765 2c0a 2020 2020 5061  turePage,.    Pa
+00001350: 6765 5374 7275 6374 7572 6554 6f6b 656e  geStructureToken
+00001360: 2061 7320 5061 6765 5374 7275 6374 7572   as PageStructur
+00001370: 6554 6f6b 656e 2c0a 2020 2020 5061 7261  eToken,.    Para
+00001380: 6772 6170 6820 6173 2050 6172 6167 7261  graph as Paragra
+00001390: 7068 2c0a 2020 2020 5061 7261 6772 6170  ph,.    Paragrap
+000013a0: 6841 6e6e 6f74 6174 696f 6e20 6173 2050  hAnnotation as P
+000013b0: 6172 6167 7261 7068 416e 6e6f 7461 7469  aragraphAnnotati
+000013c0: 6f6e 2c0a 2020 2020 5061 7261 6772 6170  on,.    Paragrap
+000013d0: 6852 656c 6174 696f 6e73 2061 7320 5061  hRelations as Pa
+000013e0: 7261 6772 6170 6852 656c 6174 696f 6e73  ragraphRelations
+000013f0: 2c0a 2020 2020 506f 7369 7469 6f6e 2061  ,.    Position a
+00001400: 7320 506f 7369 7469 6f6e 2c0a 2020 2020  s Position,.    
+00001410: 506f 7369 7469 6f6e 7320 6173 2050 6f73  Positions as Pos
+00001420: 6974 696f 6e73 2c0a 2020 2020 5175 6573  itions,.    Ques
+00001430: 7469 6f6e 2061 7320 5175 6573 7469 6f6e  tion as Question
+00001440: 2c0a 2020 2020 5175 6573 7469 6f6e 416e  ,.    QuestionAn
+00001450: 7377 6572 2061 7320 5175 6573 7469 6f6e  swer as Question
+00001460: 416e 7377 6572 2c0a 2020 2020 5175 6573  Answer,.    Ques
+00001470: 7469 6f6e 416e 7377 6572 416e 6e6f 7461  tionAnswerAnnota
+00001480: 7469 6f6e 2061 7320 5175 6573 7469 6f6e  tion as Question
+00001490: 416e 7377 6572 416e 6e6f 7461 7469 6f6e  AnswerAnnotation
+000014a0: 2c0a 2020 2020 5175 6573 7469 6f6e 416e  ,.    QuestionAn
+000014b0: 7377 6572 7320 6173 2051 7565 7374 696f  swers as Questio
+000014c0: 6e41 6e73 7765 7273 2c0a 2020 2020 5265  nAnswers,.    Re
+000014d0: 6c61 7469 6f6e 7320 6173 2052 656c 6174  lations as Relat
+000014e0: 696f 6e73 2c0a 2020 2020 5265 7072 6573  ions,.    Repres
+000014f0: 656e 7461 7469 6f6e 2061 7320 5265 7072  entation as Repr
+00001500: 6573 656e 7461 7469 6f6e 2c0a 2020 2020  esentation,.    
+00001510: 526f 7773 5072 6576 6965 7720 6173 2052  RowsPreview as R
+00001520: 6f77 7350 7265 7669 6577 2c0a 2020 2020  owsPreview,.    
+00001530: 5365 6e74 656e 6365 2061 7320 5365 6e74  Sentence as Sent
+00001540: 656e 6365 2c0a 2020 2020 5445 5854 2061  ence,.    TEXT a
+00001550: 7320 5445 5854 2c0a 2020 2020 546f 6b65  s TEXT,.    Toke
+00001560: 6e53 706c 6974 2061 7320 546f 6b65 6e53  nSplit as TokenS
+00001570: 706c 6974 2c0a 2020 2020 5573 6572 4669  plit,.    UserFi
+00001580: 656c 644d 6574 6164 6174 6120 6173 2055  eldMetadata as U
+00001590: 7365 7246 6965 6c64 4d65 7461 6461 7461  serFieldMetadata
+000015a0: 2c0a 2020 2020 5573 6572 4d65 7461 6461  ,.    UserMetada
+000015b0: 7461 2061 7320 5573 6572 4d65 7461 6461  ta as UserMetada
+000015c0: 7461 2c0a 2020 2020 5573 6572 5665 6374  ta,.    UserVect
+000015d0: 6f72 7357 7261 7070 6572 2061 7320 5573  orsWrapper as Us
+000015e0: 6572 5665 6374 6f72 7357 7261 7070 6572  erVectorsWrapper
+000015f0: 2c0a 2020 2020 5669 7375 616c 5365 6c65  ,.    VisualSele
+00001600: 6374 696f 6e20 6173 2056 6973 7561 6c53  ction as VisualS
+00001610: 656c 6563 7469 6f6e 2c0a 290a 0a44 4553  election,.)..DES
+00001620: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+00001630: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+00001640: 746f 722e 4669 6c65 4465 7363 7269 7074  tor.FileDescript
+00001650: 6f72 0a0a 636c 6173 7320 5f4e 6f74 6966  or..class _Notif
+00001660: 6963 6174 696f 6e53 6f75 7263 653a 0a20  icationSource:. 
+00001670: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
+00001680: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
+00001690: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
+000016a0: 696e 732e 696e 7429 0a20 2020 2056 3a20  ins.int).    V: 
+000016b0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
+000016c0: 732e 5479 7065 416c 6961 7320 3d20 5661  s.TypeAlias = Va
+000016d0: 6c75 6554 7970 650a 0a63 6c61 7373 205f  lueType..class _
+000016e0: 4e6f 7469 6669 6361 7469 6f6e 536f 7572  NotificationSour
+000016f0: 6365 456e 756d 5479 7065 5772 6170 7065  ceEnumTypeWrappe
+00001700: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
+00001710: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
+00001720: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
+00001730: 756d 5479 7065 5772 6170 7065 725b 5f4e  umTypeWrapper[_N
+00001740: 6f74 6966 6963 6174 696f 6e53 6f75 7263  otificationSourc
+00001750: 652e 5661 6c75 6554 7970 655d 2c20 6275  e.ValueType], bu
+00001760: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
+00001770: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00001780: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00001790: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
+000017a0: 6372 6970 746f 720a 2020 2020 554e 5345  criptor.    UNSE
+000017b0: 543a 205f 4e6f 7469 6669 6361 7469 6f6e  T: _Notification
+000017c0: 536f 7572 6365 2e56 616c 7565 5479 7065  Source.ValueType
+000017d0: 2020 2320 300a 2020 2020 5752 4954 4552    # 0.    WRITER
+000017e0: 3a20 5f4e 6f74 6966 6963 6174 696f 6e53  : _NotificationS
+000017f0: 6f75 7263 652e 5661 6c75 6554 7970 6520  ource.ValueType 
+00001800: 2023 2031 0a20 2020 2050 524f 4345 5353   # 1.    PROCESS
+00001810: 4f52 3a20 5f4e 6f74 6966 6963 6174 696f  OR: _Notificatio
+00001820: 6e53 6f75 7263 652e 5661 6c75 6554 7970  nSource.ValueTyp
+00001830: 6520 2023 2032 0a0a 636c 6173 7320 4e6f  e  # 2..class No
+00001840: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
+00001850: 285f 4e6f 7469 6669 6361 7469 6f6e 536f  (_NotificationSo
+00001860: 7572 6365 2c20 6d65 7461 636c 6173 733d  urce, metaclass=
+00001870: 5f4e 6f74 6966 6963 6174 696f 6e53 6f75  _NotificationSou
+00001880: 7263 6545 6e75 6d54 7970 6557 7261 7070  rceEnumTypeWrapp
+00001890: 6572 293a 202e 2e2e 0a0a 554e 5345 543a  er): .....UNSET:
+000018a0: 204e 6f74 6966 6963 6174 696f 6e53 6f75   NotificationSou
+000018b0: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
+000018c0: 2030 0a57 5249 5445 523a 204e 6f74 6966   0.WRITER: Notif
+000018d0: 6963 6174 696f 6e53 6f75 7263 652e 5661  icationSource.Va
+000018e0: 6c75 6554 7970 6520 2023 2031 0a50 524f  lueType  # 1.PRO
+000018f0: 4345 5353 4f52 3a20 4e6f 7469 6669 6361  CESSOR: Notifica
+00001900: 7469 6f6e 536f 7572 6365 2e56 616c 7565  tionSource.Value
+00001910: 5479 7065 2020 2320 320a 676c 6f62 616c  Type  # 2.global
+00001920: 5f5f 5f4e 6f74 6966 6963 6174 696f 6e53  ___NotificationS
+00001930: 6f75 7263 6520 3d20 4e6f 7469 6669 6361  ource = Notifica
+00001940: 7469 6f6e 536f 7572 6365 0a0a 4074 7970  tionSource..@typ
+00001950: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+00001960: 4175 6469 7428 676f 6f67 6c65 2e70 726f  Audit(google.pro
+00001970: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+00001980: 7373 6167 6529 3a0a 2020 2020 2222 2257  ssage):.    """W
+00001990: 6520 7265 6365 6976 6520 7468 6973 2069  e receive this i
+000019a0: 6e66 6f72 6d61 7469 6f6e 2074 6872 6f77  nformation throw
+000019b0: 2061 6e20 7374 7265 616d 2073 7973 7465   an stream syste
+000019c0: 6d22 2222 0a0a 2020 2020 4445 5343 5249  m"""..    DESCRI
+000019d0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+000019e0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+000019f0: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+00001a00: 2063 6c61 7373 205f 536f 7572 6365 3a0a   class _Source:.
+00001a10: 2020 2020 2020 2020 5661 6c75 6554 7970          ValueTyp
+00001a20: 6520 3d20 7479 7069 6e67 2e4e 6577 5479  e = typing.NewTy
+00001a30: 7065 2822 5661 6c75 6554 7970 6522 2c20  pe("ValueType", 
+00001a40: 6275 696c 7469 6e73 2e69 6e74 290a 2020  builtins.int).  
+00001a50: 2020 2020 2020 563a 2074 7970 696e 675f        V: typing_
+00001a60: 6578 7465 6e73 696f 6e73 2e54 7970 6541  extensions.TypeA
+00001a70: 6c69 6173 203d 2056 616c 7565 5479 7065  lias = ValueType
+00001a80: 0a0a 2020 2020 636c 6173 7320 5f53 6f75  ..    class _Sou
+00001a90: 7263 6545 6e75 6d54 7970 6557 7261 7070  rceEnumTypeWrapp
+00001aa0: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
+00001ab0: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
+00001ac0: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
+00001ad0: 6e75 6d54 7970 6557 7261 7070 6572 5b41  numTypeWrapper[A
+00001ae0: 7564 6974 2e5f 536f 7572 6365 2e56 616c  udit._Source.Val
+00001af0: 7565 5479 7065 5d2c 2062 7569 6c74 696e  ueType], builtin
+00001b00: 732e 7479 7065 293a 0a20 2020 2020 2020  s.type):.       
+00001b10: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+00001b20: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+00001b30: 6372 6970 746f 722e 456e 756d 4465 7363  criptor.EnumDesc
+00001b40: 7269 7074 6f72 0a20 2020 2020 2020 2048  riptor.        H
+00001b50: 5454 503a 2041 7564 6974 2e5f 536f 7572  TTP: Audit._Sour
+00001b60: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
+00001b70: 300a 2020 2020 2020 2020 4441 5348 424f  0.        DASHBO
+00001b80: 4152 443a 2041 7564 6974 2e5f 536f 7572  ARD: Audit._Sour
+00001b90: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
+00001ba0: 310a 2020 2020 2020 2020 4445 534b 544f  1.        DESKTO
+00001bb0: 503a 2041 7564 6974 2e5f 536f 7572 6365  P: Audit._Source
+00001bc0: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+00001bd0: 0a20 2020 2063 6c61 7373 2053 6f75 7263  .    class Sourc
+00001be0: 6528 5f53 6f75 7263 652c 206d 6574 6163  e(_Source, metac
+00001bf0: 6c61 7373 3d5f 536f 7572 6365 456e 756d  lass=_SourceEnum
+00001c00: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
+00001c10: 2e0a 2020 2020 4854 5450 3a20 4175 6469  ..    HTTP: Audi
+00001c20: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
+00001c30: 7065 2020 2320 300a 2020 2020 4441 5348  pe  # 0.    DASH
+00001c40: 424f 4152 443a 2041 7564 6974 2e53 6f75  BOARD: Audit.Sou
+00001c50: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
+00001c60: 2031 0a20 2020 2044 4553 4b54 4f50 3a20   1.    DESKTOP: 
+00001c70: 4175 6469 742e 536f 7572 6365 2e56 616c  Audit.Source.Val
+00001c80: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
+00001c90: 2055 5345 525f 4649 454c 445f 4e55 4d42   USER_FIELD_NUMB
+00001ca0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00001cb0: 0a20 2020 2057 4845 4e5f 4649 454c 445f  .    WHEN_FIELD_
+00001cc0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00001cd0: 2e69 6e74 0a20 2020 204f 5249 4749 4e5f  .int.    ORIGIN_
+00001ce0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00001cf0: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
+00001d00: 4f55 5243 455f 4649 454c 445f 4e55 4d42  OURCE_FIELD_NUMB
+00001d10: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00001d20: 0a20 2020 204b 4249 445f 4649 454c 445f  .    KBID_FIELD_
+00001d30: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00001d40: 2e69 6e74 0a20 2020 2055 5549 445f 4649  .int.    UUID_FI
+00001d50: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00001d60: 7469 6e73 2e69 6e74 0a20 2020 204d 4553  tins.int.    MES
+00001d70: 5341 4745 5f53 4f55 5243 455f 4649 454c  SAGE_SOURCE_FIEL
+00001d80: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00001d90: 6e73 2e69 6e74 0a20 2020 2046 4945 4c44  ns.int.    FIELD
+00001da0: 5f4d 4554 4144 4154 415f 4649 454c 445f  _METADATA_FIELD_
+00001db0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00001dc0: 2e69 6e74 0a20 2020 2041 5544 4954 5f46  .int.    AUDIT_F
+00001dd0: 4945 4c44 535f 4649 454c 445f 4e55 4d42  IELDS_FIELD_NUMB
+00001de0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00001df0: 0a20 2020 2075 7365 723a 2062 7569 6c74  .    user: built
+00001e00: 696e 732e 7374 720a 2020 2020 6f72 6967  ins.str.    orig
+00001e10: 696e 3a20 6275 696c 7469 6e73 2e73 7472  in: builtins.str
+00001e20: 0a20 2020 2073 6f75 7263 653a 2067 6c6f  .    source: glo
+00001e30: 6261 6c5f 5f5f 4175 6469 742e 536f 7572  bal___Audit.Sour
+00001e40: 6365 2e56 616c 7565 5479 7065 0a20 2020  ce.ValueType.   
+00001e50: 206b 6269 643a 2062 7569 6c74 696e 732e   kbid: builtins.
+00001e60: 7374 720a 2020 2020 7575 6964 3a20 6275  str.    uuid: bu
+00001e70: 696c 7469 6e73 2e73 7472 0a20 2020 206d  iltins.str.    m
+00001e80: 6573 7361 6765 5f73 6f75 7263 653a 2067  essage_source: g
+00001e90: 6c6f 6261 6c5f 5f5f 4272 6f6b 6572 4d65  lobal___BrokerMe
+00001ea0: 7373 6167 652e 4d65 7373 6167 6553 6f75  ssage.MessageSou
+00001eb0: 7263 652e 5661 6c75 6554 7970 650a 2020  rce.ValueType.  
+00001ec0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00001ed0: 6465 6620 7768 656e 2873 656c 6629 202d  def when(self) -
+00001ee0: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
+00001ef0: 662e 7469 6d65 7374 616d 705f 7062 322e  f.timestamp_pb2.
+00001f00: 5469 6d65 7374 616d 703a 202e 2e2e 0a20  Timestamp: .... 
+00001f10: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00001f20: 2064 6566 2066 6965 6c64 5f6d 6574 6164   def field_metad
+00001f30: 6174 6128 7365 6c66 2920 2d3e 2067 6f6f  ata(self) -> goo
+00001f40: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+00001f50: 6572 6e61 6c2e 636f 6e74 6169 6e65 7273  ernal.containers
+00001f60: 2e52 6570 6561 7465 6443 6f6d 706f 7369  .RepeatedComposi
+00001f70: 7465 4669 656c 6443 6f6e 7461 696e 6572  teFieldContainer
+00001f80: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
+00001f90: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00001fa0: 6965 6c64 4944 5d3a 202e 2e2e 0a20 2020  ieldID]: ....   
+00001fb0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00001fc0: 6566 2061 7564 6974 5f66 6965 6c64 7328  ef audit_fields(
+00001fd0: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
+00001fe0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
+00001ff0: 6c2e 636f 6e74 6169 6e65 7273 2e52 6570  l.containers.Rep
+00002000: 6561 7465 6443 6f6d 706f 7369 7465 4669  eatedCompositeFi
+00002010: 656c 6443 6f6e 7461 696e 6572 5b6e 7563  eldContainer[nuc
+00002020: 6c69 6164 625f 7072 6f74 6f73 2e61 7564  liadb_protos.aud
+00002030: 6974 5f70 6232 2e41 7564 6974 4669 656c  it_pb2.AuditFiel
+00002040: 645d 3a20 2e2e 2e0a 2020 2020 6465 6620  d]: ....    def 
+00002050: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00002060: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00002070: 2a2c 0a20 2020 2020 2020 2075 7365 723a  *,.        user:
+00002080: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+00002090: 2e2e 2e2c 0a20 2020 2020 2020 2077 6865  ...,.        whe
+000020a0: 6e3a 2067 6f6f 676c 652e 7072 6f74 6f62  n: google.protob
+000020b0: 7566 2e74 696d 6573 7461 6d70 5f70 6232  uf.timestamp_pb2
+000020c0: 2e54 696d 6573 7461 6d70 207c 204e 6f6e  .Timestamp | Non
+000020d0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+000020e0: 206f 7269 6769 6e3a 2062 7569 6c74 696e   origin: builtin
+000020f0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00002100: 2020 2020 2073 6f75 7263 653a 2067 6c6f       source: glo
+00002110: 6261 6c5f 5f5f 4175 6469 742e 536f 7572  bal___Audit.Sour
+00002120: 6365 2e56 616c 7565 5479 7065 203d 202e  ce.ValueType = .
+00002130: 2e2e 2c0a 2020 2020 2020 2020 6b62 6964  ..,.        kbid
+00002140: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00002150: 202e 2e2e 2c0a 2020 2020 2020 2020 7575   ...,.        uu
+00002160: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
+00002170: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00002180: 6d65 7373 6167 655f 736f 7572 6365 3a20  message_source: 
+00002190: 676c 6f62 616c 5f5f 5f42 726f 6b65 724d  global___BrokerM
+000021a0: 6573 7361 6765 2e4d 6573 7361 6765 536f  essage.MessageSo
+000021b0: 7572 6365 2e56 616c 7565 5479 7065 203d  urce.ValueType =
+000021c0: 202e 2e2e 2c0a 2020 2020 2020 2020 6669   ...,.        fi
+000021d0: 656c 645f 6d65 7461 6461 7461 3a20 636f  eld_metadata: co
+000021e0: 6c6c 6563 7469 6f6e 732e 6162 632e 4974  llections.abc.It
+000021f0: 6572 6162 6c65 5b6e 7563 6c69 6164 625f  erable[nucliadb_
+00002200: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+00002210: 5f70 6232 2e46 6965 6c64 4944 5d20 7c20  _pb2.FieldID] | 
+00002220: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00002230: 2020 2020 6175 6469 745f 6669 656c 6473      audit_fields
+00002240: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
+00002250: 632e 4974 6572 6162 6c65 5b6e 7563 6c69  c.Iterable[nucli
+00002260: 6164 625f 7072 6f74 6f73 2e61 7564 6974  adb_protos.audit
+00002270: 5f70 6232 2e41 7564 6974 4669 656c 645d  _pb2.AuditField]
+00002280: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00002290: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+000022a0: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
+000022b0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+000022c0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+000022d0: 7261 6c5b 2277 6865 6e22 2c20 6222 7768  ral["when", b"wh
+000022e0: 656e 225d 2920 2d3e 2062 7569 6c74 696e  en"]) -> builtin
+000022f0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+00002300: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+00002310: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00002320: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00002330: 2261 7564 6974 5f66 6965 6c64 7322 2c20  "audit_fields", 
+00002340: 6222 6175 6469 745f 6669 656c 6473 222c  b"audit_fields",
+00002350: 2022 6669 656c 645f 6d65 7461 6461 7461   "field_metadata
+00002360: 222c 2062 2266 6965 6c64 5f6d 6574 6164  ", b"field_metad
+00002370: 6174 6122 2c20 226b 6269 6422 2c20 6222  ata", "kbid", b"
+00002380: 6b62 6964 222c 2022 6d65 7373 6167 655f  kbid", "message_
+00002390: 736f 7572 6365 222c 2062 226d 6573 7361  source", b"messa
+000023a0: 6765 5f73 6f75 7263 6522 2c20 226f 7269  ge_source", "ori
+000023b0: 6769 6e22 2c20 6222 6f72 6967 696e 222c  gin", b"origin",
+000023c0: 2022 736f 7572 6365 222c 2062 2273 6f75   "source", b"sou
+000023d0: 7263 6522 2c20 2275 7365 7222 2c20 6222  rce", "user", b"
+000023e0: 7573 6572 222c 2022 7575 6964 222c 2062  user", "uuid", b
+000023f0: 2275 7569 6422 2c20 2277 6865 6e22 2c20  "uuid", "when", 
+00002400: 6222 7768 656e 225d 2920 2d3e 204e 6f6e  b"when"]) -> Non
+00002410: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+00002420: 5f41 7564 6974 203d 2041 7564 6974 0a0a  _Audit = Audit..
+00002430: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
+00002440: 6173 7320 4572 726f 7228 676f 6f67 6c65  ass Error(google
+00002450: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+00002460: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+00002470: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+00002480: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+00002490: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+000024a0: 720a 0a20 2020 2063 6c61 7373 205f 4572  r..    class _Er
+000024b0: 726f 7243 6f64 653a 0a20 2020 2020 2020  rorCode:.       
+000024c0: 2056 616c 7565 5479 7065 203d 2074 7970   ValueType = typ
+000024d0: 696e 672e 4e65 7754 7970 6528 2256 616c  ing.NewType("Val
+000024e0: 7565 5479 7065 222c 2062 7569 6c74 696e  ueType", builtin
+000024f0: 732e 696e 7429 0a20 2020 2020 2020 2056  s.int).        V
+00002500: 3a20 7479 7069 6e67 5f65 7874 656e 7369  : typing_extensi
+00002510: 6f6e 732e 5479 7065 416c 6961 7320 3d20  ons.TypeAlias = 
+00002520: 5661 6c75 6554 7970 650a 0a20 2020 2063  ValueType..    c
+00002530: 6c61 7373 205f 4572 726f 7243 6f64 6545  lass _ErrorCodeE
+00002540: 6e75 6d54 7970 6557 7261 7070 6572 2867  numTypeWrapper(g
+00002550: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+00002560: 6e74 6572 6e61 6c2e 656e 756d 5f74 7970  nternal.enum_typ
+00002570: 655f 7772 6170 7065 722e 5f45 6e75 6d54  e_wrapper._EnumT
+00002580: 7970 6557 7261 7070 6572 5b45 7272 6f72  ypeWrapper[Error
+00002590: 2e5f 4572 726f 7243 6f64 652e 5661 6c75  ._ErrorCode.Valu
+000025a0: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
+000025b0: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
+000025c0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+000025d0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+000025e0: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
+000025f0: 6970 746f 720a 2020 2020 2020 2020 4745  iptor.        GE
+00002600: 4e45 5249 433a 2045 7272 6f72 2e5f 4572  NERIC: Error._Er
+00002610: 726f 7243 6f64 652e 5661 6c75 6554 7970  rorCode.ValueTyp
+00002620: 6520 2023 2030 0a20 2020 2020 2020 2045  e  # 0.        E
+00002630: 5854 5241 4354 3a20 4572 726f 722e 5f45  XTRACT: Error._E
+00002640: 7272 6f72 436f 6465 2e56 616c 7565 5479  rrorCode.ValueTy
+00002650: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
+00002660: 5052 4f43 4553 533a 2045 7272 6f72 2e5f  PROCESS: Error._
+00002670: 4572 726f 7243 6f64 652e 5661 6c75 6554  ErrorCode.ValueT
+00002680: 7970 6520 2023 2032 0a0a 2020 2020 636c  ype  # 2..    cl
+00002690: 6173 7320 4572 726f 7243 6f64 6528 5f45  ass ErrorCode(_E
+000026a0: 7272 6f72 436f 6465 2c20 6d65 7461 636c  rrorCode, metacl
+000026b0: 6173 733d 5f45 7272 6f72 436f 6465 456e  ass=_ErrorCodeEn
+000026c0: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
+000026d0: 2e2e 2e0a 2020 2020 4745 4e45 5249 433a  ....    GENERIC:
+000026e0: 2045 7272 6f72 2e45 7272 6f72 436f 6465   Error.ErrorCode
+000026f0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
+00002700: 2020 2020 4558 5452 4143 543a 2045 7272      EXTRACT: Err
+00002710: 6f72 2e45 7272 6f72 436f 6465 2e56 616c  or.ErrorCode.Val
+00002720: 7565 5479 7065 2020 2320 310a 2020 2020  ueType  # 1.    
+00002730: 5052 4f43 4553 533a 2045 7272 6f72 2e45  PROCESS: Error.E
+00002740: 7272 6f72 436f 6465 2e56 616c 7565 5479  rrorCode.ValueTy
+00002750: 7065 2020 2320 320a 0a20 2020 2046 4945  pe  # 2..    FIE
+00002760: 4c44 5f46 4945 4c44 5f4e 554d 4245 523a  LD_FIELD_NUMBER:
+00002770: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00002780: 2020 4649 454c 445f 5459 5045 5f46 4945    FIELD_TYPE_FIE
+00002790: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000027a0: 696e 732e 696e 740a 2020 2020 4552 524f  ins.int.    ERRO
+000027b0: 525f 4649 454c 445f 4e55 4d42 4552 3a20  R_FIELD_NUMBER: 
+000027c0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000027d0: 2043 4f44 455f 4649 454c 445f 4e55 4d42   CODE_FIELD_NUMB
+000027e0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+000027f0: 0a20 2020 2066 6965 6c64 3a20 6275 696c  .    field: buil
+00002800: 7469 6e73 2e73 7472 0a20 2020 2066 6965  tins.str.    fie
+00002810: 6c64 5f74 7970 653a 206e 7563 6c69 6164  ld_type: nucliad
+00002820: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00002830: 6573 5f70 6232 2e46 6965 6c64 5479 7065  es_pb2.FieldType
+00002840: 2e56 616c 7565 5479 7065 0a20 2020 2065  .ValueType.    e
+00002850: 7272 6f72 3a20 6275 696c 7469 6e73 2e73  rror: builtins.s
+00002860: 7472 0a20 2020 2063 6f64 653a 2067 6c6f  tr.    code: glo
+00002870: 6261 6c5f 5f5f 4572 726f 722e 4572 726f  bal___Error.Erro
+00002880: 7243 6f64 652e 5661 6c75 6554 7970 650a  rCode.ValueType.
+00002890: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000028a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000028b0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000028c0: 2020 2066 6965 6c64 3a20 6275 696c 7469     field: builti
+000028d0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+000028e0: 2020 2020 2020 6669 656c 645f 7479 7065        field_type
+000028f0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00002900: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00002910: 4669 656c 6454 7970 652e 5661 6c75 6554  FieldType.ValueT
+00002920: 7970 6520 3d20 2e2e 2e2c 0a20 2020 2020  ype = ...,.     
+00002930: 2020 2065 7272 6f72 3a20 6275 696c 7469     error: builti
+00002940: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00002950: 2020 2020 2020 636f 6465 3a20 676c 6f62        code: glob
+00002960: 616c 5f5f 5f45 7272 6f72 2e45 7272 6f72  al___Error.Error
+00002970: 436f 6465 2e56 616c 7565 5479 7065 203d  Code.ValueType =
+00002980: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+00002990: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+000029a0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+000029b0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+000029c0: 7069 6e67 2e4c 6974 6572 616c 5b22 636f  ping.Literal["co
+000029d0: 6465 222c 2062 2263 6f64 6522 2c20 2265  de", b"code", "e
+000029e0: 7272 6f72 222c 2062 2265 7272 6f72 222c  rror", b"error",
+000029f0: 2022 6669 656c 6422 2c20 6222 6669 656c   "field", b"fiel
+00002a00: 6422 2c20 2266 6965 6c64 5f74 7970 6522  d", "field_type"
+00002a10: 2c20 6222 6669 656c 645f 7479 7065 225d  , b"field_type"]
+00002a20: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
+00002a30: 676c 6f62 616c 5f5f 5f45 7272 6f72 203d  global___Error =
+00002a40: 2045 7272 6f72 0a0a 4074 7970 696e 672e   Error..@typing.
+00002a50: 6669 6e61 6c0a 636c 6173 7320 4272 6f6b  final.class Brok
+00002a60: 6572 4d65 7373 6167 6528 676f 6f67 6c65  erMessage(google
+00002a70: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+00002a80: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+00002a90: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+00002aa0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+00002ab0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+00002ac0: 720a 0a20 2020 2063 6c61 7373 205f 4d65  r..    class _Me
+00002ad0: 7373 6167 6554 7970 653a 0a20 2020 2020  ssageType:.     
+00002ae0: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
+00002af0: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
+00002b00: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
+00002b10: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
+00002b20: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
+00002b30: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
+00002b40: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
+00002b50: 2063 6c61 7373 205f 4d65 7373 6167 6554   class _MessageT
+00002b60: 7970 6545 6e75 6d54 7970 6557 7261 7070  ypeEnumTypeWrapp
+00002b70: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
+00002b80: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
+00002b90: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
+00002ba0: 6e75 6d54 7970 6557 7261 7070 6572 5b42  numTypeWrapper[B
+00002bb0: 726f 6b65 724d 6573 7361 6765 2e5f 4d65  rokerMessage._Me
+00002bc0: 7373 6167 6554 7970 652e 5661 6c75 6554  ssageType.ValueT
+00002bd0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
+00002be0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
+00002bf0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00002c00: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00002c10: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
+00002c20: 746f 720a 2020 2020 2020 2020 4155 544f  tor.        AUTO
+00002c30: 434f 4d4d 4954 3a20 4272 6f6b 6572 4d65  COMMIT: BrokerMe
+00002c40: 7373 6167 652e 5f4d 6573 7361 6765 5479  ssage._MessageTy
+00002c50: 7065 2e56 616c 7565 5479 7065 2020 2320  pe.ValueType  # 
+00002c60: 300a 2020 2020 2020 2020 4d55 4c54 493a  0.        MULTI:
+00002c70: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
+00002c80: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
+00002c90: 6554 7970 6520 2023 2031 0a20 2020 2020  eType  # 1.     
+00002ca0: 2020 2043 4f4d 4d49 543a 2042 726f 6b65     COMMIT: Broke
+00002cb0: 724d 6573 7361 6765 2e5f 4d65 7373 6167  rMessage._Messag
+00002cc0: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
+00002cd0: 2023 2032 0a20 2020 2020 2020 2052 4f4c   # 2.        ROL
+00002ce0: 4c42 4143 4b3a 2042 726f 6b65 724d 6573  LBACK: BrokerMes
+00002cf0: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
+00002d00: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
+00002d10: 0a20 2020 2020 2020 2044 454c 4554 453a  .        DELETE:
+00002d20: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
+00002d30: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
+00002d40: 6554 7970 6520 2023 2034 0a0a 2020 2020  eType  # 4..    
+00002d50: 636c 6173 7320 4d65 7373 6167 6554 7970  class MessageTyp
+00002d60: 6528 5f4d 6573 7361 6765 5479 7065 2c20  e(_MessageType, 
+00002d70: 6d65 7461 636c 6173 733d 5f4d 6573 7361  metaclass=_Messa
+00002d80: 6765 5479 7065 456e 756d 5479 7065 5772  geTypeEnumTypeWr
+00002d90: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
+00002da0: 4155 544f 434f 4d4d 4954 3a20 4272 6f6b  AUTOCOMMIT: Brok
+00002db0: 6572 4d65 7373 6167 652e 4d65 7373 6167  erMessage.Messag
+00002dc0: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
+00002dd0: 2023 2030 0a20 2020 204d 554c 5449 3a20   # 0.    MULTI: 
+00002de0: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
+00002df0: 7373 6167 6554 7970 652e 5661 6c75 6554  ssageType.ValueT
+00002e00: 7970 6520 2023 2031 0a20 2020 2043 4f4d  ype  # 1.    COM
+00002e10: 4d49 543a 2042 726f 6b65 724d 6573 7361  MIT: BrokerMessa
+00002e20: 6765 2e4d 6573 7361 6765 5479 7065 2e56  ge.MessageType.V
+00002e30: 616c 7565 5479 7065 2020 2320 320a 2020  alueType  # 2.  
+00002e40: 2020 524f 4c4c 4241 434b 3a20 4272 6f6b    ROLLBACK: Brok
+00002e50: 6572 4d65 7373 6167 652e 4d65 7373 6167  erMessage.Messag
+00002e60: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
+00002e70: 2023 2033 0a20 2020 2044 454c 4554 453a   # 3.    DELETE:
+00002e80: 2042 726f 6b65 724d 6573 7361 6765 2e4d   BrokerMessage.M
+00002e90: 6573 7361 6765 5479 7065 2e56 616c 7565  essageType.Value
+00002ea0: 5479 7065 2020 2320 340a 0a20 2020 2063  Type  # 4..    c
+00002eb0: 6c61 7373 205f 4d65 7373 6167 6553 6f75  lass _MessageSou
+00002ec0: 7263 653a 0a20 2020 2020 2020 2056 616c  rce:.        Val
+00002ed0: 7565 5479 7065 203d 2074 7970 696e 672e  ueType = typing.
+00002ee0: 4e65 7754 7970 6528 2256 616c 7565 5479  NewType("ValueTy
+00002ef0: 7065 222c 2062 7569 6c74 696e 732e 696e  pe", builtins.in
+00002f00: 7429 0a20 2020 2020 2020 2056 3a20 7479  t).        V: ty
+00002f10: 7069 6e67 5f65 7874 656e 7369 6f6e 732e  ping_extensions.
+00002f20: 5479 7065 416c 6961 7320 3d20 5661 6c75  TypeAlias = Valu
+00002f30: 6554 7970 650a 0a20 2020 2063 6c61 7373  eType..    class
+00002f40: 205f 4d65 7373 6167 6553 6f75 7263 6545   _MessageSourceE
+00002f50: 6e75 6d54 7970 6557 7261 7070 6572 2867  numTypeWrapper(g
+00002f60: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+00002f70: 6e74 6572 6e61 6c2e 656e 756d 5f74 7970  nternal.enum_typ
+00002f80: 655f 7772 6170 7065 722e 5f45 6e75 6d54  e_wrapper._EnumT
+00002f90: 7970 6557 7261 7070 6572 5b42 726f 6b65  ypeWrapper[Broke
+00002fa0: 724d 6573 7361 6765 2e5f 4d65 7373 6167  rMessage._Messag
+00002fb0: 6553 6f75 7263 652e 5661 6c75 6554 7970  eSource.ValueTyp
+00002fc0: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
+00002fd0: 6529 3a0a 2020 2020 2020 2020 4445 5343  e):.        DESC
+00002fe0: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+00002ff0: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+00003000: 6f72 2e45 6e75 6d44 6573 6372 6970 746f  or.EnumDescripto
+00003010: 720a 2020 2020 2020 2020 5752 4954 4552  r.        WRITER
+00003020: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
+00003030: 5f4d 6573 7361 6765 536f 7572 6365 2e56  _MessageSource.V
+00003040: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
+00003050: 2020 2020 2020 5052 4f43 4553 534f 523a        PROCESSOR:
+00003060: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
+00003070: 4d65 7373 6167 6553 6f75 7263 652e 5661  MessageSource.Va
+00003080: 6c75 6554 7970 6520 2023 2031 0a0a 2020  lueType  # 1..  
+00003090: 2020 636c 6173 7320 4d65 7373 6167 6553    class MessageS
+000030a0: 6f75 7263 6528 5f4d 6573 7361 6765 536f  ource(_MessageSo
+000030b0: 7572 6365 2c20 6d65 7461 636c 6173 733d  urce, metaclass=
+000030c0: 5f4d 6573 7361 6765 536f 7572 6365 456e  _MessageSourceEn
+000030d0: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
+000030e0: 2e2e 2e0a 2020 2020 5752 4954 4552 3a20  ....    WRITER: 
+000030f0: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
+00003100: 7373 6167 6553 6f75 7263 652e 5661 6c75  ssageSource.Valu
+00003110: 6554 7970 6520 2023 2030 0a20 2020 2050  eType  # 0.    P
+00003120: 524f 4345 5353 4f52 3a20 4272 6f6b 6572  ROCESSOR: Broker
+00003130: 4d65 7373 6167 652e 4d65 7373 6167 6553  Message.MessageS
+00003140: 6f75 7263 652e 5661 6c75 6554 7970 6520  ource.ValueType 
+00003150: 2023 2031 0a0a 2020 2020 4074 7970 696e   # 1..    @typin
+00003160: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
+00003170: 7320 436f 6e76 6572 7361 7469 6f6e 7345  s ConversationsE
+00003180: 6e74 7279 2867 6f6f 676c 652e 7072 6f74  ntry(google.prot
+00003190: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+000031a0: 7361 6765 293a 0a20 2020 2020 2020 2044  sage):.        D
+000031b0: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+000031c0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+000031d0: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+000031e0: 0a0a 2020 2020 2020 2020 4b45 595f 4649  ..        KEY_FI
+000031f0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00003200: 7469 6e73 2e69 6e74 0a20 2020 2020 2020  tins.int.       
+00003210: 2056 414c 5545 5f46 4945 4c44 5f4e 554d   VALUE_FIELD_NUM
+00003220: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00003230: 740a 2020 2020 2020 2020 6b65 793a 2062  t.        key: b
+00003240: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+00003250: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00003260: 2020 2020 2020 6465 6620 7661 6c75 6528        def value(
+00003270: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+00003280: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00003290: 6573 5f70 6232 2e43 6f6e 7665 7273 6174  es_pb2.Conversat
+000032a0: 696f 6e3a 202e 2e2e 0a20 2020 2020 2020  ion: ....       
+000032b0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000032c0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+000032d0: 0a20 2020 2020 2020 2020 2020 202a 2c0a  .            *,.
+000032e0: 2020 2020 2020 2020 2020 2020 6b65 793a              key:
+000032f0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+00003300: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+00003310: 2076 616c 7565 3a20 6e75 636c 6961 6462   value: nucliadb
+00003320: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00003330: 735f 7062 322e 436f 6e76 6572 7361 7469  s_pb2.Conversati
+00003340: 6f6e 207c 204e 6f6e 6520 3d20 2e2e 2e2c  on | None = ...,
+00003350: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
+00003360: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
+00003370: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+00003380: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00003390: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
+000033a0: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
+000033b0: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+000033c0: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
+000033d0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+000033e0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+000033f0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00003400: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
+00003410: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
+00003420: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00003430: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+00003440: 616c 0a20 2020 2063 6c61 7373 204c 6179  al.    class Lay
+00003450: 6f75 7473 456e 7472 7928 676f 6f67 6c65  outsEntry(google
+00003460: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+00003470: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+00003480: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+00003490: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+000034a0: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+000034b0: 6970 746f 720a 0a20 2020 2020 2020 204b  iptor..        K
+000034c0: 4559 5f46 4945 4c44 5f4e 554d 4245 523a  EY_FIELD_NUMBER:
+000034d0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+000034e0: 2020 2020 2020 5641 4c55 455f 4649 454c        VALUE_FIEL
+000034f0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00003500: 6e73 2e69 6e74 0a20 2020 2020 2020 206b  ns.int.        k
+00003510: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
+00003520: 0a20 2020 2020 2020 2040 7072 6f70 6572  .        @proper
+00003530: 7479 0a20 2020 2020 2020 2064 6566 2076  ty.        def v
+00003540: 616c 7565 2873 656c 6629 202d 3e20 6e75  alue(self) -> nu
+00003550: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00003560: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+00003570: 644c 6179 6f75 743a 202e 2e2e 0a20 2020  dLayout: ....   
+00003580: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
+00003590: 5f28 0a20 2020 2020 2020 2020 2020 2073  _(.            s
+000035a0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000035b0: 202a 2c0a 2020 2020 2020 2020 2020 2020   *,.            
+000035c0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+000035d0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+000035e0: 2020 2020 2076 616c 7565 3a20 6e75 636c       value: nucl
+000035f0: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
+00003600: 7572 6365 735f 7062 322e 4669 656c 644c  urces_pb2.FieldL
+00003610: 6179 6f75 7420 7c20 4e6f 6e65 203d 202e  ayout | None = .
+00003620: 2e2e 2c0a 2020 2020 2020 2020 2920 2d3e  ..,.        ) ->
+00003630: 204e 6f6e 653a 202e 2e2e 0a20 2020 2020   None: ....     
+00003640: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
+00003650: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+00003660: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+00003670: 5b22 7661 6c75 6522 2c20 6222 7661 6c75  ["value", b"valu
+00003680: 6522 5d29 202d 3e20 6275 696c 7469 6e73  e"]) -> builtins
+00003690: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2020  .bool: ....     
+000036a0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+000036b0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+000036c0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+000036d0: 616c 5b22 6b65 7922 2c20 6222 6b65 7922  al["key", b"key"
+000036e0: 2c20 2276 616c 7565 222c 2062 2276 616c  , "value", b"val
+000036f0: 7565 225d 2920 2d3e 204e 6f6e 653a 202e  ue"]) -> None: .
+00003700: 2e2e 0a0a 2020 2020 4074 7970 696e 672e  ....    @typing.
+00003710: 6669 6e61 6c0a 2020 2020 636c 6173 7320  final.    class 
+00003720: 5465 7874 7345 6e74 7279 2867 6f6f 676c  TextsEntry(googl
+00003730: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00003740: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00003750: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
+00003760: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00003770: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+00003780: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
+00003790: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+000037a0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+000037b0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
+000037c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000037d0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+000037e0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+000037f0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
+00003800: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
+00003810: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
+00003820: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00003830: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00003840: 6c64 5465 7874 3a20 2e2e 2e0a 2020 2020  ldText: ....    
+00003850: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00003860: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00003870: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00003880: 2a2c 0a20 2020 2020 2020 2020 2020 206b  *,.            k
+00003890: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
+000038a0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+000038b0: 2020 2020 7661 6c75 653a 206e 7563 6c69      value: nucli
+000038c0: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
+000038d0: 7263 6573 5f70 6232 2e46 6965 6c64 5465  rces_pb2.FieldTe
+000038e0: 7874 207c 204e 6f6e 6520 3d20 2e2e 2e2c  xt | None = ...,
+000038f0: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
+00003900: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
+00003910: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+00003920: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00003930: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
+00003940: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
+00003950: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+00003960: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
+00003970: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+00003980: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00003990: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+000039a0: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
+000039b0: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
+000039c0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+000039d0: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+000039e0: 616c 0a20 2020 2063 6c61 7373 204b 6579  al.    class Key
+000039f0: 776f 7264 7365 7473 456e 7472 7928 676f  wordsetsEntry(go
+00003a00: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+00003a10: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+00003a20: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+00003a30: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+00003a40: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+00003a50: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
+00003a60: 2020 204b 4559 5f46 4945 4c44 5f4e 554d     KEY_FIELD_NUM
+00003a70: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00003a80: 740a 2020 2020 2020 2020 5641 4c55 455f  t.        VALUE_
+00003a90: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00003aa0: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
+00003ab0: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
+00003ac0: 2e73 7472 0a20 2020 2020 2020 2040 7072  .str.        @pr
+00003ad0: 6f70 6572 7479 0a20 2020 2020 2020 2064  operty.        d
+00003ae0: 6566 2076 616c 7565 2873 656c 6629 202d  ef value(self) -
+00003af0: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
+00003b00: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00003b10: 4669 656c 644b 6579 776f 7264 7365 743a  FieldKeywordset:
+00003b20: 202e 2e2e 0a20 2020 2020 2020 2064 6566   ....        def
+00003b30: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00003b40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00003b50: 2020 2020 2020 2020 202a 2c0a 2020 2020           *,.    
+00003b60: 2020 2020 2020 2020 6b65 793a 2062 7569          key: bui
+00003b70: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+00003b80: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00003b90: 7565 3a20 6e75 636c 6961 6462 5f70 726f  ue: nucliadb_pro
+00003ba0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+00003bb0: 322e 4669 656c 644b 6579 776f 7264 7365  2.FieldKeywordse
+00003bc0: 7420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  t | None = ...,.
+00003bd0: 2020 2020 2020 2020 2920 2d3e 204e 6f6e          ) -> Non
+00003be0: 653a 202e 2e2e 0a20 2020 2020 2020 2064  e: ....        d
+00003bf0: 6566 2048 6173 4669 656c 6428 7365 6c66  ef HasField(self
+00003c00: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00003c10: 7069 6e67 2e4c 6974 6572 616c 5b22 7661  ping.Literal["va
+00003c20: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
+00003c30: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
+00003c40: 6c3a 202e 2e2e 0a20 2020 2020 2020 2064  l: ....        d
+00003c50: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
+00003c60: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
+00003c70: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
+00003c80: 6b65 7922 2c20 6222 6b65 7922 2c20 2276  key", b"key", "v
+00003c90: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
+00003ca0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
+00003cb0: 2020 2020 4074 7970 696e 672e 6669 6e61      @typing.fina
+00003cc0: 6c0a 2020 2020 636c 6173 7320 4461 7465  l.    class Date
+00003cd0: 7469 6d65 7345 6e74 7279 2867 6f6f 676c  timesEntry(googl
+00003ce0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00003cf0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00003d00: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
+00003d10: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00003d20: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+00003d30: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
+00003d40: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+00003d50: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00003d60: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
+00003d70: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00003d80: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+00003d90: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+00003da0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
+00003db0: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
+00003dc0: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
+00003dd0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00003de0: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00003df0: 6c64 4461 7465 7469 6d65 3a20 2e2e 2e0a  ldDatetime: ....
+00003e00: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+00003e10: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
+00003e20: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00003e30: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
+00003e40: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
+00003e50: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00003e60: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
+00003e70: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00003e80: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00003e90: 6c64 4461 7465 7469 6d65 207c 204e 6f6e  ldDatetime | Non
+00003ea0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+00003eb0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00003ec0: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
+00003ed0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00003ee0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00003ef0: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
+00003f00: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
+00003f10: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
+00003f20: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
+00003f30: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00003f40: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00003f50: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
+00003f60: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
+00003f70: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
+00003f80: 6e65 3a20 2e2e 2e0a 0a20 2020 2040 7479  ne: .....    @ty
+00003f90: 7069 6e67 2e66 696e 616c 0a20 2020 2063  ping.final.    c
+00003fa0: 6c61 7373 204c 696e 6b73 456e 7472 7928  lass LinksEntry(
+00003fb0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00003fc0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+00003fd0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
+00003fe0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+00003ff0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+00004000: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+00004010: 2020 2020 204b 4559 5f46 4945 4c44 5f4e       KEY_FIELD_N
+00004020: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004030: 696e 740a 2020 2020 2020 2020 5641 4c55  int.        VALU
+00004040: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
+00004050: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004060: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
+00004070: 6e73 2e73 7472 0a20 2020 2020 2020 2040  ns.str.        @
+00004080: 7072 6f70 6572 7479 0a20 2020 2020 2020  property.       
+00004090: 2064 6566 2076 616c 7565 2873 656c 6629   def value(self)
+000040a0: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+000040b0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+000040c0: 322e 4669 656c 644c 696e 6b3a 202e 2e2e  2.FieldLink: ...
+000040d0: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
+000040e0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
+000040f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00004100: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00004110: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
+00004120: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00004130: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
+00004140: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00004150: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
+00004160: 656c 644c 696e 6b20 7c20 4e6f 6e65 203d  eldLink | None =
+00004170: 202e 2e2e 2c0a 2020 2020 2020 2020 2920   ...,.        ) 
+00004180: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+00004190: 2020 2020 2064 6566 2048 6173 4669 656c       def HasFiel
+000041a0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+000041b0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+000041c0: 616c 5b22 7661 6c75 6522 2c20 6222 7661  al["value", b"va
+000041d0: 6c75 6522 5d29 202d 3e20 6275 696c 7469  lue"]) -> builti
+000041e0: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+000041f0: 2020 2020 2064 6566 2043 6c65 6172 4669       def ClearFi
+00004200: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
+00004210: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
+00004220: 6572 616c 5b22 6b65 7922 2c20 6222 6b65  eral["key", b"ke
+00004230: 7922 2c20 2276 616c 7565 222c 2062 2276  y", "value", b"v
+00004240: 616c 7565 225d 2920 2d3e 204e 6f6e 653a  alue"]) -> None:
+00004250: 202e 2e2e 0a0a 2020 2020 4074 7970 696e   .....    @typin
+00004260: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
+00004270: 7320 4669 6c65 7345 6e74 7279 2867 6f6f  s FilesEntry(goo
+00004280: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+00004290: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+000042a0: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
+000042b0: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
+000042c0: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
+000042d0: 7363 7269 7074 6f72 0a0a 2020 2020 2020  scriptor..      
+000042e0: 2020 4b45 595f 4649 454c 445f 4e55 4d42    KEY_FIELD_NUMB
+000042f0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00004300: 0a20 2020 2020 2020 2056 414c 5545 5f46  .        VALUE_F
+00004310: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004320: 6c74 696e 732e 696e 740a 2020 2020 2020  ltins.int.      
+00004330: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
+00004340: 7374 720a 2020 2020 2020 2020 4070 726f  str.        @pro
+00004350: 7065 7274 790a 2020 2020 2020 2020 6465  perty.        de
+00004360: 6620 7661 6c75 6528 7365 6c66 2920 2d3e  f value(self) ->
+00004370: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00004380: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00004390: 6965 6c64 4669 6c65 3a20 2e2e 2e0a 2020  ieldFile: ....  
+000043a0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+000043b0: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+000043c0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+000043d0: 2020 2a2c 0a20 2020 2020 2020 2020 2020    *,.           
+000043e0: 206b 6579 3a20 6275 696c 7469 6e73 2e73   key: builtins.s
+000043f0: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+00004400: 2020 2020 2020 7661 6c75 653a 206e 7563        value: nuc
+00004410: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
+00004420: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
+00004430: 4669 6c65 207c 204e 6f6e 6520 3d20 2e2e  File | None = ..
+00004440: 2e2c 0a20 2020 2020 2020 2029 202d 3e20  .,.        ) -> 
+00004450: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 2020  None: ....      
+00004460: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
+00004470: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00004480: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00004490: 2276 616c 7565 222c 2062 2276 616c 7565  "value", b"value
+000044a0: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
+000044b0: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 2020  bool: ....      
+000044c0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
+000044d0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+000044e0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+000044f0: 6c5b 226b 6579 222c 2062 226b 6579 222c  l["key", b"key",
+00004500: 2022 7661 6c75 6522 2c20 6222 7661 6c75   "value", b"valu
+00004510: 6522 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  e"]) -> None: ..
+00004520: 2e0a 0a20 2020 204b 4249 445f 4649 454c  ...    KBID_FIEL
+00004530: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004540: 6e73 2e69 6e74 0a20 2020 2055 5549 445f  ns.int.    UUID_
+00004550: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00004560: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
+00004570: 4c55 475f 4649 454c 445f 4e55 4d42 4552  LUG_FIELD_NUMBER
+00004580: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00004590: 2020 2041 5544 4954 5f46 4945 4c44 5f4e     AUDIT_FIELD_N
+000045a0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+000045b0: 696e 740a 2020 2020 5459 5045 5f46 4945  int.    TYPE_FIE
+000045c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000045d0: 696e 732e 696e 740a 2020 2020 4d55 4c54  ins.int.    MULT
+000045e0: 4949 445f 4649 454c 445f 4e55 4d42 4552  IID_FIELD_NUMBER
+000045f0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00004600: 2020 2042 4153 4943 5f46 4945 4c44 5f4e     BASIC_FIELD_N
+00004610: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004620: 696e 740a 2020 2020 4f52 4947 494e 5f46  int.    ORIGIN_F
+00004630: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004640: 6c74 696e 732e 696e 740a 2020 2020 5245  ltins.int.    RE
+00004650: 4c41 5449 4f4e 535f 4649 454c 445f 4e55  LATIONS_FIELD_NU
+00004660: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00004670: 6e74 0a20 2020 2043 4f4e 5645 5253 4154  nt.    CONVERSAT
+00004680: 494f 4e53 5f46 4945 4c44 5f4e 554d 4245  IONS_FIELD_NUMBE
+00004690: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+000046a0: 2020 2020 4c41 594f 5554 535f 4649 454c      LAYOUTS_FIEL
+000046b0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+000046c0: 6e73 2e69 6e74 0a20 2020 2054 4558 5453  ns.int.    TEXTS
+000046d0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+000046e0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000046f0: 4b45 5957 4f52 4453 4554 535f 4649 454c  KEYWORDSETS_FIEL
+00004700: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004710: 6e73 2e69 6e74 0a20 2020 2044 4154 4554  ns.int.    DATET
+00004720: 494d 4553 5f46 4945 4c44 5f4e 554d 4245  IMES_FIELD_NUMBE
+00004730: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00004740: 2020 2020 4c49 4e4b 535f 4649 454c 445f      LINKS_FIELD_
+00004750: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00004760: 2e69 6e74 0a20 2020 2046 494c 4553 5f46  .int.    FILES_F
+00004770: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004780: 6c74 696e 732e 696e 740a 2020 2020 4c49  ltins.int.    LI
+00004790: 4e4b 5f45 5854 5241 4354 4544 5f44 4154  NK_EXTRACTED_DAT
+000047a0: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
+000047b0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000047c0: 2046 494c 455f 4558 5452 4143 5445 445f   FILE_EXTRACTED_
+000047d0: 4441 5441 5f46 4945 4c44 5f4e 554d 4245  DATA_FIELD_NUMBE
+000047e0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+000047f0: 2020 2020 4558 5452 4143 5445 445f 5445      EXTRACTED_TE
+00004800: 5854 5f46 4945 4c44 5f4e 554d 4245 523a  XT_FIELD_NUMBER:
+00004810: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00004820: 2020 4649 454c 445f 4d45 5441 4441 5441    FIELD_METADATA
+00004830: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00004840: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00004850: 4649 454c 445f 5645 4354 4f52 535f 4649  FIELD_VECTORS_FI
+00004860: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00004870: 7469 6e73 2e69 6e74 0a20 2020 2046 4945  tins.int.    FIE
+00004880: 4c44 5f4c 4152 4745 5f4d 4554 4144 4154  LD_LARGE_METADAT
+00004890: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
+000048a0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000048b0: 2044 454c 4554 455f 4649 454c 4453 5f46   DELETE_FIELDS_F
+000048c0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+000048d0: 6c74 696e 732e 696e 740a 2020 2020 4f52  ltins.int.    OR
+000048e0: 4947 494e 5f53 4551 5f46 4945 4c44 5f4e  IGIN_SEQ_FIELD_N
+000048f0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004900: 696e 740a 2020 2020 534c 4f57 5f50 524f  int.    SLOW_PRO
+00004910: 4345 5353 494e 475f 5449 4d45 5f46 4945  CESSING_TIME_FIE
+00004920: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00004930: 696e 732e 696e 740a 2020 2020 5052 455f  ins.int.    PRE_
+00004940: 5052 4f43 4553 5349 4e47 5f54 494d 455f  PROCESSING_TIME_
+00004950: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00004960: 696c 7469 6e73 2e69 6e74 0a20 2020 2044  iltins.int.    D
+00004970: 4f4e 455f 5449 4d45 5f46 4945 4c44 5f4e  ONE_TIME_FIELD_N
+00004980: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004990: 696e 740a 2020 2020 5458 5345 5149 445f  int.    TXSEQID_
+000049a0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+000049b0: 696c 7469 6e73 2e69 6e74 0a20 2020 2045  iltins.int.    E
+000049c0: 5252 4f52 535f 4649 454c 445f 4e55 4d42  RRORS_FIELD_NUMB
+000049d0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+000049e0: 0a20 2020 2050 524f 4345 5353 494e 475f  .    PROCESSING_
+000049f0: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
+00004a00: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00004a10: 2020 534f 5552 4345 5f46 4945 4c44 5f4e    SOURCE_FIELD_N
+00004a20: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004a30: 696e 740a 2020 2020 4143 434f 554e 545f  int.    ACCOUNT_
+00004a40: 5345 515f 4649 454c 445f 4e55 4d42 4552  SEQ_FIELD_NUMBER
+00004a50: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00004a60: 2020 2055 5345 525f 5645 4354 4f52 535f     USER_VECTORS_
+00004a70: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00004a80: 696c 7469 6e73 2e69 6e74 0a20 2020 2052  iltins.int.    R
+00004a90: 4549 4e44 4558 5f46 4945 4c44 5f4e 554d  EINDEX_FIELD_NUM
+00004aa0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00004ab0: 740a 2020 2020 4558 5452 415f 4649 454c  t.    EXTRA_FIEL
+00004ac0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004ad0: 6e73 2e69 6e74 0a20 2020 2051 5545 5354  ns.int.    QUEST
+00004ae0: 494f 4e5f 414e 5357 4552 535f 4649 454c  ION_ANSWERS_FIEL
+00004af0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004b00: 6e73 2e69 6e74 0a20 2020 2053 4543 5552  ns.int.    SECUR
+00004b10: 4954 595f 4649 454c 445f 4e55 4d42 4552  ITY_FIELD_NUMBER
+00004b20: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00004b30: 2020 206b 6269 643a 2062 7569 6c74 696e     kbid: builtin
+00004b40: 732e 7374 720a 2020 2020 7575 6964 3a20  s.str.    uuid: 
+00004b50: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+00004b60: 2073 6c75 673a 2062 7569 6c74 696e 732e   slug: builtins.
+00004b70: 7374 720a 2020 2020 7479 7065 3a20 676c  str.    type: gl
+00004b80: 6f62 616c 5f5f 5f42 726f 6b65 724d 6573  obal___BrokerMes
+00004b90: 7361 6765 2e4d 6573 7361 6765 5479 7065  sage.MessageType
+00004ba0: 2e56 616c 7565 5479 7065 0a20 2020 206d  .ValueType.    m
+00004bb0: 756c 7469 6964 3a20 6275 696c 7469 6e73  ultiid: builtins
+00004bc0: 2e73 7472 0a20 2020 206f 7269 6769 6e5f  .str.    origin_
+00004bd0: 7365 713a 2062 7569 6c74 696e 732e 696e  seq: builtins.in
+00004be0: 740a 2020 2020 736c 6f77 5f70 726f 6365  t.    slow_proce
+00004bf0: 7373 696e 675f 7469 6d65 3a20 6275 696c  ssing_time: buil
+00004c00: 7469 6e73 2e66 6c6f 6174 0a20 2020 2070  tins.float.    p
+00004c10: 7265 5f70 726f 6365 7373 696e 675f 7469  re_processing_ti
+00004c20: 6d65 3a20 6275 696c 7469 6e73 2e66 6c6f  me: builtins.flo
+00004c30: 6174 0a20 2020 2074 7873 6571 6964 3a20  at.    txseqid: 
+00004c40: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004c50: 2022 2222 4e6f 7420 6e65 6564 6564 2061   """Not needed a
+00004c60: 6e79 6d6f 7265 2222 220a 2020 2020 7072  nymore""".    pr
+00004c70: 6f63 6573 7369 6e67 5f69 643a 2062 7569  ocessing_id: bui
+00004c80: 6c74 696e 732e 7374 720a 2020 2020 736f  ltins.str.    so
+00004c90: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
+00004ca0: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
+00004cb0: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
+00004cc0: 5479 7065 0a20 2020 2061 6363 6f75 6e74  Type.    account
+00004cd0: 5f73 6571 3a20 6275 696c 7469 6e73 2e69  _seq: builtins.i
+00004ce0: 6e74 0a20 2020 2072 6569 6e64 6578 3a20  nt.    reindex: 
+00004cf0: 6275 696c 7469 6e73 2e62 6f6f 6c0a 2020  builtins.bool.  
+00004d00: 2020 2222 2249 6620 7472 7565 2c20 666f    """If true, fo
+00004d10: 7263 6520 7265 696e 6465 7820 616c 6c20  rce reindex all 
+00004d20: 7061 7261 6772 6170 6873 2069 6e20 6120  paragraphs in a 
+00004d30: 7265 736f 7572 6365 2222 220a 2020 2020  resource""".    
+00004d40: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00004d50: 6620 6175 6469 7428 7365 6c66 2920 2d3e  f audit(self) ->
+00004d60: 2067 6c6f 6261 6c5f 5f5f 4175 6469 743a   global___Audit:
+00004d70: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
+00004d80: 7479 0a20 2020 2064 6566 2062 6173 6963  ty.    def basic
+00004d90: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
+00004da0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00004db0: 6365 735f 7062 322e 4261 7369 633a 202e  ces_pb2.Basic: .
+00004dc0: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00004dd0: 0a20 2020 2064 6566 206f 7269 6769 6e28  .    def origin(
+00004de0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+00004df0: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00004e00: 6573 5f70 6232 2e4f 7269 6769 6e3a 202e  es_pb2.Origin: .
+00004e10: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00004e20: 0a20 2020 2064 6566 2072 656c 6174 696f  .    def relatio
+00004e30: 6e73 2873 656c 6629 202d 3e20 676f 6f67  ns(self) -> goog
+00004e40: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00004e50: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+00004e60: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+00004e70: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+00004e80: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00004e90: 7574 696c 735f 7062 322e 5265 6c61 7469  utils_pb2.Relati
+00004ea0: 6f6e 5d3a 202e 2e2e 0a20 2020 2040 7072  on]: ....    @pr
+00004eb0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00004ec0: 6f6e 7665 7273 6174 696f 6e73 2873 656c  onversations(sel
+00004ed0: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
+00004ee0: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
+00004ef0: 6f6e 7461 696e 6572 732e 4d65 7373 6167  ontainers.Messag
+00004f00: 654d 6170 5b62 7569 6c74 696e 732e 7374  eMap[builtins.st
+00004f10: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
+00004f20: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
+00004f30: 2e43 6f6e 7665 7273 6174 696f 6e5d 3a0a  .Conversation]:.
+00004f40: 2020 2020 2020 2020 2222 2246 6965 6c64          """Field
+00004f50: 2043 6f6e 7665 7273 6174 696f 6e73 2222   Conversations""
+00004f60: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
+00004f70: 0a20 2020 2064 6566 206c 6179 6f75 7473  .    def layouts
+00004f80: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
+00004f90: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
+00004fa0: 616c 2e63 6f6e 7461 696e 6572 732e 4d65  al.containers.Me
+00004fb0: 7373 6167 654d 6170 5b62 7569 6c74 696e  ssageMap[builtin
+00004fc0: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
+00004fd0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+00004fe0: 5f70 6232 2e46 6965 6c64 4c61 796f 7574  _pb2.FieldLayout
+00004ff0: 5d3a 0a20 2020 2020 2020 2022 2222 4669  ]:.        """Fi
+00005000: 656c 6420 4c61 796f 7574 2222 220a 0a20  eld Layout""".. 
+00005010: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00005020: 2064 6566 2074 6578 7473 2873 656c 6629   def texts(self)
+00005030: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
+00005040: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
+00005050: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
+00005060: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
+00005070: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00005080: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00005090: 6965 6c64 5465 7874 5d3a 0a20 2020 2020  ieldText]:.     
+000050a0: 2020 2022 2222 4669 656c 6420 5465 7874     """Field Text
+000050b0: 2222 220a 0a20 2020 2040 7072 6f70 6572  """..    @proper
+000050c0: 7479 0a20 2020 2064 6566 206b 6579 776f  ty.    def keywo
+000050d0: 7264 7365 7473 2873 656c 6629 202d 3e20  rdsets(self) -> 
+000050e0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+000050f0: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
+00005100: 6572 732e 4d65 7373 6167 654d 6170 5b62  ers.MessageMap[b
+00005110: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
+00005120: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
+00005130: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
+00005140: 4b65 7977 6f72 6473 6574 5d3a 0a20 2020  Keywordset]:.   
+00005150: 2020 2020 2022 2222 4669 656c 6420 6b65       """Field ke
+00005160: 7977 6f72 6422 2222 0a0a 2020 2020 4070  yword"""..    @p
+00005170: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00005180: 6461 7465 7469 6d65 7328 7365 6c66 2920  datetimes(self) 
+00005190: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
+000051a0: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
+000051b0: 6169 6e65 7273 2e4d 6573 7361 6765 4d61  ainers.MessageMa
+000051c0: 705b 6275 696c 7469 6e73 2e73 7472 2c20  p[builtins.str, 
+000051d0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+000051e0: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
+000051f0: 656c 6444 6174 6574 696d 655d 3a0a 2020  eldDatetime]:.  
+00005200: 2020 2020 2020 2222 2246 6965 6c64 2044        """Field D
+00005210: 6174 6574 696d 6522 2222 0a0a 2020 2020  atetime"""..    
+00005220: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00005230: 6620 6c69 6e6b 7328 7365 6c66 2920 2d3e  f links(self) ->
+00005240: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00005250: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
+00005260: 6e65 7273 2e4d 6573 7361 6765 4d61 705b  ners.MessageMap[
+00005270: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
+00005280: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00005290: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+000052a0: 644c 696e 6b5d 3a0a 2020 2020 2020 2020  dLink]:.        
+000052b0: 2222 2246 6965 6c64 204c 696e 6b73 2222  """Field Links""
+000052c0: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
+000052d0: 0a20 2020 2064 6566 2066 696c 6573 2873  .    def files(s
+000052e0: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
+000052f0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+00005300: 2e63 6f6e 7461 696e 6572 732e 4d65 7373  .containers.Mess
+00005310: 6167 654d 6170 5b62 7569 6c74 696e 732e  ageMap[builtins.
+00005320: 7374 722c 206e 7563 6c69 6164 625f 7072  str, nucliadb_pr
+00005330: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00005340: 6232 2e46 6965 6c64 4669 6c65 5d3a 0a20  b2.FieldFile]:. 
+00005350: 2020 2020 2020 2022 2222 4669 656c 6420         """Field 
+00005360: 4669 6c65 2222 220a 0a20 2020 2040 7072  File"""..    @pr
+00005370: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+00005380: 696e 6b5f 6578 7472 6163 7465 645f 6461  ink_extracted_da
+00005390: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
+000053a0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+000053b0: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+000053c0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+000053d0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+000053e0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+000053f0: 7265 736f 7572 6365 735f 7062 322e 4c69  resources_pb2.Li
+00005400: 6e6b 4578 7472 6163 7465 6444 6174 615d  nkExtractedData]
+00005410: 3a0a 2020 2020 2020 2020 2222 224c 696e  :.        """Lin
+00005420: 6b20 6578 7472 6163 7465 6420 6578 7472  k extracted extr
+00005430: 6120 696e 666f 2222 220a 0a20 2020 2040  a info"""..    @
+00005440: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00005450: 2066 696c 655f 6578 7472 6163 7465 645f   file_extracted_
+00005460: 6461 7461 2873 656c 6629 202d 3e20 676f  data(self) -> go
+00005470: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+00005480: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+00005490: 732e 5265 7065 6174 6564 436f 6d70 6f73  s.RepeatedCompos
+000054a0: 6974 6546 6965 6c64 436f 6e74 6169 6e65  iteFieldContaine
+000054b0: 725b 6e75 636c 6961 6462 5f70 726f 746f  r[nucliadb_proto
+000054c0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+000054d0: 4669 6c65 4578 7472 6163 7465 6444 6174  FileExtractedDat
+000054e0: 615d 3a0a 2020 2020 2020 2020 2222 2246  a]:.        """F
+000054f0: 696c 6520 6578 7472 6163 7465 6420 6578  ile extracted ex
+00005500: 7472 6120 696e 666f 2222 220a 0a20 2020  tra info"""..   
+00005510: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00005520: 6566 2065 7874 7261 6374 6564 5f74 6578  ef extracted_tex
+00005530: 7428 7365 6c66 2920 2d3e 2067 6f6f 676c  t(self) -> googl
+00005540: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+00005550: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
+00005560: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
+00005570: 4669 656c 6443 6f6e 7461 696e 6572 5b6e  FieldContainer[n
+00005580: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00005590: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
+000055a0: 7261 6374 6564 5465 7874 5772 6170 7065  ractedTextWrappe
+000055b0: 725d 3a0a 2020 2020 2020 2020 2222 2246  r]:.        """F
+000055c0: 6965 6c64 2045 7874 7261 6374 6564 2f43  ield Extracted/C
+000055d0: 6f6d 7075 7465 6420 696e 666f 726d 6174  omputed informat
+000055e0: 696f 6e22 2222 0a0a 2020 2020 4070 726f  ion"""..    @pro
+000055f0: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
+00005600: 656c 645f 6d65 7461 6461 7461 2873 656c  eld_metadata(sel
+00005610: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
+00005620: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
+00005630: 6f6e 7461 696e 6572 732e 5265 7065 6174  ontainers.Repeat
+00005640: 6564 436f 6d70 6f73 6974 6546 6965 6c64  edCompositeField
+00005650: 436f 6e74 6169 6e65 725b 6e75 636c 6961  Container[nuclia
+00005660: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00005670: 6365 735f 7062 322e 4669 656c 6443 6f6d  ces_pb2.FieldCom
+00005680: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
+00005690: 7070 6572 5d3a 202e 2e2e 0a20 2020 2040  pper]: ....    @
+000056a0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000056b0: 2066 6965 6c64 5f76 6563 746f 7273 2873   field_vectors(s
+000056c0: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
+000056d0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+000056e0: 2e63 6f6e 7461 696e 6572 732e 5265 7065  .containers.Repe
+000056f0: 6174 6564 436f 6d70 6f73 6974 6546 6965  atedCompositeFie
+00005700: 6c64 436f 6e74 6169 6e65 725b 6e75 636c  ldContainer[nucl
+00005710: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
+00005720: 7572 6365 735f 7062 322e 4578 7472 6163  urces_pb2.Extrac
+00005730: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
+00005740: 725d 3a20 2e2e 2e0a 2020 2020 4070 726f  r]: ....    @pro
+00005750: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
+00005760: 656c 645f 6c61 7267 655f 6d65 7461 6461  eld_large_metada
+00005770: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
+00005780: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00005790: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+000057a0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+000057b0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+000057c0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+000057d0: 7265 736f 7572 6365 735f 7062 322e 4c61  resources_pb2.La
+000057e0: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
+000057f0: 6174 6157 7261 7070 6572 5d3a 0a20 2020  ataWrapper]:.   
+00005800: 2020 2020 2022 2222 5265 736f 7572 6365       """Resource
+00005810: 204c 6172 6765 2043 6f6d 7075 7465 6420   Large Computed 
+00005820: 4d65 7461 6461 7461 2222 220a 0a20 2020  Metadata"""..   
+00005830: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00005840: 6566 2064 656c 6574 655f 6669 656c 6473  ef delete_fields
+00005850: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
+00005860: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
+00005870: 616c 2e63 6f6e 7461 696e 6572 732e 5265  al.containers.Re
+00005880: 7065 6174 6564 436f 6d70 6f73 6974 6546  peatedCompositeF
+00005890: 6965 6c64 436f 6e74 6169 6e65 725b 6e75  ieldContainer[nu
+000058a0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+000058b0: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+000058c0: 6449 445d 3a20 2e2e 2e0a 2020 2020 4070  dID]: ....    @p
+000058d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000058e0: 646f 6e65 5f74 696d 6528 7365 6c66 2920  done_time(self) 
+000058f0: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
+00005900: 7566 2e74 696d 6573 7461 6d70 5f70 6232  uf.timestamp_pb2
+00005910: 2e54 696d 6573 7461 6d70 3a20 2e2e 2e0a  .Timestamp: ....
+00005920: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00005930: 2020 6465 6620 6572 726f 7273 2873 656c    def errors(sel
+00005940: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
+00005950: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
+00005960: 6f6e 7461 696e 6572 732e 5265 7065 6174  ontainers.Repeat
+00005970: 6564 436f 6d70 6f73 6974 6546 6965 6c64  edCompositeField
+00005980: 436f 6e74 6169 6e65 725b 676c 6f62 616c  Container[global
+00005990: 5f5f 5f45 7272 6f72 5d3a 202e 2e2e 0a20  ___Error]: .... 
+000059a0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000059b0: 2064 6566 2075 7365 725f 7665 6374 6f72   def user_vector
+000059c0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
+000059d0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+000059e0: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
+000059f0: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
+00005a00: 4669 656c 6443 6f6e 7461 696e 6572 5b6e  FieldContainer[n
+00005a10: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00005a20: 6573 6f75 7263 6573 5f70 6232 2e55 7365  esources_pb2.Use
+00005a30: 7256 6563 746f 7273 5772 6170 7065 725d  rVectorsWrapper]
+00005a40: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
+00005a50: 7274 790a 2020 2020 6465 6620 6578 7472  rty.    def extr
+00005a60: 6128 7365 6c66 2920 2d3e 206e 7563 6c69  a(self) -> nucli
+00005a70: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
+00005a80: 7263 6573 5f70 6232 2e45 7874 7261 3a20  rces_pb2.Extra: 
+00005a90: 2e2e 2e0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00005aa0: 790a 2020 2020 6465 6620 7175 6573 7469  y.    def questi
+00005ab0: 6f6e 5f61 6e73 7765 7273 2873 656c 6629  on_answers(self)
+00005ac0: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
+00005ad0: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
+00005ae0: 7461 696e 6572 732e 5265 7065 6174 6564  tainers.Repeated
+00005af0: 436f 6d70 6f73 6974 6546 6965 6c64 436f  CompositeFieldCo
+00005b00: 6e74 6169 6e65 725b 6e75 636c 6961 6462  ntainer[nucliadb
+00005b10: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00005b20: 735f 7062 322e 4669 656c 6451 7565 7374  s_pb2.FieldQuest
+00005b30: 696f 6e41 6e73 7765 7257 7261 7070 6572  ionAnswerWrapper
+00005b40: 5d3a 202e 2e2e 0a20 2020 2040 7072 6f70  ]: ....    @prop
+00005b50: 6572 7479 0a20 2020 2064 6566 2073 6563  erty.    def sec
+00005b60: 7572 6974 7928 7365 6c66 2920 2d3e 206e  urity(self) -> n
+00005b70: 7563 6c69 6164 625f 7072 6f74 6f73 2e75  ucliadb_protos.u
+00005b80: 7469 6c73 5f70 6232 2e53 6563 7572 6974  tils_pb2.Securit
+00005b90: 793a 202e 2e2e 0a20 2020 2064 6566 205f  y: ....    def _
+00005ba0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00005bb0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+00005bc0: 2c0a 2020 2020 2020 2020 6b62 6964 3a20  ,.        kbid: 
+00005bd0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00005be0: 2e2e 2c0a 2020 2020 2020 2020 7575 6964  ..,.        uuid
+00005bf0: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00005c00: 202e 2e2e 2c0a 2020 2020 2020 2020 736c   ...,.        sl
+00005c10: 7567 3a20 6275 696c 7469 6e73 2e73 7472  ug: builtins.str
+00005c20: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00005c30: 6175 6469 743a 2067 6c6f 6261 6c5f 5f5f  audit: global___
+00005c40: 4175 6469 7420 7c20 4e6f 6e65 203d 202e  Audit | None = .
+00005c50: 2e2e 2c0a 2020 2020 2020 2020 7479 7065  ..,.        type
+00005c60: 3a20 676c 6f62 616c 5f5f 5f42 726f 6b65  : global___Broke
+00005c70: 724d 6573 7361 6765 2e4d 6573 7361 6765  rMessage.Message
+00005c80: 5479 7065 2e56 616c 7565 5479 7065 203d  Type.ValueType =
+00005c90: 202e 2e2e 2c0a 2020 2020 2020 2020 6d75   ...,.        mu
+00005ca0: 6c74 6969 643a 2062 7569 6c74 696e 732e  ltiid: builtins.
+00005cb0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+00005cc0: 2020 2062 6173 6963 3a20 6e75 636c 6961     basic: nuclia
+00005cd0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00005ce0: 6365 735f 7062 322e 4261 7369 6320 7c20  ces_pb2.Basic | 
+00005cf0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00005d00: 2020 2020 6f72 6967 696e 3a20 6e75 636c      origin: nucl
+00005d10: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
+00005d20: 7572 6365 735f 7062 322e 4f72 6967 696e  urces_pb2.Origin
+00005d30: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00005d40: 2020 2020 2020 2072 656c 6174 696f 6e73         relations
+00005d50: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
+00005d60: 632e 4974 6572 6162 6c65 5b6e 7563 6c69  c.Iterable[nucli
+00005d70: 6164 625f 7072 6f74 6f73 2e75 7469 6c73  adb_protos.utils
+00005d80: 5f70 6232 2e52 656c 6174 696f 6e5d 207c  _pb2.Relation] |
+00005d90: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+00005da0: 2020 2020 2063 6f6e 7665 7273 6174 696f       conversatio
+00005db0: 6e73 3a20 636f 6c6c 6563 7469 6f6e 732e  ns: collections.
+00005dc0: 6162 632e 4d61 7070 696e 675b 6275 696c  abc.Mapping[buil
+00005dd0: 7469 6e73 2e73 7472 2c20 6e75 636c 6961  tins.str, nuclia
+00005de0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00005df0: 6365 735f 7062 322e 436f 6e76 6572 7361  ces_pb2.Conversa
+00005e00: 7469 6f6e 5d20 7c20 4e6f 6e65 203d 202e  tion] | None = .
+00005e10: 2e2e 2c0a 2020 2020 2020 2020 6c61 796f  ..,.        layo
+00005e20: 7574 733a 2063 6f6c 6c65 6374 696f 6e73  uts: collections
+00005e30: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
+00005e40: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+00005e50: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
+00005e60: 7263 6573 5f70 6232 2e46 6965 6c64 4c61  rces_pb2.FieldLa
+00005e70: 796f 7574 5d20 7c20 4e6f 6e65 203d 202e  yout] | None = .
+00005e80: 2e2e 2c0a 2020 2020 2020 2020 7465 7874  ..,.        text
+00005e90: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
+00005ea0: 6263 2e4d 6170 7069 6e67 5b62 7569 6c74  bc.Mapping[built
+00005eb0: 696e 732e 7374 722c 206e 7563 6c69 6164  ins.str, nucliad
+00005ec0: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00005ed0: 6573 5f70 6232 2e46 6965 6c64 5465 7874  es_pb2.FieldText
+00005ee0: 5d20 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  ] | None = ...,.
+00005ef0: 2020 2020 2020 2020 6b65 7977 6f72 6473          keywords
+00005f00: 6574 733a 2063 6f6c 6c65 6374 696f 6e73  ets: collections
+00005f10: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
+00005f20: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+00005f30: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
+00005f40: 7263 6573 5f70 6232 2e46 6965 6c64 4b65  rces_pb2.FieldKe
+00005f50: 7977 6f72 6473 6574 5d20 7c20 4e6f 6e65  ywordset] | None
+00005f60: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00005f70: 6461 7465 7469 6d65 733a 2063 6f6c 6c65  datetimes: colle
+00005f80: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+00005f90: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+00005fa0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00005fb0: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00005fc0: 6965 6c64 4461 7465 7469 6d65 5d20 7c20  ieldDatetime] | 
+00005fd0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00005fe0: 2020 2020 6c69 6e6b 733a 2063 6f6c 6c65      links: colle
+00005ff0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+00006000: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+00006010: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00006020: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00006030: 6965 6c64 4c69 6e6b 5d20 7c20 4e6f 6e65  ieldLink] | None
+00006040: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00006050: 6669 6c65 733a 2063 6f6c 6c65 6374 696f  files: collectio
+00006060: 6e73 2e61 6263 2e4d 6170 7069 6e67 5b62  ns.abc.Mapping[b
+00006070: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
+00006080: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
+00006090: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
+000060a0: 4669 6c65 5d20 7c20 4e6f 6e65 203d 202e  File] | None = .
+000060b0: 2e2e 2c0a 2020 2020 2020 2020 6c69 6e6b  ..,.        link
+000060c0: 5f65 7874 7261 6374 6564 5f64 6174 613a  _extracted_data:
+000060d0: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+000060e0: 2e49 7465 7261 626c 655b 6e75 636c 6961  .Iterable[nuclia
+000060f0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00006100: 6365 735f 7062 322e 4c69 6e6b 4578 7472  ces_pb2.LinkExtr
+00006110: 6163 7465 6444 6174 615d 207c 204e 6f6e  actedData] | Non
+00006120: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+00006130: 2066 696c 655f 6578 7472 6163 7465 645f   file_extracted_
+00006140: 6461 7461 3a20 636f 6c6c 6563 7469 6f6e  data: collection
+00006150: 732e 6162 632e 4974 6572 6162 6c65 5b6e  s.abc.Iterable[n
+00006160: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00006170: 6573 6f75 7263 6573 5f70 6232 2e46 696c  esources_pb2.Fil
+00006180: 6545 7874 7261 6374 6564 4461 7461 5d20  eExtractedData] 
+00006190: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+000061a0: 2020 2020 2020 6578 7472 6163 7465 645f        extracted_
+000061b0: 7465 7874 3a20 636f 6c6c 6563 7469 6f6e  text: collection
+000061c0: 732e 6162 632e 4974 6572 6162 6c65 5b6e  s.abc.Iterable[n
+000061d0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+000061e0: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
+000061f0: 7261 6374 6564 5465 7874 5772 6170 7065  ractedTextWrappe
+00006200: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
+00006210: 0a20 2020 2020 2020 2066 6965 6c64 5f6d  .        field_m
+00006220: 6574 6164 6174 613a 2063 6f6c 6c65 6374  etadata: collect
+00006230: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
+00006240: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
+00006250: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00006260: 4669 656c 6443 6f6d 7075 7465 644d 6574  FieldComputedMet
+00006270: 6164 6174 6157 7261 7070 6572 5d20 7c20  adataWrapper] | 
+00006280: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00006290: 2020 2020 6669 656c 645f 7665 6374 6f72      field_vector
+000062a0: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
+000062b0: 6263 2e49 7465 7261 626c 655b 6e75 636c  bc.Iterable[nucl
+000062c0: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
+000062d0: 7572 6365 735f 7062 322e 4578 7472 6163  urces_pb2.Extrac
+000062e0: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
+000062f0: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
+00006300: 0a20 2020 2020 2020 2066 6965 6c64 5f6c  .        field_l
+00006310: 6172 6765 5f6d 6574 6164 6174 613a 2063  arge_metadata: c
+00006320: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
+00006330: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
+00006340: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00006350: 735f 7062 322e 4c61 7267 6543 6f6d 7075  s_pb2.LargeCompu
+00006360: 7465 644d 6574 6164 6174 6157 7261 7070  tedMetadataWrapp
+00006370: 6572 5d20 7c20 4e6f 6e65 203d 202e 2e2e  er] | None = ...
+00006380: 2c0a 2020 2020 2020 2020 6465 6c65 7465  ,.        delete
+00006390: 5f66 6965 6c64 733a 2063 6f6c 6c65 6374  _fields: collect
+000063a0: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
+000063b0: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
+000063c0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+000063d0: 4669 656c 6449 445d 207c 204e 6f6e 6520  FieldID] | None 
+000063e0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206f  = ...,.        o
+000063f0: 7269 6769 6e5f 7365 713a 2062 7569 6c74  rigin_seq: built
+00006400: 696e 732e 696e 7420 3d20 2e2e 2e2c 0a20  ins.int = ...,. 
+00006410: 2020 2020 2020 2073 6c6f 775f 7072 6f63         slow_proc
+00006420: 6573 7369 6e67 5f74 696d 653a 2062 7569  essing_time: bui
+00006430: 6c74 696e 732e 666c 6f61 7420 3d20 2e2e  ltins.float = ..
+00006440: 2e2c 0a20 2020 2020 2020 2070 7265 5f70  .,.        pre_p
+00006450: 726f 6365 7373 696e 675f 7469 6d65 3a20  rocessing_time: 
+00006460: 6275 696c 7469 6e73 2e66 6c6f 6174 203d  builtins.float =
+00006470: 202e 2e2e 2c0a 2020 2020 2020 2020 646f   ...,.        do
+00006480: 6e65 5f74 696d 653a 2067 6f6f 676c 652e  ne_time: google.
+00006490: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
+000064a0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
+000064b0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+000064c0: 2020 2020 2020 2074 7873 6571 6964 3a20         txseqid: 
+000064d0: 6275 696c 7469 6e73 2e69 6e74 203d 202e  builtins.int = .
+000064e0: 2e2e 2c0a 2020 2020 2020 2020 6572 726f  ..,.        erro
+000064f0: 7273 3a20 636f 6c6c 6563 7469 6f6e 732e  rs: collections.
+00006500: 6162 632e 4974 6572 6162 6c65 5b67 6c6f  abc.Iterable[glo
+00006510: 6261 6c5f 5f5f 4572 726f 725d 207c 204e  bal___Error] | N
+00006520: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+00006530: 2020 2070 726f 6365 7373 696e 675f 6964     processing_id
+00006540: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00006550: 202e 2e2e 2c0a 2020 2020 2020 2020 736f   ...,.        so
+00006560: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
+00006570: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
+00006580: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
+00006590: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+000065a0: 2020 2020 6163 636f 756e 745f 7365 713a      account_seq:
+000065b0: 2062 7569 6c74 696e 732e 696e 7420 3d20   builtins.int = 
+000065c0: 2e2e 2e2c 0a20 2020 2020 2020 2075 7365  ...,.        use
+000065d0: 725f 7665 6374 6f72 733a 2063 6f6c 6c65  r_vectors: colle
+000065e0: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
+000065f0: 626c 655b 6e75 636c 6961 6462 5f70 726f  ble[nucliadb_pro
+00006600: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+00006610: 322e 5573 6572 5665 6374 6f72 7357 7261  2.UserVectorsWra
+00006620: 7070 6572 5d20 7c20 4e6f 6e65 203d 202e  pper] | None = .
+00006630: 2e2e 2c0a 2020 2020 2020 2020 7265 696e  ..,.        rein
+00006640: 6465 783a 2062 7569 6c74 696e 732e 626f  dex: builtins.bo
+00006650: 6f6c 203d 202e 2e2e 2c0a 2020 2020 2020  ol = ...,.      
+00006660: 2020 6578 7472 613a 206e 7563 6c69 6164    extra: nucliad
+00006670: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00006680: 6573 5f70 6232 2e45 7874 7261 207c 204e  es_pb2.Extra | N
+00006690: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+000066a0: 2020 2071 7565 7374 696f 6e5f 616e 7377     question_answ
+000066b0: 6572 733a 2063 6f6c 6c65 6374 696f 6e73  ers: collections
+000066c0: 2e61 6263 2e49 7465 7261 626c 655b 6e75  .abc.Iterable[nu
+000066d0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+000066e0: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+000066f0: 6451 7565 7374 696f 6e41 6e73 7765 7257  dQuestionAnswerW
+00006700: 7261 7070 6572 5d20 7c20 4e6f 6e65 203d  rapper] | None =
+00006710: 202e 2e2e 2c0a 2020 2020 2020 2020 7365   ...,.        se
+00006720: 6375 7269 7479 3a20 6e75 636c 6961 6462  curity: nucliadb
+00006730: 5f70 726f 746f 732e 7574 696c 735f 7062  _protos.utils_pb
+00006740: 322e 5365 6375 7269 7479 207c 204e 6f6e  2.Security | Non
+00006750: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+00006760: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+00006770: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+00006780: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00006790: 7970 696e 672e 4c69 7465 7261 6c5b 2261  yping.Literal["a
+000067a0: 7564 6974 222c 2062 2261 7564 6974 222c  udit", b"audit",
+000067b0: 2022 6261 7369 6322 2c20 6222 6261 7369   "basic", b"basi
+000067c0: 6322 2c20 2264 6f6e 655f 7469 6d65 222c  c", "done_time",
+000067d0: 2062 2264 6f6e 655f 7469 6d65 222c 2022   b"done_time", "
+000067e0: 6578 7472 6122 2c20 6222 6578 7472 6122  extra", b"extra"
+000067f0: 2c20 226f 7269 6769 6e22 2c20 6222 6f72  , "origin", b"or
+00006800: 6967 696e 222c 2022 7365 6375 7269 7479  igin", "security
+00006810: 222c 2062 2273 6563 7572 6974 7922 5d29  ", b"security"])
+00006820: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
+00006830: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
+00006840: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+00006850: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00006860: 6e67 2e4c 6974 6572 616c 5b22 6163 636f  ng.Literal["acco
+00006870: 756e 745f 7365 7122 2c20 6222 6163 636f  unt_seq", b"acco
+00006880: 756e 745f 7365 7122 2c20 2261 7564 6974  unt_seq", "audit
+00006890: 222c 2062 2261 7564 6974 222c 2022 6261  ", b"audit", "ba
+000068a0: 7369 6322 2c20 6222 6261 7369 6322 2c20  sic", b"basic", 
+000068b0: 2263 6f6e 7665 7273 6174 696f 6e73 222c  "conversations",
+000068c0: 2062 2263 6f6e 7665 7273 6174 696f 6e73   b"conversations
+000068d0: 222c 2022 6461 7465 7469 6d65 7322 2c20  ", "datetimes", 
+000068e0: 6222 6461 7465 7469 6d65 7322 2c20 2264  b"datetimes", "d
+000068f0: 656c 6574 655f 6669 656c 6473 222c 2062  elete_fields", b
+00006900: 2264 656c 6574 655f 6669 656c 6473 222c  "delete_fields",
+00006910: 2022 646f 6e65 5f74 696d 6522 2c20 6222   "done_time", b"
+00006920: 646f 6e65 5f74 696d 6522 2c20 2265 7272  done_time", "err
+00006930: 6f72 7322 2c20 6222 6572 726f 7273 222c  ors", b"errors",
+00006940: 2022 6578 7472 6122 2c20 6222 6578 7472   "extra", b"extr
+00006950: 6122 2c20 2265 7874 7261 6374 6564 5f74  a", "extracted_t
+00006960: 6578 7422 2c20 6222 6578 7472 6163 7465  ext", b"extracte
+00006970: 645f 7465 7874 222c 2022 6669 656c 645f  d_text", "field_
+00006980: 6c61 7267 655f 6d65 7461 6461 7461 222c  large_metadata",
+00006990: 2062 2266 6965 6c64 5f6c 6172 6765 5f6d   b"field_large_m
+000069a0: 6574 6164 6174 6122 2c20 2266 6965 6c64  etadata", "field
+000069b0: 5f6d 6574 6164 6174 6122 2c20 6222 6669  _metadata", b"fi
+000069c0: 656c 645f 6d65 7461 6461 7461 222c 2022  eld_metadata", "
+000069d0: 6669 656c 645f 7665 6374 6f72 7322 2c20  field_vectors", 
+000069e0: 6222 6669 656c 645f 7665 6374 6f72 7322  b"field_vectors"
+000069f0: 2c20 2266 696c 655f 6578 7472 6163 7465  , "file_extracte
+00006a00: 645f 6461 7461 222c 2062 2266 696c 655f  d_data", b"file_
+00006a10: 6578 7472 6163 7465 645f 6461 7461 222c  extracted_data",
+00006a20: 2022 6669 6c65 7322 2c20 6222 6669 6c65   "files", b"file
+00006a30: 7322 2c20 226b 6269 6422 2c20 6222 6b62  s", "kbid", b"kb
+00006a40: 6964 222c 2022 6b65 7977 6f72 6473 6574  id", "keywordset
+00006a50: 7322 2c20 6222 6b65 7977 6f72 6473 6574  s", b"keywordset
+00006a60: 7322 2c20 226c 6179 6f75 7473 222c 2062  s", "layouts", b
+00006a70: 226c 6179 6f75 7473 222c 2022 6c69 6e6b  "layouts", "link
+00006a80: 5f65 7874 7261 6374 6564 5f64 6174 6122  _extracted_data"
+00006a90: 2c20 6222 6c69 6e6b 5f65 7874 7261 6374  , b"link_extract
+00006aa0: 6564 5f64 6174 6122 2c20 226c 696e 6b73  ed_data", "links
+00006ab0: 222c 2062 226c 696e 6b73 222c 2022 6d75  ", b"links", "mu
+00006ac0: 6c74 6969 6422 2c20 6222 6d75 6c74 6969  ltiid", b"multii
+00006ad0: 6422 2c20 226f 7269 6769 6e22 2c20 6222  d", "origin", b"
+00006ae0: 6f72 6967 696e 222c 2022 6f72 6967 696e  origin", "origin
+00006af0: 5f73 6571 222c 2062 226f 7269 6769 6e5f  _seq", b"origin_
+00006b00: 7365 7122 2c20 2270 7265 5f70 726f 6365  seq", "pre_proce
+00006b10: 7373 696e 675f 7469 6d65 222c 2062 2270  ssing_time", b"p
+00006b20: 7265 5f70 726f 6365 7373 696e 675f 7469  re_processing_ti
+00006b30: 6d65 222c 2022 7072 6f63 6573 7369 6e67  me", "processing
+00006b40: 5f69 6422 2c20 6222 7072 6f63 6573 7369  _id", b"processi
+00006b50: 6e67 5f69 6422 2c20 2271 7565 7374 696f  ng_id", "questio
+00006b60: 6e5f 616e 7377 6572 7322 2c20 6222 7175  n_answers", b"qu
+00006b70: 6573 7469 6f6e 5f61 6e73 7765 7273 222c  estion_answers",
+00006b80: 2022 7265 696e 6465 7822 2c20 6222 7265   "reindex", b"re
+00006b90: 696e 6465 7822 2c20 2272 656c 6174 696f  index", "relatio
+00006ba0: 6e73 222c 2062 2272 656c 6174 696f 6e73  ns", b"relations
+00006bb0: 222c 2022 7365 6375 7269 7479 222c 2062  ", "security", b
+00006bc0: 2273 6563 7572 6974 7922 2c20 2273 6c6f  "security", "slo
+00006bd0: 775f 7072 6f63 6573 7369 6e67 5f74 696d  w_processing_tim
+00006be0: 6522 2c20 6222 736c 6f77 5f70 726f 6365  e", b"slow_proce
+00006bf0: 7373 696e 675f 7469 6d65 222c 2022 736c  ssing_time", "sl
+00006c00: 7567 222c 2062 2273 6c75 6722 2c20 2273  ug", b"slug", "s
+00006c10: 6f75 7263 6522 2c20 6222 736f 7572 6365  ource", b"source
+00006c20: 222c 2022 7465 7874 7322 2c20 6222 7465  ", "texts", b"te
+00006c30: 7874 7322 2c20 2274 7873 6571 6964 222c  xts", "txseqid",
+00006c40: 2062 2274 7873 6571 6964 222c 2022 7479   b"txseqid", "ty
+00006c50: 7065 222c 2062 2274 7970 6522 2c20 2275  pe", b"type", "u
+00006c60: 7365 725f 7665 6374 6f72 7322 2c20 6222  ser_vectors", b"
+00006c70: 7573 6572 5f76 6563 746f 7273 222c 2022  user_vectors", "
+00006c80: 7575 6964 222c 2062 2275 7569 6422 5d29  uuid", b"uuid"])
+00006c90: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+00006ca0: 6c6f 6261 6c5f 5f5f 4272 6f6b 6572 4d65  lobal___BrokerMe
+00006cb0: 7373 6167 6520 3d20 4272 6f6b 6572 4d65  ssage = BrokerMe
+00006cc0: 7373 6167 650a 0a40 7479 7069 6e67 2e66  ssage..@typing.f
+00006cd0: 696e 616c 0a63 6c61 7373 2042 726f 6b65  inal.class Broke
+00006ce0: 724d 6573 7361 6765 426c 6f62 5265 6665  rMessageBlobRefe
+00006cf0: 7265 6e63 6528 676f 6f67 6c65 2e70 726f  rence(google.pro
+00006d00: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+00006d10: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
+00006d20: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+00006d30: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+00006d40: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
+00006d50: 2020 204b 4249 445f 4649 454c 445f 4e55     KBID_FIELD_NU
+00006d60: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00006d70: 6e74 0a20 2020 2055 5549 445f 4649 454c  nt.    UUID_FIEL
+00006d80: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00006d90: 6e73 2e69 6e74 0a20 2020 2053 544f 5241  ns.int.    STORA
+00006da0: 4745 5f4b 4559 5f46 4945 4c44 5f4e 554d  GE_KEY_FIELD_NUM
+00006db0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00006dc0: 740a 2020 2020 6b62 6964 3a20 6275 696c  t.    kbid: buil
+00006dd0: 7469 6e73 2e73 7472 0a20 2020 2075 7569  tins.str.    uui
+00006de0: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
+00006df0: 2020 2020 7374 6f72 6167 655f 6b65 793a      storage_key:
+00006e00: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
+00006e10: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00006e20: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00006e30: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+00006e40: 206b 6269 643a 2062 7569 6c74 696e 732e   kbid: builtins.
+00006e50: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+00006e60: 2020 2075 7569 643a 2062 7569 6c74 696e     uuid: builtin
+00006e70: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00006e80: 2020 2020 2073 746f 7261 6765 5f6b 6579       storage_key
+00006e90: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00006ea0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+00006eb0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+00006ec0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+00006ed0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00006ee0: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
+00006ef0: 6964 222c 2062 226b 6269 6422 2c20 2273  id", b"kbid", "s
+00006f00: 746f 7261 6765 5f6b 6579 222c 2062 2273  torage_key", b"s
+00006f10: 746f 7261 6765 5f6b 6579 222c 2022 7575  torage_key", "uu
+00006f20: 6964 222c 2062 2275 7569 6422 5d29 202d  id", b"uuid"]) -
+00006f30: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+00006f40: 6261 6c5f 5f5f 4272 6f6b 6572 4d65 7373  bal___BrokerMess
+00006f50: 6167 6542 6c6f 6252 6566 6572 656e 6365  ageBlobReference
+00006f60: 203d 2042 726f 6b65 724d 6573 7361 6765   = BrokerMessage
+00006f70: 426c 6f62 5265 6665 7265 6e63 650a 0a40  BlobReference..@
+00006f80: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
+00006f90: 7373 2057 7269 7465 7253 7461 7475 7352  ss WriterStatusR
+00006fa0: 6573 706f 6e73 6528 676f 6f67 6c65 2e70  esponse(google.p
+00006fb0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00006fc0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00006fd0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00006fe0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00006ff0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00007000: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+00007010: 616c 0a20 2020 2063 6c61 7373 204d 7367  al.    class Msg
+00007020: 6964 456e 7472 7928 676f 6f67 6c65 2e70  idEntry(google.p
+00007030: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00007040: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
+00007050: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00007060: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00007070: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+00007080: 746f 720a 0a20 2020 2020 2020 204b 4559  tor..        KEY
+00007090: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+000070a0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000070b0: 2020 2020 5641 4c55 455f 4649 454c 445f      VALUE_FIELD_
+000070c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+000070d0: 2e69 6e74 0a20 2020 2020 2020 206b 6579  .int.        key
+000070e0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+000070f0: 2020 2020 2020 2076 616c 7565 3a20 6275         value: bu
+00007100: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
+00007110: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00007120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007130: 662c 0a20 2020 2020 2020 2020 2020 202a  f,.            *
+00007140: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+00007150: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
+00007160: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2020  = ...,.         
+00007170: 2020 2076 616c 7565 3a20 6275 696c 7469     value: builti
+00007180: 6e73 2e69 6e74 203d 202e 2e2e 2c0a 2020  ns.int = ...,.  
+00007190: 2020 2020 2020 2920 2d3e 204e 6f6e 653a        ) -> None:
+000071a0: 202e 2e2e 0a20 2020 2020 2020 2064 6566   ....        def
+000071b0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+000071c0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+000071d0: 7069 6e67 2e4c 6974 6572 616c 5b22 6b65  ping.Literal["ke
+000071e0: 7922 2c20 6222 6b65 7922 2c20 2276 616c  y", b"key", "val
+000071f0: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
+00007200: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 2020  -> None: .....  
+00007210: 2020 4b4e 4f57 4c45 4447 4542 4f58 4553    KNOWLEDGEBOXES
+00007220: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00007230: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00007240: 4d53 4749 445f 4649 454c 445f 4e55 4d42  MSGID_FIELD_NUMB
+00007250: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00007260: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00007270: 2020 2064 6566 206b 6e6f 776c 6564 6765     def knowledge
+00007280: 626f 7865 7328 7365 6c66 2920 2d3e 2067  boxes(self) -> g
+00007290: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+000072a0: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
+000072b0: 7273 2e52 6570 6561 7465 6453 6361 6c61  rs.RepeatedScala
+000072c0: 7246 6965 6c64 436f 6e74 6169 6e65 725b  rFieldContainer[
+000072d0: 6275 696c 7469 6e73 2e73 7472 5d3a 202e  builtins.str]: .
+000072e0: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+000072f0: 0a20 2020 2064 6566 206d 7367 6964 2873  .    def msgid(s
+00007300: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
+00007310: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+00007320: 2e63 6f6e 7461 696e 6572 732e 5363 616c  .containers.Scal
+00007330: 6172 4d61 705b 6275 696c 7469 6e73 2e73  arMap[builtins.s
+00007340: 7472 2c20 6275 696c 7469 6e73 2e69 6e74  tr, builtins.int
+00007350: 5d3a 0a20 2020 2020 2020 2022 2222 6d61  ]:.        """ma
+00007360: 7020 6f66 206c 6173 7420 6d65 7373 6167  p of last messag
+00007370: 6520 7072 6f63 6573 7365 6422 2222 0a0a  e processed"""..
+00007380: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00007390: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000073a0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000073b0: 2020 206b 6e6f 776c 6564 6765 626f 7865     knowledgeboxe
+000073c0: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
+000073d0: 6263 2e49 7465 7261 626c 655b 6275 696c  bc.Iterable[buil
+000073e0: 7469 6e73 2e73 7472 5d20 7c20 4e6f 6e65  tins.str] | None
+000073f0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00007400: 6d73 6769 643a 2063 6f6c 6c65 6374 696f  msgid: collectio
+00007410: 6e73 2e61 6263 2e4d 6170 7069 6e67 5b62  ns.abc.Mapping[b
+00007420: 7569 6c74 696e 732e 7374 722c 2062 7569  uiltins.str, bui
+00007430: 6c74 696e 732e 696e 745d 207c 204e 6f6e  ltins.int] | Non
+00007440: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+00007450: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+00007460: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+00007470: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00007480: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00007490: 226b 6e6f 776c 6564 6765 626f 7865 7322  "knowledgeboxes"
+000074a0: 2c20 6222 6b6e 6f77 6c65 6467 6562 6f78  , b"knowledgebox
+000074b0: 6573 222c 2022 6d73 6769 6422 2c20 6222  es", "msgid", b"
+000074c0: 6d73 6769 6422 5d29 202d 3e20 4e6f 6e65  msgid"]) -> None
+000074d0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+000074e0: 5772 6974 6572 5374 6174 7573 5265 7370  WriterStatusResp
+000074f0: 6f6e 7365 203d 2057 7269 7465 7253 7461  onse = WriterSta
+00007500: 7475 7352 6573 706f 6e73 650a 0a40 7479  tusResponse..@ty
+00007510: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00007520: 2057 7269 7465 7253 7461 7475 7352 6571   WriterStatusReq
+00007530: 7565 7374 2867 6f6f 676c 652e 7072 6f74  uest(google.prot
+00007540: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+00007550: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+00007560: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00007570: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+00007580: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+00007590: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000075a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000075b0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+000075c0: 0a0a 676c 6f62 616c 5f5f 5f57 7269 7465  ..global___Write
+000075d0: 7253 7461 7475 7352 6571 7565 7374 203d  rStatusRequest =
+000075e0: 2057 7269 7465 7253 7461 7475 7352 6571   WriterStatusReq
+000075f0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+00007600: 6e61 6c0a 636c 6173 7320 5365 744c 6162  nal.class SetLab
+00007610: 656c 7352 6571 7565 7374 2867 6f6f 676c  elsRequest(googl
+00007620: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00007630: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00007640: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+00007650: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+00007660: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+00007670: 6f72 0a0a 2020 2020 4b42 5f46 4945 4c44  or..    KB_FIELD
+00007680: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00007690: 732e 696e 740a 2020 2020 4944 5f46 4945  s.int.    ID_FIE
+000076a0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000076b0: 696e 732e 696e 740a 2020 2020 4c41 4245  ins.int.    LABE
+000076c0: 4c53 4554 5f46 4945 4c44 5f4e 554d 4245  LSET_FIELD_NUMBE
+000076d0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+000076e0: 2020 2020 6964 3a20 6275 696c 7469 6e73      id: builtins
+000076f0: 2e73 7472 0a20 2020 2040 7072 6f70 6572  .str.    @proper
+00007700: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
+00007710: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+00007720: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+00007730: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+00007740: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
+00007750: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00007760: 6620 6c61 6265 6c73 6574 2873 656c 6629  f labelset(self)
+00007770: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+00007780: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+00007790: 5f70 6232 2e4c 6162 656c 5365 743a 202e  _pb2.LabelSet: .
+000077a0: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+000077b0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000077c0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
+000077d0: 2020 2020 2020 6b62 3a20 6e75 636c 6961        kb: nuclia
+000077e0: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
+000077f0: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
+00007800: 6564 6765 426f 7849 4420 7c20 4e6f 6e65  edgeBoxID | None
+00007810: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00007820: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
+00007830: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00007840: 6c61 6265 6c73 6574 3a20 6e75 636c 6961  labelset: nuclia
+00007850: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
+00007860: 6467 6562 6f78 5f70 6232 2e4c 6162 656c  dgebox_pb2.Label
+00007870: 5365 7420 7c20 4e6f 6e65 203d 202e 2e2e  Set | None = ...
+00007880: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00007890: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
+000078a0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+000078b0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+000078c0: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
+000078d0: 6222 2c20 226c 6162 656c 7365 7422 2c20  b", "labelset", 
+000078e0: 6222 6c61 6265 6c73 6574 225d 2920 2d3e  b"labelset"]) ->
+000078f0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+00007900: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00007910: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00007920: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00007930: 4c69 7465 7261 6c5b 2269 6422 2c20 6222  Literal["id", b"
+00007940: 6964 222c 2022 6b62 222c 2062 226b 6222  id", "kb", b"kb"
+00007950: 2c20 226c 6162 656c 7365 7422 2c20 6222  , "labelset", b"
+00007960: 6c61 6265 6c73 6574 225d 2920 2d3e 204e  labelset"]) -> N
+00007970: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
+00007980: 5f5f 5f53 6574 4c61 6265 6c73 5265 7175  ___SetLabelsRequ
+00007990: 6573 7420 3d20 5365 744c 6162 656c 7352  est = SetLabelsR
+000079a0: 6571 7565 7374 0a0a 4074 7970 696e 672e  equest..@typing.
+000079b0: 6669 6e61 6c0a 636c 6173 7320 4465 6c4c  final.class DelL
+000079c0: 6162 656c 7352 6571 7565 7374 2867 6f6f  abelsRequest(goo
+000079d0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+000079e0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+000079f0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00007a00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00007a10: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+00007a20: 7074 6f72 0a0a 2020 2020 4b42 5f46 4945  ptor..    KB_FIE
+00007a30: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00007a40: 696e 732e 696e 740a 2020 2020 4944 5f46  ins.int.    ID_F
+00007a50: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00007a60: 6c74 696e 732e 696e 740a 2020 2020 6964  ltins.int.    id
+00007a70: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00007a80: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007a90: 2064 6566 206b 6228 7365 6c66 2920 2d3e   def kb(self) ->
+00007aa0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00007ab0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+00007ac0: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
+00007ad0: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
+00007ae0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00007af0: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+00007b00: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
+00007b10: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+00007b20: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
+00007b30: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
+00007b40: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+00007b50: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
+00007b60: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2029  str = ...,.    )
+00007b70: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+00007b80: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
+00007b90: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00007ba0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00007bb0: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
+00007bc0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+00007bd0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00007be0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00007bf0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00007c00: 4c69 7465 7261 6c5b 2269 6422 2c20 6222  Literal["id", b"
+00007c10: 6964 222c 2022 6b62 222c 2062 226b 6222  id", "kb", b"kb"
+00007c20: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00007c30: 0a67 6c6f 6261 6c5f 5f5f 4465 6c4c 6162  .global___DelLab
+00007c40: 656c 7352 6571 7565 7374 203d 2044 656c  elsRequest = Del
+00007c50: 4c61 6265 6c73 5265 7175 6573 740a 0a40  LabelsRequest..@
+00007c60: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
+00007c70: 7373 2047 6574 4c61 6265 6c73 5265 7370  ss GetLabelsResp
+00007c80: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
+00007c90: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+00007ca0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+00007cb0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00007cc0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+00007cd0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+00007ce0: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
+00007cf0: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
+00007d00: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
+00007d10: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
+00007d20: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
+00007d30: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
+00007d40: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
+00007d50: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
+00007d60: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
+00007d70: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
+00007d80: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
+00007d90: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
+00007da0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
+00007db0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
+00007dc0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
+00007dd0: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
+00007de0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
+00007df0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
+00007e00: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00007e10: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00007e20: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
+00007e30: 746f 720a 2020 2020 2020 2020 4f4b 3a20  tor.        OK: 
+00007e40: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
+00007e50: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
+00007e60: 7970 6520 2023 2030 0a20 2020 2020 2020  ype  # 0.       
+00007e70: 204e 4f54 464f 554e 443a 2047 6574 4c61   NOTFOUND: GetLa
+00007e80: 6265 6c73 5265 7370 6f6e 7365 2e5f 5374  belsResponse._St
+00007e90: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+00007ea0: 2320 310a 0a20 2020 2063 6c61 7373 2053  # 1..    class S
+00007eb0: 7461 7475 7328 5f53 7461 7475 732c 206d  tatus(_Status, m
+00007ec0: 6574 6163 6c61 7373 3d5f 5374 6174 7573  etaclass=_Status
+00007ed0: 456e 756d 5479 7065 5772 6170 7065 7229  EnumTypeWrapper)
+00007ee0: 3a20 2e2e 2e0a 2020 2020 4f4b 3a20 4765  : ....    OK: Ge
+00007ef0: 744c 6162 656c 7352 6573 706f 6e73 652e  tLabelsResponse.
+00007f00: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+00007f10: 2020 2320 300a 2020 2020 4e4f 5446 4f55    # 0.    NOTFOU
+00007f20: 4e44 3a20 4765 744c 6162 656c 7352 6573  ND: GetLabelsRes
+00007f30: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+00007f40: 7565 5479 7065 2020 2320 310a 0a20 2020  ueType  # 1..   
+00007f50: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
+00007f60: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00007f70: 2020 204c 4142 454c 535f 4649 454c 445f     LABELS_FIELD_
+00007f80: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00007f90: 2e69 6e74 0a20 2020 2053 5441 5455 535f  .int.    STATUS_
+00007fa0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00007fb0: 696c 7469 6e73 2e69 6e74 0a20 2020 2073  iltins.int.    s
+00007fc0: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
+00007fd0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
+00007fe0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+00007ff0: 7065 0a20 2020 2040 7072 6f70 6572 7479  pe.    @property
+00008000: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
+00008010: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00008020: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+00008030: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
+00008040: 6f78 4944 3a20 2e2e 2e0a 2020 2020 4070  oxID: ....    @p
+00008050: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00008060: 6c61 6265 6c73 2873 656c 6629 202d 3e20  labels(self) -> 
+00008070: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00008080: 6b6e 6f77 6c65 6467 6562 6f78 5f70 6232  knowledgebox_pb2
+00008090: 2e4c 6162 656c 733a 202e 2e2e 0a20 2020  .Labels: ....   
+000080a0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000080b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000080c0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+000080d0: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
+000080e0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+000080f0: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
+00008100: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
+00008110: 2c0a 2020 2020 2020 2020 6c61 6265 6c73  ,.        labels
+00008120: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00008130: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+00008140: 6232 2e4c 6162 656c 7320 7c20 4e6f 6e65  b2.Labels | None
+00008150: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00008160: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
+00008170: 5f47 6574 4c61 6265 6c73 5265 7370 6f6e  _GetLabelsRespon
+00008180: 7365 2e53 7461 7475 732e 5661 6c75 6554  se.Status.ValueT
+00008190: 7970 6520 3d20 2e2e 2e2c 0a20 2020 2029  ype = ...,.    )
+000081a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+000081b0: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
+000081c0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+000081d0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+000081e0: 226b 6222 2c20 6222 6b62 222c 2022 6c61  "kb", b"kb", "la
+000081f0: 6265 6c73 222c 2062 226c 6162 656c 7322  bels", b"labels"
+00008200: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
+00008210: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
+00008220: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+00008230: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00008240: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
+00008250: 222c 2062 226b 6222 2c20 226c 6162 656c  ", b"kb", "label
+00008260: 7322 2c20 6222 6c61 6265 6c73 222c 2022  s", b"labels", "
+00008270: 7374 6174 7573 222c 2062 2273 7461 7475  status", b"statu
+00008280: 7322 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  s"]) -> None: ..
+00008290: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765 744c  ...global___GetL
+000082a0: 6162 656c 7352 6573 706f 6e73 6520 3d20  abelsResponse = 
+000082b0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
+000082c0: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
+000082d0: 0a63 6c61 7373 2047 6574 4c61 6265 6c73  .class GetLabels
+000082e0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
+000082f0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00008300: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00008310: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00008320: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00008330: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00008340: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
+00008350: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00008360: 6e74 0a20 2020 2040 7072 6f70 6572 7479  nt.    @property
+00008370: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
+00008380: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00008390: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+000083a0: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
+000083b0: 6f78 4944 3a20 2e2e 2e0a 2020 2020 6465  oxID: ....    de
+000083c0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000083d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000083e0: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
+000083f0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00008400: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+00008410: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
+00008420: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00008430: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+00008440: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
+00008450: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+00008460: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+00008470: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
+00008480: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+00008490: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
+000084a0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
+000084b0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+000084c0: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
+000084d0: 2c20 6222 6b62 225d 2920 2d3e 204e 6f6e  , b"kb"]) -> Non
+000084e0: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+000084f0: 5f47 6574 4c61 6265 6c73 5265 7175 6573  _GetLabelsReques
+00008500: 7420 3d20 4765 744c 6162 656c 7352 6571  t = GetLabelsReq
+00008510: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+00008520: 6e61 6c0a 636c 6173 7320 4e65 7745 6e74  nal.class NewEnt
+00008530: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
+00008540: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
+00008550: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+00008560: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+00008570: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+00008580: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+00008590: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
+000085a0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
+000085b0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000085c0: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
+000085d0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+000085e0: 740a 2020 2020 454e 5449 5449 4553 5f46  t.    ENTITIES_F
+000085f0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00008600: 6c74 696e 732e 696e 740a 2020 2020 6772  ltins.int.    gr
+00008610: 6f75 703a 2062 7569 6c74 696e 732e 7374  oup: builtins.st
+00008620: 720a 2020 2020 4070 726f 7065 7274 790a  r.    @property.
+00008630: 2020 2020 6465 6620 6b62 2873 656c 6629      def kb(self)
+00008640: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+00008650: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+00008660: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
+00008670: 7849 443a 202e 2e2e 0a20 2020 2040 7072  xID: ....    @pr
+00008680: 6f70 6572 7479 0a20 2020 2064 6566 2065  operty.    def e
+00008690: 6e74 6974 6965 7328 7365 6c66 2920 2d3e  ntities(self) ->
+000086a0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+000086b0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+000086c0: 322e 456e 7469 7469 6573 4772 6f75 703a  2.EntitiesGroup:
+000086d0: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
+000086e0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000086f0: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+00008700: 2020 2020 2020 2020 6b62 3a20 6e75 636c          kb: nucl
+00008710: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+00008720: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
+00008730: 776c 6564 6765 426f 7849 4420 7c20 4e6f  wledgeBoxID | No
+00008740: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00008750: 2020 6772 6f75 703a 2062 7569 6c74 696e    group: builtin
+00008760: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00008770: 2020 2020 2065 6e74 6974 6965 733a 206e       entities: n
+00008780: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+00008790: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+000087a0: 456e 7469 7469 6573 4772 6f75 7020 7c20  EntitiesGroup | 
+000087b0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+000087c0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+000087d0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
+000087e0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+000087f0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+00008800: 5b22 656e 7469 7469 6573 222c 2062 2265  ["entities", b"e
+00008810: 6e74 6974 6965 7322 2c20 226b 6222 2c20  ntities", "kb", 
+00008820: 6222 6b62 225d 2920 2d3e 2062 7569 6c74  b"kb"]) -> built
+00008830: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+00008840: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
+00008850: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+00008860: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+00008870: 6c5b 2265 6e74 6974 6965 7322 2c20 6222  l["entities", b"
+00008880: 656e 7469 7469 6573 222c 2022 6772 6f75  entities", "grou
+00008890: 7022 2c20 6222 6772 6f75 7022 2c20 226b  p", b"group", "k
+000088a0: 6222 2c20 6222 6b62 225d 2920 2d3e 204e  b", b"kb"]) -> N
+000088b0: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
+000088c0: 5f5f 5f4e 6577 456e 7469 7469 6573 4772  ___NewEntitiesGr
+000088d0: 6f75 7052 6571 7565 7374 203d 204e 6577  oupRequest = New
+000088e0: 456e 7469 7469 6573 4772 6f75 7052 6571  EntitiesGroupReq
+000088f0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+00008900: 6e61 6c0a 636c 6173 7320 4e65 7745 6e74  nal.class NewEnt
+00008910: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+00008920: 7365 2867 6f6f 676c 652e 7072 6f74 6f62  se(google.protob
+00008930: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+00008940: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+00008950: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+00008960: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+00008970: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+00008980: 636c 6173 7320 5f53 7461 7475 733a 0a20  class _Status:. 
+00008990: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
+000089a0: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
+000089b0: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
+000089c0: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
+000089d0: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
+000089e0: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
+000089f0: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
+00008a00: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
+00008a10: 7573 456e 756d 5479 7065 5772 6170 7065  usEnumTypeWrappe
+00008a20: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
+00008a30: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
+00008a40: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
+00008a50: 756d 5479 7065 5772 6170 7065 725b 4e65  umTypeWrapper[Ne
+00008a60: 7745 6e74 6974 6965 7347 726f 7570 5265  wEntitiesGroupRe
+00008a70: 7370 6f6e 7365 2e5f 5374 6174 7573 2e56  sponse._Status.V
+00008a80: 616c 7565 5479 7065 5d2c 2062 7569 6c74  alueType], built
+00008a90: 696e 732e 7479 7065 293a 0a20 2020 2020  ins.type):.     
+00008aa0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00008ab0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00008ac0: 6573 6372 6970 746f 722e 456e 756d 4465  escriptor.EnumDe
+00008ad0: 7363 7269 7074 6f72 0a20 2020 2020 2020  scriptor.       
+00008ae0: 204f 4b3a 204e 6577 456e 7469 7469 6573   OK: NewEntities
+00008af0: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
+00008b00: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+00008b10: 2023 2030 0a20 2020 2020 2020 2045 5252   # 0.        ERR
+00008b20: 4f52 3a20 4e65 7745 6e74 6974 6965 7347  OR: NewEntitiesG
+00008b30: 726f 7570 5265 7370 6f6e 7365 2e5f 5374  roupResponse._St
+00008b40: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+00008b50: 2320 310a 2020 2020 2020 2020 4b42 5f4e  # 1.        KB_N
+00008b60: 4f54 5f46 4f55 4e44 3a20 4e65 7745 6e74  OT_FOUND: NewEnt
+00008b70: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+00008b80: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+00008b90: 5479 7065 2020 2320 320a 2020 2020 2020  Type  # 2.      
+00008ba0: 2020 414c 5245 4144 595f 4558 4953 5453    ALREADY_EXISTS
+00008bb0: 3a20 4e65 7745 6e74 6974 6965 7347 726f  : NewEntitiesGro
+00008bc0: 7570 5265 7370 6f6e 7365 2e5f 5374 6174  upResponse._Stat
+00008bd0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+00008be0: 330a 0a20 2020 2063 6c61 7373 2053 7461  3..    class Sta
+00008bf0: 7475 7328 5f53 7461 7475 732c 206d 6574  tus(_Status, met
+00008c00: 6163 6c61 7373 3d5f 5374 6174 7573 456e  aclass=_StatusEn
+00008c10: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
+00008c20: 2e2e 2e0a 2020 2020 4f4b 3a20 4e65 7745  ....    OK: NewE
+00008c30: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
+00008c40: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+00008c50: 6554 7970 6520 2023 2030 0a20 2020 2045  eType  # 0.    E
+00008c60: 5252 4f52 3a20 4e65 7745 6e74 6974 6965  RROR: NewEntitie
+00008c70: 7347 726f 7570 5265 7370 6f6e 7365 2e53  sGroupResponse.S
+00008c80: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+00008c90: 2023 2031 0a20 2020 204b 425f 4e4f 545f   # 1.    KB_NOT_
+00008ca0: 464f 554e 443a 204e 6577 456e 7469 7469  FOUND: NewEntiti
+00008cb0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
+00008cc0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+00008cd0: 2020 2320 320a 2020 2020 414c 5245 4144    # 2.    ALREAD
+00008ce0: 595f 4558 4953 5453 3a20 4e65 7745 6e74  Y_EXISTS: NewEnt
+00008cf0: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+00008d00: 7365 2e53 7461 7475 732e 5661 6c75 6554  se.Status.ValueT
+00008d10: 7970 6520 2023 2033 0a0a 2020 2020 5354  ype  # 3..    ST
+00008d20: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
+00008d30: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00008d40: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+00008d50: 616c 5f5f 5f4e 6577 456e 7469 7469 6573  al___NewEntities
+00008d60: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
+00008d70: 6174 7573 2e56 616c 7565 5479 7065 0a20  atus.ValueType. 
+00008d80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00008d90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00008da0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00008db0: 2020 7374 6174 7573 3a20 676c 6f62 616c    status: global
+00008dc0: 5f5f 5f4e 6577 456e 7469 7469 6573 4772  ___NewEntitiesGr
+00008dd0: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
+00008de0: 7573 2e56 616c 7565 5479 7065 203d 202e  us.ValueType = .
+00008df0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
+00008e00: 653a 202e 2e2e 0a20 2020 2064 6566 2043  e: ....    def C
+00008e10: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+00008e20: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00008e30: 6e67 2e4c 6974 6572 616c 5b22 7374 6174  ng.Literal["stat
+00008e40: 7573 222c 2062 2273 7461 7475 7322 5d29  us", b"status"])
+00008e50: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+00008e60: 6c6f 6261 6c5f 5f5f 4e65 7745 6e74 6974  lobal___NewEntit
+00008e70: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+00008e80: 203d 204e 6577 456e 7469 7469 6573 4772   = NewEntitiesGr
+00008e90: 6f75 7052 6573 706f 6e73 650a 0a40 7479  oupResponse..@ty
+00008ea0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00008eb0: 2053 6574 456e 7469 7469 6573 5265 7175   SetEntitiesRequ
+00008ec0: 6573 7428 676f 6f67 6c65 2e70 726f 746f  est(google.proto
+00008ed0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
+00008ee0: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
+00008ef0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+00008f00: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+00008f10: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+00008f20: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
+00008f30: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00008f40: 2020 2047 524f 5550 5f46 4945 4c44 5f4e     GROUP_FIELD_N
+00008f50: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00008f60: 696e 740a 2020 2020 454e 5449 5449 4553  int.    ENTITIES
+00008f70: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00008f80: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00008f90: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
+00008fa0: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
+00008fb0: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
+00008fc0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
+00008fd0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+00008fe0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+00008ff0: 426f 7849 443a 202e 2e2e 0a20 2020 2040  BoxID: ....    @
+00009000: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00009010: 2065 6e74 6974 6965 7328 7365 6c66 2920   entities(self) 
+00009020: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+00009030: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+00009040: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
+00009050: 703a 202e 2e2e 0a20 2020 2064 6566 205f  p: ....    def _
+00009060: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00009070: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+00009080: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
+00009090: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+000090a0: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
+000090b0: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
+000090c0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+000090d0: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
+000090e0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+000090f0: 2020 2020 2020 2065 6e74 6974 6965 733a         entities:
+00009100: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00009110: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+00009120: 322e 456e 7469 7469 6573 4772 6f75 7020  2.EntitiesGroup 
+00009130: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00009140: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+00009150: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
+00009160: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+00009170: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+00009180: 616c 5b22 656e 7469 7469 6573 222c 2062  al["entities", b
+00009190: 2265 6e74 6974 6965 7322 2c20 226b 6222  "entities", "kb"
+000091a0: 2c20 6222 6b62 225d 2920 2d3e 2062 7569  , b"kb"]) -> bui
+000091b0: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
+000091c0: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
+000091d0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+000091e0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+000091f0: 7261 6c5b 2265 6e74 6974 6965 7322 2c20  ral["entities", 
+00009200: 6222 656e 7469 7469 6573 222c 2022 6772  b"entities", "gr
+00009210: 6f75 7022 2c20 6222 6772 6f75 7022 2c20  oup", b"group", 
+00009220: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
+00009230: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+00009240: 616c 5f5f 5f53 6574 456e 7469 7469 6573  al___SetEntities
+00009250: 5265 7175 6573 7420 3d20 5365 7445 6e74  Request = SetEnt
+00009260: 6974 6965 7352 6571 7565 7374 0a0a 4074  itiesRequest..@t
+00009270: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
+00009280: 7320 5570 6461 7465 456e 7469 7469 6573  s UpdateEntities
+00009290: 4772 6f75 7052 6571 7565 7374 2867 6f6f  GroupRequest(goo
+000092a0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+000092b0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+000092c0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+000092d0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+000092e0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+000092f0: 7074 6f72 0a0a 2020 2020 4074 7970 696e  ptor..    @typin
+00009300: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
+00009310: 7320 4164 6445 6e74 7279 2867 6f6f 676c  s AddEntry(googl
+00009320: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00009330: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00009340: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
+00009350: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00009360: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+00009370: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
+00009380: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+00009390: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+000093a0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
+000093b0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000093c0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+000093d0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+000093e0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
+000093f0: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
+00009400: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
+00009410: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+00009420: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+00009430: 456e 7469 7479 3a20 2e2e 2e0a 2020 2020  Entity: ....    
+00009440: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00009450: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00009460: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00009470: 2a2c 0a20 2020 2020 2020 2020 2020 206b  *,.            k
+00009480: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
+00009490: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+000094a0: 2020 2020 7661 6c75 653a 206e 7563 6c69      value: nucli
+000094b0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+000094c0: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+000094d0: 7479 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ty | None = ...,
+000094e0: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
+000094f0: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
+00009500: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+00009510: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00009520: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
+00009530: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
+00009540: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+00009550: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
+00009560: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+00009570: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00009580: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00009590: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
+000095a0: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
+000095b0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+000095c0: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+000095d0: 616c 0a20 2020 2063 6c61 7373 2055 7064  al.    class Upd
+000095e0: 6174 6545 6e74 7279 2867 6f6f 676c 652e  ateEntry(google.
+000095f0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+00009600: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
+00009610: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00009620: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00009630: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+00009640: 7074 6f72 0a0a 2020 2020 2020 2020 4b45  ptor..        KE
+00009650: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
+00009660: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00009670: 2020 2020 2056 414c 5545 5f46 4945 4c44       VALUE_FIELD
+00009680: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00009690: 732e 696e 740a 2020 2020 2020 2020 6b65  s.int.        ke
+000096a0: 793a 2062 7569 6c74 696e 732e 7374 720a  y: builtins.str.
+000096b0: 2020 2020 2020 2020 4070 726f 7065 7274          @propert
+000096c0: 790a 2020 2020 2020 2020 6465 6620 7661  y.        def va
+000096d0: 6c75 6528 7365 6c66 2920 2d3e 206e 7563  lue(self) -> nuc
+000096e0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+000096f0: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
+00009700: 7469 7479 3a20 2e2e 2e0a 2020 2020 2020  tity: ....      
+00009710: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00009720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009730: 2c0a 2020 2020 2020 2020 2020 2020 2a2c  ,.            *,
+00009740: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+00009750: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00009760: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00009770: 2020 7661 6c75 653a 206e 7563 6c69 6164    value: nucliad
+00009780: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+00009790: 6765 626f 785f 7062 322e 456e 7469 7479  gebox_pb2.Entity
+000097a0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+000097b0: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
+000097c0: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+000097d0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+000097e0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+000097f0: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
+00009800: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
+00009810: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+00009820: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+00009830: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
+00009840: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00009850: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+00009860: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
+00009870: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
+00009880: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
+00009890: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
+000098a0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+000098b0: 0a20 2020 2047 524f 5550 5f46 4945 4c44  .    GROUP_FIELD
+000098c0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+000098d0: 732e 696e 740a 2020 2020 4144 445f 4649  s.int.    ADD_FI
+000098e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000098f0: 7469 6e73 2e69 6e74 0a20 2020 2055 5044  tins.int.    UPD
+00009900: 4154 455f 4649 454c 445f 4e55 4d42 4552  ATE_FIELD_NUMBER
+00009910: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00009920: 2020 2044 454c 4554 455f 4649 454c 445f     DELETE_FIELD_
+00009930: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00009940: 2e69 6e74 0a20 2020 2054 4954 4c45 5f46  .int.    TITLE_F
+00009950: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00009960: 6c74 696e 732e 696e 740a 2020 2020 434f  ltins.int.    CO
+00009970: 4c4f 525f 4649 454c 445f 4e55 4d42 4552  LOR_FIELD_NUMBER
+00009980: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00009990: 2020 2067 726f 7570 3a20 6275 696c 7469     group: builti
+000099a0: 6e73 2e73 7472 0a20 2020 2074 6974 6c65  ns.str.    title
+000099b0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+000099c0: 2020 2063 6f6c 6f72 3a20 6275 696c 7469     color: builti
+000099d0: 6e73 2e73 7472 0a20 2020 2040 7072 6f70  ns.str.    @prop
+000099e0: 6572 7479 0a20 2020 2064 6566 206b 6228  erty.    def kb(
+000099f0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+00009a00: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+00009a10: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
+00009a20: 6467 6542 6f78 4944 3a20 2e2e 2e0a 2020  dgeBoxID: ....  
+00009a30: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00009a40: 6465 6620 6164 6428 7365 6c66 2920 2d3e  def add(self) ->
+00009a50: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00009a60: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
+00009a70: 6e65 7273 2e4d 6573 7361 6765 4d61 705b  ners.MessageMap[
+00009a80: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
+00009a90: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+00009aa0: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
+00009ab0: 6e74 6974 795d 3a0a 2020 2020 2020 2020  ntity]:.        
+00009ac0: 2222 2265 6e74 6974 795f 6964 3a20 456e  """entity_id: En
+00009ad0: 7469 7479 2222 220a 0a20 2020 2040 7072  tity"""..    @pr
+00009ae0: 6f70 6572 7479 0a20 2020 2064 6566 2075  operty.    def u
+00009af0: 7064 6174 6528 7365 6c66 2920 2d3e 2067  pdate(self) -> g
+00009b00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+00009b10: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
+00009b20: 7273 2e4d 6573 7361 6765 4d61 705b 6275  rs.MessageMap[bu
+00009b30: 696c 7469 6e73 2e73 7472 2c20 6e75 636c  iltins.str, nucl
+00009b40: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+00009b50: 6c65 6467 6562 6f78 5f70 6232 2e45 6e74  ledgebox_pb2.Ent
+00009b60: 6974 795d 3a0a 2020 2020 2020 2020 2222  ity]:.        ""
+00009b70: 2265 6e74 6974 795f 6964 3a20 456e 7469  "entity_id: Enti
+00009b80: 7479 2222 220a 0a20 2020 2040 7072 6f70  ty"""..    @prop
+00009b90: 6572 7479 0a20 2020 2064 6566 2064 656c  erty.    def del
+00009ba0: 6574 6528 7365 6c66 2920 2d3e 2067 6f6f  ete(self) -> goo
+00009bb0: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+00009bc0: 6572 6e61 6c2e 636f 6e74 6169 6e65 7273  ernal.containers
+00009bd0: 2e52 6570 6561 7465 6453 6361 6c61 7246  .RepeatedScalarF
+00009be0: 6965 6c64 436f 6e74 6169 6e65 725b 6275  ieldContainer[bu
+00009bf0: 696c 7469 6e73 2e73 7472 5d3a 0a20 2020  iltins.str]:.   
+00009c00: 2020 2020 2022 2222 656e 7469 7479 5f69       """entity_i
+00009c10: 6422 2222 0a0a 2020 2020 6465 6620 5f5f  d"""..    def __
+00009c20: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00009c30: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+00009c40: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
+00009c50: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+00009c60: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
+00009c70: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
+00009c80: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+00009c90: 2020 2067 726f 7570 3a20 6275 696c 7469     group: builti
+00009ca0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00009cb0: 2020 2020 2020 6164 643a 2063 6f6c 6c65        add: colle
+00009cc0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+00009cd0: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+00009ce0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00009cf0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+00009d00: 322e 456e 7469 7479 5d20 7c20 4e6f 6e65  2.Entity] | None
+00009d10: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00009d20: 7570 6461 7465 3a20 636f 6c6c 6563 7469  update: collecti
+00009d30: 6f6e 732e 6162 632e 4d61 7070 696e 675b  ons.abc.Mapping[
+00009d40: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
+00009d50: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+00009d60: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
+00009d70: 6e74 6974 795d 207c 204e 6f6e 6520 3d20  ntity] | None = 
+00009d80: 2e2e 2e2c 0a20 2020 2020 2020 2064 656c  ...,.        del
+00009d90: 6574 653a 2063 6f6c 6c65 6374 696f 6e73  ete: collections
+00009da0: 2e61 6263 2e49 7465 7261 626c 655b 6275  .abc.Iterable[bu
+00009db0: 696c 7469 6e73 2e73 7472 5d20 7c20 4e6f  iltins.str] | No
+00009dc0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00009dd0: 2020 7469 746c 653a 2062 7569 6c74 696e    title: builtin
+00009de0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00009df0: 2020 2020 2063 6f6c 6f72 3a20 6275 696c       color: buil
+00009e00: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+00009e10: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+00009e20: 2e2e 0a20 2020 2064 6566 2048 6173 4669  ...    def HasFi
+00009e30: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
+00009e40: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
+00009e50: 6572 616c 5b22 6b62 222c 2062 226b 6222  eral["kb", b"kb"
+00009e60: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
+00009e70: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
+00009e80: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+00009e90: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00009ea0: 7069 6e67 2e4c 6974 6572 616c 5b22 6164  ping.Literal["ad
+00009eb0: 6422 2c20 6222 6164 6422 2c20 2263 6f6c  d", b"add", "col
+00009ec0: 6f72 222c 2062 2263 6f6c 6f72 222c 2022  or", b"color", "
+00009ed0: 6465 6c65 7465 222c 2062 2264 656c 6574  delete", b"delet
+00009ee0: 6522 2c20 2267 726f 7570 222c 2062 2267  e", "group", b"g
+00009ef0: 726f 7570 222c 2022 6b62 222c 2062 226b  roup", "kb", b"k
+00009f00: 6222 2c20 2274 6974 6c65 222c 2062 2274  b", "title", b"t
+00009f10: 6974 6c65 222c 2022 7570 6461 7465 222c  itle", "update",
+00009f20: 2062 2275 7064 6174 6522 5d29 202d 3e20   b"update"]) -> 
+00009f30: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
+00009f40: 6c5f 5f5f 5570 6461 7465 456e 7469 7469  l___UpdateEntiti
+00009f50: 6573 4772 6f75 7052 6571 7565 7374 203d  esGroupRequest =
+00009f60: 2055 7064 6174 6545 6e74 6974 6965 7347   UpdateEntitiesG
+00009f70: 726f 7570 5265 7175 6573 740a 0a40 7479  roupRequest..@ty
+00009f80: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00009f90: 2055 7064 6174 6545 6e74 6974 6965 7347   UpdateEntitiesG
+00009fa0: 726f 7570 5265 7370 6f6e 7365 2867 6f6f  roupResponse(goo
+00009fb0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+00009fc0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+00009fd0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00009fe0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00009ff0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+0000a000: 7074 6f72 0a0a 2020 2020 636c 6173 7320  ptor..    class 
+0000a010: 5f53 7461 7475 733a 0a20 2020 2020 2020  _Status:.       
+0000a020: 2056 616c 7565 5479 7065 203d 2074 7970   ValueType = typ
+0000a030: 696e 672e 4e65 7754 7970 6528 2256 616c  ing.NewType("Val
+0000a040: 7565 5479 7065 222c 2062 7569 6c74 696e  ueType", builtin
+0000a050: 732e 696e 7429 0a20 2020 2020 2020 2056  s.int).        V
+0000a060: 3a20 7479 7069 6e67 5f65 7874 656e 7369  : typing_extensi
+0000a070: 6f6e 732e 5479 7065 416c 6961 7320 3d20  ons.TypeAlias = 
+0000a080: 5661 6c75 6554 7970 650a 0a20 2020 2063  ValueType..    c
+0000a090: 6c61 7373 205f 5374 6174 7573 456e 756d  lass _StatusEnum
+0000a0a0: 5479 7065 5772 6170 7065 7228 676f 6f67  TypeWrapper(goog
+0000a0b0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+0000a0c0: 726e 616c 2e65 6e75 6d5f 7479 7065 5f77  rnal.enum_type_w
+0000a0d0: 7261 7070 6572 2e5f 456e 756d 5479 7065  rapper._EnumType
+0000a0e0: 5772 6170 7065 725b 5570 6461 7465 456e  Wrapper[UpdateEn
+0000a0f0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+0000a100: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+0000a110: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
+0000a120: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
+0000a130: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+0000a140: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+0000a150: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
+0000a160: 6970 746f 720a 2020 2020 2020 2020 4f4b  iptor.        OK
+0000a170: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
+0000a180: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
+0000a190: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000a1a0: 2023 2030 0a20 2020 2020 2020 2045 5252   # 0.        ERR
+0000a1b0: 4f52 3a20 5570 6461 7465 456e 7469 7469  OR: UpdateEntiti
+0000a1c0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
+0000a1d0: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
+0000a1e0: 6520 2023 2031 0a20 2020 2020 2020 204b  e  # 1.        K
+0000a1f0: 425f 4e4f 545f 464f 554e 443a 2055 7064  B_NOT_FOUND: Upd
+0000a200: 6174 6545 6e74 6974 6965 7347 726f 7570  ateEntitiesGroup
+0000a210: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+0000a220: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+0000a230: 2020 2020 2020 2020 454e 5449 5449 4553          ENTITIES
+0000a240: 5f47 524f 5550 5f4e 4f54 5f46 4f55 4e44  _GROUP_NOT_FOUND
+0000a250: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
+0000a260: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
+0000a270: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000a280: 2023 2033 0a0a 2020 2020 636c 6173 7320   # 3..    class 
+0000a290: 5374 6174 7573 285f 5374 6174 7573 2c20  Status(_Status, 
+0000a2a0: 6d65 7461 636c 6173 733d 5f53 7461 7475  metaclass=_Statu
+0000a2b0: 7345 6e75 6d54 7970 6557 7261 7070 6572  sEnumTypeWrapper
+0000a2c0: 293a 202e 2e2e 0a20 2020 204f 4b3a 2055  ): ....    OK: U
+0000a2d0: 7064 6174 6545 6e74 6974 6965 7347 726f  pdateEntitiesGro
+0000a2e0: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
+0000a2f0: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
+0000a300: 0a20 2020 2045 5252 4f52 3a20 5570 6461  .    ERROR: Upda
+0000a310: 7465 456e 7469 7469 6573 4772 6f75 7052  teEntitiesGroupR
+0000a320: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
+0000a330: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
+0000a340: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
+0000a350: 5570 6461 7465 456e 7469 7469 6573 4772  UpdateEntitiesGr
+0000a360: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
+0000a370: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000a380: 320a 2020 2020 454e 5449 5449 4553 5f47  2.    ENTITIES_G
+0000a390: 524f 5550 5f4e 4f54 5f46 4f55 4e44 3a20  ROUP_NOT_FOUND: 
+0000a3a0: 5570 6461 7465 456e 7469 7469 6573 4772  UpdateEntitiesGr
+0000a3b0: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
+0000a3c0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000a3d0: 330a 0a20 2020 2053 5441 5455 535f 4649  3..    STATUS_FI
+0000a3e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+0000a3f0: 7469 6e73 2e69 6e74 0a20 2020 2073 7461  tins.int.    sta
+0000a400: 7475 733a 2067 6c6f 6261 6c5f 5f5f 5570  tus: global___Up
+0000a410: 6461 7465 456e 7469 7469 6573 4772 6f75  dateEntitiesGrou
+0000a420: 7052 6573 706f 6e73 652e 5374 6174 7573  pResponse.Status
+0000a430: 2e56 616c 7565 5479 7065 0a20 2020 2064  .ValueType.    d
+0000a440: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0000a450: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000a460: 2020 202a 2c0a 2020 2020 2020 2020 7374     *,.        st
+0000a470: 6174 7573 3a20 676c 6f62 616c 5f5f 5f55  atus: global___U
+0000a480: 7064 6174 6545 6e74 6974 6965 7347 726f  pdateEntitiesGro
+0000a490: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
+0000a4a0: 732e 5661 6c75 6554 7970 6520 3d20 2e2e  s.ValueType = ..
+0000a4b0: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+0000a4c0: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+0000a4d0: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+0000a4e0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+0000a4f0: 672e 4c69 7465 7261 6c5b 2273 7461 7475  g.Literal["statu
+0000a500: 7322 2c20 6222 7374 6174 7573 225d 2920  s", b"status"]) 
+0000a510: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
+0000a520: 6f62 616c 5f5f 5f55 7064 6174 6545 6e74  obal___UpdateEnt
+0000a530: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+0000a540: 7365 203d 2055 7064 6174 6545 6e74 6974  se = UpdateEntit
+0000a550: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+0000a560: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
+0000a570: 636c 6173 7320 4c69 7374 456e 7469 7469  class ListEntiti
+0000a580: 6573 4772 6f75 7073 5265 7175 6573 7428  esGroupsRequest(
+0000a590: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000a5a0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+0000a5b0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+0000a5c0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+0000a5d0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+0000a5e0: 6372 6970 746f 720a 0a20 2020 204b 425f  criptor..    KB_
+0000a5f0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000a600: 696c 7469 6e73 2e69 6e74 0a20 2020 2040  iltins.int.    @
+0000a610: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000a620: 206b 6228 7365 6c66 2920 2d3e 206e 7563   kb(self) -> nuc
+0000a630: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+0000a640: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
+0000a650: 6f77 6c65 6467 6542 6f78 4944 3a20 2e2e  owledgeBoxID: ..
+0000a660: 2e0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+0000a670: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0000a680: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+0000a690: 2020 2020 206b 623a 206e 7563 6c69 6164       kb: nucliad
+0000a6a0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+0000a6b0: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
+0000a6c0: 6467 6542 6f78 4944 207c 204e 6f6e 6520  dgeBoxID | None 
+0000a6d0: 3d20 2e2e 2e2c 0a20 2020 2029 202d 3e20  = ...,.    ) -> 
+0000a6e0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000a6f0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+0000a700: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000a710: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
+0000a720: 2c20 6222 6b62 225d 2920 2d3e 2062 7569  , b"kb"]) -> bui
+0000a730: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
+0000a740: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
+0000a750: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+0000a760: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+0000a770: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
+0000a780: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
+0000a790: 676c 6f62 616c 5f5f 5f4c 6973 7445 6e74  global___ListEnt
+0000a7a0: 6974 6965 7347 726f 7570 7352 6571 7565  itiesGroupsReque
+0000a7b0: 7374 203d 204c 6973 7445 6e74 6974 6965  st = ListEntitie
+0000a7c0: 7347 726f 7570 7352 6571 7565 7374 0a0a  sGroupsRequest..
+0000a7d0: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
+0000a7e0: 6173 7320 4c69 7374 456e 7469 7469 6573  ass ListEntities
+0000a7f0: 4772 6f75 7073 5265 7370 6f6e 7365 2867  GroupsResponse(g
+0000a800: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
+0000a810: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
+0000a820: 0a20 2020 2044 4553 4352 4950 544f 523a  .    DESCRIPTOR:
+0000a830: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+0000a840: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+0000a850: 7269 7074 6f72 0a0a 2020 2020 636c 6173  riptor..    clas
+0000a860: 7320 5f53 7461 7475 733a 0a20 2020 2020  s _Status:.     
+0000a870: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
+0000a880: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
+0000a890: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
+0000a8a0: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
+0000a8b0: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
+0000a8c0: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
+0000a8d0: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
+0000a8e0: 2063 6c61 7373 205f 5374 6174 7573 456e   class _StatusEn
+0000a8f0: 756d 5479 7065 5772 6170 7065 7228 676f  umTypeWrapper(go
+0000a900: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+0000a910: 7465 726e 616c 2e65 6e75 6d5f 7479 7065  ternal.enum_type
+0000a920: 5f77 7261 7070 6572 2e5f 456e 756d 5479  _wrapper._EnumTy
+0000a930: 7065 5772 6170 7065 725b 4c69 7374 456e  peWrapper[ListEn
+0000a940: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
+0000a950: 6f6e 7365 2e5f 5374 6174 7573 2e56 616c  onse._Status.Val
+0000a960: 7565 5479 7065 5d2c 2062 7569 6c74 696e  ueType], builtin
+0000a970: 732e 7479 7065 293a 0a20 2020 2020 2020  s.type):.       
+0000a980: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+0000a990: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+0000a9a0: 6372 6970 746f 722e 456e 756d 4465 7363  criptor.EnumDesc
+0000a9b0: 7269 7074 6f72 0a20 2020 2020 2020 204f  riptor.        O
+0000a9c0: 4b3a 204c 6973 7445 6e74 6974 6965 7347  K: ListEntitiesG
+0000a9d0: 726f 7570 7352 6573 706f 6e73 652e 5f53  roupsResponse._S
+0000a9e0: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000a9f0: 2023 2030 0a20 2020 2020 2020 204e 4f54   # 0.        NOT
+0000aa00: 464f 554e 443a 204c 6973 7445 6e74 6974  FOUND: ListEntit
+0000aa10: 6965 7347 726f 7570 7352 6573 706f 6e73  iesGroupsRespons
+0000aa20: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
+0000aa30: 7970 6520 2023 2031 0a20 2020 2020 2020  ype  # 1.       
+0000aa40: 2045 5252 4f52 3a20 4c69 7374 456e 7469   ERROR: ListEnti
+0000aa50: 7469 6573 4772 6f75 7073 5265 7370 6f6e  tiesGroupsRespon
+0000aa60: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+0000aa70: 5479 7065 2020 2320 320a 0a20 2020 2063  Type  # 2..    c
+0000aa80: 6c61 7373 2053 7461 7475 7328 5f53 7461  lass Status(_Sta
+0000aa90: 7475 732c 206d 6574 6163 6c61 7373 3d5f  tus, metaclass=_
+0000aaa0: 5374 6174 7573 456e 756d 5479 7065 5772  StatusEnumTypeWr
+0000aab0: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
+0000aac0: 4f4b 3a20 4c69 7374 456e 7469 7469 6573  OK: ListEntities
+0000aad0: 4772 6f75 7073 5265 7370 6f6e 7365 2e53  GroupsResponse.S
+0000aae0: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000aaf0: 2023 2030 0a20 2020 204e 4f54 464f 554e   # 0.    NOTFOUN
+0000ab00: 443a 204c 6973 7445 6e74 6974 6965 7347  D: ListEntitiesG
+0000ab10: 726f 7570 7352 6573 706f 6e73 652e 5374  roupsResponse.St
+0000ab20: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+0000ab30: 2320 310a 2020 2020 4552 524f 523a 204c  # 1.    ERROR: L
+0000ab40: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
+0000ab50: 7352 6573 706f 6e73 652e 5374 6174 7573  sResponse.Status
+0000ab60: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+0000ab70: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+0000ab80: 616c 0a20 2020 2063 6c61 7373 2047 726f  al.    class Gro
+0000ab90: 7570 7345 6e74 7279 2867 6f6f 676c 652e  upsEntry(google.
+0000aba0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+0000abb0: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
+0000abc0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+0000abd0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+0000abe0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+0000abf0: 7074 6f72 0a0a 2020 2020 2020 2020 4b45  ptor..        KE
+0000ac00: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
+0000ac10: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000ac20: 2020 2020 2056 414c 5545 5f46 4945 4c44       VALUE_FIELD
+0000ac30: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+0000ac40: 732e 696e 740a 2020 2020 2020 2020 6b65  s.int.        ke
+0000ac50: 793a 2062 7569 6c74 696e 732e 7374 720a  y: builtins.str.
+0000ac60: 2020 2020 2020 2020 4070 726f 7065 7274          @propert
+0000ac70: 790a 2020 2020 2020 2020 6465 6620 7661  y.        def va
+0000ac80: 6c75 6528 7365 6c66 2920 2d3e 206e 7563  lue(self) -> nuc
+0000ac90: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+0000aca0: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
+0000acb0: 7469 7469 6573 4772 6f75 7053 756d 6d61  titiesGroupSumma
+0000acc0: 7279 3a20 2e2e 2e0a 2020 2020 2020 2020  ry: ....        
+0000acd0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000ace0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+0000acf0: 2020 2020 2020 2020 2020 2020 2a2c 0a20              *,. 
+0000ad00: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
+0000ad10: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+0000ad20: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+0000ad30: 7661 6c75 653a 206e 7563 6c69 6164 625f  value: nucliadb_
+0000ad40: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000ad50: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
+0000ad60: 4772 6f75 7053 756d 6d61 7279 207c 204e  GroupSummary | N
+0000ad70: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+0000ad80: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+0000ad90: 2e0a 2020 2020 2020 2020 6465 6620 4861  ..        def Ha
+0000ada0: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
+0000adb0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000adc0: 4c69 7465 7261 6c5b 2276 616c 7565 222c  Literal["value",
+0000add0: 2062 2276 616c 7565 225d 2920 2d3e 2062   b"value"]) -> b
+0000ade0: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+0000adf0: 2e0a 2020 2020 2020 2020 6465 6620 436c  ..        def Cl
+0000ae00: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+0000ae10: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+0000ae20: 672e 4c69 7465 7261 6c5b 226b 6579 222c  g.Literal["key",
+0000ae30: 2062 226b 6579 222c 2022 7661 6c75 6522   b"key", "value"
+0000ae40: 2c20 6222 7661 6c75 6522 5d29 202d 3e20  , b"value"]) -> 
+0000ae50: 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020 2047  None: .....    G
+0000ae60: 524f 5550 535f 4649 454c 445f 4e55 4d42  ROUPS_FIELD_NUMB
+0000ae70: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000ae80: 0a20 2020 2053 5441 5455 535f 4649 454c  .    STATUS_FIEL
+0000ae90: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000aea0: 6e73 2e69 6e74 0a20 2020 2073 7461 7475  ns.int.    statu
+0000aeb0: 733a 2067 6c6f 6261 6c5f 5f5f 4c69 7374  s: global___List
+0000aec0: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
+0000aed0: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
+0000aee0: 6c75 6554 7970 650a 2020 2020 4070 726f  lueType.    @pro
+0000aef0: 7065 7274 790a 2020 2020 6465 6620 6772  perty.    def gr
+0000af00: 6f75 7073 2873 656c 6629 202d 3e20 676f  oups(self) -> go
+0000af10: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+0000af20: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+0000af30: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
+0000af40: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+0000af50: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000af60: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+0000af70: 7469 6573 4772 6f75 7053 756d 6d61 7279  tiesGroupSummary
+0000af80: 5d3a 202e 2e2e 0a20 2020 2064 6566 205f  ]: ....    def _
+0000af90: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000afa0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0000afb0: 2c0a 2020 2020 2020 2020 6772 6f75 7073  ,.        groups
+0000afc0: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
+0000afd0: 632e 4d61 7070 696e 675b 6275 696c 7469  c.Mapping[builti
+0000afe0: 6e73 2e73 7472 2c20 6e75 636c 6961 6462  ns.str, nucliadb
+0000aff0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
+0000b000: 6562 6f78 5f70 6232 2e45 6e74 6974 6965  ebox_pb2.Entitie
+0000b010: 7347 726f 7570 5375 6d6d 6172 795d 207c  sGroupSummary] |
+0000b020: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+0000b030: 2020 2020 2073 7461 7475 733a 2067 6c6f       status: glo
+0000b040: 6261 6c5f 5f5f 4c69 7374 456e 7469 7469  bal___ListEntiti
+0000b050: 6573 4772 6f75 7073 5265 7370 6f6e 7365  esGroupsResponse
+0000b060: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+0000b070: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+0000b080: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+0000b090: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+0000b0a0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000b0b0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000b0c0: 2267 726f 7570 7322 2c20 6222 6772 6f75  "groups", b"grou
+0000b0d0: 7073 222c 2022 7374 6174 7573 222c 2062  ps", "status", b
+0000b0e0: 2273 7461 7475 7322 5d29 202d 3e20 4e6f  "status"]) -> No
+0000b0f0: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
+0000b100: 5f5f 4c69 7374 456e 7469 7469 6573 4772  __ListEntitiesGr
+0000b110: 6f75 7073 5265 7370 6f6e 7365 203d 204c  oupsResponse = L
+0000b120: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
+0000b130: 7352 6573 706f 6e73 650a 0a40 7479 7069  sResponse..@typi
+0000b140: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
+0000b150: 6574 456e 7469 7469 6573 5265 7175 6573  etEntitiesReques
+0000b160: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
+0000b170: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+0000b180: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+0000b190: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000b1a0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000b1b0: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
+0000b1c0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
+0000b1d0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000b1e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000b1f0: 6566 206b 6228 7365 6c66 2920 2d3e 206e  ef kb(self) -> n
+0000b200: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+0000b210: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+0000b220: 4b6e 6f77 6c65 6467 6542 6f78 4944 3a20  KnowledgeBoxID: 
+0000b230: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+0000b240: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0000b250: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
+0000b260: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
+0000b270: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000b280: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
+0000b290: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
+0000b2a0: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+0000b2b0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+0000b2c0: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+0000b2d0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+0000b2e0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+0000b2f0: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
+0000b300: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+0000b310: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+0000b320: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000b330: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000b340: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
+0000b350: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
+0000b360: 0a0a 676c 6f62 616c 5f5f 5f47 6574 456e  ..global___GetEn
+0000b370: 7469 7469 6573 5265 7175 6573 7420 3d20  titiesRequest = 
+0000b380: 4765 7445 6e74 6974 6965 7352 6571 7565  GetEntitiesReque
+0000b390: 7374 0a0a 4074 7970 696e 672e 6669 6e61  st..@typing.fina
+0000b3a0: 6c0a 636c 6173 7320 4765 7445 6e74 6974  l.class GetEntit
+0000b3b0: 6965 7352 6573 706f 6e73 6528 676f 6f67  iesResponse(goog
+0000b3c0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+0000b3d0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+0000b3e0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000b3f0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000b400: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000b410: 746f 720a 0a20 2020 2063 6c61 7373 205f  tor..    class _
+0000b420: 5374 6174 7573 3a0a 2020 2020 2020 2020  Status:.        
+0000b430: 5661 6c75 6554 7970 6520 3d20 7479 7069  ValueType = typi
+0000b440: 6e67 2e4e 6577 5479 7065 2822 5661 6c75  ng.NewType("Valu
+0000b450: 6554 7970 6522 2c20 6275 696c 7469 6e73  eType", builtins
+0000b460: 2e69 6e74 290a 2020 2020 2020 2020 563a  .int).        V:
+0000b470: 2074 7970 696e 675f 6578 7465 6e73 696f   typing_extensio
+0000b480: 6e73 2e54 7970 6541 6c69 6173 203d 2056  ns.TypeAlias = V
+0000b490: 616c 7565 5479 7065 0a0a 2020 2020 636c  alueType..    cl
+0000b4a0: 6173 7320 5f53 7461 7475 7345 6e75 6d54  ass _StatusEnumT
+0000b4b0: 7970 6557 7261 7070 6572 2867 6f6f 676c  ypeWrapper(googl
+0000b4c0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+0000b4d0: 6e61 6c2e 656e 756d 5f74 7970 655f 7772  nal.enum_type_wr
+0000b4e0: 6170 7065 722e 5f45 6e75 6d54 7970 6557  apper._EnumTypeW
+0000b4f0: 7261 7070 6572 5b47 6574 456e 7469 7469  rapper[GetEntiti
+0000b500: 6573 5265 7370 6f6e 7365 2e5f 5374 6174  esResponse._Stat
+0000b510: 7573 2e56 616c 7565 5479 7065 5d2c 2062  us.ValueType], b
+0000b520: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
+0000b530: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
+0000b540: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
+0000b550: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
+0000b560: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
+0000b570: 2020 2020 204f 4b3a 2047 6574 456e 7469       OK: GetEnti
+0000b580: 7469 6573 5265 7370 6f6e 7365 2e5f 5374  tiesResponse._St
+0000b590: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+0000b5a0: 2320 300a 2020 2020 2020 2020 4e4f 5446  # 0.        NOTF
+0000b5b0: 4f55 4e44 3a20 4765 7445 6e74 6974 6965  OUND: GetEntitie
+0000b5c0: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
+0000b5d0: 732e 5661 6c75 6554 7970 6520 2023 2031  s.ValueType  # 1
+0000b5e0: 0a20 2020 2020 2020 2045 5252 4f52 3a20  .        ERROR: 
+0000b5f0: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
+0000b600: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+0000b610: 6554 7970 6520 2023 2032 0a0a 2020 2020  eType  # 2..    
+0000b620: 636c 6173 7320 5374 6174 7573 285f 5374  class Status(_St
+0000b630: 6174 7573 2c20 6d65 7461 636c 6173 733d  atus, metaclass=
+0000b640: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
+0000b650: 7261 7070 6572 293a 202e 2e2e 0a20 2020  rapper): ....   
+0000b660: 204f 4b3a 2047 6574 456e 7469 7469 6573   OK: GetEntities
+0000b670: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
+0000b680: 5661 6c75 6554 7970 6520 2023 2030 0a20  ValueType  # 0. 
+0000b690: 2020 204e 4f54 464f 554e 443a 2047 6574     NOTFOUND: Get
+0000b6a0: 456e 7469 7469 6573 5265 7370 6f6e 7365  EntitiesResponse
+0000b6b0: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+0000b6c0: 6520 2023 2031 0a20 2020 2045 5252 4f52  e  # 1.    ERROR
+0000b6d0: 3a20 4765 7445 6e74 6974 6965 7352 6573  : GetEntitiesRes
+0000b6e0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000b6f0: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
+0000b700: 2040 7479 7069 6e67 2e66 696e 616c 0a20   @typing.final. 
+0000b710: 2020 2063 6c61 7373 2047 726f 7570 7345     class GroupsE
+0000b720: 6e74 7279 2867 6f6f 676c 652e 7072 6f74  ntry(google.prot
+0000b730: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+0000b740: 7361 6765 293a 0a20 2020 2020 2020 2044  sage):.        D
+0000b750: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+0000b760: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+0000b770: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+0000b780: 0a0a 2020 2020 2020 2020 4b45 595f 4649  ..        KEY_FI
+0000b790: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+0000b7a0: 7469 6e73 2e69 6e74 0a20 2020 2020 2020  tins.int.       
+0000b7b0: 2056 414c 5545 5f46 4945 4c44 5f4e 554d   VALUE_FIELD_NUM
+0000b7c0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000b7d0: 740a 2020 2020 2020 2020 6b65 793a 2062  t.        key: b
+0000b7e0: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+0000b7f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000b800: 2020 2020 2020 6465 6620 7661 6c75 6528        def value(
+0000b810: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+0000b820: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+0000b830: 6765 626f 785f 7062 322e 456e 7469 7469  gebox_pb2.Entiti
+0000b840: 6573 4772 6f75 703a 202e 2e2e 0a20 2020  esGroup: ....   
+0000b850: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
+0000b860: 5f28 0a20 2020 2020 2020 2020 2020 2073  _(.            s
+0000b870: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000b880: 202a 2c0a 2020 2020 2020 2020 2020 2020   *,.            
+0000b890: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+0000b8a0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+0000b8b0: 2020 2020 2076 616c 7565 3a20 6e75 636c       value: nucl
+0000b8c0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+0000b8d0: 6c65 6467 6562 6f78 5f70 6232 2e45 6e74  ledgebox_pb2.Ent
+0000b8e0: 6974 6965 7347 726f 7570 207c 204e 6f6e  itiesGroup | Non
+0000b8f0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+0000b900: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+0000b910: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
+0000b920: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000b930: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000b940: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
+0000b950: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
+0000b960: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
+0000b970: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
+0000b980: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+0000b990: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000b9a0: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
+0000b9b0: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
+0000b9c0: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
+0000b9d0: 6e65 3a20 2e2e 2e0a 0a20 2020 204b 425f  ne: .....    KB_
+0000b9e0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000b9f0: 696c 7469 6e73 2e69 6e74 0a20 2020 2047  iltins.int.    G
+0000ba00: 524f 5550 535f 4649 454c 445f 4e55 4d42  ROUPS_FIELD_NUMB
+0000ba10: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000ba20: 0a20 2020 2053 5441 5455 535f 4649 454c  .    STATUS_FIEL
+0000ba30: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000ba40: 6e73 2e69 6e74 0a20 2020 2073 7461 7475  ns.int.    statu
+0000ba50: 733a 2067 6c6f 6261 6c5f 5f5f 4765 7445  s: global___GetE
+0000ba60: 6e74 6974 6965 7352 6573 706f 6e73 652e  ntitiesResponse.
+0000ba70: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000ba80: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000ba90: 2020 2064 6566 206b 6228 7365 6c66 2920     def kb(self) 
+0000baa0: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+0000bab0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000bac0: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
+0000bad0: 4944 3a20 2e2e 2e0a 2020 2020 4070 726f  ID: ....    @pro
+0000bae0: 7065 7274 790a 2020 2020 6465 6620 6772  perty.    def gr
+0000baf0: 6f75 7073 2873 656c 6629 202d 3e20 676f  oups(self) -> go
+0000bb00: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+0000bb10: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+0000bb20: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
+0000bb30: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+0000bb40: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000bb50: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+0000bb60: 7469 6573 4772 6f75 705d 3a20 2e2e 2e0a  tiesGroup]: ....
+0000bb70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000bb80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000bb90: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000bba0: 2020 206b 623a 206e 7563 6c69 6164 625f     kb: nucliadb_
+0000bbb0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000bbc0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+0000bbd0: 6542 6f78 4944 207c 204e 6f6e 6520 3d20  eBoxID | None = 
+0000bbe0: 2e2e 2e2c 0a20 2020 2020 2020 2067 726f  ...,.        gro
+0000bbf0: 7570 733a 2063 6f6c 6c65 6374 696f 6e73  ups: collections
+0000bc00: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
+0000bc10: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+0000bc20: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000bc30: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+0000bc40: 7469 6573 4772 6f75 705d 207c 204e 6f6e  tiesGroup] | Non
+0000bc50: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+0000bc60: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
+0000bc70: 5f5f 4765 7445 6e74 6974 6965 7352 6573  __GetEntitiesRes
+0000bc80: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000bc90: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
+0000bca0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+0000bcb0: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
+0000bcc0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+0000bcd0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+0000bce0: 616c 5b22 6b62 222c 2062 226b 6222 5d29  al["kb", b"kb"])
+0000bcf0: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
+0000bd00: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
+0000bd10: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+0000bd20: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+0000bd30: 6e67 2e4c 6974 6572 616c 5b22 6772 6f75  ng.Literal["grou
+0000bd40: 7073 222c 2062 2267 726f 7570 7322 2c20  ps", b"groups", 
+0000bd50: 226b 6222 2c20 6222 6b62 222c 2022 7374  "kb", b"kb", "st
+0000bd60: 6174 7573 222c 2062 2273 7461 7475 7322  atus", b"status"
+0000bd70: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+0000bd80: 0a67 6c6f 6261 6c5f 5f5f 4765 7445 6e74  .global___GetEnt
+0000bd90: 6974 6965 7352 6573 706f 6e73 6520 3d20  itiesResponse = 
+0000bda0: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
+0000bdb0: 6e73 650a 0a40 7479 7069 6e67 2e66 696e  nse..@typing.fin
+0000bdc0: 616c 0a63 6c61 7373 2044 656c 456e 7469  al.class DelEnti
+0000bdd0: 7469 6573 5265 7175 6573 7428 676f 6f67  tiesRequest(goog
+0000bde0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+0000bdf0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+0000be00: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000be10: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000be20: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000be30: 746f 720a 0a20 2020 204b 425f 4649 454c  tor..    KB_FIEL
+0000be40: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000be50: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
+0000be60: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000be70: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000be80: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
+0000be90: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
+0000bea0: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
+0000beb0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
+0000bec0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000bed0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000bee0: 426f 7849 443a 202e 2e2e 0a20 2020 2064  BoxID: ....    d
+0000bef0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0000bf00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000bf10: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
+0000bf20: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+0000bf30: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000bf40: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
+0000bf50: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
+0000bf60: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
+0000bf70: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+0000bf80: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+0000bf90: 3a20 2e2e 2e0a 2020 2020 6465 6620 4861  : ....    def Ha
+0000bfa0: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
+0000bfb0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000bfc0: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
+0000bfd0: 6b62 225d 2920 2d3e 2062 7569 6c74 696e  kb"]) -> builtin
+0000bfe0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+0000bff0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+0000c000: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000c010: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000c020: 2267 726f 7570 222c 2062 2267 726f 7570  "group", b"group
+0000c030: 222c 2022 6b62 222c 2062 226b 6222 5d29  ", "kb", b"kb"])
+0000c040: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+0000c050: 6c6f 6261 6c5f 5f5f 4465 6c45 6e74 6974  lobal___DelEntit
+0000c060: 6965 7352 6571 7565 7374 203d 2044 656c  iesRequest = Del
+0000c070: 456e 7469 7469 6573 5265 7175 6573 740a  EntitiesRequest.
+0000c080: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
+0000c090: 6c61 7373 204d 6572 6765 456e 7469 7469  lass MergeEntiti
+0000c0a0: 6573 5265 7175 6573 7428 676f 6f67 6c65  esRequest(google
+0000c0b0: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+0000c0c0: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+0000c0d0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+0000c0e0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+0000c0f0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+0000c100: 720a 0a20 2020 2040 7479 7069 6e67 2e66  r..    @typing.f
+0000c110: 696e 616c 0a20 2020 2063 6c61 7373 2045  inal.    class E
+0000c120: 6e74 6974 7949 4428 676f 6f67 6c65 2e70  ntityID(google.p
+0000c130: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000c140: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
+0000c150: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000c160: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000c170: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000c180: 746f 720a 0a20 2020 2020 2020 2047 524f  tor..        GRO
+0000c190: 5550 5f46 4945 4c44 5f4e 554d 4245 523a  UP_FIELD_NUMBER:
+0000c1a0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000c1b0: 2020 2020 2020 454e 5449 5459 5f46 4945        ENTITY_FIE
+0000c1c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000c1d0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+0000c1e0: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
+0000c1f0: 7374 720a 2020 2020 2020 2020 656e 7469  str.        enti
+0000c200: 7479 3a20 6275 696c 7469 6e73 2e73 7472  ty: builtins.str
+0000c210: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
+0000c220: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
+0000c230: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000c240: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+0000c250: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
+0000c260: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+0000c270: 2020 2020 2020 2020 2020 2065 6e74 6974             entit
+0000c280: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
+0000c290: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
+0000c2a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+0000c2b0: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
+0000c2c0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000c2d0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000c2e0: 7465 7261 6c5b 2265 6e74 6974 7922 2c20  teral["entity", 
+0000c2f0: 6222 656e 7469 7479 222c 2022 6772 6f75  b"entity", "grou
+0000c300: 7022 2c20 6222 6772 6f75 7022 5d29 202d  p", b"group"]) -
+0000c310: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020  > None: .....   
+0000c320: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
+0000c330: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000c340: 2020 2046 524f 4d5f 4649 454c 445f 4e55     FROM_FIELD_NU
+0000c350: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+0000c360: 6e74 0a20 2020 2054 4f5f 4649 454c 445f  nt.    TO_FIELD_
+0000c370: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000c380: 2e69 6e74 0a20 2020 2040 7072 6f70 6572  .int.    @proper
+0000c390: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
+0000c3a0: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+0000c3b0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000c3c0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+0000c3d0: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
+0000c3e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000c3f0: 6620 746f 2873 656c 6629 202d 3e20 676c  f to(self) -> gl
+0000c400: 6f62 616c 5f5f 5f4d 6572 6765 456e 7469  obal___MergeEnti
+0000c410: 7469 6573 5265 7175 6573 742e 456e 7469  tiesRequest.Enti
+0000c420: 7479 4944 3a20 2e2e 2e0a 2020 2020 6465  tyID: ....    de
+0000c430: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0000c440: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000c450: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
+0000c460: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000c470: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000c480: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
+0000c490: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+0000c4a0: 2020 2020 2020 2074 6f3a 2067 6c6f 6261         to: globa
+0000c4b0: 6c5f 5f5f 4d65 7267 6545 6e74 6974 6965  l___MergeEntitie
+0000c4c0: 7352 6571 7565 7374 2e45 6e74 6974 7949  sRequest.EntityI
+0000c4d0: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
+0000c4e0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+0000c4f0: 2e2e 0a20 2020 2064 6566 2048 6173 4669  ...    def HasFi
+0000c500: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
+0000c510: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
+0000c520: 6572 616c 5b22 6672 6f6d 222c 2062 2266  eral["from", b"f
+0000c530: 726f 6d22 2c20 226b 6222 2c20 6222 6b62  rom", "kb", b"kb
+0000c540: 222c 2022 746f 222c 2062 2274 6f22 5d29  ", "to", b"to"])
+0000c550: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
+0000c560: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
+0000c570: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+0000c580: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+0000c590: 6e67 2e4c 6974 6572 616c 5b22 6672 6f6d  ng.Literal["from
+0000c5a0: 222c 2062 2266 726f 6d22 2c20 226b 6222  ", b"from", "kb"
+0000c5b0: 2c20 6222 6b62 222c 2022 746f 222c 2062  , b"kb", "to", b
+0000c5c0: 2274 6f22 5d29 202d 3e20 4e6f 6e65 3a20  "to"]) -> None: 
+0000c5d0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4d65  .....global___Me
+0000c5e0: 7267 6545 6e74 6974 6965 7352 6571 7565  rgeEntitiesReque
+0000c5f0: 7374 203d 204d 6572 6765 456e 7469 7469  st = MergeEntiti
+0000c600: 6573 5265 7175 6573 740a 0a40 7479 7069  esRequest..@typi
+0000c610: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
+0000c620: 6574 4c61 6265 6c53 6574 5265 7175 6573  etLabelSetReques
+0000c630: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
+0000c640: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+0000c650: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+0000c660: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000c670: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000c680: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
+0000c690: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
+0000c6a0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000c6b0: 204c 4142 454c 5345 545f 4649 454c 445f   LABELSET_FIELD_
+0000c6c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000c6d0: 2e69 6e74 0a20 2020 206c 6162 656c 7365  .int.    labelse
+0000c6e0: 743a 2062 7569 6c74 696e 732e 7374 720a  t: builtins.str.
+0000c6f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000c700: 2020 6465 6620 6b62 2873 656c 6629 202d    def kb(self) -
+0000c710: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
+0000c720: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000c730: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
+0000c740: 443a 202e 2e2e 0a20 2020 2064 6566 205f  D: ....    def _
+0000c750: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000c760: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0000c770: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
+0000c780: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+0000c790: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
+0000c7a0: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
+0000c7b0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+0000c7c0: 2020 2020 6c61 6265 6c73 6574 3a20 6275      labelset: bu
+0000c7d0: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
+0000c7e0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+0000c7f0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
+0000c800: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+0000c810: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+0000c820: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
+0000c830: 6222 5d29 202d 3e20 6275 696c 7469 6e73  b"]) -> builtins
+0000c840: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2064  .bool: ....    d
+0000c850: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
+0000c860: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
+0000c870: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
+0000c880: 6b62 222c 2062 226b 6222 2c20 226c 6162  kb", b"kb", "lab
+0000c890: 656c 7365 7422 2c20 6222 6c61 6265 6c73  elset", b"labels
+0000c8a0: 6574 225d 2920 2d3e 204e 6f6e 653a 202e  et"]) -> None: .
+0000c8b0: 2e2e 0a0a 676c 6f62 616c 5f5f 5f47 6574  ....global___Get
+0000c8c0: 4c61 6265 6c53 6574 5265 7175 6573 7420  LabelSetRequest 
+0000c8d0: 3d20 4765 744c 6162 656c 5365 7452 6571  = GetLabelSetReq
+0000c8e0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+0000c8f0: 6e61 6c0a 636c 6173 7320 4765 744c 6162  nal.class GetLab
+0000c900: 656c 5365 7452 6573 706f 6e73 6528 676f  elSetResponse(go
+0000c910: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+0000c920: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+0000c930: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+0000c940: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000c950: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+0000c960: 6970 746f 720a 0a20 2020 2063 6c61 7373  iptor..    class
+0000c970: 205f 5374 6174 7573 3a0a 2020 2020 2020   _Status:.      
+0000c980: 2020 5661 6c75 6554 7970 6520 3d20 7479    ValueType = ty
+0000c990: 7069 6e67 2e4e 6577 5479 7065 2822 5661  ping.NewType("Va
+0000c9a0: 6c75 6554 7970 6522 2c20 6275 696c 7469  lueType", builti
+0000c9b0: 6e73 2e69 6e74 290a 2020 2020 2020 2020  ns.int).        
+0000c9c0: 563a 2074 7970 696e 675f 6578 7465 6e73  V: typing_extens
+0000c9d0: 696f 6e73 2e54 7970 6541 6c69 6173 203d  ions.TypeAlias =
+0000c9e0: 2056 616c 7565 5479 7065 0a0a 2020 2020   ValueType..    
+0000c9f0: 636c 6173 7320 5f53 7461 7475 7345 6e75  class _StatusEnu
+0000ca00: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
+0000ca10: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+0000ca20: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
+0000ca30: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
+0000ca40: 6557 7261 7070 6572 5b47 6574 4c61 6265  eWrapper[GetLabe
+0000ca50: 6c53 6574 5265 7370 6f6e 7365 2e5f 5374  lSetResponse._St
+0000ca60: 6174 7573 2e56 616c 7565 5479 7065 5d2c  atus.ValueType],
+0000ca70: 2062 7569 6c74 696e 732e 7479 7065 293a   builtins.type):
+0000ca80: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+0000ca90: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+0000caa0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+0000cab0: 456e 756d 4465 7363 7269 7074 6f72 0a20  EnumDescriptor. 
+0000cac0: 2020 2020 2020 204f 4b3a 2047 6574 4c61         OK: GetLa
+0000cad0: 6265 6c53 6574 5265 7370 6f6e 7365 2e5f  belSetResponse._
+0000cae0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000caf0: 2020 2320 300a 2020 2020 2020 2020 4e4f    # 0.        NO
+0000cb00: 5446 4f55 4e44 3a20 4765 744c 6162 656c  TFOUND: GetLabel
+0000cb10: 5365 7452 6573 706f 6e73 652e 5f53 7461  SetResponse._Sta
+0000cb20: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000cb30: 2031 0a0a 2020 2020 636c 6173 7320 5374   1..    class St
+0000cb40: 6174 7573 285f 5374 6174 7573 2c20 6d65  atus(_Status, me
+0000cb50: 7461 636c 6173 733d 5f53 7461 7475 7345  taclass=_StatusE
+0000cb60: 6e75 6d54 7970 6557 7261 7070 6572 293a  numTypeWrapper):
+0000cb70: 202e 2e2e 0a20 2020 204f 4b3a 2047 6574   ....    OK: Get
+0000cb80: 4c61 6265 6c53 6574 5265 7370 6f6e 7365  LabelSetResponse
+0000cb90: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+0000cba0: 6520 2023 2030 0a20 2020 204e 4f54 464f  e  # 0.    NOTFO
+0000cbb0: 554e 443a 2047 6574 4c61 6265 6c53 6574  UND: GetLabelSet
+0000cbc0: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
+0000cbd0: 5661 6c75 6554 7970 6520 2023 2031 0a0a  ValueType  # 1..
+0000cbe0: 2020 2020 4b42 5f46 4945 4c44 5f4e 554d      KB_FIELD_NUM
+0000cbf0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000cc00: 740a 2020 2020 4c41 4245 4c53 4554 5f46  t.    LABELSET_F
+0000cc10: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000cc20: 6c74 696e 732e 696e 740a 2020 2020 5354  ltins.int.    ST
+0000cc30: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
+0000cc40: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000cc50: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+0000cc60: 616c 5f5f 5f47 6574 4c61 6265 6c53 6574  al___GetLabelSet
+0000cc70: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
+0000cc80: 5661 6c75 6554 7970 650a 2020 2020 4070  ValueType.    @p
+0000cc90: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000cca0: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
+0000ccb0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+0000ccc0: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
+0000ccd0: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
+0000cce0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000ccf0: 2020 2064 6566 206c 6162 656c 7365 7428     def labelset(
+0000cd00: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+0000cd10: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+0000cd20: 6765 626f 785f 7062 322e 4c61 6265 6c53  gebox_pb2.LabelS
+0000cd30: 6574 3a20 2e2e 2e0a 2020 2020 6465 6620  et: ....    def 
+0000cd40: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0000cd50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000cd60: 2a2c 0a20 2020 2020 2020 206b 623a 206e  *,.        kb: n
+0000cd70: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+0000cd80: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+0000cd90: 4b6e 6f77 6c65 6467 6542 6f78 4944 207c  KnowledgeBoxID |
+0000cda0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+0000cdb0: 2020 2020 206c 6162 656c 7365 743a 206e       labelset: n
+0000cdc0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+0000cdd0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+0000cde0: 4c61 6265 6c53 6574 207c 204e 6f6e 6520  LabelSet | None 
+0000cdf0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2073  = ...,.        s
+0000ce00: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
+0000ce10: 4765 744c 6162 656c 5365 7452 6573 706f  GetLabelSetRespo
+0000ce20: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+0000ce30: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+0000ce40: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+0000ce50: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
+0000ce60: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000ce70: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000ce80: 5b22 6b62 222c 2062 226b 6222 2c20 226c  ["kb", b"kb", "l
+0000ce90: 6162 656c 7365 7422 2c20 6222 6c61 6265  abelset", b"labe
+0000cea0: 6c73 6574 225d 2920 2d3e 2062 7569 6c74  lset"]) -> built
+0000ceb0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+0000cec0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
+0000ced0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+0000cee0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+0000cef0: 6c5b 226b 6222 2c20 6222 6b62 222c 2022  l["kb", b"kb", "
+0000cf00: 6c61 6265 6c73 6574 222c 2062 226c 6162  labelset", b"lab
+0000cf10: 656c 7365 7422 2c20 2273 7461 7475 7322  elset", "status"
+0000cf20: 2c20 6222 7374 6174 7573 225d 2920 2d3e  , b"status"]) ->
+0000cf30: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+0000cf40: 616c 5f5f 5f47 6574 4c61 6265 6c53 6574  al___GetLabelSet
+0000cf50: 5265 7370 6f6e 7365 203d 2047 6574 4c61  Response = GetLa
+0000cf60: 6265 6c53 6574 5265 7370 6f6e 7365 0a0a  belSetResponse..
+0000cf70: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
+0000cf80: 6173 7320 4765 7445 6e74 6974 6965 7347  ass GetEntitiesG
+0000cf90: 726f 7570 5265 7175 6573 7428 676f 6f67  roupRequest(goog
+0000cfa0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+0000cfb0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+0000cfc0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000cfd0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000cfe0: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000cff0: 746f 720a 0a20 2020 204b 425f 4649 454c  tor..    KB_FIEL
+0000d000: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000d010: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
+0000d020: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000d030: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000d040: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
+0000d050: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
+0000d060: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
+0000d070: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
+0000d080: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000d090: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000d0a0: 426f 7849 443a 202e 2e2e 0a20 2020 2064  BoxID: ....    d
+0000d0b0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0000d0c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000d0d0: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
+0000d0e0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+0000d0f0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000d100: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
+0000d110: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
+0000d120: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
+0000d130: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+0000d140: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+0000d150: 3a20 2e2e 2e0a 2020 2020 6465 6620 4861  : ....    def Ha
+0000d160: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
+0000d170: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000d180: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
+0000d190: 6b62 225d 2920 2d3e 2062 7569 6c74 696e  kb"]) -> builtin
+0000d1a0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+0000d1b0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+0000d1c0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000d1d0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000d1e0: 2267 726f 7570 222c 2062 2267 726f 7570  "group", b"group
+0000d1f0: 222c 2022 6b62 222c 2062 226b 6222 5d29  ", "kb", b"kb"])
+0000d200: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+0000d210: 6c6f 6261 6c5f 5f5f 4765 7445 6e74 6974  lobal___GetEntit
+0000d220: 6965 7347 726f 7570 5265 7175 6573 7420  iesGroupRequest 
+0000d230: 3d20 4765 7445 6e74 6974 6965 7347 726f  = GetEntitiesGro
+0000d240: 7570 5265 7175 6573 740a 0a40 7479 7069  upRequest..@typi
+0000d250: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
+0000d260: 6574 456e 7469 7469 6573 4772 6f75 7052  etEntitiesGroupR
+0000d270: 6573 706f 6e73 6528 676f 6f67 6c65 2e70  esponse(google.p
+0000d280: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000d290: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+0000d2a0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+0000d2b0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+0000d2c0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+0000d2d0: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
+0000d2e0: 7573 3a0a 2020 2020 2020 2020 5661 6c75  us:.        Valu
+0000d2f0: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
+0000d300: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
+0000d310: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
+0000d320: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
+0000d330: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
+0000d340: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
+0000d350: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
+0000d360: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
+0000d370: 7261 7070 6572 2867 6f6f 676c 652e 7072  rapper(google.pr
+0000d380: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
+0000d390: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
+0000d3a0: 722e 5f45 6e75 6d54 7970 6557 7261 7070  r._EnumTypeWrapp
+0000d3b0: 6572 5b47 6574 456e 7469 7469 6573 4772  er[GetEntitiesGr
+0000d3c0: 6f75 7052 6573 706f 6e73 652e 5f53 7461  oupResponse._Sta
+0000d3d0: 7475 732e 5661 6c75 6554 7970 655d 2c20  tus.ValueType], 
+0000d3e0: 6275 696c 7469 6e73 2e74 7970 6529 3a0a  builtins.type):.
+0000d3f0: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+0000d400: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000d410: 6275 662e 6465 7363 7269 7074 6f72 2e45  buf.descriptor.E
+0000d420: 6e75 6d44 6573 6372 6970 746f 720a 2020  numDescriptor.  
+0000d430: 2020 2020 2020 4f4b 3a20 4765 7445 6e74        OK: GetEnt
+0000d440: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+0000d450: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+0000d460: 5479 7065 2020 2320 300a 2020 2020 2020  Type  # 0.      
+0000d470: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
+0000d480: 4765 7445 6e74 6974 6965 7347 726f 7570  GetEntitiesGroup
+0000d490: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+0000d4a0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
+0000d4b0: 2020 2020 2020 2020 454e 5449 5449 4553          ENTITIES
+0000d4c0: 5f47 524f 5550 5f4e 4f54 5f46 4f55 4e44  _GROUP_NOT_FOUND
+0000d4d0: 3a20 4765 7445 6e74 6974 6965 7347 726f  : GetEntitiesGro
+0000d4e0: 7570 5265 7370 6f6e 7365 2e5f 5374 6174  upResponse._Stat
+0000d4f0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000d500: 320a 2020 2020 2020 2020 4552 524f 523a  2.        ERROR:
+0000d510: 2047 6574 456e 7469 7469 6573 4772 6f75   GetEntitiesGrou
+0000d520: 7052 6573 706f 6e73 652e 5f53 7461 7475  pResponse._Statu
+0000d530: 732e 5661 6c75 6554 7970 6520 2023 2033  s.ValueType  # 3
+0000d540: 0a0a 2020 2020 636c 6173 7320 5374 6174  ..    class Stat
+0000d550: 7573 285f 5374 6174 7573 2c20 6d65 7461  us(_Status, meta
+0000d560: 636c 6173 733d 5f53 7461 7475 7345 6e75  class=_StatusEnu
+0000d570: 6d54 7970 6557 7261 7070 6572 293a 202e  mTypeWrapper): .
+0000d580: 2e2e 0a20 2020 204f 4b3a 2047 6574 456e  ...    OK: GetEn
+0000d590: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+0000d5a0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+0000d5b0: 5479 7065 2020 2320 300a 2020 2020 4b42  Type  # 0.    KB
+0000d5c0: 5f4e 4f54 5f46 4f55 4e44 3a20 4765 7445  _NOT_FOUND: GetE
+0000d5d0: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
+0000d5e0: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+0000d5f0: 6554 7970 6520 2023 2031 0a20 2020 2045  eType  # 1.    E
+0000d600: 4e54 4954 4945 535f 4752 4f55 505f 4e4f  NTITIES_GROUP_NO
+0000d610: 545f 464f 554e 443a 2047 6574 456e 7469  T_FOUND: GetEnti
+0000d620: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+0000d630: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+0000d640: 7065 2020 2320 320a 2020 2020 4552 524f  pe  # 2.    ERRO
+0000d650: 523a 2047 6574 456e 7469 7469 6573 4772  R: GetEntitiesGr
+0000d660: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
+0000d670: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000d680: 330a 0a20 2020 204b 425f 4649 454c 445f  3..    KB_FIELD_
+0000d690: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000d6a0: 2e69 6e74 0a20 2020 2047 524f 5550 5f46  .int.    GROUP_F
+0000d6b0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000d6c0: 6c74 696e 732e 696e 740a 2020 2020 5354  ltins.int.    ST
+0000d6d0: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
+0000d6e0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000d6f0: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+0000d700: 616c 5f5f 5f47 6574 456e 7469 7469 6573  al___GetEntities
+0000d710: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
+0000d720: 6174 7573 2e56 616c 7565 5479 7065 0a20  atus.ValueType. 
+0000d730: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000d740: 2064 6566 206b 6228 7365 6c66 2920 2d3e   def kb(self) ->
+0000d750: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000d760: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000d770: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
+0000d780: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
+0000d790: 7274 790a 2020 2020 6465 6620 6772 6f75  rty.    def grou
+0000d7a0: 7028 7365 6c66 2920 2d3e 206e 7563 6c69  p(self) -> nucli
+0000d7b0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000d7c0: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+0000d7d0: 7469 6573 4772 6f75 703a 202e 2e2e 0a20  tiesGroup: .... 
+0000d7e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000d7f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000d800: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0000d810: 2020 6b62 3a20 6e75 636c 6961 6462 5f70    kb: nucliadb_p
+0000d820: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000d830: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000d840: 426f 7849 4420 7c20 4e6f 6e65 203d 202e  BoxID | None = .
+0000d850: 2e2e 2c0a 2020 2020 2020 2020 6772 6f75  ..,.        grou
+0000d860: 703a 206e 7563 6c69 6164 625f 7072 6f74  p: nucliadb_prot
+0000d870: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000d880: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
+0000d890: 7020 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  p | None = ...,.
+0000d8a0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
+0000d8b0: 676c 6f62 616c 5f5f 5f47 6574 456e 7469  global___GetEnti
+0000d8c0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+0000d8d0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+0000d8e0: 7065 203d 202e 2e2e 2c0a 2020 2020 2920  pe = ...,.    ) 
+0000d8f0: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+0000d900: 2064 6566 2048 6173 4669 656c 6428 7365   def HasField(se
+0000d910: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
+0000d920: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
+0000d930: 6772 6f75 7022 2c20 6222 6772 6f75 7022  group", b"group"
+0000d940: 2c20 226b 6222 2c20 6222 6b62 225d 2920  , "kb", b"kb"]) 
+0000d950: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+0000d960: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+0000d970: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+0000d980: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+0000d990: 672e 4c69 7465 7261 6c5b 2267 726f 7570  g.Literal["group
+0000d9a0: 222c 2062 2267 726f 7570 222c 2022 6b62  ", b"group", "kb
+0000d9b0: 222c 2062 226b 6222 2c20 2273 7461 7475  ", b"kb", "statu
+0000d9c0: 7322 2c20 6222 7374 6174 7573 225d 2920  s", b"status"]) 
+0000d9d0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
+0000d9e0: 6f62 616c 5f5f 5f47 6574 456e 7469 7469  obal___GetEntiti
+0000d9f0: 6573 4772 6f75 7052 6573 706f 6e73 6520  esGroupResponse 
+0000da00: 3d20 4765 7445 6e74 6974 6965 7347 726f  = GetEntitiesGro
+0000da10: 7570 5265 7370 6f6e 7365 0a0a 4074 7970  upResponse..@typ
+0000da20: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+0000da30: 4765 7456 6563 746f 7253 6574 7352 6571  GetVectorSetsReq
+0000da40: 7565 7374 2867 6f6f 676c 652e 7072 6f74  uest(google.prot
+0000da50: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+0000da60: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+0000da70: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+0000da80: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+0000da90: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+0000daa0: 2020 4b42 5f46 4945 4c44 5f4e 554d 4245    KB_FIELD_NUMBE
+0000dab0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000dac0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000dad0: 2020 6465 6620 6b62 2873 656c 6629 202d    def kb(self) -
+0000dae0: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
+0000daf0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000db00: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
+0000db10: 443a 202e 2e2e 0a20 2020 2064 6566 205f  D: ....    def _
+0000db20: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000db30: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0000db40: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
+0000db50: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+0000db60: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
+0000db70: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
+0000db80: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+0000db90: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+0000dba0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
+0000dbb0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000dbc0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000dbd0: 5b22 6b62 222c 2062 226b 6222 5d29 202d  ["kb", b"kb"]) -
+0000dbe0: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
+0000dbf0: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
+0000dc00: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+0000dc10: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+0000dc20: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
+0000dc30: 226b 6222 5d29 202d 3e20 4e6f 6e65 3a20  "kb"]) -> None: 
+0000dc40: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765  .....global___Ge
+0000dc50: 7456 6563 746f 7253 6574 7352 6571 7565  tVectorSetsReque
+0000dc60: 7374 203d 2047 6574 5665 6374 6f72 5365  st = GetVectorSe
+0000dc70: 7473 5265 7175 6573 740a 0a40 7479 7069  tsRequest..@typi
+0000dc80: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
+0000dc90: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
+0000dca0: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
+0000dcb0: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+0000dcc0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+0000dcd0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+0000dce0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+0000dcf0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+0000dd00: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
+0000dd10: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
+0000dd20: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
+0000dd30: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
+0000dd40: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
+0000dd50: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
+0000dd60: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
+0000dd70: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
+0000dd80: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
+0000dd90: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
+0000dda0: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
+0000ddb0: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
+0000ddc0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
+0000ddd0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
+0000dde0: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
+0000ddf0: 706f 6e73 652e 5f53 7461 7475 732e 5661  ponse._Status.Va
+0000de00: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
+0000de10: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
+0000de20: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000de30: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000de40: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
+0000de50: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
+0000de60: 4f4b 3a20 4765 7456 6563 746f 7253 6574  OK: GetVectorSet
+0000de70: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
+0000de80: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
+0000de90: 0a20 2020 2020 2020 204e 4f54 464f 554e  .        NOTFOUN
+0000dea0: 443a 2047 6574 5665 6374 6f72 5365 7473  D: GetVectorSets
+0000deb0: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+0000dec0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
+0000ded0: 2020 2020 2020 2020 4552 524f 523a 2047          ERROR: G
+0000dee0: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
+0000def0: 6f6e 7365 2e5f 5374 6174 7573 2e56 616c  onse._Status.Val
+0000df00: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
+0000df10: 2063 6c61 7373 2053 7461 7475 7328 5f53   class Status(_S
+0000df20: 7461 7475 732c 206d 6574 6163 6c61 7373  tatus, metaclass
+0000df30: 3d5f 5374 6174 7573 456e 756d 5479 7065  =_StatusEnumType
+0000df40: 5772 6170 7065 7229 3a20 2e2e 2e0a 2020  Wrapper): ....  
+0000df50: 2020 4f4b 3a20 4765 7456 6563 746f 7253    OK: GetVectorS
+0000df60: 6574 7352 6573 706f 6e73 652e 5374 6174  etsResponse.Stat
+0000df70: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000df80: 300a 2020 2020 4e4f 5446 4f55 4e44 3a20  0.    NOTFOUND: 
+0000df90: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
+0000dfa0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000dfb0: 7565 5479 7065 2020 2320 310a 2020 2020  ueType  # 1.    
+0000dfc0: 4552 524f 523a 2047 6574 5665 6374 6f72  ERROR: GetVector
+0000dfd0: 5365 7473 5265 7370 6f6e 7365 2e53 7461  SetsResponse.Sta
+0000dfe0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000dff0: 2032 0a0a 2020 2020 4b42 5f46 4945 4c44   2..    KB_FIELD
+0000e000: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+0000e010: 732e 696e 740a 2020 2020 5645 4354 4f52  s.int.    VECTOR
+0000e020: 5345 5453 5f46 4945 4c44 5f4e 554d 4245  SETS_FIELD_NUMBE
+0000e030: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000e040: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
+0000e050: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+0000e060: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
+0000e070: 3a20 676c 6f62 616c 5f5f 5f47 6574 5665  : global___GetVe
+0000e080: 6374 6f72 5365 7473 5265 7370 6f6e 7365  ctorSetsResponse
+0000e090: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+0000e0a0: 650a 2020 2020 4070 726f 7065 7274 790a  e.    @property.
+0000e0b0: 2020 2020 6465 6620 6b62 2873 656c 6629      def kb(self)
+0000e0c0: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+0000e0d0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+0000e0e0: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
+0000e0f0: 7849 443a 202e 2e2e 0a20 2020 2040 7072  xID: ....    @pr
+0000e100: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
+0000e110: 6563 746f 7273 6574 7328 7365 6c66 2920  ectorsets(self) 
+0000e120: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+0000e130: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000e140: 7062 322e 5665 6374 6f72 5365 7473 3a20  pb2.VectorSets: 
+0000e150: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+0000e160: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0000e170: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
+0000e180: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
+0000e190: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000e1a0: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
+0000e1b0: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
+0000e1c0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+0000e1d0: 2076 6563 746f 7273 6574 733a 206e 7563   vectorsets: nuc
+0000e1e0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+0000e1f0: 776c 6564 6765 626f 785f 7062 322e 5665  wledgebox_pb2.Ve
+0000e200: 6374 6f72 5365 7473 207c 204e 6f6e 6520  ctorSets | None 
+0000e210: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2073  = ...,.        s
+0000e220: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
+0000e230: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
+0000e240: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000e250: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
+0000e260: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+0000e270: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
+0000e280: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+0000e290: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+0000e2a0: 616c 5b22 6b62 222c 2062 226b 6222 2c20  al["kb", b"kb", 
+0000e2b0: 2276 6563 746f 7273 6574 7322 2c20 6222  "vectorsets", b"
+0000e2c0: 7665 6374 6f72 7365 7473 225d 2920 2d3e  vectorsets"]) ->
+0000e2d0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+0000e2e0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+0000e2f0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+0000e300: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000e310: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
+0000e320: 6b62 222c 2022 7374 6174 7573 222c 2062  kb", "status", b
+0000e330: 2273 7461 7475 7322 2c20 2276 6563 746f  "status", "vecto
+0000e340: 7273 6574 7322 2c20 6222 7665 6374 6f72  rsets", b"vector
+0000e350: 7365 7473 225d 2920 2d3e 204e 6f6e 653a  sets"]) -> None:
+0000e360: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f47   .....global___G
+0000e370: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
+0000e380: 6f6e 7365 203d 2047 6574 5665 6374 6f72  onse = GetVector
+0000e390: 5365 7473 5265 7370 6f6e 7365 0a0a 4074  SetsResponse..@t
+0000e3a0: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
+0000e3b0: 7320 4465 6c56 6563 746f 7253 6574 5265  s DelVectorSetRe
+0000e3c0: 7175 6573 7428 676f 6f67 6c65 2e70 726f  quest(google.pro
+0000e3d0: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+0000e3e0: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
+0000e3f0: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+0000e400: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+0000e410: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
+0000e420: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
+0000e430: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000e440: 0a20 2020 2056 4543 544f 5253 4554 5f46  .    VECTORSET_F
+0000e450: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000e460: 6c74 696e 732e 696e 740a 2020 2020 7665  ltins.int.    ve
+0000e470: 6374 6f72 7365 743a 2062 7569 6c74 696e  ctorset: builtin
+0000e480: 732e 7374 720a 2020 2020 4070 726f 7065  s.str.    @prope
+0000e490: 7274 790a 2020 2020 6465 6620 6b62 2873  rty.    def kb(s
+0000e4a0: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
+0000e4b0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
+0000e4c0: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
+0000e4d0: 6765 426f 7849 443a 202e 2e2e 0a20 2020  geBoxID: ....   
+0000e4e0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0000e4f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000e500: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+0000e510: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
+0000e520: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+0000e530: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
+0000e540: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
+0000e550: 2c0a 2020 2020 2020 2020 7665 6374 6f72  ,.        vector
+0000e560: 7365 743a 2062 7569 6c74 696e 732e 7374  set: builtins.st
+0000e570: 7220 3d20 2e2e 2e2c 0a20 2020 2029 202d  r = ...,.    ) -
+0000e580: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+0000e590: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+0000e5a0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+0000e5b0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+0000e5c0: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
+0000e5d0: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+0000e5e0: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+0000e5f0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000e600: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000e610: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
+0000e620: 222c 2022 7665 6374 6f72 7365 7422 2c20  ", "vectorset", 
+0000e630: 6222 7665 6374 6f72 7365 7422 5d29 202d  b"vectorset"]) -
+0000e640: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+0000e650: 6261 6c5f 5f5f 4465 6c56 6563 746f 7253  bal___DelVectorS
+0000e660: 6574 5265 7175 6573 7420 3d20 4465 6c56  etRequest = DelV
+0000e670: 6563 746f 7253 6574 5265 7175 6573 740a  ectorSetRequest.
+0000e680: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
+0000e690: 6c61 7373 2053 6574 5665 6374 6f72 5365  lass SetVectorSe
+0000e6a0: 7452 6571 7565 7374 2867 6f6f 676c 652e  tRequest(google.
+0000e6b0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+0000e6c0: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
+0000e6d0: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+0000e6e0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+0000e6f0: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+0000e700: 0a0a 2020 2020 4b42 5f46 4945 4c44 5f4e  ..    KB_FIELD_N
+0000e710: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000e720: 696e 740a 2020 2020 4944 5f46 4945 4c44  int.    ID_FIELD
+0000e730: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+0000e740: 732e 696e 740a 2020 2020 5645 4354 4f52  s.int.    VECTOR
+0000e750: 5345 545f 4649 454c 445f 4e55 4d42 4552  SET_FIELD_NUMBER
+0000e760: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000e770: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
+0000e780: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
+0000e790: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
+0000e7a0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
+0000e7b0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000e7c0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000e7d0: 426f 7849 443a 202e 2e2e 0a20 2020 2040  BoxID: ....    @
+0000e7e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000e7f0: 2076 6563 746f 7273 6574 2873 656c 6629   vectorset(self)
+0000e800: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+0000e810: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+0000e820: 5f70 6232 2e56 6563 746f 7253 6574 3a20  _pb2.VectorSet: 
+0000e830: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+0000e840: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0000e850: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
+0000e860: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
+0000e870: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000e880: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
+0000e890: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
+0000e8a0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+0000e8b0: 2069 643a 2062 7569 6c74 696e 732e 7374   id: builtins.st
+0000e8c0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+0000e8d0: 2076 6563 746f 7273 6574 3a20 6e75 636c   vectorset: nucl
+0000e8e0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+0000e8f0: 6c65 6467 6562 6f78 5f70 6232 2e56 6563  ledgebox_pb2.Vec
+0000e900: 746f 7253 6574 207c 204e 6f6e 6520 3d20  torSet | None = 
+0000e910: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
+0000e920: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+0000e930: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
+0000e940: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+0000e950: 672e 4c69 7465 7261 6c5b 226b 6222 2c20  g.Literal["kb", 
+0000e960: 6222 6b62 222c 2022 7665 6374 6f72 7365  b"kb", "vectorse
+0000e970: 7422 2c20 6222 7665 6374 6f72 7365 7422  t", b"vectorset"
+0000e980: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
+0000e990: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
+0000e9a0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+0000e9b0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+0000e9c0: 7069 6e67 2e4c 6974 6572 616c 5b22 6964  ping.Literal["id
+0000e9d0: 222c 2062 2269 6422 2c20 226b 6222 2c20  ", b"id", "kb", 
+0000e9e0: 6222 6b62 222c 2022 7665 6374 6f72 7365  b"kb", "vectorse
+0000e9f0: 7422 2c20 6222 7665 6374 6f72 7365 7422  t", b"vectorset"
+0000ea00: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+0000ea10: 0a67 6c6f 6261 6c5f 5f5f 5365 7456 6563  .global___SetVec
+0000ea20: 746f 7253 6574 5265 7175 6573 7420 3d20  torSetRequest = 
+0000ea30: 5365 7456 6563 746f 7253 6574 5265 7175  SetVectorSetRequ
+0000ea40: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
+0000ea50: 616c 0a63 6c61 7373 204f 7053 7461 7475  al.class OpStatu
+0000ea60: 7357 7269 7465 7228 676f 6f67 6c65 2e70  sWriter(google.p
+0000ea70: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000ea80: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+0000ea90: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+0000eaa0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+0000eab0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+0000eac0: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
+0000ead0: 7573 3a0a 2020 2020 2020 2020 5661 6c75  us:.        Valu
+0000eae0: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
+0000eaf0: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
+0000eb00: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
+0000eb10: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
+0000eb20: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
+0000eb30: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
+0000eb40: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
+0000eb50: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
+0000eb60: 7261 7070 6572 2867 6f6f 676c 652e 7072  rapper(google.pr
+0000eb70: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
+0000eb80: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
+0000eb90: 722e 5f45 6e75 6d54 7970 6557 7261 7070  r._EnumTypeWrapp
+0000eba0: 6572 5b4f 7053 7461 7475 7357 7269 7465  er[OpStatusWrite
+0000ebb0: 722e 5f53 7461 7475 732e 5661 6c75 6554  r._Status.ValueT
+0000ebc0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
+0000ebd0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
+0000ebe0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+0000ebf0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+0000ec00: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
+0000ec10: 746f 720a 2020 2020 2020 2020 4f4b 3a20  tor.        OK: 
+0000ec20: 4f70 5374 6174 7573 5772 6974 6572 2e5f  OpStatusWriter._
+0000ec30: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000ec40: 2020 2320 300a 2020 2020 2020 2020 4552    # 0.        ER
+0000ec50: 524f 523a 204f 7053 7461 7475 7357 7269  ROR: OpStatusWri
+0000ec60: 7465 722e 5f53 7461 7475 732e 5661 6c75  ter._Status.Valu
+0000ec70: 6554 7970 6520 2023 2031 0a20 2020 2020  eType  # 1.     
+0000ec80: 2020 204e 4f54 464f 554e 443a 204f 7053     NOTFOUND: OpS
+0000ec90: 7461 7475 7357 7269 7465 722e 5f53 7461  tatusWriter._Sta
+0000eca0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000ecb0: 2032 0a0a 2020 2020 636c 6173 7320 5374   2..    class St
+0000ecc0: 6174 7573 285f 5374 6174 7573 2c20 6d65  atus(_Status, me
+0000ecd0: 7461 636c 6173 733d 5f53 7461 7475 7345  taclass=_StatusE
+0000ece0: 6e75 6d54 7970 6557 7261 7070 6572 293a  numTypeWrapper):
+0000ecf0: 202e 2e2e 0a20 2020 204f 4b3a 204f 7053   ....    OK: OpS
+0000ed00: 7461 7475 7357 7269 7465 722e 5374 6174  tatusWriter.Stat
+0000ed10: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000ed20: 300a 2020 2020 4552 524f 523a 204f 7053  0.    ERROR: OpS
+0000ed30: 7461 7475 7357 7269 7465 722e 5374 6174  tatusWriter.Stat
+0000ed40: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000ed50: 310a 2020 2020 4e4f 5446 4f55 4e44 3a20  1.    NOTFOUND: 
+0000ed60: 4f70 5374 6174 7573 5772 6974 6572 2e53  OpStatusWriter.S
+0000ed70: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000ed80: 2023 2032 0a0a 2020 2020 5354 4154 5553   # 2..    STATUS
+0000ed90: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000eda0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000edb0: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
+0000edc0: 5f4f 7053 7461 7475 7357 7269 7465 722e  _OpStatusWriter.
+0000edd0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000ede0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000edf0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0000ee00: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000ee10: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+0000ee20: 616c 5f5f 5f4f 7053 7461 7475 7357 7269  al___OpStatusWri
+0000ee30: 7465 722e 5374 6174 7573 2e56 616c 7565  ter.Status.Value
+0000ee40: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+0000ee50: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+0000ee60: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+0000ee70: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+0000ee80: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+0000ee90: 616c 5b22 7374 6174 7573 222c 2062 2273  al["status", b"s
+0000eea0: 7461 7475 7322 5d29 202d 3e20 4e6f 6e65  tatus"]) -> None
+0000eeb0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+0000eec0: 4f70 5374 6174 7573 5772 6974 6572 203d  OpStatusWriter =
+0000eed0: 204f 7053 7461 7475 7357 7269 7465 720a   OpStatusWriter.
+0000eee0: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
+0000eef0: 6c61 7373 204e 6f74 6966 6963 6174 696f  lass Notificatio
+0000ef00: 6e28 676f 6f67 6c65 2e70 726f 746f 6275  n(google.protobu
+0000ef10: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+0000ef20: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+0000ef30: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000ef40: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000ef50: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
+0000ef60: 6c61 7373 205f 4163 7469 6f6e 3a0a 2020  lass _Action:.  
+0000ef70: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
+0000ef80: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
+0000ef90: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
+0000efa0: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
+0000efb0: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
+0000efc0: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
+0000efd0: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
+0000efe0: 2020 2020 636c 6173 7320 5f41 6374 696f      class _Actio
+0000eff0: 6e45 6e75 6d54 7970 6557 7261 7070 6572  nEnumTypeWrapper
+0000f000: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
+0000f010: 2e69 6e74 6572 6e61 6c2e 656e 756d 5f74  .internal.enum_t
+0000f020: 7970 655f 7772 6170 7065 722e 5f45 6e75  ype_wrapper._Enu
+0000f030: 6d54 7970 6557 7261 7070 6572 5b4e 6f74  mTypeWrapper[Not
+0000f040: 6966 6963 6174 696f 6e2e 5f41 6374 696f  ification._Actio
+0000f050: 6e2e 5661 6c75 6554 7970 655d 2c20 6275  n.ValueType], bu
+0000f060: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
+0000f070: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
+0000f080: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+0000f090: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
+0000f0a0: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
+0000f0b0: 2020 2020 434f 4d4d 4954 3a20 4e6f 7469      COMMIT: Noti
+0000f0c0: 6669 6361 7469 6f6e 2e5f 4163 7469 6f6e  fication._Action
+0000f0d0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
+0000f0e0: 2020 2020 2020 2020 4142 4f52 543a 204e          ABORT: N
+0000f0f0: 6f74 6966 6963 6174 696f 6e2e 5f41 6374  otification._Act
+0000f100: 696f 6e2e 5661 6c75 6554 7970 6520 2023  ion.ValueType  #
+0000f110: 2031 0a20 2020 2020 2020 2049 4e44 4558   1.        INDEX
+0000f120: 4544 3a20 4e6f 7469 6669 6361 7469 6f6e  ED: Notification
+0000f130: 2e5f 4163 7469 6f6e 2e56 616c 7565 5479  ._Action.ValueTy
+0000f140: 7065 2020 2320 320a 0a20 2020 2063 6c61  pe  # 2..    cla
+0000f150: 7373 2041 6374 696f 6e28 5f41 6374 696f  ss Action(_Actio
+0000f160: 6e2c 206d 6574 6163 6c61 7373 3d5f 4163  n, metaclass=_Ac
+0000f170: 7469 6f6e 456e 756d 5479 7065 5772 6170  tionEnumTypeWrap
+0000f180: 7065 7229 3a20 2e2e 2e0a 2020 2020 434f  per): ....    CO
+0000f190: 4d4d 4954 3a20 4e6f 7469 6669 6361 7469  MMIT: Notificati
+0000f1a0: 6f6e 2e41 6374 696f 6e2e 5661 6c75 6554  on.Action.ValueT
+0000f1b0: 7970 6520 2023 2030 0a20 2020 2041 424f  ype  # 0.    ABO
+0000f1c0: 5254 3a20 4e6f 7469 6669 6361 7469 6f6e  RT: Notification
+0000f1d0: 2e41 6374 696f 6e2e 5661 6c75 6554 7970  .Action.ValueTyp
+0000f1e0: 6520 2023 2031 0a20 2020 2049 4e44 4558  e  # 1.    INDEX
+0000f1f0: 4544 3a20 4e6f 7469 6669 6361 7469 6f6e  ED: Notification
+0000f200: 2e41 6374 696f 6e2e 5661 6c75 6554 7970  .Action.ValueTyp
+0000f210: 6520 2023 2032 0a0a 2020 2020 636c 6173  e  # 2..    clas
+0000f220: 7320 5f57 7269 7465 5479 7065 3a0a 2020  s _WriteType:.  
+0000f230: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
+0000f240: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
+0000f250: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
+0000f260: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
+0000f270: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
+0000f280: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
+0000f290: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
+0000f2a0: 2020 2020 636c 6173 7320 5f57 7269 7465      class _Write
+0000f2b0: 5479 7065 456e 756d 5479 7065 5772 6170  TypeEnumTypeWrap
+0000f2c0: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
+0000f2d0: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
+0000f2e0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
+0000f2f0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
+0000f300: 4e6f 7469 6669 6361 7469 6f6e 2e5f 5772  Notification._Wr
+0000f310: 6974 6554 7970 652e 5661 6c75 6554 7970  iteType.ValueTyp
+0000f320: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
+0000f330: 6529 3a0a 2020 2020 2020 2020 4445 5343  e):.        DESC
+0000f340: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+0000f350: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+0000f360: 6f72 2e45 6e75 6d44 6573 6372 6970 746f  or.EnumDescripto
+0000f370: 720a 2020 2020 2020 2020 554e 5345 543a  r.        UNSET:
+0000f380: 204e 6f74 6966 6963 6174 696f 6e2e 5f57   Notification._W
+0000f390: 7269 7465 5479 7065 2e56 616c 7565 5479  riteType.ValueTy
+0000f3a0: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
+0000f3b0: 4352 4541 5445 443a 204e 6f74 6966 6963  CREATED: Notific
+0000f3c0: 6174 696f 6e2e 5f57 7269 7465 5479 7065  ation._WriteType
+0000f3d0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
+0000f3e0: 2020 2020 2020 2020 4d4f 4449 4649 4544          MODIFIED
+0000f3f0: 3a20 4e6f 7469 6669 6361 7469 6f6e 2e5f  : Notification._
+0000f400: 5772 6974 6554 7970 652e 5661 6c75 6554  WriteType.ValueT
+0000f410: 7970 6520 2023 2032 0a20 2020 2020 2020  ype  # 2.       
+0000f420: 2044 454c 4554 4544 3a20 4e6f 7469 6669   DELETED: Notifi
+0000f430: 6361 7469 6f6e 2e5f 5772 6974 6554 7970  cation._WriteTyp
+0000f440: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
+0000f450: 0a0a 2020 2020 636c 6173 7320 5772 6974  ..    class Writ
+0000f460: 6554 7970 6528 5f57 7269 7465 5479 7065  eType(_WriteType
+0000f470: 2c20 6d65 7461 636c 6173 733d 5f57 7269  , metaclass=_Wri
+0000f480: 7465 5479 7065 456e 756d 5479 7065 5772  teTypeEnumTypeWr
+0000f490: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
+0000f4a0: 554e 5345 543a 204e 6f74 6966 6963 6174  UNSET: Notificat
+0000f4b0: 696f 6e2e 5772 6974 6554 7970 652e 5661  ion.WriteType.Va
+0000f4c0: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
+0000f4d0: 2043 5245 4154 4544 3a20 4e6f 7469 6669   CREATED: Notifi
+0000f4e0: 6361 7469 6f6e 2e57 7269 7465 5479 7065  cation.WriteType
+0000f4f0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
+0000f500: 2020 2020 4d4f 4449 4649 4544 3a20 4e6f      MODIFIED: No
+0000f510: 7469 6669 6361 7469 6f6e 2e57 7269 7465  tification.Write
+0000f520: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
+0000f530: 2320 320a 2020 2020 4445 4c45 5445 443a  # 2.    DELETED:
+0000f540: 204e 6f74 6966 6963 6174 696f 6e2e 5772   Notification.Wr
+0000f550: 6974 6554 7970 652e 5661 6c75 6554 7970  iteType.ValueTyp
+0000f560: 6520 2023 2033 0a0a 2020 2020 5041 5254  e  # 3..    PART
+0000f570: 4954 494f 4e5f 4649 454c 445f 4e55 4d42  ITION_FIELD_NUMB
+0000f580: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000f590: 0a20 2020 204d 554c 5449 5f46 4945 4c44  .    MULTI_FIELD
+0000f5a0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+0000f5b0: 732e 696e 740a 2020 2020 5555 4944 5f46  s.int.    UUID_F
+0000f5c0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000f5d0: 6c74 696e 732e 696e 740a 2020 2020 4b42  ltins.int.    KB
+0000f5e0: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
+0000f5f0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000f600: 2020 5345 5149 445f 4649 454c 445f 4e55    SEQID_FIELD_NU
+0000f610: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+0000f620: 6e74 0a20 2020 2041 4354 494f 4e5f 4649  nt.    ACTION_FI
+0000f630: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+0000f640: 7469 6e73 2e69 6e74 0a20 2020 2057 5249  tins.int.    WRI
+0000f650: 5445 5f54 5950 455f 4649 454c 445f 4e55  TE_TYPE_FIELD_NU
+0000f660: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+0000f670: 6e74 0a20 2020 204d 4553 5341 4745 5f46  nt.    MESSAGE_F
+0000f680: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000f690: 6c74 696e 732e 696e 740a 2020 2020 534f  ltins.int.    SO
+0000f6a0: 5552 4345 5f46 4945 4c44 5f4e 554d 4245  URCE_FIELD_NUMBE
+0000f6b0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000f6c0: 2020 2020 5052 4f43 4553 5349 4e47 5f45      PROCESSING_E
+0000f6d0: 5252 4f52 535f 4649 454c 445f 4e55 4d42  RRORS_FIELD_NUMB
+0000f6e0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000f6f0: 0a20 2020 204d 4553 5341 4745 5f41 5544  .    MESSAGE_AUD
+0000f700: 4954 5f46 4945 4c44 5f4e 554d 4245 523a  IT_FIELD_NUMBER:
+0000f710: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000f720: 2020 7061 7274 6974 696f 6e3a 2062 7569    partition: bui
+0000f730: 6c74 696e 732e 696e 740a 2020 2020 6d75  ltins.int.    mu
+0000f740: 6c74 693a 2062 7569 6c74 696e 732e 7374  lti: builtins.st
+0000f750: 720a 2020 2020 7575 6964 3a20 6275 696c  r.    uuid: buil
+0000f760: 7469 6e73 2e73 7472 0a20 2020 206b 6269  tins.str.    kbi
+0000f770: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
+0000f780: 2020 2020 7365 7169 643a 2062 7569 6c74      seqid: built
+0000f790: 696e 732e 696e 740a 2020 2020 6163 7469  ins.int.    acti
+0000f7a0: 6f6e 3a20 676c 6f62 616c 5f5f 5f4e 6f74  on: global___Not
+0000f7b0: 6966 6963 6174 696f 6e2e 4163 7469 6f6e  ification.Action
+0000f7c0: 2e56 616c 7565 5479 7065 0a20 2020 2077  .ValueType.    w
+0000f7d0: 7269 7465 5f74 7970 653a 2067 6c6f 6261  rite_type: globa
+0000f7e0: 6c5f 5f5f 4e6f 7469 6669 6361 7469 6f6e  l___Notification
+0000f7f0: 2e57 7269 7465 5479 7065 2e56 616c 7565  .WriteType.Value
+0000f800: 5479 7065 0a20 2020 2073 6f75 7263 653a  Type.    source:
+0000f810: 2067 6c6f 6261 6c5f 5f5f 4e6f 7469 6669   global___Notifi
+0000f820: 6361 7469 6f6e 536f 7572 6365 2e56 616c  cationSource.Val
+0000f830: 7565 5479 7065 0a20 2020 2070 726f 6365  ueType.    proce
+0000f840: 7373 696e 675f 6572 726f 7273 3a20 6275  ssing_errors: bu
+0000f850: 696c 7469 6e73 2e62 6f6f 6c0a 2020 2020  iltins.bool.    
+0000f860: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000f870: 6620 6d65 7373 6167 6528 7365 6c66 2920  f message(self) 
+0000f880: 2d3e 2067 6c6f 6261 6c5f 5f5f 4272 6f6b  -> global___Brok
+0000f890: 6572 4d65 7373 6167 653a 202e 2e2e 0a20  erMessage: .... 
+0000f8a0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000f8b0: 2064 6566 206d 6573 7361 6765 5f61 7564   def message_aud
+0000f8c0: 6974 2873 656c 6629 202d 3e20 676c 6f62  it(self) -> glob
+0000f8d0: 616c 5f5f 5f41 7564 6974 3a20 2e2e 2e0a  al___Audit: ....
+0000f8e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000f8f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000f900: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000f910: 2020 2070 6172 7469 7469 6f6e 3a20 6275     partition: bu
+0000f920: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
+0000f930: 2c0a 2020 2020 2020 2020 6d75 6c74 693a  ,.        multi:
+0000f940: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+0000f950: 2e2e 2e2c 0a20 2020 2020 2020 2075 7569  ...,.        uui
+0000f960: 643a 2062 7569 6c74 696e 732e 7374 7220  d: builtins.str 
+0000f970: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206b  = ...,.        k
+0000f980: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
+0000f990: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+0000f9a0: 2073 6571 6964 3a20 6275 696c 7469 6e73   seqid: builtins
+0000f9b0: 2e69 6e74 203d 202e 2e2e 2c0a 2020 2020  .int = ...,.    
+0000f9c0: 2020 2020 6163 7469 6f6e 3a20 676c 6f62      action: glob
+0000f9d0: 616c 5f5f 5f4e 6f74 6966 6963 6174 696f  al___Notificatio
+0000f9e0: 6e2e 4163 7469 6f6e 2e56 616c 7565 5479  n.Action.ValueTy
+0000f9f0: 7065 203d 202e 2e2e 2c0a 2020 2020 2020  pe = ...,.      
+0000fa00: 2020 7772 6974 655f 7479 7065 3a20 676c    write_type: gl
+0000fa10: 6f62 616c 5f5f 5f4e 6f74 6966 6963 6174  obal___Notificat
+0000fa20: 696f 6e2e 5772 6974 6554 7970 652e 5661  ion.WriteType.Va
+0000fa30: 6c75 6554 7970 6520 3d20 2e2e 2e2c 0a20  lueType = ...,. 
+0000fa40: 2020 2020 2020 206d 6573 7361 6765 3a20         message: 
+0000fa50: 676c 6f62 616c 5f5f 5f42 726f 6b65 724d  global___BrokerM
+0000fa60: 6573 7361 6765 207c 204e 6f6e 6520 3d20  essage | None = 
+0000fa70: 2e2e 2e2c 0a20 2020 2020 2020 2073 6f75  ...,.        sou
+0000fa80: 7263 653a 2067 6c6f 6261 6c5f 5f5f 4e6f  rce: global___No
+0000fa90: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
+0000faa0: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
+0000fab0: 2c0a 2020 2020 2020 2020 7072 6f63 6573  ,.        proces
+0000fac0: 7369 6e67 5f65 7272 6f72 733a 2062 7569  sing_errors: bui
+0000fad0: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
+0000fae0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+0000faf0: 655f 6175 6469 743a 2067 6c6f 6261 6c5f  e_audit: global_
+0000fb00: 5f5f 4175 6469 7420 7c20 4e6f 6e65 203d  __Audit | None =
+0000fb10: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+0000fb20: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+0000fb30: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+0000fb40: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+0000fb50: 6e67 2e4c 6974 6572 616c 5b22 6d65 7373  ng.Literal["mess
+0000fb60: 6167 6522 2c20 6222 6d65 7373 6167 6522  age", b"message"
+0000fb70: 2c20 226d 6573 7361 6765 5f61 7564 6974  , "message_audit
+0000fb80: 222c 2062 226d 6573 7361 6765 5f61 7564  ", b"message_aud
+0000fb90: 6974 225d 2920 2d3e 2062 7569 6c74 696e  it"]) -> builtin
+0000fba0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+0000fbb0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+0000fbc0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000fbd0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000fbe0: 2261 6374 696f 6e22 2c20 6222 6163 7469  "action", b"acti
+0000fbf0: 6f6e 222c 2022 6b62 6964 222c 2062 226b  on", "kbid", b"k
+0000fc00: 6269 6422 2c20 226d 6573 7361 6765 222c  bid", "message",
+0000fc10: 2062 226d 6573 7361 6765 222c 2022 6d65   b"message", "me
+0000fc20: 7373 6167 655f 6175 6469 7422 2c20 6222  ssage_audit", b"
+0000fc30: 6d65 7373 6167 655f 6175 6469 7422 2c20  message_audit", 
+0000fc40: 226d 756c 7469 222c 2062 226d 756c 7469  "multi", b"multi
+0000fc50: 222c 2022 7061 7274 6974 696f 6e22 2c20  ", "partition", 
+0000fc60: 6222 7061 7274 6974 696f 6e22 2c20 2270  b"partition", "p
+0000fc70: 726f 6365 7373 696e 675f 6572 726f 7273  rocessing_errors
+0000fc80: 222c 2062 2270 726f 6365 7373 696e 675f  ", b"processing_
+0000fc90: 6572 726f 7273 222c 2022 7365 7169 6422  errors", "seqid"
+0000fca0: 2c20 6222 7365 7169 6422 2c20 2273 6f75  , b"seqid", "sou
+0000fcb0: 7263 6522 2c20 6222 736f 7572 6365 222c  rce", b"source",
+0000fcc0: 2022 7575 6964 222c 2062 2275 7569 6422   "uuid", b"uuid"
+0000fcd0: 2c20 2277 7269 7465 5f74 7970 6522 2c20  , "write_type", 
+0000fce0: 6222 7772 6974 655f 7479 7065 225d 2920  b"write_type"]) 
+0000fcf0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
+0000fd00: 6f62 616c 5f5f 5f4e 6f74 6966 6963 6174  obal___Notificat
+0000fd10: 696f 6e20 3d20 4e6f 7469 6669 6361 7469  ion = Notificati
+0000fd20: 6f6e 0a0a 4074 7970 696e 672e 6669 6e61  on..@typing.fina
+0000fd30: 6c0a 636c 6173 7320 4d65 6d62 6572 2867  l.class Member(g
+0000fd40: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
+0000fd50: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
+0000fd60: 0a20 2020 2022 2222 5468 6520 6d65 6d62  .    """The memb
+0000fd70: 6572 2069 6e66 6f72 6d61 7469 6f6e 2e22  er information."
+0000fd80: 2222 0a0a 2020 2020 4445 5343 5249 5054  ""..    DESCRIPT
+0000fd90: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000fda0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000fdb0: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
+0000fdc0: 6c61 7373 205f 5479 7065 3a0a 2020 2020  lass _Type:.    
+0000fdd0: 2020 2020 5661 6c75 6554 7970 6520 3d20      ValueType = 
+0000fde0: 7479 7069 6e67 2e4e 6577 5479 7065 2822  typing.NewType("
+0000fdf0: 5661 6c75 6554 7970 6522 2c20 6275 696c  ValueType", buil
+0000fe00: 7469 6e73 2e69 6e74 290a 2020 2020 2020  tins.int).      
+0000fe10: 2020 563a 2074 7970 696e 675f 6578 7465    V: typing_exte
+0000fe20: 6e73 696f 6e73 2e54 7970 6541 6c69 6173  nsions.TypeAlias
+0000fe30: 203d 2056 616c 7565 5479 7065 0a0a 2020   = ValueType..  
+0000fe40: 2020 636c 6173 7320 5f54 7970 6545 6e75    class _TypeEnu
+0000fe50: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
+0000fe60: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+0000fe70: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
+0000fe80: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
+0000fe90: 6557 7261 7070 6572 5b4d 656d 6265 722e  eWrapper[Member.
+0000fea0: 5f54 7970 652e 5661 6c75 6554 7970 655d  _Type.ValueType]
+0000feb0: 2c20 6275 696c 7469 6e73 2e74 7970 6529  , builtins.type)
+0000fec0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
+0000fed0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+0000fee0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+0000fef0: 2e45 6e75 6d44 6573 6372 6970 746f 720a  .EnumDescriptor.
+0000ff00: 2020 2020 2020 2020 494f 3a20 4d65 6d62          IO: Memb
+0000ff10: 6572 2e5f 5479 7065 2e56 616c 7565 5479  er._Type.ValueTy
+0000ff20: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
+0000ff30: 5345 4152 4348 3a20 4d65 6d62 6572 2e5f  SEARCH: Member._
+0000ff40: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
+0000ff50: 2320 310a 2020 2020 2020 2020 494e 4745  # 1.        INGE
+0000ff60: 5354 3a20 4d65 6d62 6572 2e5f 5479 7065  ST: Member._Type
+0000ff70: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+0000ff80: 2020 2020 2020 2020 5452 4149 4e3a 204d          TRAIN: M
+0000ff90: 656d 6265 722e 5f54 7970 652e 5661 6c75  ember._Type.Valu
+0000ffa0: 6554 7970 6520 2023 2033 0a20 2020 2020  eType  # 3.     
+0000ffb0: 2020 2055 4e4b 4e4f 574e 3a20 4d65 6d62     UNKNOWN: Memb
+0000ffc0: 6572 2e5f 5479 7065 2e56 616c 7565 5479  er._Type.ValueTy
+0000ffd0: 7065 2020 2320 340a 0a20 2020 2063 6c61  pe  # 4..    cla
+0000ffe0: 7373 2054 7970 6528 5f54 7970 652c 206d  ss Type(_Type, m
+0000fff0: 6574 6163 6c61 7373 3d5f 5479 7065 456e  etaclass=_TypeEn
+00010000: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
+00010010: 2e2e 2e0a 2020 2020 494f 3a20 4d65 6d62  ....    IO: Memb
+00010020: 6572 2e54 7970 652e 5661 6c75 6554 7970  er.Type.ValueTyp
+00010030: 6520 2023 2030 0a20 2020 2053 4541 5243  e  # 0.    SEARC
+00010040: 483a 204d 656d 6265 722e 5479 7065 2e56  H: Member.Type.V
+00010050: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
+00010060: 2020 494e 4745 5354 3a20 4d65 6d62 6572    INGEST: Member
+00010070: 2e54 7970 652e 5661 6c75 6554 7970 6520  .Type.ValueType 
+00010080: 2023 2032 0a20 2020 2054 5241 494e 3a20   # 2.    TRAIN: 
+00010090: 4d65 6d62 6572 2e54 7970 652e 5661 6c75  Member.Type.Valu
+000100a0: 6554 7970 6520 2023 2033 0a20 2020 2055  eType  # 3.    U
+000100b0: 4e4b 4e4f 574e 3a20 4d65 6d62 6572 2e54  NKNOWN: Member.T
+000100c0: 7970 652e 5661 6c75 6554 7970 6520 2023  ype.ValueType  #
+000100d0: 2034 0a0a 2020 2020 4944 5f46 4945 4c44   4..    ID_FIELD
+000100e0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+000100f0: 732e 696e 740a 2020 2020 4c49 5354 454e  s.int.    LISTEN
+00010100: 5f41 4444 5245 5353 5f46 4945 4c44 5f4e  _ADDRESS_FIELD_N
+00010110: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00010120: 696e 740a 2020 2020 4953 5f53 454c 465f  int.    IS_SELF_
+00010130: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00010140: 696c 7469 6e73 2e69 6e74 0a20 2020 2054  iltins.int.    T
+00010150: 5950 455f 4649 454c 445f 4e55 4d42 4552  YPE_FIELD_NUMBER
+00010160: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00010170: 2020 2044 554d 4d59 5f46 4945 4c44 5f4e     DUMMY_FIELD_N
+00010180: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00010190: 696e 740a 2020 2020 4c4f 4144 5f53 434f  int.    LOAD_SCO
+000101a0: 5245 5f46 4945 4c44 5f4e 554d 4245 523a  RE_FIELD_NUMBER:
+000101b0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+000101c0: 2020 5348 4152 445f 434f 554e 545f 4649    SHARD_COUNT_FI
+000101d0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000101e0: 7469 6e73 2e69 6e74 0a20 2020 2050 5249  tins.int.    PRI
+000101f0: 4d41 5259 5f49 445f 4649 454c 445f 4e55  MARY_ID_FIELD_NU
+00010200: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00010210: 6e74 0a20 2020 2069 643a 2062 7569 6c74  nt.    id: built
+00010220: 696e 732e 7374 720a 2020 2020 2222 222f  ins.str.    """/
+00010230: 204d 656d 6265 7220 4944 2ee3 8080 4120   Member ID....A 
+00010240: 7374 7269 6e67 206f 6620 7468 6520 5555  string of the UU
+00010250: 4944 2e22 2222 0a20 2020 206c 6973 7465  ID.""".    liste
+00010260: 6e5f 6164 6472 6573 733a 2062 7569 6c74  n_address: built
+00010270: 696e 732e 7374 720a 2020 2020 2222 222f  ins.str.    """/
+00010280: 2043 6c75 7374 6572 206c 6973 7465 6e20   Cluster listen 
+00010290: 6164 6472 6573 732e 2073 7472 696e 6720  address. string 
+000102a0: 6f66 2049 5020 616e 6420 706f 7274 206e  of IP and port n
+000102b0: 756d 6265 722e 0a20 2020 202f 2045 2e67  umber..    / E.g
+000102c0: 2e20 3132 372e 302e 302e 313a 3530 3030  . 127.0.0.1:5000
+000102d0: 0a20 2020 2022 2222 0a20 2020 2069 735f  .    """.    is_
+000102e0: 7365 6c66 3a20 6275 696c 7469 6e73 2e62  self: builtins.b
+000102f0: 6f6f 6c0a 2020 2020 2222 222f 2049 6620  ool.    """/ If 
+00010300: 7472 7565 2c20 6974 206d 6561 6e73 2073  true, it means s
+00010310: 656c 662e 2222 220a 2020 2020 7479 7065  elf.""".    type
+00010320: 3a20 676c 6f62 616c 5f5f 5f4d 656d 6265  : global___Membe
+00010330: 722e 5479 7065 2e56 616c 7565 5479 7065  r.Type.ValueType
+00010340: 0a20 2020 2022 2222 2f20 496f 2c20 496e  .    """/ Io, In
+00010350: 6765 7374 2c20 5365 6172 6368 2c20 5472  gest, Search, Tr
+00010360: 6169 6e2e 2222 220a 2020 2020 6475 6d6d  ain.""".    dumm
+00010370: 793a 2062 7569 6c74 696e 732e 626f 6f6c  y: builtins.bool
+00010380: 0a20 2020 2022 2222 2f20 4475 6d6d 7920  .    """/ Dummy 
+00010390: 4d65 6d62 6572 2222 220a 2020 2020 6c6f  Member""".    lo
+000103a0: 6164 5f73 636f 7265 3a20 6275 696c 7469  ad_score: builti
+000103b0: 6e73 2e66 6c6f 6174 0a20 2020 2022 2222  ns.float.    """
+000103c0: 2f20 5468 6520 6c6f 6164 2073 636f 7265  / The load score
+000103d0: 206f 6620 7468 6520 6d65 6d62 6572 2e22   of the member."
+000103e0: 2222 0a20 2020 2073 6861 7264 5f63 6f75  "".    shard_cou
+000103f0: 6e74 3a20 6275 696c 7469 6e73 2e69 6e74  nt: builtins.int
+00010400: 0a20 2020 2022 2222 2f20 5468 6520 6e75  .    """/ The nu
+00010410: 6d62 6572 206f 6620 7368 6172 6473 2069  mber of shards i
+00010420: 6e20 7468 6520 6e6f 6465 2e22 2222 0a20  n the node.""". 
+00010430: 2020 2070 7269 6d61 7279 5f69 643a 2062     primary_id: b
+00010440: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+00010450: 2222 222f 2054 6865 2069 6420 6f66 2074  """/ The id of t
+00010460: 6865 2070 7269 6d61 7279 206e 6f64 6520  he primary node 
+00010470: 2869 6620 6974 2069 7320 6120 7365 636f  (if it is a seco
+00010480: 6e64 6172 7920 6e6f 6465 292e 2222 220a  ndary node).""".
+00010490: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000104a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000104b0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000104c0: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
+000104d0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+000104e0: 2020 206c 6973 7465 6e5f 6164 6472 6573     listen_addres
+000104f0: 733a 2062 7569 6c74 696e 732e 7374 7220  s: builtins.str 
+00010500: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2069  = ...,.        i
+00010510: 735f 7365 6c66 3a20 6275 696c 7469 6e73  s_self: builtins
+00010520: 2e62 6f6f 6c20 3d20 2e2e 2e2c 0a20 2020  .bool = ...,.   
+00010530: 2020 2020 2074 7970 653a 2067 6c6f 6261       type: globa
+00010540: 6c5f 5f5f 4d65 6d62 6572 2e54 7970 652e  l___Member.Type.
+00010550: 5661 6c75 6554 7970 6520 3d20 2e2e 2e2c  ValueType = ...,
+00010560: 0a20 2020 2020 2020 2064 756d 6d79 3a20  .        dummy: 
+00010570: 6275 696c 7469 6e73 2e62 6f6f 6c20 3d20  builtins.bool = 
+00010580: 2e2e 2e2c 0a20 2020 2020 2020 206c 6f61  ...,.        loa
+00010590: 645f 7363 6f72 653a 2062 7569 6c74 696e  d_score: builtin
+000105a0: 732e 666c 6f61 7420 3d20 2e2e 2e2c 0a20  s.float = ...,. 
+000105b0: 2020 2020 2020 2073 6861 7264 5f63 6f75         shard_cou
+000105c0: 6e74 3a20 6275 696c 7469 6e73 2e69 6e74  nt: builtins.int
+000105d0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+000105e0: 7072 696d 6172 795f 6964 3a20 6275 696c  primary_id: buil
+000105f0: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+00010600: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+00010610: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
+00010620: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+00010630: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+00010640: 6974 6572 616c 5b22 6475 6d6d 7922 2c20  iteral["dummy", 
+00010650: 6222 6475 6d6d 7922 2c20 2269 6422 2c20  b"dummy", "id", 
+00010660: 6222 6964 222c 2022 6973 5f73 656c 6622  b"id", "is_self"
+00010670: 2c20 6222 6973 5f73 656c 6622 2c20 226c  , b"is_self", "l
+00010680: 6973 7465 6e5f 6164 6472 6573 7322 2c20  isten_address", 
+00010690: 6222 6c69 7374 656e 5f61 6464 7265 7373  b"listen_address
+000106a0: 222c 2022 6c6f 6164 5f73 636f 7265 222c  ", "load_score",
+000106b0: 2062 226c 6f61 645f 7363 6f72 6522 2c20   b"load_score", 
+000106c0: 2270 7269 6d61 7279 5f69 6422 2c20 6222  "primary_id", b"
+000106d0: 7072 696d 6172 795f 6964 222c 2022 7368  primary_id", "sh
+000106e0: 6172 645f 636f 756e 7422 2c20 6222 7368  ard_count", b"sh
+000106f0: 6172 645f 636f 756e 7422 2c20 2274 7970  ard_count", "typ
+00010700: 6522 2c20 6222 7479 7065 225d 2920 2d3e  e", b"type"]) ->
+00010710: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+00010720: 616c 5f5f 5f4d 656d 6265 7220 3d20 4d65  al___Member = Me
+00010730: 6d62 6572 0a0a 4074 7970 696e 672e 6669  mber..@typing.fi
+00010740: 6e61 6c0a 636c 6173 7320 4c69 7374 4d65  nal.class ListMe
+00010750: 6d62 6572 7352 6571 7565 7374 2867 6f6f  mbersRequest(goo
+00010760: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+00010770: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+00010780: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00010790: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+000107a0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+000107b0: 7074 6f72 0a0a 2020 2020 6465 6620 5f5f  ptor..    def __
+000107c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000107d0: 7365 6c66 2c0a 2020 2020 2920 2d3e 204e  self,.    ) -> N
+000107e0: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
+000107f0: 5f5f 5f4c 6973 744d 656d 6265 7273 5265  ___ListMembersRe
+00010800: 7175 6573 7420 3d20 4c69 7374 4d65 6d62  quest = ListMemb
+00010810: 6572 7352 6571 7565 7374 0a0a 4074 7970  ersRequest..@typ
+00010820: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+00010830: 4c69 7374 4d65 6d62 6572 7352 6573 706f  ListMembersRespo
+00010840: 6e73 6528 676f 6f67 6c65 2e70 726f 746f  nse(google.proto
+00010850: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
+00010860: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
+00010870: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+00010880: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+00010890: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+000108a0: 204d 454d 4245 5253 5f46 4945 4c44 5f4e   MEMBERS_FIELD_N
+000108b0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+000108c0: 696e 740a 2020 2020 4070 726f 7065 7274  int.    @propert
+000108d0: 790a 2020 2020 6465 6620 6d65 6d62 6572  y.    def member
+000108e0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
+000108f0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+00010900: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
+00010910: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
+00010920: 4669 656c 6443 6f6e 7461 696e 6572 5b67  FieldContainer[g
+00010930: 6c6f 6261 6c5f 5f5f 4d65 6d62 6572 5d3a  lobal___Member]:
+00010940: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
+00010950: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00010960: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+00010970: 2020 2020 2020 2020 6d65 6d62 6572 733a          members:
+00010980: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00010990: 2e49 7465 7261 626c 655b 676c 6f62 616c  .Iterable[global
+000109a0: 5f5f 5f4d 656d 6265 725d 207c 204e 6f6e  ___Member] | Non
+000109b0: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+000109c0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+000109d0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+000109e0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+000109f0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00010a00: 226d 656d 6265 7273 222c 2062 226d 656d  "members", b"mem
+00010a10: 6265 7273 225d 2920 2d3e 204e 6f6e 653a  bers"]) -> None:
+00010a20: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f4c   .....global___L
+00010a30: 6973 744d 656d 6265 7273 5265 7370 6f6e  istMembersRespon
+00010a40: 7365 203d 204c 6973 744d 656d 6265 7273  se = ListMembers
+00010a50: 5265 7370 6f6e 7365 0a0a 4074 7970 696e  Response..@typin
+00010a60: 672e 6669 6e61 6c0a 636c 6173 7320 5368  g.final.class Sh
+00010a70: 6172 6452 6570 6c69 6361 2867 6f6f 676c  ardReplica(googl
+00010a80: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00010a90: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00010aa0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+00010ab0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+00010ac0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+00010ad0: 6f72 0a0a 2020 2020 5348 4152 445f 4649  or..    SHARD_FI
+00010ae0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00010af0: 7469 6e73 2e69 6e74 0a20 2020 204e 4f44  tins.int.    NOD
+00010b00: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
+00010b10: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00010b20: 206e 6f64 653a 2062 7569 6c74 696e 732e   node: builtins.
+00010b30: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
+00010b40: 790a 2020 2020 6465 6620 7368 6172 6428  y.    def shard(
+00010b50: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+00010b60: 625f 7072 6f74 6f73 2e6e 6f64 6572 6573  b_protos.noderes
+00010b70: 6f75 7263 6573 5f70 6232 2e53 6861 7264  ources_pb2.Shard
+00010b80: 4372 6561 7465 643a 202e 2e2e 0a20 2020  Created: ....   
+00010b90: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00010ba0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00010bb0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00010bc0: 7368 6172 643a 206e 7563 6c69 6164 625f  shard: nucliadb_
+00010bd0: 7072 6f74 6f73 2e6e 6f64 6572 6573 6f75  protos.noderesou
+00010be0: 7263 6573 5f70 6232 2e53 6861 7264 4372  rces_pb2.ShardCr
+00010bf0: 6561 7465 6420 7c20 4e6f 6e65 203d 202e  eated | None = .
+00010c00: 2e2e 2c0a 2020 2020 2020 2020 6e6f 6465  ..,.        node
+00010c10: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00010c20: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+00010c30: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+00010c40: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+00010c50: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00010c60: 6e67 2e4c 6974 6572 616c 5b22 7368 6172  ng.Literal["shar
+00010c70: 6422 2c20 6222 7368 6172 6422 5d29 202d  d", b"shard"]) -
+00010c80: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
+00010c90: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
+00010ca0: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+00010cb0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+00010cc0: 2e4c 6974 6572 616c 5b22 6e6f 6465 222c  .Literal["node",
+00010cd0: 2062 226e 6f64 6522 2c20 2273 6861 7264   b"node", "shard
+00010ce0: 222c 2062 2273 6861 7264 225d 2920 2d3e  ", b"shard"]) ->
+00010cf0: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+00010d00: 616c 5f5f 5f53 6861 7264 5265 706c 6963  al___ShardReplic
+00010d10: 6120 3d20 5368 6172 6452 6570 6c69 6361  a = ShardReplica
+00010d20: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
+00010d30: 636c 6173 7320 5368 6172 644f 626a 6563  class ShardObjec
+00010d40: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
+00010d50: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+00010d60: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+00010d70: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+00010d80: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+00010d90: 6573 6372 6970 746f 720a 0a20 2020 2053  escriptor..    S
+00010da0: 4841 5244 5f46 4945 4c44 5f4e 554d 4245  HARD_FIELD_NUMBE
+00010db0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00010dc0: 2020 2020 5245 504c 4943 4153 5f46 4945      REPLICAS_FIE
+00010dd0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00010de0: 696e 732e 696e 740a 2020 2020 5449 4d45  ins.int.    TIME
+00010df0: 5354 414d 505f 4649 454c 445f 4e55 4d42  STAMP_FIELD_NUMB
+00010e00: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00010e10: 0a20 2020 2052 4541 445f 4f4e 4c59 5f46  .    READ_ONLY_F
+00010e20: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00010e30: 6c74 696e 732e 696e 740a 2020 2020 7368  ltins.int.    sh
+00010e40: 6172 643a 2062 7569 6c74 696e 732e 7374  ard: builtins.st
+00010e50: 720a 2020 2020 7265 6164 5f6f 6e6c 793a  r.    read_only:
+00010e60: 2062 7569 6c74 696e 732e 626f 6f6c 0a20   builtins.bool. 
+00010e70: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00010e80: 2064 6566 2072 6570 6c69 6361 7328 7365   def replicas(se
+00010e90: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
+00010ea0: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
+00010eb0: 636f 6e74 6169 6e65 7273 2e52 6570 6561  containers.Repea
+00010ec0: 7465 6443 6f6d 706f 7369 7465 4669 656c  tedCompositeFiel
+00010ed0: 6443 6f6e 7461 696e 6572 5b67 6c6f 6261  dContainer[globa
+00010ee0: 6c5f 5f5f 5368 6172 6452 6570 6c69 6361  l___ShardReplica
+00010ef0: 5d3a 202e 2e2e 0a20 2020 2040 7072 6f70  ]: ....    @prop
+00010f00: 6572 7479 0a20 2020 2064 6566 2074 696d  erty.    def tim
+00010f10: 6573 7461 6d70 2873 656c 6629 202d 3e20  estamp(self) -> 
+00010f20: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00010f30: 7469 6d65 7374 616d 705f 7062 322e 5469  timestamp_pb2.Ti
+00010f40: 6d65 7374 616d 703a 202e 2e2e 0a20 2020  mestamp: ....   
+00010f50: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00010f60: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00010f70: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00010f80: 7368 6172 643a 2062 7569 6c74 696e 732e  shard: builtins.
+00010f90: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+00010fa0: 2020 2072 6570 6c69 6361 733a 2063 6f6c     replicas: col
+00010fb0: 6c65 6374 696f 6e73 2e61 6263 2e49 7465  lections.abc.Ite
+00010fc0: 7261 626c 655b 676c 6f62 616c 5f5f 5f53  rable[global___S
+00010fd0: 6861 7264 5265 706c 6963 615d 207c 204e  hardReplica] | N
+00010fe0: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+00010ff0: 2020 2074 696d 6573 7461 6d70 3a20 676f     timestamp: go
+00011000: 6f67 6c65 2e70 726f 746f 6275 662e 7469  ogle.protobuf.ti
+00011010: 6d65 7374 616d 705f 7062 322e 5469 6d65  mestamp_pb2.Time
+00011020: 7374 616d 7020 7c20 4e6f 6e65 203d 202e  stamp | None = .
+00011030: 2e2e 2c0a 2020 2020 2020 2020 7265 6164  ..,.        read
+00011040: 5f6f 6e6c 793a 2062 7569 6c74 696e 732e  _only: builtins.
+00011050: 626f 6f6c 203d 202e 2e2e 2c0a 2020 2020  bool = ...,.    
+00011060: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00011070: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
+00011080: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+00011090: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+000110a0: 5b22 7469 6d65 7374 616d 7022 2c20 6222  ["timestamp", b"
+000110b0: 7469 6d65 7374 616d 7022 5d29 202d 3e20  timestamp"]) -> 
+000110c0: 6275 696c 7469 6e73 2e62 6f6f 6c3a 202e  builtins.bool: .
+000110d0: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
+000110e0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+000110f0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+00011100: 6974 6572 616c 5b22 7265 6164 5f6f 6e6c  iteral["read_onl
+00011110: 7922 2c20 6222 7265 6164 5f6f 6e6c 7922  y", b"read_only"
+00011120: 2c20 2272 6570 6c69 6361 7322 2c20 6222  , "replicas", b"
+00011130: 7265 706c 6963 6173 222c 2022 7368 6172  replicas", "shar
+00011140: 6422 2c20 6222 7368 6172 6422 2c20 2274  d", b"shard", "t
+00011150: 696d 6573 7461 6d70 222c 2062 2274 696d  imestamp", b"tim
+00011160: 6573 7461 6d70 225d 2920 2d3e 204e 6f6e  estamp"]) -> Non
+00011170: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+00011180: 5f53 6861 7264 4f62 6a65 6374 203d 2053  _ShardObject = S
+00011190: 6861 7264 4f62 6a65 6374 0a0a 4074 7970  hardObject..@typ
+000111a0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+000111b0: 5368 6172 6473 2867 6f6f 676c 652e 7072  Shards(google.pr
+000111c0: 6f74 6f62 7566 2e6d 6573 7361 6765 2e4d  otobuf.message.M
+000111d0: 6573 7361 6765 293a 0a20 2020 2044 4553  essage):.    DES
+000111e0: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+000111f0: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+00011200: 746f 722e 4465 7363 7269 7074 6f72 0a0a  tor.Descriptor..
+00011210: 2020 2020 4074 7970 696e 672e 6669 6e61      @typing.fina
+00011220: 6c0a 2020 2020 636c 6173 7320 4578 7472  l.    class Extr
+00011230: 6145 6e74 7279 2867 6f6f 676c 652e 7072  aEntry(google.pr
+00011240: 6f74 6f62 7566 2e6d 6573 7361 6765 2e4d  otobuf.message.M
+00011250: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
+00011260: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+00011270: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+00011280: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+00011290: 6f72 0a0a 2020 2020 2020 2020 4b45 595f  or..        KEY_
+000112a0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+000112b0: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
+000112c0: 2020 2056 414c 5545 5f46 4945 4c44 5f4e     VALUE_FIELD_N
+000112d0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+000112e0: 696e 740a 2020 2020 2020 2020 6b65 793a  int.        key:
+000112f0: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
+00011300: 2020 2020 2020 7661 6c75 653a 2062 7569        value: bui
+00011310: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
+00011320: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00011330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011340: 2c0a 2020 2020 2020 2020 2020 2020 2a2c  ,.            *,
+00011350: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+00011360: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00011370: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00011380: 2020 7661 6c75 653a 2062 7569 6c74 696e    value: builtin
+00011390: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+000113a0: 2020 2020 2029 202d 3e20 4e6f 6e65 3a20       ) -> None: 
+000113b0: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
+000113c0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
+000113d0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+000113e0: 696e 672e 4c69 7465 7261 6c5b 226b 6579  ing.Literal["key
+000113f0: 222c 2062 226b 6579 222c 2022 7661 6c75  ", b"key", "valu
+00011400: 6522 2c20 6222 7661 6c75 6522 5d29 202d  e", b"value"]) -
+00011410: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020  > None: .....   
+00011420: 2053 4841 5244 535f 4649 454c 445f 4e55   SHARDS_FIELD_NU
+00011430: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00011440: 6e74 0a20 2020 204b 4249 445f 4649 454c  nt.    KBID_FIEL
+00011450: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00011460: 6e73 2e69 6e74 0a20 2020 2041 4354 5541  ns.int.    ACTUA
+00011470: 4c5f 4649 454c 445f 4e55 4d42 4552 3a20  L_FIELD_NUMBER: 
+00011480: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00011490: 2053 494d 494c 4152 4954 595f 4649 454c   SIMILARITY_FIEL
+000114a0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+000114b0: 6e73 2e69 6e74 0a20 2020 204d 4f44 454c  ns.int.    MODEL
+000114c0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+000114d0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000114e0: 5245 4c45 4153 455f 4348 414e 4e45 4c5f  RELEASE_CHANNEL_
+000114f0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00011500: 696c 7469 6e73 2e69 6e74 0a20 2020 2045  iltins.int.    E
+00011510: 5854 5241 5f46 4945 4c44 5f4e 554d 4245  XTRA_FIELD_NUMBE
+00011520: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00011530: 2020 2020 6b62 6964 3a20 6275 696c 7469      kbid: builti
+00011540: 6e73 2e73 7472 0a20 2020 2061 6374 7561  ns.str.    actua
+00011550: 6c3a 2062 7569 6c74 696e 732e 696e 740a  l: builtins.int.
+00011560: 2020 2020 2222 2244 4550 5245 4341 5445      """DEPRECATE
+00011570: 4420 6120 4b42 206b 6e6f 7720 6361 6e20  D a KB know can 
+00011580: 6861 7665 206d 756c 7469 706c 6520 616c  have multiple al
+00011590: 6976 6520 7368 6172 6473 2061 6e64 2069  ive shards and i
+000115a0: 7320 7472 6163 6b65 6420 696e 0a20 2020  s tracked in.   
+000115b0: 2065 6163 6820 5368 6172 644f 626a 6563   each ShardObjec
+000115c0: 740a 2020 2020 2222 220a 2020 2020 7369  t.    """.    si
+000115d0: 6d69 6c61 7269 7479 3a20 6e75 636c 6961  milarity: nuclia
+000115e0: 6462 5f70 726f 746f 732e 7574 696c 735f  db_protos.utils_
+000115f0: 7062 322e 5665 6374 6f72 5369 6d69 6c61  pb2.VectorSimila
+00011600: 7269 7479 2e56 616c 7565 5479 7065 0a20  rity.ValueType. 
+00011610: 2020 2022 2222 4445 5052 4543 4154 4544     """DEPRECATED
+00011620: 2069 6e20 6661 766f 7220 6f66 2060 6d6f   in favor of `mo
+00011630: 6465 6c60 2074 6f20 696e 636c 7564 6520  del` to include 
+00011640: 6d6f 7265 2064 6174 6122 2222 0a20 2020  more data""".   
+00011650: 2072 656c 6561 7365 5f63 6861 6e6e 656c   release_channel
+00011660: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00011670: 732e 7574 696c 735f 7062 322e 5265 6c65  s.utils_pb2.Rele
+00011680: 6173 6543 6861 6e6e 656c 2e56 616c 7565  aseChannel.Value
+00011690: 5479 7065 0a20 2020 2040 7072 6f70 6572  Type.    @proper
+000116a0: 7479 0a20 2020 2064 6566 2073 6861 7264  ty.    def shard
+000116b0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
+000116c0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+000116d0: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
+000116e0: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
+000116f0: 4669 656c 6443 6f6e 7461 696e 6572 5b67  FieldContainer[g
+00011700: 6c6f 6261 6c5f 5f5f 5368 6172 644f 626a  lobal___ShardObj
+00011710: 6563 745d 3a20 2e2e 2e0a 2020 2020 4070  ect]: ....    @p
+00011720: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00011730: 6d6f 6465 6c28 7365 6c66 2920 2d3e 206e  model(self) -> n
+00011740: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+00011750: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+00011760: 5365 6d61 6e74 6963 4d6f 6465 6c4d 6574  SemanticModelMet
+00011770: 6164 6174 613a 202e 2e2e 0a20 2020 2040  adata: ....    @
+00011780: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00011790: 2065 7874 7261 2873 656c 6629 202d 3e20   extra(self) -> 
+000117a0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+000117b0: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
+000117c0: 6572 732e 5363 616c 6172 4d61 705b 6275  ers.ScalarMap[bu
+000117d0: 696c 7469 6e73 2e73 7472 2c20 6275 696c  iltins.str, buil
+000117e0: 7469 6e73 2e73 7472 5d3a 202e 2e2e 0a20  tins.str]: .... 
+000117f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00011800: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00011810: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00011820: 2020 7368 6172 6473 3a20 636f 6c6c 6563    shards: collec
+00011830: 7469 6f6e 732e 6162 632e 4974 6572 6162  tions.abc.Iterab
+00011840: 6c65 5b67 6c6f 6261 6c5f 5f5f 5368 6172  le[global___Shar
+00011850: 644f 626a 6563 745d 207c 204e 6f6e 6520  dObject] | None 
+00011860: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206b  = ...,.        k
+00011870: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
+00011880: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+00011890: 2061 6374 7561 6c3a 2062 7569 6c74 696e   actual: builtin
+000118a0: 732e 696e 7420 3d20 2e2e 2e2c 0a20 2020  s.int = ...,.   
+000118b0: 2020 2020 2073 696d 696c 6172 6974 793a       similarity:
+000118c0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+000118d0: 2e75 7469 6c73 5f70 6232 2e56 6563 746f  .utils_pb2.Vecto
+000118e0: 7253 696d 696c 6172 6974 792e 5661 6c75  rSimilarity.Valu
+000118f0: 6554 7970 6520 3d20 2e2e 2e2c 0a20 2020  eType = ...,.   
+00011900: 2020 2020 206d 6f64 656c 3a20 6e75 636c       model: nucl
+00011910: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+00011920: 6c65 6467 6562 6f78 5f70 6232 2e53 656d  ledgebox_pb2.Sem
+00011930: 616e 7469 634d 6f64 656c 4d65 7461 6461  anticModelMetada
+00011940: 7461 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ta | None = ...,
+00011950: 0a20 2020 2020 2020 2072 656c 6561 7365  .        release
+00011960: 5f63 6861 6e6e 656c 3a20 6e75 636c 6961  _channel: nuclia
+00011970: 6462 5f70 726f 746f 732e 7574 696c 735f  db_protos.utils_
+00011980: 7062 322e 5265 6c65 6173 6543 6861 6e6e  pb2.ReleaseChann
+00011990: 656c 2e56 616c 7565 5479 7065 203d 202e  el.ValueType = .
+000119a0: 2e2e 2c0a 2020 2020 2020 2020 6578 7472  ..,.        extr
+000119b0: 613a 2063 6f6c 6c65 6374 696f 6e73 2e61  a: collections.a
+000119c0: 6263 2e4d 6170 7069 6e67 5b62 7569 6c74  bc.Mapping[built
+000119d0: 696e 732e 7374 722c 2062 7569 6c74 696e  ins.str, builtin
+000119e0: 732e 7374 725d 207c 204e 6f6e 6520 3d20  s.str] | None = 
+000119f0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
+00011a00: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+00011a10: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
+00011a20: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00011a30: 672e 4c69 7465 7261 6c5b 226d 6f64 656c  g.Literal["model
+00011a40: 222c 2062 226d 6f64 656c 225d 2920 2d3e  ", b"model"]) ->
+00011a50: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+00011a60: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00011a70: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00011a80: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00011a90: 4c69 7465 7261 6c5b 2261 6374 7561 6c22  Literal["actual"
+00011aa0: 2c20 6222 6163 7475 616c 222c 2022 6578  , b"actual", "ex
+00011ab0: 7472 6122 2c20 6222 6578 7472 6122 2c20  tra", b"extra", 
+00011ac0: 226b 6269 6422 2c20 6222 6b62 6964 222c  "kbid", b"kbid",
+00011ad0: 2022 6d6f 6465 6c22 2c20 6222 6d6f 6465   "model", b"mode
+00011ae0: 6c22 2c20 2272 656c 6561 7365 5f63 6861  l", "release_cha
+00011af0: 6e6e 656c 222c 2062 2272 656c 6561 7365  nnel", b"release
+00011b00: 5f63 6861 6e6e 656c 222c 2022 7368 6172  _channel", "shar
+00011b10: 6473 222c 2062 2273 6861 7264 7322 2c20  ds", b"shards", 
+00011b20: 2273 696d 696c 6172 6974 7922 2c20 6222  "similarity", b"
+00011b30: 7369 6d69 6c61 7269 7479 225d 2920 2d3e  similarity"]) ->
+00011b40: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+00011b50: 616c 5f5f 5f53 6861 7264 7320 3d20 5368  al___Shards = Sh
+00011b60: 6172 6473 0a0a 4074 7970 696e 672e 6669  ards..@typing.fi
+00011b70: 6e61 6c0a 636c 6173 7320 496e 6465 7852  nal.class IndexR
+00011b80: 6573 6f75 7263 6528 676f 6f67 6c65 2e70  esource(google.p
+00011b90: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00011ba0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00011bb0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00011bc0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00011bd0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00011be0: 0a20 2020 204b 4249 445f 4649 454c 445f  .    KBID_FIELD_
+00011bf0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00011c00: 2e69 6e74 0a20 2020 2052 4944 5f46 4945  .int.    RID_FIE
+00011c10: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00011c20: 696e 732e 696e 740a 2020 2020 5245 494e  ins.int.    REIN
+00011c30: 4445 585f 5645 4354 4f52 535f 4649 454c  DEX_VECTORS_FIEL
+00011c40: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00011c50: 6e73 2e69 6e74 0a20 2020 206b 6269 643a  ns.int.    kbid:
+00011c60: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
+00011c70: 2020 7269 643a 2062 7569 6c74 696e 732e    rid: builtins.
+00011c80: 7374 720a 2020 2020 7265 696e 6465 785f  str.    reindex_
+00011c90: 7665 6374 6f72 733a 2062 7569 6c74 696e  vectors: builtin
+00011ca0: 732e 626f 6f6c 0a20 2020 2064 6566 205f  s.bool.    def _
+00011cb0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00011cc0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+00011cd0: 2c0a 2020 2020 2020 2020 6b62 6964 3a20  ,.        kbid: 
+00011ce0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00011cf0: 2e2e 2c0a 2020 2020 2020 2020 7269 643a  ..,.        rid:
+00011d00: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+00011d10: 2e2e 2e2c 0a20 2020 2020 2020 2072 6569  ...,.        rei
+00011d20: 6e64 6578 5f76 6563 746f 7273 3a20 6275  ndex_vectors: bu
+00011d30: 696c 7469 6e73 2e62 6f6f 6c20 3d20 2e2e  iltins.bool = ..
+00011d40: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+00011d50: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+00011d60: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+00011d70: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00011d80: 672e 4c69 7465 7261 6c5b 226b 6269 6422  g.Literal["kbid"
+00011d90: 2c20 6222 6b62 6964 222c 2022 7265 696e  , b"kbid", "rein
+00011da0: 6465 785f 7665 6374 6f72 7322 2c20 6222  dex_vectors", b"
+00011db0: 7265 696e 6465 785f 7665 6374 6f72 7322  reindex_vectors"
+00011dc0: 2c20 2272 6964 222c 2062 2272 6964 225d  , "rid", b"rid"]
+00011dd0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
+00011de0: 676c 6f62 616c 5f5f 5f49 6e64 6578 5265  global___IndexRe
+00011df0: 736f 7572 6365 203d 2049 6e64 6578 5265  source = IndexRe
+00011e00: 736f 7572 6365 0a0a 4074 7970 696e 672e  source..@typing.
+00011e10: 6669 6e61 6c0a 636c 6173 7320 496e 6465  final.class Inde
+00011e20: 7853 7461 7475 7328 676f 6f67 6c65 2e70  xStatus(google.p
+00011e30: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00011e40: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00011e50: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00011e60: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00011e70: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00011e80: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00011e90: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00011ea0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+00011eb0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 496e  .....global___In
+00011ec0: 6465 7853 7461 7475 7320 3d20 496e 6465  dexStatus = Inde
+00011ed0: 7853 7461 7475 730a 0a40 7479 7069 6e67  xStatus..@typing
+00011ee0: 2e66 696e 616c 0a63 6c61 7373 2053 6574  .final.class Set
+00011ef0: 5665 6374 6f72 7352 6571 7565 7374 2867  VectorsRequest(g
+00011f00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
+00011f10: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
+00011f20: 0a20 2020 2044 4553 4352 4950 544f 523a  .    DESCRIPTOR:
+00011f30: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00011f40: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+00011f50: 7269 7074 6f72 0a0a 2020 2020 5645 4354  riptor..    VECT
+00011f60: 4f52 535f 4649 454c 445f 4e55 4d42 4552  ORS_FIELD_NUMBER
+00011f70: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00011f80: 2020 204b 4249 445f 4649 454c 445f 4e55     KBID_FIELD_NU
+00011f90: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00011fa0: 6e74 0a20 2020 2052 4944 5f46 4945 4c44  nt.    RID_FIELD
+00011fb0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00011fc0: 732e 696e 740a 2020 2020 4649 454c 445f  s.int.    FIELD_
+00011fd0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00011fe0: 696c 7469 6e73 2e69 6e74 0a20 2020 206b  iltins.int.    k
+00011ff0: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
+00012000: 720a 2020 2020 7269 643a 2062 7569 6c74  r.    rid: built
+00012010: 696e 732e 7374 720a 2020 2020 4070 726f  ins.str.    @pro
+00012020: 7065 7274 790a 2020 2020 6465 6620 7665  perty.    def ve
+00012030: 6374 6f72 7328 7365 6c66 2920 2d3e 206e  ctors(self) -> n
+00012040: 7563 6c69 6164 625f 7072 6f74 6f73 2e75  ucliadb_protos.u
+00012050: 7469 6c73 5f70 6232 2e56 6563 746f 724f  tils_pb2.VectorO
+00012060: 626a 6563 743a 202e 2e2e 0a20 2020 2040  bject: ....    @
+00012070: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00012080: 2066 6965 6c64 2873 656c 6629 202d 3e20   field(self) -> 
+00012090: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+000120a0: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
+000120b0: 656c 6449 443a 202e 2e2e 0a20 2020 2064  eldID: ....    d
+000120c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000120d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000120e0: 2020 202a 2c0a 2020 2020 2020 2020 7665     *,.        ve
+000120f0: 6374 6f72 733a 206e 7563 6c69 6164 625f  ctors: nucliadb_
+00012100: 7072 6f74 6f73 2e75 7469 6c73 5f70 6232  protos.utils_pb2
+00012110: 2e56 6563 746f 724f 626a 6563 7420 7c20  .VectorObject | 
+00012120: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00012130: 2020 2020 6b62 6964 3a20 6275 696c 7469      kbid: builti
+00012140: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00012150: 2020 2020 2020 7269 643a 2062 7569 6c74        rid: built
+00012160: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+00012170: 2020 2020 2020 2066 6965 6c64 3a20 6e75         field: nu
+00012180: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00012190: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+000121a0: 6449 4420 7c20 4e6f 6e65 203d 202e 2e2e  dID | None = ...
+000121b0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+000121c0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
+000121d0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+000121e0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+000121f0: 6974 6572 616c 5b22 6669 656c 6422 2c20  iteral["field", 
+00012200: 6222 6669 656c 6422 2c20 2276 6563 746f  b"field", "vecto
+00012210: 7273 222c 2062 2276 6563 746f 7273 225d  rs", b"vectors"]
+00012220: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+00012230: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
+00012240: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
+00012250: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+00012260: 696e 672e 4c69 7465 7261 6c5b 2266 6965  ing.Literal["fie
+00012270: 6c64 222c 2062 2266 6965 6c64 222c 2022  ld", b"field", "
+00012280: 6b62 6964 222c 2062 226b 6269 6422 2c20  kbid", b"kbid", 
+00012290: 2272 6964 222c 2062 2272 6964 222c 2022  "rid", b"rid", "
+000122a0: 7665 6374 6f72 7322 2c20 6222 7665 6374  vectors", b"vect
+000122b0: 6f72 7322 5d29 202d 3e20 4e6f 6e65 3a20  ors"]) -> None: 
+000122c0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 5365  .....global___Se
+000122d0: 7456 6563 746f 7273 5265 7175 6573 7420  tVectorsRequest 
+000122e0: 3d20 5365 7456 6563 746f 7273 5265 7175  = SetVectorsRequ
+000122f0: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
+00012300: 616c 0a63 6c61 7373 2053 6574 5665 6374  al.class SetVect
+00012310: 6f72 7352 6573 706f 6e73 6528 676f 6f67  orsResponse(goog
+00012320: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+00012330: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+00012340: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00012350: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00012360: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+00012370: 746f 720a 0a20 2020 2046 4f55 4e44 5f46  tor..    FOUND_F
+00012380: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00012390: 6c74 696e 732e 696e 740a 2020 2020 666f  ltins.int.    fo
+000123a0: 756e 643a 2062 7569 6c74 696e 732e 626f  und: builtins.bo
+000123b0: 6f6c 0a20 2020 2064 6566 205f 5f69 6e69  ol.    def __ini
+000123c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000123d0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
+000123e0: 2020 2020 2020 666f 756e 643a 2062 7569        found: bui
+000123f0: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
+00012400: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00012410: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
+00012420: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+00012430: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+00012440: 2e4c 6974 6572 616c 5b22 666f 756e 6422  .Literal["found"
+00012450: 2c20 6222 666f 756e 6422 5d29 202d 3e20  , b"found"]) -> 
+00012460: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
+00012470: 6c5f 5f5f 5365 7456 6563 746f 7273 5265  l___SetVectorsRe
+00012480: 7370 6f6e 7365 203d 2053 6574 5665 6374  sponse = SetVect
+00012490: 6f72 7352 6573 706f 6e73 650a 0a40 7479  orsResponse..@ty
+000124a0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+000124b0: 2046 696c 6552 6571 7565 7374 2867 6f6f   FileRequest(goo
+000124c0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+000124d0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+000124e0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+000124f0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00012500: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+00012510: 7074 6f72 0a0a 2020 2020 4255 434b 4554  ptor..    BUCKET
+00012520: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00012530: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00012540: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+00012550: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00012560: 2020 2062 7563 6b65 743a 2062 7569 6c74     bucket: built
+00012570: 696e 732e 7374 720a 2020 2020 6b65 793a  ins.str.    key:
+00012580: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
+00012590: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000125a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000125b0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+000125c0: 2062 7563 6b65 743a 2062 7569 6c74 696e   bucket: builtin
+000125d0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+000125e0: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
+000125f0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00012600: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+00012610: 0a20 2020 2064 6566 2043 6c65 6172 4669  .    def ClearFi
+00012620: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
+00012630: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
+00012640: 6572 616c 5b22 6275 636b 6574 222c 2062  eral["bucket", b
+00012650: 2262 7563 6b65 7422 2c20 226b 6579 222c  "bucket", "key",
+00012660: 2062 226b 6579 225d 2920 2d3e 204e 6f6e   b"key"]) -> Non
+00012670: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+00012680: 5f46 696c 6552 6571 7565 7374 203d 2046  _FileRequest = F
+00012690: 696c 6552 6571 7565 7374 0a0a 4074 7970  ileRequest..@typ
+000126a0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+000126b0: 4269 6e61 7279 4461 7461 2867 6f6f 676c  BinaryData(googl
+000126c0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+000126d0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+000126e0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+000126f0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+00012700: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+00012710: 6f72 0a0a 2020 2020 4441 5441 5f46 4945  or..    DATA_FIE
+00012720: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00012730: 696e 732e 696e 740a 2020 2020 6461 7461  ins.int.    data
+00012740: 3a20 6275 696c 7469 6e73 2e62 7974 6573  : builtins.bytes
+00012750: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00012760: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00012770: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00012780: 2020 2020 6461 7461 3a20 6275 696c 7469      data: builti
+00012790: 6e73 2e62 7974 6573 203d 202e 2e2e 2c0a  ns.bytes = ...,.
+000127a0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+000127b0: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
+000127c0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+000127d0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+000127e0: 6974 6572 616c 5b22 6461 7461 222c 2062  iteral["data", b
+000127f0: 2264 6174 6122 5d29 202d 3e20 4e6f 6e65  "data"]) -> None
+00012800: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+00012810: 4269 6e61 7279 4461 7461 203d 2042 696e  BinaryData = Bin
+00012820: 6172 7944 6174 610a 0a40 7479 7069 6e67  aryData..@typing
+00012830: 2e66 696e 616c 0a63 6c61 7373 2042 696e  .final.class Bin
+00012840: 6172 794d 6574 6164 6174 6128 676f 6f67  aryMetadata(goog
+00012850: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+00012860: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+00012870: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00012880: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00012890: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+000128a0: 746f 720a 0a20 2020 204b 4249 445f 4649  tor..    KBID_FI
+000128b0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000128c0: 7469 6e73 2e69 6e74 0a20 2020 204b 4559  tins.int.    KEY
+000128d0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+000128e0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000128f0: 5349 5a45 5f46 4945 4c44 5f4e 554d 4245  SIZE_FIELD_NUMBE
+00012900: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00012910: 2020 2020 4649 4c45 4e41 4d45 5f46 4945      FILENAME_FIE
+00012920: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00012930: 696e 732e 696e 740a 2020 2020 434f 4e54  ins.int.    CONT
+00012940: 454e 545f 5459 5045 5f46 4945 4c44 5f4e  ENT_TYPE_FIELD_N
+00012950: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00012960: 696e 740a 2020 2020 6b62 6964 3a20 6275  int.    kbid: bu
+00012970: 696c 7469 6e73 2e73 7472 0a20 2020 206b  iltins.str.    k
+00012980: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
+00012990: 0a20 2020 2073 697a 653a 2062 7569 6c74  .    size: built
+000129a0: 696e 732e 696e 740a 2020 2020 6669 6c65  ins.int.    file
+000129b0: 6e61 6d65 3a20 6275 696c 7469 6e73 2e73  name: builtins.s
+000129c0: 7472 0a20 2020 2063 6f6e 7465 6e74 5f74  tr.    content_t
+000129d0: 7970 653a 2062 7569 6c74 696e 732e 7374  ype: builtins.st
+000129e0: 720a 2020 2020 6465 6620 5f5f 696e 6974  r.    def __init
+000129f0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00012a00: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+00012a10: 2020 2020 206b 6269 643a 2062 7569 6c74       kbid: built
+00012a20: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+00012a30: 2020 2020 2020 206b 6579 3a20 6275 696c         key: buil
+00012a40: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+00012a50: 2020 2020 2020 2020 7369 7a65 3a20 6275          size: bu
+00012a60: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
+00012a70: 2c0a 2020 2020 2020 2020 6669 6c65 6e61  ,.        filena
+00012a80: 6d65 3a20 6275 696c 7469 6e73 2e73 7472  me: builtins.str
+00012a90: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00012aa0: 636f 6e74 656e 745f 7479 7065 3a20 6275  content_type: bu
+00012ab0: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
+00012ac0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00012ad0: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
+00012ae0: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+00012af0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+00012b00: 2e4c 6974 6572 616c 5b22 636f 6e74 656e  .Literal["conten
+00012b10: 745f 7479 7065 222c 2062 2263 6f6e 7465  t_type", b"conte
+00012b20: 6e74 5f74 7970 6522 2c20 2266 696c 656e  nt_type", "filen
+00012b30: 616d 6522 2c20 6222 6669 6c65 6e61 6d65  ame", b"filename
+00012b40: 222c 2022 6b62 6964 222c 2062 226b 6269  ", "kbid", b"kbi
+00012b50: 6422 2c20 226b 6579 222c 2062 226b 6579  d", "key", b"key
+00012b60: 222c 2022 7369 7a65 222c 2062 2273 697a  ", "size", b"siz
+00012b70: 6522 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  e"]) -> None: ..
+00012b80: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4269 6e61  ...global___Bina
+00012b90: 7279 4d65 7461 6461 7461 203d 2042 696e  ryMetadata = Bin
+00012ba0: 6172 794d 6574 6164 6174 610a 0a40 7479  aryMetadata..@ty
+00012bb0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00012bc0: 2055 706c 6f61 6442 696e 6172 7944 6174   UploadBinaryDat
+00012bd0: 6128 676f 6f67 6c65 2e70 726f 746f 6275  a(google.protobu
+00012be0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+00012bf0: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+00012c00: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+00012c10: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+00012c20: 6573 6372 6970 746f 720a 0a20 2020 2043  escriptor..    C
+00012c30: 4f55 4e54 5f46 4945 4c44 5f4e 554d 4245  OUNT_FIELD_NUMBE
+00012c40: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00012c50: 2020 2020 4d45 5441 4441 5441 5f46 4945      METADATA_FIE
+00012c60: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00012c70: 696e 732e 696e 740a 2020 2020 5041 594c  ins.int.    PAYL
+00012c80: 4f41 445f 4649 454c 445f 4e55 4d42 4552  OAD_FIELD_NUMBER
+00012c90: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00012ca0: 2020 2063 6f75 6e74 3a20 6275 696c 7469     count: builti
+00012cb0: 6e73 2e69 6e74 0a20 2020 2070 6179 6c6f  ns.int.    paylo
+00012cc0: 6164 3a20 6275 696c 7469 6e73 2e62 7974  ad: builtins.byt
+00012cd0: 6573 0a20 2020 2040 7072 6f70 6572 7479  es.    @property
+00012ce0: 0a20 2020 2064 6566 206d 6574 6164 6174  .    def metadat
+00012cf0: 6128 7365 6c66 2920 2d3e 2067 6c6f 6261  a(self) -> globa
+00012d00: 6c5f 5f5f 4269 6e61 7279 4d65 7461 6461  l___BinaryMetada
+00012d10: 7461 3a20 2e2e 2e0a 2020 2020 6465 6620  ta: ....    def 
+00012d20: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00012d30: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00012d40: 2a2c 0a20 2020 2020 2020 2063 6f75 6e74  *,.        count
+00012d50: 3a20 6275 696c 7469 6e73 2e69 6e74 203d  : builtins.int =
+00012d60: 202e 2e2e 2c0a 2020 2020 2020 2020 6d65   ...,.        me
+00012d70: 7461 6461 7461 3a20 676c 6f62 616c 5f5f  tadata: global__
+00012d80: 5f42 696e 6172 794d 6574 6164 6174 6120  _BinaryMetadata 
+00012d90: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00012da0: 2020 2020 2020 7061 796c 6f61 643a 2062        payload: b
+00012db0: 7569 6c74 696e 732e 6279 7465 7320 3d20  uiltins.bytes = 
+00012dc0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
+00012dd0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+00012de0: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
+00012df0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00012e00: 672e 4c69 7465 7261 6c5b 2264 6174 6122  g.Literal["data"
+00012e10: 2c20 6222 6461 7461 222c 2022 6d65 7461  , b"data", "meta
+00012e20: 6461 7461 222c 2062 226d 6574 6164 6174  data", b"metadat
+00012e30: 6122 2c20 2270 6179 6c6f 6164 222c 2062  a", "payload", b
+00012e40: 2270 6179 6c6f 6164 225d 2920 2d3e 2062  "payload"]) -> b
+00012e50: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+00012e60: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+00012e70: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00012e80: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00012e90: 7465 7261 6c5b 2263 6f75 6e74 222c 2062  teral["count", b
+00012ea0: 2263 6f75 6e74 222c 2022 6461 7461 222c  "count", "data",
+00012eb0: 2062 2264 6174 6122 2c20 226d 6574 6164   b"data", "metad
+00012ec0: 6174 6122 2c20 6222 6d65 7461 6461 7461  ata", b"metadata
+00012ed0: 222c 2022 7061 796c 6f61 6422 2c20 6222  ", "payload", b"
+00012ee0: 7061 796c 6f61 6422 5d29 202d 3e20 4e6f  payload"]) -> No
+00012ef0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+00012f00: 5768 6963 684f 6e65 6f66 2873 656c 662c  WhichOneof(self,
+00012f10: 206f 6e65 6f66 5f67 726f 7570 3a20 7479   oneof_group: ty
+00012f20: 7069 6e67 2e4c 6974 6572 616c 5b22 6461  ping.Literal["da
+00012f30: 7461 222c 2062 2264 6174 6122 5d29 202d  ta", b"data"]) -
+00012f40: 3e20 7479 7069 6e67 2e4c 6974 6572 616c  > typing.Literal
+00012f50: 5b22 6d65 7461 6461 7461 222c 2022 7061  ["metadata", "pa
+00012f60: 796c 6f61 6422 5d20 7c20 4e6f 6e65 3a20  yload"] | None: 
+00012f70: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 5570  .....global___Up
+00012f80: 6c6f 6164 4269 6e61 7279 4461 7461 203d  loadBinaryData =
+00012f90: 2055 706c 6f61 6442 696e 6172 7944 6174   UploadBinaryDat
+00012fa0: 610a 0a40 7479 7069 6e67 2e66 696e 616c  a..@typing.final
+00012fb0: 0a63 6c61 7373 2046 696c 6555 706c 6f61  .class FileUploa
+00012fc0: 6465 6428 676f 6f67 6c65 2e70 726f 746f  ded(google.proto
+00012fd0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
+00012fe0: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
+00012ff0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+00013000: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+00013010: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+00013020: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00013030: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00013040: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00013050: 0a67 6c6f 6261 6c5f 5f5f 4669 6c65 5570  .global___FileUp
+00013060: 6c6f 6164 6564 203d 2046 696c 6555 706c  loaded = FileUpl
+00013070: 6f61 6465 640a 0a40 7479 7069 6e67 2e66  oaded..@typing.f
+00013080: 696e 616c 0a63 6c61 7373 2053 796e 6f6e  inal.class Synon
+00013090: 796d 7352 6571 7565 7374 2867 6f6f 676c  ymsRequest(googl
+000130a0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+000130b0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+000130c0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+000130d0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+000130e0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+000130f0: 6f72 0a0a 2020 2020 4b42 4944 5f46 4945  or..    KBID_FIE
+00013100: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00013110: 696e 732e 696e 740a 2020 2020 6b62 6964  ins.int.    kbid
+00013120: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00013130: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00013140: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00013150: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00013160: 2020 6b62 6964 3a20 6275 696c 7469 6e73    kbid: builtins
+00013170: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00013180: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00013190: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+000131a0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+000131b0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+000131c0: 616c 5b22 6b62 6964 222c 2062 226b 6269  al["kbid", b"kbi
+000131d0: 6422 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  d"]) -> None: ..
+000131e0: 2e0a 0a67 6c6f 6261 6c5f 5f5f 5379 6e6f  ...global___Syno
+000131f0: 6e79 6d73 5265 7175 6573 7420 3d20 5379  nymsRequest = Sy
+00013200: 6e6f 6e79 6d73 5265 7175 6573 740a       nonymsRequest.
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,25 +37,27 @@
     GCKnowledgeBoxResponse as GCKnowledgeBoxResponse,
     KBConfiguration as KBConfiguration,
     KnowledgeBoxConfig as KnowledgeBoxConfig,
     KnowledgeBoxID as KnowledgeBoxID,
     KnowledgeBoxNew as KnowledgeBoxNew,
     KnowledgeBoxResponseStatus as KnowledgeBoxResponseStatus,
     KnowledgeBoxUpdate as KnowledgeBoxUpdate,
+    KnowledgeBoxVectorSetsConfig as KnowledgeBoxVectorSetsConfig,
     Label as Label,
     LabelSet as LabelSet,
     Labels as Labels,
     NOTFOUND as NOTFOUND,
     NewKnowledgeBoxResponse as NewKnowledgeBoxResponse,
     OK as OK,
     SemanticModelMetadata as SemanticModelMetadata,
     Synonyms as Synonyms,
     TermSynonyms as TermSynonyms,
     UpdateKnowledgeBoxResponse as UpdateKnowledgeBoxResponse,
     VectorSet as VectorSet,
+    VectorSetConfig as VectorSetConfig,
     VectorSets as VectorSets,
 )
 from nucliadb_protos.noderesources_pb2 import (
     EmptyQuery as EmptyQuery,
     EmptyResponse as EmptyResponse,
     IndexMetadata as IndexMetadata,
     IndexParagraph as IndexParagraph,
```

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/python/setup.py` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/python/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/reader.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/reader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/replication.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/replication.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/resources.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/resources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/standalone.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/standalone.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/train.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/train.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/utils.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/utils.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/nucliadb_protos/writer.proto` & `nucliadb_node_binding-4.0.1.post1380/nucliadb_protos/writer.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/pyproject.toml` & `nucliadb_node_binding-4.0.1.post1380/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/collect_garbage.rs` & `nucliadb_node_binding-4.0.1.post1380/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/errors.rs` & `nucliadb_node_binding-4.0.1.post1380/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/lib.rs` & `nucliadb_node_binding-4.0.1.post1380/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/reader.rs` & `nucliadb_node_binding-4.0.1.post1380/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/update.rs` & `nucliadb_node_binding-4.0.1.post1380/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/src/writer.rs` & `nucliadb_node_binding-4.0.1.post1380/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/tests/__init__.py` & `nucliadb_node_binding-4.0.1.post1380/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/tests/conftest.py` & `nucliadb_node_binding-4.0.1.post1380/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1376/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.1.post1380/tests/integration/test_indexing.py`

 * *Files identical despite different names*

