# Comparing `tmp/baseplate-2.7.0b1.tar.gz` & `tmp/baseplate-2.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseplate-2.7.0b1.tar", max compression
+gzip compressed data, was "baseplate-2.7.0b2.tar", max compression
```

## Comparing `baseplate-2.7.0b1.tar` & `baseplate-2.7.0b2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1476 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/LICENSE
--rw-r--r--   0        0        0     2784 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/README.md
--rw-r--r--   0        0        0    26348 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/clients/__init__.py
--rw-r--r--   0        0        0    16053 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/clients/cassandra.py
--rw-r--r--   0        0        0    11682 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/kombu.py
--rw-r--r--   0        0        0    16132 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/memcache/__init__.py
--rw-r--r--   0        0        0     8464 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/memcache/lib.py
--rw-r--r--   0        0        0    14548 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/redis.py
--rw-r--r--   0        0        0    22396 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/redis_cluster.py
--rw-r--r--   0        0        0    17110 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/requests.py
--rw-r--r--   0        0        0    13557 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/sqlalchemy.py
--rw-r--r--   0        0        0    15350 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/thrift.py
--rw-r--r--   0        0        0      162 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/__init__.py
--rw-r--r--   0        0        0    16283 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/pyramid/__init__.py
--rw-r--r--   0        0        0     5341 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/pyramid/csrf.py
--rw-r--r--   0        0        0        0 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/__init__.py
--rw-r--r--   0        0        0    24917 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kafka.py
--rw-r--r--   0        0        0    18799 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kombu.py
--rw-r--r--   0        0        0    10209 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/thrift/__init__.py
--rw-r--r--   0        0        0     2627 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/thrift/command.py
--rw-r--r--   0        0        0     1827 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/_requests.py
--rw-r--r--   0        0        0    17148 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/config.py
--rw-r--r--   0        0        0     5390 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/crypto.py
--rw-r--r--   0        0        0     1016 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/datetime.py
--rw-r--r--   0        0        0      447 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/edgecontext.py
--rw-r--r--   0        0        0      490 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/errors.py
--rw-r--r--   0        0        0     3964 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/events.py
--rw-r--r--   0        0        0     7004 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/file_watcher.py
--rw-r--r--   0        0        0      120 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/__init__.py
--rw-r--r--   0        0        0     3277 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/writer.py
--rw-r--r--   0        0        0     3724 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/zookeeper.py
--rw-r--r--   0        0        0      697 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/log_formatter.py
--rw-r--r--   0        0        0     5653 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/message_queue.py
--rw-r--r--   0        0        0    19944 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/metrics.py
--rw-r--r--   0        0        0     1621 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/prometheus_metrics.py
--rw-r--r--   0        0        0     3250 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/random.py
--rw-r--r--   0        0        0      290 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/__init__.py
--rw-r--r--   0        0        0      868 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/__init__.py
--rw-r--r--   0        0        0     2660 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/memcache.py
--rw-r--r--   0        0        0     2560 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/redis.py
--rw-r--r--   0        0        0     2765 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/ratelimit.py
--rw-r--r--   0        0        0     4217 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/retry.py
--rw-r--r--   0        0        0    17956 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/secrets.py
--rw-r--r--   0        0        0     3904 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/service_discovery.py
--rw-r--r--   0        0        0    10377 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/thrift_pool.py
--rw-r--r--   0        0        0      250 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/__init__.py
--rw-r--r--   0        0        0     3481 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/db_query_string_format_plugin.py
--rw-r--r--   0        0        0     2675 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/example_plugin.py
--rw-r--r--   0        0        0        0 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/__init__.py
--rw-r--r--   0        0        0      578 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/logging.py
--rw-r--r--   0        0        0     5918 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/metrics.py
--rw-r--r--   0        0        0     7971 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/metrics_tagged.py
--rw-r--r--   0        0        0     5687 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/sentry.py
--rw-r--r--   0        0        0     2703 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/timeout.py
--rw-r--r--   0        0        0    22594 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/tracing.py
--rw-r--r--   0        0        0       71 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/py.typed
--rw-r--r--   0        0        0    18997 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/__init__.py
--rw-r--r--   0        0        0       81 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/__main__.py
--rw-r--r--   0        0        0     2166 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/einhorn.py
--rw-r--r--   0        0        0     2704 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/healthcheck.py
--rw-r--r--   0        0        0      581 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/monkey.py
--rw-r--r--   0        0        0      971 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/net.py
--rw-r--r--   0        0        0     3358 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/prometheus.py
--rw-r--r--   0        0        0    12793 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/queue_consumer.py
--rw-r--r--   0        0        0     1944 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/reloader.py
--rw-r--r--   0        0        0    10523 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/runtime_monitor.py
--rw-r--r--   0        0        0     2730 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/thrift.py
--rw-r--r--   0        0        0     1733 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/server/wsgi.py
--rw-r--r--   0        0        0     1924 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/__init__.py
--rw-r--r--   0        0        0     8097 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/event_publisher.py
--rw-r--r--   0        0        0    10475 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/live_data_watcher.py
--rw-r--r--   0        0        0    15929 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/secrets_fetcher.py
--rw-r--r--   0        0        0     6678 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/trace_publisher.py
--rw-r--r--   0        0        0        0 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/__init__.py
--rw-r--r--   0        0        0     1409 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/file_watcher.py
--rw-r--r--   0        0        0     1250 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/secrets.py
--rw-r--r--   0        0        0     8857 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/BaseplateService.py
--rw-r--r--   0        0        0     9586 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/BaseplateServiceV2.py
--rw-r--r--   0        0        0       76 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/__init__.py
--rw-r--r--   0        0        0     8232 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/baseplate.thrift
--rw-r--r--   0        0        0      472 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/constants.py
--rw-r--r--   0        0        0    13730 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/ttypes.py
--rwxr-xr-x   0        0        0      138 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-healthcheck
--rwxr-xr-x   0        0        0      453 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-script
--rwxr-xr-x   0        0        0      461 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-serve
--rwxr-xr-x   0        0        0      451 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-shell
--rwxr-xr-x   0        0        0      554 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-tshell
--rw-r--r--   0        0        0     3323 2024-04-30 19:26:16.046085 baseplate-2.7.0b1/pyproject.toml
--rw-r--r--   0        0        0     5270 1970-01-01 00:00:00.000000 baseplate-2.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1476 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/LICENSE
+-rw-r--r--   0        0        0     2784 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/README.md
+-rw-r--r--   0        0        0    26348 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/__init__.py
+-rw-r--r--   0        0        0    16053 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/cassandra.py
+-rw-r--r--   0        0        0    11682 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/kombu.py
+-rw-r--r--   0        0        0    16132 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/memcache/__init__.py
+-rw-r--r--   0        0        0     8464 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/memcache/lib.py
+-rw-r--r--   0        0        0    14548 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/redis.py
+-rw-r--r--   0        0        0    22396 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/redis_cluster.py
+-rw-r--r--   0        0        0    17110 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/requests.py
+-rw-r--r--   0        0        0    13557 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/sqlalchemy.py
+-rw-r--r--   0        0        0    15350 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/clients/thrift.py
+-rw-r--r--   0        0        0      162 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/__init__.py
+-rw-r--r--   0        0        0    16283 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/pyramid/__init__.py
+-rw-r--r--   0        0        0     5341 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/pyramid/csrf.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/queue_consumer/__init__.py
+-rw-r--r--   0        0        0    26217 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/queue_consumer/kafka.py
+-rw-r--r--   0        0        0    18799 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/queue_consumer/kombu.py
+-rw-r--r--   0        0        0    10209 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/thrift/__init__.py
+-rw-r--r--   0        0        0     2627 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/frameworks/thrift/command.py
+-rw-r--r--   0        0        0     1827 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/__init__.py
+-rw-r--r--   0        0        0     1730 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/_requests.py
+-rw-r--r--   0        0        0    17148 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/config.py
+-rw-r--r--   0        0        0     5390 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/crypto.py
+-rw-r--r--   0        0        0     1016 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/datetime.py
+-rw-r--r--   0        0        0      447 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/edgecontext.py
+-rw-r--r--   0        0        0      490 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/errors.py
+-rw-r--r--   0        0        0     3964 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/events.py
+-rw-r--r--   0        0        0     7004 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/file_watcher.py
+-rw-r--r--   0        0        0      120 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/live_data/__init__.py
+-rw-r--r--   0        0        0     3277 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/live_data/writer.py
+-rw-r--r--   0        0        0     3724 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/live_data/zookeeper.py
+-rw-r--r--   0        0        0      697 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/log_formatter.py
+-rw-r--r--   0        0        0     5653 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/message_queue.py
+-rw-r--r--   0        0        0    19944 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/metrics.py
+-rw-r--r--   0        0        0     1621 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/prometheus_metrics.py
+-rw-r--r--   0        0        0     3250 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/random.py
+-rw-r--r--   0        0        0      290 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/ratelimit/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/memcache.py
+-rw-r--r--   0        0        0     2560 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/redis.py
+-rw-r--r--   0        0        0     2765 2024-05-30 16:46:30.763566 baseplate-2.7.0b2/baseplate/lib/ratelimit/ratelimit.py
+-rw-r--r--   0        0        0     4217 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lib/retry.py
+-rw-r--r--   0        0        0    17956 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lib/secrets.py
+-rw-r--r--   0        0        0     3904 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lib/service_discovery.py
+-rw-r--r--   0        0        0    10377 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lib/thrift_pool.py
+-rw-r--r--   0        0        0      250 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lint/__init__.py
+-rw-r--r--   0        0        0     3481 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lint/db_query_string_format_plugin.py
+-rw-r--r--   0        0        0     2675 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/lint/example_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/__init__.py
+-rw-r--r--   0        0        0      578 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/logging.py
+-rw-r--r--   0        0        0     5918 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/metrics.py
+-rw-r--r--   0        0        0     7971 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/metrics_tagged.py
+-rw-r--r--   0        0        0     5687 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/sentry.py
+-rw-r--r--   0        0        0     2703 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/timeout.py
+-rw-r--r--   0        0        0    22594 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/observers/tracing.py
+-rw-r--r--   0        0        0       71 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/py.typed
+-rw-r--r--   0        0        0    18997 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/__main__.py
+-rw-r--r--   0        0        0     2166 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/einhorn.py
+-rw-r--r--   0        0        0     2704 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/healthcheck.py
+-rw-r--r--   0        0        0      581 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/monkey.py
+-rw-r--r--   0        0        0      971 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/net.py
+-rw-r--r--   0        0        0     3358 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/prometheus.py
+-rw-r--r--   0        0        0    12793 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/queue_consumer.py
+-rw-r--r--   0        0        0     1944 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/reloader.py
+-rw-r--r--   0        0        0    10523 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/runtime_monitor.py
+-rw-r--r--   0        0        0     2730 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/thrift.py
+-rw-r--r--   0        0        0     1733 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/server/wsgi.py
+-rw-r--r--   0        0        0     1924 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/sidecars/__init__.py
+-rw-r--r--   0        0        0     8097 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/sidecars/event_publisher.py
+-rw-r--r--   0        0        0    10475 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/sidecars/live_data_watcher.py
+-rw-r--r--   0        0        0    15929 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/sidecars/secrets_fetcher.py
+-rw-r--r--   0        0        0     6678 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/sidecars/trace_publisher.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/testing/lib/__init__.py
+-rw-r--r--   0        0        0     1409 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/testing/lib/file_watcher.py
+-rw-r--r--   0        0        0     1250 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/testing/lib/secrets.py
+-rw-r--r--   0        0        0     8857 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/BaseplateService.py
+-rw-r--r--   0        0        0     9586 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/BaseplateServiceV2.py
+-rw-r--r--   0        0        0       76 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/__init__.py
+-rw-r--r--   0        0        0     8232 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/baseplate.thrift
+-rw-r--r--   0        0        0      472 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/constants.py
+-rw-r--r--   0        0        0    13730 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/baseplate/thrift/ttypes.py
+-rwxr-xr-x   0        0        0      138 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/bin/baseplate-healthcheck
+-rwxr-xr-x   0        0        0      578 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/bin/baseplate-script
+-rwxr-xr-x   0        0        0      586 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/bin/baseplate-serve
+-rwxr-xr-x   0        0        0      576 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/bin/baseplate-shell
+-rwxr-xr-x   0        0        0      679 2024-05-30 16:46:30.767566 baseplate-2.7.0b2/bin/baseplate-tshell
+-rw-r--r--   0        0        0     3403 2024-05-30 16:46:30.775566 baseplate-2.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 baseplate-2.7.0b2/PKG-INFO
```

### Comparing `baseplate-2.7.0b1/LICENSE` & `baseplate-2.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/README.md` & `baseplate-2.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/__init__.py` & `baseplate-2.7.0b2/baseplate/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/__init__.py` & `baseplate-2.7.0b2/baseplate/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/cassandra.py` & `baseplate-2.7.0b2/baseplate/clients/cassandra.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/kombu.py` & `baseplate-2.7.0b2/baseplate/clients/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/memcache/__init__.py` & `baseplate-2.7.0b2/baseplate/clients/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/memcache/lib.py` & `baseplate-2.7.0b2/baseplate/clients/memcache/lib.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/redis.py` & `baseplate-2.7.0b2/baseplate/clients/redis.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/redis_cluster.py` & `baseplate-2.7.0b2/baseplate/clients/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/requests.py` & `baseplate-2.7.0b2/baseplate/clients/requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/sqlalchemy.py` & `baseplate-2.7.0b2/baseplate/clients/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/clients/thrift.py` & `baseplate-2.7.0b2/baseplate/clients/thrift.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/pyramid/__init__.py` & `baseplate-2.7.0b2/baseplate/frameworks/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/pyramid/csrf.py` & `baseplate-2.7.0b2/baseplate/frameworks/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kafka.py` & `baseplate-2.7.0b2/baseplate/frameworks/queue_consumer/kafka.py`

 * *Files 3% similar despite different names*

```diff
@@ -400,29 +400,44 @@
 
     The `InOrderConsumerFactory` attempts to achieve in order, exactly once
     message processing.
 
     This will run a single `KafkaConsumerWorker` that reads messages from Kafka and
     puts them into an internal work queue. Then it will run a single `KafkaMessageHandler`
     that reads messages from the internal work queue, processes them with the
-    `handler_fn`, and then commits each message's offset to Kafka.
+    `handler_fn`, and then commits each message's offset to the kafka consumer's internal state.
+
+    The Kafka Consumer will commit the offsets back to Kafka based on the auto.commit.interval.ms default which is 5 seconds
 
     This one-at-a-time, in-order processing ensures that when a failure happens
     during processing we don't commit its offset (or the offset of any later
     messages) and that when the server restarts it will receive the failed
     message and attempt to process it again. Additionally, because each
     message's offset is committed immediately after processing we should
     never process a message more than once.
 
     For most cases where you just need a basic consumer with sensible defaults
     you can use `InOrderConsumerFactory.new`.
 
     If you need more control, you can create the :py:class:`~confluent_kafka.Consumer`
     yourself and use the constructor directly.
 
+    UPDATE: The InOrderConsumerFactory can NEVER achieve in-order, exactly once message processing.
+
+    Message processing in Kafka to enable exactly once starts at the Producer enabling transactions,
+    and downstream consumers enabling reading exclusively from the committed offsets within a transactions.
+
+    Secondly, without defined keys in the messages from the producer, messages will be sent in a round robin fashion to all partitions in the topic.
+    This means that newer messages could be consumed before older ones if the consumer of those partitions with newer messages are faster.
+
+    Some improvements are made instead that retain the current behaviour, but don't put as much pressure on Kafka by committing every single offset.
+
+    Instead of committing every single message's offset back to Kafka,
+    the consumer now commits each offset to it's local offset store, and commits the highest seen value for each partition at a defined interval (auto.commit.interval.ms).
+    "enable.auto.offset.store" is set to false to give our application explicit control of when to store offsets.
     """
 
     # we need to ensure that only a single message handler worker exists (max_concurrency = 1)
     # otherwise we could have out of order processing and mess up committing offsets to kafka!
     message_handler_count = 0
 
     @classmethod
@@ -440,16 +455,17 @@
             # will rebalance in order to reassign the partitions to another consumer
             # group member.
             # Note: It is recommended to set enable.auto.offset.store=false for
             # long-time processing applications and then explicitly store offsets
             # after message processing, to make sure offsets are not auto-committed
             # prior to processing has finished.
             "max.poll.interval.ms": 300000,
-            # disable offset autocommit, we'll manually commit.
-            "enable.auto.commit": "false",
+            # Enable offset autocommit, but disable offset store.
+            "enable.auto.commit": "true",
+            "enable.auto.offset.store": "false",
         }
 
     def build_message_handler(self) -> KafkaMessageHandler:
         assert self.message_handler_count == 0, "Can only run 1 message handler!"
 
         self.message_handler_count += 1
 
@@ -460,15 +476,15 @@
             logger.debug(
                 "committing topic %s partition %s offset %s",
                 message.topic(),
                 message.partition(),
                 message.offset(),
             )
             with context.span.make_child("kafka.commit"):
-                self.consumer.commit(message=message, asynchronous=False)
+                self.consumer.store_offsets(message=message)
 
         return KafkaMessageHandler(
             self.baseplate,
             self.name,
             self.handler_fn,
             self.message_unpack_fn,
             # commit offset after each successful message handle()
```

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kombu.py` & `baseplate-2.7.0b2/baseplate/frameworks/queue_consumer/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/thrift/__init__.py` & `baseplate-2.7.0b2/baseplate/frameworks/thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/frameworks/thrift/command.py` & `baseplate-2.7.0b2/baseplate/frameworks/thrift/command.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/__init__.py` & `baseplate-2.7.0b2/baseplate/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/_requests.py` & `baseplate-2.7.0b2/baseplate/lib/_requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/config.py` & `baseplate-2.7.0b2/baseplate/lib/config.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/crypto.py` & `baseplate-2.7.0b2/baseplate/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/datetime.py` & `baseplate-2.7.0b2/baseplate/lib/datetime.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/events.py` & `baseplate-2.7.0b2/baseplate/lib/events.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/file_watcher.py` & `baseplate-2.7.0b2/baseplate/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/live_data/writer.py` & `baseplate-2.7.0b2/baseplate/lib/live_data/writer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/live_data/zookeeper.py` & `baseplate-2.7.0b2/baseplate/lib/live_data/zookeeper.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/log_formatter.py` & `baseplate-2.7.0b2/baseplate/lib/log_formatter.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/message_queue.py` & `baseplate-2.7.0b2/baseplate/lib/message_queue.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/metrics.py` & `baseplate-2.7.0b2/baseplate/lib/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/prometheus_metrics.py` & `baseplate-2.7.0b2/baseplate/lib/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/random.py` & `baseplate-2.7.0b2/baseplate/lib/random.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/__init__.py` & `baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/memcache.py` & `baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/memcache.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/redis.py` & `baseplate-2.7.0b2/baseplate/lib/ratelimit/backends/redis.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/ratelimit/ratelimit.py` & `baseplate-2.7.0b2/baseplate/lib/ratelimit/ratelimit.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/retry.py` & `baseplate-2.7.0b2/baseplate/lib/retry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/secrets.py` & `baseplate-2.7.0b2/baseplate/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/service_discovery.py` & `baseplate-2.7.0b2/baseplate/lib/service_discovery.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lib/thrift_pool.py` & `baseplate-2.7.0b2/baseplate/lib/thrift_pool.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lint/db_query_string_format_plugin.py` & `baseplate-2.7.0b2/baseplate/lint/db_query_string_format_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/lint/example_plugin.py` & `baseplate-2.7.0b2/baseplate/lint/example_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/logging.py` & `baseplate-2.7.0b2/baseplate/observers/logging.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/metrics.py` & `baseplate-2.7.0b2/baseplate/observers/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/metrics_tagged.py` & `baseplate-2.7.0b2/baseplate/observers/metrics_tagged.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/sentry.py` & `baseplate-2.7.0b2/baseplate/observers/sentry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/timeout.py` & `baseplate-2.7.0b2/baseplate/observers/timeout.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/observers/tracing.py` & `baseplate-2.7.0b2/baseplate/observers/tracing.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/__init__.py` & `baseplate-2.7.0b2/baseplate/server/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/einhorn.py` & `baseplate-2.7.0b2/baseplate/server/einhorn.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/healthcheck.py` & `baseplate-2.7.0b2/baseplate/server/healthcheck.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/monkey.py` & `baseplate-2.7.0b2/baseplate/server/monkey.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/net.py` & `baseplate-2.7.0b2/baseplate/server/net.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/prometheus.py` & `baseplate-2.7.0b2/baseplate/server/prometheus.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/queue_consumer.py` & `baseplate-2.7.0b2/baseplate/server/queue_consumer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/reloader.py` & `baseplate-2.7.0b2/baseplate/server/reloader.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/runtime_monitor.py` & `baseplate-2.7.0b2/baseplate/server/runtime_monitor.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/thrift.py` & `baseplate-2.7.0b2/baseplate/server/thrift.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/server/wsgi.py` & `baseplate-2.7.0b2/baseplate/server/wsgi.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/sidecars/__init__.py` & `baseplate-2.7.0b2/baseplate/sidecars/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/sidecars/event_publisher.py` & `baseplate-2.7.0b2/baseplate/sidecars/event_publisher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/sidecars/live_data_watcher.py` & `baseplate-2.7.0b2/baseplate/sidecars/live_data_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/sidecars/secrets_fetcher.py` & `baseplate-2.7.0b2/baseplate/sidecars/secrets_fetcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/sidecars/trace_publisher.py` & `baseplate-2.7.0b2/baseplate/sidecars/trace_publisher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/testing/lib/file_watcher.py` & `baseplate-2.7.0b2/baseplate/testing/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/testing/lib/secrets.py` & `baseplate-2.7.0b2/baseplate/testing/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/thrift/BaseplateService.py` & `baseplate-2.7.0b2/baseplate/thrift/BaseplateService.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/thrift/BaseplateServiceV2.py` & `baseplate-2.7.0b2/baseplate/thrift/BaseplateServiceV2.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/thrift/baseplate.thrift` & `baseplate-2.7.0b2/baseplate/thrift/baseplate.thrift`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/baseplate/thrift/ttypes.py` & `baseplate-2.7.0b2/baseplate/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0b1/bin/baseplate-tshell` & `baseplate-2.7.0b2/bin/baseplate-tshell`

 * *Files 17% similar despite different names*

```diff
@@ -8,13 +8,22 @@
 from gevent.monkey import patch_all
 
 from baseplate.server.monkey import patch_stdlib_queues
 
 patch_all()
 patch_stdlib_queues()
 
+try:
+    import psycopg2
+    from psycogreen.gevent import patch_psycopg
+
+    patch_psycopg()
+except ImportError:
+    pass
+
+
 from baseplate.server import load_and_run_shell
 
 print("baseplate-tshell has been renamed to baseplate-shell. Please use that in the future!")
 print()
 
 load_and_run_shell()
```

### Comparing `baseplate-2.7.0b1/pyproject.toml` & `baseplate-2.7.0b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseplate"
-version = "2.7.0b1"
+version = "2.7.0b2"
 description = "reddit's python service framework"
 authors = ["reddit"]
 license = "BSD"
 readme = "README.md"
 homepage = "https://github.com/reddit/baseplate.py"
 repository = "https://github.com/reddit/baseplate.py"
 documentation = "https://baseplate.readthedocs.io/en/stable/"
@@ -35,14 +35,16 @@
 redis = { version = ">=2.10.0,<4.0.0", optional = true }
 redis-py-cluster = { version = ">=2.1.2,<3.0.0", optional = true }
 requests = ">=2.21.0,<3.0"
 sentry-sdk = { version = ">=1.35.0,<2.0", optional = true }
 sqlalchemy = { version = ">=1.4.49,<2", optional = true }
 thrift-unofficial = ">=0.19.0,<1.0"
 typing-extensions = "^4.11.0"
+psycopg2 = "^2.0.0"
+psycogreen = "^1.0.0"
 
 [tool.poetry.extras]
 amqp = ["kombu"]
 cassandra = ["cassandra-driver"]
 cqlmapper = ["reddit-cqlmapper"]
 kafka = ["confluent-kafka"]
 memcache = ["pymemcache"]
@@ -51,14 +53,15 @@
 redis = ["redis"]
 redis-py-cluster = ["redis-py-cluster"]
 refcycle = ["objgraph"]
 requests = ["advocate"]
 s3fetcher = []  # Kept for backwards compatibility, these are now main requirements
 sentry = ["sentry-sdk"]
 sql = ["sqlalchemy"]
+psycopg2 = ["psycopg2", "psycogreen"]
 zookeeper = ["kazoo"]
 
 [tool.poetry.group.dev.dependencies]
 black = "21.10b0"
 # TODO: This can be removed once we upgrade to a newer Black version.
 # https://github.com/psf/black/issues/2964
 click = "<8.1.0"
```

### Comparing `baseplate-2.7.0b1/PKG-INFO` & `baseplate-2.7.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseplate
-Version: 2.7.0b1
+Version: 2.7.0b2
 Summary: reddit's python service framework
 Home-page: https://github.com/reddit/baseplate.py
 License: BSD
 Author: reddit
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Provides-Extra: amqp
 Provides-Extra: cassandra
 Provides-Extra: cqlmapper
 Provides-Extra: kafka
 Provides-Extra: memcache
 Provides-Extra: prometheus
+Provides-Extra: psycopg2
 Provides-Extra: pyramid
 Provides-Extra: redis
 Provides-Extra: redis-py-cluster
 Provides-Extra: refcycle
 Provides-Extra: requests
 Provides-Extra: s3fetcher
 Provides-Extra: sentry
@@ -38,14 +39,16 @@
 Requires-Dist: confluent-kafka (>=2.3.0) ; extra == "kafka"
 Requires-Dist: gevent (>=23.9.1)
 Requires-Dist: kazoo (>=2.5.0,<3.0) ; extra == "zookeeper"
 Requires-Dist: kombu (>=5.3.3) ; extra == "amqp"
 Requires-Dist: objgraph (>=3.6.0) ; extra == "refcycle"
 Requires-Dist: posix-ipc (>=1.0.0,<2.0)
 Requires-Dist: prometheus-client (>=0.12.0)
+Requires-Dist: psycogreen (>=1.0.0,<2.0.0) ; extra == "psycopg2"
+Requires-Dist: psycopg2 (>=2.0.0,<3.0.0) ; extra == "psycopg2"
 Requires-Dist: pymemcache (>=1.3.0,<1.4.4) ; extra == "memcache"
 Requires-Dist: pyramid (>=1.10.8,<2.0) ; extra == "pyramid"
 Requires-Dist: python-json-logger (>=2.0.5,<3.0)
 Requires-Dist: reddit-cqlmapper (>=0.3.0,<1.0) ; extra == "cqlmapper"
 Requires-Dist: redis (>=2.10.0,<4.0.0) ; extra == "redis"
 Requires-Dist: redis-py-cluster (>=2.1.2,<3.0.0) ; extra == "redis-py-cluster"
 Requires-Dist: requests (>=2.21.0,<3.0)
```

