# Comparing `tmp/faststream-0.5.8.tar.gz` & `tmp/faststream-0.5.9.tar.gz`

## Comparing `faststream-0.5.8.tar` & `faststream-0.5.9.tar`

### file list

```diff
@@ -1,352 +1,352 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.8/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.8/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.8/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.8/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.8/SECURITY.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.8/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.8/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/security.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/types.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13590 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/message.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/security.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    68318 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0   102616 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/__init__.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/factory.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/message.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/parser.py
--rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/security.py
--rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    76258 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   120064 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/factory.py
--rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/log/logging.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/__init__.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/annotations.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/message.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/parser.py
--rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/security.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36834 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/__init__.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/bucket_declarer.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/obj_storage_declarer.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/helpers/object_builder.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/middleware.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/kv_watch.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/obj_watch.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/factory.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/subscription.py
--rw-r--r--   0        0        0    31761 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/consts.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/middleware.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/opentelemetry/provider.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    21894 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    31321 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/middleware.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/factory.py
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/message.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/parser.py
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/security.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27863 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/middleware.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/opentelemetry/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/factory.py
--rw-r--r--   0        0        0    21757 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/app.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.8/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.8/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.8/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.8/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.8/README.md
--rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 faststream-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 faststream-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.9/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.9/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.9/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.9/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.9/SECURITY.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.9/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.9/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/security.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13590 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    68318 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0   102616 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/subscriber/factory.py
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/security.py
+-rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    76258 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   120064 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/subscriber/factory.py
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/log/logging.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/annotations.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/message.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/parser.py
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/security.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36834 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/helpers/__init__.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/helpers/bucket_declarer.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/helpers/obj_storage_declarer.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/helpers/object_builder.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/schemas/kv_watch.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/schemas/obj_watch.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/subscriber/factory.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/subscriber/subscription.py
+-rw-r--r--   0        0        0    31761 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/opentelemetry/consts.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/opentelemetry/provider.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    21894 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    31321 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/subscriber/factory.py
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/message.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/security.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27863 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/subscriber/factory.py
+-rw-r--r--   0        0        0    21757 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/testing/app.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.9/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.9/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.9/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.9/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.9/README.md
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 faststream-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 faststream-0.5.9/PKG-INFO
```

### Comparing `faststream-0.5.8/.pre-commit-config.yaml` & `faststream-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.secrets.baseline` & `faststream-0.5.9/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/CITATION.cff` & `faststream-0.5.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/CODE_OF_CONDUCT.md` & `faststream-0.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/CONTRIBUTING.md` & `faststream-0.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/SECURITY.md` & `faststream-0.5.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/dependabot.yml` & `faststream-0.5.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.9/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/codeql.yml` & `faststream-0.5.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/dependency-review.yaml` & `faststream-0.5.9/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/deploy-docs.yaml` & `faststream-0.5.9/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/publish_coverage.yml` & `faststream-0.5.9/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/publish_pypi.yml` & `faststream-0.5.9/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/test.yaml` & `faststream-0.5.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/.github/workflows/update_release_notes.yaml` & `faststream-0.5.9/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e02_1_basic_publisher.py` & `faststream-0.5.9/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e02_2_basic_publisher.py` & `faststream-0.5.9/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e02_3_basic_publisher.py` & `faststream-0.5.9/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e03_miltiple_pubsub.py` & `faststream-0.5.9/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e04_msg_filter.py` & `faststream-0.5.9/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e07_ack_immediately.py` & `faststream-0.5.9/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e09_testing_mocks.py` & `faststream-0.5.9/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e10_middlewares.py` & `faststream-0.5.9/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/e11_settings.py` & `faststream-0.5.9/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/fastapi_integration/testing.py` & `faststream-0.5.9/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/howto/structlogs.py` & `faststream-0.5.9/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/kafka/testing.py` & `faststream-0.5.9/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/nats/e03_publisher.py` & `faststream-0.5.9/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/nats/e04_js_basic.py` & `faststream-0.5.9/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/nats/e05_basic_and_js.py` & `faststream-0.5.9/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/nats/e07_object_storage.py` & `faststream-0.5.9/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/rabbit/direct.py` & `faststream-0.5.9/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/rabbit/fanout.py` & `faststream-0.5.9/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/rabbit/header.py` & `faststream-0.5.9/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/rabbit/topic.py` & `faststream-0.5.9/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/redis/channel_sub_pattern.py` & `faststream-0.5.9/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/redis/rpc.py` & `faststream-0.5.9/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/router/basic_publish.py` & `faststream-0.5.9/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/serialization/avro/avro.py` & `faststream-0.5.9/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/serialization/msgpack/pack.py` & `faststream-0.5.9/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.9/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/__init__.py` & `faststream-0.5.9/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/_compat.py` & `faststream-0.5.9/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/app.py` & `faststream-0.5.9/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/exceptions.py` & `faststream-0.5.9/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/security.py` & `faststream-0.5.9/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/types.py` & `faststream-0.5.9/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/abc.py` & `faststream-0.5.9/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/generate.py` & `faststream-0.5.9/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/message.py` & `faststream-0.5.9/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/proto.py` & `faststream-0.5.9/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/site.py` & `faststream-0.5.9/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/utils.py` & `faststream-0.5.9/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.9/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/channels.py` & `faststream-0.5.9/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/info.py` & `faststream-0.5.9/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/main.py` & `faststream-0.5.9/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/message.py` & `faststream-0.5.9/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/operations.py` & `faststream-0.5.9/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/security.py` & `faststream-0.5.9/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/servers.py` & `faststream-0.5.9/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/utils.py` & `faststream-0.5.9/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.9/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.9/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/message.py` & `faststream-0.5.9/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/router.py` & `faststream-0.5.9/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/schemas.py` & `faststream-0.5.9/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/types.py` & `faststream-0.5.9/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/utils.py` & `faststream-0.5.9/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/core/abc.py` & `faststream-0.5.9/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/core/logging.py` & `faststream-0.5.9/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/core/usecase.py` & `faststream-0.5.9/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/fastapi/context.py` & `faststream-0.5.9/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.9/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/fastapi/route.py` & `faststream-0.5.9/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/fastapi/router.py` & `faststream-0.5.9/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/middlewares/base.py` & `faststream-0.5.9/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/middlewares/logging.py` & `faststream-0.5.9/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/publisher/fake.py` & `faststream-0.5.9/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/publisher/proto.py` & `faststream-0.5.9/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/publisher/usecase.py` & `faststream-0.5.9/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/subscriber/call_item.py` & `faststream-0.5.9/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/subscriber/proto.py` & `faststream-0.5.9/faststream/broker/subscriber/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/subscriber/usecase.py` & `faststream-0.5.9/faststream/broker/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/wrapper/call.py` & `faststream-0.5.9/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/broker/wrapper/proto.py` & `faststream-0.5.9/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/main.py` & `faststream-0.5.9/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/docs/app.py` & `faststream-0.5.9/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/supervisors/basereload.py` & `faststream-0.5.9/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.9/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/supervisors/utils.py` & `faststream-0.5.9/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.9/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/utils/imports.py` & `faststream-0.5.9/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/utils/logs.py` & `faststream-0.5.9/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/cli/utils/parser.py` & `faststream-0.5.9/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/annotations.py` & `faststream-0.5.9/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/client.py` & `faststream-0.5.9/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/message.py` & `faststream-0.5.9/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/parser.py` & `faststream-0.5.9/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/router.py` & `faststream-0.5.9/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/security.py` & `faststream-0.5.9/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/testing.py` & `faststream-0.5.9/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/broker/broker.py` & `faststream-0.5.9/faststream/confluent/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/broker/logging.py` & `faststream-0.5.9/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/broker/registrator.py` & `faststream-0.5.9/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.9/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.9/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/confluent/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/opentelemetry/provider.py` & `faststream-0.5.9/faststream/confluent/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.9/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/publisher/producer.py` & `faststream-0.5.9/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/publisher/usecase.py` & `faststream-0.5.9/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/schemas/params.py` & `faststream-0.5.9/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.9/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/subscriber/factory.py` & `faststream-0.5.9/faststream/confluent/subscriber/factory.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.9/faststream/confluent/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/annotations.py` & `faststream-0.5.9/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/message.py` & `faststream-0.5.9/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/parser.py` & `faststream-0.5.9/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/router.py` & `faststream-0.5.9/faststream/kafka/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/security.py` & `faststream-0.5.9/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/testing.py` & `faststream-0.5.9/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/broker/broker.py` & `faststream-0.5.9/faststream/kafka/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/broker/logging.py` & `faststream-0.5.9/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/broker/registrator.py` & `faststream-0.5.9/faststream/kafka/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.9/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.9/faststream/kafka/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/kafka/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/opentelemetry/provider.py` & `faststream-0.5.9/faststream/kafka/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.9/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/publisher/producer.py` & `faststream-0.5.9/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/publisher/usecase.py` & `faststream-0.5.9/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/schemas/params.py` & `faststream-0.5.9/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.9/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/subscriber/factory.py` & `faststream-0.5.9/faststream/kafka/subscriber/factory.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.9/faststream/kafka/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/log/formatter.py` & `faststream-0.5.9/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/log/logging.py` & `faststream-0.5.9/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/__init__.py` & `faststream-0.5.9/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/annotations.py` & `faststream-0.5.9/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/message.py` & `faststream-0.5.9/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/parser.py` & `faststream-0.5.9/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/router.py` & `faststream-0.5.9/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/security.py` & `faststream-0.5.9/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/testing.py` & `faststream-0.5.9/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/broker/broker.py` & `faststream-0.5.9/faststream/nats/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/broker/logging.py` & `faststream-0.5.9/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/broker/registrator.py` & `faststream-0.5.9/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/fastapi/__init__.py` & `faststream-0.5.9/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.9/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/helpers/bucket_declarer.py` & `faststream-0.5.9/faststream/nats/helpers/bucket_declarer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/helpers/obj_storage_declarer.py` & `faststream-0.5.9/faststream/nats/helpers/obj_storage_declarer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/helpers/object_builder.py` & `faststream-0.5.9/faststream/nats/helpers/object_builder.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/nats/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/opentelemetry/provider.py` & `faststream-0.5.9/faststream/nats/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.9/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/publisher/producer.py` & `faststream-0.5.9/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/publisher/usecase.py` & `faststream-0.5.9/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/schemas/js_stream.py` & `faststream-0.5.9/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/schemas/kv_watch.py` & `faststream-0.5.9/faststream/nats/schemas/kv_watch.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/schemas/obj_watch.py` & `faststream-0.5.9/faststream/nats/schemas/obj_watch.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.9/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.9/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/subscriber/factory.py` & `faststream-0.5.9/faststream/nats/subscriber/factory.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/subscriber/subscription.py` & `faststream-0.5.9/faststream/nats/subscriber/subscription.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/nats/subscriber/usecase.py` & `faststream-0.5.9/faststream/nats/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/opentelemetry/provider.py` & `faststream-0.5.9/faststream/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/__init__.py` & `faststream-0.5.9/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/annotations.py` & `faststream-0.5.9/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/message.py` & `faststream-0.5.9/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/parser.py` & `faststream-0.5.9/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/router.py` & `faststream-0.5.9/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/security.py` & `faststream-0.5.9/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/testing.py` & `faststream-0.5.9/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/utils.py` & `faststream-0.5.9/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/broker/broker.py` & `faststream-0.5.9/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/broker/logging.py` & `faststream-0.5.9/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/broker/registrator.py` & `faststream-0.5.9/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.9/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/fastapi/router.py` & `faststream-0.5.9/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/rabbit/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/opentelemetry/provider.py` & `faststream-0.5.9/faststream/rabbit/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.9/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/publisher/producer.py` & `faststream-0.5.9/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.9/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/schemas/constants.py` & `faststream-0.5.9/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.9/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/schemas/queue.py` & `faststream-0.5.9/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/schemas/reply.py` & `faststream-0.5.9/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.9/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/subscriber/factory.py` & `faststream-0.5.9/faststream/rabbit/subscriber/factory.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.9/faststream/rabbit/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/__init__.py` & `faststream-0.5.9/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/annotations.py` & `faststream-0.5.9/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/message.py` & `faststream-0.5.9/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/parser.py` & `faststream-0.5.9/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/router.py` & `faststream-0.5.9/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/security.py` & `faststream-0.5.9/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/testing.py` & `faststream-0.5.9/faststream/redis/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/broker/broker.py` & `faststream-0.5.9/faststream/redis/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/broker/logging.py` & `faststream-0.5.9/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/broker/registrator.py` & `faststream-0.5.9/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/fastapi/__init__.py` & `faststream-0.5.9/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.9/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/opentelemetry/middleware.py` & `faststream-0.5.9/faststream/redis/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/opentelemetry/provider.py` & `faststream-0.5.9/faststream/redis/opentelemetry/provider.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.9/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/publisher/producer.py` & `faststream-0.5.9/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/publisher/usecase.py` & `faststream-0.5.9/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/schemas/list_sub.py` & `faststream-0.5.9/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/schemas/proto.py` & `faststream-0.5.9/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.9/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.9/faststream/redis/schemas/stream_sub.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,8 +53,12 @@
         self.batch = batch
         self.no_ack = no_ack
         self.last_id = last_id
         self.maxlen = maxlen
         self.max_records = max_records
 
     def __hash__(self) -> int:
+        if self.group is not None:
+            return hash(
+                f"stream:{self.name} group:{self.group} consumer:{self.consumer}"
+            )
         return hash(f"stream:{self.name}")
```

### Comparing `faststream-0.5.8/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.9/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/subscriber/factory.py` & `faststream-0.5.9/faststream/redis/subscriber/factory.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/redis/subscriber/usecase.py` & `faststream-0.5.9/faststream/redis/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/testing/app.py` & `faststream-0.5.9/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/testing/broker.py` & `faststream-0.5.9/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/ast.py` & `faststream-0.5.9/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/classes.py` & `faststream-0.5.9/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/data.py` & `faststream-0.5.9/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/functions.py` & `faststream-0.5.9/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/no_cast.py` & `faststream-0.5.9/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/path.py` & `faststream-0.5.9/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/context/builders.py` & `faststream-0.5.9/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/context/repository.py` & `faststream-0.5.9/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/faststream/utils/context/types.py` & `faststream-0.5.9/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/scripts/build-docs-pre-commit.sh` & `faststream-0.5.9/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/scripts/lint-pre-commit.sh` & `faststream-0.5.9/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/scripts/set_variables.sh` & `faststream-0.5.9/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/scripts/static-pre-commit.sh` & `faststream-0.5.9/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/LICENSE` & `faststream-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/README.md` & `faststream-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.8/pyproject.toml` & `faststream-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 dynamic = ["version"]
 
 dependencies = [
     "anyio>=3.7.1,<5",
     "fast-depends>=2.4.0b0,<2.5.0",
     "typer>=0.9,!=0.12,<1",
-    "typing-extensions>=4.8.0",
+    "typing-extensions>=4.8.0,!=4.12.*",
 ]
 
 [project.optional-dependencies]
 # public distributions
 rabbit = ["aio-pika>=9,<10"]
 
 kafka = ["aiokafka>=0.9,<0.11"]
```

### Comparing `faststream-0.5.8/PKG-INFO` & `faststream-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.8
+Version: 0.5.9
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -37,15 +37,15 @@
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: anyio<5,>=3.7.1
 Requires-Dist: fast-depends<2.5.0,>=2.4.0b0
 Requires-Dist: typer!=0.12,<1,>=0.9
-Requires-Dist: typing-extensions>=4.8.0
+Requires-Dist: typing-extensions!=4.12.*,>=4.8.0
 Provides-Extra: confluent
 Requires-Dist: confluent-kafka<3,>=2; extra == 'confluent'
 Provides-Extra: dev
 Requires-Dist: aio-pika<10,>=9; extra == 'dev'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'dev'
 Requires-Dist: bandit==1.7.8; extra == 'dev'
 Requires-Dist: cairosvg; extra == 'dev'
```

