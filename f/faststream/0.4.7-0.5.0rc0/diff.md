# Comparing `tmp/faststream-0.4.7.tar.gz` & `tmp/faststream-0.5.0rc0.tar.gz`

## Comparing `faststream-0.4.7.tar` & `faststream-0.5.0rc0.tar`

### file list

```diff
@@ -1,305 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.4.7/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.4.7/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.4.7/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.4.7/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.4.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.4.7/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16510 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.4.7/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/howto/__init__.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.4.7/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/__main__.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/_compat.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/annotations.py
--rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/app.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/constants.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/py.typed
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/security.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/types.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/base.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/__init__.py
--rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/handler.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/message.py
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/middlewares.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/parsers.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/publisher.py
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/push_back_watcher.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/router.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/schemas.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/security.py
--rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/test.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/types.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/utils.py
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0    21061 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/core/abc.py
--rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/core/asynchronous.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/core/mixins.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    24777 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/__init__.py
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/annotations.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/asyncapi.py
--rw-r--r--   0        0        0    20757 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/broker.py
--rw-r--r--   0        0        0    12478 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/broker.pyi
--rw-r--r--   0        0        0    24608 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/client.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/fastapi.py
--rw-r--r--   0        0        0    15431 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/fastapi.pyi
--rw-r--r--   0        0        0     8551 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/handler.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/message.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/parser.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/producer.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/publisher.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/router.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/router.pyi
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/security.py
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/logging.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/publisher.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/router.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/router.pyi
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/confluent/shared/schemas.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/asyncapi.py
--rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/broker.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/broker.pyi
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/fastapi.py
--rw-r--r--   0        0        0    15057 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/fastapi.pyi
--rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/handler.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/message.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/parser.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/producer.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/publisher.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/router.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/router.pyi
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/security.py
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/logging.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/publisher.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/router.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/router.pyi
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/kafka/shared/schemas.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/log/__init__.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/log/formatter.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/log/logging.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/__init__.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/annotations.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/asyncapi.py
--rw-r--r--   0        0        0    16182 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/broker.py
--rw-r--r--   0        0        0    10657 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/broker.pyi
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/fastapi.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/fastapi.pyi
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/handler.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/js_stream.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/js_stream.pyi
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/message.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/parser.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/producer.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/publisher.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/pull_sub.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/router.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/router.pyi
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/security.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/shared/__init__.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/shared/logging.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/shared/router.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/nats/shared/router.pyi
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/asyncapi.py
--rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/broker.py
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/broker.pyi
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/fastapi.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/fastapi.pyi
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/handler.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/helpers.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/message.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/producer.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/publisher.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/publisher.pyi
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/router.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/router.pyi
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/test.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/__init__.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/constants.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/logging.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/publisher.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/router.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/router.pyi
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/schemas.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/types.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/rabbit/shared/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/asyncapi.py
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/broker.py
--rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/broker.pyi
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/fastapi.py
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/fastapi.pyi
--rw-r--r--   0        0        0    10227 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/handler.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/message.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/parser.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/producer.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/publisher.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/router.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/router.pyi
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/schemas.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/security.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/shared/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/shared/logging.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/shared/router.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/redis/shared/router.pyi
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/ast.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/data.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 faststream-0.4.7/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      194 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.4.7/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.4.7/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.4.7/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.4.7/README.md
--rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 faststream-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    19991 2020-02-02 00:00:00.000000 faststream-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__main__.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/annotations.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/py.typed
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/security.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/message.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/router.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/types.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    19248 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    18762 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29413 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    65980 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   112731 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10087 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/message.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/router.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/security.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/testing.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    26992 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/router.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19471 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30361 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/message.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/router.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/security.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15867 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27625 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/app.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/data.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/README.md
+-rw-r--r--   0        0        0     9839 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/PKG-INFO
```

### Comparing `faststream-0.4.7/.pre-commit-config.yaml` & `faststream-0.5.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.secrets.baseline` & `faststream-0.5.0rc0/.secrets.baseline`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8991666666666667%*

 * *Differences: {"'generated_at'": "'2024-03-14T06:43:32Z'",*

 * * "'results'": "{'docs/docs/en/release.md': {0: {'line_number': 710}}}"}*

```diff
@@ -35,15 +35,15 @@
         {
             "path": "detect_secrets.filters.heuristic.is_swagger_file"
         },
         {
             "path": "detect_secrets.filters.heuristic.is_templated_secret"
         }
     ],
-    "generated_at": "2024-03-04T15:19:29Z",
+    "generated_at": "2024-03-14T06:43:32Z",
     "plugins_used": [
         {
             "name": "ArtifactoryDetector"
         },
         {
             "name": "AWSKeyDetector"
         },
@@ -124,15 +124,15 @@
         ],
         "docs/docs/en/release.md": [
             {
                 "filename": "docs/docs/en/release.md",
                 "hashed_secret": "35675e68f4b5af7b995d9205ad0fc43842f16450",
                 "is_secret": false,
                 "is_verified": false,
-                "line_number": 689,
+                "line_number": 710,
                 "type": "Basic Auth Credentials"
             }
         ],
         "examples/e10_middlewares.py": [
             {
                 "filename": "examples/e10_middlewares.py",
                 "hashed_secret": "35675e68f4b5af7b995d9205ad0fc43842f16450",
```

### Comparing `faststream-0.4.7/CITATION.cff` & `faststream-0.5.0rc0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/CODE_OF_CONDUCT.md` & `faststream-0.5.0rc0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/CONTRIBUTING.md` & `faststream-0.5.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/SECURITY.md` & `faststream-0.5.0rc0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.0rc0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/dependabot.yml` & `faststream-0.5.0rc0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.0rc0/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/codeql.yml` & `faststream-0.5.0rc0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/dependency-review.yaml` & `faststream-0.5.0rc0/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/deploy-docs.yaml` & `faststream-0.5.0rc0/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/publish_coverage.yml` & `faststream-0.5.0rc0/.github/workflows/publish_coverage.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     steps:
       - uses: actions/setup-python@v5
         with:
           python-version: "3.9"
 
       - run: pip install smokeshow
 
-      - uses: dawidd6/action-download-artifact@v3.1.2 # nosemgrep
+      - uses: dawidd6/action-download-artifact@v3.1.4 # nosemgrep
         with:
           workflow: test.yaml
           commit: ${{ github.event.workflow_run.head_sha }}
 
       - run: smokeshow upload coverage-html
         env:
           SMOKESHOW_GITHUB_STATUS_DESCRIPTION: Coverage {coverage-percentage}
```

### Comparing `faststream-0.4.7/.github/workflows/publish_pypi.yml` & `faststream-0.5.0rc0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/.github/workflows/test.yaml` & `faststream-0.5.0rc0/.github/workflows/test.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with:
           python-version: 3.9
       - name: Install Dependencies and library
         shell: bash
         run: |
           set -ux
           python -m pip install --upgrade pip
-          pip install -e ".[docs,rabbit,kafka,confluent,redis,nats,lint]"
+          pip install -e ".[rabbit,kafka,confluent,redis,nats,lint]"
 
       - name: Run ruff
         shell: bash
         run: ruff faststream
 
       - name: Run mypy
         shell: bash
@@ -80,15 +80,15 @@
       - uses: actions/cache@v4
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,docs,testing]
+        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
       - name: Install Pydantic v1
         if: matrix.pydantic-version == 'pydantic-v1'
         run: pip install "pydantic>=1.10.0,<2.0.0"
       - name: Install Pydantic v2
         if: matrix.pydantic-version == 'pydantic-v2'
         run: pip install --pre "pydantic>=2.0.0b2,<3.0.0"
       - run: mkdir coverage
@@ -113,15 +113,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing] orjson
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing] orjson
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m"(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
         env:
           COVERAGE_FILE: coverage/.coverage.orjson
           CONTEXT: orjson
       - name: Store coverage files
@@ -140,15 +140,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,docs,testing]
+        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
       - name: Test
         run: bash scripts/test.sh -m "(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
 
   test-windows-latest:
     if: github.event.pull_request.draft == false
     runs-on: windows-latest
     steps:
@@ -157,15 +157,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,docs,testing]
+        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
       - name: Test
         run: bash scripts/test.sh -m "(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
 
   test-kafka-real:
     if: github.event.pull_request.draft == false
     runs-on: ubuntu-latest
     services:
@@ -190,15 +190,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing]
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and kafka) or kafka"
         env:
           COVERAGE_FILE: coverage/.coverage.kafka-py
           CONTEXT: kafka-py
       - name: Store coverage files
@@ -250,15 +250,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing]
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and confluent) or confluent"
         env:
           COVERAGE_FILE: coverage/.coverage.confluent-py
           CONTEXT: confluent-py
       - name: Store coverage files
@@ -299,15 +299,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing]
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and rabbit) or rabbit"
         env:
           COVERAGE_FILE: coverage/.coverage.rabbit-py
           CONTEXT: rabbit-py
       - name: Store coverage files
@@ -348,15 +348,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing]
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and nats) or nats"
         env:
           COVERAGE_FILE: coverage/.coverage.nats-py
           CONTEXT: nats-py
       - name: Store coverage files
@@ -397,15 +397,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,docs,testing]
+        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and redis) or redis"
         env:
           COVERAGE_FILE: coverage/.coverage.redis-py
           CONTEXT: redis-py
       - name: Store coverage files
```

### Comparing `faststream-0.4.7/.github/workflows/update_release_notes.yaml` & `faststream-0.5.0rc0/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e02_1_basic_publisher.py` & `faststream-0.5.0rc0/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e02_2_basic_publisher.py` & `faststream-0.5.0rc0/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e02_3_basic_publisher.py` & `faststream-0.5.0rc0/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e03_miltiple_pubsub.py` & `faststream-0.5.0rc0/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e04_msg_filter.py` & `faststream-0.5.0rc0/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e07_ack_immediately.py` & `faststream-0.5.0rc0/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e09_testing_mocks.py` & `faststream-0.5.0rc0/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/e10_middlewares.py` & `faststream-0.5.0rc0/examples/e10_middlewares.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import asynccontextmanager
 from types import TracebackType
 from typing import Optional, Type
 
 from faststream import BaseMiddleware, FastStream
 from faststream.rabbit import RabbitBroker
 from faststream.types import DecodedMessage
 
@@ -11,28 +12,25 @@
         print(f"call toplevel middleware with msg: {self.msg}")
         return await super().on_receive()
 
     async def after_processed(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
+        exc_tb: Optional[TracebackType] = None,
     ) -> bool:
         print("highlevel middleware out")
-        return await super().after_processed(exc_type, exc_val, exec_tb)
+        return await super().after_processed(exc_type, exc_val, exc_tb)
 
 
-class HandlerMiddleware(BaseMiddleware):
-    async def on_consume(self, msg: DecodedMessage) -> DecodedMessage:
-        print(f"call handler middleware with body: {msg}")
-        return "fake message"
-
-    async def after_consume(self, err: Optional[Exception]) -> None:
-        print("handler middleware out")
-        return await super().after_consume(err)
+@asynccontextmanager
+async def HandlerMiddleware(msg: DecodedMessage) -> DecodedMessage:
+    print(f"call handler middleware with body: {msg}")
+    yield "fake message"
+    print("handler middleware out")
 
 
 broker = RabbitBroker(
     "amqp://guest:guest@localhost:5672/",
     middlewares=(TopLevelMiddleware,),
 )
 app = FastStream(broker)
```

### Comparing `faststream-0.4.7/examples/e11_settings.py` & `faststream-0.5.0rc0/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/fastapi_integration/testing.py` & `faststream-0.5.0rc0/examples/fastapi_integration/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import pytest_asyncio
 from fastapi.exceptions import RequestValidationError
 
-from faststream.rabbit.test import TestRabbitBroker
+from faststream.rabbit import TestRabbitBroker
 
 from .app import handler, publisher, router
 
 
 @pytest_asyncio.fixture
 async def broker():
     async with TestRabbitBroker(router.broker) as br:
```

### Comparing `faststream-0.4.7/examples/howto/structlogs.py` & `faststream-0.5.0rc0/examples/howto/structlogs.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 def merge_contextvars(
     logger: structlog.types.WrappedLogger,
     method_name: str,
     event_dict: structlog.types.EventDict,
 ) -> structlog.types.EventDict:
     event_dict["extra"] = event_dict.get(
         "extra",
-        context.get("log_context", {}),
+        context.get_local("log_context") or {},
     )
     return event_dict
 
 
-shared_processors = [
+shared_processors = (
     merge_contextvars,
     structlog.processors.add_log_level,
     structlog.processors.StackInfoRenderer(),
     structlog.dev.set_exc_info,
     structlog.processors.TimeStamper(fmt="iso"),
-]
+)
 
 if sys.stderr.isatty():
-    processors = shared_processors + [structlog.dev.ConsoleRenderer()]
+    processors = [
+        *shared_processors,
+        structlog.dev.ConsoleRenderer(),
+    ]
 else:
-    processors = shared_processors + [
+    processors = [
+        *shared_processors,
         structlog.processors.dict_tracebacks,
         structlog.processors.JSONRenderer(),
     ]
 
 structlog.configure(
     processors=processors,
     logger_factory=structlog.PrintLoggerFactory(),
```

### Comparing `faststream-0.4.7/examples/kafka/testing.py` & `faststream-0.5.0rc0/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/nats/e03_publisher.py` & `faststream-0.5.0rc0/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/nats/e04_js_basic.py` & `faststream-0.5.0rc0/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/nats/e05_basic_and_js.py` & `faststream-0.5.0rc0/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/nats/e06_key_value.py` & `faststream-0.5.0rc0/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/nats/e07_object_storage.py` & `faststream-0.5.0rc0/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/rabbit/direct.py` & `faststream-0.5.0rc0/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/rabbit/fanout.py` & `faststream-0.5.0rc0/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/rabbit/header.py` & `faststream-0.5.0rc0/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/rabbit/topic.py` & `faststream-0.5.0rc0/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/redis/channel_sub_pattern.py` & `faststream-0.5.0rc0/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/redis/rpc.py` & `faststream-0.5.0rc0/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/router/basic_publish.py` & `faststream-0.5.0rc0/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/serialization/avro/avro.py` & `faststream-0.5.0rc0/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/serialization/msgpack/pack.py` & `faststream-0.5.0rc0/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.0rc0/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/__init__.py` & `faststream-0.5.0rc0/faststream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A Python framework for building services interacting with Apache Kafka, RabbitMQ, NATS and Redis."""
 
 from faststream.annotations import ContextRepo, Logger, NoCast
 from faststream.app import FastStream
 from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.test import TestApp
+from faststream.testing.app import TestApp
 from faststream.utils import Context, Depends, Header, Path, apply_types, context
 
 __all__ = (
     # app
     "FastStream",
     "TestApp",
     # utils
```

### Comparing `faststream-0.4.7/faststream/_compat.py` & `faststream-0.5.0rc0/faststream/_compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from importlib.metadata import version as get_version
 from typing import Any, Callable, Dict, List, Mapping, Optional, Type, TypeVar, Union
 
 from fast_depends._compat import PYDANTIC_V2 as PYDANTIC_V2
 from fast_depends._compat import (  # type: ignore[attr-defined]
     PYDANTIC_VERSION as PYDANTIC_VERSION,
 )
-from pydantic import BaseModel
+from pydantic import BaseModel as BaseModel
 from typing_extensions import Never
 
 from faststream.types import AnyDict
 
 IS_WINDOWS = (
     sys.platform == "win32" or sys.platform == "cygwin" or sys.platform == "msys"
 )
@@ -70,14 +70,21 @@
             raise RequestValidationError(errors, ROUTER_VALIDATION_ERROR_MODEL)  # type: ignore[misc]
 
 except ImportError:
     HAS_FASTAPI = False
 
 JsonSchemaValue = Mapping[str, Any]
 
+PValidationError: Optional[Type[Exception]]
+try:
+    from pydantic import ValidationError
+    PValidationError = ValidationError
+except ImportError:
+    PValidationError = None
+
 if PYDANTIC_V2:
     if PYDANTIC_VERSION >= "2.4.0":
         from pydantic.annotated_handlers import (
             GetJsonSchemaHandler as GetJsonSchemaHandler,
         )
         from pydantic_core.core_schema import (  # type: ignore[attr-defined]
             with_info_plain_validator_function as with_info_plain_validator_function,
@@ -86,14 +93,15 @@
         from pydantic._internal._annotated_handlers import (  # type: ignore[no-redef]
             GetJsonSchemaHandler as GetJsonSchemaHandler,
         )
         from pydantic_core.core_schema import (
             general_plain_validator_function as with_info_plain_validator_function,
         )
 
+    from pydantic.fields import FieldInfo as FieldInfo
     from pydantic_core import CoreSchema as CoreSchema
     from pydantic_core import PydanticUndefined as PydanticUndefined
     from pydantic_core import to_jsonable_python
 
     SCHEMA_FIELD = "json_schema_extra"
     DEF_KEY = "$defs"
 
@@ -108,29 +116,24 @@
 
     def get_model_fields(model: Type[BaseModel]) -> Dict[str, Any]:
         return model.model_fields
 
     def model_to_json(model: BaseModel, **kwargs: Any) -> str:
         return model.model_dump_json(**kwargs)
 
-    def model_to_dict(model: BaseModel, **kwargs: Any) -> AnyDict:
-        return model.model_dump(**kwargs)
-
     def model_parse(
         model: Type[ModelVar], data: Union[str, bytes], **kwargs: Any
     ) -> ModelVar:
         return model.model_validate_json(data, **kwargs)
 
     def model_schema(model: Type[BaseModel], **kwargs: Any) -> AnyDict:
         return model.model_json_schema(**kwargs)
 
-    def model_copy(model: ModelVar, **kwargs: Any) -> ModelVar:
-        return model.model_copy(**kwargs)
-
 else:
+    from pydantic.fields import FieldInfo as FieldInfo
     from pydantic.json import pydantic_encoder
 
     GetJsonSchemaHandler = Any  # type: ignore[assignment,misc]
     CoreSchema = Any  # type: ignore[assignment,misc]
 
     SCHEMA_FIELD = "schema_extra"
     DEF_KEY = "definitions"
@@ -142,34 +145,28 @@
 
     def get_model_fields(model: Type[BaseModel]) -> Dict[str, Any]:
         return model.__fields__  # type: ignore[return-value]
 
     def model_to_json(model: BaseModel, **kwargs: Any) -> str:
         return model.json(**kwargs)
 
-    def model_to_dict(model: BaseModel, **kwargs: Any) -> AnyDict:
-        return model.dict(**kwargs)
-
     def model_parse(
         model: Type[ModelVar], data: Union[str, bytes], **kwargs: Any
     ) -> ModelVar:
         return model.parse_raw(data, **kwargs)
 
     def model_schema(model: Type[BaseModel], **kwargs: Any) -> AnyDict:
         return model.schema(**kwargs)
 
     def model_to_jsonable(
         model: BaseModel,
         **kwargs: Any,
     ) -> Any:
         return json_loads(model.json(**kwargs))
 
-    def model_copy(model: ModelVar, **kwargs: Any) -> ModelVar:
-        return model.copy(**kwargs)
-
     # TODO: pydantic types misc
     def with_info_plain_validator_function(  # type: ignore[misc]
         function: Callable[..., Any],
         *,
         ref: Optional[str] = None,
         metadata: Any = None,
         serialization: Any = None,
```

### Comparing `faststream-0.4.7/faststream/security.py` & `faststream-0.5.0rc0/faststream/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,35 @@
             Get the security requirements in the form of a list of dictionaries.
 
         get_schema(self) -> Dict[str, Dict[str, str]]:
             Get the security schema as a dictionary.
 
     """
 
+    ssl_context: Optional[SSLContext]
+    use_ssl: bool
+
     def __init__(
         self,
         ssl_context: Optional[SSLContext] = None,
         use_ssl: Optional[bool] = None,
     ) -> None:
         """Initialize the security configuration.
 
         Args:
             ssl_context (Optional[SSLContext]): An SSLContext object for SSL encryption. If None, SSL encryption is disabled.
             use_ssl (Optional[bool]): A boolean indicating whether to use SSL encryption. Defaults to True.
+            **kwargs (Any): inheritance options.
         """
         if ssl_context is not None:
             use_ssl = True
 
+        if use_ssl is None:
+            use_ssl = False
+
         self.use_ssl = use_ssl
         self.ssl_context = ssl_context
 
     def get_requirement(self) -> List[AnyDict]:
         """Get the security requirements.
 
         Returns:
@@ -79,17 +86,24 @@
 
     Methods:
         get_requirement(self) -> List[AnyDict]:
             Get the security requirements for SASL/PLAINTEXT authentication.
 
         get_schema(self) -> Dict[str, Dict[str, str]]:
             Get the security schema for SASL/PLAINTEXT authentication.
-
     """
 
+    # TODO: mv to SecretStr
+    __slots__ = (
+        "use_ssl",
+        "ssl_context",
+        "username",
+        "password",
+    )
+
     def __init__(
         self,
         username: str,
         password: str,
         ssl_context: Optional[SSLContext] = None,
         use_ssl: Optional[bool] = None,
     ) -> None:
@@ -97,17 +111,21 @@
 
         Args:
             username (str): The username for authentication.
             password (str): The password for authentication.
             ssl_context (Optional[SSLContext]): An SSLContext object for SSL encryption. If None, SSL encryption is disabled.
             use_ssl (Optional[bool]): A boolean indicating whether to use SSL encryption. Defaults to True.
         """
-        super().__init__(ssl_context, use_ssl)
-        self.username = username
-        self.password = password
+        super().__init__(
+            ssl_context=ssl_context,
+            use_ssl=use_ssl,
+        )
+
+        self.username=username
+        self.password=password
 
     def get_requirement(self) -> List[AnyDict]:
         """Get the security requirements for SASL/PLAINTEXT authentication.
 
         Returns:
             List[AnyDict]: A list of dictionaries representing security requirements.
         """
@@ -138,14 +156,22 @@
             Get the security requirements for SASL/SCRAM-SHA-256 authentication.
 
         get_schema(self) -> Dict[str, Dict[str, str]]:
             Get the security schema for SASL/SCRAM-SHA-256 authentication.
 
     """
 
+    # TODO: mv to SecretStr
+    __slots__ = (
+        "use_ssl",
+        "ssl_context",
+        "username",
+        "password",
+    )
+
     def __init__(
         self,
         username: str,
         password: str,
         ssl_context: Optional[SSLContext] = None,
         use_ssl: Optional[bool] = None,
     ) -> None:
@@ -153,17 +179,21 @@
 
         Args:
             username (str): The username for authentication.
             password (str): The password for authentication.
             ssl_context (Optional[SSLContext]): An SSLContext object for SSL encryption. If None, SSL encryption is disabled.
             use_ssl (Optional[bool]): A boolean indicating whether to use SSL encryption. Defaults to True.
         """
-        super().__init__(ssl_context, use_ssl)
-        self.username = username
-        self.password = password
+        super().__init__(
+            ssl_context=ssl_context,
+            use_ssl=use_ssl,
+        )
+
+        self.username=username
+        self.password=password
 
     def get_requirement(self) -> List[AnyDict]:
         """Get the security requirements for SASL/SCRAM-SHA-256 authentication.
 
         Returns:
             List[AnyDict]: A list of dictionaries representing security requirements.
         """
@@ -191,17 +221,24 @@
 
     Methods:
         get_requirement(self) -> List[AnyDict]:
             Get the security requirements for SASL/SCRAM-SHA-512 authentication.
 
         get_schema(self) -> Dict[str, Dict[str, str]]:
             Get the security schema for SASL/SCRAM-SHA-512 authentication.
-
     """
 
+    # TODO: mv to SecretStr
+    __slots__ = (
+        "use_ssl",
+        "ssl_context",
+        "username",
+        "password",
+    )
+
     def __init__(
         self,
         username: str,
         password: str,
         ssl_context: Optional[SSLContext] = None,
         use_ssl: Optional[bool] = None,
     ) -> None:
@@ -209,17 +246,21 @@
 
         Args:
             username (str): The username for authentication.
             password (str): The password for authentication.
             ssl_context (Optional[SSLContext]): An SSLContext object for SSL encryption. If None, SSL encryption is disabled.
             use_ssl (Optional[bool]): A boolean indicating whether to use SSL encryption. Defaults to True.
         """
-        super().__init__(ssl_context, use_ssl)
-        self.username = username
-        self.password = password
+        super().__init__(
+            ssl_context=ssl_context,
+            use_ssl=use_ssl,
+        )
+
+        self.username=username
+        self.password=password
 
     def get_requirement(self) -> List[AnyDict]:
         """Get the security requirements for SASL/SCRAM-SHA-512 authentication.
 
         Returns:
             List[AnyDict]: A list of dictionaries representing security requirements.
         """
```

### Comparing `faststream-0.4.7/faststream/asyncapi/generate.py` & `faststream-0.5.0rc0/faststream/asyncapi/generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 
 if TYPE_CHECKING:
     if HAS_FASTAPI:
         from faststream.broker.fastapi.router import StreamRouter
 
 
 def get_app_schema(app: Union[FastStream, "StreamRouter[Any]"]) -> Schema:
-    """Get the application schema.
-
-    Args:
-        app: An instance of FastStream or StreamRouter.
-
-    Returns:
-        The schema object.
+    """Get the application schema."""
+    broker = app.broker
+    if broker is None:  # pragma: no cover
+        raise RuntimeError()
+    broker.setup()
 
-    """
-    servers = get_app_broker_server(app)
-    channels = get_app_broker_channels(app)
+    servers = get_broker_server(broker)
+    channels = get_broker_channels(broker)
 
     messages: Dict[str, Message] = {}
     payloads: Dict[str, Dict[str, Any]] = {}
     for channel_name, ch in channels.items():
         ch.servers = list(servers.keys())
 
         if ch.subscribe is not None:
@@ -54,18 +51,14 @@
                 ch.publish.message = _resolve_msg_payloads(
                     m,
                     channel_name,
                     payloads,
                     messages,
                 )
 
-    broker = app.broker
-    if broker is None:  # pragma: no cover
-        raise RuntimeError()
-
     schema = Schema(
         info=Info(
             title=app.title,
             version=app.version,
             description=app.description,
             termsOfService=app.terms_of_service,
             contact=app.contact,
@@ -84,37 +77,18 @@
             if broker.security is None
             else broker.security.get_schema(),
         ),
     )
     return schema
 
 
-def get_app_broker_server(
-    app: Union[FastStream, "StreamRouter[Any]"],
-) -> Dict[str, Server]:
-    """Get the broker server for an application.
-
-    Args:
-        app: An instance of `FastStream` or `StreamRouter` representing the application.
-
-    Returns:
-        A dictionary containing the broker servers. The keys are the server names and the values are instances of `Server` class.
-
-    Raises:
-        AssertionError: If the `broker` attribute of the app is not present.
-
-    Note:
-        This function is currently incomplete and the following fields in the `broker_meta` dictionary are not populated: "security", "variables", "bindings".
-
-    """
+def get_broker_server(broker) -> Dict[str, Server]:
+    """Get the broker server for an application."""
     servers = {}
 
-    broker = app.broker
-    assert broker  # nosec B101
-
     broker_meta: Dict[str, Any] = {
         "protocol": broker.protocol,
         "protocolVersion": broker.protocol_version,
         "description": broker.description,
         "tags": broker.tags,
         # TODO
         # "variables": "",
@@ -142,36 +116,22 @@
                 url=url,
                 **broker_meta,
             )
 
     return servers
 
 
-def get_app_broker_channels(
-    app: Union[FastStream, "StreamRouter[Any]"],
-) -> Dict[str, Channel]:
-    """Get the broker channels for an application.
-
-    Args:
-        app: An instance of FastStream or StreamRouter.
-
-    Returns:
-        A dictionary of channel names and their corresponding Channel objects.
-
-    Raises:
-        AssertionError: If the app does not have a broker.
-
-    """
+def get_broker_channels(broker) -> Dict[str, Channel]:
+    """Get the broker channels for an application."""
     channels = {}
-    assert app.broker  # nosec B101
 
-    for h in app.broker.handlers.values():
+    for h in broker._subscribers.values():
         channels.update(h.schema())
 
-    for p in app.broker._publishers.values():
+    for p in broker._publishers.values():
         channels.update(p.schema())
 
     return channels
 
 
 def _resolve_msg_payloads(
     m: Message,
```

### Comparing `faststream-0.4.7/faststream/asyncapi/utils.py` & `faststream-0.5.0rc0/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/channels.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/info.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/main.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/message.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/operations.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/security.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/servers.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/utils.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+"""AsyncAPI AMQP bindings.
+
+References: https://github.com/asyncapi/bindings/tree/master/amqp
+"""
+
 from typing import Literal, Optional
 
 from pydantic import BaseModel, Field, PositiveInt
 
 
 class Queue(BaseModel):
     """A class to represent a queue.
 
     Attributes:
         name : name of the queue
         durable : indicates if the queue is durable
         exclusive : indicates if the queue is exclusive
         autoDelete : indicates if the queue should be automatically deleted
         vhost : virtual host of the queue (default is "/")
-
     """
 
     name: str
     durable: bool
     exclusive: bool
     autoDelete: bool
     vhost: str = "/"
@@ -27,44 +31,41 @@
 
     Attributes:
         name : name of the exchange (optional)
         type : type of the exchange, can be one of "default", "direct", "topic", "fanout", "headers"
         durable : whether the exchange is durable (optional)
         autoDelete : whether the exchange is automatically deleted (optional)
         vhost : virtual host of the exchange, default is "/"
-
     """
 
     name: Optional[str] = None
     type: Literal["default", "direct", "topic", "fanout", "headers"]
     durable: Optional[bool] = None
     autoDelete: Optional[bool] = None
     vhost: str = "/"
 
 
 class ServerBinding(BaseModel):
     """A class to represent a server binding.
 
     Attributes:
         bindingVersion : version of the binding (default: "0.2.0")
-
     """
 
     bindingVersion: str = "0.2.0"
 
 
 class ChannelBinding(BaseModel):
     """A class to represent channel binding.
 
     Attributes:
         is_ : Type of binding, can be "queue" or "routingKey"
         bindingVersion : Version of the binding
         queue : Optional queue object
         exchange : Optional exchange object
-
     """
 
     is_: Literal["queue", "routingKey"] = Field(..., alias="is")
     bindingVersion: str = "0.2.0"
     queue: Optional[Queue] = None
     exchange: Optional[Exchange] = None
 
@@ -73,15 +74,14 @@
     """A class to represent an operation binding.
 
     Attributes:
         cc : optional string representing the cc
         ack : boolean indicating if the operation is acknowledged
         replyTo : optional dictionary representing the replyTo
         bindingVersion : string representing the binding version
-
     """
 
     cc: Optional[str] = None
     ack: bool = True
     replyTo: Optional[str] = None
     deliveryMode: Optional[int] = None
     mandatory: Optional[bool] = None
```

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+"""AsyncAPI Kafka bindings.
+
+References: https://github.com/asyncapi/bindings/tree/master/kafka
+"""
+
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, PositiveInt
 
 
 class ServerBinding(BaseModel):
     """A class to represent a server binding.
 
     Attributes:
         bindingVersion : version of the binding (default: "0.4.0")
-
     """
 
     bindingVersion: str = "0.4.0"
 
 
 class ChannelBinding(BaseModel):
     """A class to represent a channel binding.
 
     Attributes:
         topic : optional string representing the topic
         partitions : optional positive integer representing the number of partitions
         replicas : optional positive integer representing the number of replicas
         bindingVersion : string representing the binding version
-
     """
 
     topic: Optional[str] = None
     partitions: Optional[PositiveInt] = None
     replicas: Optional[PositiveInt] = None
     # TODO:
     # topicConfiguration
@@ -37,14 +40,13 @@
     """A class to represent an operation binding.
 
     Attributes:
         groupId : optional dictionary representing the group ID
         clientId : optional dictionary representing the client ID
         replyTo : optional dictionary representing the reply-to
         bindingVersion : version of the binding (default: "0.4.0")
-
     """
 
     groupId: Optional[Dict[str, Any]] = None
     clientId: Optional[Dict[str, Any]] = None
     replyTo: Optional[Dict[str, Any]] = None
     bindingVersion: str = "0.4.0"
```

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
+"""AsyncAPI SQS bindings.
+
+References: https://github.com/asyncapi/bindings/tree/master/sqs
+"""
+
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel
 
 
 class ServerBinding(BaseModel):
     """A class to represent a server binding.
 
     Attributes:
         bindingVersion : version of the binding (default: "custom")
-
     """
 
     bindingVersion: str = "custom"
 
 
 class ChannelBinding(BaseModel):
     """A class to represent channel binding.
 
     Attributes:
-        subject : subject of the channel binding
-        queue : optional queue for the channel binding
-        bindingVersion : version of the channel binding, default is "custom"
-
+        queue : a dictionary representing the queue
+        bindingVersion : a string representing the binding version (default: "custom")
     """
 
-    subject: str
-    queue: Optional[str] = None
+    queue: Dict[str, Any]
     bindingVersion: str = "custom"
 
 
 class OperationBinding(BaseModel):
     """A class to represent an operation binding.
 
     Attributes:
         replyTo : optional dictionary containing reply information
-        bindingVersion : version of the binding (default is "custom")
-
+        bindingVersion : version of the binding, default is "custom"
     """
 
     replyTo: Optional[Dict[str, Any]] = None
     bindingVersion: str = "custom"
```

### Comparing `faststream-0.4.7/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+"""AsyncAPI Redis bindings.
+
+References: https://github.com/asyncapi/bindings/tree/master/redis
+"""
+
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel
 
 
 class ServerBinding(BaseModel):
     """A class to represent a server binding.
 
     Attributes:
         bindingVersion : version of the binding (default: "custom")
-
     """
 
     bindingVersion: str = "custom"
 
 
 class ChannelBinding(BaseModel):
     """A class to represent channel binding.
 
     Attributes:
         channel : the channel name
         method : the method used for binding (ssubscribe, psubscribe, subscribe)
         bindingVersion : the version of the binding
-
     """
 
     channel: str
     method: Optional[str] = None
     group_name: Optional[str] = None
     consumer_name: Optional[str] = None
     bindingVersion: str = "custom"
@@ -33,12 +36,11 @@
 
 class OperationBinding(BaseModel):
     """A class to represent an operation binding.
 
     Attributes:
         replyTo : optional dictionary containing reply information
         bindingVersion : version of the binding (default is "custom")
-
     """
 
     replyTo: Optional[Dict[str, Any]] = None
     bindingVersion: str = "custom"
```

### Comparing `faststream-0.4.7/faststream/broker/handler.py` & `faststream-0.5.0rc0/faststream/broker/subscriber/usecase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,426 +1,406 @@
-import asyncio
 from abc import abstractmethod
-from contextlib import AsyncExitStack, suppress
-from inspect import unwrap
+from contextlib import AsyncExitStack, asynccontextmanager
+from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
-    Awaitable,
+    AsyncIterator,
     Callable,
+    ContextManager,
     Dict,
     Generic,
+    Iterable,
     List,
     Optional,
-    Sequence,
     Tuple,
     Union,
-    cast,
+    overload,
 )
 
-import anyio
-from fast_depends.core import CallModel
 from typing_extensions import Self, override
 
-from faststream._compat import IS_OPTIMIZED
-from faststream.asyncapi.base import AsyncAPIOperation
+from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import parse_handler_params
 from faststream.asyncapi.utils import to_camelcase
-from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.subscriber.call_item import HandlerItem
+from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.types import (
-    AsyncDecoder,
-    AsyncParser,
-    CustomDecoder,
-    CustomParser,
-    Filter,
     MsgType,
     P_HandlerParams,
-    SyncDecoder,
-    SyncParser,
     T_HandlerReturn,
-    WrappedReturn,
 )
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.exceptions import HandlerException, StopConsume
-from faststream.types import AnyDict, SendableMessage
+from faststream.broker.utils import MultiLock, get_watcher_context, resolve_custom_func
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.exceptions import SetupError, StopConsume
 from faststream.utils.context.repository import context
-from faststream.utils.functions import to_async
+from faststream.utils.functions import sync_fake_context, to_async
 
 if TYPE_CHECKING:
-    from contextvars import Token
+    from fast_depends.dependencies import Depends
 
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.middlewares import BaseMiddleware
+    from faststream.broker.types import (
+        AsyncDecoder,
+        AsyncParser,
+        BrokerMiddleware,
+        CustomDecoder,
+        CustomParser,
+        Filter,
+        SubscriberMiddleware,
+    )
+    from faststream.types import AnyDict, LoggerProto
+
+
+class _CallOptions(Generic[MsgType]):
+    __slots__ = (
+        "filter",
+        "parser",
+        "decoder",
+        "middlewares",
+        "dependencies",
+    )
 
-class BaseHandler(AsyncAPIOperation, Generic[MsgType]):
-    """A base handler class for asynchronous API operations.
-
-    Attributes:
-        calls : List of tuples representing handler calls, filters, parsers, decoders, middlewares, and dependants.
-        global_middlewares : Sequence of global middlewares.
-
-    Methods:
-        __init__ : Initializes the BaseHandler object.
-        name : Returns the name of the handler.
-        call_name : Returns the name of the handler call.
-        description : Returns the description of the handler.
-        consume : Abstract method to consume a message.
-
-    Note: This class inherits from AsyncAPIOperation and is a generic class with type parameter MsgType.
-
-    """
-
-    calls: Union[
-        List[
-            Tuple[
-                HandlerCallWrapper[MsgType, Any, SendableMessage],  # handler
-                Callable[[StreamMessage[MsgType]], bool],  # filter
-                SyncParser[MsgType, StreamMessage[MsgType]],  # parser
-                SyncDecoder[StreamMessage[MsgType]],  # decoder
-                Sequence[Callable[[Any], BaseMiddleware]],  # middlewares
-                CallModel[Any, SendableMessage],  # dependant
-            ]
-        ],
-        List[
-            Tuple[
-                HandlerCallWrapper[MsgType, Any, SendableMessage],  # handler
-                Callable[[StreamMessage[MsgType]], Awaitable[bool]],  # filter
-                AsyncParser[MsgType, StreamMessage[MsgType]],  # parser
-                AsyncDecoder[StreamMessage[MsgType]],  # decoder
-                Sequence[Callable[[Any], BaseMiddleware]],  # middlewares
-                CallModel[Any, SendableMessage],  # dependant
-            ]
-        ],
-    ]
+    def __init__(
+        self,
+        *,
+        filter: "Filter[StreamMessage[MsgType]]",
+        parser: Optional["CustomParser[MsgType]"],
+        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        middlewares: Iterable["SubscriberMiddleware"],
+        dependencies: Iterable["Depends"],
+    ) -> None:
+        self.filter = filter
+        self.parser = parser
+        self.decoder = decoder
+        self.middlewares = middlewares
+        self.dependencies = dependencies
+
+
+class SubscriberUsecase(
+    AsyncAPIOperation,
+    SubscriberProto[MsgType],
+):
+    """A class representing an asynchronous handler."""
+
+    lock: ContextManager[Any]
+    extra_watcher_options: "AnyDict"
+    extra_context: "AnyDict"
+    graceful_timeout: Optional[float]
 
-    global_middlewares: Sequence[Callable[[Any], BaseMiddleware]]
+    _broker_dependecies: Iterable["Depends"]
+    _call_options: Optional["_CallOptions[MsgType]"]
 
     def __init__(
         self,
         *,
-        log_context_builder: Callable[[StreamMessage[Any]], Dict[str, str]],
-        description: Optional[str] = None,
-        title: Optional[str] = None,
-        include_in_schema: bool = True,
+        no_ack: bool,
+        retry: Union[bool, int],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
+        default_parser: "AsyncParser[MsgType]",
+        default_decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        # AsyncAPI information
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Initialize a new instance of the class.
-
-        Args:
-            log_context_builder: A callable that builds the log context.
-            description: Optional description of the instance.
-            title: Optional title of the instance.
-            include_in_schema: Whether to include the instance in the schema.
+        """Initialize a new instance of the class."""
+        self.calls = []
 
-        """
-        self.calls = []  # type: ignore[assignment]
-        self.global_middlewares = []
+        self._default_parser = default_parser
+        self._default_decoder = default_decoder
+        # Watcher args
+        self._no_ack = no_ack
+        self._retry = retry
 
-        self.log_context_builder = log_context_builder
+        self._call_options = None
         self.running = False
+        self.lock = sync_fake_context()
 
-        # AsyncAPI information
-        self._description = description
-        self._title = title
+        # Setup in include
+        self._broker_dependecies = broker_dependencies
+        self._broker_middlewares = broker_middlewares
+
+        # register in setup later
+        self._producer = None
+        self.graceful_timeout = None
+        self.extra_context = {}
+        self.extra_watcher_options = {}
+
+        # AsyncAPI
+        self.title_ = title_
+        self.description_ = description_
         self.include_in_schema = include_in_schema
 
-    @property
-    def call_name(self) -> str:
-        """Returns the name of the handler call."""
-        caller = unwrap(self.calls[0][0]._original_call)
-        name = getattr(caller, "__name__", str(caller))
-        return to_camelcase(name)
-
-    @property
-    def description(self) -> Optional[str]:
-        """Returns the description of the handler."""
-        if not self.calls:  # pragma: no cover
-            description = None
-
-        else:
-            caller = unwrap(self.calls[0][0]._original_call)
-            description = getattr(caller, "__doc__", None)
-
-        return self._description or description
-
-    @abstractmethod
-    def consume(self, msg: MsgType) -> SendableMessage:
-        """Consume a message.
-
-        Args:
-            msg: The message to be consumed.
-
-        Returns:
-            The sendable message.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
+    @override
+    def setup(  # type: ignore[override]
+        self,
+        *,
+        logger: Optional["LoggerProto"],
+        producer: Optional[ProducerProto],
+        graceful_timeout: Optional[float],
+        extra_context: Optional["AnyDict"],
+        # broker options
+        broker_parser: Optional["CustomParser[MsgType]"],
+        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        # dependant args
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
+    ) -> None:
+        self.lock = MultiLock()
 
-        """
-        raise NotImplementedError()
+        self._producer = producer
+        self.graceful_timeout = graceful_timeout
+        self.extra_context = extra_context or {}
 
-    def get_payloads(self) -> List[Tuple[AnyDict, str]]:
-        """Get the payloads of the handler."""
-        payloads: List[Tuple[AnyDict, str]] = []
+        self.watcher = get_watcher_context(logger, self._no_ack, self._retry)
 
-        for h, _, _, _, _, dep in self.calls:
-            body = parse_handler_params(
-                dep,
-                prefix=f"{self._title or self.call_name}:Message",
-            )
-            payloads.append(
-                (
-                    body,
-                    to_camelcase(unwrap(h._original_call).__name__),
-                ),
+        for call in self.calls:
+            if parser := call.item_parser or broker_parser:
+                async_parser = resolve_custom_func(to_async(parser), self._default_parser)
+            else:
+                async_parser = self._default_parser
+
+            if decoder := call.item_decoder or broker_decoder:
+                async_decoder = resolve_custom_func(to_async(decoder), self._default_decoder)
+            else:
+                async_decoder = self._default_decoder
+
+            call.setup(
+                parser=async_parser,
+                decoder=async_decoder,
+                apply_types=apply_types,
+                is_validate=is_validate,
+                _get_dependant=_get_dependant,
+                broker_dependencies=self._broker_dependecies,
             )
 
-        return payloads
+            call.handler.refresh(with_mock=False)
 
+    @abstractmethod
+    async def start(self) -> None:
+        """Start the handler."""
+        self.running = True
 
-class AsyncHandler(BaseHandler[MsgType]):
-    """A class representing an asynchronous handler.
+    @abstractmethod
+    async def close(self) -> None:
+        """Close the handler.
 
-    Attributes:
-        calls : a list of tuples containing the following information:
-            - handler : the handler function
-            - filter : a callable that filters the stream message
-            - parser : an async parser for the message
-            - decoder : an async decoder for the message
-            - middlewares : a sequence of middlewares
-            - dependant : a call model for the handler
-
-    Methods:
-        add_call : adds a new call to the list of calls
-        consume : consumes a message and returns a sendable message
-        start : starts the handler
-        close : closes the handler
-
-    """
-
-    calls: List[
-        Tuple[
-            HandlerCallWrapper[MsgType, Any, SendableMessage],  # handler
-            Callable[[StreamMessage[MsgType]], Awaitable[bool]],  # filter
-            AsyncParser[MsgType, Any],  # parser
-            AsyncDecoder[StreamMessage[MsgType]],  # decoder
-            Sequence[Callable[[Any], BaseMiddleware]],  # middlewares
-            CallModel[Any, SendableMessage],  # dependant
-        ]
-    ]
+        Blocks event loop up to graceful_timeout seconds.
+        """
+        self.running = False
+        if isinstance(self.lock, MultiLock):
+            await self.lock.wait_release(self.graceful_timeout)
 
-    def __init__(
+    def add_call(
         self,
         *,
-        log_context_builder: Callable[[StreamMessage[Any]], Dict[str, str]],
-        description: Optional[str] = None,
-        title: Optional[str] = None,
-        include_in_schema: bool = True,
-        graceful_timeout: Optional[float] = None,
-    ) -> None:
-        """Initialize a new instance of the class."""
-        super().__init__(
-            log_context_builder=log_context_builder,
-            description=description,
-            title=title,
-            include_in_schema=include_in_schema,
+        filter_: "Filter[StreamMessage[MsgType]]",
+        parser_: Optional["CustomParser[MsgType]"],
+        decoder_: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        middlewares_: Iterable["SubscriberMiddleware"],
+        dependencies_: Iterable["Depends"],
+    ) -> Self:
+        self._call_options = _CallOptions[MsgType](
+            filter=filter_,
+            parser=parser_,
+            decoder=decoder_,
+            middlewares=middlewares_,
+            dependencies=dependencies_,
         )
-        self.lock = MultiLock()
-        self.graceful_timeout = graceful_timeout
+        return self
 
-    def add_call(
+    @overload
+    def __call__(
         self,
+        func: None = None,
         *,
-        handler: HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-        parser: CustomParser[MsgType, Any],
-        decoder: CustomDecoder[Any],
-        dependant: CallModel[P_HandlerParams, T_HandlerReturn],
-        filter: Filter[StreamMessage[MsgType]],
-        middlewares: Optional[Sequence[Callable[[Any], BaseMiddleware]]],
-    ) -> None:
-        """Adds a call to the handler.
-
-        Args:
-            handler: The handler call wrapper.
-            parser: The custom parser.
-            decoder: The custom decoder.
-            dependant: The call model.
-            filter: The filter for stream messages.
-            middlewares: Optional sequence of middlewares.
+        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
+        parser: Optional["CustomParser[MsgType]"] = None,
+        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        middlewares: Iterable["SubscriberMiddleware"] = (),
+        dependencies: Iterable["Depends"] = (),
+    ) -> Callable[
+        [Callable[P_HandlerParams, T_HandlerReturn]],
+        "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
+    ]:
+        ...
 
-        Returns:
-            None
+    @overload
+    def __call__(
+        self,
+        func: Callable[P_HandlerParams, T_HandlerReturn],
+        *,
+        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
+        parser: Optional["CustomParser[MsgType]"] = None,
+        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        middlewares: Iterable["SubscriberMiddleware"] = (),
+        dependencies: Iterable["Depends"] = (),
+    ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]":
+        ...
 
-        """
-        self.calls.append(
-            (
-                handler,
-                to_async(filter),
-                to_async(parser) if parser else None,  # type: ignore[arg-type]
-                to_async(decoder) if decoder else None,  # type: ignore[arg-type]
-                middlewares or (),
-                dependant,
+    def __call__(
+        self,
+        func: Optional[Callable[P_HandlerParams, T_HandlerReturn]] = None,
+        *,
+        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
+        parser: Optional["CustomParser[MsgType]"] = None,
+        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        middlewares: Iterable["SubscriberMiddleware"] = (),
+        dependencies: Iterable["Depends"] = (),
+    ) -> Any:
+        if (options := self._call_options) is None:
+            raise SetupError("You can't create subscriber directly.")
+
+        total_deps = (*options.dependencies, *dependencies)
+        total_middlewares = (*options.middlewares, *middlewares)
+
+        def real_wrapper(
+            func: Callable[P_HandlerParams, T_HandlerReturn],
+        ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]":
+            handler = HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn](
+                func
             )
-        )
-
-    @override
-    async def consume(self, msg: MsgType) -> SendableMessage:  # type: ignore[override]
-        """Consume a message asynchronously.
-
-        Args:
-            msg: The message to be consumed.
 
-        Returns:
-            The sendable message.
+            self.calls.append(
+                HandlerItem[MsgType](
+                    handler=handler,
+                    filter=to_async(filter or options.filter),
+                    item_parser=parser or options.parser,
+                    item_decoder=decoder or options.decoder,
+                    item_middlewares=total_middlewares,
+                    dependencies=total_deps,
+                )
+            )
 
-        Raises:
-            StopConsume: If the consumption needs to be stopped.
+            return handler
 
-        Raises:
-            Exception: If an error occurs during consumption.
+        if func is None:
+            return real_wrapper
 
-        """
-        result: Optional[WrappedReturn[SendableMessage]] = None
-        result_msg: SendableMessage = None
+        else:
+            return real_wrapper(func)
 
+    async def consume(self, msg: MsgType) -> Any:
+        """Consume a message asynchronously."""
         if not self.running:
-            return result_msg
+            return None
 
-        log_context_tag: Optional["Token[Any]"] = None
         async with AsyncExitStack() as stack:
             stack.enter_context(self.lock)
 
+            # Enter context before middlewares
+            for k, v in self.extra_context.items():
+                stack.enter_context(context.scope(k, v))
+
             stack.enter_context(context.scope("handler_", self))
+            # Stop handler at StopConsume exception
+            await stack.enter_async_context(self._stop_scope())
+
+            # enter all middlewares
+            middlewares: List["BaseMiddleware"] = []
+            for base_m in self._broker_middlewares:
+                middleware = base_m(msg)
+                middlewares.append(middleware)
+                await middleware.__aenter__()
+
+            cache: Dict[Any, Any] = {}
+            for h in self.calls:
+                if (message := await h.is_suitable(msg, cache)) is not None:
+                    # Acknowledgement scope
+                    await stack.enter_async_context(
+                        self.watcher(
+                            message,
+                            **self.extra_watcher_options,
+                        )
+                    )
 
-            gl_middlewares: List[BaseMiddleware] = [
-                await stack.enter_async_context(m(msg)) for m in self.global_middlewares
-            ]
-
-            logged = False
-            processed = False
-            for handler, filter_, parser, decoder, middlewares, _ in self.calls:
-                local_middlewares: List[BaseMiddleware] = [
-                    await stack.enter_async_context(m(msg)) for m in middlewares
-                ]
-
-                all_middlewares = gl_middlewares + local_middlewares
-
-                # TODO: add parser & decoder caches
-                message = await parser(msg)
-
-                if not logged:  # pragma: no branch
-                    log_context_tag = context.set_local(
-                        "log_context",
-                        self.log_context_builder(message),
+                    stack.enter_context(
+                        context.scope("log_context", self.get_log_context(message))
                     )
+                    stack.enter_context(context.scope("message", message))
 
-                message.decoded_body = await decoder(message)
-                message.processed = processed
+                    # Middlewares should be exited before scope release
+                    for m in middlewares:
+                        stack.push_async_exit(m.__aexit__)
+
+                    result_msg = await h.call(
+                        message=message,
+                        # consumer middlewares
+                        _extra_middlewares=(m.consume_scope for m in middlewares),
+                    )
 
-                if await filter_(message):
-                    assert (  # nosec B101
-                        not processed
-                    ), "You can't process a message with multiple consumers"
-
-                    try:
-                        async with AsyncExitStack() as consume_stack:
-                            for m_consume in all_middlewares:
-                                message.decoded_body = (
-                                    await consume_stack.enter_async_context(
-                                        m_consume.consume_scope(message.decoded_body)
-                                    )
-                                )
-
-                            result = await cast(
-                                Awaitable[Optional[WrappedReturn[SendableMessage]]],
-                                handler.call_wrapped(message),
-                            )
-
-                        if result is not None:
-                            result_msg, pub_response = result
-
-                            # TODO: suppress all publishing errors and raise them after all publishers will be tried
-                            for publisher in (pub_response, *handler._publishers):
-                                if publisher is not None:
-                                    async with AsyncExitStack() as pub_stack:
-                                        result_to_send = result_msg
-
-                                        for m_pub in all_middlewares:
-                                            result_to_send = (
-                                                await pub_stack.enter_async_context(
-                                                    m_pub.publish_scope(result_to_send)
-                                                )
-                                            )
-
-                                        await publisher.publish(
-                                            message=result_to_send,
-                                            correlation_id=message.correlation_id,
-                                        )
-
-                    except StopConsume:
-                        await self.close()
-                        handler.trigger()
-
-                    except HandlerException as e:  # pragma: no cover
-                        handler.trigger()
-                        raise e
-
-                    except Exception as e:
-                        handler.trigger(error=e)
-                        raise e
-
-                    else:
-                        handler.trigger(result=result[0] if result else None)
-                        message.processed = processed = True
-                        if IS_OPTIMIZED:  # pragma: no cover
-                            break
+                    for p in chain(
+                        self._make_response_publisher(message),
+                        h.handler._publishers,
+                    ):
+                        await p.publish(
+                            result_msg,
+                            correlation_id=message.correlation_id,
+                            # publisher middlewares
+                            _extra_middlewares=(m.publish_scope for m in middlewares),
+                        )
+
+                    return result_msg
+
+            # Suitable handler is not founded
+            for m in middlewares:
+                stack.push_async_exit(m.__aexit__)
 
-            assert not self.running or processed, "You have to consume message"  # nosec B101
+            raise AssertionError(f"There is no suitable handler for {msg=}")
 
-        if log_context_tag is not None:
-            context.reset_local("log_context", log_context_tag)
+        return None
 
-        return result_msg
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[MsgType]"],
+    ) -> Dict[str, str]:
+        """Generate log context."""
+        return {
+            "message_id": getattr(message, "message_id", ""),
+        }
+
+    @asynccontextmanager
+    async def _stop_scope(self) -> AsyncIterator[None]:
+        try:
+            yield
+        except StopConsume:
+            await self.close()
+        except SystemExit:
+            await self.close()
+            context.get("app").exit()
 
-    @abstractmethod
-    async def start(self) -> None:
-        """Start the handler."""
-        self.running = True
+    # AsyncAPI methods
 
-    @abstractmethod
-    async def close(self) -> None:
-        """Close the handler."""
-        self.running = False
-        await self.lock.wait_release(self.graceful_timeout)
+    @property
+    def call_name(self) -> str:
+        """Returns the name of the handler call."""
+        return to_camelcase(self.calls[0].call_name)
 
+    def get_description(self) -> Optional[str]:
+        """Returns the description of the handler."""
+        if not self.calls:  # pragma: no cover
+            return None
 
-class MultiLock:
-    """A class representing a multi lock."""
+        else:
+            return self.calls[0].description
 
-    def __init__(self) -> None:
-        """Initialize a new instance of the class."""
-        self.queue: "asyncio.Queue[None]" = asyncio.Queue()
+    def get_payloads(self) -> List[Tuple["AnyDict", str]]:
+        """Get the payloads of the handler."""
+        payloads: List[Tuple["AnyDict", str]] = []
 
-    def __enter__(self) -> Self:
-        """Enter the context."""
-        self.queue.put_nowait(None)
-        return self
+        for h in self.calls:
+            if h.dependant is None:
+                raise SetupError("You should setup `Handler` at first.")
 
-    def __exit__(self, *args: Any, **kwargs: Any) -> None:
-        """Exit the context."""
-        with suppress(asyncio.QueueEmpty, ValueError):
-            self.queue.get_nowait()
-            self.queue.task_done()
+            body = parse_handler_params(
+                h.dependant,
+                prefix=f"{self.title_ or self.call_name}:Message",
+            )
 
-    @property
-    def qsize(self) -> int:
-        """Return the size of the queue."""
-        return self.queue.qsize()
+            payloads.append((body, to_camelcase(h.call_name)))
 
-    @property
-    def empty(self) -> bool:
-        """Return whether the queue is empty."""
-        return self.queue.empty()
-
-    async def wait_release(self, timeout: Optional[float] = None) -> None:
-        """Wait for the queue to be released."""
-        if timeout:
-            with anyio.move_on_after(timeout):
-                await self.queue.join()
+        return payloads
```

### Comparing `faststream-0.4.7/faststream/broker/middlewares.py` & `faststream-0.5.0rc0/faststream/confluent/testing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,280 +1,247 @@
-import logging
-from contextlib import asynccontextmanager
-from types import TracebackType
-from typing import Any, AsyncIterator, Optional, Type
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Tuple
 
-from typing_extensions import Self
+from typing_extensions import override
 
-from faststream.types import DecodedMessage, SendableMessage
-from faststream.utils.context.repository import context
-
-
-class BaseMiddleware:
-    """A base middleware class.
-
-    Attributes:
-        msg: Any - a message
-
-    Methods:
-        on_receive() -> None:
-            Called when a message is received.
-
-        after_processed(exc_type: Optional[Type[BaseException]] = None, exc_val: Optional[BaseException] = None, exec_tb: Optional[TracebackType] = None) -> Optional[bool]:
-            Called after processing a message.
-
-        __aenter__() -> Self:
-            Called when entering a context.
-
-        __aexit__(exc_type: Optional[Type[BaseException]] = None, exc_val: Optional[BaseException] = None, exec_tb: Optional[TracebackType] = None) -> Optional[bool]:
-            Called when exiting a context.
-
-        on_consume(msg: DecodedMessage) -> DecodedMessage:
-            Called before consuming a message.
-
-        after_consume(err: Optional[Exception]) -> None:
-            Called after consuming a message.
+from faststream.broker.message import encode_message, gen_cor_id
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.confluent.broker import KafkaBroker
+from faststream.confluent.publisher.asyncapi import (
+    AsyncAPIBatchPublisher,
+    AsyncAPIPublisher,
+)
+from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
+from faststream.confluent.subscriber.asyncapi import AsyncAPIBatchSubscriber
+from faststream.testing.broker import TestBroker, call_handler
+from faststream.types import SendableMessage
+
+__all__ = ("TestKafkaBroker",)
+
+
+class TestKafkaBroker(TestBroker[KafkaBroker]):
+    """A class to test Kafka brokers."""
+
+    @staticmethod
+    async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
+        broker._producer = FakeProducer(broker)
+
+    @staticmethod
+    def create_publisher_fake_subscriber(
+        broker: KafkaBroker,
+        publisher: AsyncAPIPublisher,
+    ) -> HandlerCallWrapper[Any, Any, Any]:
+        sub = broker.subscriber(  # type: ignore[call-overload,misc]
+            publisher.topic,
+            batch=isinstance(publisher, AsyncAPIBatchPublisher),
+        )
+
+        if not sub.calls:
+
+            @sub
+            def f(msg: Any) -> None:
+                pass
+
+            broker.setup_subscriber(sub)
+
+        return sub.calls[0].handler
+
+    @staticmethod
+    def remove_publisher_fake_subscriber(
+        broker: KafkaBroker,
+        publisher: AsyncAPIPublisher,
+    ) -> None:
+        broker._subscribers.pop(hash(publisher), None)
 
-        consume_scope(msg: DecodedMessage) -> AsyncIterator[DecodedMessage]:
-            Context manager for consuming a message.
 
-        on_publish(msg: SendableMessage) -> SendableMessage:
-            Called before publishing a message.
+class FakeProducer(AsyncConfluentFastProducer):
+    """A fake Kafka producer for testing purposes.
 
-        after_publish(err: Optional[Exception]) -> None:
-            Asynchronous function to handle the after publish event.
+    This class extends AsyncConfluentFastProducer and is used to simulate Kafka message publishing during tests.
     """
 
-    def __init__(self, msg: Any) -> None:
-        """Initialize the class.
-
-        Args:
-            msg: Any message to be stored.
-        """
-        self.msg = msg
-
-    async def on_receive(self) -> None:
-        pass
+    def __init__(self, broker: KafkaBroker) -> None:
+        self.broker = broker
 
-    async def after_processed(
+    @override
+    async def publish(  # type: ignore[override]
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> Optional[bool]:
-        """Asynchronously called after processing.
-
-        Args:
-            exc_type: Optional exception type
-            exc_val: Optional exception value
-            exec_tb: Optional traceback
-
-        Returns:
-            Optional boolean value indicating whether the processing was successful or not.
-        """
-        return False
-
-    async def __aenter__(self) -> Self:
-        await self.on_receive()
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> Optional[bool]:
-        """Exit the asynchronous context manager.
-
-        Args:
-            exc_type: The type of the exception raised, if any.
-            exc_val: The exception instance raised, if any.
-            exec_tb: The traceback for the exception raised, if any.
-
-        Returns:
-            A boolean indicating whether the exception was handled or not.
-        """
-        return await self.after_processed(exc_type, exc_val, exec_tb)
-
-    async def on_consume(self, msg: DecodedMessage) -> DecodedMessage:
-        """Asynchronously consumes a message.
-
-        Args:
-            msg: The message to be consumed.
-
-        Returns:
-            The consumed message.
-        """
-        return msg
-
-    async def after_consume(self, err: Optional[Exception]) -> None:
-        """A function to handle the result of consuming a resource asynchronously.
-
-        Args:
-            err : Optional exception that occurred during consumption
-
-        Raises:
-            err : If an exception occurred during consumption
-        """
-        if err is not None:
-            raise err
-
-    @asynccontextmanager
-    async def consume_scope(self, msg: DecodedMessage) -> AsyncIterator[DecodedMessage]:
-        """Asynchronously consumes a message and returns an asynchronous iterator of decoded messages.
-
-        Args:
-            msg: The decoded message to consume.
-
-        Yields:
-            An asynchronous iterator of decoded messages.
-
-        Returns:
-            An asynchronous iterator of decoded messages.
-
-        Raises:
-            Exception: If an error occurs while consuming the message.
-
-        AsyncIterator:
-            An asynchronous iterator that yields decoded messages.
-
-        Note:
-            This function is an async function.
-        """
-        err: Optional[Exception]
-        try:
-            yield await self.on_consume(msg)
-        except Exception as e:
-            err = e
-        else:
-            err = None
-        await self.after_consume(err)
-
-    async def on_publish(self, msg: SendableMessage) -> SendableMessage:
-        """Asynchronously handle a publish event.
-
-        Args:
-            msg: The message to be published.
-
-        Returns:
-            The published message.
-        """
-        return msg
-
-    async def after_publish(self, err: Optional[Exception]) -> None:
-        """Asynchronous function to handle the after publish event.
-
-        Args:
-            err: Optional exception that occurred during the publish
-
-        Returns:
-            None
-
-        Raises:
-            Exception: If an error occurred during the publish
-        """
-        if err is not None:
-            raise err
-
-    @asynccontextmanager
-    async def publish_scope(
-        self, msg: SendableMessage
-    ) -> AsyncIterator[SendableMessage]:
-        """Publish a message and return an async iterator.
-
-        Args:
-            msg: The message to be published.
-
-        Yields:
-            A sendable message.
-
-        Returns:
-            An async iterator of sendable messages.
-
-        Raises:
-            Exception: If an error occurs during publishing.
-
-        """
-        err: Optional[Exception]
-        try:
-            yield await self.on_publish(msg)
-        except Exception as e:
-            err = e
-        else:
-            err = None
-        await self.after_publish(err)
-
-
-class CriticalLogMiddleware(BaseMiddleware):
-    """A middleware class for logging critical errors.
-
-    Args:
-        logger: The logger object to use for logging
+        message: SendableMessage,
+        topic: str,
+        key: Optional[bytes] = None,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[Dict[str, str]] = None,
+        correlation_id: Optional[str] = None,
+        *,
+        reply_to: str = "",
+        rpc: bool = False,
+        rpc_timeout: Optional[float] = None,
+        raise_timeout: bool = False,
+    ) -> Optional[Any]:
+        """Publish a message to the Kafka broker."""
+        correlation_id = correlation_id or gen_cor_id()
+
+        incoming = build_message(
+            message=message,
+            topic=topic,
+            key=key,
+            partition=partition,
+            timestamp_ms=timestamp_ms,
+            headers=headers,
+            correlation_id=correlation_id,
+            reply_to=reply_to,
+        )
+
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            if topic in handler.topics:
+                return await call_handler(
+                    handler=handler,
+                    message=[incoming]
+                    if isinstance(handler, AsyncAPIBatchSubscriber)
+                    else incoming,
+                    rpc=rpc,
+                    rpc_timeout=rpc_timeout,
+                    raise_timeout=raise_timeout,
+                )
 
-    Methods:
-        __call__(msg: Any) -> Self: Returns the middleware instance
-        after_processed(exc_type: Optional[Type[BaseException]] = None, exc_val: Optional[BaseException] = None, exec_tb: Optional[TracebackType] = None) -> bool: Logs critical errors if they occur and returns True
-    """
+        return None
 
-    def __init__(
+    async def publish_batch(
         self,
-        logger: Optional[logging.Logger],
-        log_level: int,
+        *msgs: SendableMessage,
+        topic: str,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[Dict[str, str]] = None,
+        reply_to: str = "",
+        correlation_id: Optional[str] = None,
     ) -> None:
-        """Initialize the class.
-
-        Args:
-            logger: an instance of the logging.Logger class
-            log_level: the log level to use for logging
-
-        Returns:
-            None
-        """
-        self.logger = logger
-        self.log_level = log_level
-
-    def __call__(self, msg: Any) -> Self:
-        """Call the object with a message.
+        """Publish a batch of messages to the Kafka broker."""
+        correlation_id = correlation_id or gen_cor_id()
 
-        Args:
-            msg: Any message to be passed to the object.
-
-        Returns:
-            The object itself.
-        """
-        return self
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            if topic in handler.topics:
+                messages = (
+                    build_message(
+                        message=message,
+                        topic=topic,
+                        partition=partition,
+                        timestamp_ms=timestamp_ms,
+                        headers=headers,
+                        correlation_id=correlation_id,
+                        reply_to=reply_to,
+                    )
+                    for message in msgs
+                )
 
-    async def on_consume(self, msg: DecodedMessage) -> DecodedMessage:
-        if self.logger is not None:
-            c = context.get_local("log_context")
-            self.logger.log(self.log_level, "Received", extra=c)
+                if isinstance(handler, AsyncAPIBatchSubscriber):
+                    await call_handler(
+                        handler=handler,
+                        message=list(messages),
+                    )
+
+                else:
+                    for m in messages:
+                        await call_handler(
+                            handler=handler,
+                            message=m,
+                        )
+        return None
 
-        return await super().on_consume(msg)
 
-    async def after_processed(
+class MockConfluentMessage:
+    def __init__(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> bool:
-        """Asynchronously called after processing.
-
-        Args:
-            exc_type (Optional[Type[BaseException]]): Type of the exception raised during processing.
-            exc_val (Optional[BaseException]): Value of the exception raised during processing.
-            exec_tb (Optional[TracebackType]): Traceback of the exception raised during processing.
-
-        Returns:
-            bool: True if the method is successfully executed.
-        """
-        if self.logger is not None:
-            c = context.get_local("log_context")
-
-            if exc_type and exc_val:
-                self.logger.error(
-                    f"{exc_type.__name__}: {exc_val}",
-                    exc_info=exc_val,
-                    extra=c,
-                )
+        raw_msg: bytes,
+        topic: str,
+        key: bytes,
+        headers: List[Tuple[str, bytes]],
+        offset: int,
+        partition: int,
+        timestamp_type: int,
+        timestamp_ms: int,
+        error: Optional[str] = None,
+    ):
+        self._raw_msg = raw_msg
+        self._topic = topic
+        self._key = key
+        self._headers = headers
+        self._error = error
+        self._offset = offset
+        self._partition = partition
+        self._timestamp = (timestamp_type, timestamp_ms)
+
+    def len(self) -> int:
+        return len(self._raw_msg)
+
+    def error(self) -> Optional[str]:
+        return self._error
+
+    def headers(self) -> List[Tuple[str, bytes]]:
+        return self._headers
+
+    def key(self) -> bytes:
+        return self._key
+
+    def offset(self) -> int:
+        return self._offset
+
+    def partition(self) -> int:
+        return self._partition
+
+    def timestamp(self) -> Tuple[int, int]:
+        return self._timestamp
+
+    def topic(self) -> str:
+        return self._topic
+
+    def value(self) -> bytes:
+        return self._raw_msg
+
+
+def build_message(
+    message: SendableMessage,
+    topic: str,
+    *,
+    correlation_id: str,
+    partition: Optional[int] = None,
+    timestamp_ms: Optional[int] = None,
+    key: Optional[bytes] = None,
+    headers: Optional[Dict[str, str]] = None,
+    reply_to: str = "",
+) -> MockConfluentMessage:
+    """Build a mock confluent_kafka.Message for a sendable message.
 
-            self.logger.log(self.log_level, "Processed", extra=c)
-        return True
+    Args:
+        message (SendableMessage): The sendable message to be encoded.
+        topic (str): The Kafka topic for the message.
+        partition (Optional[int], optional): The Kafka partition for the message. Defaults to None.
+        timestamp_ms (Optional[int], optional): The message timestamp in milliseconds. Defaults to None.
+        key (Optional[bytes], optional): The message key. Defaults to None.
+        headers (Optional[Dict[str, str]], optional): Additional headers for the message. Defaults to None.
+        correlation_id (Optional[str], optional): The correlation ID for the message. Defaults to None.
+        reply_to (str, optional): The topic to which responses should be sent. Defaults to "".
+
+    Returns:
+        MockConfluentMessage: A mock confluent_kafka.Message object.
+    """
+    msg, content_type = encode_message(message)
+    k = key or b""
+    headers = {
+        "content-type": content_type or "",
+        "correlation_id": correlation_id,
+        "reply_to": reply_to,
+        **(headers or {}),
+    }
+
+    # https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html#confluent_kafka.Message.timestamp
+    return MockConfluentMessage(
+        raw_msg=msg,
+        topic=topic,
+        key=k,
+        headers=[(i, j.encode()) for i, j in headers.items()],
+        offset=0,
+        partition=partition or 0,
+        timestamp_type=0 + 1,
+        timestamp_ms=timestamp_ms or int(datetime.now().timestamp()),
+    )
```

### Comparing `faststream-0.4.7/faststream/broker/publisher.py` & `faststream-0.5.0rc0/faststream/broker/publisher/usecase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,142 @@
-from abc import abstractmethod
-from dataclasses import dataclass, field
+from abc import ABC
 from inspect import unwrap
-from typing import Any, Callable, Generic, List, Optional, Tuple
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+)
 from unittest.mock import MagicMock
 
 from fast_depends._compat import create_model, get_config_base
 from fast_depends.core import CallModel, build_call_model
+from typing_extensions import Annotated, Doc, override
 
-from faststream.asyncapi.base import AsyncAPIOperation
+from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import get_response_schema
 from faststream.asyncapi.utils import to_camelcase
-from faststream.broker.types import MsgType, P_HandlerParams, T_HandlerReturn
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.types import AnyDict, SendableMessage
-
-
-@dataclass
-class BasePublisher(AsyncAPIOperation, Generic[MsgType]):
-    """A base class for publishers in an asynchronous API.
-
-    Attributes:
-        title : optional title of the publisher
-        _description : optional description of the publisher
-        _fake_handler : boolean indicating if a fake handler is used
-        calls : list of callable objects
-        mock : MagicMock object for mocking purposes
-
-    Methods:
-        description() : returns the description of the publisher
-        __call__(func) : decorator to register a function as a handler for the publisher
-        publish(message, correlation_id, **kwargs) : publishes a message with optional correlation ID
-
-    Raises:
-        NotImplementedError: if the publish method is not implemented.
-
-    """
-
-    title: Optional[str] = field(default=None)
-    _description: Optional[str] = field(default=None)
-    _schema: Optional[Any] = field(default=None)
-
-    calls: List[Callable[..., Any]] = field(
-        init=False, default_factory=list, repr=False
-    )
-    _fake_handler: bool = field(default=False, repr=False)
-    mock: Optional[MagicMock] = field(init=False, default=None, repr=False)
-
-    @property
-    def description(self) -> Optional[str]:
-        return self._description
+from faststream.broker.publisher.proto import ProducerProto, PublisherProto
+from faststream.broker.types import (
+    BrokerMiddleware,
+    MsgType,
+    P_HandlerParams,
+    PublisherMiddleware,
+    T_HandlerReturn,
+)
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.types import AnyDict
+
+
+class PublisherUsecase(
+    ABC,
+    AsyncAPIOperation,
+    PublisherProto[MsgType],
+):
+    """A base class for publishers in an asynchronous API."""
+
+    mock: Optional[MagicMock]
+    calls: List[Callable[..., Any]]
+
+    def __init__(
+        self,
+        *,
+        broker_middlewares: Annotated[
+            Iterable[BrokerMiddleware[MsgType]],
+            Doc("Top-level middlewares to use in direct `.publish` call."),
+        ],
+        middlewares: Annotated[
+            Iterable[PublisherMiddleware],
+            Doc("Publisher middlewares."),
+        ],
+        # AsyncAPI args
+        schema_: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type"
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
+        ],
+        title_: Annotated[
+            Optional[str],
+            Doc("AsyncAPI object title."),
+        ],
+        description_: Annotated[
+            Optional[str],
+            Doc("AsyncAPI object description."),
+        ],
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ],
+    ) -> None:
+        self.calls = []
+        self._middlewares = middlewares
+        self._broker_middlewares = broker_middlewares
+        self._producer = None
+
+        self._fake_handler = False
+        self.mock = None
+
+        # AsyncAPI
+        self.title_ = title_
+        self.description_ = description_
+        self.include_in_schema = include_in_schema
+        self.schema_ = schema_
+
+    @override
+    def setup(  # type: ignore[override]
+        self,
+        *,
+        producer: Optional[ProducerProto],
+    ) -> None:
+        self._producer = producer
 
     def set_test(
         self,
-        mock: MagicMock,
-        with_fake: bool,
+        *,
+        mock: Annotated[
+            MagicMock,
+            Doc("Mock object to check in tests."),
+        ],
+        with_fake: Annotated[
+            bool,
+            Doc("Whetevet publisher's fake subscriber created or not."),
+        ],
     ) -> None:
+        """Turn publisher to testing mode."""
         self.mock = mock
         self._fake_handler = with_fake
 
     def reset_test(self) -> None:
+        """Turn off publisher's testing mode."""
         self._fake_handler = False
         self.mock = None
 
     def __call__(
         self,
         func: Callable[P_HandlerParams, T_HandlerReturn],
     ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
-        """This is a Python function.
-
-        Args:
-            func: A callable object that takes `P_HandlerParams` as input and returns `T_HandlerReturn`.
-
-        Returns:
-            An instance of `HandlerCallWrapper` class.
-
-        Raises:
-            TypeError: If `func` is not callable.
-
-        """
-        handler_call: HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn] = (
-            HandlerCallWrapper(func)
-        )
+        """Decorate user's function by current publisher."""
+        handler_call = HandlerCallWrapper[
+            MsgType,
+            P_HandlerParams,
+            T_HandlerReturn,
+        ](func)
         handler_call._publishers.append(self)
         self.calls.append(handler_call._original_call)
         return handler_call
 
-    @abstractmethod
-    async def publish(
-        self,
-        message: SendableMessage,
-        correlation_id: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Optional[SendableMessage]:
-        """Publish a message.
-
-        Args:
-            message: The message to be published.
-            correlation_id: Optional correlation ID for the message.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            The published message.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        raise NotImplementedError()
-
     def get_payloads(self) -> List[Tuple[AnyDict, str]]:
         payloads: List[Tuple[AnyDict, str]] = []
 
-        if self._schema:
-            params = {"response__": (self._schema, ...)}
+        if self.schema_:
+            params = {"response__": (self.schema_, ...)}
 
             call_model: CallModel[Any, Any] = CallModel(
                 call=lambda: None,
                 model=create_model("Fake"),
                 response_model=create_model(  # type: ignore[call-overload]
                     "",
                     __config__=get_config_base(),  # type: ignore[arg-type]
```

### Comparing `faststream-0.4.7/faststream/broker/router.py` & `faststream-0.5.0rc0/faststream/broker/core/usecase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,343 +1,342 @@
+import logging
 from abc import abstractmethod
+from contextlib import AsyncExitStack
 from typing import (
+    TYPE_CHECKING,
     Any,
-    AsyncContextManager,
     Callable,
-    Dict,
     Generic,
+    Iterable,
     List,
     Optional,
-    Sequence,
-    Tuple,
-    TypeVar,
+    Type,
+    Union,
+    cast,
 )
 
-from fast_depends.dependencies import Depends
+from typing_extensions import Annotated, Doc, Self
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.publisher import BasePublisher
+from faststream._compat import is_test_env
+from faststream.broker.core.logging import LoggingBroker
+from faststream.broker.middlewares.logging import CriticalLogMiddleware
+from faststream.broker.proto import SetupAble
+from faststream.broker.publisher.proto import ProducerProto, PublisherProto
+from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.types import (
+    AsyncCustomDecoder,
+    AsyncCustomParser,
+    BrokerMiddleware,
+    ConnectionType,
     CustomDecoder,
     CustomParser,
     MsgType,
-    P_HandlerParams,
-    T_HandlerReturn,
 )
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.types import AnyDict, SendableMessage
-
-PublisherKeyType = TypeVar("PublisherKeyType")
-
-
-class BrokerRoute(Generic[MsgType, T_HandlerReturn]):
-    """A generic class to represent a broker route.
-
-    Attributes:
-        call : callable object representing the route
-        args : tuple of arguments for the route
-        kwargs : dictionary of keyword arguments for the route
-
-    Args:
-        call : callable object representing the route
-        *args : variable length arguments for the route
-        **kwargs : variable length keyword arguments for the route
-
-    """
-
-    call: Callable[..., T_HandlerReturn]
-    args: Tuple[Any, ...]
-    kwargs: AnyDict
+from faststream.exceptions import NOT_CONNECTED_YET
+from faststream.log.logging import set_logger_fmt
+from faststream.utils.context.repository import context
+from faststream.utils.functions import to_async
+
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from fast_depends.dependencies import Depends
+
+    from faststream.asyncapi.schema import Tag, TagDict
+    from faststream.broker.message import StreamMessage
+    from faststream.security import BaseSecurity
+    from faststream.types import AnyDict, LoggerProto
+
+
+class BrokerUsecase(
+    LoggingBroker[MsgType],
+    SetupAble,
+    Generic[MsgType, ConnectionType],
+):
+    """A class representing a broker async use case."""
+
+    url: Union[str, Iterable[str], None]
+    _connection: Optional[ConnectionType]
+    _producer: Optional[ProducerProto]
 
     def __init__(
         self,
-        call: Callable[..., T_HandlerReturn],
-        *args: Any,
-        **kwargs: Any,
+        *,
+        decoder: Annotated[
+            Optional["CustomDecoder[StreamMessage[MsgType]]"],
+            Doc("Custom decoder object."),
+        ],
+        parser: Annotated[
+            Optional["CustomParser[MsgType]"],
+            Doc("Custom parser object."),
+        ],
+        dependencies: Annotated[
+            Iterable["Depends"],
+            Doc("Dependencies to apply to all broker subscribers."),
+        ],
+        middlewares: Annotated[
+            Iterable["BrokerMiddleware[MsgType]"],
+            Doc("Middlewares to apply to all broker publishers/subscribers."),
+        ],
+        graceful_timeout: Annotated[
+            Optional[float],
+            Doc(
+                "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
+            ),
+        ],
+        # Logging args
+        default_logger: Annotated[
+            logging.Logger,
+            Doc("Logger object to use if `logger` is not setted."),
+        ],
+        logger: Annotated[
+            Union["LoggerProto", None, object],
+            Doc("User specified logger to pass into Context and log service messages."),
+        ],
+        log_level: Annotated[
+            int,
+            Doc("Service messages log level."),
+        ],
+        log_fmt: Annotated[
+            Optional[str],
+            Doc("Default logger log format."),
+        ],
+        # FastDepends args
+        apply_types: Annotated[
+            bool,
+            Doc("Whether to use FastDepends or not."),
+        ],
+        validate: Annotated[
+            bool,
+            Doc("Whether to cast types using Pydantic validation."),
+        ],
+        _get_dependant: Annotated[
+            Optional[Callable[..., Any]],
+            Doc("Custom library dependant generator callback."),
+        ],
+        # AsyncAPI kwargs
+        protocol: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server protocol."),
+        ],
+        protocol_version: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server protocol version."),
+        ],
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server description."),
+        ],
+        tags: Annotated[
+            Optional[Iterable[Union["Tag", "TagDict"]]],
+            Doc("AsyncAPI server tags."),
+        ],
+        asyncapi_url: Annotated[
+            Union[str, List[str], None],
+            Doc("AsyncAPI hardcoded server addresses."),
+        ],
+        security: Annotated[
+            Optional["BaseSecurity"],
+            Doc(
+                "Security options to connect broker and generate AsyncAPI server security."
+            ),
+        ],
+        **connection_kwargs: Any,
     ) -> None:
-        """Initialize a callable object with arguments and keyword arguments.
-
-        Args:
-            call: A callable object.
-            *args: Positional arguments to be passed to the callable object.
-            **kwargs: Keyword arguments to be passed to the callable object.
-
-        """
-        self.call = call
-        self.args = args
-        self.kwargs = kwargs
-
-
-class BrokerRouter(Generic[PublisherKeyType, MsgType]):
-    """A generic class representing a broker router.
-
-    Attributes:
-        prefix : prefix for the router
-        _handlers : list of broker routes
-        _publishers : dictionary of publishers
-
-    Methods:
-        _get_publisher_key : abstract method to get the publisher key
-        _update_publisher_prefix : abstract method to update the publisher prefix
-        __init__ : constructor method
-        subscriber : abstract method to define a subscriber
-        _wrap_subscriber : method to wrap a subscriber function
-        publisher : abstract method to define a publisher
-        include_router : method to include a router
-        include_routers : method to include multiple routers
-
-    """
-
-    prefix: str
-    _handlers: List[BrokerRoute[MsgType, Any]]
-    _publishers: Dict[PublisherKeyType, BasePublisher[MsgType]]
-
-    @staticmethod
-    @abstractmethod
-    def _get_publisher_key(publisher: BasePublisher[MsgType]) -> PublisherKeyType:
-        """This is a Python function.
-
-        _get_publisher_key function:
-
-        Args:
-            publisher: An instance of BasePublisher class.
-
-        Returns:
-            The publisher key.
-
-        Raises:
-            NotImplementedError: This function is not implemented.
-
-        """
-        raise NotImplementedError()
-
-    @staticmethod
-    @abstractmethod
-    def _update_publisher_prefix(
-        prefix: str,
-        publisher: BasePublisher[MsgType],
-    ) -> BasePublisher[MsgType]:
-        """Updates the publisher prefix.
-
-        Args:
-            prefix: The new prefix to be set.
-            publisher: The publisher to update.
-
-        Returns:
-            The updated publisher.
-
-        Raises:
-            NotImplementedError: If the function is not implemented.
+        super().__init__(
+            middlewares=middlewares,
+            dependencies=dependencies,
+            decoder=cast(
+                Optional["AsyncCustomDecoder[StreamMessage[MsgType]]"],
+                to_async(decoder) if decoder else None,
+            ),
+            parser=cast(
+                Optional["AsyncCustomParser[MsgType]"],
+                to_async(parser) if parser else None,
+            ),
+            # Broker is a root router
+            include_in_schema=True,
+            prefix="",
+            # Logging args
+            default_logger=default_logger,
+            log_level=log_level,
+            log_fmt=log_fmt,
+            logger=logger,
+        )
+
+        self.running = False
+        self.graceful_timeout = graceful_timeout
+
+        self._connection_kwargs = connection_kwargs
+        self._connection = None
+        self._producer = None
+
+        if not is_test_env():
+            self._middlewares = (
+                CriticalLogMiddleware(self.logger, log_level),
+                *self._middlewares,
+            )
 
-        """
-        raise NotImplementedError()
+        # TODO: move this context to Handlers' extra_context to support multiple brokers
+        context.set_global("logger", self.logger)
+        context.set_global("broker", self)
+
+        # FastDepends args
+        self._is_apply_types = apply_types
+        self._is_validate = validate
+        self._get_dependant = _get_dependant
+
+        # AsyncAPI information
+        self.url = asyncapi_url
+        self.protocol = protocol
+        self.protocol_version = protocol_version
+        self.description = description
+        self.tags = tags
+        self.security = security
+
+    async def __aenter__(self) -> "Self":
+        await self.connect()
+        return self
 
-    def __init__(
+    async def __aexit__(
         self,
-        prefix: str = "",
-        handlers: Sequence[BrokerRoute[MsgType, SendableMessage]] = (),
-        dependencies: Sequence[Depends] = (),
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [StreamMessage[MsgType]],
-                    AsyncContextManager[None],
-                ]
-            ]
-        ] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        include_in_schema: Optional[bool] = None,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional["TracebackType"],
     ) -> None:
-        """Initialize a class object.
-
-        Args:
-            prefix (str): Prefix for the object.
-            handlers (Sequence[BrokerRoute[MsgType, SendableMessage]]): Handlers for the object.
-            dependencies (Sequence[Depends]): Dependencies for the object.
-            middlewares (Optional[Sequence[Callable[[StreamMessage[MsgType]], AsyncContextManager[None]]]]): Middlewares for the object.
-            parser (Optional[CustomParser[MsgType]]): Parser for the object.
-            decoder (Optional[CustomDecoder[StreamMessage[MsgType]]]): Decoder for the object.
-            include_in_schema (Optional[bool]): Whether to include the object in the schema.
-
-        """
-        self.prefix = prefix
-        self.include_in_schema = include_in_schema
-        self._handlers = list(handlers)
-        self._publishers = {}
-        self._dependencies = dependencies
-        self._middlewares = middlewares
-        self._parser = parser
-        self._decoder = decoder
+        await self.close(exc_type, exc_val, exc_tb)
 
     @abstractmethod
-    def subscriber(
-        self,
-        subj: str,
-        *args: Any,
-        dependencies: Sequence[Depends] = (),
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [StreamMessage[MsgType]],
-                    AsyncContextManager[None],
-                ]
-            ]
-        ] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        include_in_schema: Optional[bool] = None,
-        **kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-    ]:
-        """A function to subscribe to a subject.
-
-        Args:
-            subj : subject to subscribe to
-            *args : additional arguments
-            dependencies : sequence of dependencies
-            middlewares : optional sequence of middlewares
-            parser : optional custom parser
-            decoder : optional custom decoder
-            include_in_schema : whether to include the object in the schema
-            **kwargs : additional keyword arguments
-
-        Returns:
-            A callable handler function
-
-        Raises:
-            NotImplementedError: If the function is not implemented
+    async def start(self) -> None:
+        """Start the broker async use case."""
+        self._abc_start()
+        await self.connect()
+        self.setup()
+
+    def setup(self) -> None:
+        """Prepare all Broker entities to startup."""
+        for h in self._subscribers.values():
+            self.setup_subscriber(h)
 
-        """
-        raise NotImplementedError()
+        for p in self._publishers.values():
+            self.setup_publisher(p)
 
-    def _wrap_subscriber(
+    def setup_subscriber(
         self,
-        *args: Any,
-        dependencies: Sequence[Depends] = (),
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [StreamMessage[MsgType]],
-                    AsyncContextManager[None],
-                ]
-            ]
-        ] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        include_in_schema: bool = True,
+        subscriber: SubscriberProto[MsgType],
         **kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-    ]:
-        """This is a function named `_wrap_subscriber` that returns a callable object. It is used as a decorator for another function.
-
-        Args:
-            *args: Variable length arguments
-            dependencies: Sequence of dependencies
-            middlewares: Optional sequence of middlewares
-            parser: Optional custom parser
-            decoder: Optional custom decoder
-            include_in_schema: Whether to include the object in the schema
-            **kwargs: Variable length keyword arguments
-
-        Returns:
-            A callable object that wraps the decorated function
-
-        This function is decorated with `@abstractmethod`, indicating that it is an abstract method and must be implemented by any subclass.
-
-        """
-
-        def router_subscriber_wrapper(
-            func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
-            """Wraps a function with a router subscriber.
-
-            Args:
-                func: The function to be wrapped.
-
-            Returns:
-                The wrapped function.
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            wrapped_func: HandlerCallWrapper[
-                MsgType, P_HandlerParams, T_HandlerReturn
-            ] = HandlerCallWrapper(func)
-            route: BrokerRoute[MsgType, T_HandlerReturn] = BrokerRoute(
-                wrapped_func,
-                *args,
-                dependencies=(*self._dependencies, *dependencies),
-                middlewares=(*(self._middlewares or ()), *(middlewares or ())),
-                parser=parser or self._parser,
-                decoder=decoder or self._decoder,
-                include_in_schema=(
-                    include_in_schema
-                    if self.include_in_schema is None
-                    else self.include_in_schema
-                ),
-                **kwargs,
-            )
-            self._handlers.append(route)
-            return wrapped_func
-
-        return router_subscriber_wrapper
+    ) -> None:
+        """Setup the Subscriber to prepare it to starting."""
+        subscriber.setup(
+            logger=self.logger,
+            producer=self._producer,
+            graceful_timeout=self.graceful_timeout,
+            extra_context={},
+            # broker options
+            broker_parser=self._parser,
+            broker_decoder=self._decoder,
+            # dependant args
+            apply_types=self._is_apply_types,
+            is_validate=self._is_validate,
+            _get_dependant=self._get_dependant,
+            **self._subscriber_setup_extra,
+            **kwargs,
+        )
 
-    @abstractmethod
-    def publisher(
+    def setup_publisher(
         self,
-        subj: str,
-        *args: Any,
+        publisher: PublisherProto[MsgType],
         **kwargs: Any,
-    ) -> BasePublisher[MsgType]:
-        """Publishes a message.
-
-        Args:
-            subj: Subject of the message
-            *args: Additional arguments
-            **kwargs: Additional keyword arguments
-
-        Returns:
-            The published message
-
-        Raises:
-            NotImplementedError: If the method is not implemented
+    ) -> None:
+        """Setup the Publisher to prepare it to starting."""
+        publisher.setup(
+            producer=self._producer,
+            **self._publisher_setup_extra,
+            **kwargs,
+        )
+
+    @property
+    def _subscriber_setup_extra(self) -> "AnyDict":
+        return {}
+
+    @property
+    def _publisher_setup_extra(self) -> "AnyDict":
+        return {}
+
+    def publisher(self, *args: Any, **kwargs: Any) -> PublisherProto[MsgType]:
+        pub = super().publisher(*args, **kwargs)
+        if self.running:
+            self.setup_publisher(pub)
+        return pub
+
+    def _abc_start(self) -> None:
+        for h in self._subscribers.values():
+            log_context = h.get_log_context(None)
+            log_context.pop("message_id", None)
+            self._setup_log_context(**log_context)
+
+        if not self.running:
+            self.running = True
+
+            if not self.use_custom and self.logger is not None:
+                set_logger_fmt(
+                    cast(logging.Logger, self.logger),
+                    self._get_fmt(),
+                )
+
+    async def connect(self, **kwargs: Any) -> ConnectionType:
+        """Connect to a remote server."""
+        if self._connection is None:
+            connection_kwargs = self._connection_kwargs.copy()
+            connection_kwargs.update(kwargs)
+            self._connection = await self._connect(**connection_kwargs)
+        return self._connection
 
-        """
+    @abstractmethod
+    async def _connect(self) -> ConnectionType:
+        """Connect to a resource."""
         raise NotImplementedError()
 
-    def include_router(self, router: "BrokerRouter[PublisherKeyType, MsgType]") -> None:
-        """Includes a router in the current object.
-
-        Args:
-            router: The router to be included.
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exc_tb: Optional["TracebackType"] = None,
+    ) -> None:
+        """Closes the object."""
+        self.running = False
 
-        Returns:
-            None
+        for h in self._subscribers.values():
+            await h.close()
 
-        """
-        for h in router._handlers:
-            self.subscriber(*h.args, **h.kwargs)(h.call)
-
-        for p in router._publishers.values():
-            p = self._update_publisher_prefix(self.prefix, p)
-            key = self._get_publisher_key(p)
-            self._publishers[key] = self._publishers.get(key, p)
+        if self._connection is not None:
+            await self._close(exc_type, exc_val, exc_tb)
 
-    def include_routers(
-        self, *routers: "BrokerRouter[PublisherKeyType, MsgType]"
+    @abstractmethod
+    async def _close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
-        """Includes routers in the object.
+        """Close the object."""
+        self._connection = None
 
-        Args:
-            *routers: Variable length argument list of routers to include.
+    async def publish(
+        self,
+        msg: Any,
+        *,
+        producer: Optional[ProducerProto],
+        **kwargs: Any,
+    ) -> Optional[Any]:
+        """Publish message directly."""
+        assert producer, NOT_CONNECTED_YET  # nosec B101
+
+        async with AsyncExitStack() as stack:
+            for m in self._middlewares:
+                msg = await stack.enter_async_context(
+                    m(None).publish_scope(msg, **kwargs)
+                )
 
-        Returns:
-            None
+            return await producer.publish(msg, **kwargs)
 
-        """
-        for r in routers:
-            self.include_router(r)
+        return None
```

### Comparing `faststream-0.4.7/faststream/broker/utils.py` & `faststream-0.5.0rc0/faststream/log/formatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,74 @@
 import logging
-from functools import wraps
-from typing import Awaitable, Callable, Optional, Union
+import sys
+from typing import Literal, Optional
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.push_back_watcher import (
-    BaseWatcher,
-    CounterWatcher,
-    EndlessWatcher,
-    OneTryWatcher,
-)
-from faststream.broker.types import MsgType, T_HandlerReturn, WrappedReturn
-from faststream.utils import context
+COLORED_LEVELS = {
+    logging.DEBUG: "\033[36mDEBUG\033[0m",
+    logging.INFO: "\033[32mINFO\033[0m",
+    logging.WARNING: "\033[33mWARNING\033[0m",
+    logging.ERROR: "\033[31mERROR\033[0m",
+    logging.CRITICAL: "\033[91mCRITICAL\033[0m",
+}
+
+
+class ColourizedFormatter(logging.Formatter):
+    """A class to format log messages with colorized level names.
+
+    Methods:
+        __init__ : Initialize the formatter with specified format strings.
+        formatMessage : Format the log record message with colorized level name.
+    """
 
+    def __init__(
+        self,
+        fmt: Optional[str] = None,
+        datefmt: Optional[str] = None,
+        style: Literal["%", "{", "$"] = "%",
+        use_colors: Optional[bool] = None,
+    ) -> None:
+        """Initialize the formatter with specified format strings.
+
+        Initialize the formatter either with the specified format string, or a
+        default as described above. Allow for specialized date formatting with
+        the optional datefmt argument. If datefmt is omitted, you get an
+        ISO8601-like (or RFC 3339-like) format.
+
+        Use a style parameter of '%', '{' or '$' to specify that you want to
+        use one of %-formatting, :meth:`str.format` (``{}``) formatting or
+        :class:`string.Template` formatting in your format string.
+        """
+        if use_colors in (True, False):
+            self.use_colors = use_colors
+        else:
+            self.use_colors = sys.stdout.isatty()
+        super().__init__(fmt=fmt, datefmt=datefmt, style=style)
 
-def change_logger_handlers(logger: logging.Logger, fmt: str) -> None:
-    """Change the formatter of the logger handlers.
+    def formatMessage(self, record: logging.LogRecord) -> str:  # noqa: N802
+        """Formats the log message.
 
-    Args:
-        logger (logging.Logger): The logger object.
-        fmt (str): The format string for the formatter.
+        Args:
+            record (logging.LogRecord): The log record to format.
 
-    Returns:
-        None
+        Returns:
+            str: The formatted log message.
+        """
+        if self.use_colors:
+            record.levelname = expand_log_field(
+                field=COLORED_LEVELS.get(record.levelno, record.levelname),
+                symbols=17,
+            )
 
-    """
-    for handler in getattr(logger, "handlers", ()):
-        formatter = handler.formatter
-        if formatter is not None:  # pragma: no branch
-            use_colors = getattr(formatter, "use_colors", None)
-            kwargs = (
-                {"use_colors": use_colors} if use_colors is not None else {}
-            )  # pragma: no branch
-
-            handler.setFormatter(type(formatter)(fmt, **kwargs))
-
-
-def get_watcher(
-    logger: Optional[logging.Logger],
-    try_number: Union[bool, int] = True,
-) -> BaseWatcher:
-    """Get a watcher object based on the provided parameters.
+        return super().formatMessage(record)
 
-    Args:
-        logger: Optional logger object for logging messages.
-        try_number: Optional parameter to specify the type of watcher.
-            - If set to True, an EndlessWatcher object will be returned.
-            - If set to False, a OneTryWatcher object will be returned.
-            - If set to an integer, a CounterWatcher object with the specified maximum number of tries will be returned.
 
-    Returns:
-        A watcher object based on the provided parameters.
-
-    """
-    watcher: Optional[BaseWatcher]
-    if try_number is True:
-        watcher = EndlessWatcher()
-    elif try_number is False:
-        watcher = OneTryWatcher()
-    else:
-        watcher = CounterWatcher(logger=logger, max_tries=try_number)
-    return watcher
-
-
-def set_message_context(
-    func: Callable[
-        [StreamMessage[MsgType]],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ],
-) -> Callable[[StreamMessage[MsgType]], Awaitable[WrappedReturn[T_HandlerReturn]]]:
-    """Sets the message context for a function.
+def expand_log_field(field: str, symbols: int) -> str:
+    """Expands a log field by adding spaces.
 
     Args:
-        func: The function to set the message context for.
+        field: The log field to expand.
+        symbols: The desired length of the expanded field.
 
     Returns:
-        The function with the message context set.
-
+        The expanded log field.
     """
-
-    @wraps(func)
-    async def set_message_wrapper(
-        message: StreamMessage[MsgType],
-    ) -> WrappedReturn[T_HandlerReturn]:
-        """Wraps a function that handles a stream message.
-
-        Args:
-            message: The stream message to be handled.
-
-        Returns:
-            The wrapped return value of the handler function.
-
-        """
-        with context.scope("message", message):
-            return await func(message)
-
-    return set_message_wrapper
+    return field + (" " * (symbols - len(field)))
```

### Comparing `faststream-0.4.7/faststream/broker/core/abc.py` & `faststream-0.5.0rc0/faststream/broker/fastapi/router.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,622 +1,495 @@
-import logging
-import warnings
-from abc import ABC, abstractmethod
-from functools import partial
-from itertools import chain
+import json
+from abc import abstractmethod
+from contextlib import asynccontextmanager
+from enum import Enum
 from types import TracebackType
 from typing import (
     Any,
-    AsyncContextManager,
+    AsyncIterator,
     Awaitable,
     Callable,
+    Dict,
     Generic,
+    Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
-    Sized,
-    Tuple,
     Type,
     Union,
     cast,
+    overload,
 )
+from weakref import WeakSet
 
-from fast_depends._compat import PYDANTIC_V2
-from fast_depends.core import CallModel, build_call_model
-from fast_depends.dependencies import Depends
-from pydantic import Field, create_model
+from fastapi import APIRouter, FastAPI, params
+from fastapi.background import BackgroundTasks
+from fastapi.datastructures import Default
+from fastapi.responses import HTMLResponse
+from fastapi.routing import APIRoute
+from fastapi.types import IncEx
+from fastapi.utils import generate_unique_id
+from starlette import routing
+from starlette.responses import JSONResponse, Response
+from starlette.routing import BaseRoute, _DefaultLifespan
+from starlette.types import ASGIApp, AppType, Lifespan
 
-from faststream._compat import PydanticUndefined, is_test_env
 from faststream.asyncapi import schema as asyncapi
-from faststream.broker.core.mixins import LoggingMixin
-from faststream.broker.handler import BaseHandler
-from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware, CriticalLogMiddleware
-from faststream.broker.publisher import BasePublisher
-from faststream.broker.push_back_watcher import WatcherContext
-from faststream.broker.router import BrokerRouter
+from faststream.asyncapi.schema import Schema
+from faststream.asyncapi.site import get_asyncapi_html
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.broker.fastapi.get_dependant import get_fastapi_dependant
+from faststream.broker.fastapi.route import StreamRoute
+from faststream.broker.middlewares import BaseMiddleware
+from faststream.broker.publisher.proto import PublisherProto
+from faststream.broker.schemas import NameRequired
 from faststream.broker.types import (
-    ConnectionType,
-    CustomDecoder,
-    CustomParser,
-    Filter,
+    BrokerMiddleware,
     MsgType,
     P_HandlerParams,
     T_HandlerReturn,
-    WrappedReturn,
-)
-from faststream.broker.utils import (
-    change_logger_handlers,
-    get_watcher,
-    set_message_context,
-)
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.log import access_logger
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict, F_Return, F_Spec
-from faststream.utils import apply_types, context
-from faststream.utils.functions import (
-    fake_context,
-    get_function_positional_arguments,
-    to_async,
 )
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.broker.wrapper.proto import WrapperProto
+from faststream.types import AnyDict
+from faststream.utils.context.repository import context
+from faststream.utils.functions import to_async
 
 
-class BrokerUsecase(
-    ABC,
-    Generic[MsgType, ConnectionType],
-    LoggingMixin,
-):
-    """A class representing a broker use case.
-
-    Attributes:
-        logger : optional logger object
-        log_level : log level
-        handlers : dictionary of handlers
-        _publishers : dictionary of publishers
-        dependencies : sequence of dependencies
-        started : boolean indicating if the broker has started
-        middlewares : sequence of middleware functions
-        _global_parser : optional custom parser object
-        _global_decoder : optional custom decoder object
-        _connection : optional connection object
-        _fmt : optional string format
-
-    Methods:
-        __init__ : constructor method
-        include_router : include a router in the broker
-        include_routers : include multiple routers in the broker
-        _resolve_connection_kwargs : resolve connection kwargs
-        _wrap_handler : wrap a handler function
-        _abc_start : start the broker
-        _abc_close : close the broker
-        _abc__close : close the broker connection
-        _process_message : process a message
-        subscriber : decorator to register a subscriber
-        publisher : register a publisher
-        _wrap_decode_message : wrap a message decoding function
-
-    """
-
-    logger: Optional[logging.Logger]
-    log_level: int
-    handlers: Mapping[Any, BaseHandler[MsgType]]
-    _publishers: Mapping[Any, BasePublisher[MsgType]]
-
-    dependencies: Sequence[Depends]
-    started: bool
-    middlewares: Sequence[Callable[[Any], BaseMiddleware]]
-    _global_parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]]
-    _global_decoder: Optional[CustomDecoder[StreamMessage[MsgType]]]
-    _connection: Optional[ConnectionType]
-    _fmt: Optional[str]
-
-    def __init__(
+class _BackgroundMiddleware(BaseMiddleware):
+    async def after_processed(
         self,
-        url: Union[str, List[str]],
-        *args: Any,
-        # AsyncAPI kwargs
-        protocol: Optional[str] = None,
-        protocol_version: Optional[str] = None,
-        description: Optional[str] = None,
-        tags: Optional[Sequence[Union[asyncapi.Tag, asyncapi.TagDict]]] = None,
-        asyncapi_url: Union[str, List[str], None] = None,
-        # broker kwargs
-        apply_types: bool = True,
-        validate: bool = True,
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
-        dependencies: Sequence[Depends] = (),
-        middlewares: Optional[Sequence[Callable[[MsgType], BaseMiddleware]]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        security: Optional[BaseSecurity] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize a broker.
-
-        Args:
-            url: The URL or list of URLs to connect to.
-            *args: Additional arguments.
-            protocol: The protocol to use for the connection.
-            protocol_version: The version of the protocol.
-            description: A description of the broker.
-            tags: Tags associated with the broker.
-            asyncapi_url: The URL or list of URLs to the AsyncAPI schema.
-            apply_types: Whether to apply types to messages.
-            validate: Whether to cast types using Pydantic validation.
-            logger: The logger to use.
-            log_level: The log level to use.
-            log_fmt: The log format to use.
-            dependencies: Dependencies of the broker.
-            middlewares: Middlewares to use.
-            decoder: Custom decoder for messages.
-            parser: Custom parser for messages.
-            security: Security scheme to use.
-            **kwargs: Additional keyword arguments.
-
-        """
-        super().__init__(
-            logger=logger,
-            log_level=log_level,
-            log_fmt=log_fmt,
-        )
-
-        self._connection = None
-        self._is_apply_types = apply_types
-        self._is_validate = validate
-        self.handlers = {}
-        self._publishers = {}
-        empty_middleware: Sequence[Callable[[MsgType], BaseMiddleware]] = ()
-        midd_args: Sequence[Callable[[MsgType], BaseMiddleware]] = (
-            middlewares or empty_middleware
-        )
-        self.middlewares = [CriticalLogMiddleware(logger, log_level), *midd_args]
-        self.dependencies = dependencies
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exc_tb: Optional[TracebackType] = None,
+    ) -> Optional[bool]:
+        if not exc_type and (
+            background := cast(
+                Optional[BackgroundTasks],
+                getattr(context.get_local("message"), "background", None),
+            )
+        ):
+            await background()
 
-        self._connection_args = (url, *args)
-        self._connection_kwargs = kwargs
+        return await super().after_processed(exc_type, exc_val, exc_tb)
 
-        self._global_parser = parser
-        self._global_decoder = decoder
 
-        context.set_global("logger", logger)
-        context.set_global("broker", self)
+class StreamRouter(APIRouter, Generic[MsgType]):
+    """A class to route streams."""
 
-        self.started = False
+    broker_class: Type[BrokerUsecase[MsgType, Any]]
+    broker: BrokerUsecase[MsgType, Any]
+    docs_router: Optional[APIRouter]
+    _after_startup_hooks: List[Callable[[Any], Awaitable[Optional[Mapping[str, Any]]]]]
+    _on_shutdown_hooks: List[Callable[[Any], Awaitable[None]]]
+    schema: Optional[Schema]
+
+    title: str
+    description: str
+    version: str
+    license: Optional[AnyDict]
+    contact: Optional[AnyDict]
 
+    def __init__(
+        self,
+        *connection_args: Any,
+        middlewares: Iterable[BrokerMiddleware[MsgType]] = (),
+        prefix: str = "",
+        tags: Optional[List[Union[str, Enum]]] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
+        default_response_class: Type[Response] = Default(JSONResponse),
+        responses: Optional[Dict[Union[int, str], AnyDict]] = None,
+        callbacks: Optional[List[routing.BaseRoute]] = None,
+        routes: Optional[List[routing.BaseRoute]] = None,
+        redirect_slashes: bool = True,
+        default: Optional[ASGIApp] = None,
+        dependency_overrides_provider: Optional[Any] = None,
+        route_class: Type[APIRoute] = APIRoute,
+        on_startup: Optional[Sequence[Callable[[], Any]]] = None,
+        on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
+        deprecated: Optional[bool] = None,
+        include_in_schema: bool = True,
+        setup_state: bool = True,
+        lifespan: Optional[Lifespan[Any]] = None,
+        generate_unique_id_function: Callable[[APIRoute], str] = Default(
+            generate_unique_id
+        ),
         # AsyncAPI information
-        self.url = asyncapi_url or url
-        self.protocol = protocol
-        self.protocol_version = protocol_version
-        self.description = description
-        self.tags = tags
-        self.security = security
-
-    def include_router(self, router: BrokerRouter[Any, MsgType]) -> None:
-        """Includes a router in the current object.
-
-        Args:
-            router: The router to be included.
-
-        Returns:
-            None
-
-        """
-        for r in router._handlers:
-            self.subscriber(*r.args, **r.kwargs)(r.call)
-
-        self._publishers = {**self._publishers, **router._publishers}
-
-    def include_routers(self, *routers: BrokerRouter[Any, MsgType]) -> None:
-        """Includes routers in the current object.
+        asyncapi_tags: Optional[Iterable[Union[asyncapi.Tag, asyncapi.TagDict]]] = None,
+        schema_url: Optional[str] = "/asyncapi",
+        **connection_kwars: Any,
+    ) -> None:
+        assert (  # nosec B101
+            self.broker_class
+        ), "You should specify `broker_class` at your implementation"
+
+        self.broker = self.broker_class(
+            *connection_args,
+            middlewares=(
+                *middlewares,
+                # allow to catch background exceptions in user middlewares
+                _BackgroundMiddleware,
+            ),
+            _get_dependant=get_fastapi_dependant,
+            tags=asyncapi_tags,
+            **connection_kwars,
+        )
 
-        Args:
-            *routers: Variable length argument list of routers to include.
+        self.setup_state = setup_state
 
-        Returns:
-            None
+        # AsyncAPI information
+        # Empty
+        self.terms_of_service = None
+        self.identifier = None
+        self.asyncapi_tags = None
+        self.external_docs = None
+        # parse from FastAPI app on startup
+        self.title = ""
+        self.version = ""
+        self.description = ""
+        self.license = None
+        self.contact = None
 
-        """
-        for r in routers:
-            self.include_router(r)
+        self.schema = None
 
-    def _resolve_connection_kwargs(self, *args: Any, **kwargs: Any) -> AnyDict:
-        """Resolve connection keyword arguments.
+        super().__init__(
+            prefix=prefix,
+            tags=tags,
+            dependencies=dependencies,
+            default_response_class=default_response_class,
+            responses=responses,
+            callbacks=callbacks,
+            routes=routes,
+            redirect_slashes=redirect_slashes,
+            default=default,
+            dependency_overrides_provider=dependency_overrides_provider,
+            route_class=route_class,
+            deprecated=deprecated,
+            include_in_schema=include_in_schema,
+            generate_unique_id_function=generate_unique_id_function,
+            lifespan=self._wrap_lifespan(lifespan),
+            on_startup=on_startup,
+            on_shutdown=on_shutdown,
+        )
 
-        Args:
-            *args: Positional arguments passed to the function.
-            **kwargs: Keyword arguments passed to the function.
+        self.weak_dependencies_provider: "WeakSet[Any]" = WeakSet()
+        if dependency_overrides_provider is not None:
+            self.weak_dependencies_provider.add(dependency_overrides_provider)
 
-        Returns:
-            A dictionary containing the resolved connection keyword arguments.
+        if self.include_in_schema:
+            self.docs_router = self._asyncapi_router(schema_url)
+        else:
+            self.docs_router = None
 
-        """
-        arguments = get_function_positional_arguments(self.__init__)  # type: ignore
-        init_kwargs = {
-            **self._connection_kwargs,
-            **dict(zip(arguments, self._connection_args)),
-        }
+        self._after_startup_hooks = []
+        self._on_shutdown_hooks = []
 
-        connect_kwargs = {
-            **kwargs,
-            **dict(zip(arguments, args)),
-        }
-        return {**init_kwargs, **connect_kwargs}
+    def _get_dependencies_overides_provider(self) -> Optional[Any]:
+        """Dependency provider WeakRef resolver."""
+        if self.dependency_overrides_provider is not None:
+            return self.dependency_overrides_provider
+        else:
+            return next(iter(self.weak_dependencies_provider), None)
 
-    def _wrap_handler(
+    def _add_api_mq_route(
         self,
-        func: Union[
-            HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-            Callable[P_HandlerParams, T_HandlerReturn],
-        ],
-        *,
-        retry: Union[bool, int] = False,
-        extra_dependencies: Sequence[Depends] = (),
-        no_ack: bool = False,
-        _raw: bool = False,
-        _get_dependant: Optional[Any] = None,
-        _process_kwargs: Optional[AnyDict] = None,
-    ) -> Tuple[
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-        CallModel[Any, Any],
-    ]:
-        """Wrap a handler function.
-
-        Args:
-            func: The handler function to wrap.
-            retry: Whether to retry the handler function if it fails. Can be a boolean or an integer specifying the number of retries.
-            extra_dependencies: Additional dependencies for the handler function.
-            no_ack: Whether not to ack/nack/reject messages.
-            _raw: Whether to use the raw handler function.
-            _get_dependant: The dependant function to use.
-            **broker_log_context_kwargs: Additional keyword arguments for the broker log context.
-
-        Returns:
-            A tuple containing the wrapped handler function and the call model.
-
-        Raises:
-            NotImplementedError: If silent animals are not supported.
-
-        """
-        build_dep = cast(
-            Callable[[Callable[F_Spec, F_Return]], CallModel[F_Spec, F_Return]],
-            _get_dependant or partial(build_call_model, cast=self._is_validate),
+        path: Union[NameRequired, str],
+        *extra: Union[NameRequired, str],
+        endpoint: Callable[P_HandlerParams, T_HandlerReturn],
+        dependencies: Iterable[params.Depends],
+        response_model: Any,
+        response_model_include: Optional[IncEx],
+        response_model_exclude: Optional[IncEx],
+        response_model_by_alias: bool,
+        response_model_exclude_unset: bool,
+        response_model_exclude_defaults: bool,
+        response_model_exclude_none: bool,
+        **broker_kwargs: Any,
+    ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
+        """Add an API message queue route."""
+        route = StreamRoute[MsgType, P_HandlerParams, T_HandlerReturn](
+            path,
+            *extra,
+            endpoint=endpoint,
+            dependencies=(*self.dependencies, *dependencies),
+            provider_factory=self._get_dependencies_overides_provider,
+            broker=self.broker,
+            response_model=response_model,
+            response_model_include=response_model_include,
+            response_model_exclude=response_model_exclude,
+            response_model_by_alias=response_model_by_alias,
+            response_model_exclude_unset=response_model_exclude_unset,
+            response_model_exclude_defaults=response_model_exclude_defaults,
+            response_model_exclude_none=response_model_exclude_none,
+            **broker_kwargs,
         )
+        self.routes.append(route)
+        return route.handler
 
-        if isinstance(func, HandlerCallWrapper):
-            handler_call, func = func, func._original_call
-            if handler_call._wrapped_call is not None:
-                return handler_call, build_dep(func)
-        else:
-            handler_call = HandlerCallWrapper(func)
-
-        f = to_async(func)
-
-        dependant = build_dep(f)
-
-        extra = [
-            build_dep(d.dependency)
-            for d in chain(extra_dependencies, self.dependencies)
-        ]
-
-        extend_dependencies(extra, dependant)
-
-        if getattr(dependant, "flat_params", None) is None:  # handle FastAPI Dependant
-            dependant = _patch_fastapi_dependant(dependant)
-
-        if self._is_apply_types and not _raw:
-            f = apply_types(None, cast=self._is_validate)(f, dependant)  # type: ignore[arg-type,assignment]
-
-        decode_f = self._wrap_decode_message(
-            func=f,
-            _raw=_raw,
-            params=set(
-                chain(
-                    dependant.flat_params.keys(), *(d.flat_params.keys() for d in extra)
-                )
-            ),
-        )
+    def subscriber(
+        self,
+        path: Union[str, NameRequired],
+        *extra: Union[NameRequired, str],
+        dependencies: Iterable[params.Depends],
+        response_model: Any,
+        response_model_include: Optional[IncEx],
+        response_model_exclude: Optional[IncEx],
+        response_model_by_alias: bool,
+        response_model_exclude_unset: bool,
+        response_model_exclude_defaults: bool,
+        response_model_exclude_none: bool,
+        **broker_kwargs: Any,
+    ) -> WrapperProto[MsgType]:
+        """A function decorator for subscribing to a message queue."""
 
-        process_f = self._process_message(
-            func=decode_f,
-            watcher=(
-                partial(WatcherContext, watcher=get_watcher(self.logger, retry))  # type: ignore[arg-type]
-                if not no_ack
-                else fake_context
-            ),
-            **(_process_kwargs or {}),
-        )
+        def decorator(
+            func: Callable[P_HandlerParams, T_HandlerReturn],
+        ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
+            """A decorator function."""
+            return self._add_api_mq_route(
+                path,
+                *extra,
+                endpoint=func,
+                dependencies=dependencies,
+                response_model=response_model,
+                response_model_include=response_model_include,
+                response_model_exclude=response_model_exclude,
+                response_model_by_alias=response_model_by_alias,
+                response_model_exclude_unset=response_model_exclude_unset,
+                response_model_exclude_defaults=response_model_exclude_defaults,
+                response_model_exclude_none=response_model_exclude_none,
+                **broker_kwargs,
+            )
 
-        process_f = set_message_context(process_f)
+        return decorator
 
-        handler_call.set_wrapped(process_f)
-        return handler_call, dependant
+    def _wrap_lifespan(self, lifespan: Optional[Lifespan[Any]] = None) -> Lifespan[Any]:
+        lifespan_context = lifespan if lifespan is not None else _DefaultLifespan(self)
 
-    def _abc_start(self) -> None:
-        if not self.started:
-            self.started = True
+        @asynccontextmanager
+        async def start_broker_lifespan(
+            app: FastAPI,
+        ) -> AsyncIterator[Mapping[str, Any]]:
+            """Starts the lifespan of a broker."""
+            if not len(self.weak_dependencies_provider):
+                self.weak_dependencies_provider.add(app)
+
+            if self.docs_router:
+                self.title = app.title
+                self.description = app.description
+                self.version = app.version
+                self.contact = app.contact
+                self.license = app.license_info
+
+                from faststream.asyncapi.generate import get_app_schema
+                self.schema = get_app_schema(self)
+
+                app.include_router(self.docs_router)
+
+            if not len(self.weak_dependencies_provider):
+                self.weak_dependencies_provider.add(app)
+
+            async with lifespan_context(app) as maybe_context:
+                if maybe_context is None:
+                    context: AnyDict = {}
+                else:
+                    context = dict(maybe_context)
+
+                context.update({"broker": self.broker})
+                await self.broker.start()
+
+                for h in self._after_startup_hooks:
+                    h_context = await h(app)
+                    if h_context:  # pragma: no branch
+                        context.update(h_context)
+
+                try:
+                    if self.setup_state:
+                        yield context
+                    else:
+                        # NOTE: old asgi compatibility
+                        yield  # type: ignore
+
+                    for h in self._on_shutdown_hooks:
+                        await h(app)
 
-            for h in self.handlers.values():
-                h.global_middlewares = (*self.middlewares, *h.global_middlewares)
+                finally:
+                    await self.broker.close()
 
-            if self.logger is not None:
-                change_logger_handlers(self.logger, self.fmt)
+        return start_broker_lifespan
 
-    def _abc_close(
+    @overload
+    def after_startup(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> None:
-        """Closes the ABC.
+        func: Callable[[AppType], Mapping[str, Any]],
+    ) -> Callable[[AppType], Mapping[str, Any]]: ...
 
-        Args:
-            exc_type: The exception type
-            exc_val: The exception value
-            exec_tb: The traceback
-
-        Returns:
-            None
-
-        """
-        self.started = False
-
-    def _abc__close(
+    @overload
+    def after_startup(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> None:
-        """Closes the connection.
+        func: Callable[[AppType], Awaitable[Mapping[str, Any]]],
+    ) -> Callable[[AppType], Awaitable[Mapping[str, Any]]]: ...
 
-        Args:
-            exc_type: The type of the exception being handled (optional)
-            exc_val: The exception instance being handled (optional)
-            exec_tb: The traceback for the exception being handled (optional)
-
-        Returns:
-            None
-
-        Note:
-            This is an abstract method and must be implemented by subclasses.
-
-        """
-        self._connection = None
-
-    @abstractmethod
-    def _process_message(
+    @overload
+    def after_startup(
         self,
-        func: Callable[[StreamMessage[MsgType]], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[[StreamMessage[MsgType]], Awaitable[WrappedReturn[T_HandlerReturn]]]:
-        """Processes a message using a given function and watcher.
-
-        Args:
-            func: A callable that takes a StreamMessage of type MsgType and returns an Awaitable of type T_HandlerReturn.
-            watcher: An instance of BaseWatcher.
-            disable_watcher: Whether to use watcher context.
-            kwargs: Additional keyword arguments.
-
-        Returns:
-            A callable that takes a StreamMessage of type MsgType and returns an Awaitable of type WrappedReturn[T_HandlerReturn].
+        func: Callable[[AppType], None],
+    ) -> Callable[[AppType], None]: ...
 
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        raise NotImplementedError()
+    @overload
+    def after_startup(
+        self,
+        func: Callable[[AppType], Awaitable[None]],
+    ) -> Callable[[AppType], Awaitable[None]]: ...
 
-    @abstractmethod
-    def subscriber(  # type: ignore[return]
+    def after_startup(
         self,
-        *broker_args: Any,
-        retry: Union[bool, int] = False,
-        dependencies: Sequence[Depends] = (),
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [StreamMessage[MsgType]],
-                    BaseMiddleware,
-                ]
-            ]
-        ] = None,
-        filter: Filter[StreamMessage[MsgType]] = lambda m: not m.processed,
-        _raw: bool = False,
-        _get_dependant: Optional[Any] = None,
-        **broker_kwargs: Any,
-    ) -> Callable[
-        [
-            Union[
-                Callable[P_HandlerParams, T_HandlerReturn],
-                HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-            ]
+        func: Union[
+            Callable[[AppType], Mapping[str, Any]],
+            Callable[[AppType], Awaitable[Mapping[str, Any]]],
+            Callable[[AppType], None],
+            Callable[[AppType], Awaitable[None]],
         ],
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
+    ) -> Union[
+        Callable[[AppType], Mapping[str, Any]],
+        Callable[[AppType], Awaitable[Mapping[str, Any]]],
+        Callable[[AppType], None],
+        Callable[[AppType], Awaitable[None]],
     ]:
-        """This is a function decorator for subscribing to a message broker.
+        """Register a function to be executed after startup."""
+        self._after_startup_hooks.append(to_async(func))  # type: ignore
+        return func
 
-        Args:
-            *broker_args: Positional arguments to be passed to the broker.
-            retry: Whether to retry the subscription if it fails. Can be a boolean or an integer specifying the number of retries.
-            dependencies: Sequence of dependencies to be injected into the handler function.
-            decoder: Custom decoder function to decode the message.
-            parser: Custom parser function to parse the decoded message.
-            middlewares: Sequence of middleware functions to be applied to the message.
-            filter: Filter function to filter the messages to be processed.
-            _raw: Whether to return the raw message instead of the processed message.
-            _get_dependant: Optional parameter to get the dependant object.
-            **broker_kwargs: Keyword arguments to be passed to the broker.
-
-        Returns:
-            A callable object that can be used as a decorator for a handler function.
-
-        Raises:
-            RuntimeWarning: If the broker is already running.
-
-        """
-        if self.started and not is_test_env():  # pragma: no cover
-            warnings.warn(
-                "You are trying to register `handler` with already running broker\n"
-                "It has no effect until broker restarting.",
-                category=RuntimeWarning,
-                stacklevel=1,
-            )
-
-    @abstractmethod
-    def publisher(
+    @overload
+    def on_broker_shutdown(
         self,
-        key: Any,
-        publisher: BasePublisher[MsgType],
-    ) -> BasePublisher[MsgType]:
-        """Publishes a publisher.
-
-        Args:
-            key: The key associated with the publisher.
-            publisher: The publisher to be published.
-
-        Returns:
-            The published publisher.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        self._publishers = {**self._publishers, key: publisher}
-        return publisher
+        func: Callable[[AppType], None],
+    ) -> Callable[[AppType], None]: ...
 
-    @abstractmethod
-    def _wrap_decode_message(
+    @overload
+    def on_broker_shutdown(
         self,
-        func: Callable[..., Awaitable[T_HandlerReturn]],
-        params: Sized = (),
-        _raw: bool = False,
-    ) -> Callable[[StreamMessage[MsgType]], Awaitable[T_HandlerReturn]]:
-        """Wrap a decoding message function.
-
-        Args:
-            func: The function to wrap.
-            params: The parameters to pass to the function.
-            _raw: Whether to return the raw message or not.
-
-        Returns:
-            The wrapped function.
+        func: Callable[[AppType], Awaitable[None]],
+    ) -> Callable[[AppType], Awaitable[None]]: ...
 
-        Raises:
-            NotImplementedError: If the method is not implemented.
+    def on_broker_shutdown(
+        self,
+        func: Union[
+            Callable[[AppType], None],
+            Callable[[AppType], Awaitable[None]],
+        ],
+    ) -> Union[
+        Callable[[AppType], None],
+        Callable[[AppType], Awaitable[None]],
+    ]:
+        """Register a function to be executed before broker stop."""
+        self._on_shutdown_hooks.append(to_async(func))  # type: ignore
+        return func
 
-        """
+    @abstractmethod
+    def publisher(self) -> PublisherProto[MsgType]:
+        """Create Publisher object."""
         raise NotImplementedError()
 
+    def _asyncapi_router(self, schema_url: Optional[str]) -> Optional[APIRouter]:
+        """Creates an API router for serving AsyncAPI documentation."""
+        if not self.include_in_schema or not schema_url:
+            return None
+
+        def download_app_json_schema() -> Response:
+            assert (  # nosec B101
+                self.schema
+            ), "You need to run application lifespan at first"
+
+            return Response(
+                content=json.dumps(self.schema.to_jsonable(), indent=2),
+                headers={"Content-Type": "application/octet-stream"},
+            )
 
-def extend_dependencies(
-    extra: Sequence[CallModel[Any, Any]], dependant: CallModel[Any, Any]
-) -> CallModel[Any, Any]:
-    """Extends the dependencies of a function or FastAPI dependency.
-
-    Args:
-        extra: Additional dependencies to be added.
-        dependant: The function or FastAPI dependency whose dependencies will be extended.
-
-    Returns:
-        The updated function or FastAPI dependency.
-
-    """
-    if isinstance(dependant, CallModel):
-        dependant.extra_dependencies = (*dependant.extra_dependencies, *extra)
-    else:  # FastAPI dependencies
-        dependant.dependencies.extend(extra)
-    return dependant
-
-
-def _patch_fastapi_dependant(
-    dependant: CallModel[P_HandlerParams, Awaitable[T_HandlerReturn]],
-) -> CallModel[P_HandlerParams, Awaitable[T_HandlerReturn]]:
-    """Patch FastAPI dependant.
-
-    Args:
-        dependant: The dependant to be patched.
-
-    Returns:
-        The patched dependant.
-
-    """
-    params = dependant.query_params + dependant.body_params  # type: ignore[attr-defined]
-
-    for d in dependant.dependencies:
-        params.extend(d.query_params + d.body_params)  # type: ignore[attr-defined]
-
-    params_unique = {}
-    for p in params:
-        if p.name not in params_unique:
-            info = p.field_info if PYDANTIC_V2 else p
-
-            field_data = {
-                "default": ... if info.default is PydanticUndefined else info.default,
-                "default_factory": info.default_factory,
-                "alias": info.alias,
-            }
-
-            if PYDANTIC_V2:
-                from pydantic.fields import FieldInfo
-
-                info = cast(FieldInfo, info)
-
-                field_data.update(
-                    {
-                        "title": info.title,
-                        "alias_priority": info.alias_priority,
-                        "validation_alias": info.validation_alias,
-                        "serialization_alias": info.serialization_alias,
-                        "description": info.description,
-                        "discriminator": info.discriminator,
-                        "examples": info.examples,
-                        "exclude": info.exclude,
-                        "json_schema_extra": info.json_schema_extra,
-                    }
-                )
-
-                f = next(
-                    filter(
-                        lambda x: isinstance(x, FieldInfo),
-                        p.field_info.metadata or (),
-                    ),
-                    Field(**field_data),  # type: ignore[pydantic-field]
-                )
-
-            else:
-                from pydantic.fields import ModelField  # type: ignore[attr-defined]
-
-                info = cast(ModelField, info)
+        def download_app_yaml_schema() -> Response:
+            assert (  # nosec B101
+                self.schema
+            ), "You need to run application lifespan at first"
+
+            return Response(
+                content=self.schema.to_yaml(),
+                headers={
+                    "Content-Type": "application/octet-stream",
+                },
+            )
 
-                field_data.update(
-                    {
-                        "title": info.field_info.title,
-                        "description": info.field_info.description,
-                        "discriminator": info.field_info.discriminator,
-                        "exclude": info.field_info.exclude,
-                        "gt": info.field_info.gt,
-                        "ge": info.field_info.ge,
-                        "lt": info.field_info.lt,
-                        "le": info.field_info.le,
-                    }
+        def serve_asyncapi_schema(
+            sidebar: bool = True,
+            info: bool = True,
+            servers: bool = True,
+            operations: bool = True,
+            messages: bool = True,
+            schemas: bool = True,
+            errors: bool = True,
+            expandMessageExamples: bool = True,
+        ) -> HTMLResponse:
+            """Serve the AsyncAPI schema as an HTML response."""
+            assert (  # nosec B101
+                self.schema
+            ), "You need to run application lifespan at first"
+
+            return HTMLResponse(
+                content=get_asyncapi_html(
+                    self.schema,
+                    sidebar=sidebar,
+                    info=info,
+                    servers=servers,
+                    operations=operations,
+                    messages=messages,
+                    schemas=schemas,
+                    errors=errors,
+                    expand_message_examples=expandMessageExamples,
+                    title=self.schema.info.title,
                 )
-                f = Field(**field_data)  # type: ignore[pydantic-field]
-
-            params_unique[p.name] = (
-                info.annotation,
-                f,
             )
 
-    dependant.model = create_model(
-        getattr(dependant.call, "__name__", type(dependant.call).__name__)
-    )
-
-    dependant.custom_fields = {}
-    dependant.flat_params = params_unique  # type: ignore[assignment,misc]
+        docs_router = APIRouter(
+            prefix=self.prefix,
+            tags=["asyncapi"],
+            redirect_slashes=self.redirect_slashes,
+            default=self.default,
+            deprecated=self.deprecated,
+        )
+        docs_router.get(schema_url)(serve_asyncapi_schema)
+        docs_router.get(f"{schema_url}.json")(download_app_json_schema)
+        docs_router.get(f"{schema_url}.yaml")(download_app_yaml_schema)
+        return docs_router
 
-    return dependant
+    def include_router(
+        self,
+        router: "APIRouter",
+        *,
+        prefix: str = "",
+        tags: Optional[List[Union[str, Enum]]] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
+        default_response_class: Type[Response] = Default(JSONResponse),
+        responses: Optional[Dict[Union[int, str], AnyDict]] = None,
+        callbacks: Optional[List[BaseRoute]] = None,
+        deprecated: Optional[bool] = None,
+        include_in_schema: bool = True,
+        generate_unique_id_function: Callable[[APIRoute], str] = Default(
+            generate_unique_id
+        ),
+    ) -> None:
+        """Includes a router in the API."""
+        if isinstance(router, StreamRouter):  # pragma: no branch
+            self.broker.include_router(router.broker)
+            router.weak_dependencies_provider = self.weak_dependencies_provider
+
+        super().include_router(
+            router=router,
+            prefix=prefix,
+            tags=tags,
+            dependencies=dependencies,
+            default_response_class=default_response_class,
+            responses=responses,
+            callbacks=callbacks,
+            deprecated=deprecated,
+            include_in_schema=include_in_schema,
+            generate_unique_id_function=generate_unique_id_function,
+        )
```

### Comparing `faststream-0.4.7/faststream/broker/core/asynchronous.py` & `faststream-0.5.0rc0/faststream/confluent/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,450 +1,409 @@
-import logging
-from abc import abstractmethod
-from functools import wraps
-from types import TracebackType
+import asyncio
+from ssl import SSLContext
+from time import time
 from typing import (
     Any,
-    AsyncContextManager,
-    Awaitable,
     Callable,
-    Mapping,
+    Dict,
+    Iterable,
+    List,
+    NamedTuple,
     Optional,
-    Sequence,
-    Sized,
     Tuple,
-    Type,
     Union,
-    cast,
 )
 
-from fast_depends.core import CallModel
-from fast_depends.dependencies import Depends
-from typing_extensions import Self, override
-
-from faststream.broker.core.abc import BrokerUsecase
-from faststream.broker.handler import AsyncHandler
-from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.types import (
-    AsyncCustomDecoder,
-    AsyncCustomParser,
-    ConnectionType,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    MsgType,
-    P_HandlerParams,
-    T_HandlerReturn,
-    WrappedReturn,
-)
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.log import access_logger
-from faststream.types import AnyDict, SendableMessage
-from faststream.utils.functions import to_async
-
-
-async def default_filter(msg: StreamMessage[Any]) -> bool:
-    """A function to filter stream messages.
+from confluent_kafka import Consumer, KafkaError, KafkaException, Message, Producer
+from confluent_kafka.admin import AdminClient, NewTopic
+from pydantic import BaseModel
 
-    Args:
-        msg : A stream message object
+from faststream.log import logger
+from faststream.utils.functions import call_or_await
 
-    Returns:
-        True if the message has not been processed, False otherwise
-
-    """
-    return not msg.processed
+_missing = object()
 
 
-class BrokerAsyncUsecase(BrokerUsecase[MsgType, ConnectionType]):
-    """A class representing a broker async use case.
+class MsgToSend(BaseModel):
+    """A Pydantic model representing a message to be sent to Kafka.
 
     Attributes:
-        handlers : A dictionary of handlers for different message types.
-        middlewares : A sequence of middleware functions.
-        _global_parser : An optional global parser for messages.
-        _global_decoder : An optional global decoder for messages.
-
-    Methods:
-        start() : Abstract method to start the broker async use case.
-        _connect(**kwargs: Any) : Abstract method to connect to the broker.
-        _close(exc_type: Optional[Type[BaseException]] = None, exc_val: Optional[BaseException] = None, exec_tb: Optional[TracebackType] = None) : Abstract method to close the connection to the broker.
-        close(exc_type: Optional[Type[BaseException]] = None, exc_val: Optional[BaseException] = None, exec_tb: Optional[TracebackType] = None) : Close the connection to the broker.
-        _process_message(func: Callable[[StreamMessage[MsgType]], Awaitable[T_HandlerReturn]], watcher: BaseWatcher) : Abstract method to process a message.
-        publish(message: SendableMessage, *args: Any, reply_to: str = "", rpc: bool = False, rpc_timeout: Optional[float]
-
+        timestamp (int): The timestamp of the message.
+        key (Optional[Union[str, bytes]]): The key of the message, can be a string or bytes.
+        value (Optional[Union[str, bytes]]): The value of the message, can be a string or bytes.
+        headers (List[Tuple[str, bytes]]): A list of headers associated with the message.
     """
 
-    handlers: Mapping[Any, AsyncHandler[MsgType]]
-    middlewares: Sequence[Callable[[MsgType], BaseMiddleware]]
-    _global_parser: Optional[AsyncCustomParser[MsgType, StreamMessage[MsgType]]]
-    _global_decoder: Optional[AsyncCustomDecoder[StreamMessage[MsgType]]]
-
-    @abstractmethod
-    async def start(self) -> None:
-        """Start the broker async use case."""
-        super()._abc_start()
-        for h in self.handlers.values():
-            for f, _, _, _, _, _ in h.calls:
-                f.refresh(with_mock=False)
-        await self.connect()
-
-    @abstractmethod
-    async def _connect(self, **kwargs: Any) -> ConnectionType:
-        """Connect to a resource.
-
-        Args:
-            **kwargs: Additional keyword arguments for the connection.
+    timestamp: int
+    key: Optional[Union[str, bytes]]
+    value: Optional[Union[str, bytes]]
+    headers: List[Tuple[str, bytes]]
 
-        Returns:
-            The connection object.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
 
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    async def _close(
-        self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> None:
-        """Close the object.
-
-        Args:
-            exc_type: Optional. The type of the exception.
-            exc_val: Optional. The exception value.
-            exec_tb: Optional. The traceback of the exception.
-
-        Returns:
-            None
+class BatchBuilder:
+    """A helper class to build a batch of messages to send to Kafka."""
 
-        """
-        super()._abc__close(exc_type, exc_val, exec_tb)
+    def __init__(self) -> None:
+        """Initializes a new BatchBuilder instance."""
+        self._builder: List[MsgToSend] = []
 
-    async def close(
+    def append(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
+        *,
+        timestamp: Optional[int] = None,
+        key: Optional[Union[str, bytes]] = None,
+        value: Optional[Union[str, bytes]] = None,
+        headers: Optional[List[Tuple[str, bytes]]] = None,
     ) -> None:
-        """Closes the object.
-
-        Args:
-            exc_type: The type of the exception being handled, if any.
-            exc_val: The exception instance being handled, if any.
-            exec_tb: The traceback of the exception being handled, if any.
-
-        Returns:
-            None
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        super()._abc_close(exc_type, exc_val, exec_tb)
-
-        for h in self.handlers.values():
-            await h.close()
+        """Appends a message to the batch with optional timestamp, key, value, and headers."""
+        if timestamp is None:
+            timestamp = round(time() * 1000)
+
+        if key is None and value is None:
+            raise KafkaException(
+                KafkaError(40, reason="Both key and value can't be None")
+            )
 
-        if self._connection is not None:
-            await self._close(exc_type, exc_val, exec_tb)
-
-    @override
-    @abstractmethod
-    def _process_message(
-        self,
-        func: Callable[[StreamMessage[MsgType]], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[
-        [StreamMessage[MsgType]],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ]:
-        """Process a message.
-
-        Args:
-            func: A callable function that takes a StreamMessage and returns an Awaitable.
-            watcher: An instance of BaseWatcher.
-            disable_watcher: Whether to use watcher context.
-            kwargs: Additional keyword arguments.
-
-        Returns:
-            A callable function that takes a StreamMessage and returns an Awaitable.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    async def publish(
-        self,
-        message: SendableMessage,
-        *args: Any,
-        reply_to: str = "",
-        rpc: bool = False,
-        rpc_timeout: Optional[float] = None,
-        raise_timeout: bool = False,
-        **kwargs: Any,
-    ) -> Optional[SendableMessage]:
-        """Publish a message.
-
-        Args:
-            message: The message to be published.
-            *args: Additional arguments.
-            reply_to: The reply-to address for the message.
-            rpc: Whether the message is for RPC.
-            rpc_timeout: The timeout for RPC.
-            raise_timeout: Whether to raise an exception on timeout.
-            **kwargs: Additional keyword arguments.
+        if headers is None:
+            headers = []
 
-        Returns:
-            The published message.
-
-        Raises:
-            NotImplementedError: If the method is not implemented.
-
-        """
-        raise NotImplementedError()
-
-    @override
-    @abstractmethod
-    def subscriber(  # type: ignore[override,return]
-        self,
-        *broker_args: Any,
-        retry: Union[bool, int] = False,
-        dependencies: Sequence[Depends] = (),
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        middlewares: Optional[Sequence[Callable[[MsgType], BaseMiddleware]]] = None,
-        filter: Filter[StreamMessage[MsgType]] = default_filter,
-        _raw: bool = False,
-        _get_dependant: Optional[Any] = None,
-        **broker_kwargs: Any,
-    ) -> Callable[
-        [
-            Union[
-                Callable[P_HandlerParams, T_HandlerReturn],
-                HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-            ]
-        ],
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-    ]:
-        """A function decorator for subscribing to a message broker.
-
-        Args:
-            *broker_args: Positional arguments to be passed to the message broker.
-            retry: Whether to retry the subscription if it fails. Can be a boolean or an integer specifying the number of retries.
-            dependencies: Sequence of dependencies to be injected into the decorated function.
-            decoder: Custom decoder function for decoding the message.
-            parser: Custom parser function for parsing the decoded message.
-            middlewares: Sequence of middleware functions to be applied to the message.
-            filter: Filter function for filtering the messages to be processed.
-            _raw: Whether to return the raw message instead of the processed result.
-            _get_dependant: Optional argument to get the dependant object.
-            **broker_kwargs: Keyword arguments to be passed to the message broker.
-
-        Returns:
-            A callable decorator that wraps the decorated function and handles the subscription.
+        self._builder.append(
+            MsgToSend(timestamp=timestamp, key=key, value=value, headers=headers)
+        )
 
-        Raises:
-            NotImplementedError: If silent animals are not supported.
 
-        """
-        super().subscriber()
+class AsyncConfluentProducer:
+    """An asynchronous Python Kafka client using the "confluent-kafka" package."""
 
     def __init__(
         self,
-        *args: Any,
-        apply_types: bool = True,
-        validate: bool = True,
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
-        dependencies: Sequence[Depends] = (),
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType, StreamMessage[MsgType]]] = None,
-        middlewares: Optional[Sequence[Callable[[MsgType], BaseMiddleware]]] = None,
-        graceful_timeout: Optional[float] = None,
-        **kwargs: Any,
+        *,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        bootstrap_servers: Union[str, List[str]] = "localhost",
+        client_id: Optional[str] = None,
+        metadata_max_age_ms: int = 300000,
+        request_timeout_ms: int = 40000,
+        api_version: str = "auto",
+        acks: Any = _missing,
+        key_serializer: Optional[Callable[[bytes], bytes]] = None,
+        value_serializer: Optional[Callable[[bytes], bytes]] = None,
+        compression_type: Optional[str] = None,
+        max_batch_size: int = 16384,
+        partitioner: str = "consistent_random",
+        max_request_size: int = 1048576,
+        linger_ms: int = 0,
+        send_backoff_ms: int = 100,
+        retry_backoff_ms: int = 100,
+        security_protocol: str = "PLAINTEXT",
+        ssl_context: Optional[SSLContext] = None,
+        connections_max_idle_ms: int = 540000,
+        enable_idempotence: bool = False,
+        transactional_id: Optional[Union[str, int]] = None,
+        transaction_timeout_ms: int = 60000,
+        sasl_mechanism: Optional[str] = None,
+        sasl_plain_password: Optional[str] = None,
+        sasl_plain_username: Optional[str] = None,
+        sasl_kerberos_service_name: str = "kafka",
+        sasl_kerberos_domain_name: Optional[str] = None,
+        sasl_oauth_token_provider: Optional[str] = None,
     ) -> None:
-        """Initialize the class.
-
-        Args:
-            *args: Variable length arguments
-            apply_types: Whether to apply types or not
-            validate: Whether to cast types using Pydantic validation.
-            logger: Logger object for logging
-            log_level: Log level for logging
-            log_fmt: Log format for logging
-            dependencies: Sequence of dependencies
-            decoder: Custom decoder object
-            parser: Custom parser object
-            middlewares: Sequence of middlewares
-            graceful_timeout: Graceful timeout
-            **kwargs: Keyword arguments
+        if isinstance(bootstrap_servers, Iterable) and not isinstance(
+            bootstrap_servers, str
+        ):
+            bootstrap_servers = ",".join(bootstrap_servers)
+
+        if compression_type is None:
+            compression_type = "none"
+
+        if acks is _missing or acks == "all":
+            acks = -1
+
+        self.config = {
+            # "topic.metadata.refresh.interval.ms": 1000,
+            "bootstrap.servers": bootstrap_servers,
+            "client.id": client_id,
+            "metadata.max.age.ms": metadata_max_age_ms,
+            "request.timeout.ms": request_timeout_ms,
+            "acks": acks,
+            "compression.type": compression_type,
+            "partitioner": partitioner,
+            "message.max.bytes": max_request_size,
+            "linger.ms": linger_ms,
+            "enable.idempotence": enable_idempotence,
+            "transactional.id": transactional_id,
+            "transaction.timeout.ms": transaction_timeout_ms,
+            "retry.backoff.ms": retry_backoff_ms,
+            "security.protocol": security_protocol.lower(),
+            "connections.max.idle.ms": connections_max_idle_ms,
+            "sasl.kerberos.service.name": sasl_kerberos_service_name,
+        }
+        if sasl_mechanism:
+            self.config.update(
+                {
+                    "sasl.mechanism": sasl_mechanism,
+                    "sasl.username": sasl_plain_username,
+                    "sasl.password": sasl_plain_password,
+                }
+            )
+
+        self.producer = Producer(self.config)
+        # self.producer.init_transactions()
+        self.producer.list_topics()
+        self.loop = loop or asyncio.get_event_loop()
+
+    async def stop(self) -> None:
+        """Stop the Kafka producer and flush remaining messages."""
+        self.producer.flush()
 
-        """
-        super().__init__(
-            *args,
-            apply_types=apply_types,
-            validate=validate,
-            logger=logger,
-            log_level=log_level,
-            log_fmt=log_fmt,
-            dependencies=dependencies,
-            decoder=cast(
-                Optional[AsyncCustomDecoder[StreamMessage[MsgType]]],
-                to_async(decoder) if decoder else None,
-            ),
-            parser=cast(
-                Optional[AsyncCustomParser[MsgType, StreamMessage[MsgType]]],
-                to_async(parser) if parser else None,
-            ),
-            middlewares=middlewares,
+    async def send(
+        self,
+        topic: str,
+        value: Optional[Union[str, bytes]] = None,
+        key: Optional[Union[str, bytes]] = None,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[List[Tuple[str, Union[str, bytes]]]] = None,
+    ) -> None:
+        """Sends a single message to a Kafka topic."""
+        kwargs = {
+            k: v
+            for k, v in {
+                "value": value,
+                "key": key,
+                "partition": partition,
+                "headers": headers,
+            }.items()
+            if v is not None
+        }
+        if timestamp_ms is not None:
+            kwargs["timestamp"] = timestamp_ms
+        self.producer.produce(
+            topic,
             **kwargs,
         )
-        self.graceful_timeout = graceful_timeout
-
-    async def connect(self, *args: Any, **kwargs: Any) -> ConnectionType:
-        """Connect to a remote server.
+        self.producer.poll(0)
 
-        Args:
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
+    def create_batch(self) -> BatchBuilder:
+        """Creates a batch for sending multiple messages.
 
         Returns:
-            The connection object.
-
+            BatchBuilder: An instance of BatchBuilder for building message batches.
         """
-        if self._connection is None:
-            _kwargs = self._resolve_connection_kwargs(*args, **kwargs)
-            self._connection = await self._connect(**_kwargs)
-        return self._connection
-
-    async def __aenter__(self) -> Self:
-        """Enter the context manager."""
-        await self.connect()
-        return self
+        return BatchBuilder()
 
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exec_tb: Optional[TracebackType],
+    async def send_batch(
+        self, batch: BatchBuilder, topic: str, *, partition: Optional[int]
     ) -> None:
-        """Exit the context manager.
+        """Sends a batch of messages to a Kafka topic."""
+        tasks = [
+            self.send(
+                topic=topic,
+                partition=partition,
+                timestamp_ms=msg.timestamp,
+                key=msg.key,
+                value=msg.value,
+                headers=msg.headers,  # type: ignore[arg-type]
+            )
+            for msg in batch._builder
+        ]
+        await asyncio.gather(*tasks)
+
+
+class TopicPartition(NamedTuple):
+    """A named tuple representing a Kafka topic and partition."""
+
+    topic: str
+    partition: int
+
+
+def create_topics(
+    topics: List[str],
+    config: Dict[str, Optional[Union[str, int, float, bool, Any]]],
+) -> None:
+    """Creates Kafka topics using the provided configuration."""
+    required_config_params = (
+        "allow.auto.create.topics",
+        "bootstrap.servers",
+        "client.id",
+        "request.timeout.ms",
+        "metadata.max.age.ms",
+        "security.protocol",
+        "connections.max.idle.ms",
+        "sasl.mechanism",
+        "sasl.username",
+        "sasl.password",
+        "sasl.kerberos.service.name",
+    )
+
+    admin_client = AdminClient(
+        {x: config[x] for x in required_config_params if x in config}
+    )
+
+    fs = admin_client.create_topics(
+        [NewTopic(topic, num_partitions=1, replication_factor=1) for topic in topics]
+    )
+
+    for topic, f in fs.items():
+        try:
+            f.result()  # The result itself is None
+        except Exception as e:  # noqa: PERF203
+            if "TOPIC_ALREADY_EXISTS" not in str(e):
+                logger.warning(f"Failed to create topic {topic}: {e}")
+        else:
+            logger.info(f"Topic `{topic}` created.")
 
-        Args:
-            exc_type: The type of the exception raised, if any.
-            exc_val: The exception raised, if any.
-            exec_tb: The traceback of the exception raised, if any.
 
-        Returns:
-            None
-
-        Overrides:
-            This method overrides the __aexit__ method of the base class.
+class AsyncConfluentConsumer:
+    """An asynchronous Python Kafka client for consuming messages using the "confluent-kafka" package."""
 
-        """
-        await self.close(exc_type, exc_val, exec_tb)
-
-    @override
-    def _wrap_decode_message(
+    def __init__(
         self,
-        func: Callable[..., Awaitable[T_HandlerReturn]],
-        params: Sized = (),
-        _raw: bool = False,
-    ) -> Callable[[StreamMessage[MsgType]], Awaitable[T_HandlerReturn]]:
-        """Wraps a function to decode a message and pass it as an argument to the wrapped function.
-
-        Args:
-            func: The function to be wrapped.
-            params: The parameters to be passed to the wrapped function.
-            _raw: Whether to return the raw message or not.
+        *topics: str,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        bootstrap_servers: Union[str, List[str]] = "localhost",
+        client_id: Optional[str] = "confluent-kafka-consumer",
+        group_id: Optional[str] = None,
+        group_instance_id: Optional[str] = None,
+        key_deserializer: Optional[Callable[[bytes], bytes]] = None,
+        value_deserializer: Optional[Callable[[bytes], bytes]] = None,
+        fetch_max_wait_ms: int = 500,
+        fetch_max_bytes: int = 52428800,
+        fetch_min_bytes: int = 1,
+        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
+        request_timeout_ms: int = 40 * 1000,
+        retry_backoff_ms: int = 100,
+        auto_offset_reset: str = "latest",
+        enable_auto_commit: bool = True,
+        auto_commit_interval_ms: int = 5000,
+        check_crcs: bool = True,
+        metadata_max_age_ms: int = 5 * 60 * 1000,
+        partition_assignment_strategy: Union[str, List[Any]] = "roundrobin",
+        max_poll_interval_ms: int = 300000,
+        rebalance_timeout_ms: Optional[int] = None,
+        session_timeout_ms: int = 10000,
+        heartbeat_interval_ms: int = 3000,
+        consumer_timeout_ms: int = 200,
+        max_poll_records: Optional[int] = None,
+        ssl_context: Optional[SSLContext] = None,
+        security_protocol: str = "PLAINTEXT",
+        api_version: str = "auto",
+        exclude_internal_topics: bool = True,
+        connections_max_idle_ms: int = 540000,
+        isolation_level: str = "read_uncommitted",
+        sasl_mechanism: Optional[str] = None,
+        sasl_plain_password: Optional[str] = None,
+        sasl_plain_username: Optional[str] = None,
+        sasl_kerberos_service_name: str = "kafka",
+        sasl_kerberos_domain_name: Optional[str] = None,
+        sasl_oauth_token_provider: Optional[str] = None,
+    ) -> None:
+        if group_id is None:
+            group_id = "confluent-kafka-consumer-group"
 
-        Returns:
-            The wrapped function.
+        if isinstance(bootstrap_servers, Iterable) and not isinstance(
+            bootstrap_servers, str
+        ):
+            bootstrap_servers = ",".join(bootstrap_servers)
+
+        self.topics = list(topics)
+
+        if not isinstance(partition_assignment_strategy, str):
+            partition_assignment_strategy = ",".join(
+                [
+                    x if isinstance(x, str) else x().name
+                    for x in partition_assignment_strategy
+                ]
+            )
+        self.config = {
+            "allow.auto.create.topics": True,
+            # "topic.metadata.refresh.interval.ms": 1000,
+            "bootstrap.servers": bootstrap_servers,
+            "client.id": client_id,
+            "group.id": group_id,
+            "group.instance.id": group_instance_id,
+            "fetch.wait.max.ms": fetch_max_wait_ms,
+            "fetch.max.bytes": fetch_max_bytes,
+            "fetch.min.bytes": fetch_min_bytes,
+            "max.partition.fetch.bytes": max_partition_fetch_bytes,
+            # "request.timeout.ms": request_timeout_ms,
+            "fetch.error.backoff.ms": retry_backoff_ms,
+            "auto.offset.reset": auto_offset_reset,
+            "enable.auto.commit": enable_auto_commit,
+            "auto.commit.interval.ms": auto_commit_interval_ms,
+            "check.crcs": check_crcs,
+            "metadata.max.age.ms": metadata_max_age_ms,
+            "partition.assignment.strategy": partition_assignment_strategy,
+            "max.poll.interval.ms": max_poll_interval_ms,
+            "session.timeout.ms": session_timeout_ms,
+            "heartbeat.interval.ms": heartbeat_interval_ms,
+            "security.protocol": security_protocol.lower(),
+            "connections.max.idle.ms": connections_max_idle_ms,
+            "isolation.level": isolation_level,
+            "sasl.kerberos.service.name": sasl_kerberos_service_name,
+        }
+        if sasl_mechanism:
+            self.config.update(
+                {
+                    "sasl.mechanism": sasl_mechanism,
+                    "sasl.username": sasl_plain_username,
+                    "sasl.password": sasl_plain_password,
+                }
+            )
 
-        Raises:
-            AssertionError: If the code reaches an unreachable state.
+        self.loop = loop or asyncio.get_event_loop()
 
-        """
-        params_ln = len(params)
+        create_topics(topics=self.topics, config=self.config)
+        self.consumer = Consumer(self.config)
 
-        @wraps(func)
-        async def decode_wrapper(message: StreamMessage[MsgType]) -> T_HandlerReturn:
-            """A wrapper function to decode and handle a message.
-
-            Args:
-                message : The message to be decoded and handled
-
-            Returns:
-                The return value of the handler function
-
-            Raises:
-                AssertionError: If the code reaches an unreachable state
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            if _raw is True:
-                return await func(message)
-
-            msg = message.decoded_body
-            if params_ln > 1:
-                if isinstance(msg, Mapping):
-                    return await func(**msg)
-                elif isinstance(msg, Sequence):
-                    return await func(*msg)
+    async def start(self) -> None:
+        """Starts the Kafka consumer and subscribes to the specified topics."""
+        self.consumer.subscribe(self.topics)
+
+    async def commit(self, asynchronous: bool = True) -> None:
+        """Commits the offsets of all messages returned by the last poll operation."""
+        await call_or_await(self.consumer.commit, asynchronous=asynchronous)
+
+    async def stop(self) -> None:
+        """Stops the Kafka consumer and releases all resources."""
+        # NOTE: If we don't explicitly call commit and then close the consumer, the confluent consumer gets stuck.
+        # We are doing this to avoid the issue.
+        enable_auto_commit = self.config["enable.auto.commit"]
+        try:
+            if enable_auto_commit:
+                await self.commit(asynchronous=False)
+
+        except Exception as e:
+            # No offset stored issue is not a problem - https://github.com/confluentinc/confluent-kafka-python/issues/295#issuecomment-355907183
+            if "No offset stored" in str(e):
+                pass
             else:
-                return await func(msg)
+                raise e
 
-            raise AssertionError("unreachable")
+        # Wrap calls to async to make method cancelable by timeout
+        await call_or_await(self.consumer.close)
 
-        return decode_wrapper
+    async def getone(self, timeout_ms: int = 1000) -> Optional[Message]:
+        """Consumes a single message from Kafka."""
+        msg = await call_or_await(self.consumer.poll, timeout_ms / 1000)
+        return check_msg_error(msg)
 
-    @override
-    def _wrap_handler(
+    async def getmany(
         self,
-        func: Callable[P_HandlerParams, T_HandlerReturn],
-        *,
-        retry: Union[bool, int] = False,
-        extra_dependencies: Sequence[Depends] = (),
-        no_ack: bool = False,
-        _raw: bool = False,
-        _get_dependant: Optional[Any] = None,
-        _process_kwargs: Optional[AnyDict] = None,
-    ) -> Tuple[
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-        CallModel[P_HandlerParams, T_HandlerReturn],
-    ]:
-        """Wrap a handler function.
-
-        Args:
-            func: The handler function to wrap.
-            retry: Whether to retry the handler function if it fails. Can be a boolean or an integer specifying the number of retries.
-            extra_dependencies: Additional dependencies to inject into the handler function.
-            no_ack: Whether not to ack/nack/reject messages.
-            _raw: Whether to return the raw response from the handler function.
-            _get_dependant: An optional object to use as the dependant for the handler function.
-            **broker_log_context_kwargs: Additional keyword arguments to pass to the broker log context.
+        timeout_ms: int = 0,
+        max_records: Optional[int] = 10,
+    ) -> Tuple[Message, ...]:
+        """Consumes a batch of messages from Kafka and groups them by topic and partition."""
+        raw_messages: List[Optional[Message]] = await call_or_await(
+            self.consumer.consume,
+            num_messages=max_records or 10,
+            timeout=timeout_ms / 1000,
+        )
 
-        Returns:
-            A tuple containing the wrapped handler function and the call model.
+        return tuple(x for x in map(check_msg_error, raw_messages) if x is not None)
 
-        """
-        return super()._wrap_handler(  # type: ignore[return-value]
-            func,
-            retry=retry,
-            extra_dependencies=extra_dependencies,
-            no_ack=no_ack,
-            _raw=_raw,
-            _get_dependant=_get_dependant,
-            _process_kwargs=_process_kwargs,
-        )
+
+def check_msg_error(msg: Optional[Message]) -> Optional[Message]:
+    """Checks for errors in the consumed message."""
+    if msg is None or msg.error():
+        return None
+
+    return msg
```

### Comparing `faststream-0.4.7/faststream/broker/core/mixins.py` & `faststream-0.5.0rc0/faststream/nats/broker/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,71 @@
 import logging
-from typing import Any, Optional
+from inspect import Parameter
+from typing import Any, ClassVar, Optional, Union
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import MsgType
-from faststream.log import access_logger
-from faststream.types import AnyDict
+from nats.aio.client import Client
+from nats.aio.msg import Msg
 
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.log.logging import get_broker_logger
 
-class LoggingMixin:
-    """A mixin class for logging.
 
-    Attributes:
-        logger : logger object used for logging
-        log_level : log level for logging
-        _fmt : format string for log messages
+class NatsLoggingBroker(BrokerUsecase[Msg, Client]):
+    """A class that extends the LoggingMixin class and adds additional functionality for logging NATS related information."""
 
-    Methods:
-        fmt : getter method for _fmt attribute
-        _get_log_context : returns a dictionary with log context information
-        _log : logs a message with optional log level, extra data, and exception info
-
-    """
+    _max_queue_len: int
+    _max_subject_len: int
+    __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
+        logger: Union[logging.Logger, object, None] = Parameter.empty,
         log_level: int = logging.INFO,
-        log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
+        log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize the class.
-
-        Args:
-            *args: Variable length argument list
-            logger: Optional logger object
-            log_level: Log level (default: logging.INFO)
-            log_fmt: Log format (default: "%(asctime)s %(levelname)s - %(message)s")
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            None
-
-        """
-        self.logger = logger
-        self.log_level = log_level
-        self._fmt = log_fmt
-        self._message_id_ln = 10
-
-    @property
-    def fmt(self) -> str:  # pragma: no cover
-        """Getter method for _fmt attribute."""
-        return self._fmt or ""
+        """Initialize the NATS logging mixin."""
+        super().__init__(
+            *args,
+            logger=logger,
+            # TODO: generate unique logger names to not share between brokers
+            default_logger=get_broker_logger(
+                name="nats",
+                default_context={
+                    "subject": "",
+                    "stream": "",
+                    "queue": "",
+                },
+                message_id_ln=self.__max_msg_id_ln,
+            ),
+            log_level=log_level,
+            log_fmt=log_fmt,
+            **kwargs,
+        )
+
+        self._max_queue_len = 0
+        self._max_stream_len = 0
+        self._max_subject_len = 4
+
+    def get_fmt(self) -> str:
+        """Fallback method to get log format if `log_fmt` if not specified."""
+        return (
+            "%(asctime)s %(levelname)-8s - "
+            + (f"%(stream)-{self._max_stream_len}s | " if self._max_stream_len else "")
+            + (f"%(queue)-{self._max_queue_len}s | " if self._max_queue_len else "")
+            + f"%(subject)-{self._max_subject_len}s | "
+            + f"%(message_id)-{self.__max_msg_id_ln}s - "
+            "%(message)s"
+        )
 
-    def _get_log_context(
+    def _setup_log_context(
         self,
-        message: Optional[StreamMessage[MsgType]],
-        **kwargs: str,
-    ) -> AnyDict:
-        """Get the log context.
-
-        Args:
-            message: Optional stream message
-            **kwargs: Additional keyword arguments
-
-        Returns:
-            A dictionary containing the log context with the following keys:
-                - message_id: The first 10 characters of the message_id if message is not None, otherwise an empty string
-
-        """
-        return {
-            "message_id": message.message_id[: self._message_id_ln] if message else "",
-        }
-
-    def _log(
-        self,
-        message: str,
-        log_level: Optional[int] = None,
-        extra: Optional[AnyDict] = None,
-        exc_info: Optional[Exception] = None,
+        *,
+        queue: Optional[str] = None,
+        subject: Optional[str] = None,
+        stream: Optional[str] = None,
     ) -> None:
-        """Logs a message.
-
-        Args:
-            message: The message to be logged.
-            log_level: The log level of the message. If not provided, the default log level of the logger will be used.
-            extra: Additional information to be logged along with the message. This should be a dictionary.
-            exc_info: An exception to be logged along with the message.
-
-        Returns:
-            None
-
-        """
-        if self.logger is not None:
-            self.logger.log(
-                (log_level or self.log_level),
-                message,
-                extra=extra,
-                exc_info=exc_info,
-            )
+        """Setup subscriber's information to generate default log format."""
+        self._max_subject_len = max((self._max_subject_len, len(subject or "")))
+        self._max_queue_len = max((self._max_queue_len, len(queue or "")))
+        self._max_stream_len = max((self._max_stream_len, len(stream or "")))
```

### Comparing `faststream-0.4.7/faststream/broker/fastapi/context.py` & `faststream-0.5.0rc0/faststream/broker/fastapi/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
-from inspect import Signature
+from inspect import Parameter
 from typing import Any, Callable, Optional
 
 from fastapi import params
 from typing_extensions import Annotated
 
 from faststream.utils.context import ContextRepo as CR
 from faststream.utils.context.types import resolve_context_by_name
 
 
 def Context(  # noqa: N802
     name: str,
     *,
-    default: Any = Signature.empty,
+    default: Any = Parameter.empty,
     initial: Optional[Callable[..., Any]] = None,
 ) -> Any:
+    """Get access to objects of the Context."""
     return params.Depends(
         lambda: resolve_context_by_name(
             name=name,
             default=default,
             initial=initial,
         ),
         use_cache=True,
```

### Comparing `faststream-0.4.7/faststream/broker/fastapi/route.py` & `faststream-0.5.0rc0/faststream/broker/fastapi/route.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,311 +1,281 @@
 import asyncio
 import inspect
 from contextlib import AsyncExitStack
 from functools import wraps
 from itertools import dropwhile
 from typing import (
+    TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
-    Coroutine,
     Generic,
+    Iterable,
     List,
-    Sequence,
+    Optional,
     Union,
-    cast,
 )
 
 from fastapi import params
+from fastapi.background import BackgroundTasks
 from fastapi.dependencies.models import Dependant
-from fastapi.dependencies.utils import (
-    get_dependant,
-    get_parameterless_sub_dependant,
-    solve_dependencies,
-)
-from fastapi.routing import run_endpoint_function
+from fastapi.dependencies.utils import solve_dependencies
+from fastapi.routing import run_endpoint_function, serialize_response
+from fastapi.utils import create_response_field
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
 from faststream._compat import FASTAPI_V106, raise_fastapi_validation_error
-from faststream.broker.core.asynchronous import BrokerAsyncUsecase
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.broker.fastapi.get_dependant import get_fastapi_native_dependant
 from faststream.broker.message import StreamMessage as NativeMessage
 from faststream.broker.schemas import NameRequired
 from faststream.broker.types import MsgType, P_HandlerParams, T_HandlerReturn
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.types import AnyDict, SendableMessage
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from fastapi._compat import ModelField
+    from fastapi.types import IncEx
 
-class StreamRoute(BaseRoute, Generic[MsgType, P_HandlerParams, T_HandlerReturn]):
-    """A class representing a stream route.
 
-    Attributes:
-        handler : HandlerCallWrapper object representing the handler for the route
-        path : path of the route
-        broker : BrokerAsyncUsecase object representing the broker for the route
-        dependant : Dependable object representing the dependencies for the route
-    """
+class StreamRoute(BaseRoute, Generic[MsgType, P_HandlerParams, T_HandlerReturn]):
+    """A class representing a stream route."""
 
     handler: HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]
 
     def __init__(
         self,
         path: Union[NameRequired, str, None],
-        *extra: Union[NameRequired, str],
+        *extra: Any,
+        provider_factory: Callable[[], Any],
         endpoint: Union[
             Callable[P_HandlerParams, T_HandlerReturn],
             HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
         ],
-        broker: BrokerAsyncUsecase[MsgType, Any],
-        dependencies: Sequence[params.Depends],
-        provider_factory: Callable[[], Any],
+        broker: BrokerUsecase[MsgType, Any],
+        dependencies: Iterable[params.Depends],
+        response_model: Any,
+        response_model_include: Optional["IncEx"],
+        response_model_exclude: Optional["IncEx"],
+        response_model_by_alias: bool,
+        response_model_exclude_unset: bool,
+        response_model_exclude_defaults: bool,
+        response_model_exclude_none: bool,
         **handle_kwargs: Any,
     ) -> None:
-        """Initialize a class instance.
-
-        Args:
-            path: The path of the instance.
-            *extra: Additional arguments.
-            endpoint: The endpoint of the instance.
-            broker: The broker of the instance.
-            dependencies: The dependencies of the instance.
-            provider_factory: Provider factory for dependency overrides.
-            **handle_kwargs: Additional keyword arguments.
-
-        Returns:
-            None.
-        """
-        self.path = path or ""
+        self.path, path_name = path or "", getattr(path, "name", "")
         self.broker = broker
 
-        path_name = self.path if isinstance(self.path, str) else self.path.name
-
         if isinstance(endpoint, HandlerCallWrapper):
             orig_call = endpoint._original_call
+            while hasattr(orig_call, "__consumer__"):
+                orig_call = orig_call.__wrapped__  # type: ignore[attr-defined]
+
         else:
             orig_call = endpoint
 
-        dependant = get_dependant(
-            path=path_name,
-            call=orig_call,
+        dependent = get_fastapi_native_dependant(
+            orig_call,
+            list(dependencies),
+            path_name=path_name,
         )
-        for depends in dependencies[::-1]:
-            dependant.dependencies.insert(
-                0,
-                get_parameterless_sub_dependant(depends=depends, path=path_name),
+
+        if response_model:
+            response_field = create_response_field(
+                name="ResponseModel",
+                type_=response_model,
+                mode="serialization",
             )
-        self.dependant = dependant
+        else:
+            response_field = None
 
         call = wraps(orig_call)(
-            StreamMessage.get_session(
-                dependant,
-                provider_factory,
+            StreamMessage.get_consumer(
+                dependent=dependent,
+                provider_factory=provider_factory,
+                response_field=response_field,
+                response_model_include=response_model_include,
+                response_model_exclude=response_model_exclude,
+                response_model_by_alias=response_model_by_alias,
+                response_model_exclude_unset=response_model_exclude_unset,
+                response_model_exclude_defaults=response_model_exclude_defaults,
+                response_model_exclude_none=response_model_exclude_none,
             )
         )
 
         if isinstance(endpoint, HandlerCallWrapper):
             endpoint._original_call = call
             handler = endpoint
 
         else:
             handler = call
 
-        self.handler = broker.subscriber(
+        self.handler = broker.subscriber(  # type: ignore[assignment,call-arg]
             *extra,
-            _raw=True,
-            _get_dependant=lambda call: dependant,
+            dependencies=list(dependencies),
             **handle_kwargs,
-        )(
-            handler  # type: ignore[arg-type]
-        )
+        )(handler)
 
 
 class StreamMessage(Request):
-    """A class to represent a stream message.
-
-    Attributes:
-        scope : dictionary representing the scope of the message
-        _cookies : dictionary representing the cookies of the message
-        _headers : dictionary representing the headers of the message
-        _body : dictionary representing the body of the message
-        _query_params : dictionary representing the query parameters of the message
-
-    Methods:
-        __init__ : initializes the StreamMessage object
-        get_session : returns a callable function that handles the session of the message
-    """
+    """A class to represent a stream message."""
 
     scope: AnyDict
     _cookies: AnyDict
     _headers: AnyDict  # type: ignore
     _body: Union[AnyDict, List[Any]]  # type: ignore
     _query_params: AnyDict  # type: ignore
+    _background: Optional[BackgroundTasks]
 
     def __init__(
         self,
         *,
         body: Union[AnyDict, List[Any]],
         headers: AnyDict,
         path: AnyDict,
     ) -> None:
-        """Initialize a class instance.
-
-        Args:
-            body: The body of the request as a dictionary.
-            headers: The headers of the request as a dictionary.
-            path: The path of the request as a dictionary.
-
-        Attributes:
-            scope: A dictionary to store the scope of the request.
-            _cookies: A dictionary to store the cookies of the request.
-            _headers: A dictionary to store the headers of the request.
-            _body: A dictionary to store the body of the request.
-            _query_params: A dictionary to store the query parameters of the request.
-
-        """
+        """Initialize a class instance."""
         self._headers = headers
         self._body = body
         self._query_params = path
 
         self.scope = {"path_params": self._query_params}
         self._cookies = {}
 
     @classmethod
-    def get_session(
-        cls, dependant: Dependant, provider_factory: Callable[[], Any]
-    ) -> Callable[[NativeMessage[Any]], Awaitable[SendableMessage]]:
-        """Creates a session for handling requests.
-
-        Args:
-            dependant: The dependant object representing the session.
-            provider_factory: Provider factory for dependency overrides.
-
-        Returns:
-            A callable that takes a native message and returns an awaitable sendable message.
-
-        Raises:
-            AssertionError: If the dependant call is not defined.
-
-        Note:
-            This function is used to create a session for handling requests. It takes a dependant object, which represents the session, and a dependency overrides provider, which allows for overriding dependencies. It returns a callable that takes a native message and returns an awaitable sendable message. The session is created based on the dependant object and the message passed to the callable. The session is then used to call the function obtained from the dependant object, and the result is returned.
-        """
-        assert dependant.call  # nosec B101
-
-        func = get_app(dependant, provider_factory)
+    def get_consumer(
+        cls,
+        *,
+        dependent: Dependant,
+        provider_factory: Callable[[], Any],
+        response_field: Optional["ModelField"],
+        response_model_include: Optional["IncEx"],
+        response_model_exclude: Optional["IncEx"],
+        response_model_by_alias: bool,
+        response_model_exclude_unset: bool,
+        response_model_exclude_defaults: bool,
+        response_model_exclude_none: bool,
+    ) -> Callable[[NativeMessage[Any]], Awaitable[Any]]:
+        """Creates a session for handling requests."""
+        assert dependent.call  # nosec B101
+
+        consume = make_fastapi_execution(
+            dependent=dependent,
+            provider_factory=provider_factory,
+            response_field=response_field,
+            response_model_include=response_model_include,
+            response_model_exclude=response_model_exclude,
+            response_model_by_alias=response_model_by_alias,
+            response_model_exclude_unset=response_model_exclude_unset,
+            response_model_exclude_defaults=response_model_exclude_defaults,
+            response_model_exclude_none=response_model_exclude_none,
+        )
 
-        dependencies_names = tuple(i.name for i in dependant.dependencies)
+        dependencies_names = tuple(i.name for i in dependent.dependencies)
 
         first_arg = next(
             dropwhile(
                 lambda i: i in dependencies_names,
-                inspect.signature(dependant.call).parameters,
+                inspect.signature(dependent.call).parameters,
             ),
             None,
         )
 
-        async def app(message: NativeMessage[Any]) -> SendableMessage:
-            """An asynchronous function that processes an incoming message and returns a sendable message.
-
-            Args:
-                message : The incoming message to be processed
-
-            Returns:
-                The sendable message
-
-            Raises:
-                TypeError: If the body of the message is not a dictionary
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
+        async def real_consumer(message: NativeMessage[Any]) -> Any:
+            """An asynchronous function that processes an incoming message and returns a sendable message."""
             body = message.decoded_body
 
             fastapi_body: Union[AnyDict, List[Any]]
             if first_arg is not None:
                 if isinstance(body, dict):
                     path = fastapi_body = body or {}
                 elif isinstance(body, list):
                     fastapi_body, path = body, {}
                 else:
                     path = fastapi_body = {first_arg: body}
 
-                session = cls(
+                stream_message = cls(
                     body=fastapi_body,
                     headers=message.headers,
                     path={**path, **message.path},
                 )
 
             else:
-                session = cls(
+                stream_message = cls(
                     body={},
                     headers={},
                     path={},
                 )
 
-            return await func(session)
+            return await consume(stream_message, message)
 
-        return app
+        real_consumer.__consumer__ = True  # type: ignore[attr-defined]
+        return real_consumer
 
 
-def get_app(
-    dependant: Dependant,
+def make_fastapi_execution(
+    *,
+    dependent: Dependant,
     provider_factory: Callable[[], Any],
+    response_field: Optional["ModelField"],
+    response_model_include: Optional["IncEx"],
+    response_model_exclude: Optional["IncEx"],
+    response_model_by_alias: bool,
+    response_model_exclude_unset: bool,
+    response_model_exclude_defaults: bool,
+    response_model_exclude_none: bool,
 ) -> Callable[
-    [StreamMessage],
-    Coroutine[Any, Any, SendableMessage],
+    [StreamMessage, NativeMessage[Any]],
+    Awaitable[Any],
 ]:
-    """Creates a FastAPI application.
-
-    Args:
-        dependant: The dependant object that defines the endpoint function and its dependencies.
-        provider_factory: Provider factory for dependency overrides.
+    """Creates a FastAPI application."""
+    is_coroutine = asyncio.iscoroutinefunction(dependent.call)
 
-    Returns:
-        The FastAPI application as a callable that takes a StreamMessage object as input and returns a SendableMessage coroutine.
-
-    Raises:
-        AssertionError: If the code reaches an unreachable state.
-    """
-
-    async def app(request: StreamMessage) -> SendableMessage:
-        """Handle an HTTP request and return a response.
-
-        Args:
-            request: The incoming HTTP request.
-
-        Returns:
-            The response to be sent back to the client.
-
-        Raises:
-            AssertionError: If the code reaches an unreachable point.
-        """
+    async def app(
+        request: StreamMessage,
+        raw_message: NativeMessage[Any],
+    ) -> Any:
+        """Consume StreamMessage and return user function result."""
         async with AsyncExitStack() as stack:
             if FASTAPI_V106:
                 kwargs = {"async_exit_stack": stack}
             else:
                 request.scope["fastapi_astack"] = stack
                 kwargs = {}
 
             solved_result = await solve_dependencies(
                 request=request,
                 body=request._body,  # type: ignore[arg-type]
-                dependant=dependant,
+                dependant=dependent,
                 dependency_overrides_provider=provider_factory(),
                 **kwargs,  # type: ignore[arg-type]
             )
 
-            values, errors, _, _2, _3 = solved_result
+            values, errors, raw_message.background, _, _2 = solved_result  # type: ignore[attr-defined]
+
             if errors:
                 raise_fastapi_validation_error(errors, request._body)  # type: ignore[arg-type]
 
-            return cast(
-                SendableMessage,
-                await run_endpoint_function(
-                    dependant=dependant,
-                    values=values,
-                    is_coroutine=asyncio.iscoroutinefunction(dependant.call),
-                ),
+            raw_reponse = await run_endpoint_function(
+                dependant=dependent,
+                values=values,
+                is_coroutine=is_coroutine,
+            )
+
+            content = await serialize_response(
+                response_content=raw_reponse,
+                field=response_field,
+                include=response_model_include,
+                exclude=response_model_exclude,
+                by_alias=response_model_by_alias,
+                exclude_unset=response_model_exclude_unset,
+                exclude_defaults=response_model_exclude_defaults,
+                exclude_none=response_model_exclude_none,
+                is_coroutine=is_coroutine,
             )
 
-        raise AssertionError("unreachable")
+            return content
+
+        return None
 
     return app
```

### Comparing `faststream-0.4.7/faststream/cli/main.py` & `faststream-0.5.0rc0/faststream/cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import logging
 import sys
 import warnings
 from contextlib import suppress
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 import anyio
 import typer
 from click.exceptions import MissingParameter
-from pydantic import ValidationError
 from typer.core import TyperOption
 
+from faststream import FastStream
 from faststream.__about__ import INSTALL_WATCHFILES, __version__
+from faststream.broker.core.usecase import BrokerUsecase
 from faststream.cli.docs.app import docs_app
 from faststream.cli.utils.imports import import_from_string
 from faststream.cli.utils.logs import LogLevels, get_log_level, set_log_level
 from faststream.cli.utils.parser import parse_cli_args
-from faststream.types import SettingField
+from faststream.exceptions import SetupError, ValidationError
+from faststream.types import AnyDict, SettingField
 
 cli = typer.Typer(pretty_exceptions_short=True)
 cli.add_typer(docs_app, name="docs", help="AsyncAPI schema commands")
 
 
 def version_callback(version: bool) -> None:
-    """Callback function for displaying version information.
-
-    Args:
-        version: If True, display version information
-
-    Returns:
-        None
-    """
-    if version is True:
+    """Callback function for displaying version information."""
+    if version:
         import platform
 
         typer.echo(
             "Running FastStream {} with {} {} on {}".format(
                 __version__,
                 platform.python_implementation(),
                 platform.python_version(),
@@ -84,17 +79,17 @@
         "--reload",
         is_flag=True,
         help="Restart app at directory files changes",
     ),
     watch_extensions: List[str] = typer.Option(
         (),
         "--extension",
+        "--ext",
         "--reload-extension",
         "--reload-ext",
-        "--ext",
         help="List of file extensions to watch by",
     ),
     app_dir: str = typer.Option(
         ".",
         "--app-dir",
         help=(
             "Look for APP in the specified directory, by adding this to the PYTHONPATH."
@@ -114,30 +109,35 @@
 
     if app_dir:  # pragma: no branch
         sys.path.insert(0, app_dir)
 
     args = (app, extra, casted_log_level)
 
     if reload and workers > 1:
-        raise ValueError("You can't use reload option with multiprocessing")
+        raise SetupError("You can't use reload option with multiprocessing")
 
-    if reload is True:
+    if reload:
         try:
             from faststream.cli.supervisors.watchfiles import WatchReloader
         except ImportError:
             warnings.warn(INSTALL_WATCHFILES, category=ImportWarning, stacklevel=1)
             _run(*args)
 
         else:
             module_path, _ = import_from_string(app)
 
+            if app_dir != ".":
+                reload_dirs = [str(module_path), app_dir]
+            else:
+                reload_dirs = [str(module_path)]
+
             WatchReloader(
                 target=_run,
                 args=args,
-                reload_dirs=[str(module_path)] + ([app_dir] if app_dir else []),
+                reload_dirs=reload_dirs,
             ).run()
 
     elif workers > 1:
         from faststream.cli.supervisors.multiprocess import Multiprocess
 
         Multiprocess(
             target=_run,
@@ -152,30 +152,22 @@
 def _run(
     # NOTE: we should pass `str` due FastStream is not picklable
     app: str,
     extra_options: Dict[str, SettingField],
     log_level: int = logging.INFO,
     app_level: int = logging.INFO,
 ) -> None:
-    """Runs the specified application.
-
-    Args:
-        app: path to FastStream application.
-        extra_options: Additional options for the application.
-        log_level: Log level for the application (default: logging.INFO).
-        app_level: Log level for the application (default: logging.INFO).
-
-    Returns:
-        None
-
-    Note:
-        This function uses the `anyio.run()` function to run the application.
-    """
+    """Runs the specified application."""
     _, app_obj = import_from_string(app)
 
+    if not isinstance(app_obj, FastStream):
+        raise typer.BadParameter(
+            f'Imported object "{app_obj}" must be "FastStream" type.',
+        )
+
     set_log_level(log_level, app_obj)
 
     if sys.platform not in ("win32", "cygwin", "cli"):  # pragma: no cover
         with suppress(ImportError):
             import uvloop
 
             uvloop.install()  # type: ignore[attr-defined]
@@ -185,18 +177,66 @@
             app_obj.run,
             app_level,
             extra_options,
         )
 
     except ValidationError as e:
         ex = MissingParameter(
-            param=TyperOption(param_decls=[f"--{x['loc'][0]}" for x in e.errors()])
+            param=TyperOption(param_decls=[f"--{x}" for x in e.fields])
         )
 
         try:
             from typer import rich_utils
 
             rich_utils.rich_format_error(ex)
         except ImportError:
             ex.show()
 
         sys.exit(1)
+
+
+@cli.command(
+    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
+)
+def publish(
+    ctx: typer.Context,
+    app: str = typer.Argument(..., help="FastStream app instance, e.g., main:app"),
+    message: str = typer.Argument(..., help="Message to be published"),
+    rpc: bool = typer.Option(False, help="Enable RPC mode and system output"),
+) -> None:
+    """Publish a message using the specified broker in a FastStream application.
+
+    This command publishes a message to a broker configured in a FastStream app instance.
+    It supports various brokers and can handle extra arguments specific to each broker type.
+    These are parsed and passed to the broker's publish method.
+    """
+    app, extra = parse_cli_args(app, *ctx.args)
+    extra["message"] = message
+    extra["rpc"] = rpc
+
+    try:
+        if not app:
+            raise ValueError("App parameter is required.")
+        if not message:
+            raise ValueError("Message parameter is required.")
+
+        _, app_obj = import_from_string(app)
+        if not app_obj.broker:
+            raise ValueError("Broker instance not found in the app.")
+
+        result = anyio.run(publish_message, app_obj.broker, extra)
+
+        if rpc:
+            typer.echo(result)
+
+    except Exception as e:
+        typer.echo(f"Publish error: {e}")
+        sys.exit(1)
+
+
+async def publish_message(broker: BrokerUsecase[Any, Any], extra: AnyDict) -> Any:
+    try:
+        async with broker:
+            return await broker.publish(**extra)  # type: ignore[union-attr]
+    except Exception as e:
+        typer.echo(f"Error when broker was publishing: {e}")
+        sys.exit(1)
```

### Comparing `faststream-0.4.7/faststream/cli/docs/app.py` & `faststream-0.5.0rc0/faststream/cli/docs/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import json
 import sys
 import warnings
 from pathlib import Path
-from typing import Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence
 
 import typer
 
 from faststream.__about__ import INSTALL_WATCHFILES, INSTALL_YAML
 from faststream._compat import json_dumps, model_parse
 from faststream.asyncapi.generate import get_app_schema
 from faststream.asyncapi.schema import Schema
 from faststream.asyncapi.site import serve_app
 from faststream.cli.utils.imports import import_from_string
+from faststream.log import logger as default_logger
+
+if TYPE_CHECKING:
+    from logging import Logger
 
 docs_app = typer.Typer(pretty_exceptions_short=True)
 
 
 @docs_app.command(name="serve")
 def serve(
     app: str = typer.Argument(
@@ -56,15 +60,15 @@
         extra_extensions: Sequence[str] = ()
 
     else:
         module_parent = Path.cwd()
         schema_filepath = module_parent / app
         extra_extensions = (schema_filepath.suffix,)
 
-    if reload is True:
+    if reload:
         try:
             from faststream.cli.supervisors.watchfiles import WatchReloader
 
         except ImportError:
             warnings.warn(INSTALL_WATCHFILES, category=ImportWarning, stacklevel=1)
             _parse_and_serve(app, host, port)
 
@@ -135,17 +139,20 @@
 
 
 def _parse_and_serve(
     app: str,
     host: str = "localhost",
     port: int = 8000,
 ) -> None:
+    logger: Optional["Logger"] = None
+
     if ":" in app:
         _, app_obj = import_from_string(app)
         raw_schema = get_app_schema(app_obj)
+        logger = app_obj.logger
 
     else:
         schema_filepath = Path.cwd() / app
 
         if schema_filepath.suffix == ".json":
             data = schema_filepath.read_bytes()
 
@@ -164,8 +171,8 @@
         else:
             raise ValueError(
                 f"Unknown extension given - {app}; Please provide app in format [python_module:FastStream] or [asyncapi.yaml/.json] - path to your application or documentation"
             )
 
         raw_schema = model_parse(Schema, data)
 
-    serve_app(raw_schema, host, port)
+    serve_app(raw_schema, host, port, logger=logger or default_logger)
```

### Comparing `faststream-0.4.7/faststream/cli/supervisors/basereload.py` & `faststream-0.5.0rc0/faststream/cli/supervisors/basereload.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,23 @@
         Args:
             target: The target callable object
             args: Tuple of arguments to be passed to the target callable
             reload_delay: Optional delay in seconds before reloading the target callable (default is 0.5 seconds)
 
         Returns:
             None
-
         """
         self._target = target
         self._args = args
 
         self.should_exit = threading.Event()
         self.pid = os.getpid()
         self.reload_delay = reload_delay
 
-        set_exit(lambda *_: self.should_exit.set())
+        set_exit(lambda *_: self.should_exit.set(), sync=True)
 
     def run(self) -> None:
         self.startup()
         while not self.should_exit.wait(self.reload_delay):
             if self.should_restart():  # pragma: no branch
                 self.restart()
         self.shutdown()
```

### Comparing `faststream-0.4.7/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.0rc0/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/cli/supervisors/utils.py` & `faststream-0.5.0rc0/faststream/cli/supervisors/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import asyncio
 import multiprocessing
 import os
 import signal
 import sys
+from contextlib import suppress
 from multiprocessing.context import SpawnProcess
 from types import FrameType
 from typing import Any, Callable, Optional
 
 from faststream.types import DecoratedCallableNone
 
 multiprocessing.allow_connection_pickling()
@@ -14,24 +16,35 @@
 
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
 
 
-def set_exit(func: Callable[[int, Optional[FrameType]], Any]) -> None:
+def set_exit(
+    func: Callable[[int, Optional[FrameType]], Any],
+    *,
+    sync: bool = False,
+) -> None:
     """Set exit handler for signals.
 
     Args:
         func: A callable object that takes an integer and an optional frame type as arguments and returns any value.
+        sync: set sync or async signal callback.
+    """
+    if not sync:
+        with suppress(NotImplementedError):
+            loop = asyncio.get_event_loop()
 
-    Returns:
-        None
+            for sig in HANDLED_SIGNALS:
+                loop.add_signal_handler(sig, func, sig, None)
 
-    """
+            return
+
+    # Windows or sync mode
     for sig in HANDLED_SIGNALS:
         signal.signal(sig, func)
 
 
 def get_subprocess(target: DecoratedCallableNone, args: Any) -> SpawnProcess:
     """Spawn a subprocess.
 
@@ -40,15 +53,14 @@
         args: The arguments to be passed to the target function.
 
     Returns:
         The spawned subprocess.
 
     Raises:
         OSError: If there is an error getting the file descriptor of sys.stdin.
-
     """
     stdin_fileno: Optional[int]
     try:
         stdin_fileno = sys.stdin.fileno()
     except OSError:
         stdin_fileno = None
```

### Comparing `faststream-0.4.7/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.0rc0/faststream/cli/supervisors/watchfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from faststream.log import logger
 from faststream.types import DecoratedCallable
 
 
 class ExtendedFilter(watchfiles.PythonFilter):  # type: ignore[misc]
     """A class that extends the `watchfiles.PythonFilter` class."""
 
-    ignore_dirs: Tuple[str, ...]
-
     def __init__(
         self,
         *,
         ignore_paths: Optional[Sequence[Union[str, Path]]] = None,
         extra_extensions: Sequence[str] = (),
     ) -> None:
         """Initialize the class.
@@ -26,15 +24,15 @@
             extra_extensions: Sequence of extra extensions to include.
 
         Returns:
             None
 
         """
         super().__init__(ignore_paths=ignore_paths, extra_extensions=extra_extensions)
-        self.ignore_dirs = (
+        self.ignore_dirs: Sequence[str] = (
             *self.ignore_dirs,
             "venv",
             "env",
             ".github",
             ".mypy_cache",
             ".pytest_cache",
             ".ruff_cache",
```

### Comparing `faststream-0.4.7/faststream/cli/utils/imports.py` & `faststream-0.5.0rc0/faststream/cli/utils/imports.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from typing import Tuple
 
 import typer
 
 from faststream.app import FastStream
+from faststream.exceptions import SetupError
 
 
 def try_import_app(module: Path, app: str) -> FastStream:
     """Tries to import a FastStream app from a module.
 
     Args:
         module: Path to the module containing the app.
@@ -61,15 +62,15 @@
     if spec is None:  # pragma: no cover
         raise FileNotFoundError(module)
 
     mod = module_from_spec(spec)
     loader = spec.loader
 
     if loader is None:  # pragma: no cover
-        raise ValueError(f"{spec} has no loader")
+        raise SetupError(f"{spec} has no loader")
 
     loader.exec_module(mod)
 
     try:
         obj = getattr(mod, app)
     except AttributeError as e:
         raise FileNotFoundError(module) from e
@@ -87,15 +88,15 @@
         Tuple[Path, str]: A tuple containing the path to the module and the name of the application.
 
     Raises:
         ValueError: If the given app is not in the format "module:app_name".
 
     """
     if ":" not in app:
-        raise ValueError(f"`{app}` is not a FastStream")
+        raise SetupError(f"`{app}` is not a FastStream")
 
     module, app_name = app.split(":", 2)
 
     mod_path = Path.cwd()
     for i in module.split("."):
         mod_path = mod_path / i
```

### Comparing `faststream-0.4.7/faststream/cli/utils/logs.py` & `faststream-0.5.0rc0/faststream/cli/utils/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 from collections import defaultdict
 from enum import Enum
-from typing import DefaultDict, Optional, Union
+from typing import TYPE_CHECKING, DefaultDict, Optional, Union
 
 from faststream.app import FastStream
 
+if TYPE_CHECKING:
+    from faststream.types import LoggerProto
+
 
 class LogLevels(str, Enum):
     """A class to represent log levels.
 
     Attributes:
         critical : critical log level
         error : error log level
@@ -61,15 +64,14 @@
 
     Args:
         level (int): The log level to set.
         app (FastStream): The application object.
 
     Returns:
         None
-
     """
     if app.logger and isinstance(app.logger, logging.Logger):
         app.logger.setLevel(level)
 
-    broker_logger: Optional[logging.Logger] = getattr(app.broker, "logger", None)
+    broker_logger: Optional["LoggerProto"] = getattr(app.broker, "logger", None)
     if broker_logger is not None and isinstance(broker_logger, logging.Logger):
         broker_logger.setLevel(level)
```

### Comparing `faststream-0.4.7/faststream/cli/utils/parser.py` & `faststream-0.5.0rc0/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/confluent/annotations.py` & `faststream-0.5.0rc0/faststream/confluent/annotations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
 from faststream.confluent.broker import KafkaBroker as KB
 from faststream.confluent.message import KafkaMessage as KM
-from faststream.confluent.producer import AsyncConfluentFastProducer
+from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
     "KafkaMessage",
```

### Comparing `faststream-0.4.7/faststream/confluent/broker.py` & `faststream-0.5.0rc0/faststream/confluent/broker/broker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,547 +1,525 @@
-from functools import partial, wraps
+import logging
+from asyncio import AbstractEventLoop
+from contextlib import AsyncExitStack
+from inspect import Parameter
 from types import TracebackType
 from typing import (
     Any,
-    AsyncContextManager,
-    Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
-    Sequence,
     Tuple,
     Type,
+    TypeVar,
     Union,
 )
 
-import confluent_kafka
+from confluent_kafka import Message
 from fast_depends.dependencies import Depends
-from typing_extensions import override
+from typing_extensions import Annotated, Doc, override
 
-from faststream.__about__ import __version__
-from faststream.broker.core.asynchronous import BrokerAsyncUsecase, default_filter
-from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
+from faststream.__about__ import SERVICE_NAME
+from faststream.asyncapi import schema as asyncapi
+from faststream.broker.message import StreamMessage, gen_cor_id
 from faststream.broker.types import (
-    AsyncPublisherProtocol,
+    BrokerMiddleware,
     CustomDecoder,
     CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-    WrappedReturn,
 )
-from faststream.broker.wrapper import FakePublisher, HandlerCallWrapper
-from faststream.confluent.asyncapi import Handler, Publisher
-from faststream.confluent.client import AsyncConfluentConsumer, AsyncConfluentProducer
-from faststream.confluent.message import KafkaMessage
-from faststream.confluent.producer import AsyncConfluentFastProducer
+from faststream.confluent.broker.logging import KafkaLoggingBroker
+from faststream.confluent.broker.registrator import KafkaRegistrator
+from faststream.confluent.client import AsyncConfluentProducer, _missing
+from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
+from faststream.confluent.schemas.params import ConsumerConnectionParams
 from faststream.confluent.security import parse_security
-from faststream.confluent.shared.logging import KafkaLoggingMixin
-from faststream.confluent.shared.schemas import ConsumerConnectionParams
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.security import BaseSecurity
-from faststream.utils import context
+from faststream.types import AnyDict, SendableMessage
 from faststream.utils.data import filter_by_dict
 
+Partition = TypeVar("Partition")
+
 
 class KafkaBroker(
-    KafkaLoggingMixin,
-    BrokerAsyncUsecase[confluent_kafka.Message, ConsumerConnectionParams],
+    KafkaRegistrator,
+    KafkaLoggingBroker,
 ):
-    """KafkaBroker is a class for managing Kafka message consumption and publishing.
-
-    It extends BrokerAsyncUsecase to handle asynchronous operations.
-
-    Args:
-        bootstrap_servers (Union[str, Iterable[str]]): Kafka bootstrap server(s).
-        protocol (str): The protocol used (default is "kafka").
-        protocol_version (str): The Kafka protocol version (default is "auto").
-        client_id (str): The client ID for the Kafka client.
-        **kwargs: Additional keyword arguments.
-
-    Attributes:
-        handlers (Dict[str, Handler]): A dictionary of message handlers.
-        _publishers (Dict[str, Publisher]): A dictionary of message publishers.
-        _producer (Optional[AsyncConfluentFastProducer]): An optional Kafka producer.
-
-    Methods:
-        connect(*args, **kwargs): Establishes a connection to Kafka.
-        start(): Starts the KafkaBroker and message handlers.
-        publish(*args, **kwargs): Publishes a message to Kafka.
-    """
-
     url: List[str]
-    handlers: Dict[str, Handler]
-    _publishers: Dict[str, Publisher]
     _producer: Optional[AsyncConfluentFastProducer]
 
     def __init__(
         self,
-        bootstrap_servers: Union[str, Iterable[str]] = "localhost",
+        bootstrap_servers: Annotated[
+            Union[str, Iterable[str]],
+            Doc(
+                """
+            A `host[:port]` string (or list of `host[:port]` strings) that the consumer should contact to bootstrap
+            initial cluster metadata.
+
+            This does not have to be the full node list.
+            It just needs to have at least one broker that will respond to a
+            Metadata API Request. Default port is 9092.
+            """
+            ),
+        ] = "localhost",
         *,
-        protocol: Optional[str] = None,
-        protocol_version: str = "auto",
-        client_id: str = "faststream-" + __version__,
-        security: Optional[BaseSecurity] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize a KafkaBroker instance.
+        # both
+        request_timeout_ms: Annotated[
+            int,
+            Doc("Client request timeout in milliseconds."),
+        ] = 40 * 1000,
+        retry_backoff_ms: Annotated[
+            int,
+            Doc(" Milliseconds to backoff when retrying on errors."),
+        ] = 100,
+        metadata_max_age_ms: Annotated[
+            int,
+            Doc(
+                """
+            The period of time in milliseconds after
+            which we force a refresh of metadata even if we haven't seen any
+            partition leadership changes to proactively discover any new
+            brokers or partitions.
+            """
+            ),
+        ] = 5 * 60 * 1000,
+        connections_max_idle_ms: Annotated[
+            int,
+            Doc(
+                """
+             Close idle connections after the number
+            of milliseconds specified by this config. Specifying `None` will
+            disable idle checks.
+            """
+            ),
+        ] = 9 * 60 * 1000,
+        sasl_kerberos_service_name: str = "kafka",
+        sasl_kerberos_domain_name: Optional[str] = None,
+        sasl_oauth_token_provider: Annotated[
+            Optional[str], Doc("OAuthBearer token provider.")
+        ] = None,
+        loop: Optional[AbstractEventLoop] = None,
+        client_id: Annotated[
+            Optional[str],
+            Doc(
+                """
+            A name for this client. This string is passed in
+            each request to servers and can be used to identify specific
+            server-side log entries that correspond to this client. Also
+            submitted to :class:`~.consumer.group_coordinator.GroupCoordinator`
+            for logging with respect to consumer group administration.
+            """
+            ),
+        ] = SERVICE_NAME,
+        # publisher args
+        acks: Annotated[
+            Union[Literal[0, 1, -1, "all"], object],
+            Doc(
+                """
+            One of ``0``, ``1``, ``all``. The number of acknowledgments
+            the producer requires the leader to have received before considering a
+            request complete. This controls the durability of records that are
+            sent. The following settings are common:
+
+            * ``0``: Producer will not wait for any acknowledgment from the server
+              at all. The message will immediately be added to the socket
+              buffer and considered sent. No guarantee can be made that the
+              server has received the record in this case, and the retries
+              configuration will not take effect (as the client won't
+              generally know of any failures). The offset given back for each
+              record will always be set to -1.
+            * ``1``: The broker leader will write the record to its local log but
+              will respond without awaiting full acknowledgement from all
+              followers. In this case should the leader fail immediately
+              after acknowledging the record but before the followers have
+              replicated it then the record will be lost.
+            * ``all``: The broker leader will wait for the full set of in-sync
+              replicas to acknowledge the record. This guarantees that the
+              record will not be lost as long as at least one in-sync replica
+              remains alive. This is the strongest available guarantee.
 
-        Args:
-            bootstrap_servers (Union[str, Iterable[str]]): Kafka bootstrap server(s).
-            protocol (str): The protocol used (default is "kafka").
-            protocol_version (str): The Kafka protocol version (default is "auto").
-            client_id (str): The client ID for the Kafka client.
-            security (Optional[BaseSecurity]): Security protocol to use in communication with the broker (default is None).
-            **kwargs: Additional keyword arguments.
-        """
+            If unset, defaults to ``acks=1``. If `enable_idempotence` is
+            :data:`True` defaults to ``acks=all``.
+            """
+            ),
+        ] = _missing,
+        key_serializer: Annotated[
+            Optional[Callable[[Any], bytes]],
+            Doc("Used to convert user-supplied keys to bytes."),
+        ] = None,
+        value_serializer: Annotated[
+            Optional[Callable[[Any], bytes]],
+            Doc("used to convert user-supplied message values to bytes."),
+        ] = None,
+        compression_type: Annotated[
+            Optional[Literal["gzip", "snappy", "lz4", "zstd"]],
+            Doc(
+                """
+            The compression type for all data generated bythe producer.
+            Compression is of full batches of data, so the efficacy of batching
+            will also impact the compression ratio (more batching means better
+            compression).
+            """
+            ),
+        ] = None,
+        max_batch_size: Annotated[
+            int,
+            Doc(
+                """
+            Maximum size of buffered data per partition.
+            After this amount `send` coroutine will block until batch is drained.
+            """
+            ),
+        ] = 16 * 1024,
+        partitioner: Annotated[
+            Union[
+                str,
+                Callable[
+                    [bytes, List[Partition], List[Partition]],
+                    Partition,
+                ],
+            ],
+            Doc(
+                """
+            Callable used to determine which partition
+            each message is assigned to. Called (after key serialization):
+            ``partitioner(key_bytes, all_partitions, available_partitions)``.
+            The default partitioner implementation hashes each non-None key
+            using the same murmur2 algorithm as the Java client so that
+            messages with the same key are assigned to the same partition.
+            When a key is :data:`None`, the message is delivered to a random partition
+            (filtered to partitions with available leaders only, if possible).
+            """
+            ),
+        ] = "consistent_random",
+        max_request_size: Annotated[
+            int,
+            Doc(
+                """
+            The maximum size of a request. This is also
+            effectively a cap on the maximum record size. Note that the server
+            has its own cap on record size which may be different from this.
+            This setting will limit the number of record batches the producer
+            will send in a single request to avoid sending huge requests.
+            """
+            ),
+        ] = 1024 * 1024,
+        linger_ms: Annotated[
+            int,
+            Doc(
+                """
+            The producer groups together any records that arrive
+            in between request transmissions into a single batched request.
+            Normally this occurs only under load when records arrive faster
+            than they can be sent out. However in some circumstances the client
+            may want to reduce the number of requests even under moderate load.
+            This setting accomplishes this by adding a small amount of
+            artificial delay; that is, if first request is processed faster,
+            than `linger_ms`, producer will wait ``linger_ms - process_time``.
+            """
+            ),
+        ] = 0,
+        send_backoff_ms: int = 100,
+        enable_idempotence: Annotated[
+            bool,
+            Doc(
+                """
+            When set to `True`, the producer will
+            ensure that exactly one copy of each message is written in the
+            stream. If `False`, producer retries due to broker failures,
+            etc., may write duplicates of the retried message in the stream.
+            Note that enabling idempotence acks to set to ``all``. If it is not
+            explicitly set by the user it will be chosen.
+            """
+            ),
+        ] = False,
+        transactional_id: Optional[str] = None,
+        transaction_timeout_ms: int = 60 * 1000,
+        # broker base args
+        graceful_timeout: Annotated[
+            Optional[float],
+            Doc(
+                "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
+            ),
+        ] = 15.0,
+        decoder: Annotated[
+            Optional[
+                Union[
+                    CustomDecoder[StreamMessage[Message]],
+                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
+                ]
+            ],
+            Doc("Custom decoder object."),
+        ] = None,
+        parser: Annotated[
+            Optional[Union[CustomParser[Message], CustomParser[Tuple[Message, ...]]]],
+            Doc("Custom parser object."),
+        ] = None,
+        dependencies: Annotated[
+            Iterable[Depends],
+            Doc("Dependencies to apply to all broker subscribers."),
+        ] = (),
+        middlewares: Annotated[
+            Iterable[
+                Union[
+                    BrokerMiddleware[Message],
+                    BrokerMiddleware[Tuple[Message, ...]],
+                ]
+            ],
+            Doc("Middlewares to apply to all broker publishers/subscribers."),
+        ] = (),
+        # AsyncAPI args
+        security: Annotated[
+            Optional["BaseSecurity"],
+            Doc(
+                "Security options to connect broker and generate AsyncAPI server security information."
+            ),
+        ] = None,
+        asyncapi_url: Annotated[
+            Union[str, Iterable[str], None],
+            Doc("AsyncAPI hardcoded server addresses. Use `servers` if not specified."),
+        ] = None,
+        protocol: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server protocol."),
+        ] = None,
+        protocol_version: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server protocol version."),
+        ] = "auto",
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI server description."),
+        ] = None,
+        tags: Annotated[
+            Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
+            Doc("AsyncAPI server tags."),
+        ] = None,
+        # logging args
+        logger: Annotated[
+            Union[logging.Logger, None, object],
+            Doc("User specified logger to pass into Context and log service messages."),
+        ] = Parameter.empty,
+        log_level: Annotated[
+            int,
+            Doc("Service messages log level."),
+        ] = logging.INFO,
+        log_fmt: Annotated[
+            Optional[str],
+            Doc("Default logger log format."),
+        ] = None,
+        # FastDepends args
+        apply_types: Annotated[
+            bool,
+            Doc("Whether to use FastDepends or not."),
+        ] = True,
+        validate: Annotated[
+            bool,
+            Doc("Whether to cast types using Pydantic validation."),
+        ] = True,
+        _get_dependant: Annotated[
+            Optional[Callable[..., Any]],
+            Doc("Custom library dependant generator callback."),
+        ] = None,
+    ) -> None:
         if protocol is None:
             if security is not None and security.use_ssl:
                 protocol = "kafka-secure"
             else:
                 protocol = "kafka"
 
-        super().__init__(
-            url=[bootstrap_servers]
+        servers = (
+            [bootstrap_servers]
             if isinstance(bootstrap_servers, str)
-            else list(bootstrap_servers),
+            else list(bootstrap_servers)
+        )
+
+        if asyncapi_url is not None:
+            if isinstance(asyncapi_url, str):
+                asyncapi_url = [asyncapi_url]
+            else:
+                asyncapi_url = list(asyncapi_url)
+        else:
+            asyncapi_url = servers
+
+        super().__init__(
+            bootstrap_servers=servers,
+            # both args
+            client_id=client_id,
+            api_version=protocol_version,
+            request_timeout_ms=request_timeout_ms,
+            retry_backoff_ms=retry_backoff_ms,
+            metadata_max_age_ms=metadata_max_age_ms,
+            connections_max_idle_ms=connections_max_idle_ms,
+            sasl_kerberos_service_name=sasl_kerberos_service_name,
+            sasl_kerberos_domain_name=sasl_kerberos_domain_name,
+            sasl_oauth_token_provider=sasl_oauth_token_provider,
+            loop=loop,
+            # publisher args
+            acks=acks,
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+            compression_type=compression_type,
+            max_batch_size=max_batch_size,
+            partitioner=partitioner,
+            max_request_size=max_request_size,
+            linger_ms=linger_ms,
+            send_backoff_ms=send_backoff_ms,
+            enable_idempotence=enable_idempotence,
+            transactional_id=transactional_id,
+            transaction_timeout_ms=transaction_timeout_ms,
+            # Basic args
+            graceful_timeout=graceful_timeout,
+            dependencies=dependencies,
+            decoder=decoder,
+            parser=parser,
+            middlewares=middlewares,
+            # AsyncAPI args
+            description=description,
+            asyncapi_url=asyncapi_url,
             protocol=protocol,
             protocol_version=protocol_version,
             security=security,
-            **kwargs,
-            client_id=client_id,
-            bootstrap_servers=bootstrap_servers,
+            tags=tags,
+            # Logging args
+            logger=logger,
+            log_level=log_level,
+            log_fmt=log_fmt,
+            # FastDepends args
+            _get_dependant=_get_dependant,
+            apply_types=apply_types,
+            validate=validate,
         )
         self.client_id = client_id
         self._producer = None
 
     async def _close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
+        exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        """Close the KafkaBroker, stopping the producer and cleaning up resources.
-
-        Args:
-            exc_type (Optional[Type[BaseException]]): The exception type.
-            exc_val (Optional[BaseException]]): The exception value.
-            exec_tb (Optional[TracebackType]]): The traceback.
-        """
         if self._producer is not None:  # pragma: no branch
             await self._producer.stop()
             self._producer = None
 
-        await super()._close(exc_type, exc_val, exec_tb)
+        await super()._close(exc_type, exc_val, exc_tb)
 
     async def connect(
         self,
-        *args: Any,
+        bootstrap_servers: Annotated[
+            Union[str, Iterable[str], object],
+            Doc("Kafka addresses to connect."),
+        ] = Parameter.empty,
         **kwargs: Any,
     ) -> ConsumerConnectionParams:
-        """Establishes a connection to Kafka and returns connection parameters.
+        if bootstrap_servers is not Parameter.empty:
+            kwargs["bootstrap_servers"] = bootstrap_servers
 
-        Args:
-            *args: Additional arguments.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            ConsumerConnectionParams: The connection parameters.
-        """
-        connection = await super().connect(*args, **kwargs)
-        for p in self._publishers.values():
-            p._producer = self._producer
-        return connection
+        return await super().connect(**kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
         self,
         *,
         client_id: str,
         **kwargs: Any,
     ) -> ConsumerConnectionParams:
-        """Connects to Kafka, initializes the producer, and returns connection parameters.
-
-        Args:
-            client_id (str): The client ID.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            ConsumerConnectionParams: The connection parameters.
-        """
         security_params = parse_security(self.security)
         producer = AsyncConfluentProducer(
-            **kwargs, **security_params, client_id=client_id
+            **kwargs,
+            **security_params,
+            client_id=client_id,
         )
-        await producer.start()
         self._producer = AsyncConfluentFastProducer(
             producer=producer,
         )
         return filter_by_dict(ConsumerConnectionParams, {**kwargs, **security_params})
 
     async def start(self) -> None:
-        """Start the KafkaBroker and message handlers."""
-        context.set_global(
-            "default_log_context",
-            self._get_log_context(None, ""),
-        )
-
         await super().start()
 
-        for handler in self.handlers.values():
-            c = self._get_log_context(None, handler.topics, handler.group_id)
-            self._log(f"`{handler.call_name}` waiting for messages", extra=c)
-            await handler.start(**(self._connection or {}))
-
-    def _process_message(
-        self,
-        func: Callable[[KafkaMessage], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[
-        [KafkaMessage],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ]:
-        """Wrap a message processing function with a watcher and publisher.
-
-        Args:
-            func (Callable[[KafkaMessage], Awaitable[T_HandlerReturn]]): The message processing function.
-            watcher (BaseWatcher): The message watcher.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            Callable[[KafkaMessage], Awaitable[WrappedReturn[T_HandlerReturn]]]: The wrapped message processing function.
-        """
-
-        @wraps(func)
-        async def process_wrapper(
-            message: KafkaMessage,
-        ) -> WrappedReturn[T_HandlerReturn]:
-            """Asynchronously process a Kafka message and wrap the return value.
-
-            Args:
-                message (KafkaMessage): The Kafka message to process.
-
-            Returns:
-                WrappedReturn[T_HandlerReturn]: The wrapped return value.
-
-            Raises:
-                AssertionError: If the code reaches an unreachable point.
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            async with watcher(message):
-                r = await func(message)
-
-                pub_response: Optional[AsyncPublisherProtocol]
-                if message.reply_to:
-                    pub_response = FakePublisher(
-                        partial(self.publish, topic=message.reply_to)
-                    )
-                else:
-                    pub_response = None
-
-                return r, pub_response
-
-        return process_wrapper
-
-    @override
-    def subscriber(  # type: ignore[override]
-        self,
-        *topics: str,
-        group_id: Optional[str] = None,
-        key_deserializer: Optional[Callable[[bytes], Any]] = None,
-        value_deserializer: Optional[Callable[[bytes], Any]] = None,
-        fetch_max_wait_ms: int = 500,
-        fetch_max_bytes: int = 52428800,
-        fetch_min_bytes: int = 1,
-        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
-        auto_offset_reset: Literal[
-            "latest",
-            "earliest",
-            "none",
-        ] = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5000,
-        check_crcs: bool = True,
-        partition_assignment_strategy: Sequence[str] = ("roundrobin",),
-        max_poll_interval_ms: int = 300000,
-        rebalance_timeout_ms: Optional[int] = None,
-        session_timeout_ms: int = 10000,
-        heartbeat_interval_ms: int = 3000,
-        consumer_timeout_ms: int = 200,
-        max_poll_records: Optional[int] = None,
-        exclude_internal_topics: bool = True,
-        isolation_level: Literal[
-            "read_uncommitted",
-            "read_committed",
-        ] = "read_uncommitted",
-        # broker arguments
-        dependencies: Sequence[Depends] = (),
-        parser: Optional[
-            Union[
-                CustomParser[confluent_kafka.Message, KafkaMessage],
-                CustomParser[Tuple[confluent_kafka.Message, ...], KafkaMessage],
-            ]
-        ] = None,
-        decoder: Optional[CustomDecoder] = None,
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [confluent_kafka.Message],
-                    BaseMiddleware,
-                ]
-            ]
-        ] = None,
-        filter: Union[
-            Filter[KafkaMessage],
-            Filter[StreamMessage[Tuple[confluent_kafka.Message, ...]]],
-        ] = default_filter,
-        batch: bool = False,
-        max_records: Optional[int] = None,
-        batch_timeout_ms: int = 200,
-        no_ack: bool = False,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
-        **original_kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        Union[
-            HandlerCallWrapper[
-                confluent_kafka.Message, P_HandlerParams, T_HandlerReturn
-            ],
-            HandlerCallWrapper[
-                Tuple[confluent_kafka.Message, ...], P_HandlerParams, T_HandlerReturn
-            ],
-        ],
-    ]:
-        """Create a message subscriber for the specified topics.
-
-        Args:
-            *topics (str): The topics to subscribe to.
-            group_id (Optional[str]): The Kafka consumer group ID.
-            key_deserializer (Optional[Callable[[bytes], Any]]): Key deserializer function.
-            value_deserializer (Optional[Callable[[bytes], Any]]): Value deserializer function.
-            fetch_max_wait_ms (int): The maximum time to wait for data.
-            fetch_max_bytes (int): The maximum number of bytes to fetch.
-            fetch_min_bytes (int): The minimum number of bytes to fetch.
-            max_partition_fetch_bytes (int): The maximum bytes to fetch for a partition.
-            auto_offset_reset (Literal["latest", "earliest", "none"]): Auto offset reset policy.
-            auto_commit (bool): Whether to enable auto-commit.
-            auto_commit_interval_ms (int): Auto-commit interval in milliseconds.
-            check_crcs (bool): Whether to check CRCs.
-            partition_assignment_strategy (Sequence[AbstractPartitionAssignor]): Partition assignment strategy.
-            max_poll_interval_ms (int): Maximum poll interval in milliseconds.
-            rebalance_timeout_ms (Optional[int]): Rebalance timeout in milliseconds.
-            session_timeout_ms (int): Session timeout in milliseconds.
-            heartbeat_interval_ms (int): Heartbeat interval in milliseconds.
-            consumer_timeout_ms (int): Consumer timeout in milliseconds.
-            max_poll_records (Optional[int]): Maximum number of records to poll.
-            exclude_internal_topics (bool): Whether to exclude internal topics.
-            isolation_level (Literal["read_uncommitted", "read_committed"]): Isolation level.
-            dependencies (Sequence[Depends]): Additional dependencies for message handling.
-            parser (Optional[Union[CustomParser[confluent_kafka.Message], CustomParser[Tuple[confluent_kafka.Message, ...]]]]): Message parser.
-            decoder (Optional[CustomDecoder]): Message decoder.
-            middlewares (Optional[Sequence[Callable[[confluent_kafka.Message], BaseMiddleware]]]): Message middlewares.
-            filter (Union[Filter[KafkaMessage], Filter[StreamMessage[Tuple[confluent_kafka.Message, ...]]]]): Message filter.
-            batch (bool): Whether to process messages in batches.
-            max_records (Optional[int]): Maximum number of records to process in each batch.
-            batch_timeout_ms (int): Batch timeout in milliseconds.
-            no_ack (bool): Whether not to ack/nack/reject messages.
-            title (Optional[str]): AsyncAPI title.
-            description (Optional[str]): AsyncAPI description.
-            include_in_schema (bool): Whether to include the handler in the AsyncAPI schema.
-            **original_kwargs: Additional keyword arguments.
-
-        Returns:
-            Callable: A decorator that wraps a message handler function.
-        """
-        super().subscriber()
-
-        self._setup_log_context(topics, group_id)
-
-        if not auto_commit and not group_id:
-            raise ValueError("You should install `group_id` with manual commit mode")
-
-        key = Handler.get_routing_hash(topics, group_id)
-        builder = partial(
-            AsyncConfluentConsumer,
-            key_deserializer=key_deserializer,
-            value_deserializer=value_deserializer,
-            fetch_max_wait_ms=fetch_max_wait_ms,
-            fetch_max_bytes=fetch_max_bytes,
-            fetch_min_bytes=fetch_min_bytes,
-            max_partition_fetch_bytes=max_partition_fetch_bytes,
-            auto_offset_reset=auto_offset_reset,
-            enable_auto_commit=auto_commit,
-            auto_commit_interval_ms=auto_commit_interval_ms,
-            check_crcs=check_crcs,
-            partition_assignment_strategy=partition_assignment_strategy,
-            max_poll_interval_ms=max_poll_interval_ms,
-            rebalance_timeout_ms=rebalance_timeout_ms,
-            session_timeout_ms=session_timeout_ms,
-            heartbeat_interval_ms=heartbeat_interval_ms,
-            consumer_timeout_ms=consumer_timeout_ms,
-            max_poll_records=max_poll_records,
-            exclude_internal_topics=exclude_internal_topics,
-            isolation_level=isolation_level,
-        )
-        handler = self.handlers.get(
-            key,
-            Handler(
-                *topics,
-                log_context_builder=partial(
-                    self._get_log_context,
-                    topics=topics,
-                    group_id=group_id,
-                ),
-                is_manual=not auto_commit,
-                group_id=group_id,
-                client_id=self.client_id,
-                builder=builder,
-                description=description,
-                title=title,
-                batch=batch,
-                batch_timeout_ms=batch_timeout_ms,
-                max_records=max_records,
-                include_in_schema=include_in_schema,
-            ),
-        )
-
-        self.handlers[key] = handler
-
-        def consumer_wrapper(
-            func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[
-            confluent_kafka.Message, P_HandlerParams, T_HandlerReturn
-        ]:
-            """A wrapper function for a consumer handler.
-
-            Args:
-                func : The consumer handler function to be wrapped.
-
-            Returns:
-                The wrapped handler call.
-
-            Raises:
-                NotImplementedError: If silent animals are not supported.
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            handler_call, dependant = self._wrap_handler(
-                func=func,
-                extra_dependencies=dependencies,
-                no_ack=no_ack,
-                **original_kwargs,
+        for handler in self._subscribers.values():
+            self._log(
+                f"`{handler.call_name}` waiting for messages",
+                extra=handler.get_log_context(None),
             )
+            await handler.start()
 
-            handler.add_call(
-                handler=handler_call,
-                filter=filter,
-                middlewares=middlewares,
-                parser=parser or self._global_parser,
-                decoder=decoder or self._global_decoder,
-                dependant=dependant,
-            )
-
-            return handler_call
-
-        return consumer_wrapper
+    @property
+    def _subscriber_setup_extra(self) -> AnyDict:
+        return {"client_id": self.client_id, "connection_data": self._connection or {}}
 
     @override
-    def publisher(  # type: ignore[override]
+    async def publish(  # type: ignore[override]
         self,
+        message: SendableMessage,
         topic: str,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
+        correlation_id: Optional[str] = None,
+        *,
         reply_to: str = "",
-        batch: bool = False,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        schema: Optional[Any] = None,
-        include_in_schema: bool = True,
-    ) -> Publisher:
-        """Create a message publisher for the specified topic.
-
-        Args:
-            topic (str): The topic to publish messages to.
-            key (Optional[bytes]): Message key.
-            partition (Optional[int]): Partition to send the message to.
-            timestamp_ms (Optional[int]): Message timestamp in milliseconds.
-            headers (Optional[Dict[str, str]]): Message headers.
-            reply_to (str): The topic to which responses should be sent.
-            batch (bool): Whether to publish messages in batches.
-            title (Optional[str]): AsyncAPI title.
-            description (Optional[str]): AsyncAPI description.
-            schema (Optional[Any]): AsyncAPI schema.
-            include_in_schema (bool): Whether to include the publisher in the AsyncAPI schema.
-
-        Returns:
-            Publisher: A message publisher.
-        """
-        publisher = self._publishers.get(
-            topic,
-            Publisher(
-                topic=topic,
-                client_id=self.client_id,
-                key=key,
-                batch=batch,
-                partition=partition,
-                timestamp_ms=timestamp_ms,
-                headers=headers,
-                reply_to=reply_to,
-                title=title,
-                _description=description,
-                _schema=schema,
-                include_in_schema=include_in_schema,
-            ),
-        )
-        super().publisher(topic, publisher)
-        if self._producer is not None:
-            publisher._producer = self._producer
-        return publisher
-
-    @override
-    async def publish(  # type: ignore[override]
-        self,
-        *args: Any,
+        # extra options to be compatible with test client
         **kwargs: Any,
-    ) -> None:
-        """Publish a message to Kafka.
+    ) -> Optional[Any]:
+        correlation_id = correlation_id or gen_cor_id()
 
-        Args:
-            *args: Positional arguments for message publishing.
-            **kwargs: Keyword arguments for message publishing.
-
-        Raises:
-            RuntimeError: If KafkaBroker is not started yet.
-        """
-        assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        return await self._producer.publish(*args, **kwargs)
+        return await super().publish(
+            message,
+            producer=self._producer,
+            topic=topic,
+            key=key,
+            partition=partition,
+            timestamp_ms=timestamp_ms,
+            headers=headers,
+            correlation_id=correlation_id,
+            reply_to=reply_to,
+            **kwargs,
+        )
 
     async def publish_batch(
         self,
-        *args: Any,
-        **kwargs: Any,
+        *msgs: SendableMessage,
+        topic: str,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[Dict[str, str]] = None,
+        reply_to: str = "",
+        correlation_id: Optional[str] = None,
     ) -> None:
-        """Publish a batch of messages to Kafka.
-
-        Args:
-            *args: Positional arguments for message publishing.
-            **kwargs: Keyword arguments for message publishing.
-
-        Raises:
-            RuntimeError: If KafkaBroker is not started yet.
-        """
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        await self._producer.publish_batch(*args, **kwargs)
+
+        correlation_id = correlation_id or gen_cor_id()
+
+        async with AsyncExitStack() as stack:
+            wrapped_messages = [
+                await stack.enter_async_context(
+                    middleware(None).publish_scope(
+                        msg,
+                        topic=topic,
+                        partition=partition,
+                        timestamp_ms=timestamp_ms,
+                        headers=headers,
+                        reply_to=reply_to,
+                        correlation_id=correlation_id,
+                    )
+                )
+                for msg in msgs
+                for middleware in self._middlewares
+            ] or msgs
+
+            await self._producer.publish_batch(
+                *wrapped_messages,
+                topic=topic,
+                partition=partition,
+                timestamp_ms=timestamp_ms,
+                headers=headers,
+                reply_to=reply_to,
+                correlation_id=correlation_id,
+            )
```

### Comparing `faststream-0.4.7/faststream/confluent/handler.py` & `faststream-0.5.0rc0/faststream/confluent/subscriber/usecase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,330 @@
 import asyncio
-from itertools import chain
-from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
+from abc import ABC, abstractmethod
+from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Tuple
 
 import anyio
 from confluent_kafka import KafkaException, Message
-from fast_depends.core import CallModel
-from typing_extensions import Unpack, override
+from fast_depends.dependencies import Depends
+from typing_extensions import override
 
-from faststream.__about__ import __version__
-from faststream.broker.handler import AsyncHandler
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.parsers import resolve_custom_func
+from faststream.broker.publisher.fake import FakePublisher
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.subscriber.usecase import SubscriberUsecase
 from faststream.broker.types import (
+    AsyncDecoder,
+    AsyncParser,
+    BrokerMiddleware,
     CustomDecoder,
     CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
+    MsgType,
 )
-from faststream.broker.wrapper import HandlerCallWrapper
 from faststream.confluent.client import AsyncConfluentConsumer
-from faststream.confluent.message import KafkaMessage
 from faststream.confluent.parser import AsyncConfluentParser
-from faststream.confluent.shared.schemas import ConsumerConnectionParams
+from faststream.confluent.schemas.params import ConsumerConnectionParams
+from faststream.types import AnyDict, LoggerProto
 
 
-class LogicHandler(AsyncHandler[Message]):
-    """A class to handle logic for consuming messages from Kafka.
-
-    Attributes:
-        topics : sequence of strings representing the topics to consume from
-        group_id : optional string representing the consumer group ID
-        consumer : optional AsyncConfluentConsumer object representing the Kafka consumer
-        task : optional asyncio.Task object representing the task for consuming messages
-        batch : boolean indicating whether to consume messages in batches
-
-    Methods:
-        __init__ : constructor method for the LogicHandler class
-        start : method to start consuming messages from Kafka
-        close : method to close the Kafka consumer and cancel the consuming task
-        add_call : method to add a handler call for processing consumed messages
-        _consume : method to consume messages from Kafka and call the appropriate handler
-
-    """
+class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
+    """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
-    group_id: Optional[str] = None
+    group_id: Optional[str]
 
-    consumer: Optional[AsyncConfluentConsumer] = None
-    task: Optional["asyncio.Task[Any]"] = None
-    batch: bool = False
+    consumer: Optional[AsyncConfluentConsumer]
+    task: Optional["asyncio.Task[None]"]
+    client_id: Optional[str]
+    batch: bool
 
-    @override
     def __init__(
         self,
         *topics: str,
-        log_context_builder: Callable[[StreamMessage[Any]], Dict[str, str]],
-        graceful_timeout: Optional[float] = None,
         # Kafka information
-        group_id: Optional[str] = None,
-        client_id: str = "faststream-" + __version__,
+        group_id: Optional[str],
         builder: Callable[..., AsyncConfluentConsumer],
-        is_manual: bool = False,
-        batch: bool = False,
-        batch_timeout_ms: int = 200,
-        max_records: Optional[int] = None,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
+        is_manual: bool,
+        # Subscriber args
+        default_parser: AsyncParser[MsgType],
+        default_decoder: AsyncDecoder[StreamMessage[MsgType]],
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Initialize a Kafka consumer for the specified topics.
-
-        Args:
-            *topics: Variable length argument list of topics to consume from.
-            log_context_builder: Callable that builds a log context from a message.
-            graceful_timeout: Optional timeout in seconds for graceful shutdown.
-            group_id: Optional group ID for the consumer.
-            client_id: Client ID for the consumer.
-            builder: Callable that constructs an AsyncConfluentConsumer instance.
-            is_manual: Flag indicating whether to manually commit offsets.
-            batch: Flag indicating whether to consume messages in batches.
-            batch_timeout_ms: Timeout in milliseconds for batch consumption.
-            max_records: Maximum number of records to consume in a batch.
-            title: Optional title for the consumer.
-            description: Optional description for the consumer.
-            include_in_schema: Flag indicating whether to include the consumer in the schema.
-
-
-        Raises:
-            ValueError: If the topics are not specified.
-
-        """
         super().__init__(
-            log_context_builder=log_context_builder,
-            description=description,
-            title=title,
+            default_parser=default_parser,
+            default_decoder=default_decoder,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
             include_in_schema=include_in_schema,
-            graceful_timeout=graceful_timeout,
         )
 
         self.group_id = group_id
-        self.client_id = client_id
         self.topics = topics
-
-        self.batch = batch
-        self.batch_timeout_ms = batch_timeout_ms
-        self.max_records = max_records
         self.is_manual = is_manual
-
         self.builder = builder
-        self.task = None
         self.consumer = None
+        self.task = None
+
+        # Setup it later
+        self.client_id = ""
+        self.__connection_data = ConsumerConnectionParams()
 
     @override
-    async def start(  # type: ignore[override]
+    def setup(  # type: ignore[override]
         self,
-        **consumer_kwargs: Unpack[ConsumerConnectionParams],
+        *,
+        client_id: Optional[str],
+        connection_data: ConsumerConnectionParams,
+        # basic args
+        logger: Optional[LoggerProto],
+        producer: Optional[ProducerProto],
+        graceful_timeout: Optional[float],
+        extra_context: Optional[AnyDict],
+        # broker options
+        broker_parser: Optional["CustomParser[MsgType]"],
+        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        # dependant args
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
-        """Start the consumer.
-
-        Args:
-            **consumer_kwargs: Additional keyword arguments to pass to the consumer.
+        self.client_id = client_id
+        self.__connection_data = connection_data
 
-        Returns:
-            None
+        super().setup(
+            logger=logger,
+            producer=producer,
+            graceful_timeout=graceful_timeout,
+            extra_context=extra_context,
+            broker_parser=broker_parser,
+            broker_decoder=broker_decoder,
+            apply_types=apply_types,
+            is_validate=is_validate,
+            _get_dependant=_get_dependant,
+        )
 
-        """
+    @override
+    async def start(self) -> None:
+        """Start the consumer."""
         self.consumer = consumer = self.builder(
             *self.topics,
             group_id=self.group_id,
             client_id=self.client_id,
-            **consumer_kwargs,
+            **self.__connection_data,
         )
         await consumer.start()
-        self.task = asyncio.create_task(self._consume())
+
         await super().start()
 
+        self.task = asyncio.create_task(self._consume())
+
     async def close(self) -> None:
         await super().close()
 
         if self.consumer is not None:
             await self.consumer.stop()
             self.consumer = None
 
-        if self.task is not None:
+        if self.task is not None and not self.task.done():
             self.task.cancel()
-            self.task = None
 
-    def add_call(
-        self,
-        *,
-        handler: HandlerCallWrapper[Message, P_HandlerParams, T_HandlerReturn],
-        dependant: CallModel[P_HandlerParams, T_HandlerReturn],
-        parser: CustomParser[Union[Message, Tuple[Message, ...]], KafkaMessage],
-        decoder: Optional[CustomDecoder[KafkaMessage]],
-        filter: Union[
-            Filter[KafkaMessage],
-            Filter[StreamMessage[Tuple[Message, ...]]],
-        ],
-        middlewares: Optional[Sequence[Callable[[Message], BaseMiddleware]]],
-    ) -> None:
-        """Adds a call to the handler.
+        self.task = None
 
-        Args:
-            handler: The handler function to be called.
-            dependant: The dependant model.
-            parser: Optional custom parser for parsing the input.
-            decoder: Optional custom decoder for decoding the input.
-            filter: The filter for filtering the input.
-            middlewares: Optional sequence of middlewares to be applied.
-
-        Returns:
-            None
-
-        """
-        parser_ = resolve_custom_func(  # type: ignore[type-var]
-            parser,  # type: ignore[arg-type]
-            (
-                AsyncConfluentParser.parse_message_batch  # type: ignore[arg-type]
-                if self.batch
-                else AsyncConfluentParser.parse_message
-            ),
-        )
-        decoder_ = resolve_custom_func(
-            decoder,  # type: ignore[arg-type]
-            (
-                AsyncConfluentParser.decode_message_batch  # type: ignore[arg-type]
-                if self.batch
-                else AsyncConfluentParser.decode_message
+    def _make_response_publisher(
+        self, message: "StreamMessage[Any]"
+    ) -> Sequence[FakePublisher]:
+        if not message.reply_to or self._producer is None:
+            return ()
+
+        return (
+            FakePublisher(
+                self._producer.publish,
+                publish_kwargs={
+                    "topic": message.reply_to,
+                },
             ),
         )
-        super().add_call(
-            handler=handler,
-            parser=parser_,
-            decoder=decoder_,
-            filter=filter,  # type: ignore[arg-type]
-            dependant=dependant,
-            middlewares=middlewares,
-        )
+
+    @abstractmethod
+    async def get_msg(self) -> Optional[MsgType]:
+        raise NotImplementedError()
 
     async def _consume(self) -> None:
         assert self.consumer, "You need to start handler first"  # nosec B101
 
         connected = True
         while self.running:
             try:
-                if self.batch:
-                    messages = await self.consumer.getmany(
-                        timeout_ms=self.batch_timeout_ms,
-                        max_records=self.max_records,
-                    )
-
-                    if not messages:  # pragma: no cover
-                        await anyio.sleep(self.batch_timeout_ms / 1000)
-                        continue
-
-                    msg: Union[Message, Tuple[Message, ...]] = tuple(
-                        chain(*messages.values())
-                    )
-                else:
-                    msg = await self.consumer.getone()
-
-            except KafkaException:  # pragma: no cover
-                if connected is True:
+                msg = await self.get_msg()
+            except KafkaException:  # pragma: no cover  # noqa: PERF203
+                if connected:
                     connected = False
                 await anyio.sleep(5)
 
             else:
-                if connected is False:  # pragma: no cover
+                if not connected:  # pragma: no cover
                     connected = True
-                await self.consume(msg)  # type: ignore[arg-type]
+
+                if msg is not None:
+                    await self.consume(msg)  # type: ignore[arg-type]
+
+    @staticmethod
+    def get_routing_hash(topics: Iterable[str], group_id: Optional[str] = None) -> int:
+        return hash("".join((*topics, group_id or "")))
+
+    def __hash__(self) -> int:
+        return self.get_routing_hash(self.topics, self.group_id)
 
     @staticmethod
-    def get_routing_hash(topics: Sequence[str], group_id: Optional[str] = None) -> str:
-        return "".join((*topics, group_id or ""))
+    def build_log_context(
+        message: Optional["StreamMessage[Any]"],
+        topic: str,
+        group_id: Optional[str] = None,
+    ) -> Dict[str, str]:
+        return {
+            "topic": topic,
+            "group_id": group_id or "",
+            "message_id": getattr(message, "message_id", ""),
+        }
+
+    def add_prefix(self, prefix: str) -> None:
+        self.topics = tuple("".join((prefix, t)) for t in self.topics)
+
+
+class DefaultSubscriber(LogicSubscriber[Message]):
+    def __init__(
+        self,
+        *topics: str,
+        # Kafka information
+        group_id: Optional[str],
+        builder: Callable[..., AsyncConfluentConsumer],
+        is_manual: bool,
+        # Subscriber args
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[Message]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        super().__init__(
+            *topics,
+            group_id=group_id,
+            builder=builder,
+            is_manual=is_manual,
+            # subscriber args
+            default_parser=AsyncConfluentParser.parse_message,
+            default_decoder=AsyncConfluentParser.decode_message,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+    async def get_msg(self) -> Optional[Message]:
+        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+        return await self.consumer.getone()
+
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[Message]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topics)
+        else:
+            topic = message.raw_message.topic() or ",".join(self.topics)
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
+
+class BatchSubscriber(LogicSubscriber[Tuple[Message, ...]]):
+    def __init__(
+        self,
+        *topics: str,
+        batch_timeout_ms: int,
+        max_records: Optional[int],
+        # Kafka information
+        group_id: Optional[str],
+        builder: Callable[..., AsyncConfluentConsumer],
+        is_manual: bool,
+        # Subscriber args
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[Tuple[Message, ...]]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        self.batch_timeout_ms = batch_timeout_ms
+        self.max_records = max_records
+
+        super().__init__(
+            *topics,
+            group_id=group_id,
+            builder=builder,
+            is_manual=is_manual,
+            # subscriber args
+            default_parser=AsyncConfluentParser.parse_message_batch,
+            default_decoder=AsyncConfluentParser.decode_message_batch,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+    async def get_msg(self) -> Optional[Tuple[Message, ...]]:
+        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+
+        messages = await self.consumer.getmany(
+            timeout_ms=self.batch_timeout_ms,
+            max_records=self.max_records,
+        )
+
+        if not messages:  # pragma: no cover
+            await anyio.sleep(self.batch_timeout_ms / 1000)
+            return None
+
+        return messages
+
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[Tuple[Message, ...]]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topics)
+        else:
+            topic = message.raw_message[0].topic() or ",".join(self.topics)
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
```

### Comparing `faststream-0.4.7/faststream/confluent/message.py` & `faststream-0.5.0rc0/faststream/confluent/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,54 @@
-from typing import Any, Protocol
+from typing import Any, Protocol, Tuple, Union
 
-import confluent_kafka
+from confluent_kafka import Message
 
 from faststream.broker.message import StreamMessage
 
 
 class ConsumerProtocol(Protocol):
     """A protocol for Kafka consumers."""
 
-    async def commit(self) -> None: ...
+    async def commit(self) -> None:
+        ...
 
 
 class FakeConsumer:
     """A fake Kafka consumer."""
 
     async def commit(self) -> None:
         pass
 
 
 FAKE_CONSUMER = FakeConsumer()
 
 
-class KafkaMessage(StreamMessage[confluent_kafka.Message]):
+class KafkaMessage(
+    StreamMessage[
+        Union[
+            Message,
+            Tuple[Message, ...],
+        ]
+    ]
+):
     """Represents a Kafka message in the FastStream framework.
 
-    This class extends `StreamMessage` and is specialized for handling Kafka ConsumerRecord objects.
-
-    Methods:
-        ack(**kwargs) -> None:
-            Acknowledge the Kafka message.
-
-        nack(**kwargs) -> None:
-            Negative acknowledgment of the Kafka message.
-
-        reject(**kwargs) -> None:
-            Reject the Kafka message.
+    This class extends `StreamMessage` and is specialized for handling confluent_kafka.Message objects.
     """
 
     def __init__(
         self,
         *args: Any,
         consumer: ConsumerProtocol,
         is_manual: bool = False,
         **kwargs: Any,
     ) -> None:
-        """Constructor method for the KafkaMessage class.
-
-        Args:
-            *args (Any): Additional positional arguments.
-            consumer (AsyncConfluentConsumer): The Kafka consumer that received the message.
-            is_manual (bool): Whether the consumer is manual or not.
-            **kwargs (Any): Additional keyword arguments.
-
-        """
         super().__init__(*args, **kwargs)
 
         self.is_manual = is_manual
         self.consumer = consumer
 
-    async def ack(self, **kwargs: Any) -> None:
-        """Acknowledge the Kafka message.
-
-        Args:
-            **kwargs (Any): Additional keyword arguments.
-
-        Returns:
-            None: This method does not return a value.
-        """
+    async def ack(self) -> None:
+        """Acknowledge the Kafka message."""
         if self.is_manual and not self.committed:
             await self.consumer.commit()
             await super().ack()
```

### Comparing `faststream-0.4.7/faststream/confluent/parser.py` & `faststream-0.5.0rc0/faststream/confluent/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,57 @@
-from typing import TYPE_CHECKING, List, Optional, Tuple
-from uuid import uuid4
+from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 from confluent_kafka import Message
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.parsers import decode_message
+from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
 from faststream.confluent.message import FAKE_CONSUMER, KafkaMessage
 from faststream.types import DecodedMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
-    from faststream.confluent.asyncapi import Handler
+    from faststream.confluent.subscriber.usecase import LogicSubscriber
 
 
 class AsyncConfluentParser:
     """A class to parse Kafka messages."""
 
     @staticmethod
     async def parse_message(
         message: Message,
     ) -> StreamMessage[Message]:
-        """Parses a Kafka message.
-
-        Args:
-            message: The Kafka message to parse.
-
-        Returns:
-            A StreamMessage object representing the parsed message.
-
-        """
+        """Parses a Kafka message."""
         headers = {}
         if message.headers() is not None:
             for i, j in message.headers():  # type: ignore[union-attr]
                 if isinstance(j, str):
                     headers[i] = j
                 else:
                     headers[i] = j.decode()
         body = message.value()
         offset = message.offset()
         _, timestamp = message.timestamp()
 
-        handler: Optional["Handler"] = context.get_local("handler_")
+        handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
         return KafkaMessage(
             body=body,
             headers=headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=f"{offset}-{timestamp}",
-            correlation_id=headers.get("correlation_id", str(uuid4())),
+            correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
     async def parse_message_batch(
         message: Tuple[Message, ...],
-    ) -> KafkaMessage:
-        """Parses a batch of messages from a Kafka consumer.
-
-        Args:
-            message : A tuple of ConsumerRecord or Message objects representing the messages to parse.
-
-        Returns:
-            A StreamMessage object containing the parsed messages.
-
-        Raises:
-            NotImplementedError: If any of the messages are silent (i.e., have no sound).
-
-        Static Method:
-            This method is a static method. It does not require an instance of the class to be called.
-
-        """
+    ) -> StreamMessage[Tuple[Message, ...]]:
+        """Parses a batch of messages from a Kafka consumer."""
         first = message[0]
         last = message[-1]
 
         headers = {}
         if first.headers() is not None:
             for i, j in first.headers():  # type: ignore[union-attr]
                 if isinstance(j, str):
@@ -83,47 +59,31 @@
                 else:
                     headers[i] = j.decode()
         body = [m.value() for m in message]
         first_offset = first.offset()
         last_offset = last.offset()
         _, first_timestamp = first.timestamp()
 
-        handler: Optional["Handler"] = context.get_local("handler_")
+        handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
         return KafkaMessage(
             body=body,
             headers=headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=f"{first_offset}-{last_offset}-{first_timestamp}",
-            correlation_id=headers.get("correlation_id", str(uuid4())),
+            correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
     async def decode_message(msg: StreamMessage[Message]) -> DecodedMessage:
-        """Decodes a message.
-
-        Args:
-            msg: The message to be decoded.
-
-        Returns:
-            The decoded message.
-
-        """
+        """Decodes a message."""
         return decode_message(msg)
 
     @classmethod
     async def decode_message_batch(
         cls, msg: StreamMessage[Tuple[Message, ...]]
-    ) -> List[DecodedMessage]:
-        """Decode a batch of messages.
-
-        Args:
-            msg: A stream message containing a tuple of consumer records.
-
-        Returns:
-            A list of decoded messages.
-
-        """
+    ) -> DecodedMessage:
+        """Decode a batch of messages."""
         return [decode_message(await cls.parse_message(m)) for m in msg.raw_message]
```

### Comparing `faststream-0.4.7/faststream/confluent/security.py` & `faststream-0.5.0rc0/faststream/confluent/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     elif type(security) == SASLPlaintext:
         return _parse_sasl_plaintext(security)
     elif type(security) == SASLScram256:
         return _parse_sasl_scram256(security)
     elif type(security) == SASLScram512:
         return _parse_sasl_scram512(security)
     else:
-        raise NotImplementedError(f"KafkaBroker does not support {type(security)}")
+        raise NotImplementedError(f"KafkaBroker does not support `{type(security)}`.")
 
 
 def _parse_base_security(security: BaseSecurity) -> AnyDict:
     return {
         "security_protocol": "SSL" if security.use_ssl else "PLAINTEXT",
         "ssl_context": security.ssl_context,
     }
 
 
 def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
-    if security.use_ssl is None:
+    if security.ssl_context is None:
         warnings.warn(
             message=ssl_not_set_error_msg,
             category=RuntimeWarning,
             stacklevel=1,
         )
 
     return {
```

### Comparing `faststream-0.4.7/faststream/confluent/test.py` & `faststream-0.5.0rc0/faststream/rabbit/testing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,256 +1,310 @@
-from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
-from uuid import uuid4
+from typing import Any, Optional, Union
+from unittest.mock import AsyncMock
 
+import aiormq
+from aio_pika.abc import DateType, HeadersType, TimeoutType
+from aio_pika.message import IncomingMessage
+from pamqp import commands as spec
+from pamqp.header import ContentHeader
 from typing_extensions import override
 
-from faststream.broker.parsers import encode_message
-from faststream.broker.test import TestBroker, call_handler
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.confluent.asyncapi import Publisher
-from faststream.confluent.broker import KafkaBroker
-from faststream.confluent.producer import AsyncConfluentFastProducer
-from faststream.types import SendableMessage
-
-__all__ = ("TestKafkaBroker",)
-
-
-class TestKafkaBroker(TestBroker[KafkaBroker]):
-    """A class to represent a test Kafka broker."""
+from faststream.broker.message import gen_cor_id
+from faststream.broker.wrapper.call import HandlerCallWrapper
+from faststream.rabbit.broker.broker import RabbitBroker
+from faststream.rabbit.parser import AioPikaParser
+from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
+from faststream.rabbit.publisher.producer import AioPikaFastProducer
+from faststream.rabbit.schemas import (
+    ExchangeType,
+    RabbitExchange,
+    RabbitQueue,
+)
+from faststream.rabbit.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.rabbit.types import AioPikaSendableMessage
+from faststream.testing.broker import TestBroker, call_handler
+
+__all__ = ("TestRabbitBroker",)
+
+
+class TestRabbitBroker(TestBroker[RabbitBroker]):
+    """A class to test RabbitMQ brokers."""
+
+    @classmethod
+    def _patch_test_broker(cls, broker: RabbitBroker) -> None:
+        broker._channel = AsyncMock()
+        broker.declarer = AsyncMock()
+        super()._patch_test_broker(broker)
 
     @staticmethod
-    async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
+    async def _fake_connect(broker: RabbitBroker, *args: Any, **kwargs: Any) -> None:
         broker._producer = FakeProducer(broker)
 
     @staticmethod
-    def patch_publisher(broker: KafkaBroker, publisher: Any) -> None:
-        publisher._producer = broker._producer
-
-    @staticmethod
     def create_publisher_fake_subscriber(
-        broker: KafkaBroker,
-        publisher: Publisher,
+        broker: RabbitBroker,
+        publisher: AsyncAPIPublisher,
     ) -> HandlerCallWrapper[Any, Any, Any]:
-        @broker.subscriber(  # type: ignore[call-overload,misc]
-            publisher.topic,
-            batch=publisher.batch,
-            _raw=True,
+        sub = broker.subscriber(
+            queue=publisher.queue,
+            exchange=publisher.exchange,
         )
-        def f(msg: Any) -> None:
-            pass
 
-        return f  # type: ignore[no-any-return]
+        if not sub.calls:
+
+            @sub
+            def f(msg: Any) -> None:
+                pass
+
+            broker.setup_subscriber(sub)
+
+        return sub.calls[0].handler
 
     @staticmethod
     def remove_publisher_fake_subscriber(
-        broker: KafkaBroker, publisher: Publisher
+        broker: RabbitBroker,
+        publisher: AsyncAPIPublisher,
     ) -> None:
-        broker.handlers.pop(publisher.topic, None)
+        broker._subscribers.pop(
+            AsyncAPISubscriber.get_routing_hash(
+                queue=publisher.queue,
+                exchange=publisher.exchange,
+            ),
+            None,
+        )
 
 
-class FakeProducer(AsyncConfluentFastProducer):
-    """A fake Kafka producer for testing purposes.
+class PatchedMessage(IncomingMessage):
+    """Patched message class for testing purposes.
 
-    This class extends AsyncConfluentFastProducer and is used to simulate Kafka message publishing during tests.
+    This class extends aio_pika's IncomingMessage class and is used to simulate RabbitMQ message handling during tests.
     """
 
-    def __init__(self, broker: KafkaBroker) -> None:
-        """Initialize the FakeProducer.
+    async def ack(self, multiple: bool = False) -> None:
+        """Asynchronously acknowledge a message."""
+        pass
+
+    async def nack(self, multiple: bool = False, requeue: bool = True) -> None:
+        """Nack the message."""
+        pass
+
+    async def reject(self, requeue: bool = False) -> None:
+        """Rejects a task."""
+        pass
+
+
+def build_message(
+    message: AioPikaSendableMessage = "",
+    queue: Union[RabbitQueue, str] = "",
+    exchange: Union["RabbitExchange", str, None] = None,
+    *,
+    routing_key: str = "",
+    persist: bool = False,
+    reply_to: Optional[str] = None,
+    headers: Optional["HeadersType"] = None,
+    content_type: Optional[str] = None,
+    content_encoding: Optional[str] = None,
+    priority: Optional[int] = None,
+    correlation_id: Optional[str] = None,
+    expiration: Optional["DateType"] = None,
+    message_id: Optional[str] = None,
+    timestamp: Optional["DateType"] = None,
+    message_type: Optional[str] = None,
+    user_id: Optional[str] = None,
+    app_id: Optional[str] = None,
+) -> PatchedMessage:
+    """Build a patched RabbitMQ message for testing."""
+    que = RabbitQueue.validate(queue)
+    exch = RabbitExchange.validate(exchange)
+
+    routing = routing_key or que.routing
+
+    msg = AioPikaParser.encode_message(
+        message=message,
+        persist=persist,
+        reply_to=reply_to,
+        headers=headers,
+        content_type=content_type,
+        content_encoding=content_encoding,
+        priority=priority,
+        correlation_id=correlation_id,
+        expiration=expiration,
+        message_id=message_id,
+        timestamp=timestamp,
+        message_type=message_type,
+        user_id=user_id,
+        app_id=app_id,
+    )
+
+    return PatchedMessage(
+        aiormq.abc.DeliveredMessage(
+            delivery=spec.Basic.Deliver(
+                exchange=getattr(exch, "name", ""),
+                routing_key=routing,
+            ),
+            header=ContentHeader(
+                properties=spec.Basic.Properties(
+                    content_type=msg.content_type,
+                    message_id=gen_cor_id(),
+                    headers=msg.headers,
+                    reply_to=reply_to,
+                )
+            ),
+            body=msg.body,
+            channel=AsyncMock(),
+        )
+    )
+
 
-        Args:
-            broker (KafkaBroker): The KafkaBroker instance to associate with this FakeProducer.
-        """
+class FakeProducer(AioPikaFastProducer):
+    """A fake RabbitMQ producer for testing purposes.
+
+    This class extends AioPikaFastProducer and is used to simulate RabbitMQ message publishing during tests.
+    """
+
+    def __init__(self, broker: RabbitBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
-        topic: str,
-        key: Optional[bytes] = None,
-        partition: Optional[int] = None,
-        timestamp_ms: Optional[int] = None,
-        headers: Optional[Dict[str, str]] = None,
-        correlation_id: Optional[str] = None,
+        message: AioPikaSendableMessage = "",
+        exchange: Union[RabbitExchange, str, None] = None,
         *,
-        reply_to: str = "",
+        routing_key: str = "",
+        mandatory: bool = True,
+        immediate: bool = False,
+        timeout: TimeoutType = None,
         rpc: bool = False,
-        rpc_timeout: Optional[float] = None,
+        rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-    ) -> Optional[SendableMessage]:
-        """Publish a message to the Kafka broker.
+        persist: bool = False,
+        reply_to: Optional[str] = None,
+        headers: Optional[HeadersType] = None,
+        content_type: Optional[str] = None,
+        content_encoding: Optional[str] = None,
+        priority: Optional[int] = None,
+        correlation_id: Optional[str] = None,
+        expiration: Optional[DateType] = None,
+        message_id: Optional[str] = None,
+        timestamp: Optional[DateType] = None,
+        message_type: Optional[str] = None,
+        user_id: Optional[str] = None,
+        app_id: Optional[str] = None,
+    ) -> Optional[Any]:
+        """Publish a message to a RabbitMQ queue or exchange."""
+        exch = RabbitExchange.validate(exchange)
 
-        Args:
-            message (SendableMessage): The message to be published.
-            topic (str): The Kafka topic to publish the message to.
-            key (Optional[bytes], optional): The message key. Defaults to None.
-            partition (Optional[int], optional): The Kafka partition to use. Defaults to None.
-            timestamp_ms (Optional[int], optional): The message timestamp in milliseconds. Defaults to None.
-            headers (Optional[Dict[str, str]], optional): Additional headers for the message. Defaults to None.
-            correlation_id (Optional[str], optional): The correlation ID for the message. Defaults to None.
-            reply_to (str, optional): The topic to which responses should be sent. Defaults to "".
-            rpc (bool, optional): If True, treat the message as an RPC request. Defaults to False.
-            rpc_timeout (Optional[float], optional): Timeout for RPC requests. Defaults to None.
-            raise_timeout (bool, optional): If True, raise an exception on timeout. Defaults to False.
-
-        Returns:
-            Optional[SendableMessage]: The response message, if this was an RPC request, otherwise None.
-        """
         incoming = build_message(
             message=message,
-            topic=topic,
-            key=key,
-            partition=partition,
-            timestamp_ms=timestamp_ms,
+            exchange=exch,
+            routing_key=routing_key,
+            reply_to=reply_to,
+            app_id=app_id,
+            user_id=user_id,
+            message_type=message_type,
             headers=headers,
+            persist=persist,
+            message_id=message_id,
+            priority=priority,
+            content_encoding=content_encoding,
+            content_type=content_type,
             correlation_id=correlation_id,
-            reply_to=reply_to,
+            expiration=expiration,
+            timestamp=timestamp,
         )
 
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            if topic in handler.topics:
-                return await call_handler(
-                    handler=handler,
-                    message=[incoming] if handler.batch else incoming,
-                    rpc=rpc,
-                    rpc_timeout=rpc_timeout,
-                    raise_timeout=raise_timeout,
-                )
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            if handler.exchange == exch:
+                call: bool = False
+
+                if (
+                    handler.exchange is None
+                    or handler.exchange.type == ExchangeType.DIRECT
+                ):
+                    call = handler.queue.name == incoming.routing_key
+
+                elif handler.exchange.type == ExchangeType.FANOUT:
+                    call = True
+
+                elif handler.exchange.type == ExchangeType.TOPIC:
+                    call = apply_pattern(
+                        handler.queue.routing,
+                        incoming.routing_key or "",
+                    )
+
+                elif handler.exchange.type == ExchangeType.HEADERS:  # pramga: no branch
+                    queue_headers = (handler.queue.bind_arguments or {}).copy()
+                    msg_headers = incoming.headers
+
+                    if not queue_headers:
+                        call = True
+
+                    else:
+                        matcher = queue_headers.pop("x-match", "all")
+
+                        full = True
+                        none = True
+                        for k, v in queue_headers.items():
+                            if msg_headers.get(k) != v:
+                                full = False
+                            else:
+                                none = False
+
+                        if not none:
+                            call = (matcher == "any") or full
+
+                else:
+                    raise AssertionError("unreachable")
+
+                if call:
+                    r = await call_handler(
+                        handler=handler,
+                        message=incoming,
+                        rpc=rpc,
+                        rpc_timeout=rpc_timeout,
+                        raise_timeout=raise_timeout,
+                    )
+
+                    if rpc:  # pragma: no branch
+                        return r
 
         return None
 
-    async def publish_batch(
-        self,
-        *msgs: SendableMessage,
-        topic: str,
-        partition: Optional[int] = None,
-        timestamp_ms: Optional[int] = None,
-        headers: Optional[Dict[str, str]] = None,
-    ) -> None:
-        """Publish a batch of messages to the Kafka broker.
 
-        Args:
-            *msgs (SendableMessage): Variable number of messages to be published.
-            topic (str): The Kafka topic to publish the messages to.
-            partition (Optional[int], optional): The Kafka partition to use. Defaults to None.
-            timestamp_ms (Optional[int], optional): The message timestamp in milliseconds. Defaults to None.
-            headers (Optional[Dict[str, str]], optional): Additional headers for the messages. Defaults to None.
-
-        Returns:
-            None: This method does not return a value.
-        """
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            if topic in handler.topics:
-                await call_handler(
-                    handler=handler,
-                    message=[
-                        build_message(
-                            message=message,
-                            topic=topic,
-                            partition=partition,
-                            timestamp_ms=timestamp_ms,
-                            headers=headers,
-                        )
-                        for message in msgs
-                    ],
-                )
+def apply_pattern(pattern: str, current: str) -> bool:
+    """Apply a pattern to a routing key."""
+    pattern_queue = iter(pattern.split("."))
+    current_queue = iter(current.split("."))
 
-        return None
+    pattern_symb = next(pattern_queue, None)
+    while pattern_symb:
+        if (next_symb := next(current_queue, None)) is None:
+            return False
 
+        elif pattern_symb == "#":
+            next_pattern = next(pattern_queue, None)
 
-class MockConfluentMessage:
-    def __init__(
-        self,
-        raw_msg: bytes,
-        topic: str,
-        key: bytes,
-        headers: List[Tuple[str, bytes]],
-        offset: int,
-        partition: int,
-        timestamp_type: int,
-        timestamp_ms: int,
-        error: Optional[str] = None,
-    ):
-        self._raw_msg = raw_msg
-        self._topic = topic
-        self._key = key
-        self._headers = headers
-        self._error = error
-        self._offset = offset
-        self._partition = partition
-        self._timestamp = (timestamp_type, timestamp_ms)
-
-    def len(self) -> int:
-        return len(self._raw_msg)
-
-    def error(self) -> Optional[str]:
-        return self._error
-
-    def headers(self) -> List[Tuple[str, bytes]]:
-        return self._headers
-
-    def key(self) -> bytes:
-        return self._key
-
-    def offset(self) -> int:
-        return self._offset
-
-    def partition(self) -> int:
-        return self._partition
+            if next_pattern is None:
+                return True
 
-    def timestamp(self) -> Tuple[int, int]:
-        return self._timestamp
+            if (next_symb := next(current_queue, None)) is None:
+                return False
 
-    def topic(self) -> str:
-        return self._topic
+            while next_pattern == "*":
+                next_pattern = next(pattern_queue, None)
+                if (next_symb := next(current_queue, None)) is None:
+                    return False
 
-    def value(self) -> bytes:
-        return self._raw_msg
+            while next_symb != next_pattern:
+                if (next_symb := next(current_queue, None)) is None:
+                    return False
 
+            pattern_symb = next(pattern_queue, None)
 
-def build_message(
-    message: SendableMessage,
-    topic: str,
-    partition: Optional[int] = None,
-    timestamp_ms: Optional[int] = None,
-    key: Optional[bytes] = None,
-    headers: Optional[Dict[str, str]] = None,
-    correlation_id: Optional[str] = None,
-    *,
-    reply_to: str = "",
-) -> MockConfluentMessage:
-    """Build a mock confluent_kafka.Message for a sendable message.
-
-    Args:
-        message (SendableMessage): The sendable message to be encoded.
-        topic (str): The Kafka topic for the message.
-        partition (Optional[int], optional): The Kafka partition for the message. Defaults to None.
-        timestamp_ms (Optional[int], optional): The message timestamp in milliseconds. Defaults to None.
-        key (Optional[bytes], optional): The message key. Defaults to None.
-        headers (Optional[Dict[str, str]], optional): Additional headers for the message. Defaults to None.
-        correlation_id (Optional[str], optional): The correlation ID for the message. Defaults to None.
-        reply_to (str, optional): The topic to which responses should be sent. Defaults to "".
+        elif pattern_symb == "*" or pattern_symb == next_symb:
+            pattern_symb = next(pattern_queue, None)
 
-    Returns:
-        MockConfluentMessage: A mock confluent_kafka.Message object.
-    """
-    msg, content_type = encode_message(message)
-    k = key or b""
-    headers = {
-        "content-type": content_type or "",
-        "correlation_id": correlation_id or str(uuid4()),
-        "reply_to": reply_to,
-        **(headers or {}),
-    }
-
-    # https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html#confluent_kafka.Message.timestamp
-    return MockConfluentMessage(
-        raw_msg=msg,
-        topic=topic,
-        key=k,
-        headers=[(i, j.encode()) for i, j in headers.items()],
-        offset=0,
-        partition=partition or 0,
-        timestamp_type=0 + 1,
-        timestamp_ms=timestamp_ms or int(datetime.now().timestamp()),
-    )
+        else:
+            return False
+
+    return next(current_queue, None) is None
```

### Comparing `faststream-0.4.7/faststream/confluent/shared/logging.py` & `faststream-0.5.0rc0/faststream/broker/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,146 @@
-import logging
-from typing import Any, Iterable, Optional, Sequence
+import asyncio
+import inspect
+from contextlib import suppress
+from functools import partial
+from types import TracebackType
+from typing import (
+    Any,
+    AsyncContextManager,
+    Callable,
+    Optional,
+    Type,
+    Union,
+    overload,
+)
 
-from confluent_kafka import Message
-from typing_extensions import override
+import anyio
+from typing_extensions import Self
 
-from faststream.broker.core.mixins import LoggingMixin
+from faststream.broker.acknowledgement_watcher import WatcherContext, get_watcher
 from faststream.broker.message import StreamMessage
-from faststream.log import access_logger
-from faststream.types import AnyDict
-
-
-class KafkaLoggingMixin(LoggingMixin):
-    """A class that provides logging functionality for Kafka.
-
-    Attributes:
-        _max_topic_len : maximum length of the topic name
+from faststream.broker.types import (
+    AsyncDecoder,
+    AsyncParser,
+    CustomDecoder,
+    CustomParser,
+    MsgType,
+)
+from faststream.types import LoggerProto
+from faststream.utils.functions import fake_context, to_async
+
+
+async def default_filter(msg: StreamMessage[Any]) -> bool:
+    """A function to filter stream messages."""
+    return not msg.processed
+
+
+def get_watcher_context(
+    logger: Optional[LoggerProto],
+    no_ack: bool,
+    retry: Union[bool, int],
+    **extra_options: Any,
+) -> Callable[..., AsyncContextManager[None]]:
+    """Create Acknowledgement scope."""
+    if no_ack:
+        return fake_context
+
+    else:
+        return partial(
+            WatcherContext,
+            watcher=get_watcher(logger, retry),
+            **extra_options,
+        )
 
-    Methods:
-        __init__ : initializes the KafkaLoggingMixin object
-        _get_log_context : returns the log context for a given message and topics
-        fmt : returns the log format string
-        _setup_log_context : sets up the log context for a given list of topics
 
-    """
+class MultiLock:
+    """A class representing a multi lock."""
 
-    _max_topic_len: int
+    def __init__(self) -> None:
+        """Initialize a new instance of the class."""
+        self.queue: "asyncio.Queue[None]" = asyncio.Queue()
+
+    def __enter__(self) -> Self:
+        """Enter the context."""
+        self.acquire()
+        return self
 
-    def __init__(
+    def __exit__(
         self,
-        *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = None,
-        **kwargs: Any,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
     ) -> None:
-        """Initialize the class.
-
-        Args:
-            *args: Variable length argument list
-            logger: Optional logger object
-            log_level: Log level (default: logging.INFO)
-            log_fmt: Optional log format string
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            None
-
-        """
-        super().__init__(
-            *args,
-            logger=logger,
-            log_level=log_level,
-            log_fmt=log_fmt,
-            **kwargs,
-        )
-        self._max_topic_len = 4
-        self._max_group_len = 0
+        """Exit the context."""
+        self.release()
 
-    @override
-    def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[StreamMessage[Message]],
-        topics: Sequence[str] = (),
-        group_id: Optional[str] = None,
-    ) -> AnyDict:
-        """Get the log context.
-
-        Args:
-            message: Optional stream message of type confluent_kafka.Message
-            topics: Sequence of topics
-            group_id: Optional group ID
-
-        Returns:
-            A dictionary containing the log context
-
-        """
-        if topics:
-            topic = ", ".join(topics)
-        elif message is not None and message.raw_message.topic() is not None:
-            topic = message.raw_message.topic()  # type: ignore[assignment]
-        else:
-            topic = ""
-
-        context = {
-            "topic": topic,
-            "group_id": group_id or "",
-            **super()._get_log_context(message),
-        }
-        return context
+    def acquire(self) -> None:
+        """Acquire lock."""
+        self.queue.put_nowait(None)
+
+    def release(self) -> None:
+        """Release lock."""
+        with suppress(asyncio.QueueEmpty, ValueError):
+            self.queue.get_nowait()
+            self.queue.task_done()
 
     @property
-    def fmt(self) -> str:
-        return super().fmt or (
-            "%(asctime)s %(levelname)s - "
-            + f"%(topic)-{self._max_topic_len}s | "
-            + (f"%(group_id)-{self._max_group_len}s | " if self._max_group_len else "")
-            + f"%(message_id)-{self._message_id_ln}s "
-            + "- %(message)s"
-        )
+    def qsize(self) -> int:
+        """Return the size of the queue."""
+        return self.queue.qsize()
 
-    def _setup_log_context(
-        self, topics: Iterable[str], group_id: Optional[str] = None
-    ) -> None:
-        """Set up log context.
-
-        Args:
-            topics: An iterable of topics.
-            group_id: Optional group ID.
+    @property
+    def empty(self) -> bool:
+        """Return whether the queue is empty."""
+        return self.queue.empty()
 
-        Returns:
-            None.
+    async def wait_release(self, timeout: Optional[float] = None) -> None:
+        """Wait for the queue to be released.
 
+        Using for graceful shutdown.
         """
-        for t in topics:
-            self._max_topic_len = max((self._max_topic_len, len(t)))
-
-        if group_id:
-            self._max_group_len = max((self._max_group_len, len(group_id)))
+        if timeout:
+            with anyio.move_on_after(timeout):
+                await self.queue.join()
+
+
+@overload
+def resolve_custom_func(
+    custom_func: Optional[CustomParser[MsgType]],
+    default_func: AsyncParser[MsgType],
+) -> AsyncParser[MsgType]:
+    ...
+
+
+@overload
+def resolve_custom_func(
+    custom_func: Optional[CustomDecoder[StreamMessage[MsgType]]],
+    default_func: AsyncDecoder[StreamMessage[MsgType]],
+) -> AsyncDecoder[StreamMessage[MsgType]]:
+    ...
+
+
+def resolve_custom_func(
+    custom_func: Union[
+        Optional[CustomDecoder[StreamMessage[MsgType]]],
+        Optional[CustomParser[MsgType]],
+    ],
+    default_func: Union[
+        AsyncDecoder[StreamMessage[MsgType]],
+        AsyncParser[MsgType],
+    ],
+) -> Union[
+    AsyncDecoder[StreamMessage[MsgType]],
+    AsyncParser[MsgType],
+]:
+    """Resolve a custom parser/decoder with default one."""
+    if custom_func is None:
+        return default_func
+
+    original_params = inspect.signature(custom_func).parameters
+
+    if len(original_params) == 1:
+        return to_async(custom_func)
+
+    else:
+        name = tuple(original_params.items())[1][0]
+        return partial(to_async(custom_func), **{name: default_func})  # type: ignore
```

### Comparing `faststream-0.4.7/faststream/confluent/shared/schemas.py` & `faststream-0.5.0rc0/faststream/kafka/schemas/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ssl
 from asyncio import AbstractEventLoop
 from typing import List, Literal, Optional, Union
 
-from typing_extensions import Required, TypedDict
+from aiokafka.abc import AbstractTokenProvider
+from typing_extensions import TypedDict
 
 
 class ConsumerConnectionParams(TypedDict, total=False):
     """A class to represent the connection parameters for a consumer.
 
     Attributes:
         bootstrap_servers : Required. The bootstrap servers to connect to.
@@ -18,18 +19,17 @@
         security_protocol : The security protocol to use for the connection. Must be one of "SSL" or "PLAINTEXT".
         api_version : The API version to use for the connection.
         connections_max_idle_ms : The maximum idle time in milliseconds before closing a connection.
         sasl_mechanism : The SASL mechanism to use for authentication. Must be one of "PLAIN", "GSSAPI", "SCRAM-SHA-256", "SCRAM-SHA-512", or "OAUTHBEARER".
         sasl_plain_password : The password to use for PLAIN SASL mechanism.
         sasl_plain_username : The username to use for PLAIN SASL mechanism.
         sasl_kerberos_service_name : The service
-
     """
 
-    bootstrap_servers: Required[Union[str, List[str]]]
+    bootstrap_servers: Union[str, List[str]]
     loop: Optional[AbstractEventLoop]
     client_id: str
     request_timeout_ms: int
     retry_backoff_ms: int
     metadata_max_age_ms: int
     security_protocol: Literal[
         "SSL",
@@ -45,8 +45,8 @@
         "OAUTHBEARER",
     ]
     sasl_plain_password: str
     sasl_plain_username: str
     sasl_kerberos_service_name: str
     sasl_kerberos_domain_name: str
     ssl_context: ssl.SSLContext
-    sasl_oauth_token_provider: str
+    sasl_oauth_token_provider: AbstractTokenProvider
```

### Comparing `faststream-0.4.7/faststream/kafka/annotations.py` & `faststream-0.5.0rc0/faststream/kafka/annotations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
 from faststream.kafka.broker import KafkaBroker as KB
 from faststream.kafka.message import KafkaMessage as KM
-from faststream.kafka.producer import AioKafkaFastProducer
+from faststream.kafka.publisher.producer import AioKafkaFastProducer
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
     "KafkaMessage",
```

### Comparing `faststream-0.4.7/faststream/kafka/broker.py` & `faststream-0.5.0rc0/faststream/kafka/router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,552 +1,554 @@
-from functools import partial, wraps
-from types import TracebackType
 from typing import (
     Any,
-    AsyncContextManager,
-    Awaitable,
     Callable,
     Dict,
     Iterable,
-    List,
     Literal,
     Optional,
     Sequence,
     Tuple,
-    Type,
     Union,
 )
 
-import aiokafka
+from aiokafka import ConsumerRecord
 from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from fast_depends.dependencies import Depends
-from typing_extensions import override
+from typing_extensions import Annotated, Doc, deprecated
 
-from faststream.__about__ import __version__
-from faststream.broker.core.asynchronous import BrokerAsyncUsecase, default_filter
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
+from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.types import (
-    AsyncPublisherProtocol,
+    BrokerMiddleware,
     CustomDecoder,
     CustomParser,
     Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-    WrappedReturn,
+    PublisherMiddleware,
+    SubscriberMiddleware,
 )
-from faststream.broker.wrapper import FakePublisher, HandlerCallWrapper
-from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.kafka.asyncapi import Handler, Publisher
-from faststream.kafka.message import KafkaMessage
-from faststream.kafka.producer import AioKafkaFastProducer
-from faststream.kafka.security import parse_security
-from faststream.kafka.shared.logging import KafkaLoggingMixin
-from faststream.kafka.shared.schemas import ConsumerConnectionParams
-from faststream.security import BaseSecurity
-from faststream.utils import context
-from faststream.utils.data import filter_by_dict
-
-
-class KafkaBroker(
-    KafkaLoggingMixin,
-    BrokerAsyncUsecase[aiokafka.ConsumerRecord, ConsumerConnectionParams],
-):
-    """KafkaBroker is a class for managing Kafka message consumption and publishing.
+from faststream.broker.utils import default_filter
+from faststream.kafka.broker.registrator import KafkaRegistrator
+from faststream.types import SendableMessage
 
-    It extends BrokerAsyncUsecase to handle asynchronous operations.
 
-    Args:
-        bootstrap_servers (Union[str, Iterable[str]]): Kafka bootstrap server(s).
-        protocol (str): The protocol used (default is "kafka").
-        protocol_version (str): The Kafka protocol version (default is "auto").
-        client_id (str): The client ID for the Kafka client.
-        **kwargs: Additional keyword arguments.
-
-    Attributes:
-        handlers (Dict[str, Handler]): A dictionary of message handlers.
-        _publishers (Dict[str, Publisher]): A dictionary of message publishers.
-        _producer (Optional[AioKafkaFastProducer]): An optional Kafka producer.
-
-    Methods:
-        connect(*args, **kwargs): Establishes a connection to Kafka.
-        start(): Starts the KafkaBroker and message handlers.
-        publish(*args, **kwargs): Publishes a message to Kafka.
-    """
+class KafkaPublisher(ArgsContainer):
+    """Delayed KafkaPublisher registration object.
 
-    url: List[str]
-    handlers: Dict[str, Handler]
-    _publishers: Dict[str, Publisher]
-    _producer: Optional[AioKafkaFastProducer]
+    Just a copy of `KafkaRegistrator.publisher(...)` arguments.
+    """
 
     def __init__(
         self,
-        bootstrap_servers: Union[str, Iterable[str]] = "localhost",
+        topic: Annotated[
+            str,
+            Doc("Topic where the message will be published."),
+        ],
         *,
-        protocol: Optional[str] = None,
-        protocol_version: str = "auto",
-        client_id: str = "faststream-" + __version__,
-        security: Optional[BaseSecurity] = None,
-        **kwargs: Any,
+        key: Annotated[
+            Union[bytes, Any, None],
+            Doc("""
+            A key to associate with the message. Can be used to
+            determine which partition to send the message to. If partition
+            is `None` (and producer's partitioner config is left as default),
+            then messages with the same key will be delivered to the same
+            partition (but if key is `None`, partition is chosen randomly).
+            Must be type `bytes`, or be serializable to bytes via configured
+            `key_serializer`.
+            """),
+        ] = None,
+        partition: Annotated[
+            Optional[int],
+            Doc("""
+            Specify a partition. If not set, the partition will be
+            selected using the configured `partitioner`.
+            """),
+        ] = None,
+        headers: Annotated[
+            Optional[Dict[str, str]],
+            Doc(
+                "Message headers to store metainformation. "
+                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("Topic name to send response."),
+        ] = "",
+        batch: Annotated[
+            bool,
+            Doc("Whether to send messages in batches or not."),
+        ] = False,
+        # basic args
+        middlewares: Annotated[
+            Iterable[PublisherMiddleware],
+            Doc("Publisher middlewares to wrap outgoing messages."),
+        ] = (),
+        # AsyncAPI args
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
     ) -> None:
-        """Initialize a KafkaBroker instance.
-
-        Args:
-            bootstrap_servers (Union[str, Iterable[str]]): Kafka bootstrap server(s).
-            protocol (str): The protocol used (default is "kafka").
-            protocol_version (str): The Kafka protocol version (default is "auto").
-            client_id (str): The client ID for the Kafka client.
-            security (Optional[BaseSecurity]): Security protocol to use in communication with the broker (default is None).
-            **kwargs: Additional keyword arguments.
-        """
-        if protocol is None:
-            if security is not None and security.use_ssl:
-                protocol = "kafka-secure"
-            else:
-                protocol = "kafka"
-
         super().__init__(
-            url=[bootstrap_servers]
-            if isinstance(bootstrap_servers, str)
-            else list(bootstrap_servers),
-            protocol=protocol,
-            protocol_version=protocol_version,
-            security=security,
-            **kwargs,
-            client_id=client_id,
-            bootstrap_servers=bootstrap_servers,
-        )
-        self.client_id = client_id
-        self._producer = None
-
-    async def _close(
-        self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
-    ) -> None:
-        """Close the KafkaBroker, stopping the producer and cleaning up resources.
-
-        Args:
-            exc_type (Optional[Type[BaseException]]): The exception type.
-            exc_val (Optional[BaseException]]): The exception value.
-            exec_tb (Optional[TracebackType]]): The traceback.
-        """
-        if self._producer is not None:  # pragma: no branch
-            await self._producer.stop()
-            self._producer = None
-
-        await super()._close(exc_type, exc_val, exec_tb)
-
-    async def connect(
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> ConsumerConnectionParams:
-        """Establishes a connection to Kafka and returns connection parameters.
-
-        Args:
-            *args: Additional arguments.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            ConsumerConnectionParams: The connection parameters.
-        """
-        connection = await super().connect(*args, **kwargs)
-        for p in self._publishers.values():
-            p._producer = self._producer
-        return connection
-
-    @override
-    async def _connect(  # type: ignore[override]
-        self,
-        *,
-        client_id: str,
-        **kwargs: Any,
-    ) -> ConsumerConnectionParams:
-        """Connects to Kafka, initializes the producer, and returns connection parameters.
-
-        Args:
-            client_id (str): The client ID.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            ConsumerConnectionParams: The connection parameters.
-        """
-        security_params = parse_security(self.security)
-        producer = aiokafka.AIOKafkaProducer(
-            **kwargs, **security_params, client_id=client_id
-        )
-        await producer.start()
-        self._producer = AioKafkaFastProducer(
-            producer=producer,
-        )
-        return filter_by_dict(ConsumerConnectionParams, {**kwargs, **security_params})
-
-    async def start(self) -> None:
-        """Start the KafkaBroker and message handlers."""
-        context.set_global(
-            "default_log_context",
-            self._get_log_context(None, ""),
+            topic=topic,
+            key=key,
+            partition=partition,
+            batch=batch,
+            headers=headers,
+            reply_to=reply_to,
+            # basic args
+            middlewares=middlewares,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            schema=schema,
+            include_in_schema=include_in_schema,
         )
 
-        await super().start()
 
-        for handler in self.handlers.values():
-            c = self._get_log_context(None, handler.topics, handler.group_id)
-            self._log(f"`{handler.call_name}` waiting for messages", extra=c)
-            await handler.start(**(self._connection or {}))
+class KafkaRoute(SubscriberRoute):
+    """Class to store delayed KafkaBroker subscriber registration."""
 
-    def _process_message(
-        self,
-        func: Callable[[KafkaMessage], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[
-        [KafkaMessage],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ]:
-        """Wrap a message processing function with a watcher and publisher.
-
-        Args:
-            func (Callable[[KafkaMessage], Awaitable[T_HandlerReturn]]): The message processing function.
-            watcher (BaseWatcher): The message watcher.
-            disable_watcher: Whether to use watcher context.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            Callable[[KafkaMessage], Awaitable[WrappedReturn[T_HandlerReturn]]]: The wrapped message processing function.
-        """
-
-        @wraps(func)
-        async def process_wrapper(
-            message: KafkaMessage,
-        ) -> WrappedReturn[T_HandlerReturn]:
-            """Asynchronously process a Kafka message and wrap the return value.
-
-            Args:
-                message (KafkaMessage): The Kafka message to process.
-
-            Returns:
-                WrappedReturn[T_HandlerReturn]: The wrapped return value.
-
-            Raises:
-                AssertionError: If the code reaches an unreachable point.
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            async with watcher(message):
-                r = await func(message)
-
-                pub_response: Optional[AsyncPublisherProtocol]
-                if message.reply_to:
-                    pub_response = FakePublisher(
-                        partial(self.publish, topic=message.reply_to)
-                    )
-                else:
-                    pub_response = None
-
-                return r, pub_response
-
-        return process_wrapper
-
-    @override
-    def subscriber(  # type: ignore[override]
+    def __init__(
         self,
-        *topics: str,
-        group_id: Optional[str] = None,
-        key_deserializer: Optional[Callable[[bytes], Any]] = None,
-        value_deserializer: Optional[Callable[[bytes], Any]] = None,
-        fetch_max_wait_ms: int = 500,
-        fetch_max_bytes: int = 52428800,
-        fetch_min_bytes: int = 1,
-        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
-        auto_offset_reset: Literal[
-            "latest",
-            "earliest",
-            "none",
+        call: Annotated[
+            Callable[..., SendableMessage],
+            Doc(
+                "Message handler function "
+                "to wrap the same with `@broker.subscriber(...)` way."
+            ),
+        ],
+        *topics: Annotated[
+            str,
+            Doc("Kafka topics to consume messages from."),
+        ],
+        publishers: Annotated[
+            Iterable[KafkaPublisher],
+            Doc("Kafka publishers to broadcast the handler result."),
+        ] = (),
+        batch: Annotated[
+            bool,
+            Doc("Whether to consume messages in batches or not."),
+        ] = False,
+        group_id: Annotated[
+            Optional[str],
+            Doc("""
+            Name of the consumer group to join for dynamic
+            partition assignment (if enabled), and to use for fetching and
+            committing offsets. If `None`, auto-partition assignment (via
+            group coordinator) and offset commits are disabled.
+            """),
+        ] = None,
+        key_deserializer: Annotated[
+            Optional[Callable[[bytes], Any]],
+            Doc(
+                "Any callable that takes a raw message `bytes` "
+                "key and returns a deserialized one."
+            ),
+        ] = None,
+        value_deserializer: Annotated[
+            Optional[Callable[[bytes], Any]],
+            Doc(
+                "Any callable that takes a raw message `bytes` "
+                "value and returns a deserialized value."
+            ),
+        ] = None,
+        fetch_max_bytes: Annotated[
+            int,
+            Doc("""
+            The maximum amount of data the server should
+            return for a fetch request. This is not an absolute maximum, if
+            the first message in the first non-empty partition of the fetch
+            is larger than this value, the message will still be returned
+            to ensure that the consumer can make progress. NOTE: consumer
+            performs fetches to multiple brokers in parallel so memory
+            usage will depend on the number of brokers containing
+            partitions for the topic.
+            """),
+        ] = 50 * 1024 * 1024,
+        fetch_min_bytes: Annotated[
+            int,
+            Doc("""
+            Minimum amount of data the server should
+            return for a fetch request, otherwise wait up to
+            `fetch_max_wait_ms` for more data to accumulate.
+            """),
+        ] = 1,
+        fetch_max_wait_ms: Annotated[
+            int,
+            Doc("""
+            The maximum amount of time in milliseconds
+            the server will block before answering the fetch request if
+            there isn't sufficient data to immediately satisfy the
+            requirement given by `fetch_min_bytes`.
+            """),
+        ] = 500,
+        max_partition_fetch_bytes: Annotated[
+            int,
+            Doc("""
+            The maximum amount of data
+            per-partition the server will return. The maximum total memory
+            used for a request ``= #partitions * max_partition_fetch_bytes``.
+            This size must be at least as large as the maximum message size
+            the server allows or else it is possible for the producer to
+            send messages larger than the consumer can fetch. If that
+            happens, the consumer can get stuck trying to fetch a large
+            message on a certain partition.
+            """),
+        ] = 1 * 1024 * 1024,
+        auto_offset_reset: Annotated[
+            Literal["latest", "earliest", "none"],
+            Doc("""
+            A policy for resetting offsets on `OffsetOutOfRangeError` errors:
+
+            * `earliest` will move to the oldest available message
+            * `latest` will move to the most recent
+            * `none` will raise an exception so you can handle this case
+            """),
         ] = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5000,
-        check_crcs: bool = True,
-        partition_assignment_strategy: Sequence[AbstractPartitionAssignor] = (
-            RoundRobinPartitionAssignor,
-        ),
-        max_poll_interval_ms: int = 300000,
-        rebalance_timeout_ms: Optional[int] = None,
-        session_timeout_ms: int = 10000,
-        heartbeat_interval_ms: int = 3000,
-        consumer_timeout_ms: int = 200,
-        max_poll_records: Optional[int] = None,
-        exclude_internal_topics: bool = True,
-        isolation_level: Literal[
-            "read_uncommitted",
-            "read_committed",
+        auto_commit: Annotated[
+            bool,
+            Doc("""
+            If `True` the consumer's offset will be
+            periodically committed in the background.
+            """),
+        ] = True,
+        auto_commit_interval_ms: Annotated[
+            int,
+            Doc("""
+            Milliseconds between automatic
+            offset commits, if `auto_commit` is `True`."""),
+        ] = 5 * 1000,
+        check_crcs: Annotated[
+            bool,
+            Doc("""
+            Automatically check the CRC32 of the records
+            consumed. This ensures no on-the-wire or on-disk corruption to
+            the messages occurred. This check adds some overhead, so it may
+            be disabled in cases seeking extreme performance.
+            """),
+        ] = True,
+        partition_assignment_strategy: Annotated[
+            Sequence[AbstractPartitionAssignor],
+            Doc("""
+            List of objects to use to
+            distribute partition ownership amongst consumer instances when
+            group management is used. This preference is implicit in the order
+            of the strategies in the list. When assignment strategy changes:
+            to support a change to the assignment strategy, new versions must
+            enable support both for the old assignment strategy and the new
+            one. The coordinator will choose the old assignment strategy until
+            all members have been updated. Then it will choose the new
+            strategy.
+            """),
+        ] = (RoundRobinPartitionAssignor,),
+        max_poll_interval_ms: Annotated[
+            int,
+            Doc("""
+            Maximum allowed time between calls to
+            consume messages in batches. If this interval
+            is exceeded the consumer is considered failed and the group will
+            rebalance in order to reassign the partitions to another consumer
+            group member. If API methods block waiting for messages, that time
+            does not count against this timeout.
+            """),
+        ] = 5 * 60 * 1000,
+        rebalance_timeout_ms: Annotated[
+            Optional[int],
+            Doc("""
+            The maximum time server will wait for this
+            consumer to rejoin the group in a case of rebalance. In Java client
+            this behaviour is bound to `max.poll.interval.ms` configuration,
+            but as ``aiokafka`` will rejoin the group in the background, we
+            decouple this setting to allow finer tuning by users that use
+            `ConsumerRebalanceListener` to delay rebalacing. Defaults
+            to ``session_timeout_ms``
+            """),
+        ] = None,
+        session_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Client group session and failure detection
+            timeout. The consumer sends periodic heartbeats
+            (`heartbeat.interval.ms`) to indicate its liveness to the broker.
+            If no hearts are received by the broker for a group member within
+            the session timeout, the broker will remove the consumer from the
+            group and trigger a rebalance. The allowed range is configured with
+            the **broker** configuration properties
+            `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
+            """),
+        ] = 10 * 1000,
+        heartbeat_interval_ms: Annotated[
+            int,
+            Doc("""
+            The expected time in milliseconds
+            between heartbeats to the consumer coordinator when using
+            Kafka's group management feature. Heartbeats are used to ensure
+            that the consumer's session stays active and to facilitate
+            rebalancing when new consumers join or leave the group. The
+            value must be set lower than `session_timeout_ms`, but typically
+            should be set no higher than 1/3 of that value. It can be
+            adjusted even lower to control the expected time for normal
+            rebalances.
+            """),
+        ] = 3 * 1000,
+        consumer_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Maximum wait timeout for background fetching
+            routine. Mostly defines how fast the system will see rebalance and
+            request new data for new partitions.
+            """),
+        ] = 200,
+        max_poll_records: Annotated[
+            Optional[int],
+            Doc("""
+            The maximum number of records returned in a
+            single call by batch consumer. Has no limit by default.
+            """),
+        ] = None,
+        exclude_internal_topics: Annotated[
+            bool,
+            Doc("""
+            Whether records from internal topics
+            (such as offsets) should be exposed to the consumer. If set to True
+            the only way to receive records from an internal topic is
+            subscribing to it.
+            """),
+        ] = True,
+        isolation_level: Annotated[
+            Literal["read_uncommitted", "read_committed"],
+            Doc("""
+            Controls how to read messages written
+            transactionally.
+
+            * `read_committed`, batch consumer will only return
+            transactional messages which have been committed.
+
+            * `read_uncommitted` (the default), batch consumer will
+            return all messages, even transactional messages which have been
+            aborted.
+
+            Non-transactional messages will be returned unconditionally in
+            either mode.
+
+            Messages will always be returned in offset order. Hence, in
+            `read_committed` mode, batch consumer will only return
+            messages up to the last stable offset (LSO), which is the one less
+            than the offset of the first open transaction. In particular any
+            messages appearing after messages belonging to ongoing transactions
+            will be withheld until the relevant transaction has been completed.
+            As a result, `read_committed` consumers will not be able to read up
+            to the high watermark when there are in flight transactions.
+            Further, when in `read_committed` the seek_to_end method will
+            return the LSO. See method docs below.
+            """),
         ] = "read_uncommitted",
-        # broker arguments
-        dependencies: Sequence[Depends] = (),
-        parser: Optional[
-            Union[
-                CustomParser[aiokafka.ConsumerRecord, KafkaMessage],
-                CustomParser[Tuple[aiokafka.ConsumerRecord, ...], KafkaMessage],
-            ]
-        ] = None,
-        decoder: Optional[CustomDecoder] = None,
-        middlewares: Optional[
-            Sequence[
-                Callable[
-                    [aiokafka.ConsumerRecord],
-                    BaseMiddleware,
+        batch_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Milliseconds spent waiting if
+            data is not available in the buffer. If 0, returns immediately
+            with any records that are available currently in the buffer,
+            else returns empty.
+            """),
+        ] = 200,
+        max_records: Annotated[
+            Optional[int],
+            Doc("Number of messages to consume as one batch."),
+        ] = None,
+        # broker args
+        dependencies: Annotated[
+            Iterable[Depends],
+            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
+        ] = (),
+        parser: Annotated[
+            Optional[
+                Union[
+                    CustomParser[ConsumerRecord],
+                    CustomParser[Tuple[ConsumerRecord, ...]],
                 ]
-            ]
+            ],
+            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
-        filter: Union[
-            Filter[KafkaMessage],
-            Filter[StreamMessage[Tuple[aiokafka.ConsumerRecord, ...]]],
-        ] = default_filter,
-        batch: bool = False,
-        max_records: Optional[int] = None,
-        batch_timeout_ms: int = 200,
-        no_ack: bool = False,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
-        **original_kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        Union[
-            HandlerCallWrapper[
-                aiokafka.ConsumerRecord, P_HandlerParams, T_HandlerReturn
+        decoder: Annotated[
+            Optional[
+                Union[
+                    CustomDecoder[StreamMessage[ConsumerRecord]],
+                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
+                ]
             ],
-            HandlerCallWrapper[
-                Tuple[aiokafka.ConsumerRecord, ...], P_HandlerParams, T_HandlerReturn
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        middlewares: Annotated[
+            Iterable[SubscriberMiddleware],
+            Doc("Subscriber middlewares to wrap incoming message processing."),
+        ] = (),
+        filter: Annotated[
+            Union[
+                Filter[StreamMessage[ConsumerRecord]],
+                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
             ],
-        ],
-    ]:
-        """Create a message subscriber for the specified topics.
-
-        Args:
-            *topics (str): The topics to subscribe to.
-            group_id (Optional[str]): The Kafka consumer group ID.
-            key_deserializer (Optional[Callable[[bytes], Any]]): Key deserializer function.
-            value_deserializer (Optional[Callable[[bytes], Any]]): Value deserializer function.
-            fetch_max_wait_ms (int): The maximum time to wait for data.
-            fetch_max_bytes (int): The maximum number of bytes to fetch.
-            fetch_min_bytes (int): The minimum number of bytes to fetch.
-            max_partition_fetch_bytes (int): The maximum bytes to fetch for a partition.
-            auto_offset_reset (Literal["latest", "earliest", "none"]): Auto offset reset policy.
-            auto_commit (bool): Whether to enable auto-commit.
-            auto_commit_interval_ms (int): Auto-commit interval in milliseconds.
-            check_crcs (bool): Whether to check CRCs.
-            partition_assignment_strategy (Sequence[AbstractPartitionAssignor]): Partition assignment strategy.
-            max_poll_interval_ms (int): Maximum poll interval in milliseconds.
-            rebalance_timeout_ms (Optional[int]): Rebalance timeout in milliseconds.
-            session_timeout_ms (int): Session timeout in milliseconds.
-            heartbeat_interval_ms (int): Heartbeat interval in milliseconds.
-            consumer_timeout_ms (int): Consumer timeout in milliseconds.
-            max_poll_records (Optional[int]): Maximum number of records to poll.
-            exclude_internal_topics (bool): Whether to exclude internal topics.
-            isolation_level (Literal["read_uncommitted", "read_committed"]): Isolation level.
-            dependencies (Sequence[Depends]): Additional dependencies for message handling.
-            parser (Optional[Union[CustomParser[aiokafka.ConsumerRecord], CustomParser[Tuple[aiokafka.ConsumerRecord, ...]]]]): Message parser.
-            decoder (Optional[CustomDecoder]): Message decoder.
-            middlewares (Optional[Sequence[Callable[[aiokafka.ConsumerRecord], BaseMiddleware]]]): Message middlewares.
-            filter (Union[Filter[KafkaMessage], Filter[StreamMessage[Tuple[aiokafka.ConsumerRecord, ...]]]]): Message filter.
-            batch (bool): Whether to process messages in batches.
-            max_records (Optional[int]): Maximum number of records to process in each batch.
-            batch_timeout_ms (int): Batch timeout in milliseconds.
-            no_ack (bool): Whether not to ack/nack/reject messages.
-            title (Optional[str]): AsyncAPI title.
-            description (Optional[str]): AsyncAPI description.
-            include_in_schema (bool): Whether to include the message handler in the AsyncAPI schema.
-            **original_kwargs: Additional keyword arguments.
-
-        Returns:
-            Callable: A decorator that wraps a message handler function.
-        """
-        super().subscriber()
-
-        self._setup_log_context(topics, group_id)
-
-        if not auto_commit and not group_id:
-            raise ValueError("You should install `group_id` with manual commit mode")
-
-        key = Handler.get_routing_hash(topics, group_id)
-        builder = partial(
-            aiokafka.AIOKafkaConsumer,
+            Doc(
+                "Overload subscriber to consume various messages from the same source."
+            ),
+            deprecated(
+                "Deprecated in **FastStream 0.5.0**. "
+                "Please, create `subscriber` object and use it explicitly instead. "
+                "Argument will be removed in **FastStream 0.6.0**."
+            ),
+        ] = default_filter,
+        retry: Annotated[
+            bool,
+            Doc("Whether to `nack` message at processing exception."),
+        ] = False,
+        no_ack: Annotated[
+            bool,
+            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
+        ] = False,
+        # AsyncAPI args
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI subscriber object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc(
+                "AsyncAPI subscriber object description. "
+                "Uses decorated docstring as default."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
+    ) -> None:
+        super().__init__(
+            call,
+            *topics,
+            publishers=publishers,
+            group_id=group_id,
             key_deserializer=key_deserializer,
             value_deserializer=value_deserializer,
             fetch_max_wait_ms=fetch_max_wait_ms,
             fetch_max_bytes=fetch_max_bytes,
             fetch_min_bytes=fetch_min_bytes,
             max_partition_fetch_bytes=max_partition_fetch_bytes,
             auto_offset_reset=auto_offset_reset,
-            enable_auto_commit=auto_commit,
+            auto_commit=auto_commit,
             auto_commit_interval_ms=auto_commit_interval_ms,
             check_crcs=check_crcs,
             partition_assignment_strategy=partition_assignment_strategy,
             max_poll_interval_ms=max_poll_interval_ms,
             rebalance_timeout_ms=rebalance_timeout_ms,
             session_timeout_ms=session_timeout_ms,
             heartbeat_interval_ms=heartbeat_interval_ms,
             consumer_timeout_ms=consumer_timeout_ms,
             max_poll_records=max_poll_records,
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
+            max_records=max_records,
+            batch_timeout_ms=batch_timeout_ms,
+            batch=batch,
+            # basic args
+            dependencies=dependencies,
+            parser=parser,
+            decoder=decoder,
+            middlewares=middlewares,
+            filter=filter,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            include_in_schema=include_in_schema,
+            # FastDepends args
+            retry=retry,
+            no_ack=no_ack,
         )
-        handler = self.handlers.get(
-            key,
-            Handler(
-                *topics,
-                log_context_builder=partial(
-                    self._get_log_context,
-                    topics=topics,
-                    group_id=group_id,
-                ),
-                is_manual=not auto_commit,
-                group_id=group_id,
-                client_id=self.client_id,
-                builder=builder,
-                description=description,
-                title=title,
-                batch=batch,
-                batch_timeout_ms=batch_timeout_ms,
-                max_records=max_records,
-                include_in_schema=include_in_schema,
-                graceful_timeout=self.graceful_timeout,
-            ),
-        )
-
-        self.handlers[key] = handler
 
-        def consumer_wrapper(
-            func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[
-            aiokafka.ConsumerRecord, P_HandlerParams, T_HandlerReturn
-        ]:
-            """A wrapper function for a consumer handler.
-
-            Args:
-                func : The consumer handler function to be wrapped.
-
-            Returns:
-                The wrapped handler call.
-
-            Raises:
-                NotImplementedError: If silent animals are not supported.
-            !!! note
-
-                The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-            """
-            handler_call, dependant = self._wrap_handler(
-                func=func,
-                extra_dependencies=dependencies,
-                no_ack=no_ack,
-                **original_kwargs,
-            )
-
-            handler.add_call(
-                handler=handler_call,
-                filter=filter,
-                middlewares=middlewares,
-                parser=parser or self._global_parser,
-                decoder=decoder or self._global_decoder,
-                dependant=dependant,
-            )
 
-            return handler_call
-
-        return consumer_wrapper
+class KafkaRouter(
+    BrokerRouter[
+        Union[
+            ConsumerRecord,
+            Tuple[ConsumerRecord, ...],
+        ]
+    ],
+    KafkaRegistrator,
+):
+    """Includable to KafkaBroker router."""
 
-    @override
-    def publisher(  # type: ignore[override]
+    def __init__(
         self,
-        topic: str,
-        key: Optional[bytes] = None,
-        partition: Optional[int] = None,
-        timestamp_ms: Optional[int] = None,
-        headers: Optional[Dict[str, str]] = None,
-        reply_to: str = "",
-        batch: bool = False,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        schema: Optional[Any] = None,
-        include_in_schema: bool = True,
-    ) -> Publisher:
-        """Create a message publisher for the specified topic.
-
-        Args:
-            topic (str): The topic to publish messages to.
-            key (Optional[bytes]): Message key.
-            partition (Optional[int]): Partition to send the message to.
-            timestamp_ms (Optional[int]): Message timestamp in milliseconds.
-            headers (Optional[Dict[str, str]]): Message headers.
-            reply_to (str): The topic to which responses should be sent.
-            batch (bool): Whether to publish messages in batches.
-            title (Optional[str]): AsyncAPI title.
-            description (Optional[str]): AsyncAPI description.
-            schema (Optional[Any]): AsyncAPI schema.
-            include_in_schema (bool): Whether to include the message publisher in the AsyncAPI schema.
-
-        Returns:
-            Publisher: A message publisher.
-        """
-        publisher = self._publishers.get(
-            topic,
-            Publisher(
-                topic=topic,
-                client_id=self.client_id,
-                key=key,
-                batch=batch,
-                partition=partition,
-                timestamp_ms=timestamp_ms,
-                headers=headers,
-                reply_to=reply_to,
-                title=title,
-                _description=description,
-                _schema=schema,
-                include_in_schema=include_in_schema,
+        prefix: Annotated[
+            str,
+            Doc("String prefix to add to all subscribers queues."),
+        ] = "",
+        handlers: Annotated[
+            Iterable[KafkaRoute],
+            Doc("Route object to include."),
+        ] = (),
+        *,
+        dependencies: Annotated[
+            Iterable[Depends],
+            Doc(
+                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
-        )
-        super().publisher(topic, publisher)
-        if self._producer is not None:
-            publisher._producer = self._producer
-        return publisher
-
-    @override
-    async def publish(  # type: ignore[override]
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        """Publish a message to Kafka.
-
-        Args:
-            *args: Positional arguments for message publishing.
-            **kwargs: Keyword arguments for message publishing.
-
-        Raises:
-            RuntimeError: If KafkaBroker is not started yet.
-        """
-        assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        return await self._producer.publish(*args, **kwargs)
-
-    async def publish_batch(
-        self,
-        *args: Any,
-        **kwargs: Any,
+        ] = (),
+        middlewares: Annotated[
+            Iterable[
+                Union[
+                    BrokerMiddleware[ConsumerRecord],
+                    BrokerMiddleware[Tuple[ConsumerRecord, ...]],
+                ]
+            ],
+            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
+        ] = (),
+        parser: Annotated[
+            Optional[
+                Union[
+                    CustomParser[ConsumerRecord],
+                    CustomParser[Tuple[ConsumerRecord, ...]],
+                ]
+            ],
+            Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional[
+                Union[
+                    CustomDecoder[StreamMessage[ConsumerRecord]],
+                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
+                ]
+            ],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        include_in_schema: Annotated[
+            Optional[bool],
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = None,
     ) -> None:
-        """Publish a batch of messages to Kafka.
-
-        Args:
-            *args: Positional arguments for message publishing.
-            **kwargs: Keyword arguments for message publishing.
-
-        Raises:
-            RuntimeError: If KafkaBroker is not started yet.
-        """
-        assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        await self._producer.publish_batch(*args, **kwargs)
+        super().__init__(
+            handlers=handlers,
+            # basic args
+            prefix=prefix,
+            dependencies=dependencies,
+            middlewares=middlewares,
+            parser=parser,
+            decoder=decoder,
+            include_in_schema=include_in_schema,
+        )
```

### Comparing `faststream-0.4.7/faststream/kafka/handler.py` & `faststream-0.5.0rc0/faststream/rabbit/publisher/producer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,237 +1,230 @@
-import asyncio
-from itertools import chain
-from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
+from types import TracebackType
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncContextManager,
+    Optional,
+    Type,
+    Union,
+    cast,
+)
 
 import anyio
-from aiokafka import AIOKafkaConsumer, ConsumerRecord
-from aiokafka.errors import KafkaError
-from fast_depends.core import CallModel
-from typing_extensions import Unpack, override
-
-from faststream.__about__ import __version__
-from faststream.broker.handler import AsyncHandler
-from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.parsers import resolve_custom_func
-from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-)
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.kafka.message import KafkaMessage
-from faststream.kafka.parser import AioKafkaParser
-from faststream.kafka.shared.schemas import ConsumerConnectionParams
-
-
-class LogicHandler(AsyncHandler[ConsumerRecord]):
-    """A class to handle logic for consuming messages from Kafka.
-
-    Attributes:
-        topics : sequence of strings representing the topics to consume from
-        group_id : optional string representing the consumer group ID
-        consumer : optional AIOKafkaConsumer object representing the Kafka consumer
-        task : optional asyncio.Task object representing the task for consuming messages
-        batch : boolean indicating whether to consume messages in batches
-
-    Methods:
-        __init__ : constructor method for the LogicHandler class
-        start : method to start consuming messages from Kafka
-        close : method to close the Kafka consumer and cancel the consuming task
-        add_call : method to add a handler call for processing consumed messages
-        _consume : method to consume messages from Kafka and call the appropriate handler
-
-    """
-
-    topics: Sequence[str]
-    group_id: Optional[str] = None
-
-    consumer: Optional[AIOKafkaConsumer] = None
-    task: Optional["asyncio.Task[Any]"] = None
-    batch: bool = False
+from aio_pika.abc import AbstractIncomingMessage
+from typing_extensions import override
+
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.utils import resolve_custom_func
+from faststream.exceptions import WRONG_PUBLISH_ARGS
+from faststream.rabbit.parser import AioPikaParser
+from faststream.rabbit.schemas import RABBIT_REPLY, RabbitExchange
+from faststream.utils.functions import fake_context, timeout_scope
+
+if TYPE_CHECKING:
+    import aiormq
+    from aio_pika import IncomingMessage, RobustChannel, RobustQueue
+    from aio_pika.abc import DateType, HeadersType, TimeoutType
+    from anyio.streams.memory import MemoryObjectReceiveStream
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import (
+        AsyncDecoder,
+        AsyncParser,
+        CustomDecoder,
+        CustomParser,
+    )
+    from faststream.rabbit.types import AioPikaSendableMessage
+    from faststream.rabbit.utils import RabbitDeclarer
+    from faststream.types import SendableMessage
+
+
+class AioPikaFastProducer(ProducerProto):
+    """A class for fast producing messages using aio-pika."""
+
+    _decoder: "AsyncDecoder[StreamMessage[IncomingMessage]]"
+    _parser: "AsyncParser[IncomingMessage]"
 
-    @override
     def __init__(
         self,
-        *topics: str,
-        log_context_builder: Callable[[StreamMessage[Any]], Dict[str, str]],
-        graceful_timeout: Optional[float] = None,
-        # Kafka information
-        group_id: Optional[str] = None,
-        client_id: str = "faststream-" + __version__,
-        builder: Callable[..., AIOKafkaConsumer],
-        is_manual: bool = False,
-        batch: bool = False,
-        batch_timeout_ms: int = 200,
-        max_records: Optional[int] = None,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
+        *,
+        channel: "RobustChannel",
+        declarer: "RabbitDeclarer",
+        parser: Optional["CustomParser[IncomingMessage]"],
+        decoder: Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
     ) -> None:
-        """Initialize a Kafka consumer for the specified topics.
-
-        Args:
-            *topics: Variable length argument list of topics to consume from.
-            log_context_builder: Callable that builds the log context.
-            graceful_timeout: Optional timeout in seconds for graceful shutdown.
-            group_id: Optional group ID for the consumer.
-            client_id: Client ID for the consumer.
-            builder: Callable that constructs an AIOKafkaConsumer instance.
-            is_manual: Flag indicating whether to manually commit offsets.
-            batch: Flag indicating whether to consume messages in batches.
-            batch_timeout_ms: Timeout in milliseconds for batch consumption.
-            max_records: Maximum number of records to consume in a batch.
-            title: Optional title for the consumer.
-            description: Optional description for the consumer.
-            include_in_schema: Flag indicating whether to include the consumer in the API specification.
-
-        Raises:
-            NotImplementedError: If silent animals are not supported.
-
-        """
-        super().__init__(
-            log_context_builder=log_context_builder,
-            description=description,
-            title=title,
-            include_in_schema=include_in_schema,
-            graceful_timeout=graceful_timeout,
-        )
-
-        self.group_id = group_id
-        self.client_id = client_id
-        self.topics = topics
-
-        self.batch = batch
-        self.batch_timeout_ms = batch_timeout_ms
-        self.max_records = max_records
-        self.is_manual = is_manual
-
-        self.builder = builder
-        self.task = None
-        self.consumer = None
+        self._channel = channel
+        self.declarer = declarer
+        self._parser = resolve_custom_func(parser, AioPikaParser.parse_message)
+        self._decoder = resolve_custom_func(decoder, AioPikaParser.decode_message)
+        self._rpc_lock = anyio.Lock()
 
     @override
-    async def start(  # type: ignore[override]
+    async def publish(  # type: ignore[override]
         self,
-        **consumer_kwargs: Unpack[ConsumerConnectionParams],
-    ) -> None:
-        """Start the consumer.
+        message: "AioPikaSendableMessage",
+        exchange: Union["RabbitExchange", str, None] = None,
+        *,
+        correlation_id: str = "",
+        routing_key: str = "",
+        mandatory: bool = True,
+        immediate: bool = False,
+        timeout: "TimeoutType" = None,
+        rpc: bool = False,
+        rpc_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
+        persist: bool = False,
+        reply_to: Optional[str] = None,
+        headers: Optional["HeadersType"] = None,
+        content_type: Optional[str] = None,
+        content_encoding: Optional[str] = None,
+        priority: Optional[int] = None,
+        expiration: Optional["DateType"] = None,
+        message_id: Optional[str] = None,
+        timestamp: Optional["DateType"] = None,
+        message_type: Optional[str] = None,
+        user_id: Optional[str] = None,
+        app_id: Optional[str] = None,
+    ) -> Optional[Any]:
+        """Publish a message to a RabbitMQ queue."""
+        context: AsyncContextManager[
+            Optional["MemoryObjectReceiveStream[IncomingMessage]"]
+        ]
+        if rpc:
+            if reply_to is not None:
+                raise WRONG_PUBLISH_ARGS
+
+            context = _RPCCallback(
+                self._rpc_lock,
+                await self.declarer.declare_queue(RABBIT_REPLY),
+            )
+        else:
+            context = fake_context()
+
+        async with context as response_queue:
+            r = await self._publish(
+                message=message,
+                exchange=exchange,
+                routing_key=routing_key,
+                mandatory=mandatory,
+                immediate=immediate,
+                timeout=timeout,
+                persist=persist,
+                reply_to=reply_to if response_queue is None else RABBIT_REPLY.name,
+                headers=headers,
+                content_type=content_type,
+                content_encoding=content_encoding,
+                priority=priority,
+                correlation_id=correlation_id,
+                expiration=expiration,
+                message_id=message_id,
+                timestamp=timestamp,
+                message_type=message_type,
+                user_id=user_id,
+                app_id=app_id,
+            )
 
-        Args:
-            **consumer_kwargs: Additional keyword arguments to pass to the consumer.
+            if response_queue is None:
+                return r
 
-        Returns:
-            None
+            else:
+                msg: Optional["IncomingMessage"] = None
+                with timeout_scope(rpc_timeout, raise_timeout):
+                    msg = await response_queue.receive()
 
-        """
-        self.consumer = consumer = self.builder(
-            *self.topics,
-            group_id=self.group_id,
-            client_id=self.client_id,
-            **consumer_kwargs,
-        )
-        await consumer.start()
-        self.task = asyncio.create_task(self._consume())
-        await super().start()
-
-    async def close(self) -> None:
-        await super().close()
-
-        if self.consumer is not None:
-            await self.consumer.stop()
-            self.consumer = None
-
-        if self.task is not None:
-            self.task.cancel()
-            self.task = None
+                if msg:  # pragma: no branch
+                    return await self._decoder(await self._parser(msg))
 
-    def add_call(
+        return None
+
+    async def _publish(
         self,
+        message: "AioPikaSendableMessage",
         *,
-        handler: HandlerCallWrapper[ConsumerRecord, P_HandlerParams, T_HandlerReturn],
-        dependant: CallModel[P_HandlerParams, T_HandlerReturn],
-        parser: CustomParser[
-            Union[ConsumerRecord, Tuple[ConsumerRecord, ...]], KafkaMessage
-        ],
-        decoder: Optional[CustomDecoder[KafkaMessage]],
-        filter: Union[
-            Filter[KafkaMessage],
-            Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-        ],
-        middlewares: Optional[Sequence[Callable[[ConsumerRecord], BaseMiddleware]]],
-    ) -> None:
-        """Adds a call to the handler.
-
-        Args:
-            handler: The handler function to be called.
-            dependant: The dependant model.
-            parser: Optional custom parser for parsing the input.
-            decoder: Optional custom decoder for decoding the input.
-            filter: The filter for filtering the input.
-            middlewares: Optional sequence of middlewares to be applied.
-
-        Returns:
-            None
-
-        """
-        parser_ = resolve_custom_func(  # type: ignore[type-var]
-            parser,  # type: ignore[arg-type]
-            (
-                AioKafkaParser.parse_message_batch  # type: ignore[arg-type]
-                if self.batch
-                else AioKafkaParser.parse_message
-            ),
-        )
-        decoder_ = resolve_custom_func(
-            decoder,  # type: ignore[arg-type]
-            (
-                AioKafkaParser.decode_message_batch  # type: ignore[arg-type]
-                if self.batch
-                else AioKafkaParser.decode_message
-            ),
+        correlation_id: str,
+        exchange: Union["RabbitExchange", str, None],
+        routing_key: str,
+        mandatory: bool,
+        immediate: bool,
+        timeout: "TimeoutType",
+        persist: bool,
+        reply_to: Optional[str],
+        headers: Optional["HeadersType"],
+        content_type: Optional[str],
+        content_encoding: Optional[str],
+        priority: Optional[int],
+        expiration: Optional["DateType"],
+        message_id: Optional[str],
+        timestamp: Optional["DateType"],
+        message_type: Optional[str],
+        user_id: Optional[str],
+        app_id: Optional[str],
+    ) -> Union["aiormq.abc.ConfirmationFrameType", "SendableMessage"]:
+        """Publish a message to a RabbitMQ exchange."""
+        p_exchange = RabbitExchange.validate(exchange)
+
+        if p_exchange is None:
+            exchange_obj = self._channel.default_exchange
+        else:
+            p_exchange.passive = True
+            exchange_obj = await self.declarer.declare_exchange(p_exchange)
+
+        message = AioPikaParser.encode_message(
+            message=message,
+            persist=persist,
+            reply_to=reply_to,
+            headers=headers,
+            content_type=content_type,
+            content_encoding=content_encoding,
+            priority=priority,
+            correlation_id=correlation_id,
+            expiration=expiration,
+            message_id=message_id,
+            timestamp=timestamp,
+            message_type=message_type,
+            user_id=user_id,
+            app_id=app_id,
         )
-        super().add_call(
-            handler=handler,
-            parser=parser_,
-            decoder=decoder_,
-            filter=filter,  # type: ignore[arg-type]
-            dependant=dependant,
-            middlewares=middlewares,
+
+        return await exchange_obj.publish(
+            message=message,
+            routing_key=routing_key,
+            mandatory=mandatory,
+            immediate=immediate,
+            timeout=timeout,
         )
 
-    async def _consume(self) -> None:
-        assert self.consumer, "You need to start handler first"  # nosec B101
 
-        connected = True
-        while self.running:
-            try:
-                if self.batch:
-                    messages = await self.consumer.getmany(
-                        timeout_ms=self.batch_timeout_ms,
-                        max_records=self.max_records,
-                    )
-
-                    if not messages:  # pragma: no cover
-                        await anyio.sleep(self.batch_timeout_ms / 1000)
-                        continue
-
-                    msg = tuple(chain(*messages.values()))
-                else:
-                    msg = await self.consumer.getone()
-
-            except KafkaError:  # pragma: no cover
-                if connected is True:
-                    connected = False
-                await anyio.sleep(5)
+class _RPCCallback:
+    """A class provides an RPC lock."""
 
-            else:
-                if connected is False:  # pragma: no cover
-                    connected = True
-                await self.consume(msg)
-
-    @staticmethod
-    def get_routing_hash(topics: Sequence[str], group_id: Optional[str] = None) -> str:
-        return "".join((*topics, group_id or ""))
+    def __init__(
+        self, lock: "anyio.Lock", callback_queue: "RobustQueue"
+    ) -> None:
+        self.lock = lock
+        self.queue = callback_queue
+
+    async def __aenter__(self) -> "MemoryObjectReceiveStream[IncomingMessage]":
+        (
+            send_response_stream,
+            receive_response_stream,
+        ) = anyio.create_memory_object_stream[AbstractIncomingMessage](max_buffer_size=1)
+        await self.lock.acquire()
+
+        self.consumer_tag = await self.queue.consume(
+            callback=send_response_stream.send,
+            no_ack=True,
+        )
+
+        return cast(
+            "MemoryObjectReceiveStream[IncomingMessage]",
+            receive_response_stream,
+        )
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exc_tb: Optional[TracebackType] = None,
+    ) -> None:
+        self.lock.release()
+        await self.queue.cancel(self.consumer_tag)
```

### Comparing `faststream-0.4.7/faststream/kafka/message.py` & `faststream-0.5.0rc0/faststream/kafka/message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,54 @@
-from typing import Any, Protocol
+from typing import Any, Protocol, Tuple, Union
 
-import aiokafka
+from aiokafka import ConsumerRecord
 
 from faststream.broker.message import StreamMessage
 
 
 class ConsumerProtocol(Protocol):
     """A protocol for Kafka consumers."""
 
-    async def commit(self) -> None: ...
+    async def commit(self) -> None:
+        ...
 
 
 class FakeConsumer:
     """A fake Kafka consumer."""
 
     async def commit(self) -> None:
         pass
 
 
 FAKE_CONSUMER = FakeConsumer()
 
 
-class KafkaMessage(StreamMessage[aiokafka.ConsumerRecord]):
+class KafkaMessage(
+    StreamMessage[
+        Union[
+            ConsumerRecord,
+            Tuple[ConsumerRecord, ...],
+        ]
+    ]
+):
     """Represents a Kafka message in the FastStream framework.
 
     This class extends `StreamMessage` and is specialized for handling Kafka ConsumerRecord objects.
-
-    Methods:
-        ack(**kwargs) -> None:
-            Acknowledge the Kafka message.
-
-        nack(**kwargs) -> None:
-            Negative acknowledgment of the Kafka message.
-
-        reject(**kwargs) -> None:
-            Reject the Kafka message.
     """
 
     def __init__(
         self,
         *args: Any,
         consumer: ConsumerProtocol,
         is_manual: bool = False,
         **kwargs: Any,
     ) -> None:
-        """Initialize the KafkaMessage object.
-
-        Args:
-            *args (Any): Additional positional arguments.
-            consumer (aiokafka.AIOKafkaConsumer): The Kafka consumer.
-            is_manual (bool): Whether the message is manually acknowledged.
-            **kwargs (Any): Additional keyword arguments.
-        """
         super().__init__(*args, **kwargs)
 
         self.is_manual = is_manual
         self.consumer = consumer
 
-    async def ack(self, **kwargs: Any) -> None:
-        """Acknowledge the Kafka message.
-
-        Args:
-            **kwargs (Any): Additional keyword arguments.
-
-        Returns:
-            None: This method does not return a value.
-        """
+    async def ack(self) -> None:
+        """Acknowledge the Kafka message."""
         if self.is_manual and not self.committed:
             await self.consumer.commit()
             await super().ack()
```

### Comparing `faststream-0.4.7/faststream/kafka/parser.py` & `faststream-0.5.0rc0/faststream/nats/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,120 @@
-from typing import TYPE_CHECKING, List, Optional, Tuple
-from uuid import uuid4
+from typing import TYPE_CHECKING, Any, List, Optional
 
-from aiokafka import ConsumerRecord
+from nats.aio.msg import Msg
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.parsers import decode_message
-from faststream.kafka.message import FAKE_CONSUMER, KafkaMessage
-from faststream.types import DecodedMessage
+from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
+from faststream.nats.message import NatsBatchMessage, NatsMessage
+from faststream.types import AnyDict, DecodedMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
-    from faststream.kafka.asyncapi import Handler
+    from faststream.nats.subscriber.usecase import LogicSubscriber
 
 
-class AioKafkaParser:
-    """A class to parse Kafka messages."""
+class NatsBaseParser:
+    """A class to parse NATS messages."""
 
     @staticmethod
+    def get_path(
+        subject: str,
+    ) -> Optional[AnyDict]:
+        path: Optional[AnyDict] = None
+
+        handler: Optional["LogicSubscriber[Any]"]
+        if (
+            (handler := context.get_local("handler_")) is not None
+            and (path_re := handler.path_regex) is not None
+            and (match := path_re.match(subject)) is not None
+        ):
+            path = match.groupdict()
+
+        return path
+
+    @staticmethod
+    async def decode_message(
+        msg: StreamMessage["Msg"],
+    ) -> DecodedMessage:
+        return decode_message(msg)
+
+
+class NatsParser(NatsBaseParser):
+    """A class to parse NATS core messages."""
+
+    @classmethod
     async def parse_message(
-        message: ConsumerRecord,
-    ) -> StreamMessage[ConsumerRecord]:
-        """Parses a Kafka message.
-
-        Args:
-            message: The Kafka message to parse.
-
-        Returns:
-            A StreamMessage object representing the parsed message.
-        """
-        headers = {i: j.decode() for i, j in message.headers}
-        handler: Optional["Handler"] = context.get_local("handler_")
-        return KafkaMessage(
-            body=message.value,
-            headers=headers,
-            reply_to=headers.get("reply_to", ""),
-            content_type=headers.get("content-type"),
-            message_id=f"{message.offset}-{message.timestamp}",
-            correlation_id=headers.get("correlation_id", str(uuid4())),
+        cls,
+        message: "Msg",
+        *,
+        path: Optional[AnyDict] = None,
+    ) -> StreamMessage["Msg"]:
+        if path is None:
+            path = cls.get_path(message.subject)
+
+        headers = message.header or {}
+
+        return StreamMessage["Msg"](
             raw_message=message,
-            consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
-            is_manual=getattr(handler, "is_manual", True),
+            body=message.data,
+            path=path or {},
+            reply_to=message.reply,
+            headers=headers,
+            content_type=headers.get("content-type", ""),
+            message_id=headers.get("message_id", gen_cor_id()),
+            correlation_id=headers.get("correlation_id", gen_cor_id()),
         )
 
-    @staticmethod
-    async def parse_message_batch(
-        message: Tuple[ConsumerRecord, ...],
-    ) -> KafkaMessage:
-        """Parses a batch of messages from a Kafka consumer.
-
-        Args:
-            message : A tuple of ConsumerRecord objects representing the messages to parse.
-
-        Returns:
-            A StreamMessage object containing the parsed messages.
-
-        Raises:
-            NotImplementedError: If any of the messages are silent (i.e., have no sound).
-
-        Static Method:
-            This method is a static method. It does not require an instance of the class to be called.
-        """
-        first = message[0]
-        last = message[-1]
-        headers = {i: j.decode() for i, j in first.headers}
-        handler: Optional["Handler"] = context.get_local("handler_")
-        return KafkaMessage(
-            body=[m.value for m in message],
-            headers=headers,
-            reply_to=headers.get("reply_to", ""),
-            content_type=headers.get("content-type"),
-            message_id=f"{first.offset}-{last.offset}-{first.timestamp}",
-            correlation_id=headers.get("correlation_id", str(uuid4())),
+
+class JsParser(NatsBaseParser):
+    """A class to parse NATS JS messages."""
+
+    @classmethod
+    async def parse_message(
+        cls,
+        message: "Msg",
+        *,
+        path: Optional[AnyDict] = None,
+    ) -> StreamMessage["Msg"]:
+        if path is None:
+            path = cls.get_path(message.subject)
+
+        headers = message.header or {}
+
+        return NatsMessage(
             raw_message=message,
-            consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
-            is_manual=getattr(handler, "is_manual", True),
+            body=message.data,
+            path=path or {},
+            reply_to=headers.get("reply_to", ""),  # differ from core
+            headers=headers,
+            content_type=headers.get("content-type", ""),
+            message_id=headers.get("message_id", gen_cor_id()),
+            correlation_id=headers.get("correlation_id", gen_cor_id()),
         )
 
-    @staticmethod
-    async def decode_message(msg: StreamMessage[ConsumerRecord]) -> DecodedMessage:
-        """Decodes a message.
 
-        Args:
-            msg: The message to be decoded.
+class BatchParser(JsParser):
+    """A class to parse NATS batch messages."""
 
-        Returns:
-            The decoded message.
-        """
-        return decode_message(msg)
+    @staticmethod
+    async def parse_batch(
+        message: List["Msg"],
+    ) -> StreamMessage[List["Msg"]]:
+        return NatsBatchMessage(
+            raw_message=message,
+            body=[m.data for m in message],
+        )
 
     @classmethod
-    async def decode_message_batch(
-        cls, msg: StreamMessage[Tuple[ConsumerRecord, ...]]
+    async def decode_batch(
+        cls,
+        msg: StreamMessage[List["Msg"]],
     ) -> List[DecodedMessage]:
-        """Decode a batch of messages.
+        data: List[DecodedMessage] = []
+
+        path: Optional[AnyDict] = None
+        for m in msg.raw_message:
+            one_msg = await cls.parse_message(m, path=path)
+            path = one_msg.path
 
-        Args:
-            msg: A stream message containing a tuple of consumer records.
+            data.append(decode_message(one_msg))
 
-        Returns:
-            A list of decoded messages.
-        """
-        return [decode_message(await cls.parse_message(m)) for m in msg.raw_message]
+        return data
```

### Comparing `faststream-0.4.7/faststream/kafka/security.py` & `faststream-0.5.0rc0/faststream/kafka/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     elif type(security) == SASLPlaintext:
         return _parse_sasl_plaintext(security)
     elif type(security) == SASLScram256:
         return _parse_sasl_scram256(security)
     elif type(security) == SASLScram512:
         return _parse_sasl_scram512(security)
     else:
-        raise NotImplementedError(f"KafkaBroker does not support {type(security)}")
+        raise NotImplementedError(f"KafkaBroker does not support `{type(security)}`.")
 
 
 def _parse_base_security(security: BaseSecurity) -> AnyDict:
     return {
         "security_protocol": "SSL" if security.use_ssl else "PLAINTEXT",
         "ssl_context": security.ssl_context,
     }
 
 
 def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
-    if security.use_ssl is None:
+    if security.ssl_context is None:
         warnings.warn(
             message=ssl_not_set_error_msg,
             category=RuntimeWarning,
             stacklevel=1,
         )
 
     return {
```

### Comparing `faststream-0.4.7/faststream/kafka/shared/logging.py` & `faststream-0.5.0rc0/faststream/broker/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,96 @@
-import logging
-from typing import Any, Iterable, Optional, Sequence
+import json
+from contextlib import suppress
+from dataclasses import dataclass, field
+from typing import Any, Generic, Optional, Sequence, Tuple, TypeVar, Union
+from uuid import uuid4
 
-from aiokafka import ConsumerRecord
-from typing_extensions import override
+from faststream._compat import dump_json, json_loads
+from faststream.constants import ContentTypes
+from faststream.types import AnyDict, DecodedMessage, SendableMessage
 
-from faststream.broker.core.mixins import LoggingMixin
-from faststream.broker.message import StreamMessage
-from faststream.log import access_logger
-from faststream.types import AnyDict
-
-
-class KafkaLoggingMixin(LoggingMixin):
-    """A class that provides logging functionality for Kafka.
-
-    Attributes:
-        _max_topic_len : maximum length of the topic name
-
-    Methods:
-        __init__ : initializes the KafkaLoggingMixin object
-        _get_log_context : returns the log context for a given message and topics
-        fmt : returns the log format string
-        _setup_log_context : sets up the log context for a given list of topics
-
-    """
-
-    _max_topic_len: int
-
-    def __init__(
-        self,
-        *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize the class.
-
-        Args:
-            *args: Variable length argument list
-            logger: Optional logger object
-            log_level: Log level (default: logging.INFO)
-            log_fmt: Optional log format string
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            None
-
-        """
-        super().__init__(
-            *args,
-            logger=logger,
-            log_level=log_level,
-            log_fmt=log_fmt,
-            **kwargs,
-        )
-        self._max_topic_len = 4
-        self._max_group_len = 0
+# prevent circular imports
+MsgType = TypeVar("MsgType")
+
+
+def gen_cor_id() -> str:
+    """Generate random string to use as ID."""
+    return str(uuid4())
+
+
+@dataclass
+class StreamMessage(Generic[MsgType]):
+    """Generic class to represent a stream message."""
+
+    raw_message: "MsgType"
+
+    body: Union[bytes, Any]
+    decoded_body: Optional[DecodedMessage] = None
+    headers: AnyDict = field(default_factory=dict)
+    path: AnyDict = field(default_factory=dict)
+
+    content_type: Optional[str] = None
+    reply_to: str = ""
+    message_id: str = field(default_factory=gen_cor_id)  # pragma: no cover
+    correlation_id: str = field(
+        default_factory=gen_cor_id  # pragma: no cover
+    )
 
-    @override
-    def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[StreamMessage[ConsumerRecord]],
-        topics: Sequence[str] = (),
-        group_id: Optional[str] = None,
-    ) -> AnyDict:
-        """Get the log context.
-
-        Args:
-            message: Optional stream message of type ConsumerRecord
-            topics: Sequence of topics
-            group_id: Optional group ID
-
-        Returns:
-            A dictionary containing the log context
-
-        """
-        if topics:
-            topic = ", ".join(topics)
-        elif message is not None:
-            topic = message.raw_message.topic
+    processed: bool = field(default=False, init=False)
+    committed: bool = field(default=False, init=False)
+
+    async def ack(self) -> None:
+        self.committed = True
+
+    async def nack(self) -> None:
+        self.committed = True
+
+    async def reject(self) -> None:
+        self.committed = True
+
+
+def decode_message(message: StreamMessage[Any]) -> DecodedMessage:
+    """Decodes a message."""
+    body: Any = getattr(message, "body", message)
+    m: DecodedMessage = body
+
+    if content_type := getattr(message, "content_type", None):
+        if ContentTypes.text.value in content_type:
+            m = body.decode()
+        elif ContentTypes.json.value in content_type:  # pragma: no branch
+            m = json_loads(body)
         else:
-            topic = ""
+            with suppress(json.JSONDecodeError):
+                m = json_loads(body)
+    else:
+        with suppress(json.JSONDecodeError):
+            m = json_loads(body)
+
+    return m
+
+
+def encode_message(
+    msg: Union[Sequence[SendableMessage], SendableMessage],
+) -> Tuple[bytes, Optional[str]]:
+    """Encodes a message."""
+    if msg is None:
+        return (
+            b"",
+            None,
+        )
 
-        context = {
-            "topic": topic,
-            "group_id": group_id or "",
-            **super()._get_log_context(message),
-        }
-        return context
-
-    @property
-    def fmt(self) -> str:
-        return super().fmt or (
-            "%(asctime)s %(levelname)s - "
-            + f"%(topic)-{self._max_topic_len}s | "
-            + (f"%(group_id)-{self._max_group_len}s | " if self._max_group_len else "")
-            + f"%(message_id)-{self._message_id_ln}s "
-            + "- %(message)s"
+    if isinstance(msg, bytes):
+        return (
+            msg,
+            None,
         )
 
-    def _setup_log_context(
-        self, topics: Iterable[str], group_id: Optional[str] = None
-    ) -> None:
-        """Set up log context.
-
-        Args:
-            topics: An iterable of topics.
-            group_id: Optional group ID.
-
-        Returns:
-            None.
-
-        """
-        for t in topics:
-            self._max_topic_len = max((self._max_topic_len, len(t)))
+    if isinstance(msg, str):
+        return (
+            msg.encode(),
+            ContentTypes.text.value,
+        )
 
-        if group_id:
-            self._max_group_len = max((self._max_group_len, len(group_id)))
+    return (
+        dump_json(msg),
+        ContentTypes.json.value,
+    )
```

### Comparing `faststream-0.4.7/faststream/nats/__init__.py` & `faststream-0.5.0rc0/faststream/nats/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,32 +9,31 @@
     ReplayPolicy,
     RetentionPolicy,
     StorageType,
     StreamConfig,
     StreamSource,
 )
 
-from faststream.broker.test import TestApp
 from faststream.nats.annotations import NatsMessage
-from faststream.nats.broker import NatsBroker
-from faststream.nats.js_stream import JStream
-from faststream.nats.pull_sub import PullSub
-from faststream.nats.router import NatsRouter
-from faststream.nats.shared.router import NatsRoute
-from faststream.nats.test import TestNatsBroker
+from faststream.nats.broker.broker import NatsBroker
+from faststream.nats.router import NatsPublisher, NatsRoute, NatsRouter
+from faststream.nats.schemas import JStream, PullSub
+from faststream.nats.testing import TestNatsBroker
+from faststream.testing.app import TestApp
 
 __all__ = (
     "TestApp",
-    "TestNatsBroker",
-    "NatsMessage",
     "NatsBroker",
-    "NatsRouter",
-    "NatsRoute",
     "JStream",
     "PullSub",
+    "NatsRoute",
+    "NatsRouter",
+    "NatsPublisher",
+    "TestNatsBroker",
+    "NatsMessage",
     # Nats imports
     "ConsumerConfig",
     "DeliverPolicy",
     "AckPolicy",
     "ReplayPolicy",
     "DiscardPolicy",
     "RetentionPolicy",
```

### Comparing `faststream-0.4.7/faststream/nats/annotations.py` & `faststream-0.5.0rc0/faststream/nats/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nats.aio.client import Client as NatsClient
 from nats.js.client import JetStreamContext
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
 from faststream.nats.broker import NatsBroker as NB
 from faststream.nats.message import NatsMessage as NM
-from faststream.nats.producer import NatsFastProducer, NatsJSFastProducer
+from faststream.nats.publisher.producer import NatsFastProducer, NatsJSFastProducer
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
     "NatsMessage",
```

### Comparing `faststream-0.4.7/faststream/nats/broker.py` & `faststream-0.5.0rc0/faststream/nats/subscriber/usecase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,504 +1,470 @@
-import logging
-import warnings
-from functools import partial, wraps
-from types import TracebackType
+import asyncio
+from abc import abstractmethod
+from contextlib import suppress
 from typing import (
+    TYPE_CHECKING,
     Any,
-    AsyncContextManager,
     Awaitable,
     Callable,
     Dict,
+    Iterable,
     List,
     Optional,
     Sequence,
     Type,
     Union,
+    cast,
 )
 
-import nats
+import anyio
 from fast_depends.dependencies import Depends
-from nats.aio.client import Callback, Client, ErrorCallback
-from nats.aio.msg import Msg
-from nats.aio.subscription import (
-    DEFAULT_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_SUB_PENDING_MSGS_LIMIT,
-)
-from nats.js import api
-from nats.js.client import (
-    DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-    JetStreamContext,
-)
-from typing_extensions import TypeAlias, override
+from nats.errors import ConnectionClosedError, TimeoutError
+from typing_extensions import Annotated, Doc, override
 
-from faststream.broker.core.asynchronous import BrokerAsyncUsecase, default_filter
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.types import (
-    AsyncPublisherProtocol,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-    WrappedReturn,
-)
-from faststream.broker.wrapper import FakePublisher, HandlerCallWrapper
-from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.nats.asyncapi import Handler, Publisher
-from faststream.nats.helpers import stream_builder
-from faststream.nats.js_stream import JStream
-from faststream.nats.message import NatsMessage
-from faststream.nats.producer import NatsFastProducer, NatsJSFastProducer
-from faststream.nats.pull_sub import PullSub
-from faststream.nats.security import parse_security
-from faststream.nats.shared.logging import NatsLoggingMixin
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict, DecodedMessage
-from faststream.utils.context.repository import context
-
-Subject: TypeAlias = str
-
-
-class NatsBroker(
-    NatsLoggingMixin,
-    BrokerAsyncUsecase[Msg, Client],
-):
-    """A class to represent a NATS broker."""
-
-    url: List[str]
-    stream: Optional[JetStreamContext]
-
-    handlers: Dict[Subject, Handler]
-    _publishers: Dict[Subject, Publisher]
-    _producer: Optional[NatsFastProducer]
-    _js_producer: Optional[NatsJSFastProducer]
+from faststream.broker.publisher.fake import FakePublisher
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.subscriber.usecase import SubscriberUsecase
+from faststream.broker.types import CustomDecoder, CustomParser, MsgType
+from faststream.exceptions import NOT_CONNECTED_YET, SetupError
+from faststream.nats.parser import BatchParser, JsParser, NatsParser
+from faststream.types import AnyDict, LoggerProto, SendableMessage
+from faststream.utils.path import compile_path
+
+if TYPE_CHECKING:
+    from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+    from nats.aio.client import Client
+    from nats.aio.msg import Msg
+    from nats.aio.subscription import Subscription
+    from nats.js import JetStreamContext
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import (
+        AsyncDecoder,
+        AsyncParser,
+        BrokerMiddleware,
+    )
+    from faststream.nats.schemas import JStream, PullSub
+
+
+class LogicSubscriber(SubscriberUsecase[MsgType]):
+    """A class to represent a NATS handler."""
+
+    subscription: Union[
+        None,
+        "Subscription",
+        "JetStreamContext.PushSubscription",
+        "JetStreamContext.PullSubscription",
+    ]
+    producer: Optional["ProducerProto"]
+    _connection: Union["Client", "JetStreamContext", None]
 
     def __init__(
         self,
-        servers: Union[str, Sequence[str]] = ("nats://localhost:4222",),
         *,
-        security: Optional[BaseSecurity] = None,
-        protocol: str = "nats",
-        protocol_version: Optional[str] = "custom",
-        **kwargs: Any,
-    ) -> None:
-        """Initialize the NatsBroker object.
-
-        Args:
-            servers (Union[str, Sequence[str]]): The NATS server(s) to connect to.
-            security (Optional[BaseSecurity]): The security options.
-            protocol (str): The protocol to use.
-            protocol_version (Optional[str]): The protocol version to use.
-            **kwargs (Any): Additional keyword arguments.
-        """
-        kwargs.update(parse_security(security))
+        subject: str,
+        extra_options: Optional[AnyDict],
+        queue: str,
+        stream: Optional["JStream"],
+        pull_sub: Optional["PullSub"],
+        # Subscriber args
+        default_parser: "AsyncParser[MsgType]",
+        default_decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        no_ack: bool,
+        retry: Union[bool, int],
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        reg, path = compile_path(
+            subject,
+            replace_symbol="*",
+            patch_regex=lambda x: x.replace(".>", "..+"),
+        )
 
-        if kwargs.get("tls"):  # pragma: no cover
-            warnings.warn(
-                (
-                    "\nNATS `tls` option was deprecated and will be removed in 0.4.0"
-                    "\nPlease, use `security` with `BaseSecurity` or `SASLPlaintext` instead"
-                ),
-                DeprecationWarning,
-                stacklevel=2,
-            )
+        self.subject = path
+        self.path_regex = reg
+        self.queue = queue
+
+        self.stream = stream
+        self.pull_sub = pull_sub
+        self.extra_options = extra_options or {}
 
         super().__init__(
-            url=([servers] if isinstance(servers, str) else list(servers)),
-            protocol=protocol,
-            protocol_version=protocol_version,
-            security=security,
-            **kwargs,
+            default_parser=default_parser,
+            default_decoder=default_decoder,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
         )
 
-        self.__is_connected = False
-        self._producer = None
+        self._connection = None
+        self.subscription = None
+        self.producer = None
+        self.tasks: List["asyncio.Task[Any]"] = []
 
-        # JS options
-        self.stream = None
-        self._js_producer = None
-
-    async def connect(
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Client:
-        connection = await super().connect(*args, **kwargs)
-        for p in self._publishers.values():
-            self.__set_publisher_producer(p)
-        return connection
-
-    async def _connect(
-        self,
-        error_cb: Optional[ErrorCallback] = None,
-        reconnected_cb: Optional[Callback] = None,
-        **kwargs: Any,
-    ) -> Client:
-        self.__is_connected = True
-
-        connect = await nats.connect(
-            error_cb=self._log_connection_broken(error_cb),
-            reconnected_cb=self._log_reconnected(reconnected_cb),
-            **kwargs,
-        )
+    @override
+    def setup(  # type: ignore[override]
+        self,
+        *,
+        connection: Union["Client", "JetStreamContext"],
+        # basic args
+        logger: Optional["LoggerProto"],
+        producer: Optional["ProducerProto"],
+        graceful_timeout: Optional[float],
+        extra_context: Optional["AnyDict"],
+        # broker options
+        broker_parser: Optional["CustomParser[MsgType]"],
+        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        # dependant args
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
+    ) -> None:
+        self._connection = connection
 
-        self._producer = NatsFastProducer(
-            connect,
-            decoder=self._global_decoder,
-            parser=self._global_parser,
+        super().setup(
+            logger=logger,
+            producer=producer,
+            graceful_timeout=graceful_timeout,
+            extra_context=extra_context,
+            broker_parser=broker_parser,
+            broker_decoder=broker_decoder,
+            apply_types=apply_types,
+            is_validate=is_validate,
+            _get_dependant=_get_dependant,
         )
 
-        stream = self.stream = connect.jetstream()
-
-        self._js_producer = NatsJSFastProducer(
-            stream,
-            decoder=self._global_decoder,
-            parser=self._global_parser,
-        )
+    async def start(
+        self
+    ) -> None:
+        """Create NATS subscription and start consume tasks."""
+        assert self._connection, NOT_CONNECTED_YET
+        await super().start()
+        await self._create_subscription(connection=self._connection)
 
-        return connect
+    async def close(self) -> None:
+        """Clean up handler subscription, cancel consume task in graceful mode."""
+        await super().close()
+
+        if self.subscription is not None:
+            await self.subscription.unsubscribe()
+            self.subscription = None
+
+        for task in self.tasks:
+            if not task.done():
+                task.cancel()
+        self.tasks = []
 
-    async def _close(
+    @abstractmethod
+    async def _create_subscription(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
+        *,
+        connection: Union["Client", "JetStreamContext"],
     ) -> None:
-        self._producer = None
-        self._js_producer = None
-        self.stream = None
-
-        if self._connection is not None:
-            await self._connection.drain()
-
-        await super()._close(exc_type, exc_val, exec_tb)
-        self.__is_connected = False
+        """Create NATS subscription object to consume messages."""
+        raise NotImplementedError()
 
-    async def start(self) -> None:
-        context.set_global(
-            "default_log_context",
-            self._get_log_context(None, ""),
+    def _make_response_publisher(
+        self,
+        message: Annotated[
+            "StreamMessage[Any]",
+            Doc("Message requiring reply"),
+        ],
+    ) -> Sequence[FakePublisher]:
+        """Create FakePublisher object to use it as one of `publishers` in `self.consume` scope."""
+        if not message.reply_to or self._producer is None:
+            return ()
+
+        return (
+            FakePublisher(
+                self._producer.publish,
+                publish_kwargs={
+                    "subject": message.reply_to,
+                },
+            ),
         )
 
-        await super().start()
-        assert self._connection  # nosec B101
-        assert self.stream, "Broker should be started already"  # nosec B101
+    def __hash__(self) -> int:
+        return self.get_routing_hash(self.subject)
 
-        for handler in self.handlers.values():
-            stream = handler.stream
+    @staticmethod
+    def get_routing_hash(
+        subject: Annotated[
+            str,
+            Doc("NATS subject to consume messages"),
+        ],
+    ) -> int:
+        """Get handler hash by outer data.
 
-            if (is_js := stream is not None) and stream.declare:
-                try:  # pragma: no branch
-                    await self.stream.add_stream(
-                        config=stream.config,
-                        subjects=stream.subjects,
-                    )
-
-                except nats.js.errors.BadRequestError as e:
-                    old_config = (await self.stream.stream_info(stream.name)).config
-
-                    c = self._get_log_context(None, "")
-                    if (
-                        e.description
-                        == "stream name already in use with a different configuration"
-                    ):
-                        self._log(str(e), logging.WARNING, c)
-                        await self.stream.update_stream(
-                            config=stream.config,
-                            subjects=tuple(
-                                set(old_config.subjects or ()).union(stream.subjects)
-                            ),
-                        )
-
-                    else:  # pragma: no cover
-                        self._log(str(e), logging.ERROR, c, exc_info=e)
-
-                finally:
-                    # prevent from double declaration
-                    stream.declare = False
-
-            c = self._get_log_context(
-                None,
-                subject=handler.subject,
-                queue=handler.queue,
-                stream=stream.name if stream else "",
-            )
-            self._log(f"`{handler.call_name}` waiting for messages", extra=c)
-            await handler.start(self.stream if is_js else self._connection)
+        Using to find handler in `broker.handlers` dictionary.
+        """
+        return hash(subject)
+
+    @staticmethod
+    def build_log_context(
+        message: Annotated[
+            Optional["StreamMessage[Any]"],
+            Doc("Message which we are building context for"),
+        ],
+        subject: Annotated[
+            str,
+            Doc("NATS subject we are listening"),
+        ],
+        *,
+        queue: Annotated[
+            str,
+            Doc("Using queue group name"),
+        ] = "",
+        stream: Annotated[
+            Optional["JStream"],
+            Doc("Stream object we are listening"),
+        ] = None,
+    ) -> Dict[str, str]:
+        """Static method to build log context out of `self.consume` scope."""
+        return {
+            "subject": subject,
+            "queue": queue,
+            "stream": getattr(stream, "name", ""),
+            "message_id": getattr(message, "message_id", ""),
+        }
 
-    def _process_message(
+    def get_log_context(
         self,
-        func: Callable[[StreamMessage[Msg]], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[
-        [StreamMessage[Msg]],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ]:
-        @wraps(func)
-        async def process_wrapper(
-            message: StreamMessage[Msg],
-        ) -> WrappedReturn[T_HandlerReturn]:
-            async with watcher(message):
-                r = await func(message)
-
-                pub_response: Optional[AsyncPublisherProtocol]
-                if message.reply_to:
-                    pub_response = FakePublisher(
-                        partial(self.publish, subject=message.reply_to)
-                    )
-                else:
-                    pub_response = None
-
-                return r, pub_response
-
-        return process_wrapper
-
-    def _log_connection_broken(
-        self,
-        error_cb: Optional[ErrorCallback] = None,
-    ) -> ErrorCallback:
-        c = self._get_log_context(None, "")
-
-        async def wrapper(err: Exception) -> None:
-            if error_cb is not None:
-                await error_cb(err)
-
-            if self.__is_connected is True:
-                self._log(str(err), logging.WARNING, c, exc_info=err)
-                self.__is_connected = False
-
-        return wrapper
-
-    def _log_reconnected(
-        self,
-        cb: Optional[Callback] = None,
-    ) -> Callback:
-        c = self._get_log_context(None, "")
-
-        async def wrapper() -> None:
-            if cb is not None:
-                await cb()
-
-            if self.__is_connected is False:
-                self._log("Connection established", logging.INFO, c)
-                self.__is_connected = True
+        message: Annotated[
+            Optional["StreamMessage[Any]"],
+            Doc("Message which we are building context for"),
+        ],
+    ) -> Dict[str, str]:
+        """Log context factory using in `self.consume` scope."""
+        return self.build_log_context(
+            message=message,
+            subject=self.subject,
+            queue=self.queue,
+            stream=self.stream,
+        )
 
-        return wrapper
+    def add_prefix(self, prefix: str) -> None:
+        """Include Subscriber in router."""
+        self.subject = "".join((prefix, self.subject))
 
-    @override
-    def subscriber(  # type: ignore[override]
-        self,
-        subject: str,
-        queue: str = "",
-        pending_msgs_limit: Optional[int] = None,
-        pending_bytes_limit: Optional[int] = None,
-        # Core arguments
-        max_msgs: int = 0,
-        # JS arguments
-        durable: Optional[str] = None,
-        config: Optional[api.ConsumerConfig] = None,
-        ordered_consumer: bool = False,
-        idle_heartbeat: Optional[float] = None,
-        flow_control: bool = False,
-        deliver_policy: Optional[api.DeliverPolicy] = None,
-        headers_only: Optional[bool] = None,
-        # pull arguments
-        pull_sub: Optional[PullSub] = None,
-        inbox_prefix: bytes = api.INBOX_PREFIX,
-        # custom
-        ack_first: bool = False,
-        stream: Union[str, JStream, None] = None,
-        # broker arguments
-        dependencies: Sequence[Depends] = (),
-        parser: Optional[CustomParser[Msg, NatsMessage]] = None,
-        decoder: Optional[CustomDecoder[NatsMessage]] = None,
-        middlewares: Optional[Sequence[Callable[[Msg], BaseMiddleware]]] = None,
-        filter: Filter[NatsMessage] = default_filter,
-        no_ack: bool = False,
-        max_workers: int = 1,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
-        **original_kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        HandlerCallWrapper[Msg, P_HandlerParams, T_HandlerReturn],
-    ]:
-        stream = stream_builder.stream(stream)
 
-        if pull_sub is not None and stream is None:
-            raise ValueError("Pull subscriber can be used only with a stream")
+class DefaultHandler(LogicSubscriber["Msg"]):
+    """One-message consumer class."""
 
-        self._setup_log_context(
-            queue=queue,
+    send_stream: "MemoryObjectSendStream[Msg]"
+    receive_stream: "MemoryObjectReceiveStream[Msg]"
+
+    def __init__(
+        self,
+        *,
+        max_workers: int,
+        # default args
+        subject: str,
+        queue: str,
+        stream: Optional["JStream"],
+        pull_sub: Optional["PullSub"],
+        extra_options: Optional[AnyDict],
+        # Subscriber args
+        no_ack: bool,
+        retry: Union[bool, int],
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable["BrokerMiddleware[Msg]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        parser_: Union[Type[NatsParser], Type[JsParser]] = (
+            NatsParser if stream is None else JsParser
+        )
+        super().__init__(
             subject=subject,
-            stream=stream.name if stream else None,
+            queue=queue,
+            stream=stream,
+            pull_sub=pull_sub,
+            extra_options=extra_options,
+            # subscriber args
+            default_parser=parser_.parse_message,
+            default_decoder=parser_.decode_message,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            description_=description_,
+            title_=title_,
+            include_in_schema=include_in_schema,
         )
-        super().subscriber()
 
-        extra_options: AnyDict = {
-            "pending_msgs_limit": pending_msgs_limit
-            or (
-                DEFAULT_JS_SUB_PENDING_MSGS_LIMIT
-                if stream
-                else DEFAULT_SUB_PENDING_MSGS_LIMIT
-            ),
-            "pending_bytes_limit": pending_bytes_limit
-            or (
-                DEFAULT_JS_SUB_PENDING_BYTES_LIMIT
-                if stream
-                else DEFAULT_SUB_PENDING_BYTES_LIMIT
-            ),
-        }
+        self.max_workers = max_workers
 
-        if stream:
-            extra_options.update(
-                {
-                    "durable": durable,
-                    "stream": stream.name,
-                    "config": config,
-                }
-            )
+        self.send_stream, self.receive_stream = anyio.create_memory_object_stream(
+            max_buffer_size=max_workers
+        )
+        self.limiter = anyio.Semaphore(max_workers)
 
-            if pull_sub is not None:
-                extra_options.update({"inbox_prefix": inbox_prefix})
+    async def _create_subscription(
+        self,
+        *,
+        connection: Union["Client", "JetStreamContext"],
+    ) -> None:
+        """Create NATS subscription and start consume task."""
+        cb: Callable[["Msg"], Awaitable[Any]]
+        if self.max_workers > 1:
+            self.tasks.append(asyncio.create_task(self._serve_consume_queue()))
+            cb = self.__put_msg
+        else:
+            cb = self.consume
 
-            else:
-                extra_options.update(
-                    {
-                        "ordered_consumer": ordered_consumer,
-                        "idle_heartbeat": idle_heartbeat,
-                        "flow_control": flow_control,
-                        "deliver_policy": deliver_policy,
-                        "headers_only": headers_only,
-                        "manual_ack": not ack_first,
-                    }
-                )
+        if self.pull_sub is not None:
+            connection = cast("JetStreamContext", connection)
+
+            if self.stream is None:
+                raise SetupError(
+                    "Pull subscriber can be used only with a stream")
+
+            self.subscription = await connection.pull_subscribe(
+                subject=self.subject,
+                **self.extra_options,
+            )
+            self.tasks.append(asyncio.create_task(self._consume_pull(cb=cb)))
 
         else:
-            extra_options.update(
-                {
-                    "max_msgs": max_msgs,
-                }
+            self.subscription = await connection.subscribe(
+                subject=self.subject,
+                queue=self.queue,
+                cb=cb,  # type: ignore[arg-type]
+                **self.extra_options,
             )
 
-        key = Handler.get_routing_hash(subject)
-        handler = self.handlers[key] = self.handlers.get(
-            key,
-            Handler(
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                pull_sub=pull_sub,
-                extra_options=extra_options,
-                title=title,
-                description=description,
-                include_in_schema=include_in_schema,
-                graceful_timeout=self.graceful_timeout,
-                max_workers=max_workers,
-                log_context_builder=partial(
-                    self._get_log_context,
-                    stream=stream.name if stream else "",
-                    subject=subject,
-                    queue=queue,
-                ),
-            ),
-        )
+    async def _serve_consume_queue(
+        self,
+    ) -> None:
+        """Endless task consuming messages from in-memory queue.
 
-        if stream:
-            stream.subjects.append(handler.subject)
+        Suitable to batch messages by amount, timestamps, etc and call `consume` for this batches.
+        """
+        async with anyio.create_task_group() as tg:
+            async for msg in self.receive_stream:
+                tg.start_soon(self.__consume_msg, msg)
 
-        def consumer_wrapper(
-            func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[
-            Msg,
-            P_HandlerParams,
-            T_HandlerReturn,
-        ]:
-            handler_call, dependant = self._wrap_handler(
-                func,
-                extra_dependencies=dependencies,
-                no_ack=no_ack,
-                **original_kwargs,
-            )
+    async def _consume_pull(
+        self,
+        cb: Callable[["Msg"], Awaitable[SendableMessage]],
+    ) -> None:
+        """Endless task consuming messages using NATS Pull subscriber."""
+        assert self.pull_sub  # nosec B101
 
-            handler.add_call(
-                handler=handler_call,
-                filter=filter,
-                middlewares=middlewares,
-                parser=parser or self._global_parser,
-                decoder=decoder or self._global_decoder,
-                dependant=dependant,
-            )
+        sub = cast("JetStreamContext.PullSubscription", self.subscription)
 
-            return handler_call
+        while self.running:  # pragma: no branch
+            messages = []
+            with suppress(TimeoutError, ConnectionClosedError):
+                messages = await sub.fetch(
+                    batch=self.pull_sub.batch_size,
+                    timeout=self.pull_sub.timeout,
+                )
 
-        return consumer_wrapper
+            if messages:
+                async with anyio.create_task_group() as tg:
+                    for msg in messages:
+                        tg.start_soon(cb, msg)
 
-    @override
-    def publisher(  # type: ignore[override]
+    async def __consume_msg(
         self,
-        subject: str,
-        headers: Optional[Dict[str, str]] = None,
-        # Core
-        reply_to: str = "",
-        # JS
-        stream: Union[str, JStream, None] = None,
-        timeout: Optional[float] = None,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        schema: Optional[Any] = None,
-        include_in_schema: bool = True,
-    ) -> Publisher:
-        if (stream := stream_builder.stream(stream)) is not None:
-            stream.subjects.append(subject)
+        msg: "Msg",
+    ) -> None:
+        """Proxy method to call `self.consume` with semaphore block."""
+        async with self.limiter:
+            await self.consume(msg)
 
-        publisher = self._publishers.get(
-            subject,
-            Publisher(
-                subject=subject,
-                headers=headers,
-                # Core
-                reply_to=reply_to,
-                # JS
-                timeout=timeout,
-                stream=stream,
-                # AsyncAPI
-                title=title,
-                _description=description,
-                _schema=schema,
-                include_in_schema=include_in_schema,
-            ),
+    async def __put_msg(self, msg: "Msg") -> None:
+        """Proxy method to put msg into in-memory queue with semaphore block."""
+        async with self.limiter:
+            await self.send_stream.send(msg)
+
+
+class BatchHandler(LogicSubscriber[List["Msg"]]):
+    """Batch-message consumer class."""
+
+    pull_sub: "PullSub"
+    stream: "JStream"
+
+    def __init__(
+        self,
+        *,
+        # default args
+        subject: str,
+        queue: str,
+        stream: Optional["JStream"],
+        pull_sub: Optional["PullSub"],
+        extra_options: Optional[AnyDict],
+        # Subscriber args
+        no_ack: bool,
+        retry: Union[bool, int],
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable["BrokerMiddleware[List[Msg]]"],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
+        super().__init__(
+            subject=subject,
+            queue=queue,
+            stream=stream,
+            pull_sub=pull_sub,
+            extra_options=extra_options,
+            # subscriber args
+            default_parser=BatchParser.parse_batch,
+            default_decoder=BatchParser.decode_batch,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            description_=description_,
+            title_=title_,
+            include_in_schema=include_in_schema,
         )
-        super().publisher(subject, publisher)
-        self.__set_publisher_producer(publisher)
-        return publisher
 
     @override
-    async def publish(  # type: ignore[override]
+    async def _create_subscription(  # type: ignore[override]
         self,
-        *args: Any,
-        stream: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Optional[DecodedMessage]:
-        if stream is None:
-            assert self._producer, NOT_CONNECTED_YET  # nosec B101
-            return await self._producer.publish(*args, **kwargs)
-        else:
-            assert self._js_producer, NOT_CONNECTED_YET  # nosec B101
-            return await self._js_producer.publish(
-                *args,
-                stream=stream,
-                **kwargs,  # type: ignore[misc]
-            )
+        *,
+        connection: "JetStreamContext",
+    ) -> None:
+        """Create NATS subscription and start consume task."""
+        self.subscription = await connection.pull_subscribe(
+            subject=self.subject,
+            **self.extra_options,
+        )
+        self.tasks.append(asyncio.create_task(self._consume_pull()))
+
+    async def _consume_pull(self) -> None:
+        """Endless task consuming messages using NATS Pull subscriber."""
+        assert self.subscription, "You should call `create_subscription` at first."  # nosec B101
+
+        sub = cast("JetStreamContext.PullSubscription", self.subscription)
+
+        while self.running:  # pragma: no branch
+            with suppress(TimeoutError, ConnectionClosedError):
+                messages = await sub.fetch(
+                    batch=self.pull_sub.batch_size,
+                    timeout=self.pull_sub.timeout,
+                )
 
-    def __set_publisher_producer(self, publisher: Publisher) -> None:
-        if publisher.stream is not None:
-            if self._js_producer is not None:
-                publisher._producer = self._js_producer
-        elif self._producer is not None:
-            publisher._producer = self._producer
+                if messages:
+                    await self.consume(messages)
```

### Comparing `faststream-0.4.7/faststream/nats/handler.py` & `faststream-0.5.0rc0/faststream/kafka/subscriber/usecase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,268 +1,332 @@
 import asyncio
-from contextlib import suppress
-from typing import Any, Awaitable, Callable, Dict, Optional, Sequence, Union, cast
+from abc import ABC, abstractmethod
+from itertools import chain
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Sequence,
+    Tuple,
+)
 
 import anyio
-from anyio.abc import TaskGroup, TaskStatus
-from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
-from fast_depends.core import CallModel
-from nats.aio.client import Client
-from nats.aio.msg import Msg
-from nats.aio.subscription import Subscription
-from nats.errors import TimeoutError
-from nats.js import JetStreamContext
-from typing_extensions import Annotated, Doc, override
+from aiokafka import AIOKafkaConsumer, ConsumerRecord
+from aiokafka.errors import ConsumerStoppedError, KafkaError
+from fast_depends.dependencies import Depends
+from typing_extensions import override
 
-from faststream.broker.handler import AsyncHandler
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.parsers import resolve_custom_func
+from faststream.broker.publisher.fake import FakePublisher
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.subscriber.usecase import SubscriberUsecase
 from faststream.broker.types import (
+    AsyncDecoder,
+    AsyncParser,
+    BrokerMiddleware,
     CustomDecoder,
     CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
+    MsgType,
 )
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.nats.js_stream import JStream
-from faststream.nats.message import NatsMessage
-from faststream.nats.parser import JsParser, Parser
-from faststream.nats.pull_sub import PullSub
-from faststream.types import AnyDict, SendableMessage
-from faststream.utils.path import compile_path
-
-
-class LogicNatsHandler(AsyncHandler[Msg]):
-    """A class to represent a NATS handler."""
-
-    subscription: Union[
-        None,
-        Subscription,
-        JetStreamContext.PushSubscription,
-        JetStreamContext.PullSubscription,
-    ]
-    task_group: Optional[TaskGroup]
-    task: Optional["asyncio.Task[Any]"]
-    send_stream: MemoryObjectSendStream[Msg]
-    receive_stream: MemoryObjectReceiveStream[Msg]
+from faststream.kafka.parser import AioKafkaParser
+from faststream.kafka.schemas.params import ConsumerConnectionParams
+from faststream.types import AnyDict, LoggerProto
 
-    def __init__(
-        self,
-        subject: Annotated[
-            str,
-            Doc("NATS subject to subscribe"),
-        ],
-        log_context_builder: Annotated[
-            Callable[[StreamMessage[Any]], Dict[str, str]],
-            Doc("Function to create log extra data by message"),
-        ],
-        queue: Annotated[
-            str,
-            Doc("NATS queue name"),
-        ] = "",
-        stream: Annotated[
-            Optional[JStream],
-            Doc("NATS Stream object"),
-        ] = None,
-        pull_sub: Annotated[
-            Optional[PullSub],
-            Doc("NATS Pull consumer parameters container"),
-        ] = None,
-        extra_options: Annotated[
-            Optional[AnyDict],
-            Doc("Extra arguments for subscription creation"),
-        ] = None,
-        graceful_timeout: Annotated[
-            Optional[float],
-            Doc(
-                "Wait up to this time (if set) in graceful shutdown mode. "
-                "Kills task forcefully if expired."
-            ),
-        ] = None,
-        max_workers: Annotated[
-            int,
-            Doc("Process up to this parameter messages concurrently"),
-        ] = 1,
-        # AsyncAPI information
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI subscriber description"),
-        ] = None,
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI subscriber title"),
-        ] = None,
-        include_in_schema: Annotated[
-            bool,
-            Doc("Whether to include the handler in AsyncAPI schema"),
-        ] = True,
-    ) -> None:
-        """Initialize the NATS handler."""
-        reg, path = compile_path(
-            subject,
-            replace_symbol="*",
-            patch_regex=lambda x: x.replace(".>", "..+"),
-        )
-        self.subject = path
-        self.path_regex = reg
 
-        self.queue = queue
+class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
+    """A class to handle logic for consuming messages from Kafka."""
 
-        self.stream = stream
-        self.pull_sub = pull_sub
-        self.extra_options = extra_options or {}
+    topics: Sequence[str]
+    group_id: Optional[str]
 
+    consumer: Optional[AIOKafkaConsumer]
+    task: Optional["asyncio.Task[None]"]
+    client_id: Optional[str]
+    batch: bool
+
+    def __init__(
+        self,
+        *topics: str,
+        # Kafka information
+        group_id: Optional[str],
+        builder: Callable[..., AIOKafkaConsumer],
+        is_manual: bool,
+        # Subscriber args
+        default_parser: AsyncParser[MsgType],
+        default_decoder: AsyncDecoder[StreamMessage[MsgType]],
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> None:
         super().__init__(
-            log_context_builder=log_context_builder,
-            description=description,
+            default_parser=default_parser,
+            default_decoder=default_decoder,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
             include_in_schema=include_in_schema,
-            title=title,
-            graceful_timeout=graceful_timeout,
         )
 
-        self.max_workers = max_workers
-        self.subscription = None
-
-        self.send_stream, self.receive_stream = anyio.create_memory_object_stream(
-            max_buffer_size=max_workers
-        )
-        self.limiter = anyio.Semaphore(max_workers)
+        self.group_id = group_id
+        self.topics = topics
+        self.is_manual = is_manual
+        self.builder = builder
+        self.consumer = None
         self.task = None
 
-    def add_call(
-        self,
-        *,
-        handler: HandlerCallWrapper[Msg, P_HandlerParams, T_HandlerReturn],
-        dependant: CallModel[P_HandlerParams, T_HandlerReturn],
-        parser: Optional[CustomParser[Msg, NatsMessage]],
-        decoder: Optional[CustomDecoder[NatsMessage]],
-        filter: Filter[NatsMessage],
-        middlewares: Optional[Sequence[Callable[[Msg], BaseMiddleware]]],
-    ) -> None:
-        parser_ = Parser if self.stream is None else JsParser
-        super().add_call(
-            handler=handler,
-            parser=resolve_custom_func(parser, parser_.parse_message),
-            decoder=resolve_custom_func(decoder, parser_.decode_message),
-            filter=filter,  # type: ignore[arg-type]
-            dependant=dependant,
-            middlewares=middlewares,
-        )
+        # Setup it later
+        self.client_id = ""
+        self.__connection_args: ConsumerConnectionParams = {}
 
     @override
-    async def start(  # type: ignore[override]
+    def setup(  # type: ignore[override]
         self,
-        connection: Annotated[
-            Union[Client, JetStreamContext],
-            Doc("NATS client or JS Context object using to create subscription"),
-        ],
+        *,
+        client_id: Optional[str],
+        connection_args: ConsumerConnectionParams,
+        # basic args
+        logger: Optional[LoggerProto],
+        producer: Optional[ProducerProto],
+        graceful_timeout: Optional[float],
+        extra_context: Optional[AnyDict],
+        # broker options
+        broker_parser: Optional["CustomParser[MsgType]"],
+        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        # dependant args
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
-        """Create NATS subscription and start consume task."""
-        cb: Callable[[Msg], Awaitable[SendableMessage]]
-        if self.max_workers > 1:
-            self.task = asyncio.create_task(self._serve_consume_queue())
-            cb = self.__put_msg
-        else:
-            cb = self.consume
+        self.client_id = client_id
+        self.__connection_args = connection_args
 
-        if self.pull_sub is not None:
-            connection = cast(JetStreamContext, connection)
-
-            if self.stream is None:
-                raise ValueError("Pull subscriber can be used only with a stream")
-
-            self.subscription = await connection.pull_subscribe(
-                subject=self.subject,
-                **self.extra_options,
-            )
-            self.task = asyncio.create_task(self._consume_pull(cb))
+        super().setup(
+            logger=logger,
+            producer=producer,
+            graceful_timeout=graceful_timeout,
+            extra_context=extra_context,
+            broker_parser=broker_parser,
+            broker_decoder=broker_decoder,
+            apply_types=apply_types,
+            is_validate=is_validate,
+            _get_dependant=_get_dependant,
+        )
 
-        else:
-            self.subscription = await connection.subscribe(
-                subject=self.subject,
-                queue=self.queue,
-                cb=cb,  # type: ignore[arg-type]
-                **self.extra_options,
-            )
+    async def start(self) -> None:
+        """Start the consumer."""
+        self.consumer = consumer = self.builder(
+            *self.topics,
+            group_id=self.group_id,
+            client_id=self.client_id,
+            **self.__connection_args,
+        )
+        await consumer.start()
 
         await super().start()
 
+        self.task = asyncio.create_task(self._consume())
+
     async def close(self) -> None:
-        """Clean up handler subscription, cancel consume task in graceful mode."""
         await super().close()
 
-        if self.subscription is not None:
-            await self.subscription.unsubscribe()
-            self.subscription = None
+        if self.consumer is not None:
+            await self.consumer.stop()
+            self.consumer = None
 
-        if self.task is not None:
+        if self.task is not None and not self.task.done():
             self.task.cancel()
-            self.task = None
 
-    async def _consume_pull(
-        self,
-        cb: Callable[[Msg], Awaitable[SendableMessage]],
-        *,
-        task_status: TaskStatus[None] = anyio.TASK_STATUS_IGNORED,
-    ) -> None:
-        """Endless task consuming messages using NATS Pull subscriber."""
-        assert self.pull_sub  # nosec B101
+        self.task = None
 
-        sub = cast(JetStreamContext.PullSubscription, self.subscription)
+    def _make_response_publisher(
+        self, message: "StreamMessage[Any]"
+    ) -> Sequence[FakePublisher]:
+        if not message.reply_to or self._producer is None:
+            return ()
+
+        return (
+            FakePublisher(
+                self._producer.publish,
+                publish_kwargs={
+                    "topic": message.reply_to,
+                },
+            ),
+        )
+
+    @abstractmethod
+    async def get_msg(self) -> MsgType:
+        raise NotImplementedError()
+
+    async def _consume(self) -> None:
+        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+
+        connected = True
+        while self.running:
+            try:
+                msg = await self.get_msg()
+
+            except KafkaError:  # pragma: no cover
+                if connected:
+                    connected = False
+                await anyio.sleep(5)
+
+            except ConsumerStoppedError:
+                return
+
+            else:
+                if not connected:  # pragma: no cover
+                    connected = True
+
+                if msg:
+                    await self.consume(msg)
 
-        task_status.started()
+    @staticmethod
+    def get_routing_hash(topics: Iterable[str], group_id: Optional[str] = None) -> int:
+        return hash("".join((*topics, group_id or "")))
+
+    def __hash__(self) -> int:
+        return self.get_routing_hash(self.topics, self.group_id)
 
-        while self.running:  # pragma: no branch
-            with suppress(TimeoutError):
-                messages = await sub.fetch(
-                    batch=self.pull_sub.batch_size,
-                    timeout=self.pull_sub.timeout,
-                )
-
-                if messages:
-                    if self.pull_sub.batch:
-                        await self.consume(messages)  # type: ignore[arg-type]
-
-                    else:
-                        async with anyio.create_task_group() as tg:
-                            for msg in messages:
-                                tg.start_soon(cb, msg)
+    @staticmethod
+    def build_log_context(
+        message: Optional["StreamMessage[Any]"],
+        topic: str,
+        group_id: Optional[str] = None,
+    ) -> Dict[str, str]:
+        return {
+            "topic": topic,
+            "group_id": group_id or "",
+            "message_id": getattr(message, "message_id", ""),
+        }
 
-    async def _serve_consume_queue(
+    def get_log_context(
         self,
-        *,
-        task_status: TaskStatus[None] = anyio.TASK_STATUS_IGNORED,
+        message: Optional["StreamMessage[ConsumerRecord]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topics)
+        elif isinstance(message.raw_message, Sequence):
+            topic = message.raw_message[0].topic
+        else:
+            topic = message.raw_message.topic
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
+
+    def add_prefix(self, prefix: str) -> None:
+        self.topics = tuple(
+            "".join((prefix, t))
+            for t in self.topics
+        )
+
+class DefaultSubscriber(LogicSubscriber[ConsumerRecord]):
+    def __init__(
+        self,
+        *topics: str,
+        # Kafka information
+        group_id: Optional[str],
+        builder: Callable[..., AIOKafkaConsumer],
+        is_manual: bool,
+        # Subscriber args
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[ConsumerRecord]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Endless task consuming messages from in-memory queue.
+        super().__init__(
+            *topics,
+            group_id=group_id,
+            builder=builder,
+            is_manual=is_manual,
+            # subscriber args
+            default_parser=AioKafkaParser.parse_message,
+            default_decoder=AioKafkaParser.decode_message,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
 
-        Suitable to batch messages by amount, timestamps, etc and call `consume` for this batches.
-        """
-        async with anyio.create_task_group() as tg:
-            task_status.started()
+    async def get_msg(self) -> ConsumerRecord:
+        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+        return await self.consumer.getone()
 
-            async for msg in self.receive_stream:
-                tg.start_soon(self.__consume_msg, msg)
 
-    async def __consume_msg(
+class BatchSubscriber(LogicSubscriber[Tuple[ConsumerRecord, ...]]):
+    def __init__(
         self,
-        msg: Msg,
+        *topics: str,
+        batch_timeout_ms: int,
+        max_records: Optional[int],
+        # Kafka information
+        group_id: Optional[str],
+        builder: Callable[..., AIOKafkaConsumer],
+        is_manual: bool,
+        # Subscriber args
+        no_ack: bool,
+        retry: bool,
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Proxy method to call `self.consume` with semaphore block."""
-        async with self.limiter:
-            await self.consume(msg)
-
-    async def __put_msg(self, msg: Msg) -> None:
-        """Proxy method to put msg into in-memory queue with semaphore block."""
-        async with self.limiter:
-            await self.send_stream.send(msg)
+        self.batch_timeout_ms = batch_timeout_ms
+        self.max_records = max_records
 
-    @staticmethod
-    def get_routing_hash(
-        subject: Annotated[str, Doc("NATS subject to consume messages")],
-    ) -> str:
-        """Get handler hash by outer data.
-
-        Using to find handler in `broker.handlers` dictionary.
-        """
-        return subject
+        super().__init__(
+            *topics,
+            group_id=group_id,
+            builder=builder,
+            is_manual=is_manual,
+            # subscriber args
+            default_parser=AioKafkaParser.parse_message_batch,
+            default_decoder=AioKafkaParser.decode_message_batch,
+            # Propagated args
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI args
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
+        )
+
+    async def get_msg(self) -> Tuple[ConsumerRecord, ...]:
+        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+
+        messages = await self.consumer.getmany(
+            timeout_ms=self.batch_timeout_ms,
+            max_records=self.max_records,
+        )
+
+        if not messages:  # pragma: no cover
+            await anyio.sleep(self.batch_timeout_ms / 1000)
+            return ()
+
+        return tuple(chain(*messages.values()))
```

### Comparing `faststream-0.4.7/faststream/nats/helpers.py` & `faststream-0.5.0rc0/faststream/nats/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from typing import Any, Dict, Optional, Union
+from typing import Dict, Optional, Union
 
-from faststream.nats.js_stream import JStream
+from faststream.nats.schemas.js_stream import JStream
 
 
 class StreamBuilder:
     """A class to build streams."""
 
     streams: Dict[str, JStream]
 
     def __init__(self) -> None:
         """Initialize the stream builder."""
         self.streams = {}
 
     def stream(
         self,
         name: Union[str, JStream, None],
-        *args: Any,
-        declare: bool = True,
-        **kwargs: Any,
     ) -> Optional[JStream]:
         """Get a stream.
 
         Args:
             *args: The arguments.
             name: The stream name.
             declare: Whether to declare the stream.
```

### Comparing `faststream-0.4.7/faststream/nats/parser.py` & `faststream-0.5.0rc0/faststream/confluent/publisher/producer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,111 @@
-from typing import TYPE_CHECKING, List, Optional, Union, overload
-from uuid import uuid4
+from typing import Dict, Optional
 
-from nats.aio.msg import Msg
+from typing_extensions import override
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.parsers import decode_message
-from faststream.nats.message import NatsMessage
-from faststream.types import AnyDict, DecodedMessage
-from faststream.utils.context.repository import context
-
-if TYPE_CHECKING:
-    from faststream.nats.asyncapi import Handler
-
-
-class NatsParser:
-    """A class to parse NATS messages."""
-
-    def __init__(self, is_js: bool) -> None:
-        """Initialize the NATS parser.
-
-        Args:
-            is_js: Whether the parser is for JetStream.
-        """
-        self.is_js = is_js
-
-    @overload
-    async def parse_message(
-        self, message: List[Msg], *, path: Optional[AnyDict] = None
-    ) -> StreamMessage[List[Msg]]: ...
-
-    @overload
-    async def parse_message(
-        self, message: Msg, *, path: Optional[AnyDict] = None
-    ) -> StreamMessage[Msg]: ...
-
-    async def parse_message(
-        self, message: Union[Msg, List[Msg]], *, path: Optional[AnyDict] = None
-    ) -> Union[
-        StreamMessage[Msg],
-        StreamMessage[List[Msg]],
-    ]:
-        if isinstance(message, list):
-            return NatsMessage(
-                is_js=self.is_js,
-                raw_message=message,  # type: ignore[arg-type]
-                body=[m.data for m in message],
-            )
+from faststream.broker.message import encode_message
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.confluent.client import AsyncConfluentProducer
+from faststream.exceptions import NOT_CONNECTED_YET
+from faststream.types import SendableMessage
 
-        else:
-            handler: Optional["Handler"]
-            if (
-                path is None
-                and (handler := context.get_local("handler_")) is not None
-                and (path_re := handler.path_regex) is not None
-                and (match := path_re.match(message.subject)) is not None
-            ):
-                path = match.groupdict()
-
-            headers = message.header or {}
-
-            return NatsMessage(
-                is_js=self.is_js,
-                raw_message=message,
-                body=message.data,
-                path=path or {},
-                reply_to=headers.get("reply_to", "") if self.is_js else message.reply,
-                headers=headers,
-                content_type=headers.get("content-type", ""),
-                message_id=headers.get("message_id", str(uuid4())),
-                correlation_id=headers.get("correlation_id", str(uuid4())),
-            )
 
-    async def decode_message(
+class AsyncConfluentFastProducer(ProducerProto):
+    """A class to represent Kafka producer."""
+
+    _producer: Optional[AsyncConfluentProducer]
+
+    def __init__(
         self,
-        msg: Union[
-            StreamMessage[Msg],
-            StreamMessage[List[Msg]],
-        ],
-    ) -> Union[List[DecodedMessage], DecodedMessage]:
-        if isinstance(msg.raw_message, list):
-            data: List[DecodedMessage] = []
+        producer: AsyncConfluentProducer,
+    ) -> None:
+        self._producer = producer
 
-            path: Optional[AnyDict] = None
-            for m in msg.raw_message:
-                msg = await self.parse_message(m, path=path)
-                path = msg.path
+    @override
+    async def publish(  # type: ignore[override]
+        self,
+        message: SendableMessage,
+        topic: str,
+        *,
+        key: Optional[bytes] = None,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[Dict[str, str]] = None,
+        correlation_id: str = "",
+        reply_to: str = "",
+    ) -> None:
+        """Publish a message to a topic."""
+        assert self._producer, NOT_CONNECTED_YET  # nosec B101
+
+        message, content_type = encode_message(message)
+
+        headers_to_send = {
+            "content-type": content_type or "",
+            "correlation_id": correlation_id,
+            **(headers or {}),
+        }
+
+        if reply_to:
+            headers_to_send["reply_to"] = headers_to_send.get(
+                "reply_to",
+                reply_to,
+            )
 
-                data.append(decode_message(msg))
+        await self._producer.send(
+            topic=topic,
+            value=message,
+            key=key,
+            partition=partition,
+            timestamp_ms=timestamp_ms,
+            headers=[(i, (j or "").encode())
+                     for i, j in headers_to_send.items()],
+        )
+
+    async def stop(self) -> None:
+        if self._producer is not None:  # pragma: no branch
+            await self._producer.stop()
 
-            return data
+    async def publish_batch(
+        self,
+        *msgs: SendableMessage,
+        topic: str,
+        partition: Optional[int] = None,
+        timestamp_ms: Optional[int] = None,
+        headers: Optional[Dict[str, str]] = None,
+        reply_to: str = "",
+        correlation_id: str = "",
+    ) -> None:
+        """Publish a batch of messages to a topic."""
+        assert self._producer, NOT_CONNECTED_YET  # nosec B101
+
+        batch = self._producer.create_batch()
+
+        headers_to_send = {
+            "correlation_id": correlation_id,
+            **(headers or {})
+        }
+
+        if reply_to:
+            headers_to_send["reply_to"] = headers_to_send.get(
+                "reply_to",
+                reply_to,
+            )
 
-        else:
-            return decode_message(msg)
+        for msg in msgs:
+            message, content_type = encode_message(msg)
 
+            if content_type:
+                final_headers = {
+                    "content-type": content_type,
+                    **headers_to_send,
+                }
+            else:
+                final_headers = headers_to_send.copy()
+
+            batch.append(
+                key=None,
+                value=message,
+                timestamp=timestamp_ms,
+                headers=[(i, j.encode()) for i, j in final_headers.items()],
+            )
 
-JsParser = NatsParser(True)
-Parser = NatsParser(False)
+        await self._producer.send_batch(batch, topic, partition=partition)
```

### Comparing `faststream-0.4.7/faststream/nats/producer.py` & `faststream-0.5.0rc0/faststream/nats/publisher/producer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import asyncio
 from secrets import token_hex
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 from uuid import uuid4
 
 import nats
-from nats.aio.client import Client
-from nats.aio.msg import Msg
-from nats.js import JetStreamContext
-
-from faststream.broker.parsers import encode_message, resolve_custom_func
-from faststream.broker.types import (
-    AsyncCustomDecoder,
-    AsyncCustomParser,
-    AsyncDecoder,
-    AsyncParser,
-)
+from typing_extensions import override
+
+from faststream.broker.message import encode_message
+from faststream.broker.publisher.proto import ProducerProto
+from faststream.broker.utils import resolve_custom_func
 from faststream.exceptions import WRONG_PUBLISH_ARGS
-from faststream.nats.message import NatsMessage
-from faststream.nats.parser import Parser
+from faststream.nats.parser import NatsParser
 from faststream.types import SendableMessage
 from faststream.utils.functions import timeout_scope
 
+if TYPE_CHECKING:
+    from nats.aio.client import Client
+    from nats.aio.msg import Msg
+    from nats.js import JetStreamContext
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import (
+        AsyncDecoder,
+        AsyncParser,
+        CustomDecoder,
+        CustomParser,
+    )
+
 
-class NatsFastProducer:
+class NatsFastProducer(ProducerProto):
     """A class to represent a NATS producer."""
 
-    _connection: Client
-    _decoder: AsyncDecoder[Any]
-    _parser: AsyncParser[Msg, Any]
+    _decoder: "AsyncDecoder[StreamMessage[Msg]]"
+    _parser: "AsyncParser[Msg]"
 
     def __init__(
         self,
-        connection: Client,
-        parser: Optional[AsyncCustomParser[Msg, NatsMessage]],
-        decoder: Optional[AsyncCustomDecoder[NatsMessage]],
+        *,
+        connection: "Client",
+        parser: Optional["CustomParser[Msg]"],
+        decoder: Optional["CustomDecoder[StreamMessage[Msg]]"],
     ) -> None:
-        """Initialize the NATS producer.
-
-        Args:
-            connection: The NATS connection.
-            parser: The parser.
-            decoder: The decoder.
-        """
         self._connection = connection
-        self._parser = resolve_custom_func(parser, Parser.parse_message)
-        self._decoder = resolve_custom_func(decoder, Parser.decode_message)
+        self._parser = resolve_custom_func(parser, NatsParser.parse_message)
+        self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
 
-    async def publish(
+    @override
+    async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
         subject: str,
+        *,
+        correlation_id: str,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
-        correlation_id: Optional[str] = None,
-        *,
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[Any]:
         payload, content_type = encode_message(message)
 
         headers_to_send = {
             "content-type": content_type or "",
-            "correlation_id": correlation_id or str(uuid4()),
+            "correlation_id": correlation_id,
             **(headers or {}),
         }
 
         client = self._connection
 
         if rpc:
             if reply_to:
@@ -100,57 +100,51 @@
                     ):
                         raise nats.errors.NoRespondersError
                 return await self._decoder(await self._parser(msg))
 
         return None
 
 
-class NatsJSFastProducer:
+class NatsJSFastProducer(ProducerProto):
     """A class to represent a NATS JetStream producer."""
 
-    _connection: JetStreamContext
-    _decoder: AsyncDecoder[Any]
-    _parser: AsyncParser[Msg, Any]
+    _decoder: "AsyncDecoder[StreamMessage[Msg]]"
+    _parser: "AsyncParser[Msg]"
 
     def __init__(
         self,
-        connection: JetStreamContext,
-        parser: Optional[AsyncCustomParser[Msg, NatsMessage]],
-        decoder: Optional[AsyncCustomDecoder[NatsMessage]],
+        *,
+        connection: "JetStreamContext",
+        parser: Optional["CustomParser[Msg]"],
+        decoder: Optional["CustomDecoder[StreamMessage[Msg]]"],
     ) -> None:
-        """Initialize the NATS JetStream producer.
-
-        Args:
-            connection: The NATS JetStream connection.
-            parser: The parser.
-            decoder: The decoder.
-        """
         self._connection = connection
-        self._parser = resolve_custom_func(parser, Parser.parse_message)
-        self._decoder = resolve_custom_func(decoder, Parser.decode_message)
+        self._parser = resolve_custom_func(parser, NatsParser.parse_message)
+        self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
 
-    async def publish(
+    @override
+    async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         subject: str,
+        *,
+        correlation_id: str,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
-        correlation_id: Optional[str] = None,
         stream: Optional[str] = None,
         timeout: Optional[float] = None,
-        *,
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[Any]:
         payload, content_type = encode_message(message)
 
         headers_to_send = {
             "content-type": content_type or "",
-            "correlation_id": correlation_id or str(uuid4()),
+            "correlation_id": correlation_id,
             **(headers or {}),
         }
 
         if rpc:
             if reply_to:
                 raise WRONG_PUBLISH_ARGS
```

### Comparing `faststream-0.4.7/faststream/nats/security.py` & `faststream-0.5.0rc0/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/nats/test.py` & `faststream-0.5.0rc0/faststream/nats/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,58 @@
-from itertools import zip_longest
-from typing import Any, Dict, Optional, Union
-from uuid import uuid4
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from nats.aio.msg import Msg
 from typing_extensions import override
 
-from faststream.broker.parsers import encode_message
-from faststream.broker.test import TestBroker, call_handler
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.nats.asyncapi import Handler, Publisher
+from faststream.broker.message import encode_message, gen_cor_id
+from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.nats.broker import NatsBroker
-from faststream.nats.producer import NatsFastProducer
+from faststream.nats.publisher.producer import NatsFastProducer
+from faststream.nats.schemas.js_stream import is_subject_match_wildcard
+from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.testing.broker import TestBroker, call_handler
 from faststream.types import AnyDict, SendableMessage
 
+if TYPE_CHECKING:
+    from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
+
 __all__ = ("TestNatsBroker",)
 
 
 class TestNatsBroker(TestBroker[NatsBroker]):
     """A class to test NATS brokers."""
 
     @staticmethod
-    def patch_publisher(broker: NatsBroker, publisher: Any) -> None:
-        publisher._producer = broker._producer
-
-    @staticmethod
     def create_publisher_fake_subscriber(
         broker: NatsBroker,
-        publisher: Publisher,
+        publisher: "AsyncAPIPublisher",
     ) -> HandlerCallWrapper[Any, Any, Any]:
-        @broker.subscriber(publisher.subject, _raw=True)
-        def f(msg: Any) -> None:
-            pass
+        sub = broker.subscriber(publisher.subject)
+
+        if not sub.calls:
+
+            @sub
+            def f(msg: Any) -> None:
+                pass
 
-        return f
+            broker.setup_subscriber(sub)
+
+        return sub.calls[0].handler
 
     @staticmethod
     async def _fake_connect(broker: NatsBroker, *args: Any, **kwargs: Any) -> None:
         broker._js_producer = broker._producer = FakeProducer(broker)  # type: ignore[assignment]
 
     @staticmethod
     def remove_publisher_fake_subscriber(
-        broker: NatsBroker, publisher: Publisher
+        broker: NatsBroker, publisher: "AsyncAPIPublisher"
     ) -> None:
-        broker.handlers.pop(Handler.get_routing_hash(publisher.subject), None)
+        broker._subscribers.pop(
+            AsyncAPISubscriber.get_routing_hash(publisher.subject), None
+        )
 
 
 class FakeProducer(NatsFastProducer):
     def __init__(self, broker: NatsBroker) -> None:
         self.broker = broker
 
     @override
@@ -60,53 +66,37 @@
         # NatsJSFastProducer compatibility
         timeout: Optional[float] = None,
         stream: Optional[str] = None,
         *,
         rpc: bool = False,
         rpc_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> Optional[SendableMessage]:
+    ) -> Any:
         incoming = build_message(
             message=message,
             subject=subject,
             headers=headers,
             correlation_id=correlation_id,
             reply_to=reply_to,
         )
 
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            call = False
-
+        for handler in self.broker._subscribers.values():  # pragma: no branch
             if stream and getattr(handler.stream, "name", None) != stream:
                 continue
 
-            if subject == handler.subject:
-                call = True
-
-            else:
-                call = True
-
-                for current, base in zip_longest(
-                    subject.split("."),
-                    handler.subject.split("."),
-                    fillvalue=None,
-                ):
-                    if base == ">":
-                        break
-
-                    if base != "*" and current != base:
-                        call = False
-                        break
+            if is_subject_match_wildcard(subject, handler.subject):
+                msg: Union[List[PatchedMessage], PatchedMessage]
+                if getattr(handler.pull_sub, "batch", False):
+                    msg = [incoming]
+                else:
+                    msg = incoming
 
-            if call:
                 r = await call_handler(
                     handler=handler,
-                    message=[incoming]
-                    if getattr(handler.pull_sub, "batch", False)
-                    else incoming,
+                    message=msg,
                     rpc=rpc,
                     rpc_timeout=rpc_timeout,
                     raise_timeout=raise_timeout,
                 )
 
                 if rpc:
                     return r
@@ -126,15 +116,15 @@
     return PatchedMessage(
         _client=None,  # type: ignore
         subject=subject,
         reply=reply_to,
         data=msg,
         headers={
             "content-type": content_type or "",
-            "correlation_id": correlation_id or str(uuid4()),
+            "correlation_id": correlation_id or gen_cor_id(),
             **(headers or {}),
         },
     )
 
 
 class PatchedMessage(Msg):
     async def ack(self) -> None:
```

### Comparing `faststream-0.4.7/faststream/nats/shared/logging.py` & `faststream-0.5.0rc0/faststream/confluent/broker/logging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,70 @@
 import logging
-from typing import Any, Optional
+from inspect import Parameter
+from typing import Any, ClassVar, Optional, Tuple, Union
 
-from typing_extensions import override
+import confluent_kafka
 
-from faststream.broker.core.mixins import LoggingMixin
-from faststream.broker.message import StreamMessage
-from faststream.log import access_logger
-from faststream.types import AnyDict
-
-
-class NatsLoggingMixin(LoggingMixin):
-    """A class to represent a NATS logging mixin."""
-
-    _max_queue_len: int
-    _max_subject_len: int
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.confluent.schemas.params import ConsumerConnectionParams
+from faststream.log.logging import get_broker_logger
+
+
+class KafkaLoggingBroker(BrokerUsecase[
+    Union[
+        confluent_kafka.Message,
+        Tuple[confluent_kafka.Message, ...]
+    ],
+    ConsumerConnectionParams,
+]):
+    """A class that extends the LoggingMixin class and adds additional functionality for logging Kafka related information."""
+
+    _max_topic_len: int
+    _max_group_len: int
+    __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
+        logger: Union[logging.Logger, object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize the NATS logging mixin.
-
-        Args:
-            *args: The arguments.
-            logger: The logger.
-            log_level: The log level.
-            log_fmt: The log format.
-            **kwargs: The keyword arguments.
-        """
+        """Initialize the class."""
         super().__init__(
             *args,
             logger=logger,
+            # TODO: generate unique logger names to not share between brokers
+            default_logger=get_broker_logger(
+                name="confluent",
+                default_context={
+                    "topic": "",
+                    "group_id": "",
+                },
+                message_id_ln=self.__max_msg_id_ln,
+            ),
             log_level=log_level,
             log_fmt=log_fmt,
             **kwargs,
         )
-        self._max_queue_len = 0
-        self._max_stream_len = 0
-        self._max_subject_len = 4
+        self._max_topic_len = 4
+        self._max_group_len = 0
 
-    @override
-    def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[StreamMessage[Any]],
-        subject: str,
-        queue: str = "",
-        stream: str = "",
-    ) -> AnyDict:
-        return {
-            "subject": subject,
-            "queue": queue,
-            "stream": stream,
-            **super()._get_log_context(message),
-        }
-
-    @property
-    def fmt(self) -> str:
-        return self._fmt or (
-            "%(asctime)s %(levelname)s - "
-            + (f"%(stream)-{self._max_stream_len}s | " if self._max_stream_len else "")
-            + (f"%(queue)-{self._max_queue_len}s | " if self._max_queue_len else "")
-            + f"%(subject)-{self._max_subject_len}s | "
-            + f"%(message_id)-{self._message_id_ln}s "
-            "- %(message)s"
+    def get_fmt(self) -> str:
+        return (
+            "%(asctime)s %(levelname)-8s - "
+            + f"%(topic)-{self._max_topic_len}s | "
+            + (f"%(group_id)-{self._max_group_len}s | " if self._max_group_len else "")
+            + f"%(message_id)-{self.__max_msg_id_ln}s "
+            + "- %(message)s"
         )
 
     def _setup_log_context(
         self,
-        queue: Optional[str] = None,
-        subject: Optional[str] = None,
-        stream: Optional[str] = None,
+        *,
+        topic: str = "",
+        group_id: Optional[str] = None,
     ) -> None:
-        self._max_subject_len = max((self._max_subject_len, len(subject or "")))
-        self._max_queue_len = max((self._max_queue_len, len(queue or "")))
-        self._max_stream_len = max((self._max_stream_len, len(stream or "")))
+        """Set up log context."""
+        self._max_topic_len = max((self._max_topic_len, len(topic)))
+        self._max_group_len = max((self._max_group_len, len(group_id or "")))
```

### Comparing `faststream-0.4.7/faststream/rabbit/annotations.py` & `faststream-0.5.0rc0/faststream/rabbit/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
 from faststream.rabbit.broker import RabbitBroker as RB
 from faststream.rabbit.message import RabbitMessage as RM
-from faststream.rabbit.producer import AioPikaFastProducer
+from faststream.rabbit.publisher.producer import AioPikaFastProducer
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
     "RabbitMessage",
```

### Comparing `faststream-0.4.7/faststream/rabbit/handler.py` & `faststream-0.5.0rc0/faststream/rabbit/subscriber/usecase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,150 @@
-from typing import Any, Callable, Dict, Optional, Sequence
+from copy import deepcopy
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Sequence,
+    Union,
+)
 
-import aio_pika
-from fast_depends.core import CallModel
+from aio_pika import IncomingMessage, RobustQueue
+from fast_depends.dependencies import Depends
 from typing_extensions import override
 
-from faststream.broker.handler import AsyncHandler
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.parsers import resolve_custom_func
-from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-)
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.rabbit.helpers import RabbitDeclarer
-from faststream.rabbit.message import RabbitMessage
+from faststream.broker.publisher.fake import FakePublisher
+from faststream.broker.subscriber.usecase import SubscriberUsecase
+from faststream.broker.types import BrokerMiddleware, CustomDecoder, CustomParser
+from faststream.exceptions import SetupError
 from faststream.rabbit.parser import AioPikaParser
-from faststream.rabbit.shared.schemas import (
+from faststream.rabbit.publisher.producer import AioPikaFastProducer
+from faststream.rabbit.schemas import (
     BaseRMQInformation,
     RabbitExchange,
     RabbitQueue,
+    ReplyConfig,
 )
-from faststream.types import AnyDict
-
+from faststream.rabbit.utils import RabbitDeclarer
+from faststream.types import AnyDict, LoggerProto
 
-class LogicHandler(AsyncHandler[aio_pika.IncomingMessage], BaseRMQInformation):
-    """A class to handle logic for RabbitMQ message consumption.
 
-    Attributes:
-        queue : RabbitQueue object representing the queue to consume from
-        exchange : Optional RabbitExchange object representing the exchange to bind the queue to
-        consume_args : Additional arguments to pass when consuming from the queue
-        _consumer_tag : Optional string representing the consumer tag
-        _queue_obj : Optional aio_pika.RobustQueue object representing the declared queue
-
-    Methods:
-        __init__ : Initializes the LogicHandler object
-        add_call : Adds a call to be handled by the LogicHandler
-        start : Starts consuming messages from the queue
-        close : Closes the consumer and cancels message consumption
-
-    """
-
-    queue: RabbitQueue
-    exchange: Optional[RabbitExchange]
-    consume_args: AnyDict
+class LogicSubscriber(
+    SubscriberUsecase[IncomingMessage],
+    BaseRMQInformation,
+):
+    """A class to handle logic for RabbitMQ message consumption."""
+    app_id: Optional[str]
+    declarer: Optional[RabbitDeclarer]
 
     _consumer_tag: Optional[str]
-    _queue_obj: Optional[aio_pika.RobustQueue]
+    _queue_obj: Optional[RobustQueue]
+    _producer: Optional[AioPikaFastProducer]
 
     def __init__(
         self,
+        *,
         queue: RabbitQueue,
-        log_context_builder: Callable[[StreamMessage[Any]], Dict[str, str]],
-        graceful_timeout: Optional[float] = None,
-        # RMQ information
-        exchange: Optional[RabbitExchange] = None,
-        consume_args: Optional[AnyDict] = None,
-        # AsyncAPI information
-        description: Optional[str] = None,
-        title: Optional[str] = None,
-        include_in_schema: bool = True,
-        virtual_host: str = "/",
+        exchange: Optional[RabbitExchange],
+        consume_args: Optional[AnyDict],
+        reply_config: Optional[ReplyConfig],
+        # Subscriber args
+        no_ack: bool,
+        retry: Union[bool, int],
+        broker_dependencies: Iterable[Depends],
+        broker_middlewares: Iterable[BrokerMiddleware[IncomingMessage]],
+        # AsyncAPI args
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
     ) -> None:
-        """Initialize a RabbitMQ consumer.
-
-        Args:
-            queue: RabbitQueue object representing the queue to consume from
-            log_context_builder: Callable that returns a dictionary with log context information
-            graceful_timeout: Optional float representing the graceful timeout
-            exchange: RabbitExchange object representing the exchange to bind the queue to (optional)
-            consume_args: Additional arguments for consuming from the queue (optional)
-            description: Description of the consumer (optional)
-            title: Title of the consumer (optional)
-            include_in_schema: Whether to include the consumer in the API specification (optional)
-            virtual_host: Virtual host to connect to (optional)
-
-        """
         super().__init__(
-            log_context_builder=log_context_builder,
-            description=description,
-            title=title,
+            default_parser=AioPikaParser.parse_message,
+            default_decoder=AioPikaParser.decode_message,
+            # Propagated options
+            no_ack=no_ack,
+            retry=retry,
+            broker_middlewares=broker_middlewares,
+            broker_dependencies=broker_dependencies,
+            # AsyncAPI
+            title_=title_,
+            description_=description_,
             include_in_schema=include_in_schema,
-            graceful_timeout=graceful_timeout,
         )
 
-        self.queue = queue
-        self.exchange = exchange
-        self.virtual_host = virtual_host
         self.consume_args = consume_args or {}
+        self.reply_config = reply_config.to_dict() if reply_config else {}
 
         self._consumer_tag = None
         self._queue_obj = None
 
-    def add_call(
+        # BaseRMQInformation
+        self.queue = queue
+        self.exchange = exchange
+        # Setup it later
+        self.app_id = None
+        self.virtual_host = ""
+        self.declarer = None
+
+    @override
+    def setup(  # type: ignore[override]
         self,
         *,
-        handler: HandlerCallWrapper[
-            aio_pika.IncomingMessage, P_HandlerParams, T_HandlerReturn
-        ],
-        dependant: CallModel[P_HandlerParams, T_HandlerReturn],
-        parser: Optional[CustomParser[aio_pika.IncomingMessage, RabbitMessage]],
-        decoder: Optional[CustomDecoder[RabbitMessage]],
-        filter: Filter[RabbitMessage],
-        middlewares: Optional[
-            Sequence[Callable[[aio_pika.IncomingMessage], BaseMiddleware]]
-        ],
+        app_id: Optional[str],
+        virtual_host: str,
+        declarer: RabbitDeclarer,
+        # basic args
+        logger: Optional["LoggerProto"],
+        producer: Optional["AioPikaFastProducer"],
+        graceful_timeout: Optional[float],
+        extra_context: Optional["AnyDict"],
+        # broker options
+        broker_parser: Optional["CustomParser[IncomingMessage]"],
+        broker_decoder: Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+        # dependant args
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
-        """Add a call to the handler.
+        self.app_id = app_id
+        self.virtual_host = virtual_host
+        self.declarer = declarer
 
-        Args:
-            handler: The handler for the call.
-            dependant: The dependant for the call.
-            parser: Optional custom parser for the call.
-            decoder: Optional custom decoder for the call.
-            filter: The filter for the call.
-            middlewares: Optional sequence of middlewares for the call.
-
-        Returns:
-            None
-
-        """
-        super().add_call(
-            handler=handler,
-            parser=resolve_custom_func(parser, AioPikaParser.parse_message),
-            decoder=resolve_custom_func(decoder, AioPikaParser.decode_message),
-            filter=filter,  # type: ignore[arg-type]
-            dependant=dependant,
-            middlewares=middlewares,
+        super().setup(
+            logger=logger,
+            producer=producer,
+            graceful_timeout=graceful_timeout,
+            extra_context=extra_context,
+            broker_parser=broker_parser,
+            broker_decoder=broker_decoder,
+            apply_types=apply_types,
+            is_validate=is_validate,
+            _get_dependant=_get_dependant,
         )
 
     @override
-    async def start(self, declarer: RabbitDeclarer) -> None:  # type: ignore[override]
-        """Starts the consumer for the RabbitMQ queue.
-
-        Args:
-            declarer: RabbitDeclarer object used to declare the queue and exchange
-
-        Returns:
-            None
+    async def start(self) -> None:
+        """Starts the consumer for the RabbitMQ queue."""
+        if self.declarer is None:
+            raise SetupError("You should setup subscriber at first.")
 
-        """
-        self._queue_obj = queue = await declarer.declare_queue(self.queue)
+        self._queue_obj = queue = await self.declarer.declare_queue(self.queue)
 
         if self.exchange is not None:
-            exchange = await declarer.declare_exchange(self.exchange)
-            await queue.bind(
-                exchange,
-                routing_key=self.queue.routing,
-                arguments=self.queue.bind_arguments,
-            )
+            exchange = await self.declarer.declare_exchange(self.exchange)
+            if not queue.passive:
+                await queue.bind(
+                    exchange,
+                    routing_key=self.queue.routing,
+                    arguments=self.queue.bind_arguments,
+                    timeout=self.queue.timeout,
+                    robust=self.queue.robust,
+                )
 
         self._consumer_tag = await queue.consume(
             # NOTE: aio-pika expects AbstractIncomingMessage, not IncomingMessage
             self.consume,  # type: ignore[arg-type]
             arguments=self.consume_args,
         )
 
@@ -166,8 +154,66 @@
         await super().close()
 
         if self._queue_obj is not None:
             if self._consumer_tag is not None:  # pragma: no branch
                 if not self._queue_obj.channel.is_closed:
                     await self._queue_obj.cancel(self._consumer_tag)
                 self._consumer_tag = None
+
             self._queue_obj = None
+
+    def _make_response_publisher(
+        self,
+        message: StreamMessage[Any],
+    ) -> Sequence[FakePublisher]:
+        if not message.reply_to or self._producer is None:
+            return ()
+
+        return (
+            FakePublisher(
+                self._producer.publish,
+                publish_kwargs={
+                    **self.reply_config,
+                    "routing_key": message.reply_to,
+                    "app_id": self.app_id,
+                },
+            ),
+        )
+
+    def __hash__(self) -> int:
+        return self.get_routing_hash(self.queue, self.exchange)
+
+    @staticmethod
+    def get_routing_hash(
+        queue: RabbitQueue,
+        exchange: Optional[RabbitExchange] = None,
+    ) -> int:
+        """Calculate the routing hash for a RabbitMQ queue and exchange."""
+        return hash(queue) + hash(exchange or "")
+
+    @staticmethod
+    def build_log_context(
+        message: Optional["StreamMessage[Any]"],
+        queue: RabbitQueue,
+        exchange: Optional[RabbitExchange] = None,
+    ) -> Dict[str, str]:
+        return {
+            "queue": queue.name,
+            "exchange": getattr(exchange, "name", ""),
+            "message_id": getattr(message, "message_id", ""),
+        }
+
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[Any]"],
+    ) -> Dict[str, str]:
+        return self.build_log_context(
+            message=message,
+            queue=self.queue,
+            exchange=self.exchange,
+        )
+
+    def add_prefix(self, prefix: str) -> None:
+        """Include Subscriber in router."""
+        new_q = deepcopy(self.queue)
+        new_q.name = "".join((prefix, new_q.name))
+        self.queue = new_q
```

### Comparing `faststream-0.4.7/faststream/rabbit/security.py` & `faststream-0.5.0rc0/faststream/rabbit/security.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     BaseSecurity,
     SASLPlaintext,
 )
 from faststream.types import AnyDict
 
 
 def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+    """Convert security object to connection arguments."""
     if security is None:
         return {}
     elif isinstance(security, SASLPlaintext):
         return _parse_sasl_plaintext(security)
     elif isinstance(security, BaseSecurity):
         return _parse_base_security(security)
     else:
```

### Comparing `faststream-0.4.7/faststream/rabbit/test.py` & `faststream-0.5.0rc0/faststream/rabbit/router.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,321 +1,337 @@
-from typing import Any, Optional, Union
-from unittest.mock import AsyncMock
-from uuid import uuid4
-
-import aiormq
-from aio_pika.message import IncomingMessage
-from pamqp import commands as spec
-from pamqp.header import ContentHeader
-
-from faststream.broker.test import TestBroker, call_handler
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.rabbit.asyncapi import Publisher
-from faststream.rabbit.broker import RabbitBroker
-from faststream.rabbit.parser import AioPikaParser
-from faststream.rabbit.producer import AioPikaFastProducer
-from faststream.rabbit.shared.constants import ExchangeType
-from faststream.rabbit.shared.schemas import (
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+
+from typing_extensions import Annotated, Doc, deprecated
+
+from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
+from faststream.broker.utils import default_filter
+from faststream.rabbit.broker.registrator import RabbitRegistrator
+from faststream.rabbit.schemas import (
     RabbitExchange,
     RabbitQueue,
 )
-from faststream.rabbit.shared.types import TimeoutType
-from faststream.rabbit.types import AioPikaSendableMessage
-from faststream.types import SendableMessage
-
-__all__ = ("TestRabbitBroker",)
-
-
-class TestRabbitBroker(TestBroker[RabbitBroker]):
-    """A class to test RabbitMQ brokers."""
-
-    @classmethod
-    def _patch_test_broker(cls, broker: RabbitBroker) -> None:
-        broker._channel = AsyncMock()
-        broker.declarer = AsyncMock()
-        super()._patch_test_broker(broker)
-
-    @staticmethod
-    async def _fake_connect(broker: RabbitBroker, *args: Any, **kwargs: Any) -> None:
-        broker._producer = FakeProducer(broker)
-
-    @staticmethod
-    def patch_publisher(broker: RabbitBroker, publisher: Any) -> None:
-        publisher._producer = broker._producer
-
-    @staticmethod
-    def create_publisher_fake_subscriber(
-        broker: RabbitBroker,
-        publisher: Publisher,
-    ) -> HandlerCallWrapper[Any, Any, Any]:
-        @broker.subscriber(
-            queue=publisher.queue,
-            exchange=publisher.exchange,
-            _raw=True,
-        )
-        def f(msg: Any) -> None:
-            pass
-
-        return f
-
-    @staticmethod
-    def remove_publisher_fake_subscriber(
-        broker: RabbitBroker,
-        publisher: Publisher,
-    ) -> None:
-        broker.handlers.pop(
-            publisher._get_routing_hash(),
-            None,
-        )
-
-
-class PatchedMessage(IncomingMessage):
-    """Patched message class for testing purposes.
 
-    This class extends aio_pika's IncomingMessage class and is used to simulate RabbitMQ message handling during tests.
-    """
-
-    async def ack(self, multiple: bool = False) -> None:
-        """Asynchronously acknowledge a message.
-
-        Args:
-            multiple (bool, optional): Whether to acknowledge multiple messages at once. Defaults to False.
-
-        Returns:
-            None
-        """
-        pass
-
-    async def nack(self, multiple: bool = False, requeue: bool = True) -> None:
-        """Nack the message.
-
-        Args:
-            multiple: Whether to nack multiple messages. Default is False.
-            requeue: Whether to requeue the message. Default is True.
-
-        Returns:
-            None
-        """
-        pass
-
-    async def reject(self, requeue: bool = False) -> None:
-        """Rejects a task.
-
-        Args:
-            requeue: Whether to requeue the task if it fails (default: False)
-
-        Returns:
-            None
-        """
-        pass
-
-
-def build_message(
-    message: AioPikaSendableMessage = "",
-    queue: Union[RabbitQueue, str] = "",
-    exchange: Union[RabbitExchange, str, None] = None,
-    *,
-    routing_key: str = "",
-    reply_to: Optional[str] = None,
-    **message_kwargs: Any,
-) -> PatchedMessage:
-    """Build a patched RabbitMQ message for testing.
-
-    Args:
-        message (AioPikaSendableMessage): The message content.
-        queue (Union[RabbitQueue, str]): The message queue.
-        exchange (Union[RabbitExchange, str, None]): The message exchange.
-        routing_key (str): The message routing key.
-        reply_to (Optional[str]): The reply-to queue.
-        **message_kwargs (Any): Additional message arguments.
-
-    Returns:
-        PatchedMessage: A patched RabbitMQ message.
-    """
-    que = RabbitQueue.validate(queue)
-    exch = RabbitExchange.validate(exchange)
-    msg = AioPikaParser.encode_message(
-        message=message,
-        persist=False,
-        reply_to=reply_to,
-        callback_queue=None,
-        **message_kwargs,
+if TYPE_CHECKING:
+    from aio_pika.abc import DateType, HeadersType, TimeoutType
+    from aio_pika.message import IncomingMessage
+    from broker.types import PublisherMiddleware
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomDecoder,
+        CustomParser,
+        Filter,
+        SubscriberMiddleware,
     )
+    from faststream.rabbit.schemas.reply import ReplyConfig
+    from faststream.rabbit.types import AioPikaSendableMessage
+    from faststream.types import AnyDict
 
-    routing = routing_key or (getattr(que, "name", ""))
-
-    return PatchedMessage(
-        aiormq.abc.DeliveredMessage(
-            delivery=spec.Basic.Deliver(
-                exchange=getattr(exch, "name", ""),
-                routing_key=routing,
-            ),
-            header=ContentHeader(
-                properties=spec.Basic.Properties(
-                    content_type=msg.content_type,
-                    message_id=str(uuid4()),
-                    headers=msg.headers,
-                    reply_to=reply_to,
-                )
-            ),
-            body=msg.body,
-            channel=AsyncMock(),
-        )
-    )
 
+class RabbitPublisher(ArgsContainer):
+    """Delayed RabbitPublisher registration object.
 
-class FakeProducer(AioPikaFastProducer):
-    """A fake RabbitMQ producer for testing purposes.
-
-    This class extends AioPikaFastProducer and is used to simulate RabbitMQ message publishing during tests.
+    Just a copy of `RabbitRegistrator.publisher(...)` arguments.
     """
 
-    def __init__(self, broker: RabbitBroker) -> None:
-        """Initialize a FakeProducer instance.
-
-        Args:
-            broker (RabbitBroker): The RabbitBroker instance to be used for message publishing.
-        """
-        self.broker = broker
-
-    async def publish(
+    def __init__(
         self,
-        message: AioPikaSendableMessage = "",
-        queue: Union[RabbitQueue, str] = "",
-        exchange: Union[RabbitExchange, str, None] = None,
+        queue: Annotated[
+            Union[RabbitQueue, str],
+            Doc("Default message routing key to publish with."),
+        ] = "",
+        exchange: Annotated[
+            Union[RabbitExchange, str, None],
+            Doc("Target exchange to publish message to."),
+        ] = None,
         *,
-        routing_key: str = "",
-        mandatory: bool = True,
-        immediate: bool = False,
-        timeout: TimeoutType = None,
-        rpc: bool = False,
-        rpc_timeout: Optional[float] = 30.0,
-        raise_timeout: bool = False,
-        persist: bool = False,
-        reply_to: Optional[str] = None,
-        **message_kwargs: Any,
-    ) -> Optional[SendableMessage]:
-        """Publish a message to a RabbitMQ queue or exchange.
-
-        Args:
-            message (AioPikaSendableMessage, optional): The message to be published.
-            queue (Union[RabbitQueue, str], optional): The target queue for the message.
-            exchange (Union[RabbitExchange, str, None], optional): The target exchange for the message.
-            routing_key (str, optional): The routing key for the message.
-            mandatory (bool, optional): Whether the message is mandatory.
-            immediate (bool, optional): Whether the message should be sent immediately.
-            timeout (TimeoutType, optional): The timeout for the message.
-            rpc (bool, optional): Whether the message is for RPC.
-            rpc_timeout (float, optional): The RPC timeout.
-            raise_timeout (bool, optional): Whether to raise a timeout exception.
-            persist (bool, optional): Whether to persist the message.
-            reply_to (str, optional): The reply-to address for RPC messages.
-            **message_kwargs (Any): Additional message properties and content.
-
-        Returns:
-            Optional[SendableMessage]: The published message if successful, or None if not.
-        """
-        exch = RabbitExchange.validate(exchange)
-
-        incoming = build_message(
-            message=message,
+        routing_key: Annotated[
+            str,
+            Doc(
+                "Default message routing key to publish with. "
+                "Overrides `queue` option if presented."
+            ),
+        ] = "",
+        mandatory: Annotated[
+            bool,
+            Doc(
+                "Client waits for confirmation that the message is placed to some queue. "
+                "RabbitMQ returns message to client if there is no suitable queue."
+            ),
+        ] = True,
+        immediate: Annotated[
+            bool,
+            Doc(
+                "Client expects that there is consumer ready to take the message to work. "
+                "RabbitMQ returns message to client if there is no suitable consumer."
+            ),
+        ] = False,
+        timeout: Annotated[
+            "TimeoutType",
+            Doc("Send confirmation time from RabbitMQ."),
+        ] = None,
+        persist: Annotated[
+            bool,
+            Doc("Restore the message on RabbitMQ reboot."),
+        ] = False,
+        reply_to: Annotated[
+            Optional[str],
+            Doc(
+                "Reply message routing key to send with (always sending to default exchange)."
+            ),
+        ] = None,
+        priority: Annotated[
+            Optional[int],
+            Doc("The message priority (0 by default)."),
+        ] = None,
+        # basic args
+        middlewares: Annotated[
+            Iterable["PublisherMiddleware"],
+            Doc("Publisher middlewares to wrap outgoing messages."),
+        ] = (),
+        # AsyncAPI args
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
+        # message args
+        headers: Annotated[
+            Optional["HeadersType"],
+            Doc(
+                "Message headers to store metainformation. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        content_type: Annotated[
+            Optional[str],
+            Doc(
+                "Message **content-type** header. "
+                "Used by application, not core RabbitMQ. "
+                "Will be setted automatically if not specified."
+            ),
+        ] = None,
+        content_encoding: Annotated[
+            Optional[str],
+            Doc("Message body content encoding, e.g. **gzip**."),
+        ] = None,
+        expiration: Annotated[
+            Optional["DateType"],
+            Doc("Message expiration (lifetime) in seconds (or datetime or timedelta)."),
+        ] = None,
+        message_type: Annotated[
+            Optional[str],
+            Doc("Application-specific message type, e.g. **orders.created**."),
+        ] = None,
+        user_id: Annotated[
+            Optional[str],
+            Doc("Publisher connection User ID, validated if set."),
+        ] = None,
+    ) -> None:
+        super().__init__(
             queue=queue,
-            exchange=exch,
+            exchange=exchange,
             routing_key=routing_key,
+            mandatory=mandatory,
+            immediate=immediate,
+            timeout=timeout,
+            persist=persist,
             reply_to=reply_to,
-            **message_kwargs,
+            priority=priority,
+            headers=headers,
+            content_type=content_type,
+            content_encoding=content_encoding,
+            expiration=expiration,
+            message_type=message_type,
+            user_id=user_id,
+            # basic args
+            middlewares=middlewares,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            schema=schema,
+            include_in_schema=include_in_schema,
         )
 
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            if handler.exchange == exch:
-                call: bool = False
-
-                if (
-                    handler.exchange is None
-                    or handler.exchange.type == ExchangeType.DIRECT
-                ):
-                    call = handler.queue.name == incoming.routing_key
-
-                elif handler.exchange.type == ExchangeType.FANOUT:
-                    call = True
 
-                elif handler.exchange.type == ExchangeType.TOPIC:
-                    call = apply_pattern(
-                        handler.queue.routing, incoming.routing_key or ""
-                    )
+class RabbitRoute(SubscriberRoute):
+    """Class to store delayed RabbitBroker subscriber registration.
 
-                elif handler.exchange.type == ExchangeType.HEADERS:  # pramga: no branch
-                    queue_headers = (handler.queue.bind_arguments or {}).copy()
-                    msg_headers = incoming.headers
-
-                    if not queue_headers:
-                        call = True
-
-                    else:
-                        matcher = queue_headers.pop("x-match", "all")
-
-                        full = True
-                        none = True
-                        for k, v in queue_headers.items():
-                            if msg_headers.get(k) != v:
-                                full = False
-                            else:
-                                none = False
-
-                        if not none:
-                            call = (matcher == "any") or full
-
-                else:  # pragma: no cover
-                    raise AssertionError("unreachable")
-
-                if call:
-                    r = await call_handler(
-                        handler=handler,
-                        message=incoming,
-                        rpc=rpc,
-                        rpc_timeout=rpc_timeout,
-                        raise_timeout=raise_timeout,
-                    )
-
-                    if rpc:  # pragma: no branch
-                        return r
-
-        return None
-
-
-def apply_pattern(pattern: str, current: str) -> bool:
-    """Apply a pattern to a routing key."""
-    pattern_queue = iter(pattern.split("."))
-    current_queue = iter(current.split("."))
-
-    pattern_symb = next(pattern_queue, None)
-    while pattern_symb:
-        if (next_symb := next(current_queue, None)) is None:
-            return False
-
-        elif pattern_symb == "#":
-            next_pattern = next(pattern_queue, None)
-
-            if next_pattern is None:
-                return True
-
-            if (next_symb := next(current_queue, None)) is None:
-                return False
-
-            while next_pattern == "*":
-                next_pattern = next(pattern_queue, None)
-                if (next_symb := next(current_queue, None)) is None:
-                    return False
-
-            while next_symb != next_pattern:
-                if (next_symb := next(current_queue, None)) is None:
-                    return False
+    Just a copy of `RabbitRegistrator.subscriber(...)` arguments.
+    """
 
-            pattern_symb = next(pattern_queue, None)
+    def __init__(
+        self,
+        call: Annotated[
+            Callable[..., "AioPikaSendableMessage"],
+            Doc(
+                "Message handler function "
+                "to wrap the same with `@broker.subscriber(...)` way."
+            ),
+        ],
+        queue: Annotated[
+            Union[str, RabbitQueue],
+            Doc(
+                "RabbitMQ queue to listen. "
+                "**FastStream** declares and binds queue object to `exchange` automatically if it is not passive (by default)."
+            ),
+        ],
+        exchange: Annotated[
+            Union[str, RabbitExchange, None],
+            Doc(
+                "RabbitMQ exchange to bind queue to. "
+                "Uses default exchange if not presented. "
+                "**FastStream** declares exchange object automatically if it is not passive (by default)."
+            ),
+        ] = None,
+        *,
+        publishers: Annotated[
+            Iterable[RabbitPublisher],
+            Doc("RabbitMQ publishers to broadcast the handler result."),
+        ] = (),
+        consume_args: Annotated[
+            Optional["AnyDict"],
+            Doc("Extra consumer arguments to use in `queue.consume(...)` method."),
+        ] = None,
+        reply_config: Annotated[
+            Optional["ReplyConfig"],
+            Doc("Extra options to use at replies publishing."),
+        ] = None,
+        # broker arguments
+        dependencies: Annotated[
+            Iterable["Depends"],
+            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
+        ] = (),
+        parser: Annotated[
+            Optional["CustomParser[IncomingMessage]"],
+            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        middlewares: Annotated[
+            Iterable["SubscriberMiddleware"],
+            Doc("Subscriber middlewares to wrap incoming message processing."),
+        ] = (),
+        filter: Annotated[
+            "Filter[StreamMessage[IncomingMessage]]",
+            Doc(
+                "Overload subscriber to consume various messages from the same source."
+            ),
+            deprecated(
+                "Deprecated in **FastStream 0.5.0**. "
+                "Please, create `subscriber` object and use it explicitly instead. "
+                "Argument will be removed in **FastStream 0.6.0**."
+            ),
+        ] = default_filter,
+        retry: Annotated[
+            Union[bool, int],
+            Doc("Whether to `nack` message at processing exception."),
+        ] = False,
+        no_ack: Annotated[
+            bool,
+            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
+        ] = False,
+        # AsyncAPI information
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI subscriber object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc(
+                "AsyncAPI subscriber object description. "
+                "Uses decorated docstring as default."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
+    ) -> None:
+        super().__init__(
+            call,
+            publishers=publishers,
+            queue=queue,
+            exchange=exchange,
+            consume_args=consume_args,
+            reply_config=reply_config,
+            dependencies=dependencies,
+            parser=parser,
+            decoder=decoder,
+            middlewares=middlewares,
+            filter=filter,
+            retry=retry,
+            no_ack=no_ack,
+            title=title,
+            description=description,
+            include_in_schema=include_in_schema,
+        )
 
-        elif pattern_symb == "*" or pattern_symb == next_symb:
-            pattern_symb = next(pattern_queue, None)
 
-        else:
-            return False
+class RabbitRouter(
+    BrokerRouter["IncomingMessage"],
+    RabbitRegistrator,
+):
+    """Includable to RabbitBroker router."""
 
-    return next(current_queue, None) is None
+    def __init__(
+        self,
+        prefix: Annotated[
+            str,
+            Doc("String prefix to add to all subscribers queues."),
+        ] = "",
+        handlers: Annotated[
+            Iterable[RabbitRoute],
+            Doc("Route object to include."),
+        ] = (),
+        *,
+        dependencies: Annotated[
+            Iterable["Depends"],
+            Doc(
+                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
+            ),
+        ] = (),
+        middlewares: Annotated[
+            Iterable["BrokerMiddleware[IncomingMessage]"],
+            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
+        ] = (),
+        parser: Annotated[
+            Optional["CustomParser[IncomingMessage]"],
+            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        include_in_schema: Annotated[
+            Optional[bool],
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = None,
+    ) -> None:
+        super().__init__(
+            handlers=handlers,
+            # basic args
+            prefix=prefix,
+            dependencies=dependencies,
+            middlewares=middlewares,
+            parser=parser,
+            decoder=decoder,
+            include_in_schema=include_in_schema,
+        )
```

### Comparing `faststream-0.4.7/faststream/rabbit/shared/constants.py` & `faststream-0.5.0rc0/faststream/rabbit/schemas/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from enum import Enum, unique
 
-RABBIT_REPLY = "amq.rabbitmq.reply-to"
-
 
 @unique
 class ExchangeType(str, Enum):
     """A class to represent the exchange type.
 
     Attributes:
         FANOUT : fanout exchange type
         DIRECT : direct exchange type
         TOPIC : topic exchange type
         HEADERS : headers exchange type
         X_DELAYED_MESSAGE : x-delayed-message exchange type
         X_CONSISTENT_HASH : x-consistent-hash exchange type
         X_MODULUS_HASH : x-modulus-hash exchange type
-
     """
 
     FANOUT = "fanout"
     DIRECT = "direct"
     TOPIC = "topic"
     HEADERS = "headers"
     X_DELAYED_MESSAGE = "x-delayed-message"
```

### Comparing `faststream-0.4.7/faststream/rabbit/shared/logging.py` & `faststream-0.5.0rc0/faststream/rabbit/broker/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,63 @@
 import logging
-from typing import Any, Optional
+from inspect import Parameter
+from typing import Any, ClassVar, Optional, Union
 
-from typing_extensions import override
+from aio_pika import IncomingMessage, RobustConnection
 
-from faststream.broker.core.mixins import LoggingMixin
-from faststream.broker.message import StreamMessage
-from faststream.log import access_logger
-from faststream.rabbit.shared.schemas import RabbitExchange, RabbitQueue
-from faststream.types import AnyDict
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.log.logging import get_broker_logger
 
 
-class RabbitLoggingMixin(LoggingMixin):
-    """A class that extends the LoggingMixin class and adds additional functionality for logging RabbitMQ related information.
-
-    Attributes:
-        _max_queue_len : maximum length of the queue name
-        _max_exchange_len : maximum length of the exchange name
-
-    Methods:
-        __init__ : Initializes the RabbitLoggingMixin object.
-        _get_log_context : Overrides the _get_log_context method of the LoggingMixin class to include RabbitMQ related context information.
-        fmt : Returns the log format string.
-        _setup_log_context : Sets up the log context by updating the maximum lengths of the queue and exchange names.
-
-    """
+class RabbitLoggingBroker(BrokerUsecase[IncomingMessage, RobustConnection]):
+    """A class that extends the LoggingMixin class and adds additional functionality for logging RabbitMQ related information."""
 
     _max_queue_len: int
     _max_exchange_len: int
+    __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
+        logger: Union[logging.Logger, object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize the class.
-
-        Args:
-            *args: Variable length argument list
-            logger: Optional logger object
-            log_level: Logging level
-            log_fmt: Optional log format
-            **kwargs: Arbitrary keyword arguments
-
-        Returns:
-            None
-
-        """
         super().__init__(
             *args,
             logger=logger,
+            # TODO: generate unique logger names to not share between brokers
+            default_logger=get_broker_logger(
+                name="rabbit",
+                default_context={
+                    "queue": "",
+                    "exchange": "",
+                },
+                message_id_ln=self.__max_msg_id_ln,
+            ),
             log_level=log_level,
             log_fmt=log_fmt,
             **kwargs,
         )
+
         self._max_queue_len = 4
         self._max_exchange_len = 4
 
-    @override
-    def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[StreamMessage[Any]],
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange] = None,
-    ) -> AnyDict:
-        """Get the log context.
-
-        Args:
-            message: Optional stream message.
-            queue: RabbitQueue object.
-            exchange: Optional RabbitExchange object.
-
-        Returns:
-            Dictionary containing the log context.
-
-        Note:
-            This is a private method and should not be called directly.
-
-        """
-        context = {
-            "queue": queue.name,
-            "exchange": exchange.name if exchange else "default",
-            **super()._get_log_context(message),
-        }
-        return context
-
-    @property
-    def fmt(self) -> str:
-        return super().fmt or (
-            "%(asctime)s %(levelname)s - "
+    def get_fmt(self) -> str:
+        return (
+            "%(asctime)s %(levelname)-8s - "
             f"%(exchange)-{self._max_exchange_len}s | "
             f"%(queue)-{self._max_queue_len}s | "
-            f"%(message_id)-{self._message_id_ln}s "
+            f"%(message_id)-{self.__max_msg_id_ln}s "
             "- %(message)s"
         )
 
     def _setup_log_context(
         self,
-        queue: Optional[RabbitQueue] = None,
-        exchange: Optional[RabbitExchange] = None,
+        *,
+        queue: Optional[str] = None,
+        exchange: Optional[str] = None,
     ) -> None:
-        """Set up log context.
-
-        Args:
-            queue: Optional RabbitQueue object representing the queue.
-            exchange: Optional RabbitExchange object representing the exchange.
-
-        Returns:
-            None
-
-        """
-        if exchange is not None:
-            self._max_exchange_len = max(
-                self._max_exchange_len, len(exchange.name or "")
-            )
-
-        if queue is not None:  # pragma: no branch
-            self._max_queue_len = max(self._max_queue_len, len(queue.name))
+        """Set up log context."""
+        self._max_exchange_len = max(self._max_exchange_len, len(exchange or ""))
+        self._max_queue_len = max(self._max_queue_len, len(queue or ""))
```

### Comparing `faststream-0.4.7/faststream/redis/annotations.py` & `faststream-0.5.0rc0/faststream/redis/annotations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from redis.asyncio.client import Redis as RedisClient
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
-from faststream.redis.broker import RedisBroker as RB
-from faststream.redis.message import RedisMessage as RM
+from faststream.broker.message import StreamMessage as BrokerStreamMessage
+from faststream.redis.broker.broker import RedisBroker as RB
+from faststream.redis.message import BaseMessage as BM
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
     "RedisMessage",
     "RedisBroker",
     "Redis",
 )
 
-RedisMessage = Annotated[RM, Context("message")]
+RedisMessage = Annotated[BrokerStreamMessage[BM], Context("message")]
 RedisBroker = Annotated[RB, Context("broker")]
 Redis = Annotated[RedisClient, Context("broker._connection")]
```

### Comparing `faststream-0.4.7/faststream/redis/broker.py` & `faststream-0.5.0rc0/faststream/confluent/router.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,342 +1,339 @@
-from functools import partial, wraps
-from types import TracebackType
 from typing import (
     Any,
-    AsyncContextManager,
-    Awaitable,
     Callable,
     Dict,
+    Iterable,
+    Literal,
     Optional,
     Sequence,
-    Type,
+    Tuple,
     Union,
 )
-from urllib.parse import urlparse
 
+from confluent_kafka import Message
 from fast_depends.dependencies import Depends
-from redis.asyncio.client import Redis
-from redis.asyncio.connection import ConnectionPool, parse_url
-from redis.exceptions import ResponseError
-from typing_extensions import TypeAlias, override
+from typing_extensions import Annotated, Doc, deprecated
 
-from faststream.broker.core.asynchronous import BrokerAsyncUsecase, default_filter
 from faststream.broker.message import StreamMessage
-from faststream.broker.middlewares import BaseMiddleware
+from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.types import (
-    AsyncPublisherProtocol,
+    BrokerMiddleware,
     CustomDecoder,
     CustomParser,
     Filter,
-    P_HandlerParams,
-    T_HandlerReturn,
-    WrappedReturn,
+    PublisherMiddleware,
+    SubscriberMiddleware,
 )
-from faststream.broker.wrapper import FakePublisher, HandlerCallWrapper
-from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.redis.asyncapi import Handler, Publisher
-from faststream.redis.message import AnyRedisDict, RedisMessage
-from faststream.redis.producer import RedisFastProducer
-from faststream.redis.schemas import INCORRECT_SETUP_MSG, ListSub, PubSub, StreamSub
-from faststream.redis.security import parse_security
-from faststream.redis.shared.logging import RedisLoggingMixin
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict, DecodedMessage
-from faststream.utils.context.repository import context
-
-Channel: TypeAlias = str
-
-
-class RedisBroker(
-    RedisLoggingMixin,
-    BrokerAsyncUsecase[AnyRedisDict, "Redis[bytes]"],
-):
-    """Redis broker."""
+from faststream.broker.utils import default_filter
+from faststream.confluent.broker.registrator import KafkaRegistrator
+from faststream.types import SendableMessage
+
 
-    url: str
-    handlers: Dict[int, Handler]
-    _publishers: Dict[int, Publisher]
+class KafkaPublisher(ArgsContainer):
+    """Delayed KafkaPublisher registration object.
 
-    _producer: Optional[RedisFastProducer]
+    Just a copy of `KafkaRegistrator.publisher(...)` arguments.
+    """
 
     def __init__(
         self,
-        url: str = "redis://localhost:6379",
-        polling_interval: Optional[float] = None,
+        topic: Annotated[
+            str,
+            Doc("Topic where the message will be published."),
+        ],
         *,
-        protocol: Optional[str] = None,
-        protocol_version: Optional[str] = "custom",
-        security: Optional[BaseSecurity] = None,
-        **kwargs: Any,
+        key: Annotated[
+            Union[bytes, Any, None],
+            Doc("""
+            A key to associate with the message. Can be used to
+            determine which partition to send the message to. If partition
+            is `None` (and producer's partitioner config is left as default),
+            then messages with the same key will be delivered to the same
+            partition (but if key is `None`, partition is chosen randomly).
+            Must be type `bytes`, or be serializable to bytes via configured
+            `key_serializer`.
+            """),
+        ] = None,
+        partition: Annotated[
+            Optional[int],
+            Doc("""
+            Specify a partition. If not set, the partition will be
+            selected using the configured `partitioner`.
+            """),
+        ] = None,
+        headers: Annotated[
+            Optional[Dict[str, str]],
+            Doc(
+                "Message headers to store metainformation. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("Topic name to send response."),
+        ] = "",
+        batch: Annotated[
+            bool,
+            Doc("Whether to send messages in batches or not."),
+        ] = False,
+        # basic args
+        middlewares: Annotated[
+            Iterable[PublisherMiddleware],
+            Doc("Publisher middlewares to wrap outgoing messages."),
+        ] = (),
+        # AsyncAPI args
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
     ) -> None:
-        """Redis broker.
-
-        Args:
-            url : URL of the Redis server
-            polling_interval : interval in seconds to poll the Redis server for new messages (default: None)
-            protocol : protocol of the Redis server (default: None)
-            protocol_version : protocol version of the Redis server (default: "custom")
-            security : security settings for the Redis server (default: None)
-            kwargs : additional keyword arguments
-        """
-        self.global_polling_interval = polling_interval
-        self._producer = None
-
         super().__init__(
-            url=url,
-            protocol_version=protocol_version,
-            security=security,
-            **kwargs,
+            topic=topic,
+            key=key,
+            partition=partition,
+            batch=batch,
+            headers=headers,
+            reply_to=reply_to,
+            # basic args
+            middlewares=middlewares,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            schema=schema,
+            include_in_schema=include_in_schema,
         )
 
-        url_kwargs = urlparse(self.url)
-        self.protocol = protocol or url_kwargs.scheme
 
-    async def connect(
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> "Redis[bytes]":
-        """Connect to the Redis server.
-
-        Args:
-            args : additional positional arguments
-            kwargs : additional keyword arguments
-        """
-        connection = await super().connect(*args, **kwargs)
-        for p in self._publishers.values():
-            p._producer = self._producer
-        return connection
+class KafkaRoute(SubscriberRoute):
+    """Class to store delaied KafkaBroker subscriber registration."""
 
-    @override
-    async def _connect(  # type: ignore[override]
-        self,
-        url: str,
-        **kwargs: Any,
-    ) -> "Redis[bytes]":
-        url_options: AnyDict = parse_url(url)
-        url_options.update(kwargs)
-        url_options.update(parse_security(self.security))
-        pool = ConnectionPool(**url_options)
-
-        client = Redis.from_pool(pool)
-        self._producer = RedisFastProducer(
-            connection=client,
-            parser=self._global_parser,  # type: ignore[arg-type]
-            decoder=self._global_parser,  # type: ignore[arg-type]
-        )
-        return client
-
-    async def _close(
+    def __init__(
         self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_val: Optional[BaseException] = None,
-        exec_tb: Optional[TracebackType] = None,
+        call: Annotated[
+            Callable[..., SendableMessage],
+            Doc("Message handler function."),
+        ],
+        *topics: str,
+        publishers: Annotated[
+            Iterable[KafkaPublisher],
+            Doc("Kafka publishers to broadcast the handler result."),
+        ] = (),
+        group_id: Optional[str] = None,
+        key_deserializer: Optional[Callable[[bytes], Any]] = None,
+        value_deserializer: Optional[Callable[[bytes], Any]] = None,
+        fetch_max_wait_ms: int = 500,
+        fetch_max_bytes: int = 52428800,
+        fetch_min_bytes: int = 1,
+        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
+        auto_offset_reset: Literal[
+            "latest",
+            "earliest",
+            "none",
+        ] = "latest",
+        auto_commit: bool = True,
+        auto_commit_interval_ms: int = 5000,
+        check_crcs: bool = True,
+        partition_assignment_strategy: Sequence[str] = (
+            "roundrobin",
+        ),
+        max_poll_interval_ms: int = 300000,
+        rebalance_timeout_ms: Optional[int] = None,
+        session_timeout_ms: int = 10000,
+        heartbeat_interval_ms: int = 3000,
+        consumer_timeout_ms: int = 200,
+        max_poll_records: Optional[int] = None,
+        exclude_internal_topics: bool = True,
+        isolation_level: Literal[
+            "read_uncommitted",
+            "read_committed",
+        ] = "read_uncommitted",
+        batch: bool = False,
+        max_records: Optional[int] = None,
+        batch_timeout_ms: int = 200,
+        # broker args
+        dependencies: Annotated[
+            Iterable[Depends],
+            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
+        ] = (),
+        parser: Annotated[
+            Optional[
+                Union[
+                    CustomParser[Message],
+                    CustomParser[Tuple[Message, ...]],
+                ]
+            ],
+            Doc("Parser to map original **Message** object to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional[
+                Union[
+                    CustomDecoder[StreamMessage[Message]],
+                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
+                ]
+            ],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        middlewares: Annotated[
+            Iterable[SubscriberMiddleware],
+            Doc("Subscriber middlewares to wrap incoming message processing."),
+        ] = (),
+        filter: Annotated[
+            Union[
+                Filter[StreamMessage[Message]],
+                Filter[StreamMessage[Tuple[Message, ...]]],
+            ],
+            Doc(
+                "Overload subscriber to consume various messages from the same source."
+            ),
+            deprecated(
+                "Deprecated in **FastStream 0.5.0**. "
+                "Please, create `subscriber` object and use it explicitly instead. "
+                "Argument will be removed in **FastStream 0.6.0**."
+            ),
+        ] = default_filter,
+        retry: Annotated[
+            bool,
+            Doc("Whether to `nack` message at processing exception."),
+        ] = False,
+        no_ack: Annotated[
+            bool,
+            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
+        ] = False,
+        # AsyncAPI args
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI subscriber object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc(
+                "AsyncAPI subscriber object description. "
+                "Uses decorated docstring as default."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
     ) -> None:
-        if self._connection is not None:
-            await self._connection.aclose()  # type: ignore[attr-defined]
-
-        await super()._close(exc_type, exc_val, exec_tb)
-
-    async def start(self) -> None:
-        context.set_global(
-            "default_log_context",
-            self._get_log_context(None, ""),
+        super().__init__(
+            call,
+            *topics,
+            publishers=publishers,
+            group_id=group_id,
+            key_deserializer=key_deserializer,
+            value_deserializer=value_deserializer,
+            fetch_max_wait_ms=fetch_max_wait_ms,
+            fetch_max_bytes=fetch_max_bytes,
+            fetch_min_bytes=fetch_min_bytes,
+            max_partition_fetch_bytes=max_partition_fetch_bytes,
+            auto_offset_reset=auto_offset_reset,
+            auto_commit=auto_commit,
+            auto_commit_interval_ms=auto_commit_interval_ms,
+            check_crcs=check_crcs,
+            partition_assignment_strategy=partition_assignment_strategy,
+            max_poll_interval_ms=max_poll_interval_ms,
+            rebalance_timeout_ms=rebalance_timeout_ms,
+            session_timeout_ms=session_timeout_ms,
+            heartbeat_interval_ms=heartbeat_interval_ms,
+            consumer_timeout_ms=consumer_timeout_ms,
+            max_poll_records=max_poll_records,
+            exclude_internal_topics=exclude_internal_topics,
+            isolation_level=isolation_level,
+            max_records=max_records,
+            batch_timeout_ms=batch_timeout_ms,
+            batch=batch,
+            # basic args
+            dependencies=dependencies,
+            parser=parser,
+            decoder=decoder,
+            middlewares=middlewares,
+            filter=filter,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            include_in_schema=include_in_schema,
+            # FastDepends args
+            retry=retry,
+            no_ack=no_ack,
         )
 
-        await super().start()
-        assert self._connection, NOT_CONNECTED_YET  # nosec B101
 
-        for handler in self.handlers.values():
-            if (stream := handler.stream_sub) is not None and stream.group:
-                try:
-                    await self._connection.xgroup_create(
-                        name=stream.name,
-                        groupname=stream.group,
-                        id=stream.last_id,
-                        mkstream=True,
-                    )
-                except ResponseError as e:
-                    if "already exists" not in str(e):
-                        raise e
-
-            c = self._get_log_context(None, handler.channel_name)
-            self._log(f"`{handler.call_name}` waiting for messages", extra=c)
-            await handler.start(self._connection)
-
-    def _process_message(
-        self,
-        func: Callable[[StreamMessage[Any]], Awaitable[T_HandlerReturn]],
-        watcher: Callable[..., AsyncContextManager[None]],
-        **kwargs: Any,
-    ) -> Callable[
-        [StreamMessage[Any]],
-        Awaitable[WrappedReturn[T_HandlerReturn]],
-    ]:
-        @wraps(func)
-        async def process_wrapper(
-            message: StreamMessage[Any],
-        ) -> WrappedReturn[T_HandlerReturn]:
-            async with watcher(
-                message,
-                redis=self._connection,
-            ):
-                r = await func(message)
-
-                pub_response: Optional[AsyncPublisherProtocol]
-                if message.reply_to:
-                    pub_response = FakePublisher(
-                        partial(self.publish, channel=message.reply_to)
-                    )
-                else:
-                    pub_response = None
-
-                return r, pub_response
-
-        return process_wrapper
+class KafkaRouter(
+    BrokerRouter[Union[
+        Message,
+        Tuple[Message, ...],
+    ]],
+    KafkaRegistrator,
+):
+    """Includable to KafkaBroker router."""
 
-    @override
-    def subscriber(  # type: ignore[override]
+    def __init__(
         self,
-        channel: Union[Channel, PubSub, None] = None,
+        prefix: Annotated[
+            str,
+            Doc("String prefix to add to all subscribers queues."),
+        ] = "",
+        handlers: Annotated[
+            Iterable[KafkaRoute],
+            Doc("Route object to include."),
+        ] = (),
         *,
-        list: Union[Channel, ListSub, None] = None,
-        stream: Union[Channel, StreamSub, None] = None,
-        # broker arguments
-        dependencies: Sequence[Depends] = (),
-        parser: Optional[CustomParser[AnyRedisDict, RedisMessage]] = None,
-        decoder: Optional[CustomDecoder[RedisMessage]] = None,
-        middlewares: Optional[
-            Sequence[Callable[[AnyRedisDict], BaseMiddleware]]
-        ] = None,
-        filter: Filter[RedisMessage] = default_filter,
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
-        **original_kwargs: Any,
-    ) -> Callable[
-        [Callable[P_HandlerParams, T_HandlerReturn]],
-        HandlerCallWrapper[Any, P_HandlerParams, T_HandlerReturn],
-    ]:
-        channel = PubSub.validate(channel)
-        list = ListSub.validate(list)
-        stream = StreamSub.validate(stream)
-
-        if (any_of := channel or list or stream) is None:
-            raise ValueError(INCORRECT_SETUP_MSG)
-
-        if all((channel, list)):
-            raise ValueError("You can't use `PubSub` and `ListSub` both")
-        elif all((channel, stream)):
-            raise ValueError("You can't use `PubSub` and `StreamSub` both")
-        elif all((list, stream)):
-            raise ValueError("You can't use `ListSub` and `StreamSub` both")
-
-        self._setup_log_context(channel=any_of.name)
-        super().subscriber()
-
-        key = Handler.get_routing_hash(any_of)
-        handler = self.handlers[key] = self.handlers.get(
-            key,
-            Handler(  # type: ignore[abstract]
-                log_context_builder=partial(
-                    self._get_log_context,
-                    channel=any_of.name,
-                ),
-                graceful_timeout=self.graceful_timeout,
-                # Redis
-                channel=channel,
-                list=list,
-                stream=stream,
-                # AsyncAPI
-                title=title,
-                description=description,
-                include_in_schema=include_in_schema,
+        dependencies: Annotated[
+            Iterable[Depends],
+            Doc(
+                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
-        )
-
-        def consumer_wrapper(
-            func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[
-            AnyRedisDict,
-            P_HandlerParams,
-            T_HandlerReturn,
-        ]:
-            handler_call, dependant = self._wrap_handler(
-                func,
-                extra_dependencies=dependencies,
-                **original_kwargs,
-            )
-
-            handler.add_call(
-                handler=handler_call,
-                filter=filter,
-                middlewares=middlewares,
-                parser=parser or self._global_parser,  # type: ignore[arg-type]
-                decoder=decoder or self._global_decoder,  # type: ignore[arg-type]
-                dependant=dependant,
-            )
-
-            return handler_call
-
-        return consumer_wrapper
-
-    @override
-    def publisher(  # type: ignore[override]
-        self,
-        channel: Union[Channel, PubSub, None] = None,
-        list: Union[Channel, ListSub, None] = None,
-        stream: Union[Channel, StreamSub, None] = None,
-        headers: Optional[AnyDict] = None,
-        reply_to: str = "",
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        schema: Optional[Any] = None,
-        include_in_schema: bool = True,
-    ) -> Publisher:
-        channel = PubSub.validate(channel)
-        list = ListSub.validate(list)
-        stream = StreamSub.validate(stream)
-
-        any_of = channel or list or stream
-        if any_of is None:
-            raise ValueError(INCORRECT_SETUP_MSG)
-
-        key = Handler.get_routing_hash(any_of)
-        publisher = self._publishers.get(
-            key,
-            Publisher(
-                channel=channel,
-                list=list,
-                stream=stream,
-                headers=headers,
-                reply_to=reply_to,
-                # AsyncAPI
-                title=title,
-                _description=description,
-                _schema=schema,
-                include_in_schema=include_in_schema,
-            ),
-        )
-        super().publisher(key, publisher)
-        if self._producer is not None:
-            publisher._producer = self._producer
-        return publisher
-
-    @override
-    async def publish(  # type: ignore[override]
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Optional[DecodedMessage]:
-        assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        return await self._producer.publish(*args, **kwargs)
-
-    async def publish_batch(
-        self,
-        *args: Any,
-        **kwargs: Any,
+        ] = (),
+        middlewares: Annotated[
+            Iterable[Union[
+                BrokerMiddleware[Message],
+                BrokerMiddleware[Tuple[Message, ...]],
+            ]],
+            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
+        ] = (),
+        parser: Annotated[
+            Optional[Union[
+                CustomParser[Message],
+                CustomParser[Tuple[Message, ...]],
+            ]],
+            Doc("Parser to map original **Message** object to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional[Union[
+                CustomDecoder[StreamMessage[Message]],
+                CustomDecoder[StreamMessage[Tuple[Message, ...]]],
+            ]],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        include_in_schema: Annotated[
+            Optional[bool],
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = None,
     ) -> None:
-        assert self._producer, NOT_CONNECTED_YET  # nosec B101
-        return await self._producer.publish_batch(*args, **kwargs)
+        super().__init__(
+            handlers=handlers,
+            # basic args
+            prefix=prefix,
+            dependencies=dependencies,
+            middlewares=middlewares,
+            parser=parser,
+            decoder=decoder,
+            include_in_schema=include_in_schema,
+        )
```

### Comparing `faststream-0.4.7/faststream/redis/parser.py` & `faststream-0.5.0rc0/faststream/redis/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,82 @@
-from typing import TYPE_CHECKING, Optional, Sequence, Tuple, Union, overload
-from uuid import uuid4
-
-from pydantic import BaseModel, Field
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Generic,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
-from faststream._compat import dump_json, model_parse, model_to_json
-from faststream.broker.parsers import decode_message, encode_message
+from faststream._compat import dump_json, json_loads
+from faststream.broker.message import (
+    StreamMessage,
+    decode_message,
+    encode_message,
+    gen_cor_id,
+)
+from faststream.constants import ContentTypes
 from faststream.redis.message import (
-    BatchMessage,
-    BatchRedisMessage,
-    OneMessage,
-    OneRedisMessage,
+    BatchListMessage,
+    BatchStreamMessage,
+    DefaultListMessage,
+    DefaultStreamMessage,
+    PubSubMessage,
+    RedisBatchListMessage,
+    RedisBatchStreamMessage,
+    RedisListMessage,
+    RedisMessage,
+    RedisStreamMessage,
+    bDATA_KEY,
 )
 from faststream.types import AnyDict, DecodedMessage, SendableMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
-    from faststream.redis.asyncapi import Handler
+    from faststream.redis.schemas import PubSub
+    from faststream.redis.subscriber.usecase import ChannelSubscriber
 
-DATA_KEY = "__data__"
-bDATA_KEY = DATA_KEY.encode()  # noqa: N816
 
+MsgType = TypeVar("MsgType", bound=Mapping[str, Any])
 
-class RawMessage(BaseModel):
+
+class RawMessage:
     """A class to represent a raw Redis message."""
 
-    data: bytes
-    headers: AnyDict = Field(default_factory=dict)
+    __slots__ = (
+        "data",
+        "headers",
+    )
+
+    def __init__(
+        self,
+        data: bytes,
+        headers: Optional["AnyDict"] = None,
+    ) -> None:
+        self.data = data
+        self.headers = headers or {}
 
     @classmethod
     def build(
         cls,
+        *,
         message: Union[Sequence[SendableMessage], SendableMessage],
-        reply_to: str = "",
-        headers: Optional[AnyDict] = None,
-        correlation_id: Optional[str] = None,
+        reply_to: Optional[str],
+        headers: Optional[AnyDict],
+        correlation_id: str,
     ) -> "RawMessage":
         payload, content_type = encode_message(message)
 
         headers_to_send = {
-            "correlation_id": correlation_id or str(uuid4()),
+            "correlation_id": correlation_id,
         }
 
         if content_type:
             headers_to_send["content-type"] = content_type
 
         if reply_to:
             headers_to_send["reply_to"] = reply_to
@@ -54,106 +88,135 @@
             data=payload,
             headers=headers_to_send,
         )
 
     @classmethod
     def encode(
         cls,
+        *,
         message: Union[Sequence[SendableMessage], SendableMessage],
-        reply_to: str = "",
-        headers: Optional[AnyDict] = None,
-        correlation_id: Optional[str] = None,
-    ) -> str:
-        return model_to_json(
-            cls.build(
-                message=message,
-                reply_to=reply_to,
-                headers=headers,
-                correlation_id=correlation_id,
-            )
+        reply_to: Optional[str],
+        headers: Optional[AnyDict],
+        correlation_id: str,
+    ) -> bytes:
+        msg = cls.build(
+            message=message,
+            reply_to=reply_to,
+            headers=headers,
+            correlation_id=correlation_id,
         )
 
+        return dump_json({
+            "data": msg.data,
+            "headers": msg.headers,
+        })
 
-class RedisParser:
-    """A class to represent a Redis parser."""
+    @staticmethod
+    def parse(data: bytes) -> Tuple[bytes, AnyDict]:
+        headers: AnyDict
 
-    @classmethod
-    @overload
-    async def parse_message(
-        cls,
-        message: OneMessage,
-    ) -> OneRedisMessage:
-        pass
+        try:
+            # FastStream message format
+            parsed_data = json_loads(data)
+            data = parsed_data["data"].encode()
+            headers = parsed_data["headers"]
 
-    @classmethod
-    @overload
-    async def parse_message(
-        cls,
-        message: BatchMessage,
-    ) -> BatchRedisMessage:
-        pass
+        except Exception:
+            # Raw Redis message format
+            data = data
+            headers = {}
 
-    @classmethod
-    async def parse_message(
-        cls,
-        message: Union[OneMessage, BatchMessage],
-    ) -> Union[OneRedisMessage, BatchRedisMessage]:
-        id_ = str(uuid4())
-
-        if message["type"] == "batch":
-            data = dump_json([cls.parse_one_msg(x)[0] for x in message["data"]])
-
-            return BatchRedisMessage(
-                raw_message=message,
-                body=data,
-                content_type="application/json",
-                message_id=id_,
-                correlation_id=id_,
-            )
+        return data, headers
 
-        else:
-            data, headers = cls.parse_one_msg(message["data"])
 
-            channel = message.get("channel", b"").decode()
+class SimpleParser(Generic[MsgType]):
+    msg_class: Type[StreamMessage[MsgType]]
 
-            handler: Optional["Handler"] = context.get_local("handler_")
-            if (
-                handler is not None
-                and handler.channel is not None
-                and (path_re := handler.channel.path_regex) is not None
-                and (match := path_re.match(channel)) is not None
-            ):
-                path = match.groupdict()
-            else:
-                path = {}
-
-            return OneRedisMessage(
-                raw_message=message,
-                body=data,
-                path=path,
-                headers=headers,
-                reply_to=headers.get("reply_to", ""),
-                content_type=headers.get("content-type", ""),
-                message_id=message.get("message_id", id_),
-                correlation_id=headers.get("correlation_id", id_),
-            )
+    @classmethod
+    async def parse_message(cls, message: MsgType) -> StreamMessage[MsgType]:
+        data, headers = cls._parse_data(message)
+        id_ = gen_cor_id()
+        return cls.msg_class(
+            raw_message=message,
+            body=data,
+            path=cls.get_path(message),
+            headers=headers,
+            reply_to=headers.get("reply_to", ""),
+            content_type=headers.get("content-type"),
+            message_id=headers.get("message_id", id_),
+            correlation_id=headers.get("correlation_id", id_),
+        )
 
     @staticmethod
-    def parse_one_msg(raw_data: bytes) -> Tuple[bytes, AnyDict]:
-        try:
-            obj = model_parse(RawMessage, raw_data)
-        except Exception:
-            # Raw Redis message format
-            data = raw_data
-            headers: AnyDict = {}
-        else:
-            # FastStream message format
-            data = obj.data
-            headers = obj.headers
+    def _parse_data(message: MsgType) -> Tuple[bytes, AnyDict]:
+        return RawMessage.parse(message["data"])
 
-        return data, headers
+    @staticmethod
+    def get_path(message: MsgType) -> AnyDict:
+        return {}
 
     @staticmethod
     async def decode_message(
-        msg: OneRedisMessage,
+        msg: StreamMessage[MsgType],
     ) -> DecodedMessage:
         return decode_message(msg)
+
+
+class RedisPubSubParser(SimpleParser[PubSubMessage]):
+    msg_class = RedisMessage
+
+    @staticmethod
+    def get_path(message: PubSubMessage) -> AnyDict:
+        if (
+            message.get("pattern")
+            and (handler := cast("ChannelSubscriber", context.get_local("handler_")))
+            and (channel := cast(Optional["PubSub"], getattr(handler, "channel", None)))
+            and (path_re := channel.path_regex)
+            and (match := path_re.match(message["channel"]))
+        ):
+            return match.groupdict()
+
+        else:
+            return {}
+
+
+class RedisListParser(SimpleParser[DefaultListMessage]):
+    msg_class = RedisListMessage
+
+
+class RedisBatchListParser(SimpleParser[BatchListMessage]):
+    msg_class = RedisBatchListMessage
+
+    @staticmethod
+    def _parse_data(message: BatchListMessage) -> Tuple[bytes, AnyDict]:
+        return (
+            dump_json(
+                RawMessage.parse(x)[0]
+                for x in message["data"]
+            ),
+            {"content-type": ContentTypes.json},
+        )
+
+
+class RedisStreamParser(SimpleParser[DefaultStreamMessage]):
+    msg_class = RedisStreamMessage
+
+    @classmethod
+    def _parse_data(cls, message: DefaultStreamMessage) -> Tuple[bytes, AnyDict]:
+        data = message["data"]
+        return RawMessage.parse(data.get(bDATA_KEY) or dump_json(data))
+
+
+class RedisBatchStreamParser(SimpleParser[BatchStreamMessage]):
+    msg_class = RedisBatchStreamMessage
+
+    @staticmethod
+    def _parse_data(message: BatchStreamMessage) -> Tuple[bytes, AnyDict]:
+        return (
+            dump_json(
+                RawMessage.parse(data)[0]
+                if (data := x.get(bDATA_KEY))
+                else x
+                for x in message["data"]
+            ),
+            {"content-type": ContentTypes.json},
+        )
```

### Comparing `faststream-0.4.7/faststream/redis/producer.py` & `faststream-0.5.0rc0/faststream/redis/publisher/producer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,72 @@
-from typing import TYPE_CHECKING, Any, Optional, Union, overload
+from typing import Any, Optional
 from uuid import uuid4
 
-from faststream.broker.parsers import encode_message, resolve_custom_func
+from redis.asyncio.client import PubSub, Redis
+from typing_extensions import override
+
+from faststream.broker.message import StreamMessage
+from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.types import (
-    AsyncCustomDecoder,
-    AsyncCustomParser,
     AsyncDecoder,
     AsyncParser,
+    CustomDecoder,
+    CustomParser,
 )
-from faststream.exceptions import WRONG_PUBLISH_ARGS
-from faststream.redis.message import (
-    AnyRedisDict,
-    BatchMessage,
-    BatchRedisMessage,
-    OneMessage,
-    OneRedisMessage,
-)
-from faststream.redis.parser import DATA_KEY, RawMessage, RedisParser
+from faststream.broker.utils import resolve_custom_func
+from faststream.exceptions import WRONG_PUBLISH_ARGS, SetupError
+from faststream.redis.message import DATA_KEY, PubSubMessage
+from faststream.redis.parser import RawMessage, RedisPubSubParser
 from faststream.redis.schemas import INCORRECT_SETUP_MSG
 from faststream.types import AnyDict, SendableMessage
 from faststream.utils.functions import timeout_scope
 
-if TYPE_CHECKING:
-    from redis.asyncio.client import PubSub, Redis
-
 
-class RedisFastProducer:
+class RedisFastProducer(ProducerProto):
     """A class to represent a Redis producer."""
 
     _connection: "Redis[bytes]"
-    _decoder: AsyncDecoder[Any]
-    _parser: AsyncParser[AnyRedisDict, Any]
-
-    @overload
-    def __init__(
-        self,
-        connection: "Redis[bytes]",
-        parser: Optional[AsyncCustomParser[OneMessage, OneRedisMessage]],
-        decoder: Optional[AsyncCustomDecoder[OneRedisMessage]],
-    ) -> None:
-        pass
-
-    @overload
-    def __init__(
-        self,
-        connection: "Redis[bytes]",
-        parser: Optional[AsyncCustomParser[BatchMessage, BatchRedisMessage]],
-        decoder: Optional[AsyncCustomDecoder[BatchRedisMessage]],
-    ) -> None:
-        pass
+    _decoder: AsyncDecoder[StreamMessage[PubSubMessage]]
+    _parser: AsyncParser[PubSubMessage]
 
     def __init__(
         self,
         connection: "Redis[bytes]",
-        parser: Union[
-            None,
-            AsyncCustomParser[OneMessage, OneRedisMessage],
-            AsyncCustomParser[BatchMessage, BatchRedisMessage],
-        ],
-        decoder: Union[
-            None,
-            AsyncCustomDecoder[OneRedisMessage],
-            AsyncCustomDecoder[BatchRedisMessage],
-        ],
+        parser: Optional[CustomParser[PubSubMessage]],
+        decoder: Optional[CustomDecoder[StreamMessage[PubSubMessage]]],
     ) -> None:
-        """Initialize the Redis producer.
-
-        Args:
-            connection: The Redis connection.
-            parser: The parser.
-            decoder: The decoder.
-        """
         self._connection = connection
         self._parser = resolve_custom_func(
             parser,  # type: ignore[arg-type,assignment]
-            RedisParser.parse_message,
+            RedisPubSubParser.parse_message,
         )
-        self._decoder = resolve_custom_func(decoder, RedisParser.decode_message)
+        self._decoder = resolve_custom_func(
+            decoder, RedisPubSubParser.decode_message)
 
-    async def publish(
+    @override
+    async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
-        channel: Optional[str] = None,
-        reply_to: str = "",
-        headers: Optional[AnyDict] = None,
-        correlation_id: Optional[str] = None,
         *,
+        correlation_id: str,
+        channel: Optional[str] = None,
         list: Optional[str] = None,
         stream: Optional[str] = None,
+        maxlen: Optional[int] = None,
+        headers: Optional[AnyDict] = None,
+        reply_to: str = "",
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-        maxlen: Optional[int] = None,
     ) -> Optional[Any]:
         if not any((channel, list, stream)):
-            raise ValueError(INCORRECT_SETUP_MSG)
+            raise SetupError(INCORRECT_SETUP_MSG)
 
-        psub: Optional["PubSub"] = None
-        if rpc is True:
+        psub: Optional[PubSub] = None
+        if rpc:
             if reply_to:
                 raise WRONG_PUBLISH_ARGS
 
             reply_to = str(uuid4())
             psub = self._connection.pubsub()
             await psub.subscribe(reply_to)
 
@@ -154,10 +119,12 @@
             else:
                 return await self._decoder(await self._parser(m))
 
     async def publish_batch(
         self,
         *msgs: SendableMessage,
         list: str,
+        correlation_id: str,
     ) -> None:
-        batch = (encode_message(msg)[0] for msg in msgs)
+        batch = (RawMessage.encode(message=msg, correlation_id=correlation_id,
+                 reply_to=None, headers=None,) for msg in msgs)
         await self._connection.rpush(list, *batch)
```

### Comparing `faststream-0.4.7/faststream/redis/router.py` & `faststream-0.5.0rc0/faststream/nats/publisher/asyncapi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Iterable, Optional, Union
 
+from nats.aio.msg import Msg
 from typing_extensions import override
 
-from faststream._compat import model_copy
-from faststream.redis.asyncapi import Handler, Publisher
-from faststream.redis.schemas import INCORRECT_SETUP_MSG, ListSub, PubSub, StreamSub
-from faststream.redis.shared.router import RedisRouter as BaseRouter
-from faststream.types import AnyDict
-
-
-class RedisRouter(BaseRouter):
-    """A class to represent a Redis router."""
-
-    _publishers: Dict[int, Publisher]  # type: ignore[assignment]
-
-    @override
-    @staticmethod
-    def _get_publisher_key(publisher: Publisher) -> int:  # type: ignore[override]
-        any_of = publisher.channel or publisher.list or publisher.stream
-        if any_of is None:
-            raise ValueError(INCORRECT_SETUP_MSG)
-        return Handler.get_routing_hash(any_of)
-
-    @override
-    @staticmethod
-    def _update_publisher_prefix(  # type: ignore[override]
-        prefix: str,
-        publisher: Publisher,
-    ) -> Publisher:
-        if publisher.channel is not None:
-            publisher.channel = model_copy(
-                publisher.channel, update={"name": prefix + publisher.channel.name}
-            )
-        elif publisher.list is not None:
-            publisher.list = model_copy(
-                publisher.list, update={"name": prefix + publisher.list.name}
-            )
-        elif publisher.stream is not None:
-            publisher.stream = model_copy(
-                publisher.stream, update={"name": prefix + publisher.stream.name}
+from faststream.asyncapi.schema import (
+    Channel,
+    ChannelBinding,
+    CorrelationId,
+    Message,
+    Operation,
+)
+from faststream.asyncapi.schema.bindings import nats
+from faststream.asyncapi.utils import resolve_payloads
+from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+from faststream.nats.helpers import stream_builder
+from faststream.nats.publisher.usecase import LogicPublisher
+from faststream.nats.schemas.js_stream import JStream
+
+
+class AsyncAPIPublisher(LogicPublisher):
+    """A class to represent a NATS publisher."""
+
+    def get_name(self) -> str:
+        return f"{self.subject}:Publisher"
+
+    def get_schema(self) -> Dict[str, Channel]:
+        payloads = self.get_payloads()
+
+        return {
+            self.name: Channel(
+                description=self.description,
+                publish=Operation(
+                    message=Message(
+                        title=f"{self.name}:Message",
+                        payload=resolve_payloads(payloads, "Publisher"),
+                        correlationId=CorrelationId(
+                            location="$message.header#/correlation_id"
+                        ),
+                    ),
+                ),
+                bindings=ChannelBinding(
+                    nats=nats.ChannelBinding(
+                        subject=self.subject,
+                    )
+                ),
             )
-        else:
-            raise AssertionError("unreachable")
-        return publisher
+        }
 
     @override
-    def publisher(  # type: ignore[override]
-        self,
-        channel: Union[str, PubSub, None] = None,
-        list: Union[str, ListSub, None] = None,
-        stream: Union[str, StreamSub, None] = None,
-        headers: Optional[AnyDict] = None,
-        reply_to: str = "",
-        # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        schema: Optional[Any] = None,
-        include_in_schema: bool = True,
-    ) -> Publisher:
-        if not any((stream, list, channel)):
-            raise ValueError(INCORRECT_SETUP_MSG)
-
-        new_publisher = self._update_publisher_prefix(
-            self.prefix,
-            Publisher(
-                channel=PubSub.validate(channel),
-                list=ListSub.validate(list),
-                stream=StreamSub.validate(stream),
-                reply_to=reply_to,
-                headers=headers,
-                title=title,
-                _description=description,
-                _schema=schema,
-                include_in_schema=(
-                    include_in_schema
-                    if self.include_in_schema is None
-                    else self.include_in_schema
-                ),
-            ),
-        )
-        publisher_key = self._get_publisher_key(new_publisher)
-        publisher = self._publishers[publisher_key] = self._publishers.get(
-            publisher_key, new_publisher
+    @classmethod
+    def create(  # type: ignore[override]
+        cls,
+        *,
+        subject: str,
+        reply_to: str,
+        headers: Optional[Dict[str, str]],
+        stream: Union[str, "JStream", None],
+        timeout: Optional[float],
+        # Publisher args
+        broker_middlewares: Iterable[BrokerMiddleware[Msg]],
+        middlewares: Iterable[PublisherMiddleware],
+        # AsyncAPI args
+        schema_: Optional[Any],
+        title_: Optional[str],
+        description_: Optional[str],
+        include_in_schema: bool,
+    ) -> "AsyncAPIPublisher":
+        if (stream := stream_builder.stream(stream)):
+            stream.add_subject(subject)
+
+        return cls(
+            subject=subject,
+            reply_to=reply_to,
+            headers=headers,
+            stream=stream,
+            timeout=timeout,
+            # Publisher args
+            broker_middlewares=broker_middlewares,
+            middlewares=middlewares,
+            # AsyncAPI args
+            schema_=schema_,
+            title_=title_,
+            description_=description_,
+            include_in_schema=include_in_schema,
         )
-        return publisher
```

### Comparing `faststream-0.4.7/faststream/redis/security.py` & `faststream-0.5.0rc0/faststream/redis/security.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,18 @@
                 _security: BaseSecurity = security,
                 **kwargs: Any,
             ) -> None:
                 self._security = _security
                 super().__init__(**kwargs)
 
             def _connection_arguments(self) -> Any:
-                kwargs = super()._connection_arguments()  # type: ignore
-                kwargs["ssl"] = self._security.ssl_context
-                return kwargs
+                return {
+                    **super()._connection_arguments(),  # type: ignore[misc]
+                    "ssl": self._security.ssl_context
+                }
 
         return {"connection_class": SSLConnection}
     else:
         return {}
 
 
 def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
```

### Comparing `faststream-0.4.7/faststream/redis/test.py` & `faststream-0.5.0rc0/faststream/broker/subscriber/call_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,177 @@
-import re
-from typing import Any, Optional, Sequence, Union
+from contextlib import AsyncExitStack
+from inspect import unwrap
+from itertools import chain
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    Optional,
+    cast,
+)
+
+from typing_extensions import override
+
+from faststream.broker.proto import SetupAble
+from faststream.broker.types import MsgType
+from faststream.exceptions import IgnoredException, SetupError
+
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import (
+        AsyncDecoder,
+        AsyncFilter,
+        AsyncParser,
+        CustomDecoder,
+        CustomParser,
+        SubscriberMiddleware,
+    )
+    from faststream.broker.wrapper.call import HandlerCallWrapper
 
-from faststream.broker.test import TestBroker, call_handler
-from faststream.broker.wrapper import HandlerCallWrapper
-from faststream.redis.asyncapi import Handler, Publisher
-from faststream.redis.broker import RedisBroker
-from faststream.redis.message import AnyRedisDict
-from faststream.redis.parser import RawMessage
-from faststream.redis.producer import RedisFastProducer
-from faststream.redis.schemas import INCORRECT_SETUP_MSG
-from faststream.types import AnyDict, SendableMessage
-
-__all__ = ("TestRedisBroker",)
-
-
-class TestRedisBroker(TestBroker[RedisBroker]):
-    """A class to test Redis brokers."""
-
-    @staticmethod
-    def patch_publisher(
-        broker: RedisBroker,
-        publisher: Any,
-    ) -> None:
-        publisher._producer = broker._producer
 
-    @staticmethod
-    def create_publisher_fake_subscriber(
-        broker: RedisBroker,
-        publisher: Publisher,
-    ) -> HandlerCallWrapper[Any, Any, Any]:
-        @broker.subscriber(
-            channel=publisher.channel,
-            list=publisher.list,
-            stream=publisher.stream,
-            _raw=True,
-        )
-        def f(msg: Any) -> None:
-            pass
+class HandlerItem(SetupAble, Generic[MsgType]):
+    """A class representing handler overloaded item."""
 
-        return f
+    __slots__ = (
+        "handler",
+        "filter",
+        "dependant",
+        "dependencies",
+        "item_parser",
+        "item_decoder",
+        "item_middlewares",
+    )
 
-    @staticmethod
-    async def _fake_connect(
-        broker: RedisBroker,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        broker._producer = FakeProducer(broker)  # type: ignore[assignment]
+    dependant: Optional[Any]
 
-    @staticmethod
-    def remove_publisher_fake_subscriber(
-        broker: RedisBroker,
-        publisher: Publisher,
+    def __init__(
+        self,
+        *,
+        handler: "HandlerCallWrapper[MsgType, ..., Any]",
+        filter: "AsyncFilter[StreamMessage[MsgType]]",
+        item_parser: Optional["CustomParser[MsgType]"],
+        item_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        item_middlewares: Iterable["SubscriberMiddleware"],
+        dependencies: Iterable["Depends"],
     ) -> None:
-        any_of = publisher.channel or publisher.list or publisher.stream
-        assert any_of  # nosec B101
-        broker.handlers.pop(Handler.get_routing_hash(any_of), None)
-
-
-class FakeProducer(RedisFastProducer):
-    def __init__(self, broker: RedisBroker) -> None:
-        self.broker = broker
+        self.handler = handler
+        self.filter = filter
+        self.item_parser = item_parser
+        self.item_decoder = item_decoder
+        self.item_middlewares = item_middlewares
+        self.dependencies = dependencies
+        self.dependant = None
+
+    def __repr__(self) -> str:
+        filter_call = unwrap(self.filter)
+        filter_name = getattr(filter_call, "__name__", str(filter_call))
+        return f"<'{self.call_name}': filter='{filter_name}'>"
 
-    async def publish(
+    @override
+    def setup(  # type: ignore[override]
         self,
-        message: SendableMessage,
-        channel: Optional[str] = None,
-        reply_to: str = "",
-        headers: Optional[AnyDict] = None,
-        correlation_id: Optional[str] = None,
         *,
-        list: Optional[str] = None,
-        stream: Optional[str] = None,
-        rpc: bool = False,
-        rpc_timeout: Optional[float] = 30.0,
-        raise_timeout: bool = False,
-        maxlen: Optional[int] = None,
-    ) -> Optional[Any]:
-        any_of = channel or list or stream
-        if any_of is None:
-            raise ValueError(INCORRECT_SETUP_MSG)
-
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            call = False
-            batch = False
-
-            if channel and (ch := handler.channel) is not None:
-                call = bool(
-                    (not ch.pattern and ch.name == channel)
-                    or (
-                        ch.pattern
-                        and re.match(
-                            ch.name.replace(".", "\\.").replace("*", ".*"),
-                            channel,
-                        )
-                    )
-                )
+        parser: "AsyncParser[MsgType]",
+        decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        broker_dependencies: Iterable["Depends"],
+        apply_types: bool,
+        is_validate: bool,
+        _get_dependant: Optional[Callable[..., Any]],
+    ) -> None:
+        if self.dependant is None:
+            self.item_parser = parser
+            self.item_decoder = decoder
+
+            dependencies = (*broker_dependencies, *self.dependencies)
+
+            dependant = self.handler.set_wrapped(
+                apply_types=apply_types,
+                is_validate=is_validate,
+                dependencies=dependencies,
+                _get_dependant=_get_dependant,
+            )
+
+            if _get_dependant is None:
+                self.dependant = dependant
+            else:
+                self.dependant = _get_dependant(self.handler._original_call, dependencies)
+
+    @property
+    def call_name(self) -> str:
+        """Returns the name of the original call."""
+        if self.handler is None:
+            return ""
+
+        caller = unwrap(self.handler._original_call)
+        name = getattr(caller, "__name__", str(caller))
+        return name
+
+    @property
+    def description(self) -> Optional[str]:
+        """Returns the description of original call."""
+        if self.handler is None:
+            return None
+
+        caller = unwrap(self.handler._original_call)
+        description = getattr(caller, "__doc__", None)
+        return description
 
-            if list and (ls := handler.list_sub) is not None:
-                batch = ls.batch
-                call = list == ls.name
-
-            if stream and (st := handler.stream_sub) is not None:
-                batch = st.batch
-                call = stream == st.name
-
-            if call:
-                r = await call_handler(
-                    handler=handler,
-                    message=build_message(
-                        message=[message] if batch else message,
-                        channel=any_of,
-                        headers=headers,
-                        correlation_id=correlation_id,
-                        reply_to=reply_to,
-                    ),
-                    rpc=rpc,
-                    rpc_timeout=rpc_timeout,
-                    raise_timeout=raise_timeout,
-                )
+    async def is_suitable(
+        self,
+        msg: MsgType,
+        cache: Dict[Any, Any],
+    ) -> Optional["StreamMessage[MsgType]"]:
+        """Check is message suite for current filter."""
+        if not (
+            parser := cast(Optional["AsyncParser[MsgType]"], self.item_parser)
+        ) or not (
+            decoder := cast(
+                Optional["AsyncDecoder[StreamMessage[MsgType]]"], self.item_decoder
+            )
+        ):
+            raise SetupError("You should setup `HandlerItem` at first.")
+
+        message = cache[parser] = cast(
+            "StreamMessage[MsgType]", cache.get(parser) or await parser(msg)
+        )
+
+        message.decoded_body = cache[decoder] = cache.get(decoder) or await decoder(
+            message
+        )
 
-                if rpc:  # pragma: no branch
-                    return r
+        if await self.filter(message):
+            return message
 
         return None
 
-    async def publish_batch(
+    async def call(
         self,
-        *msgs: SendableMessage,
-        list: str,
-    ) -> None:
-        for handler in self.broker.handlers.values():  # pragma: no branch
-            if handler.list_sub and handler.list_sub.name == list:
-                await call_handler(
-                    handler=handler,
-                    message=build_message(
-                        message=msgs,
-                        channel=list,
-                    ),
+        /,
+        message: "StreamMessage[MsgType]",
+        _extra_middlewares: Iterable["SubscriberMiddleware"],
+    ) -> Any:
+        """Execute wrapped handler with consume middlewares."""
+        async with AsyncExitStack() as consume_stack:
+            for middleware in chain(self.item_middlewares, _extra_middlewares):
+                message.decoded_body = await consume_stack.enter_async_context(
+                    middleware(message.decoded_body)
                 )
 
-        return None
-
+            try:
+                result = await self.handler.call_wrapped(message)
 
-def build_message(
-    message: Union[Sequence[SendableMessage], SendableMessage],
-    channel: str,
-    *,
-    reply_to: str = "",
-    correlation_id: Optional[str] = None,
-    headers: Optional[AnyDict] = None,
-) -> AnyRedisDict:
-    data = RawMessage.encode(
-        message=message,
-        reply_to=reply_to,
-        headers=headers,
-        correlation_id=correlation_id,
-    )
-    return AnyRedisDict(
-        channel=channel.encode(),
-        data=data.encode(),
-        type="message",
-    )
+            except (IgnoredException, SystemExit):
+                self.handler.trigger()
+                raise
+
+            except Exception as e:
+                self.handler.trigger(error=e)
+                raise e
+
+            else:
+                self.handler.trigger(result=result)
+                return result
```

### Comparing `faststream-0.4.7/faststream/redis/shared/logging.py` & `faststream-0.5.0rc0/faststream/redis/broker/logging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,54 @@
 import logging
-from typing import Any, Optional
+from inspect import Parameter
+from typing import Any, ClassVar, Optional, Union
 
-from typing_extensions import override
+from faststream.broker.core.usecase import BrokerUsecase
+from faststream.log.logging import get_broker_logger
+from faststream.redis.message import BaseMessage
 
-from faststream.broker.core.mixins import LoggingMixin
-from faststream.broker.message import StreamMessage
-from faststream.log import access_logger
-from faststream.types import AnyDict
 
-
-class RedisLoggingMixin(LoggingMixin):
-    """A class to represent a Redis logging mixin."""
+class RedisLoggingBroker(BrokerUsecase[BaseMessage, "Redis[bytes]"]):
+    """A class that extends the LoggingMixin class and adds additional functionality for logging Redis related information."""
 
     _max_channel_name: int
+    __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Optional[logging.Logger] = access_logger,
+        logger: Union[logging.Logger, object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize the Redis logging mixin.
-
-        Args:
-            *args: The arguments.
-            logger: The logger.
-            log_level: The log level.
-            log_fmt: The log format.
-            **kwargs: The keyword arguments.
-        """
         super().__init__(
             *args,
             logger=logger,
+            # TODO: generate unique logger names to not share between brokers
+            default_logger=get_broker_logger(
+                name="redis",
+                default_context={
+                    "channel": "",
+                },
+                message_id_ln=self.__max_msg_id_ln,
+            ),
             log_level=log_level,
             log_fmt=log_fmt,
             **kwargs,
         )
-        self._message_id_ln = 15
         self._max_channel_name = 4
 
-    @override
-    def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[StreamMessage[Any]],
-        channel: str,
-    ) -> AnyDict:
-        return {
-            "channel": channel,
-            **super()._get_log_context(message),
-        }
-
-    @property
-    def fmt(self) -> str:
-        return self._fmt or (
-            "%(asctime)s %(levelname)s - "
+    def get_fmt(self) -> str:
+        return (
+            "%(asctime)s %(levelname)-8s - "
             f"%(channel)-{self._max_channel_name}s | "
-            f"%(message_id)-{self._message_id_ln}s - %(message)s"
+            f"%(message_id)-{self.__max_msg_id_ln}s "
+            "- %(message)s"
         )
 
     def _setup_log_context(
         self,
+        *,
         channel: Optional[str] = None,
     ) -> None:
-        if channel is not None:  # pragma: no branch
-            self._max_channel_name = max((self._max_channel_name, len(channel)))
+        self._max_channel_name = max((self._max_channel_name, len(channel or "")))
```

### Comparing `faststream-0.4.7/faststream/utils/ast.py` & `faststream-0.5.0rc0/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/utils/classes.py` & `faststream-0.5.0rc0/faststream/utils/classes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Optional, cast
+
+from typing_extensions import Self
 
 
 class Singleton:
     """A class to implement the Singleton design pattern.
 
     Attributes:
         _instance : the single instance of the class
 
     Methods:
         __new__ : creates a new instance of the class if it doesn't exist, otherwise returns the existing instance
         _drop : sets the instance to None, allowing a new instance to be created
     """
 
-    _instance: ClassVar[Any] = None
+    _instance: ClassVar[Optional[Self]] = None
 
-    def __new__(cls, *args: Any, **kwargs: Any) -> Any:
+    def __new__(cls, *args: Any, **kwargs: Any) -> Self:
         """Create a singleton instance of a class.
 
         Args:
             *args: Variable length argument list
             **kwargs: Arbitrary keyword arguments
 
         Returns:
             The singleton instance of the class
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-        return cls._instance
+        return cast(Self, cls._instance)
 
     @classmethod
     def _drop(cls) -> None:
         """Drop the instance of a class.
 
         Returns:
             None
```

### Comparing `faststream-0.4.7/faststream/utils/data.py` & `faststream-0.5.0rc0/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/utils/no_cast.py` & `faststream-0.5.0rc0/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/faststream/utils/path.py` & `faststream-0.5.0rc0/faststream/utils/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Callable, Optional, Pattern, Tuple
 
+from faststream.exceptions import SetupError
+
 PARAM_REGEX = re.compile("{([a-zA-Z0-9_]+)}")
 
 
 def compile_path(
     path: str,
     replace_symbol: str,
     patch_regex: Callable[[str], str] = lambda x: x,
@@ -30,15 +32,15 @@
             params.add(param_name)
 
         idx = match.end()
 
     if duplicated_params:
         names = ", ".join(sorted(duplicated_params))
         ending = "s" if len(duplicated_params) > 1 else ""
-        raise ValueError(f"Duplicated param name{ending} {names} at path {path}")
+        raise SetupError(f"Duplicated param name{ending} {names} at path {path}")
 
     if idx == 0:
         regex = None
     else:
         path_regex += re.escape(path[idx:]) + "$"
         regex = re.compile(patch_regex(path_regex))
```

### Comparing `faststream-0.4.7/faststream/utils/context/builders.py` & `faststream-0.5.0rc0/faststream/utils/context/builders.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from inspect import _empty
+from inspect import Parameter
 from typing import Any, Callable, Optional
 
 from faststream.utils.context.types import Context as Context_
 
 
 def Context(  # noqa: N802
     real_name: str = "",
     *,
     cast: bool = False,
-    default: Any = _empty,
+    default: Any = Parameter.empty,
     initial: Optional[Callable[..., Any]] = None,
 ) -> Any:
     return Context_(
         real_name=real_name,
         cast=cast,
         default=default,
         initial=initial,
     )
 
 
 def Header(  # noqa: N802
     real_name: str = "",
     *,
     cast: bool = True,
-    default: Any = _empty,
+    default: Any = Parameter.empty,
 ) -> Any:
     return Context_(
         real_name=real_name,
         cast=cast,
         default=default,
         prefix="message.headers.",
     )
 
 
 def Path(  # noqa: N802
     real_name: str = "",
     *,
     cast: bool = True,
-    default: Any = _empty,
+    default: Any = Parameter.empty,
 ) -> Any:
     return Context_(
         real_name=real_name,
         cast=cast,
         default=default,
         prefix="message.path.",
     )
```

### Comparing `faststream-0.4.7/faststream/utils/context/repository.py` & `faststream-0.5.0rc0/faststream/utils/context/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import contextmanager
 from contextvars import ContextVar, Token
-from inspect import _empty
-from typing import Any, Dict, Iterator, Mapping, cast
+from inspect import Parameter
+from typing import Any, Dict, Iterator, Mapping
 
 from faststream.types import AnyDict
 from faststream.utils.classes import Singleton
 
 __all__ = ("ContextRepo", "context")
 
 
@@ -21,14 +21,21 @@
         Attributes:
             _global_context : a dictionary representing the global context
             _scope_context : a dictionary representing the scope context
         """
         self._global_context = {"context": self}
         self._scope_context = {}
 
+    @property
+    def context(self) -> AnyDict:
+        return {
+            **self._global_context,
+            **{i: j.get() for i, j in self._scope_context.items()},
+        }
+
     def set_global(self, key: str, v: Any) -> None:
         """Sets a value in the global context.
 
         Args:
             key: The key to set in the global context.
             v: The value to set.
 
@@ -82,90 +89,86 @@
         Args:
             key: The key of the local variable to retrieve.
             default: The default value to return if the local variable is not found.
 
         Returns:
             The value of the local variable.
         """
-        context_var = self._scope_context.get(key)
-        if context_var is not None:  # pragma: no branch
+        if (context_var := self._scope_context.get(key)) is not None:
             return context_var.get()
         else:
             return default
 
-    def clear(self) -> None:
-        self._global_context = {"context": self}
-        self._scope_context.clear()
+    @contextmanager
+    def scope(self, key: str, value: Any) -> Iterator[None]:
+        """Sets a local variable and yields control to the caller. After the caller is done, the local variable is reset.
+
+        Args:
+            key: The key of the local variable
+            value: The value to set the local variable to
+
+        Yields:
+            None
+
+        Returns:
+            An iterator that yields None
+        """
+        token = self.set_local(key, value)
+        try:
+            yield
+        finally:
+            self.reset_local(key, token)
 
     def get(self, key: str, default: Any = None) -> Any:
         """Get the value associated with a key.
 
         Args:
             key: The key to retrieve the value for.
             default: The default value to return if the key is not found.
 
         Returns:
             The value associated with the key.
         """
-        return self._global_context.get(key, self.get_local(key, default))
+        if (glob := self._global_context.get(key, Parameter.empty)) is Parameter.empty:
+            return self.get_local(key, default)
+        else:
+            return glob
+
+    def __getattr__(self, __name: str) -> Any:
+        """This is a function that is part of a class. It is used to get an attribute value using the `__getattr__` method.
+
+        Args:
+            __name: The name of the attribute to get.
+
+        Returns:
+            The value of the attribute.
+        """
+        return self.get(__name)
 
     def resolve(self, argument: str) -> Any:
         """Resolve the context of an argument.
 
         Args:
             argument: A string representing the argument.
 
         Returns:
             The resolved context of the argument.
 
         Raises:
-            AttributeError: If the attribute does not exist in the context.
+            AttributeError, KeyError: If the argument does not exist in the context.
         """
         first, *keys = argument.split(".")
 
-        if (v := self.get(first, _empty)) is _empty:
+        if (v := self.get(first, Parameter.empty)) is Parameter.empty:
             raise KeyError(f"`{self.context}` does not contains `{first}` key")
 
         for i in keys:
             v = v[i] if isinstance(v, Mapping) else getattr(v, i)
-        return v
-
-    def __getattr__(self, __name: str) -> Any:
-        """This is a function that is part of a class. It is used to get an attribute value using the `__getattr__` method.
 
-        Args:
-            __name: The name of the attribute to get.
-
-        Returns:
-            The value of the attribute.
-        """
-        return self.get(__name)
-
-    @property
-    def context(self) -> AnyDict:
-        return {
-            **self._global_context,
-            **{i: j.get() for i, j in self._scope_context.items()},
-        }
-
-    @contextmanager
-    def scope(self, key: str, value: Any) -> Iterator[None]:
-        """Sets a local variable and yields control to the caller. After the caller is done, the local variable is reset.
-
-        Args:
-            key: The key of the local variable
-            value: The value to set the local variable to
-
-        Yields:
-            None
+        return v
 
-        Returns:
-            An iterator that yields None
-        """
-        token = self.set_local(key, value)
-        try:
-            yield
-        finally:
-            self.reset_local(key, token)
+    def clear(self) -> None:
+        self._global_context = {"context": self}
+        self._scope_context.clear()
 
 
-context: ContextRepo = cast(ContextRepo, ContextRepo())  # type: ignore[redundant-cast]
+context = ContextRepo()
```

### Comparing `faststream-0.4.7/faststream/utils/context/types.py` & `faststream-0.5.0rc0/faststream/utils/context/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from inspect import _empty
+from inspect import Parameter
 from typing import Any, Callable, Optional
 
 from fast_depends.library import CustomField
 
 from faststream.types import AnyDict
 from faststream.utils.context.repository import context
 
@@ -20,15 +20,15 @@
 
     param_name: str
 
     def __init__(
         self,
         real_name: str = "",
         *,
-        default: Any = _empty,
+        default: Any = Parameter.empty,
         initial: Optional[Callable[..., Any]] = None,
         cast: bool = False,
         prefix: str = "",
     ) -> None:
         """Initialize the object.
 
         Args:
@@ -43,15 +43,15 @@
         """
         self.name = real_name
         self.default = default
         self.prefix = prefix
         self.initial = initial
         super().__init__(
             cast=cast,
-            required=(default is _empty),
+            required=(default is Parameter.empty),
         )
 
     def use(self, /, **kwargs: Any) -> AnyDict:
         """Use the given keyword arguments.
 
         Args:
             **kwargs: Keyword arguments to be used
@@ -67,32 +67,32 @@
 
         if (
             v := resolve_context_by_name(
                 name=name,
                 default=self.default,
                 initial=self.initial,
             )
-        ) is not _empty:
+        ) is not Parameter.empty:
             kwargs[self.param_name] = v
 
         return kwargs
 
 
 def resolve_context_by_name(
     name: str,
     default: Any,
     initial: Optional[Callable[..., Any]],
 ) -> Any:
-    value: Any = _empty
+    value: Any = Parameter.empty
 
     try:
         value = context.resolve(name)
 
     except (KeyError, AttributeError):
-        if default is not _empty:
+        if default is not Parameter.empty:
             value = default
 
         elif initial is not None:
             value = initial()
             context.set_global(name, value)
 
     return value
```

### Comparing `faststream-0.4.7/scripts/build-docs-pre-commit.sh` & `faststream-0.5.0rc0/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/scripts/lint-pre-commit.sh` & `faststream-0.5.0rc0/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/scripts/set_variables.sh` & `faststream-0.5.0rc0/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/scripts/static-pre-commit.sh` & `faststream-0.5.0rc0/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/LICENSE` & `faststream-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.4.7/README.md` & `faststream-0.5.0rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 [**FastStream**](https://faststream.airt.ai/latest/) simplifies the process of writing producers and consumers for message queues, handling all the
 parsing, networking and documentation generation automatically.
 
 Making streaming microservices has never been easier. Designed with junior developers in mind, **FastStream** simplifies your work while keeping the door open for more advanced use cases. Here's a look at the core features that make **FastStream** a go-to framework for modern, data-centric microservices.
 
 - **Multiple Brokers**: **FastStream** provides a unified API to work across multiple message brokers ([**Kafka**](https://kafka.apache.org/), [**RabbitMQ**](https://www.rabbitmq.com/), [**NATS**](https://nats.io/), [**Redis**](https://redis.io/) support)
 
-- [**Pydantic Validation**](#writing-app-code): Leverage [**Pydantic's**](https://docs.pydantic.dev/) validation capabilities to serialize and validates incoming messages
+- [**Pydantic Validation**](#writing-app-code): Leverage [**Pydantic's**](https://docs.pydantic.dev/) validation capabilities to serialize and validate incoming messages
 
 - [**Automatic Docs**](#project-documentation): Stay ahead with automatic [**AsyncAPI**](https://www.asyncapi.com/) documentation
 
 - **Intuitive**: Full-typed editor support makes your development experience smooth, catching errors before they reach runtime
 
 - [**Powerful Dependency Injection System**](#dependencies): Manage your service dependencies efficiently with **FastStream**'s built-in DI system
 
@@ -349,15 +349,15 @@
 ``` shell
 faststream_gen -i description.txt
 ```
 
 ``` shell
 ✨  Generating a new FastStream application!
  ✔ Application description validated.
- ✔ FastStream app skeleton code generated. akes around 15 to 45 seconds)...
+ ✔ FastStream app skeleton code generated. Takes around 15 to 45 seconds)...
  ✔ The app and the tests are generated.  around 30 to 90 seconds)...
  ✔ New FastStream project created.
  ✔ Integration tests were successfully completed.
  Tokens used: 10768
  Total Cost (USD): $0.03284
 ✨  All files were successfully generated!
 ```
```

### Comparing `faststream-0.4.7/pyproject.toml` & `faststream-0.5.0rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,25 @@
 
 [project]
 name = "faststream"
 description = "FastStream: the simplest way to work with a messaging queues"
 readme = "README.md"
 authors = [
     { name = "airt", email = "info@airt.ai" },
-    { name = "lancetnik", email = "diementros@gmail.com" },
+    { name = "Nikita Pastukhov", email = "nikita@pastukhov-dev.ru" },
 ]
 
-keywords = ["rabbitmq", "kafka", "framework", "nats", "redis", "message brokers"]
+keywords = [
+    "rabbitmq",
+    "kafka",
+    "framework",
+    "nats",
+    "redis",
+    "message brokers",
+]
 
 requires-python = ">=3.8"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -24,19 +31,20 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
-    "Topic :: Internet",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
+    "Topic :: System :: Networking",
+    "Topic :: System :: Distributed Computing",
     "Typing :: Typed",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
@@ -45,98 +53,84 @@
 ]
 
 dynamic = ["version"]
 
 dependencies = [
     "anyio>=3.7.1,<5",
     "fast-depends>=2.4.0b0,<2.5.0",
-    "typer>=0.9,<1",
+    "typer>=0.9,!=0.12,<1",
     "typing-extensions>=4.8.0",
 ]
 
 [project.optional-dependencies]
 # public distributions
-rabbit = [
-    "aio-pika>=9,<10",
-]
+rabbit = ["aio-pika>=9,<10"]
 
-kafka = [
-    "aiokafka>=0.9,<0.11",
-]
+kafka = ["aiokafka>=0.9,<0.11"]
 
-confluent = [
-    "confluent-kafka>=2,<3",
-]
+confluent = ["confluent-kafka>=2,<3"]
 
 nats = [
-    "nats-py>=2.3.1,<=2.7.0"
-]
-
-redis = [
-    "redis>=5.0.0,<6.0.0"
+    "nats-py>=2.3.1,<=3.0.0"
 ]
 
-docs = [
-    "fastapi>=0.100.0,<1.0.0",
-    "uvicorn>=0.17.0,<1.0.0",
-]
+redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
-    "mkdocs-material==9.5.11",
+    "mkdocs-material==9.5.13",
     "mkdocs-static-i18n==1.2.0",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.24.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.4",
     "mike==2.0.0",  # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",  # includes with variables
     "mkdocs-glightbox==0.3.7",  # img zoom
-    "pillow==10.2.0",
-    "cairosvg==2.7.1",
-    "black==24.1.1",
-    "requests",  # do not pin it
+    "pillow==10.2.0",  # required for mkdocs-glightbo
+    "cairosvg==2.7.1",  # required for mkdocs-glightbo
+    "requests",  # using in CI, do not pin it
 ]
 
 lint = [
+    # mypy extensions
     "types-PyYAML",
     "types-setuptools",
     "types-ujson",
     "types-redis",
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
-    "mypy==1.8.0",
+    "mypy==1.9.0",
     "ruff==0.3.0",
-    "bandit==1.7.7",
-    "semgrep==1.62.0",
+    "bandit==1.7.8",
+    "semgrep==1.66.0",
+    "codespell==2.2.6",
 ]
 
 test-core = [
-    "coverage[toml]==7.4.3",
-    "pytest==8.0.1",
-    "pytest-asyncio==0.23.5",
+    "coverage[toml]==7.4.4",
+    "pytest==8.1.1",
+    "pytest-asyncio==0.23.5.post1",
     "dirty-equals==0.7.1.post0",
-    "pytest-timeout==2.2.0",
-    "pytest-rerunfailures==13.0",
 ]
 
 testing = [
     "faststream[test-core]",
     "fastapi==0.109.2",
     "pydantic-settings>=2.0.0,<3.0.0",
     "httpx==0.27.0",
     "PyYAML==6.0.1",
     "watchfiles==0.21.0",
     "email-validator==2.1.1",
 ]
 
 dev = [
-    "faststream[rabbit,kafka,confluent,nats,docs,redis,lint,testing,devdocs]",
+    "faststream[rabbit,kafka,confluent,nats,redis,lint,testing,devdocs]",
     "pre-commit==3.5.0; python_version < '3.9'",
     "pre-commit==3.6.2; python_version >= '3.9'",
     "detect-secrets==1.4.0",
 ]
 
 [project.urls]
 Homepage = "https://faststream.airt.ai/latest/"
@@ -149,28 +143,23 @@
 faststream = "faststream.__main__:cli"
 
 [tool.hatch.version]
 path = "faststream/__about__.py"
 
 [tool.hatch.build]
 skip-excluded-dirs = true
-exclude = [
-    "/tests",
-    "/docs",
-]
+exclude = ["/tests", "/docs"]
 
 [tool.mypy]
 strict = true
 python_version = "3.8"
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
-plugins = [
-    "pydantic.mypy"
-]
+plugins = ["pydantic.mypy"]
 
 # from https://blog.wolt.com/engineering/2021/09/30/professional-grade-mypy-configuration/
 disallow_untyped_defs = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_return_any = true
 show_error_codes = true
@@ -180,15 +169,21 @@
 disallow_untyped_decorators = true
 disallow_any_unimported = false
 
 [tool.ruff]
 fix = true
 line-length = 88
 target-version = "py38"
-include = ["faststream/**/*.py", "faststream/**/*.pyi", "tests/**/*.py", "docs/**/*.py", "pyproject.toml"]
+include = [
+    "faststream/**/*.py",
+    "faststream/**/*.pyi",
+    "tests/**/*.py",
+    "docs/**/*.py",
+    "pyproject.toml",
+]
 exclude = ["docs/docs_src"]
 
 [tool.ruff.lint]
 select = [
     "E",     # pycodestyle errors     https://docs.astral.sh/ruff/rules/#error-e
     "W",     # pycodestyle warnings   https://docs.astral.sh/ruff/rules/#warning-w
     "C90",   # mccabe                 https://docs.astral.sh/ruff/rules/#mccabe-c90
@@ -207,89 +202,84 @@
     "TCH",   # flake8-type-checking   https://docs.astral.sh/ruff/rules/#flake8-type-checking-tch
     "RUF",   # Ruff-specific rules    https://docs.astral.sh/ruff/rules/#ruff-specific-rules-ruf
     "PERF",  # Perflint               https://docs.astral.sh/ruff/rules/#perflint-perf
     "UP",    # pyupgrade              https://docs.astral.sh/ruff/rules/#pyupgrade-up
 ]
 
 ignore = [
-    "E501",  # line too long, handled by formatter later
-    "C901",  # too complex
-    "D418",  # Function decorated with `@overload` shouldn't contain a docstring
+    "E501", # line too long, handled by formatter later
+    "C901", # too complex
 
     # todo pep8-naming
-    "N817",  # CamelCase `*` imported as acronym `*`
-    "N815",  # Variable `*` in class scope should not be mixedCase
-    "N803",  # Argument name `expandMessageExamples` should be lowercase
+    "N817", # CamelCase `*` imported as acronym `*`
+    "N815", # Variable `*` in class scope should not be mixedCase
+    "N803", # Argument name `expandMessageExamples` should be lowercase
 
     # todo pydocstyle
-    "D100",  # missing docstring in public module
+    "D100", # missing docstring in public module
+    "D104", # missing docstring in public package
+    "D105", # missing docstring in magic methods
+    "D106", # missing docstring in public nested class
+    "D107", # missing docstring in __init__
+]
+
+[tool.ruff.lint.per-file-ignores]
+"tests/**" = [
+    "D101",       # docstrings
     "D102",
     "D103",
-    "D104",  # missing docstring in public package
-    "D105",
-    "D106",  # Missing docstring in public nested class
+    "PLR2004", # magic-value-comparison 
+    "S101",    # use assert
 ]
 
 [tool.ruff.lint.isort]
 case-sensitive = true
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = [
-    "faststream.Depends", "faststream.Context", "faststream.broker.fastapi.context.Context",
-    "faststream.Header", "faststream.Path",
-    "faststream.utils.Header", "faststream.utils.Path",
-    "faststream.utils.Depends", "faststream.utils.Context",
-    "faststream.utils.context.Depends", "faststream.utils.context.Context",
-    "typer.Argument", "typer.Option",
-    "pydantic.Field", "rocketry.args.Arg",
-    "fastapi.Depends", "fastapi.Header",
+    "faststream.Depends",
+    "faststream.Context",
+    "faststream.broker.fastapi.context.Context",
+    "faststream.Header",
+    "faststream.Path",
+    "faststream.utils.Header",
+    "faststream.utils.Path",
+    "faststream.utils.Depends",
+    "faststream.utils.Context",
+    "faststream.utils.context.Depends",
+    "faststream.utils.context.Context",
+    "typer.Argument",
+    "typer.Option",
+    "pydantic.Field",
+    "rocketry.args.Arg",
+    "fastapi.Depends",
+    "fastapi.Header",
     "fastapi.datastructures.Default",
     "kafka.partitioner.default.DefaultPartitioner",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q -m 'not slow'"
-testpaths = [
-    "tests",
-]
-markers = [
-    "rabbit",
-    "kafka",
-    "confluent",
-    "nats",
-    "redis",
-    "slow",
-    "all",
-]
+testpaths = ["tests"]
+markers = ["rabbit", "kafka", "confluent", "nats", "redis", "slow", "all"]
 
 [tool.coverage.run]
 parallel = true
 branch = true
-concurrency = [
-    "multiprocessing",
-    "thread"
-]
-source = [
-    "docs/docs_src",
-    "examples",
-    "faststream",
-    "tests"
-]
+concurrency = ["multiprocessing", "thread"]
+source = ["docs/docs_src", "examples", "faststream", "tests"]
 context = '${CONTEXT}'
-omit = [
-    "**/__init__.py",
-    "tests/mypy/*",
-]
+omit = ["**/__init__.py", "tests/mypy/*"]
 
 [tool.coverage.report]
 show_missing = true
 skip_empty = true
 exclude_also = [
     "if __name__ == .__main__.:",
     "self.logger",
@@ -324,9 +314,9 @@
     'examples/serialization/msgpack/pack.py',
     'examples/serialization/protobuf/protobuf.py',
 ]
 
 [tool.bandit]
 
 [tool.codespell]
-
+skip = "./venv,./docs/site/*"
 ignore-words = ".codespell-whitelist.txt"
```

### Comparing `faststream-0.4.7/PKG-INFO` & `faststream-0.5.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: faststream
-Version: 0.4.7
+Version: 0.5.0rc0
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
-Author-email: airt <info@airt.ai>, lancetnik <diementros@gmail.com>
+Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
 License-File: LICENSE
 Keywords: framework,kafka,message brokers,nats,rabbitmq,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
@@ -26,77 +26,73 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: anyio<5,>=3.7.1
 Requires-Dist: fast-depends<2.5.0,>=2.4.0b0
-Requires-Dist: typer<1,>=0.9
+Requires-Dist: typer!=0.12,<1,>=0.9
 Requires-Dist: typing-extensions>=4.8.0
 Provides-Extra: confluent
 Requires-Dist: confluent-kafka<3,>=2; extra == 'confluent'
 Provides-Extra: dev
 Requires-Dist: detect-secrets==1.4.0; extra == 'dev'
-Requires-Dist: faststream[confluent,devdocs,docs,kafka,lint,nats,rabbit,redis,testing]; extra == 'dev'
+Requires-Dist: faststream[confluent,devdocs,kafka,lint,nats,rabbit,redis,testing]; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.6.2; (python_version >= '3.9') and extra == 'dev'
 Provides-Extra: devdocs
-Requires-Dist: black==24.1.1; extra == 'devdocs'
 Requires-Dist: cairosvg==2.7.1; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
 Requires-Dist: mike==2.0.0; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
-Requires-Dist: mkdocs-material==9.5.11; extra == 'devdocs'
+Requires-Dist: mkdocs-material==9.5.13; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.0; extra == 'devdocs'
 Requires-Dist: mkdocstrings[python]==0.24.1; extra == 'devdocs'
 Requires-Dist: pillow==10.2.0; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
-Provides-Extra: docs
-Requires-Dist: fastapi<1.0.0,>=0.100.0; extra == 'docs'
-Requires-Dist: uvicorn<1.0.0,>=0.17.0; extra == 'docs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
-Requires-Dist: bandit==1.7.7; extra == 'lint'
+Requires-Dist: bandit==1.7.8; extra == 'lint'
+Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
-Requires-Dist: mypy==1.8.0; extra == 'lint'
+Requires-Dist: mypy==1.9.0; extra == 'lint'
 Requires-Dist: ruff==0.3.0; extra == 'lint'
-Requires-Dist: semgrep==1.62.0; extra == 'lint'
+Requires-Dist: semgrep==1.66.0; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
-Requires-Dist: nats-py<=2.7.0,>=2.3.1; extra == 'nats'
+Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'nats'
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
-Requires-Dist: coverage[toml]==7.4.3; extra == 'test-core'
+Requires-Dist: coverage[toml]==7.4.4; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
-Requires-Dist: pytest-asyncio==0.23.5; extra == 'test-core'
-Requires-Dist: pytest-rerunfailures==13.0; extra == 'test-core'
-Requires-Dist: pytest-timeout==2.2.0; extra == 'test-core'
-Requires-Dist: pytest==8.0.1; extra == 'test-core'
+Requires-Dist: pytest-asyncio==0.23.5.post1; extra == 'test-core'
+Requires-Dist: pytest==8.1.1; extra == 'test-core'
 Provides-Extra: testing
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.109.2; extra == 'testing'
 Requires-Dist: faststream[test-core]; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
@@ -160,15 +156,15 @@
 [**FastStream**](https://faststream.airt.ai/latest/) simplifies the process of writing producers and consumers for message queues, handling all the
 parsing, networking and documentation generation automatically.
 
 Making streaming microservices has never been easier. Designed with junior developers in mind, **FastStream** simplifies your work while keeping the door open for more advanced use cases. Here's a look at the core features that make **FastStream** a go-to framework for modern, data-centric microservices.
 
 - **Multiple Brokers**: **FastStream** provides a unified API to work across multiple message brokers ([**Kafka**](https://kafka.apache.org/), [**RabbitMQ**](https://www.rabbitmq.com/), [**NATS**](https://nats.io/), [**Redis**](https://redis.io/) support)
 
-- [**Pydantic Validation**](#writing-app-code): Leverage [**Pydantic's**](https://docs.pydantic.dev/) validation capabilities to serialize and validates incoming messages
+- [**Pydantic Validation**](#writing-app-code): Leverage [**Pydantic's**](https://docs.pydantic.dev/) validation capabilities to serialize and validate incoming messages
 
 - [**Automatic Docs**](#project-documentation): Stay ahead with automatic [**AsyncAPI**](https://www.asyncapi.com/) documentation
 
 - **Intuitive**: Full-typed editor support makes your development experience smooth, catching errors before they reach runtime
 
 - [**Powerful Dependency Injection System**](#dependencies): Manage your service dependencies efficiently with **FastStream**'s built-in DI system
 
@@ -454,15 +450,15 @@
 ``` shell
 faststream_gen -i description.txt
 ```
 
 ``` shell
 ✨  Generating a new FastStream application!
  ✔ Application description validated.
- ✔ FastStream app skeleton code generated. akes around 15 to 45 seconds)...
+ ✔ FastStream app skeleton code generated. Takes around 15 to 45 seconds)...
  ✔ The app and the tests are generated.  around 30 to 90 seconds)...
  ✔ New FastStream project created.
  ✔ Integration tests were successfully completed.
  Tokens used: 10768
  Total Cost (USD): $0.03284
 ✨  All files were successfully generated!
 ```
```

