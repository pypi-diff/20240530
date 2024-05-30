# Comparing `tmp/petisco-2.1.3.tar.gz` & `tmp/petisco-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-2.1.3.tar", last modified: Mon Mar 18 14:41:39 2024, max compression
+gzip compressed data, was "petisco-2.1.4.tar", last modified: Thu May 30 05:34:27 2024, max compression
```

## Comparing `petisco-2.1.3.tar` & `petisco-2.1.4.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.971255 petisco-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-18 14:41:35.000000 petisco-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 14:41:35.000000 petisco-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-18 14:41:39.971255 petisco-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-18 14:41:35.000000 petisco-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.935255 petisco-2.1.3/petisco/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.935255 petisco-2.1.3/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/chaos/chaos_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/chaos/check_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/async_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/controller/meta_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/dependency_injection/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/handlers/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.939256 petisco-2.1.3/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.943256 petisco-2.1.3/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/async_app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.943256 petisco-2.1.3/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/use_case/async_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/use_case/meta_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.943256 petisco-2.1.3/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.943256 petisco-2.1.3/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.943256 petisco-2.1.3/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.947255 petisco-2.1.3/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.947255 petisco-2.1.3/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/model/legacy_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/async_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/persistence/fake_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/base/domain/value_objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/value_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/domain/value_objects/middleware_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/datetime_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/time_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/cli/petisco_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.951255 petisco-2.1.3/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/async_elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/elastic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic/is_elastic_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/elastic_apm/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic_apm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic_apm/capture_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/elastic_apm/is_elastic_apm_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/application/add_controller_responses_to_response_mocker_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/application/ensure_all_routers_are_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/application/fastapi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/application/response_mocker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/as_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.955255 petisco-2.1.3/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/loguru_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/logger/not_implemented_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/meiga/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/meiga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.959255 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21825 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/rabbitmq_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/redis/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/redis/application/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/redis/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/redis/is_redis_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.963255 petisco-2.1.3/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/async_sql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/extra/threading/pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/public_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/petisco/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.935255 petisco-2.1.3/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-18 14:41:39.000000 petisco-2.1.3/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-18 14:41:35.000000 petisco-2.1.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-18 14:41:39.971255 petisco-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-18 14:41:35.000000 petisco-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-18 14:41:35.000000 petisco-2.1.3/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:39.967255 petisco-2.1.3/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:41:35.000000 petisco-2.1.3/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 05:34:24.000000 petisco-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 05:34:24.000000 petisco-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 05:34:27.383946 petisco-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 05:34:24.000000 petisco-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.355945 petisco-2.1.4/petisco/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/legacy_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/fake_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/domain/value_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/value_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/value_objects/middleware_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/datetime_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/time_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/is_elastic_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/capture_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/add_controller_responses_to_response_mocker_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/ensure_all_routers_are_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/fastapi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/response_mocker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/meiga/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/meiga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/rabbitmq_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 05:34:24.000000 petisco-2.1.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 05:34:27.387946 petisco-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-30 05:34:24.000000 petisco-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/modules/__init__.py
```

### Comparing `petisco-2.1.3/LICENSE` & `petisco-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/PKG-INFO` & `petisco-2.1.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,198 +1,144 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7065 7469  : 2.1.Name: peti
-00000020: 7363 6f0a 5665 7273 696f 6e3a 2032 2e31  sco.Version: 2.1
-00000030: 2e33 0a53 756d 6d61 7279 3a20 5065 7469  .3.Summary: Peti
-00000040: 7363 6f20 6973 2061 2066 7261 6d65 776f  sco is a framewo
-00000050: 726b 2066 6f72 2068 656c 7069 6e67 2050  rk for helping P
-00000060: 7974 686f 6e20 6465 7665 6c6f 7065 7273  ython developers
-00000070: 2074 6f20 6275 696c 6420 636c 6561 6e20   to build clean 
-00000080: 4170 706c 6963 6174 696f 6e73 0a48 6f6d  Applications.Hom
-00000090: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-000000a0: 6769 7468 7562 2e63 6f6d 2f61 6c69 6365  github.com/alice
-000000b0: 2d62 696f 6d65 7472 6963 732f 7065 7469  -biometrics/peti
-000000c0: 7363 6f0a 4175 7468 6f72 3a20 416c 6963  sco.Author: Alic
-000000d0: 6520 4269 6f6d 6574 7269 6373 0a41 7574  e Biometrics.Aut
-000000e0: 686f 722d 656d 6169 6c3a 2073 7570 706f  hor-email: suppo
-000000f0: 7274 4061 6c69 6365 6269 6f6d 6574 7269  rt@alicebiometri
-00000100: 6373 2e63 6f6d 0a4c 6963 656e 7365 3a20  cs.com.License: 
-00000110: 4d49 540a 4b65 7977 6f72 6473 3a20 4444  MIT.Keywords: DD
-00000120: 442c 5573 6520 4361 7365 2c43 6c65 616e  D,Use Case,Clean
-00000130: 2041 7263 6869 7465 6374 7572 652c 5245   Architecture,RE
-00000140: 5354 2c41 7070 6c69 6361 7469 6f6e 730a  ST,Applications.
-00000150: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000160: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000170: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000180: 7365 0a43 6c61 7373 6966 6965 723a 2050  se.Classifier: P
-00000190: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001a0: 6167 6520 3a3a 2050 7974 686f 6e0a 436c  age :: Python.Cl
-000001b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-000001e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000200: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
-00000210: 204f 6e6c 790a 436c 6173 7369 6669 6572   Only.Classifier
-00000220: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000230: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000240: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000250: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000270: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-00000280: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000290: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002a0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000002b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002d0: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
-000002e0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
-000002f0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-00000300: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
-00000310: 2d45 7874 7261 3a20 7371 6c61 6c63 6865  -Extra: sqlalche
-00000320: 6d79 0a50 726f 7669 6465 732d 4578 7472  my.Provides-Extr
-00000330: 613a 2072 6564 6973 0a50 726f 7669 6465  a: redis.Provide
-00000340: 732d 4578 7472 613a 2072 6162 6269 746d  s-Extra: rabbitm
-00000350: 710a 5072 6f76 6964 6573 2d45 7874 7261  q.Provides-Extra
-00000360: 3a20 736c 6163 6b0a 5072 6f76 6964 6573  : slack.Provides
-00000370: 2d45 7874 7261 3a20 656c 6173 7469 630a  -Extra: elastic.
-00000380: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000390: 656c 6173 7469 632d 6170 6d0a 5072 6f76  elastic-apm.Prov
-000003a0: 6964 6573 2d45 7874 7261 3a20 6661 7374  ides-Extra: fast
-000003b0: 6170 690a 5072 6f76 6964 6573 2d45 7874  api.Provides-Ext
-000003c0: 7261 3a20 7269 6368 0a50 726f 7669 6465  ra: rich.Provide
-000003d0: 732d 4578 7472 613a 2064 6576 0a4c 6963  s-Extra: dev.Lic
-000003e0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-000003f0: 5345 0a0a 2320 7065 7469 7363 6f20 f09f  SE..# petisco ..
-00000400: 8daa 2020 0a0a 5b21 5b76 6572 7369 6f6e  ..  ..[![version
-00000410: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000420: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000430: 7265 6c65 6173 652f 616c 6963 652d 6269  release/alice-bi
-00000440: 6f6d 6574 7269 6373 2f70 6574 6973 636f  ometrics/petisco
-00000450: 2f61 6c6c 2e73 7667 295d 2868 7474 7073  /all.svg)](https
-00000460: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00000470: 6963 652d 6269 6f6d 6574 7269 6373 2f70  ice-biometrics/p
-00000480: 6574 6973 636f 2f72 656c 6561 7365 7329  etisco/releases)
-00000490: 200a 5b21 5b63 695d 2868 7474 7073 3a2f   .[![ci](https:/
-000004a0: 2f67 6974 6875 622e 636f 6d2f 616c 6963  /github.com/alic
-000004b0: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
-000004c0: 6973 636f 2f77 6f72 6b66 6c6f 7773 2f63  isco/workflows/c
-000004d0: 692f 6261 6467 652e 7376 6729 5d28 6874  i/badge.svg)](ht
-000004e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004f0: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
-00000500: 732f 7065 7469 7363 6f2f 6163 7469 6f6e  s/petisco/action
-00000510: 7329 200a 5b21 5b70 7970 695d 2868 7474  s) .[![pypi](htt
-00000520: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000530: 2e69 6f2f 7079 7069 2f64 6d2f 7065 7469  .io/pypi/dm/peti
-00000540: 7363 6f29 5d28 6874 7470 733a 2f2f 7079  sco)](https://py
-00000550: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-00000560: 6574 6973 636f 2f29 200a 5b21 5b63 6f64  etisco/) .[![cod
-00000570: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
-00000580: 6465 636f 762e 696f 2f67 682f 616c 6963  decov.io/gh/alic
-00000590: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
-000005a0: 6973 636f 2f62 7261 6e63 682f 6d61 696e  isco/branch/main
-000005b0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-000005c0: 3f74 6f6b 656e 3d59 4858 4159 4b58 3056  ?token=YHXAYKX0V
-000005d0: 4f29 5d28 6874 7470 733a 2f2f 636f 6465  O)](https://code
-000005e0: 636f 762e 696f 2f67 682f 616c 6963 652d  cov.io/gh/alice-
-000005f0: 6269 6f6d 6574 7269 6373 2f70 6574 6973  biometrics/petis
-00000600: 636f 290a 5b21 5b43 6f64 6520 7374 796c  co).[![Code styl
-00000610: 653a 2062 6c61 636b 5d28 6874 7470 733a  e: black](https:
-00000620: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000630: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000640: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000650: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000660: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00000670: 6163 6b29 0a5b 215b 496d 706f 7274 733a  ack).[![Imports:
-00000680: 2069 736f 7274 5d28 6874 7470 733a 2f2f   isort](https://
-00000690: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000006a0: 6164 6765 2f25 3230 696d 706f 7274 732d  adge/%20imports-
-000006b0: 6973 6f72 742d 2532 3331 3637 3462 313f  isort-%231674b1?
-000006c0: 7374 796c 653d 666c 6174 266c 6162 656c  style=flat&label
-000006d0: 436f 6c6f 723d 6566 3833 3336 295d 2868  Color=ef8336)](h
-000006e0: 7474 7073 3a2f 2f70 7963 7161 2e67 6974  ttps://pycqa.git
-000006f0: 6875 622e 696f 2f69 736f 7274 2f29 0a5b  hub.io/isort/).[
-00000700: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
-00000710: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000720: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000730: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
-00000740: 732f 7065 7469 7363 6f2e 7376 6729 5d28  s/petisco.svg)](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f61 6c69 6365 2d62 696f 6d65 7472  om/alice-biometr
-00000770: 6963 732f 7065 7469 7363 6f2f 626c 6f62  ics/petisco/blob
-00000780: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a5b  /main/LICENSE).[
-00000790: 215b 7665 7273 696f 6e73 5d28 6874 7470  ![versions](http
-000007a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007b0: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000007c0: 6e73 2f70 6574 6973 636f 2e73 7667 295d  ns/petisco.svg)]
-000007d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007e0: 636f 6d2f 616c 6963 652d 6269 6f6d 6574  com/alice-biomet
-000007f0: 7269 6373 2f70 6574 6973 636f 290a 0a3c  rics/petisco)..<
-00000800: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000810: 2f67 6974 6875 622e 636f 6d2f 616c 6963  /github.com/alic
-00000820: 652d 6269 6f6d 6574 7269 6373 2f63 7573  e-biometrics/cus
-00000830: 746f 6d2d 656d 6f6a 6973 2f62 6c6f 622f  tom-emojis/blob/
-00000840: 6d61 7374 6572 2f69 6d61 6765 732f 616c  master/images/al
-00000850: 6963 655f 6865 6164 6572 2e70 6e67 3f72  ice_header.png?r
-00000860: 6177 3d74 7275 6522 2077 6964 7468 3d61  aw=true" width=a
-00000870: 7574 6f3e 0a0a 2d2d 2d0a 0a2a 2a44 6f63  uto>..---..**Doc
-00000880: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c61  umentation**: <a
-00000890: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
-000008a0: 6c69 6365 2d62 696f 6d65 7472 6963 732e  lice-biometrics.
-000008b0: 6769 7468 7562 2e69 6f2f 7065 7469 7363  github.io/petisc
-000008c0: 6f2f 2220 7461 7267 6574 3d22 5f62 6c61  o/" target="_bla
-000008d0: 6e6b 223e 6874 7470 733a 2f2f 616c 6963  nk">https://alic
-000008e0: 652d 6269 6f6d 6574 7269 6373 2e67 6974  e-biometrics.git
-000008f0: 6875 622e 696f 2f70 6574 6973 636f 2f3c  hub.io/petisco/<
-00000900: 2f61 3e0a 0a2a 2a53 6f75 7263 6520 436f  /a>..**Source Co
-00000910: 6465 2a2a 3a20 3c61 2068 7265 663d 2268  de**: <a href="h
-00000920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000930: 6d2f 616c 6963 652d 6269 6f6d 6574 7269  m/alice-biometri
-00000940: 6373 2f70 6574 6973 636f 2220 7461 7267  cs/petisco" targ
-00000950: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
-00000960: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000970: 6c69 6365 2d62 696f 6d65 7472 6963 732f  lice-biometrics/
-00000980: 7065 7469 7363 6f3c 2f61 3e0a 0a2d 2d2d  petisco</a>..---
-00000990: 0a0a 2323 2057 6861 7420 6973 2070 6574  ..## What is pet
-000009a0: 6973 636f 3f20 f09f 8daa 0a0a 7065 7469  isco? ......peti
-000009b0: 7363 6f20 6973 2061 2066 7261 6d65 776f  sco is a framewo
-000009c0: 726b 2066 6f72 2068 656c 7069 6e67 2050  rk for helping P
-000009d0: 7974 686f 6e20 6465 7665 6c6f 7065 7273  ython developers
-000009e0: 2074 6f20 6275 696c 6420 636c 6561 6e20   to build clean 
-000009f0: 4170 706c 6963 6174 696f 6e73 2069 6e20  Applications in 
-00000a00: 5079 7468 6f6e 2e0a 0a23 2320 486f 7720  Python...## How 
-00000a10: 636f 756c 6420 7065 7469 7363 6f20 6865  could petisco he
-00000a20: 6c70 206d 653f 20f0 9f8d aa0a 0a70 6574  lp me? ......pet
-00000a30: 6973 636f 2070 726f 7669 6465 7320 7365  isco provides se
-00000a40: 7665 7261 6c20 6861 6e64 7920 636c 6173  veral handy clas
-00000a50: 7365 7320 746f 2068 656c 7020 796f 7520  ses to help you 
-00000a60: 6f6e 2064 6566 696e 696e 6720 796f 7572  on defining your
-00000a70: 2064 6f6d 6169 6e20 7769 7468 2068 6578   domain with hex
-00000a80: 6167 6f6e 616c 2061 7263 6869 7465 6374  agonal architect
-00000a90: 7572 652c 2065 7665 6e74 2073 7472 6561  ure, event strea
-00000aa0: 6d69 6e67 2061 6e64 2043 5152 532e 0a0a  ming and CQRS...
-00000ab0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000ac0: 20f0 9f92 bb0a 0a60 6060 636f 6e73 6f6c   ......```consol
-00000ad0: 650a 7069 7020 696e 7374 616c 6c20 7065  e.pip install pe
-00000ae0: 7469 7363 6f0a 6060 600a 0a49 6e73 7461  tisco.```..Insta
-00000af0: 6c6c 6174 696f 6e20 7769 7468 2045 7874  llation with Ext
-00000b00: 7261 7320 0a0a 6060 6063 6f6e 736f 6c65  ras ..```console
-00000b10: 0a70 6970 2069 6e73 7461 6c6c 2070 6574  .pip install pet
-00000b20: 6973 636f 5b66 6173 7461 7069 2c73 716c  isco[fastapi,sql
-00000b30: 616c 6368 656d 792c 656c 6173 7469 632c  alchemy,elastic,
-00000b40: 656c 6173 7469 632d 6170 6d2c 7261 6262  elastic-apm,rabb
-00000b50: 6974 6d71 2c73 6c61 636b 2c72 6564 6973  itmq,slack,redis
-00000b60: 5d0a 6060 600a 0a23 2320 436f 6e74 7269  ].```..## Contri
-00000b70: 6275 7465 200a 0a57 6527 6420 6c6f 7665  bute ..We'd love
-00000b80: 2079 6f75 2074 6f20 636f 6e74 7269 6275   you to contribu
-00000b90: 7465 2074 6f20 2a70 6574 6973 636f 2a20  te to *petisco* 
-00000ba0: f09f a5b3 f09f a5b3 f09f a5b3 f09f a5b3  ................
-00000bb0: f09f a5b3 f09f a5b3 efb8 8fef b88f 210a  ..............!.
-00000bc0: 0a46 6f72 206d 6f72 6520 696e 666f 726d  .For more inform
-00000bd0: 6174 696f 6e2c 2063 6865 636b 206f 7572  ation, check our
-00000be0: 205b 646f 6375 6d65 6e74 6174 696f 6e5d   [documentation]
-00000bf0: 2868 7474 7073 3a2f 2f61 6c69 6365 2d62  (https://alice-b
-00000c00: 696f 6d65 7472 6963 732e 6769 7468 7562  iometrics.github
-00000c10: 2e69 6f2f 7065 7469 7363 6f2f 636f 6e74  .io/petisco/cont
-00000c20: 7269 6275 7469 6e67 2f29 0a0a 2323 2043  ributing/)..## C
-00000c30: 6f6e 7461 6374 20f0 9f93 ac0a 0a73 7570  ontact ......sup
-00000c40: 706f 7274 4061 6c69 6365 6269 6f6d 6574  port@alicebiomet
-00000c50: 7269 6373 2e63 6f6d 0a                   rics.com.
+00000000: 2320 7065 7469 7363 6f20 f09f 8daa 2020  # petisco ....  
+00000010: 0a0a 0a0a 3c64 6976 2061 6c69 676e 3d22  ....<div align="
+00000020: 6365 6e74 6572 223e 0a20 2020 203c 696d  center">.    <im
+00000030: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+00000040: 6974 6875 622e 636f 6d2f 616c 6963 652d  ithub.com/alice-
+00000050: 6269 6f6d 6574 7269 6373 2f63 7573 746f  biometrics/custo
+00000060: 6d2d 656d 6f6a 6973 2f62 6c6f 622f 6d61  m-emojis/blob/ma
+00000070: 7374 6572 2f69 6d61 6765 732f 7065 7469  ster/images/peti
+00000080: 7363 6f2e 706e 673f 7261 773d 7472 7565  sco.png?raw=true
+00000090: 2220 7374 796c 653d 2277 6964 7468 3a20  " style="width: 
+000000a0: 3630 2522 3e0a 0a0a 205b 416c 6963 655d  60%">... [Alice]
+000000b0: 207c 205b 4765 7474 696e 6720 5374 6172   | [Getting Star
+000000c0: 7465 645d 207c 205b 446f 6375 6d65 6e74  ted] | [Document
+000000d0: 6174 696f 6e5d 207c 205b 536f 7572 6365  ation] | [Source
+000000e0: 2043 6f64 655d 207c 205b 4578 616d 706c   Code] | [Exampl
+000000f0: 6573 5d0a 0a20 5b21 5b76 6572 7369 6f6e  es].. [![version
+00000100: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000110: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000120: 7265 6c65 6173 652f 616c 6963 652d 6269  release/alice-bi
+00000130: 6f6d 6574 7269 6373 2f70 6574 6973 636f  ometrics/petisco
+00000140: 2f61 6c6c 2e73 7667 295d 2868 7474 7073  /all.svg)](https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+00000160: 6963 652d 6269 6f6d 6574 7269 6373 2f70  ice-biometrics/p
+00000170: 6574 6973 636f 2f72 656c 6561 7365 7329  etisco/releases)
+00000180: 200a 5b21 5b63 695d 2868 7474 7073 3a2f   .[![ci](https:/
+00000190: 2f67 6974 6875 622e 636f 6d2f 616c 6963  /github.com/alic
+000001a0: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
+000001b0: 6973 636f 2f77 6f72 6b66 6c6f 7773 2f63  isco/workflows/c
+000001c0: 692f 6261 6467 652e 7376 6729 5d28 6874  i/badge.svg)](ht
+000001d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001e0: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
+000001f0: 732f 7065 7469 7363 6f2f 6163 7469 6f6e  s/petisco/action
+00000200: 7329 200a 5b21 5b70 7970 695d 2868 7474  s) .[![pypi](htt
+00000210: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000220: 2e69 6f2f 7079 7069 2f64 6d2f 7065 7469  .io/pypi/dm/peti
+00000230: 7363 6f29 5d28 6874 7470 733a 2f2f 7079  sco)](https://py
+00000240: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
+00000250: 6574 6973 636f 2f29 200a 5b21 5b63 6f64  etisco/) .[![cod
+00000260: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
+00000270: 6465 636f 762e 696f 2f67 682f 616c 6963  decov.io/gh/alic
+00000280: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
+00000290: 6973 636f 2f62 7261 6e63 682f 6d61 696e  isco/branch/main
+000002a0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+000002b0: 3f74 6f6b 656e 3d59 4858 4159 4b58 3056  ?token=YHXAYKX0V
+000002c0: 4f29 5d28 6874 7470 733a 2f2f 636f 6465  O)](https://code
+000002d0: 636f 762e 696f 2f67 682f 616c 6963 652d  cov.io/gh/alice-
+000002e0: 6269 6f6d 6574 7269 6373 2f70 6574 6973  biometrics/petis
+000002f0: 636f 290a 5b21 5b6c 6963 656e 7365 5d28  co).[![license](
+00000300: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000310: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
+00000320: 6365 6e73 652f 616c 6963 652d 6269 6f6d  cense/alice-biom
+00000330: 6574 7269 6373 2f70 6574 6973 636f 2e73  etrics/petisco.s
+00000340: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000350: 6875 622e 636f 6d2f 616c 6963 652d 6269  hub.com/alice-bi
+00000360: 6f6d 6574 7269 6373 2f70 6574 6973 636f  ometrics/petisco
+00000370: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
+00000380: 5345 290a 5b21 5b76 6572 7369 6f6e 735d  SE).[![versions]
+00000390: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000003a0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000003b0: 6572 7369 6f6e 732f 7065 7469 7363 6f2e  ersions/petisco.
+000003c0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+000003d0: 7468 7562 2e63 6f6d 2f61 6c69 6365 2d62  thub.com/alice-b
+000003e0: 696f 6d65 7472 6963 732f 7065 7469 7363  iometrics/petisc
+000003f0: 6f29 0a5b 215b 5275 6666 5d28 6874 7470  o).[![Ruff](http
+00000400: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000410: 696f 2f65 6e64 706f 696e 743f 7572 6c3d  io/endpoint?url=
+00000420: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00000430: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000440: 6d2f 6173 7472 616c 2d73 682f 7275 6666  m/astral-sh/ruff
+00000450: 2f6d 6169 6e2f 6173 7365 7473 2f62 6164  /main/assets/bad
+00000460: 6765 2f76 322e 6a73 6f6e 295d 2868 7474  ge/v2.json)](htt
+00000470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000480: 6173 7472 616c 2d73 682f 7275 6666 290a  astral-sh/ruff).
+00000490: 5b21 5b50 7964 616e 7469 6320 7632 5d28  [![Pydantic v2](
+000004a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004b0: 6c64 732e 696f 2f65 6e64 706f 696e 743f  lds.io/endpoint?
+000004c0: 7572 6c3d 6874 7470 733a 2f2f 7261 772e  url=https://raw.
+000004d0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000004e0: 742e 636f 6d2f 7079 6461 6e74 6963 2f70  t.com/pydantic/p
+000004f0: 7964 616e 7469 632f 6d61 696e 2f64 6f63  ydantic/main/doc
+00000500: 732f 6261 6467 652f 7632 2e6a 736f 6e29  s/badge/v2.json)
+00000510: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+00000520: 7964 616e 7469 632e 6465 762f 6c61 7465  ydantic.dev/late
+00000530: 7374 2f63 6f6e 7472 6962 7574 696e 672f  st/contributing/
+00000540: 2362 6164 6765 7329 0a0a 3c2f 6469 763e  #badges)..</div>
+00000550: 0a0a 5b41 6c69 6365 5d3a 2068 7474 7073  ..[Alice]: https
+00000560: 3a2f 2f61 6c69 6365 6269 6f6d 6574 7269  ://alicebiometri
+00000570: 6373 2e63 6f6d 2f0a 5b47 6574 7469 6e67  cs.com/.[Getting
+00000580: 2053 7461 7274 6564 5d3a 2068 7474 7073   Started]: https
+00000590: 3a2f 2f61 6c69 6365 2d62 696f 6d65 7472  ://alice-biometr
+000005a0: 6963 732e 6769 7468 7562 2e69 6f2f 7065  ics.github.io/pe
+000005b0: 7469 7363 6f2f 6765 7474 696e 675f 7374  tisco/getting_st
+000005c0: 6172 7465 642f 0a5b 446f 6375 6d65 6e74  arted/.[Document
+000005d0: 6174 696f 6e5d 3a20 6874 7470 733a 2f2f  ation]: https://
+000005e0: 616c 6963 652d 6269 6f6d 6574 7269 6373  alice-biometrics
+000005f0: 2e67 6974 6875 622e 696f 2f70 6574 6973  .github.io/petis
+00000600: 636f 2f0a 5b53 6f75 7263 6520 436f 6465  co/.[Source Code
+00000610: 5d3a 202e 2f70 6574 6973 636f 0a5b 4578  ]: ./petisco.[Ex
+00000620: 616d 706c 6573 5d3a 202e 2f65 7861 6d70  amples]: ./examp
+00000630: 6c65 730a 0a2d 2d2d 0a0a 2323 2057 6861  les..---..## Wha
+00000640: 7420 6973 2070 6574 6973 636f 3f20 f09f  t is petisco? ..
+00000650: 8daa 0a0a 7065 7469 7363 6f20 6973 2061  ....petisco is a
+00000660: 2066 7261 6d65 776f 726b 2066 6f72 2068   framework for h
+00000670: 656c 7069 6e67 2050 7974 686f 6e20 6465  elping Python de
+00000680: 7665 6c6f 7065 7273 2074 6f20 6275 696c  velopers to buil
+00000690: 6420 636c 6561 6e20 4170 706c 6963 6174  d clean Applicat
+000006a0: 696f 6e73 2069 6e20 5079 7468 6f6e 2e0a  ions in Python..
+000006b0: 0a23 2320 486f 7720 636f 756c 6420 7065  .## How could pe
+000006c0: 7469 7363 6f20 6865 6c70 206d 653f 20f0  tisco help me? .
+000006d0: 9f8d aa0a 0a70 6574 6973 636f 2070 726f  .....petisco pro
+000006e0: 7669 6465 7320 7365 7665 7261 6c20 6861  vides several ha
+000006f0: 6e64 7920 636c 6173 7365 7320 746f 2068  ndy classes to h
+00000700: 656c 7020 796f 7520 6f6e 2064 6566 696e  elp you on defin
+00000710: 696e 6720 796f 7572 2064 6f6d 6169 6e20  ing your domain 
+00000720: 7769 7468 2068 6578 6167 6f6e 616c 2061  with hexagonal a
+00000730: 7263 6869 7465 6374 7572 652c 2065 7665  rchitecture, eve
+00000740: 6e74 2073 7472 6561 6d69 6e67 2061 6e64  nt streaming and
+00000750: 2043 5152 532e 0a0a 2323 2049 6e73 7461   CQRS...## Insta
+00000760: 6c6c 6174 696f 6e20 f09f 92bb 0a0a 6060  llation ......``
+00000770: 6063 6f6e 736f 6c65 0a70 6970 2069 6e73  `console.pip ins
+00000780: 7461 6c6c 2070 6574 6973 636f 0a60 6060  tall petisco.```
+00000790: 0a0a 496e 7374 616c 6c61 7469 6f6e 2077  ..Installation w
+000007a0: 6974 6820 4578 7472 6173 0a0a 6060 6063  ith Extras..```c
+000007b0: 6f6e 736f 6c65 0a70 6970 2069 6e73 7461  onsole.pip insta
+000007c0: 6c6c 2070 6574 6973 636f 5b66 6173 7461  ll petisco[fasta
+000007d0: 7069 2c73 716c 616c 6368 656d 792c 656c  pi,sqlalchemy,el
+000007e0: 6173 7469 632c 656c 6173 7469 632d 6170  astic,elastic-ap
+000007f0: 6d2c 7261 6262 6974 6d71 2c73 6c61 636b  m,rabbitmq,slack
+00000800: 2c72 6564 6973 5d0a 6060 600a 0a23 2320  ,redis].```..## 
+00000810: 436f 6e74 7269 6275 7465 0a0a 5765 2764  Contribute..We'd
+00000820: 206c 6f76 6520 796f 7520 746f 2063 6f6e   love you to con
+00000830: 7472 6962 7574 6520 746f 202a 7065 7469  tribute to *peti
+00000840: 7363 6f2a 20f0 9fa5 b3f0 9fa5 b3f0 9fa5  sco* ...........
+00000850: b3f0 9fa5 b3f0 9fa5 b3f0 9fa5 b3ef b88f  ................
+00000860: efb8 8f21 0a0a 466f 7220 6d6f 7265 2069  ...!..For more i
+00000870: 6e66 6f72 6d61 7469 6f6e 2c20 6368 6563  nformation, chec
+00000880: 6b20 6f75 7220 5b64 6f63 756d 656e 7461  k our [documenta
+00000890: 7469 6f6e 5d28 6874 7470 733a 2f2f 616c  tion](https://al
+000008a0: 6963 652d 6269 6f6d 6574 7269 6373 2e67  ice-biometrics.g
+000008b0: 6974 6875 622e 696f 2f70 6574 6973 636f  ithub.io/petisco
+000008c0: 2f63 6f6e 7472 6962 7574 696e 672f 290a  /contributing/).
+000008d0: 0a23 2320 436f 6e74 6163 7420 f09f 93ac  .## Contact ....
+000008e0: 0a0a 3c73 7570 706f 7274 4061 6c69 6365  ..<support@alice
+000008f0: 6269 6f6d 6574 7269 6373 2e63 6f6d 3e0a  biometrics.com>.
```

### Comparing `petisco-2.1.3/petisco/base/application/application.py` & `petisco-2.1.4/petisco/base/application/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,86 +23,67 @@
     name: str
     version: str
     organization: str
     deployed_at: datetime
     environment: str = Field(default="local", validation_alias="ENVIRONMENT")
     dependencies_provider: Callable[..., List[Dependency]] = lambda: []
     configurers: List[ApplicationConfigurer] = []
-    shared_error_map: Union[ErrorMap, None] = Field(default=dict())
-    shared_middlewares: Union[List[Type[Middleware]], None] = Field(default=list())
+    shared_error_map: Union[ErrorMap, None] = Field(default={})
+    shared_middlewares: Union[List[Type[Middleware]], None] = Field(default=[])
 
     def __init__(self, **data: Any) -> None:
         info = ApplicationInfo(
             name=data["name"],
             organization=data["organization"],
             version=data["version"],
             deployed_at=data.get("deployed_at"),
             force_recreation=True,
-            shared_error_map=data.get("shared_error_map", dict()),
-            shared_middlewares=data.get("shared_middlewares", list()),
+            shared_error_map=data.get("shared_error_map", {}),
+            shared_middlewares=data.get("shared_middlewares", []),
         )
         deployed_at = info.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
         logger.info(
             f"Application: {info.name} {info.version} ({info.organization}) deployed at {deployed_at}"
         )
         super().__init__(**data)
 
-    def configure(
-        self, testing: bool = False, overwrite_dependencies: bool = False
-    ) -> None:
+    def configure(self, testing: bool = False, overwrite_dependencies: bool = False) -> None:
         before_dependencies_configurers = [
-            configurer
-            for configurer in self.configurers
-            if configurer.execute_after_dependencies is False
+            configurer for configurer in self.configurers if configurer.execute_after_dependencies is False
         ]
-        name_configurers = [
-            configurer.__class__.__name__
-            for configurer in before_dependencies_configurers
-        ]
-        logger.info(
-            f"Application: running configurators before setting dependencies {name_configurers}..."
-        )
+        name_configurers = [configurer.__class__.__name__ for configurer in before_dependencies_configurers]
+        logger.info(f"Application: running configurators before setting dependencies {name_configurers}...")
         for configurer in before_dependencies_configurers:
             configurer.execute(testing)
 
         logger.info("Application: setting dependencies...")
         Container.set_dependencies(self.get_dependencies(), overwrite_dependencies)
 
         after_dependencies_configurers = [
-            configurer
-            for configurer in self.configurers
-            if configurer.execute_after_dependencies is True
+            configurer for configurer in self.configurers if configurer.execute_after_dependencies is True
         ]
 
-        name_configurers = [
-            configurer.__class__.__name__
-            for configurer in after_dependencies_configurers
-        ]
-        logger.info(
-            f"Application: running configurators after setting dependencies {name_configurers}..."
-        )
+        name_configurers = [configurer.__class__.__name__ for configurer in after_dependencies_configurers]
+        logger.info(f"Application: running configurators after setting dependencies {name_configurers}...")
         for configurer in after_dependencies_configurers:
             configurer.execute(testing)
 
         logger.info("Application: successful configuration")
 
     def get_dependencies(self) -> List[Dependency]:
         # TODO: review default dependencies in v2
 
-        default_dependencies = (
-            get_default_message_dependencies() + get_default_notifier_dependencies()
-        )
-        default_dependencies_dict = {
-            dependency.get_key(): dependency for dependency in default_dependencies
-        }
+        default_dependencies = get_default_message_dependencies() + get_default_notifier_dependencies()
+        default_dependencies_dict = {dependency.get_key(): dependency for dependency in default_dependencies}
         provided_dependencies = self.dependencies_provider()
         provided_dependencies_dict = {
             dependency.get_key(): dependency for dependency in provided_dependencies
         }
-        # This merged_dependencies will give preference to provided_dependencies_dict over default_dependencies_dict
+        # This merged_dependencies will give preference to provided_dependencies_dict
+        # over default_dependencies_dict
         merged_dependencies = {
             **default_dependencies_dict,
             **provided_dependencies_dict,
         }
         return list(merged_dependencies.values())
 
     def clear(self) -> None:
@@ -118,28 +99,28 @@
         del info["dependencies_provider"]
         del info["configurers"]
         del info["shared_error_map"]
         del info["shared_middlewares"]
         return info
 
     def was_deploy_few_minutes_ago(self, minutes: int = 25) -> bool:
-        return datetime.now(timezone.utc) < self.deployed_at + timedelta(
-            minutes=minutes
-        )
+        return datetime.now(timezone.utc) < self.deployed_at + timedelta(minutes=minutes)
 
     def publish_domain_event(self, domain_event: DomainEvent) -> None:
         try:
             domain_event_bus = Container.get(DomainEventBus)
             domain_event_bus.publish(domain_event)
         except Exception as exc:  # noqa
             raise TypeError(
-                f"To publish an event to the domain event bus, please add a dependency with type `DomainEventBus` on Application dependencies. {str(exc)}"
-            )
+                "To publish an event to the domain event bus, please add a dependency"
+                f" with type `DomainEventBus` on Application dependencies. {str(exc)}"
+            ) from exc
 
     def notify(self, message: NotifierMessage) -> None:
         try:
             notifier = Container.get(Notifier)
             notifier.publish(message)
-        except:  # noqa
+        except Exception as exc:  # noqa
             raise TypeError(
-                'To notify the deploy, please add a dependency with name "notifier" on Application dependencies'
-            )
+                "To notify the deploy, please add a dependency "
+                'with name "notifier" on Application dependencies'
+            ) from exc
```

### Comparing `petisco-2.1.3/petisco/base/application/application_info.py` & `petisco-2.1.4/petisco/base/application/application_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     shared_middlewares: List[Middleware]
 
     def __init__(self, **kwargs: Any) -> None:
         self.name = str(kwargs.get("name"))
         self.organization = str(kwargs.get("organization"))
         self.version = str(kwargs.get("version"))
         self.deployed_at = cast(datetime, kwargs.get("deployed_at"))
-        self.shared_error_map = cast(dict, kwargs.get("shared_error_map", dict()))
-        self.shared_middlewares = cast(list, kwargs.get("shared_middlewares", list()))
+        self.shared_error_map = cast(dict, kwargs.get("shared_error_map", {}))
+        self.shared_middlewares = cast(list, kwargs.get("shared_middlewares", []))
```

### Comparing `petisco-2.1.3/petisco/base/application/chaos/chaos_config.py` & `petisco-2.1.4/petisco/base/application/chaos/chaos_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from pydantic_settings import BaseSettings
 
 
 class ChaosConfig(BaseSettings):
     percentage_invalid_message_publication: confloat(ge=0.0, le=1.0) = Field(
         default=0,
         validation_alias="PETISCO_CHAOS_PERCENTAGE_INVALID_MESSAGE_PUBLICATION",
-        description="Percentage of invalid message publication. Where 1.0 means rejecting all the publishing messages.",
+        description=(
+            "Percentage of invalid message publication."
+            " Where 1.0 means rejecting all the publishing messages.",
+        ),
     )
     percentage_simulate_nack: confloat(ge=0.0, le=1.0) = Field(
         default=0,
         validation_alias="PETISCO_CHAOS_PERCENTAGE_SIMULATE_NACK",
         description="Percentage of simulate nack. Where 1.0 rejects all the consuming messages",
     )
     delay_after_message_consume_seconds: confloat(ge=0.0, le=60.0) = Field(
```

### Comparing `petisco-2.1.3/petisco/base/application/controller/async_controller.py` & `petisco-2.1.4/petisco/base/application/controller/async_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from petisco.base.application.controller.meta_controller import MetaController
 from petisco.base.misc.result_mapper import ResultMapper, default_failure_handler
 
 
 class AsyncController(metaclass=MetaController):
     """
     A base class for creating async controllers.
-    Inherit from this class to convert to domain the request values, configure middlewares and instantiate and execute
-     a UseCase.
+    Inherit from this class to convert to domain the request values,
+    configure middlewares and instantiate and execute a UseCase.
     """
 
     @staticmethod
     def get_default_mapper() -> ResultMapper:
         return ResultMapper()
 
     @staticmethod
@@ -26,11 +26,9 @@
         return ResultMapper(
             error_map=cast(ErrorMap, getattr(config, "error_map", None)),
             success_handler=getattr(config, "success_handler", lambda result: result),
             failure_handler=getattr(config, "failure_handler", default_failure_handler),
         )
 
     @abstractmethod
-    async def execute(
-        self, *args: tuple[str, ...], **kwargs: dict[str, Any]
-    ) -> AnyResult:
+    async def execute(self, *args: tuple[str, ...], **kwargs: dict[str, Any]) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-2.1.3/petisco/base/application/controller/controller.py` & `petisco-2.1.4/petisco/base/application/controller/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,27 +20,27 @@
     }
     return shared_and_default_error_map
 
 
 class Controller(metaclass=MetaController):
     """
     A base class for creating controllers.
-    Inherit from this class to convert to domain the request values, configure middlewares and instantiate and execute
-     a UseCase.
+    Inherit from this class to convert to domain the request values,
+    configure middlewares and instantiate and execute a UseCase.
     """
 
     @staticmethod
     def get_default_mapper() -> ResultMapper:
         error_map = get_shared_and_default_error_map()
         return ResultMapper(error_map=error_map)
 
     @staticmethod
     def get_config_mapper(config: dict[str, Any]) -> ResultMapper:
         shared_and_default_error_map = get_shared_and_default_error_map()
-        controller_error_map = cast(ErrorMap, getattr(config, "error_map", dict()))
+        controller_error_map = cast(ErrorMap, getattr(config, "error_map", {}))
 
         # This merged_dependencies will give preference to controller_error_map (given in the controller) over
         # shared_and_default_error_map
         error_map = {
             **shared_and_default_error_map,
             **controller_error_map,
         }
```

### Comparing `petisco-2.1.3/petisco/base/application/controller/http_error.py` & `petisco-2.1.4/petisco/base/application/controller/http_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/application/controller/meta_controller.py` & `petisco-2.1.4/petisco/base/application/controller/meta_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,21 @@
     return mapper
 
 
 class MetaController(type, ABC):
     middlewares: list[Middleware] = []
     use_global_middlewares: bool = True
 
-    def __new__(
-        mcs, name: str, bases: tuple[Any], namespace: dict[str, Any]
-    ) -> MetaController:
+    def __new__(mcs, name: str, bases: tuple[Any], namespace: dict[str, Any]) -> MetaController:
         config = namespace.get("Config")
 
         mapper = get_mapper(bases, config)
 
         if "execute" not in namespace:
-            raise NotImplementedError(
-                "Petisco Controller must implement an execute method"
-            )
+            raise NotImplementedError("Petisco Controller must implement an execute method")
 
         new_namespace = {}
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
                 if iscoroutinefunction(attribute):
                     attribute = async_wrapper(attribute, name, config, mapper)
                 else:
```

### Comparing `petisco-2.1.3/petisco/base/application/dependency_injection/container.py` & `petisco-2.1.4/petisco/base/application/dependency_injection/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,40 @@
 from petisco.base.misc.singleton import Singleton
 
 T = TypeVar("T", bound=ABC)
 
 
 class Container(metaclass=Singleton):
     """
-    Singleton which contains set dependencies (List[Dependency)) prepared to be instantiated in order to be injected
-     in the UseCases of our application
+    Singleton which contains set dependencies (List[Dependency)) prepared to
+    be instantiated in order to be injected in the UseCases of our application
     """
 
     def __init__(self) -> None:
         self.dependencies: dict[str, Dependency[Any]] = defaultdict()
 
     @staticmethod
     def get(base_type: type[T], *, alias: str | None = None) -> T:
         """
         Returns an instance of set Dependency.
         """
 
         container = Container()
 
-        key = (
-            base_type.__name__
-            if not alias
-            else f'{base_type.__name__} (alias="{alias}")'
-        )
+        key = base_type.__name__ if not alias else f'{base_type.__name__} (alias="{alias}")'
         dependency = container.dependencies.get(key)
         if dependency is None:
             raise IndexError(
                 f"Invalid dependency. `{key}` is not found within available dependencies [{container.get_available_dependencies()}]"
             )
         instance = dependency.get_instance()
         return instance
 
     @staticmethod
-    def set_dependencies(
-        dependencies: list[Dependency[Any]] | None = None, overwrite: bool = False
-    ) -> None:
+    def set_dependencies(dependencies: list[Dependency[Any]] | None = None, overwrite: bool = False) -> None:
         """
         Set dependencies from a list of them.
         """
         if dependencies is None:
             dependencies = []
         Container()._set_dependencies(dependencies, overwrite)
 
@@ -55,17 +49,15 @@
     def get_available_dependencies() -> list[str]:
         """
         Returns the names (keys) of set dependencies.
         """
         keys = list(Container().dependencies.keys())
         return keys
 
-    def _set_dependencies(
-        self, input_dependencies: list[Dependency[Any]], overwrite: bool = False
-    ) -> None:
+    def _set_dependencies(self, input_dependencies: list[Dependency[Any]], overwrite: bool = False) -> None:
         for dependency in input_dependencies:
             key = dependency.get_key()
 
             if key in self.dependencies and not overwrite:
                 if dependency.alias:
                     raise IndexError(
                         f"Container: dependency ({dependency.type.__name__} with alias={dependency.alias}) is already added to dependencies. Check "
```

### Comparing `petisco-2.1.3/petisco/base/application/dependency_injection/dependency.py` & `petisco-2.1.4/petisco/base/application/dependency_injection/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,19 @@
             )
 
     def _set_envar_modifier(self, envar_modifier: str | None = None):
         self.envar_modifier = None
         if envar_modifier is None and self.type:
             self.envar_modifier = (
                 # "PETISCO_" + # TODO this will break compatibility (waiting for new versions)
-                re.sub(r"(?<!^)(?=[A-Z])", "_", self.type.__name__).upper()
-                + "_TYPE"
+                re.sub(r"(?<!^)(?=[A-Z])", "_", self.type.__name__).upper() + "_TYPE"
             )
             if self.alias:
-                alias_str = (
-                    re.sub(r"(?<!^)(?=[A-Z])", "_", self.alias)
-                    .replace("-", "_")
-                    .upper()
-                )
-                self.envar_modifier = self.envar_modifier.replace(
-                    "_TYPE", f"_ALIAS_{alias_str}_TYPE"
-                )
+                alias_str = re.sub(r"(?<!^)(?=[A-Z])", "_", self.alias).replace("-", "_").upper()
+                self.envar_modifier = self.envar_modifier.replace("_TYPE", f"_ALIAS_{alias_str}_TYPE")
         else:
             self.envar_modifier = envar_modifier
 
     def _validate(self) -> None:
         if self.type and self.strict:
             if self.builders is None:
                 return
@@ -98,17 +91,15 @@
             builder = self._get_default_builder()
             instance = builder.build()
             return instance
         else:
             builder = self.builders.get(modifier)
             if not builder:
                 builder = self._get_default_builder()
-            assert isinstance(
-                builder, Builder
-            ), "Oh no! Dependency builder is corrupted!"
+            assert isinstance(builder, Builder), "Oh no! Dependency builder is corrupted!"
             instance = builder.build()
             return instance
 
     def _get_default_builder(self) -> Builder:
         builder = self.builders.get("default")
         if not builder:
             raise TypeError(
```

### Comparing `petisco-2.1.3/petisco/base/application/handlers/message_handler.py` & `petisco-2.1.4/petisco/base/application/handlers/message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,18 @@
         except Exception as exception:
             return Failure(UseCaseUncontrolledError(exception))
 
     return wrapped
 
 
 class MetaUseCase(type, ABC):
-    def __new__(
-        mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]
-    ) -> "MetaUseCase":
+    def __new__(mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]) -> "MetaUseCase":
         new_class_dict = {}
         if "execute" not in namespace:
-            raise NotImplementedError(
-                "Petisco UseCase must implement an execute method"
-            )
+            raise NotImplementedError("Petisco UseCase must implement an execute method")
 
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
                 attribute = wrapper(attribute)
             new_class_dict[attributeName] = attribute
         return type.__new__(mcs, name, bases, new_class_dict)
```

### Comparing `petisco-2.1.3/petisco/base/application/middleware/middleware.py` & `petisco-2.1.4/petisco/base/application/middleware/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,12 +40,10 @@
         meta = {}
 
         try:
             info_id = self.wrapped_class_input_arguments.get("info_id")
             if info_id and hasattr(info_id, "to_meta"):
                 meta = info_id.to_meta().get("info_id", {})
         except Exception as exc:
-            logger.error(
-                f"Middleware error getting info_id on get_meta_from_input: {str(exc)}"
-            )
+            logger.error(f"Middleware error getting info_id on get_meta_from_input: {str(exc)}")
 
         return meta
```

### Comparing `petisco-2.1.3/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.1.4/petisco/base/application/middleware/notifier_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,16 @@
                 "application_version": ApplicationInfo().version,
             }
             input_meta = self.get_meta_from_input()
 
             meta = {**app_meta, **input_meta}
 
             if issubclass(error.__class__, UnknownError):
-                notifier_exception_message = (
-                    NotifierExceptionMessage.from_unknown_error(
-                        error, title="Uncontrolled Exception"
-                    )
+                notifier_exception_message = NotifierExceptionMessage.from_unknown_error(
+                    error, title="Uncontrolled Exception"
                 )
                 notifier_exception_message.update_meta(meta)
                 self.notifier.publish_exception(notifier_exception_message)
             if issubclass(error.__class__, CriticalError):
                 notifier_message = NotifierMessage(
                     title=error.get_specific_detail(),
                     message=error.__repr__(),
```

### Comparing `petisco-2.1.3/petisco/base/application/notifier/notifier.py` & `petisco-2.1.4/petisco/base/application/notifier/notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,9 @@
 
 class Notifier(Interface):
     @abstractmethod
     def publish(self, notifier_message: NotifierMessage) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def publish_exception(
-        self, notifier_exception_message: NotifierExceptionMessage
-    ) -> None:
+    def publish_exception(self, notifier_exception_message: NotifierExceptionMessage) -> None:
         raise NotImplementedError
```

### Comparing `petisco-2.1.3/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-2.1.4/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,15 @@
         self.input_parameters = input_parameters
         self.meta = meta
 
     def update_meta(self, meta: Dict[str, Any]) -> None:
         self.meta = {**self.meta, **meta}  # type: ignore
 
     @staticmethod
-    def from_unknown_error(
-        unknown_error: UnknownError, title: str
-    ) -> "NotifierExceptionMessage":
+    def from_unknown_error(unknown_error: UnknownError, title: str) -> "NotifierExceptionMessage":
         return NotifierExceptionMessage(
             title=title,
             executor=unknown_error.executor,
             exception=unknown_error.exception,
             traceback=unknown_error.traceback,
             filename=unknown_error.filename,
             lineno=unknown_error.lineno,
```

### Comparing `petisco-2.1.3/petisco/base/application/patterns/crud_repository.py` & `petisco-2.1.4/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.1.4/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 from petisco.base.domain.errors.defaults.not_found import AggregateNotFoundError
 from petisco.base.domain.model.uuid import Uuid
 
 
 class InmemoryCrudRepository(CrudRepository[AggregateRootType]):
     def __init__(self) -> None:
-        self._data: Dict[Uuid, Any] = dict()
+        self._data: Dict[Uuid, Any] = {}
 
     @meiga
     def save(self, aggregate_root: AggregateRootType) -> BoolResult:
         if aggregate_root.aggregate_id in self._data:
             return Failure(AggregateAlreadyExistError(aggregate_root.aggregate_id))
         self._data[aggregate_root.aggregate_id] = aggregate_root
         return isSuccess
```

### Comparing `petisco-2.1.3/petisco/base/application/use_case/meta_use_case.py` & `petisco-2.1.4/petisco/base/application/use_case/meta_use_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from petisco.base.application.use_case.use_case_uncontrolled_error import (
     UseCaseUncontrolledError,
 )
 from petisco.extra.elastic_apm.capture_exception import capture_exception
 from petisco.extra.meiga import WaitingForEarlyReturn
 
 
-def use_case_wrapper(
-    method: Callable[..., AnyResult], wrapped_class_name: str
-) -> Callable[..., AnyResult]:
+def use_case_wrapper(method: Callable[..., AnyResult], wrapped_class_name: str) -> Callable[..., AnyResult]:
     @wraps(method)
     def wrapped(*args: Any, **kwargs: Any) -> AnyResult:
         try:
             return method(*args, **kwargs)
         except WaitingForEarlyReturn as exception:
             return exception.result
         except Error as error:
@@ -57,22 +55,18 @@
             capture_exception()
             return Failure(uncontrolled_error)
 
     return wrapped
 
 
 class MetaUseCase(type, ABC):
-    def __new__(
-        mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]
-    ) -> "MetaUseCase":
+    def __new__(mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]) -> "MetaUseCase":
         new_class_dict = {}
         if "execute" not in namespace:
-            raise NotImplementedError(
-                "Petisco UseCase or AsyncUseCase must implement an execute method"
-            )
+            raise NotImplementedError("Petisco UseCase or AsyncUseCase must implement an execute method")
 
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
                 if iscoroutinefunction(attribute):
                     attribute = async_use_case_wrapper(attribute, name)
                 else:
                     attribute = use_case_wrapper(attribute, name)
```

### Comparing `petisco-2.1.3/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.1.4/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.1.4/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from typing import Optional
 
 from petisco.base.domain.errors.domain_error import DomainError
 from petisco.base.domain.model.uuid import Uuid
 
 
-class AlreadyExists(DomainError):
-    ...
+class AlreadyExists(DomainError): ...
 
 
-class ClientAlreadyExists(DomainError):
-    ...
+class ClientAlreadyExists(DomainError): ...
 
 
-class UserAlreadyExists(DomainError):
-    ...
+class UserAlreadyExists(DomainError): ...
 
 
 class AggregateAlreadyExistError(DomainError):
     def __init__(
         self,
         aggregate_id: Uuid,
         repository_name: Optional[str] = None,
         table_name: Optional[str] = None,
     ):
         aggregate_id_str = f" ({aggregate_id.value})" if aggregate_id else ""
         repository_str = f" (repository: {repository_name})" if repository_name else ""
         table_str = f" (table: {table_name})" if repository_name else ""
-        message = (
-            f"Aggregate{aggregate_id_str} already exist{repository_str}{table_str}"
-        )
+        message = f"Aggregate{aggregate_id_str} already exist{repository_str}{table_str}"
         uuid_value = aggregate_id.value if aggregate_id else None
         super().__init__(uuid_value=uuid_value, additional_info={"message": message})
```

### Comparing `petisco-2.1.3/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.1.4/petisco/base/domain/errors/defaults/not_found.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from typing import Optional, Union
 
 from petisco.base.domain.errors.domain_error import DomainError
 from petisco.base.domain.model.uuid import Uuid
 
 
-class NotFound(DomainError):
-    ...
+class NotFound(DomainError): ...
 
 
-class ClientNotFound(DomainError):
-    ...
+class ClientNotFound(DomainError): ...
 
 
-class UserNotFound(DomainError):
-    ...
+class UserNotFound(DomainError): ...
 
 
 class AggregateNotFoundError(DomainError):
     def __init__(self, aggregate_id: Uuid, repository_name: Optional[str] = None):
         aggregate_id_str = f" ({aggregate_id.value})" if aggregate_id else ""
         repository_str = f" (repository: {repository_name})" if repository_name else ""
         message = f"Aggregate{aggregate_id_str} not found{repository_str}"
```

### Comparing `petisco-2.1.3/petisco/base/domain/errors/domain_error.py` & `petisco-2.1.4/petisco/base/domain/errors/domain_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     def set_additional_info(self, info: Optional[Dict[str, str]]) -> None:
         if self.additional_info:
             self.additional_info = dict(self.additional_info, **info)
         else:
             self.additional_info = info
 
     @classmethod
-    @deprecated(
-        "get_specify_detail is deprecated. Use the `get_specific_detail` instead."
-    )
+    @deprecated("get_specify_detail is deprecated. Use the `get_specific_detail` instead.")
     def get_specify_detail(cls) -> str:
         return cls.get_specific_detail()
 
     @classmethod
     def get_specific_detail(cls) -> str:
         return cls.__name__
```

### Comparing `petisco-2.1.3/petisco/base/domain/errors/unknown_error.py` & `petisco-2.1.4/petisco/base/domain/errors/unknown_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,38 +37,29 @@
     def _sanitize_input_params(self, input_parameters: Any) -> Any:
         if isinstance(input_parameters, tuple):
             return {
                 f"param_{i + 1}": param if not isinstance(param, bytes) else "bytes"
                 for i, param in enumerate(input_parameters)
             }
         elif isinstance(input_parameters, dict):
-            return {
-                k: v if not isinstance(v, bytes) else "bytes"
-                for k, v in input_parameters.items()
-            }
+            return {k: v if not isinstance(v, bytes) else "bytes" for k, v in input_parameters.items()}
         else:
             return None
 
-    def _filter_input_parameters(
-        self, filter_parameters: Union[List[str], None] = None
-    ) -> None:
+    def _filter_input_parameters(self, filter_parameters: Union[List[str], None] = None) -> None:
         if filter_parameters:
             self.input_parameters = {
-                k: v
-                for k, v in self.input_parameters.items()
-                if k not in filter_parameters
+                k: v for k, v in self.input_parameters.items() if k not in filter_parameters
             }
 
     def __repr__(self) -> str:
         executor_str = f" ({self.executor})" if self.executor else ""
         traceback_str = f"\n{self.traceback}" if self.traceback else ""
         input_parameters_str = (
-            f"\nInput Parameters: {str(self.input_parameters)}"
-            if self.input_parameters
-            else ""
+            f"\nInput Parameters: {str(self.input_parameters)}" if self.input_parameters else ""
         )
         filename_str = f"\n{self.filename}" if self.filename else ""
         lineno_str = f"\n{self.lineno}" if self.lineno else ""
         return f"{self.__class__.__name__}{executor_str}: {self.message}.{traceback_str}.{input_parameters_str}{filename_str}{lineno_str}"
 
     @classmethod
     def from_exception(
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-2.1.4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/command_bus.py` & `petisco-2.1.4/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/command_subscriber.py` & `petisco-2.1.4/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.1.4/petisco/base/domain/message/domain_event_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     @abstractmethod
     def publish(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
         """
         Publish a DomainEvent or a list of DomainEvents
         """
         raise NotImplementedError
 
-    def _check_is_domain_event(
-        self, domain_event: DomainEvent | list[DomainEvent]
-    ) -> None:
+    def _check_is_domain_event(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
         if not domain_event or not issubclass(domain_event.__class__, DomainEvent):
-            raise TypeError(
-                f"{self.__class__.__name__} only publishes DomainEvent objects"
-            )
+            raise TypeError(f"{self.__class__.__name__} only publishes DomainEvent objects")
 
     @abstractmethod
     def close(self) -> None:
         raise NotImplementedError
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-2.1.4/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/message.py` & `petisco-2.1.4/petisco/base/domain/message/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
             self._update_from_formatted_message()
 
         if not hasattr(self, "_message_id"):
             self._message_id = Uuid.v4()  # noqa
 
         if not hasattr(self, "_message_name"):
             self._message_name = (  # noqa
-                re.sub(r"(?<!^)(?=[A-Z])", "_", self.__class__.__name__)
-                .lower()
-                .replace("_", ".")
+                re.sub(r"(?<!^)(?=[A-Z])", "_", self.__class__.__name__).lower().replace("_", ".")
             )
         if hasattr(self, "Config"):
             self._message_version = get_version(self.Config)
         else:
             self._message_version = 1  # noqa
 
         if not hasattr(self, "_message_occurred_on"):
@@ -97,17 +95,15 @@
         cls,
         formatted_message: Union[Dict[str, Any], str, bytes],
         target_type: Union[type, None] = None,
     ) -> "Message":
         if not isinstance(formatted_message, dict):
             formatted_message = json.loads(formatted_message)
         data = cast(Dict[str, Any], formatted_message.get("data"))
-        attributes = (
-            data.get("attributes") if data.get("attributes") is not None else dict()
-        )
+        attributes = data.get("attributes") if data.get("attributes") is not None else {}
         target_type = target_type if target_type else cls
         message = target_type(**attributes)
         message._message_formatted_message = data
         message._update_from_formatted_message()
         return message
 
     def _get_serialized_attributes(self) -> Dict[str, Any]:
@@ -123,30 +119,26 @@
 
     def _update_from_formatted_message(self) -> None:
         kwargs = self._message_formatted_message
         self._message_id = Uuid(kwargs.get("id")) if kwargs.get("id") else Uuid.v4()
         self._message_name = str(kwargs.get("type"))
         self._message_version = int(kwargs.get("version", 1))
         self._message_occurred_on = (
-            datetime.strptime(str(kwargs.get("occurred_on")), TIME_FORMAT).replace(
-                tzinfo=timezone.utc
-            )
+            datetime.strptime(str(kwargs.get("occurred_on")), TIME_FORMAT).replace(tzinfo=timezone.utc)
             if kwargs.get("occurred_on")
             else datetime.now(timezone.utc)
         )
 
-        attributes = (
-            kwargs.get("attributes") if kwargs.get("attributes") is not None else dict()
-        )
+        attributes = kwargs.get("attributes") if kwargs.get("attributes") is not None else {}
         self._message_attributes = cast(Dict[str, Any], attributes)
         if self._message_attributes:
             for key, value in self._message_attributes.items():
                 setattr(self, key, value)
 
-        self._message_meta = cast(Dict[str, Any], kwargs.get("meta", dict()))
+        self._message_meta = cast(Dict[str, Any], kwargs.get("meta", {}))
         self._message_type = str(kwargs.get("type_message", self._message_type))
 
     def __hash__(self) -> int:
         return hash(self.format_json())
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Message):
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_bus.py` & `petisco-2.1.4/petisco/base/domain/message/message_bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,21 +42,16 @@
     @abstractmethod
     def publish(self, message: TypeMessage | list[TypeMessage]) -> None:
         """
         Publish a message or a list of messages
         """
         raise NotImplementedError
 
-    def _check_input(
-        self, message: TypeMessage | list[TypeMessage]
-    ) -> list[TypeMessage]:  # noqa
-        if isinstance(message, list):
-            messages = message
-        else:
-            messages = [message]
+    def _check_input(self, message: TypeMessage | list[TypeMessage]) -> list[TypeMessage]:  # noqa
+        messages = message if isinstance(message, list) else [message]
         return messages
 
     @abstractmethod
     def close(self) -> None:
         raise NotImplementedError
 
     def _check_is_message(self, message: TypeMessage) -> None:
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_configurer.py` & `petisco-2.1.4/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_consumer.py` & `petisco-2.1.4/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_handler_returns_none_error.py` & `petisco-2.1.4/petisco/base/domain/message/message_handler_returns_none_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 
 from petisco.base.domain.message.message import Message
 
 
 class MessageHandlerReturnsNoneError(ValueError):
     def __init__(self, handler: Callable[[Message], BoolResult]):
         handler_name = getattr(handler, "__name__", repr(handler))
-        handler_module = getattr(handler, "__module__") + "."
+        handler_module = handler.__module__ + "."
         message = f"Subscribers (event handlers) must return a Result object. Please check {handler_module}{handler_name}"
         super().__init__(message)
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_subscriber.py` & `petisco-2.1.4/petisco/base/domain/message/message_subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,19 @@
 
 class MetaMessageSubscriber(type, Interface):
     domain_event_bus: DomainEventBus = NotImplementedDomainEventBus()
     command_bus: CommandBus = NotImplementedCommandBus()
     middlewares: list[Middleware] = []
     use_global_middlewares: bool = True
 
-    def __new__(
-        mcs, name: str, bases: tuple[Any, ...], namespace: dict[str, Any]
-    ) -> MetaMessageSubscriber:
+    def __new__(mcs, name: str, bases: tuple[Any, ...], namespace: dict[str, Any]) -> MetaMessageSubscriber:
         config = namespace.get("Config")
 
         if "handle" not in namespace:
-            raise NotImplementedError(
-                "Petisco MessageSubscriber must implement an handle method"
-            )
+            raise NotImplementedError("Petisco MessageSubscriber must implement an handle method")
 
         mapper = ResultMapper()
 
         new_namespace = {}
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "handle":
                 attribute = wrapper(attribute, name, config, mapper)
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/message_subscriber_info.py` & `petisco-2.1.4/petisco/base/domain/message/message_subscriber_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,15 @@
     message_name: str
     message_version: int
     message_type: str
 
     @staticmethod
     def from_class_type(class_type: type[Message]) -> MessageSubscriberInfo:
         message_name = (  # noqa
-            re.sub(r"(?<!^)(?=[A-Z])", "_", class_type.__name__)
-            .lower()
-            .replace("_", ".")
+            re.sub(r"(?<!^)(?=[A-Z])", "_", class_type.__name__).lower().replace("_", ".")
         )
 
         message_version = 1
         if hasattr(class_type, "Config") and hasattr(class_type.Config, "version"):
             message_version = int(class_type.Config.version)
 
         message_type = "message"
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/not_implemented_command_bus.py` & `petisco-2.1.4/petisco/base/domain/message/not_implemented_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.1.4/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.message.domain_event_bus import DomainEventBus
 
 
 class NotImplementedDomainEventBus(DomainEventBus):
     def publish(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
-        domain_events = (
-            [domain_event] if isinstance(domain_event, DomainEvent) else domain_event
-        )
+        domain_events = [domain_event] if isinstance(domain_event, DomainEvent) else domain_event
         for domain_event in domain_events:
             self._check_is_domain_event(domain_event)
             meta = self.get_configured_meta()
             _ = domain_event.update_meta(meta)
 
     def retry_publish(
         self,
```

### Comparing `petisco-2.1.3/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.1.4/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 class NotImplementedMessageConsumer(MessageConsumer[Any]):
     def start(self) -> NoReturn:
         pass
 
     def add_subscribers(self, subscribers: list[MessageSubscriber]) -> None:
         pass
 
-    def add_subscriber_on_dead_letter(
-        self, subscriber: type[MessageSubscriber]
-    ) -> None:
+    def add_subscriber_on_dead_letter(self, subscriber: type[MessageSubscriber]) -> None:
         pass
 
     def add_subscriber_on_queue(
         self,
         queue_name: str,
         subscriber: type[MessageSubscriber],
         is_store: bool = False,
```

### Comparing `petisco-2.1.3/petisco/base/domain/model/aggregate_root.py` & `petisco-2.1.4/petisco/base/domain/model/aggregate_root.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,15 @@
                         isclass(union_annotation)
                         and issubclass(union_annotation, ValueObject)
                         and isinstance(value, str)
                     ):
                         new_value = union_annotation(value=value)
                         new_data[key] = new_value
             else:
-                if (
-                    isclass(annotation)
-                    and issubclass(annotation, ValueObject)
-                    and isinstance(value, str)
-                ):
+                if isclass(annotation) and issubclass(annotation, ValueObject) and isinstance(value, str):
                     new_value = annotation(value=value)
                     new_data[key] = new_value
         return new_data
 
     @field_serializer("aggregate_id")
     def serialize_aggregate_id(self, aggregate_id: Uuid) -> str:
         return aggregate_id.value
```

### Comparing `petisco-2.1.3/petisco/base/domain/model/legacy_uuid.py` & `petisco-2.1.4/petisco/base/domain/model/legacy_uuid.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/model/uuid.py` & `petisco-2.1.4/petisco/base/domain/model/uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
             python_schema=core_schema.union_schema(
                 [
                     # check if it's an instance first before doing any further work
                     core_schema.is_instance_schema(Uuid),
                     from_uuid_schema,
                 ]
             ),
-            serialization=core_schema.plain_serializer_function_ser_schema(
-                lambda instance: instance.value
-            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(lambda instance: instance.value),
         )
 
     @classmethod
     def __get_pydantic_json_schema__(
         cls, _core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         # Use the same schema that would be used for `uuid`
```

### Comparing `petisco-2.1.3/petisco/base/domain/model/value_object.py` & `petisco-2.1.4/petisco/base/domain/model/value_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from pydantic import BaseModel, PlainSerializer, field_serializer, field_validator
 
 from petisco.base.domain.errors.defaults.invalid_value_object import InvalidValueObject
 
 TypeValueObject = TypeVar("TypeValueObject", bound="ValueObject")
 
 
-ValueObjectSerializer = PlainSerializer(
-    lambda value_object: value_object.value if value_object else None
-)
+ValueObjectSerializer = PlainSerializer(lambda value_object: value_object.value if value_object else None)
 
 
 class ValueObject(BaseModel):
     """
     A base class to define ValueObject
 
     It is small object that represents a simple entity whose equality is not based on identity.
```

### Comparing `petisco-2.1.3/petisco/base/domain/persistence/async_fake_database.py` & `petisco-2.1.4/petisco/base/domain/persistence/async_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/persistence/database.py` & `petisco-2.1.4/petisco/base/domain/persistence/database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/base/domain/persistence/databases.py` & `petisco-2.1.4/petisco/base/domain/persistence/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from petisco.base.domain.persistence.async_database import AsyncDatabase
 from petisco.base.domain.persistence.database import Database
 
 T = TypeVar("T")
 
 
 def get_key(base_type: type[T], alias: str | None = None) -> str:
-    return base_type.__name__ if not alias else alias
+    return alias if alias else base_type.__name__
 
 
 @dataclass
 class _Databases:
     def __init__(self) -> None:
         self._databases: dict[str, Any] = {}
 
@@ -26,17 +26,15 @@
 
     def get_databases(self) -> list[Database[Any]]:
         return list(self._databases.values())
 
     def get_database_names(self) -> list[str]:
         return list(self._databases.keys())
 
-    def add(
-        self, database: Database | list[Database], skip_if_exist: bool = False
-    ) -> None:
+    def add(self, database: Database | list[Database], skip_if_exist: bool = False) -> None:
         if isinstance(database, list):
             for database_ in database:
                 self.add(database_, skip_if_exist)
 
         elif isinstance(database, Database):
             key = database.get_key()
             if key in self._databases:
@@ -68,55 +66,44 @@
         if key in self._databases:
             self._databases[key].delete()
             del self._databases[key]
         else:
             if skip_if_not_exist is False:
                 raise IndexError(f"Database cannot be removed. {key} does not exists")
 
-    def initialize(
-        self, initialization_arguments: dict[str, dict[str, Any]] | None = None
-    ) -> None:
+    def initialize(self, initialization_arguments: dict[str, dict[str, Any]] | None = None) -> None:
         for database in self._databases.values():
             if isinstance(database, AsyncDatabase):
                 continue
-            arguments = (
-                initialization_arguments.get(database.alias)
-                if initialization_arguments
-                else None
-            )
+            arguments = initialization_arguments.get(database.alias) if initialization_arguments else None
             if arguments:
                 database.initialize(**arguments)
             else:
                 database.initialize()
 
     async def async_initialize(
         self, initialization_arguments: dict[str, dict[str, Any]] | None = None
     ) -> None:
         for database in self._databases.values():
             if isinstance(database, AsyncDatabase):
-                arguments = (
-                    initialization_arguments.get(database.alias)
-                    if initialization_arguments
-                    else None
-                )
+                arguments = initialization_arguments.get(database.alias) if initialization_arguments else None
                 if arguments:
                     await database.initialize(**arguments)
                 else:
                     await database.initialize()
 
     def delete(self) -> None:
         for database in self._databases.values():
             database.delete()
 
     def clear_database(self, base_type: type[T], *, alias: str | None = None) -> None:
         key = get_key(base_type, alias)
         databases_ = self._databases
-        if key is not None:
-            if key not in self._databases:
-                raise IndexError(f"Database cannot clear the data. {key} not exists")
+        if key is not None and key not in self._databases:
+            raise IndexError(f"Database cannot clear the data. {key} not exists")
         for database in databases_.values():
             database.clear_data()
 
     def clear(self) -> None:
         self._databases = {}
```

### Comparing `petisco-2.1.3/petisco/base/misc/async_wrapper.py` & `petisco-2.1.4/petisco/base/misc/async_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,19 +58,19 @@
                 arguments=arguments if len(arguments) > 0 else args,
                 class_name=wrapped_class_name,
             )
             result = Failure(unknown_error)
             capture_exception()
         try:
             result.set_transformer(mapper.map)
-        except AttributeError:  # noqa
+        except AttributeError as err:  # noqa
             raise TypeError(
                 f"Controller Error: Return value `{result}` ({type(result)}) must be a `meiga.Result` to "
                 f"transform values to success and failure handlers."
-            )
+            ) from err
 
         for middleware in middlewares:
             if (
                 middleware.scope == MiddlewareScope.ALL
                 or middleware.scope == MiddlewareScope.CONTROLLER
                 and issubclass(args[0].__class__, Controller)
                 or middleware.scope == MiddlewareScope.SUBSCRIBER
@@ -80,16 +80,14 @@
             else:
                 continue
 
             if result:
                 try:
                     middleware.after(result)
                 except Exception as exception:
-                    logger.error(
-                        f"Error in the {wrapped_class_name} middlewares (after)."
-                    )
+                    logger.error(f"Error in the {wrapped_class_name} middlewares (after).")
                     logger.exception(exception)
 
         update_middlewares(config, middlewares)
         return result
 
     return wrapped
```

### Comparing `petisco-2.1.3/petisco/base/misc/builder.py` & `petisco-2.1.4/petisco/base/misc/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,10 @@
                 constructor = getattr(self.klass, self.name_constructor)
                 instance: T = constructor(*self.args, **self.kwargs)
             elif self.is_builder:
                 instance: T = self.klass.build(*self.args, **self.kwargs)
             else:
                 instance: T = self.klass(*self.args, **self.kwargs)
         except Exception as exc:
-            raise RuntimeError(
-                f"Error instantiating {self.klass.__name__}\n{repr(exc)}"
-            )
+            raise RuntimeError(f"Error instantiating {self.klass.__name__}\n{repr(exc)}") from exc
 
         return instance
```

### Comparing `petisco-2.1.3/petisco/base/misc/result_mapper.py` & `petisco-2.1.4/petisco/base/misc/result_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,42 +5,40 @@
 from meiga import AnyResult, Error, Result
 
 from petisco.base.application.controller.error_map import ErrorMap
 from petisco.base.application.controller.http_error import HttpError
 from petisco.base.domain.errors.domain_error import DomainError
 
 
-def default_failure_handler(
-    result: AnyResult, error_map: ErrorMap
-) -> Union[HttpError, AnyResult]:
+def default_failure_handler(result: AnyResult, error_map: ErrorMap) -> Union[HttpError, AnyResult]:
     error_type = type(result.value)
     mapped_result = error_map.get(error_type, result)
     return mapped_result
 
 
 class ResultMapper(ABC):
     def __init__(
         self,
         error_map: Optional[ErrorMap] = None,
         success_handler: Callable[[AnyResult], Any] = lambda result: result,
         failure_handler: Callable[
             [Result[DomainError, Error], Union[ErrorMap, None]], Any
         ] = default_failure_handler,
     ):
-        self.error_map = error_map if error_map is not None else dict()
+        self.error_map = error_map if error_map is not None else {}
         self.success_handler = success_handler
         self.failure_handler = failure_handler
 
     def map(self, result: AnyResult) -> Any:
         try:
             if result.is_success:
                 return self.success_handler(result)
             else:
                 if "error_map" in inspect.signature(self.failure_handler).parameters:
                     return self.failure_handler(result, self.error_map)
                 else:
                     return self.failure_handler(result)  # noqa
-        except AttributeError:  # noqa
+        except AttributeError as err:
             raise TypeError(
                 f"Controller Error: Return value `{result}` ({type(result)}) must be a `meiga.Result` to "
                 f"map values to success and failure handlers."
-            )
+            ) from err
```

### Comparing `petisco-2.1.3/petisco/base/misc/singleton.py` & `petisco-2.1.4/petisco/base/misc/singleton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 from typing import Any, Dict
 
 
 class Singleton(type):
     _instances: Dict[Any, Any] = {}
 
     def __call__(cls, *args: Any, **kwargs: Any) -> Any:
@@ -11,11 +12,9 @@
             cls._instances[cls] = super().__call__(*args, **kwargs)
         elif force:
             cls.clear()
             cls._instances[cls] = super().__call__(*args, **kwargs)
         return cls._instances[cls]
 
     def clear(cls) -> None:
-        try:
+        with contextlib.suppress(KeyError):
             del Singleton._instances[cls]
-        except KeyError:
-            pass
```

### Comparing `petisco-2.1.3/petisco/base/misc/wrapper.py` & `petisco-2.1.4/petisco/base/misc/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
     for middlewares_config in middlewares_configs:
         if not isinstance(middlewares_config, Middleware):
             try:
                 middlewares_instances.append(middlewares_config())
             except TypeError as exc:
                 raise TypeError(
                     f"Middlewares cannot have configurable constructor, please review your petisco extension.\n{str(exc)}"
-                )
+                ) from exc
         else:
             middlewares_instances.append(middlewares_config)
 
     return middlewares_instances
 
 
 def update_middlewares(config: Dict[str, Any], middlewares: List[Middleware]) -> None:
     if config is not None and hasattr(config, "middlewares"):
-        setattr(config, "middlewares", middlewares)
+        config.middlewares = middlewares
 
 
 def get_global_middlewares() -> List[Middleware]:
     environment_middlewares = get_middlewares_configuration_from_environment()
     shared_middlewares = ApplicationInfo().shared_middlewares
 
     return list(set(environment_middlewares + shared_middlewares))
@@ -62,23 +62,19 @@
         my_type = lookup_table.get(name)
         if not my_type:
             raise TypeError(
                 f"Value {name} in PETISCO_DEFAULT_MIDDLEWARES is not valid. Please, use {list(lookup_table.keys())}"
             )
         return my_type
 
-    default_middlewares_names: Union[str, None] = os.getenv(
-        "PETISCO_DEFAULT_MIDDLEWARES"
-    )
+    default_middlewares_names: Union[str, None] = os.getenv("PETISCO_DEFAULT_MIDDLEWARES")
     if not default_middlewares_names:
         return []
     default_middlewares_names_list = default_middlewares_names.split(",")
-    return [
-        gettype(middleware_name) for middleware_name in default_middlewares_names_list
-    ]
+    return [gettype(middleware_name) for middleware_name in default_middlewares_names_list]
 
 
 def wrapper(
     execute_func: Callable[..., Any],
     wrapped_class_name: str,
     config: Any,
     mapper: ResultMapper,
@@ -128,16 +124,15 @@
         if not isinstance(result, Result):
             raise TypeError(
                 f"Controller Error: Return value `{result}` ({type(result)}) must be a `meiga.Result`"
             )
 
         if isinstance(result.value, CriticalError) and len(arguments) > 0:
             formatted_args = {
-                k: str(v) if type(v) is not bytes else "bytes"
-                for k, v in arguments.items()
+                k: str(v) if not isinstance(v, bytes) else "bytes" for k, v in arguments.items()
             }
             result.value.set_additional_info(formatted_args)
 
         result.set_transformer(mapper.map)
         for middleware in middlewares:
             if (
                 middleware.scope == MiddlewareScope.ALL
@@ -150,16 +145,14 @@
             else:
                 continue
 
             if result:
                 try:
                     middleware.after(result)
                 except Exception as exception:
-                    logger.error(
-                        f"Error in the {wrapped_class_name} middlewares (after)."
-                    )
+                    logger.error(f"Error in the {wrapped_class_name} middlewares (after).")
                     logger.exception(exception)
 
         update_middlewares(config, middlewares)
         return result
 
     return wrapped
```

### Comparing `petisco-2.1.3/petisco/cli/petisco.py` & `petisco-2.1.4/petisco/cli/petisco.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def rename_template(original_name: str, replacement: str) -> None:
     for dname, _, _ in os.walk("."):
         if original_name in dname:
             os.rename(dname, dname.replace(original_name, replacement))
 
     blacklist = [".git/", ".idea"]
-    for dname, dirs, files in os.walk("."):
+    for dname, _dirs, files in os.walk("."):
         for fname in files:
             fpath = os.path.join(dname, fname)
             rewrite = True
             for blackfolder in blacklist:
                 if blackfolder in fpath:
                     rewrite = False
             if rewrite is False:
@@ -41,21 +41,17 @@
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog="petisco 🍪",
         description="petisco is a framework for helping Python developers to build clean Applications",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    parser.add_argument(
-        "-v", "--version", action="store_true", help="show petisco version number."
-    )
+    parser.add_argument("-v", "--version", action="store_true", help="show petisco version number.")
     parser.add_argument("-uuid", "--uuid", action="store_true", help="show an UUID v4.")
-    parser.add_argument(
-        "-utcnow", "--utcnow", action="store_true", help="show a utc now datetime"
-    )
+    parser.add_argument("-utcnow", "--utcnow", action="store_true", help="show a utc now datetime")
     parser.add_argument(
         "-rt",
         "--rename-template",
         action="store",
         dest="rename_template_replacement",
         default=None,
         help="Rename a petisco service template.",
@@ -86,11 +82,9 @@
             print(datetime.now(timezone.utc))
             return
 
         if args.rename_template_replacement:
             print(
                 f"petisco 🍪 => Changing {args.original_template_name} for {args.rename_template_replacement}..."
             )
-            rename_template(
-                args.original_template_name, args.rename_template_replacement
-            )
+            rename_template(args.original_template_name, args.rename_template_replacement)
             return
```

### Comparing `petisco-2.1.3/petisco/cli/petisco_dev.py` & `petisco-2.1.4/petisco/cli/petisco_dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def get_application(module_path: str):
     logger.remove()
     logger.add(sys.stderr, level="ERROR")
 
     try:
         module_name = importlib.import_module(module_path)
-        application = getattr(module_name, "application")
+        application = module_name.application
         return application
     except Exception as exc:  # noqa
         print(
             f"Error loading the app module. Impossible to extract information from {module_path}. "
             f"There is no application instance in {module_path}"
         )
         print(
@@ -115,30 +115,26 @@
             default_implementation = dependency.builders.pop("default").klass.__name__
 
             implementations = ""
             for key, builder in dependency.builders.items():
                 implementations += f"{key}: {builder.klass.__name__}\n"
             implementations = implementations[:-1]
 
-            table.add_row(
-                type, default_implementation, implementations, dependency.envar_modifier
-            )
+            table.add_row(type, default_implementation, implementations, dependency.envar_modifier)
 
         console.print(table)
 
 
 def show_configurers(application) -> None:
     configurers = application.configurers
 
     if is_rich_available() is False:
         print("Configurers:")
         for configurer in configurers:
-            print(
-                f"{configurer.__class__.__name__} -> {configurer.execute_after_dependencies=}"
-            )
+            print(f"{configurer.__class__.__name__} -> {configurer.execute_after_dependencies=}")
         encourage_rich_installation()
     else:
         from rich.console import Console
         from rich.table import Table
 
         table = Table()
         console = Console()
@@ -286,17 +282,15 @@
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog="petisco-dev 🍪",
         description="petisco dev tools to inspect your application",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    parser.add_argument(
-        "-i", "--info", action="store_true", help="show petisco app info."
-    )
+    parser.add_argument("-i", "--info", action="store_true", help="show petisco app info.")
     parser.add_argument(
         "-deps",
         "--dependencies",
         action="store_true",
         help="show petisco app dependencies.",
     )
     parser.add_argument(
```

### Comparing `petisco-2.1.3/petisco/cli/petisco_rabbitmq.py` & `petisco-2.1.4/petisco/cli/petisco_rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     def logging_config() -> None:
         logging.getLogger("pika").setLevel(logging.WARNING)
 
     logger = LoggingBasedLogger("example", config=logging_config)
     return logger
 
 
-class MyDomainEvent(DomainEvent):
-    ...
+class MyDomainEvent(DomainEvent): ...
 
 
 class UnackMessage(MessageSubscriber):
     def subscribed_to(self) -> List[Type[Message]]:
         return [MyDomainEvent]
 
     def handle(self, message: Message) -> BoolResult:
@@ -173,17 +172,15 @@
         class RequeueOnMessage(AllMessageSubscriber):
             def handle(self, message: Message) -> BoolResult:
                 if args.wait_to_requeue:
                     sleep(args.wait_sec)
 
                 message = cast(DomainEvent, message)
 
-                self.domain_event_bus.retry_publish(
-                    message, args.retry_routing_key, args.retry_exchange_name
-                )
+                self.domain_event_bus.retry_publish(message, args.retry_routing_key, args.retry_exchange_name)
 
                 return isSuccess
 
         consumer.add_subscriber_on_queue(
             queue_name=args.consuming_queue,
             subscriber=RequeueOnMessage,
             message_type_expected="domain_event",
```

### Comparing `petisco-2.1.3/petisco/extra/elastic/__init__.py` & `petisco-2.1.4/petisco/extra/elastic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from petisco.extra.elastic.is_elastic_available import is_elastic_available
 
-elastic = list()
+elastic = []
 if is_elastic_available():
     from petisco.extra.elastic.async_elastic_database import (
         AsyncElasticDatabase,
         AsyncElasticSessionScope,
     )
     from petisco.extra.elastic.elastic_connection import ElasticConnection
     from petisco.extra.elastic.elastic_database import (
```

### Comparing `petisco-2.1.3/petisco/extra/elastic/async_elastic_database.py` & `petisco-2.1.4/petisco/extra/elastic/async_elastic_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,19 @@
 
 
 class AsyncElasticDatabase(AsyncDatabase):
     session: AsyncElasticsearch | None = None
 
     @staticmethod
     def local_connection_checker(alias: str | None = "test") -> AsyncElasticDatabase:
-        return AsyncElasticDatabase(
-            alias=alias, connection=ElasticConnection.create_local()
-        )
+        return AsyncElasticDatabase(alias=alias, connection=ElasticConnection.create_local())
 
     def __init__(self, alias: str, connection: ElasticConnection) -> None:
         if not connection or not isinstance(connection, ElasticConnection):
-            raise ConnectionError(
-                "ElasticDatabase needs a valid ElasticConnection connection"
-            )
+            raise ConnectionError("ElasticDatabase needs a valid ElasticConnection connection")
         self.connection = connection
         super().__init__(alias)
 
     def initialize(self) -> None:
         self.session = AsyncElasticsearch(
             self.connection.to_elastic_format(), http_auth=self.connection.http_auth
         )
```

### Comparing `petisco-2.1.3/petisco/extra/elastic/elastic_connection.py` & `petisco-2.1.4/petisco/extra/elastic/elastic_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     def http_auth(self) -> Union[Tuple[str, str], None]:
         http_auth = None
         if self.username and self.password:
             http_auth = (self.username, self.password)
         return http_auth
 
     @staticmethod
-    def create(
-        username: str, password: str, host: str, port: str
-    ) -> "ElasticConnection":
+    def create(username: str, password: str, host: str, port: str) -> "ElasticConnection":
         return ElasticConnection(username, password, host, port)
 
     @staticmethod
     def create_local() -> "ElasticConnection":
         return ElasticConnection(host="http://localhost")
 
     @staticmethod
```

### Comparing `petisco-2.1.3/petisco/extra/elastic/elastic_database.py` & `petisco-2.1.4/petisco/extra/elastic/elastic_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,20 @@
 
     @staticmethod
     def local_connection_checker(alias: str | None = "test") -> ElasticDatabase:
         return ElasticDatabase(alias=alias, connection=ElasticConnection.create_local())
 
     def __init__(self, alias: str, connection: ElasticConnection) -> None:
         if not connection or not isinstance(connection, ElasticConnection):
-            raise ConnectionError(
-                "ElasticDatabase needs a valid ElasticConnection connection"
-            )
+            raise ConnectionError("ElasticDatabase needs a valid ElasticConnection connection")
         self.connection = connection
         super().__init__(alias)
 
     def initialize(self) -> None:
-        self.session = Elasticsearch(
-            self.connection.to_elastic_format(), http_auth=self.connection.http_auth
-        )
+        self.session = Elasticsearch(self.connection.to_elastic_format(), http_auth=self.connection.http_auth)
 
     def delete(self) -> None:
         pass
 
     def clear_data(self) -> None:
         pass
```

### Comparing `petisco-2.1.3/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.1.4/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/elastic/elastic_repository.py` & `petisco-2.1.4/petisco/extra/elastic/elastic_repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,41 +30,29 @@
 
     @classmethod
     def fail_if_aggregate_already_exist(
         cls, model: Any, aggregate_id: Uuid, result_error: Union[Error, None] = None
     ) -> BoolResult:
         if model:
             error = (
-                AggregateAlreadyExistError(
-                    aggregate_id, cls.__name__, model.__tablename__
-                )
-                if not result_error
-                else result_error
+                result_error
+                if result_error
+                else AggregateAlreadyExistError(aggregate_id, cls.__name__, model.__tablename__)
             )
             return Failure(error)
         return isSuccess
 
     @classmethod
     def fail_if_aggregate_not_found(
         cls, model: Any, aggregate_id: Uuid, result_error: Union[Error, None] = None
     ) -> BoolResult:
         if not model:
-            error = (
-                AggregateNotFoundError(aggregate_id, cls.__name__)
-                if not result_error
-                else result_error
-            )
+            error = result_error if result_error else AggregateNotFoundError(aggregate_id, cls.__name__)
             return Failure(error)
         return isSuccess
 
     @classmethod
-    def fail_if_aggregates_not_found(
-        cls, model: Any, result_error: Union[Error, None] = None
-    ) -> BoolResult:
+    def fail_if_aggregates_not_found(cls, model: Any, result_error: Union[Error, None] = None) -> BoolResult:
         if not model:
-            error = (
-                AggregatesNotFoundError(cls.__name__)
-                if not result_error
-                else result_error
-            )
+            error = result_error if result_error else AggregatesNotFoundError(cls.__name__)
             return Failure(error)
         return isSuccess
```

### Comparing `petisco-2.1.3/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py` & `petisco-2.1.4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     @abstractmethod
     def execute(self, *args: Any, **kwargs: Dict[str, Any]) -> AnyResult:
         return NotImplementedMethodError
 
     def _set_transaction(self, transaction: Transaction) -> None:
         self.transaction = transaction
 
-    def with_transaction(
-        self, transaction: Transaction
-    ) -> "ElasticApmMonitoringAppService":
+    def with_transaction(self, transaction: Transaction) -> "ElasticApmMonitoringAppService":
         service = copy.copy(self)
         service._set_transaction(transaction)
         return service
 
     def monitoring(self) -> None:
         if hasattr(self, "transaction"):
             execution_context.set_transaction(self.transaction)
```

### Comparing `petisco-2.1.3/petisco/extra/fastapi/__init__.py` & `petisco-2.1.4/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/fastapi/application/ensure_all_routers_are_async.py` & `petisco-2.1.4/petisco/extra/fastapi/application/ensure_all_routers_are_async.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 from loguru import logger
 
 
 def is_async_callable(route: APIRoute) -> bool:
     endpoint = route.endpoint
     import asyncio
 
-    if asyncio.iscoroutinefunction(endpoint):
-        return True
-    else:
-        return False
+    return bool(asyncio.iscoroutinefunction(endpoint))
 
 
 def ensure_all_routers_are_async(app: FastAPI) -> None:
     for route in app.routes:
-        if isinstance(route, APIRoute):
-            if not is_async_callable(route):
-                logger.error(f"Router with {route.path} is not using async definition")
-                raise SystemError(
-                    f"Router of {route.path} is not using async definition"
-                )
+        if isinstance(route, APIRoute) and not is_async_callable(route):
+            logger.error(f"Router with {route.path} is not using async definition")
+            raise SystemError(f"Router of {route.path} is not using async definition")
```

### Comparing `petisco-2.1.3/petisco/extra/fastapi/application/fastapi_application.py` & `petisco-2.1.4/petisco/extra/fastapi/application/fastapi_application.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/fastapi/application/response_mocker.py` & `petisco-2.1.4/petisco/extra/fastapi/application/response_mocker.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @classmethod
     def responses(cls) -> Union[Dict[Union[int, str], Dict[str, Any]], None]:
         controller = cls()
 
         if not hasattr(controller, "Config"):
             return None
 
-        config = getattr(controller, "Config")
+        config = controller.Config
         if not hasattr(config, "error_map"):
             return None
 
         expected_responses = {
             http_error.status_code: {"description": http_error.detail}
             for http_error in config.error_map.values()
         }
```

### Comparing `petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,46 +25,37 @@
 
         elasticapm.set_custom_context({"http_response": str(http_error)})
 
     internal_error_message = None
     if isinstance(result.value, UnknownError):
         internal_error_message = str(result.value.__dict__)
     elif error_type not in error_map:
-        internal_error_message = (
-            f"Error '{result.value.__class__.__name__}' is not mapped in controller"
-        )
+        internal_error_message = f"Error '{result.value.__class__.__name__}' is not mapped in controller"
 
     if internal_error_message is not None:
         logger.error(internal_error_message)
         if is_elastic_apm_available():
             import elasticapm  # noqa
 
-            elasticapm.set_custom_context(
-                {"internal_error_message": internal_error_message}
-            )
+            elasticapm.set_custom_context({"internal_error_message": internal_error_message})
 
     detail = http_error.detail
     if isinstance(domain_error, DomainError):
         detail = (
-            http_error.detail
-            if http_error.detail != DEFAULT_HTTP_ERROR_DETAIL
-            else domain_error.detail()
+            http_error.detail if http_error.detail != DEFAULT_HTTP_ERROR_DETAIL else domain_error.detail()
         )
     else:
         logger.warning(
             f"fastapi_failure_handler: {domain_error.__class__.__name__} is not a DomainError (warning "
             f"mapping error)"
         )
 
     assert isinstance(http_error.status_code, int)
     http_exception = HTTPException(
         status_code=http_error.status_code, detail=detail, headers=http_error.headers
     )
 
-    if (
-        isinstance(domain_error, DomainError)
-        and type(domain_error) not in DEFAULT_HTTP_ERROR_MAP.keys()
-    ):
+    if isinstance(domain_error, DomainError) and type(domain_error) not in DEFAULT_HTTP_ERROR_MAP:
         logger.error(f"DomainError:  {domain_error.__repr__()}")
         logger.error(f"HTTPException: {http_exception.__repr__()}")
 
     raise http_exception
```

### Comparing `petisco-2.1.3/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/fastapi/testing/assert_http_exception.py` & `petisco-2.1.4/petisco/extra/fastapi/testing/assert_http_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,8 +3,11 @@
 
 def assert_http_exception(
     http_exception_current: HTTPException, http_exception_expected: HTTPException
 ) -> None:
     assert (
         http_exception_current.status_code == http_exception_expected.status_code
         and http_exception_current.detail == http_exception_expected.detail
-    ), f"| status_code: {http_exception_current.status_code} - {http_exception_expected.status_code} | -> | detail: {http_exception_current.detail} - {http_exception_expected.detail}|"
+    ), (
+        f"| status_code: {http_exception_current.status_code} - {http_exception_expected.status_code} | -> "
+        f"| detail: {http_exception_current.detail} - {http_exception_expected.detail}|"
+    )
```

### Comparing `petisco-2.1.3/petisco/extra/logger/__init__.py` & `petisco-2.1.4/petisco/extra/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/logger/log_message.py` & `petisco-2.1.4/petisco/extra/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/logger/logging_based_logger.py` & `petisco-2.1.4/petisco/extra/logger/logging_based_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     def __init__(
         self,
         logger_name: str,
         format: str = "%(name)s - %(levelname)s - %(message)s",
         config: Callable = None,
     ):
         self.logging_level = os.environ.get("PETISCO_LOGGING_LEVEL", "INFO").upper()
-        logging_level_value = CORRESPONDENCES_LOGGING_LEVEL.get(
-            self.logging_level, logging.INFO
-        )
+        logging_level_value = CORRESPONDENCES_LOGGING_LEVEL.get(self.logging_level, logging.INFO)
         logging.basicConfig(format=format, level=logging_level_value)
         if config:
             config()
         self.logger = logging.getLogger(logger_name)
         self.logger.setLevel(logging_level_value)
         self.logger.info(f"Set PETISCO_LOGGING_LEVEL: {self.logging_level}")
```

### Comparing `petisco-2.1.3/petisco/extra/logger/loguru_logger.py` & `petisco-2.1.4/petisco/extra/logger/loguru_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,13 +33,10 @@
             logger.critical(message)
         elif logging_level == FATAL:
             message["meta"]["level"] = "fatal"
             logger.error(message)
         elif logging_level == ERROR:
             message["meta"]["level"] = "error"
             logger.error(message)
-        elif logging_level == WARN:
-            message["meta"]["level"] = "warning"
-            logger.warning(message)
-        elif logging_level == WARNING:
+        elif logging_level in (WARN, WARNING):
             message["meta"]["level"] = "warning"
             logger.warning(message)
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/__init__.py` & `petisco-2.1.4/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.spec import Basic
 
 from petisco.base.domain.message.chaos.message_chaos import MessageChaos
 
 MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY = "MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK"
-MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS_KEY = (
-    "MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS"
-)
-MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY = (
-    "MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES"
-)
+MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS_KEY = "MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS"
+MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY = "MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES"
 
 MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY = "MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS"
 
 
 class RabbitMqMessageChaos(MessageChaos):
     def __init__(
         self,
@@ -40,50 +36,38 @@
             Routing keys where chaos will not be applied
         """
         self._set_percentage_simulate_nack(percentage_simulate_nack)
         self._set_delay_before_even_handler_second(delay_before_event_handler_second)
         self._set_percentage_simulate_failures(percentage_simulate_failures)
         self._set_protected_routing_keys(protected_routing_keys)
 
-    def _set_percentage_simulate_nack(
-        self, percentage_simulate_nack: Optional[Union[float, str]]
-    ) -> None:
+    def _set_percentage_simulate_nack(self, percentage_simulate_nack: Optional[Union[float, str]]) -> None:
         if percentage_simulate_nack is None:
-            percentage_simulate_nack = os.environ.get(
-                MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY
-            )
+            percentage_simulate_nack = os.environ.get(MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY)
         self.percentage_simulate_nack = self._float(percentage_simulate_nack)
 
     def _set_delay_before_even_handler_second(
         self, delay_before_even_handler_second: Optional[Union[float, str]]
     ) -> None:
         if delay_before_even_handler_second is None:
             delay_before_even_handler_second = os.environ.get(
                 MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS_KEY
             )
-        self.delay_before_even_handler_second = self._float(
-            delay_before_even_handler_second
-        )
+        self.delay_before_even_handler_second = self._float(delay_before_even_handler_second)
 
     def _set_percentage_simulate_failures(
         self, percentage_simulate_failures: Optional[Union[float, str]]
     ) -> None:
         if percentage_simulate_failures is None:
-            percentage_simulate_failures = os.environ.get(
-                MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY
-            )
+            percentage_simulate_failures = os.environ.get(MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY)
         self.percentage_simulate_failures = self._float(percentage_simulate_failures)
 
-    def _set_protected_routing_keys(
-        self, protected_routing_keys: Optional[Union[List[str], str]]
-    ) -> None:
+    def _set_protected_routing_keys(self, protected_routing_keys: Optional[Union[List[str], str]]) -> None:
         if protected_routing_keys is None:
-            protected_routing_keys = os.environ.get(
-                MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY
-            )
+            protected_routing_keys = os.environ.get(MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY)
         self.protected_routing_keys = self._list(protected_routing_keys)
 
     def _float(self, value: Optional[Union[float, str]]) -> Union[float, None]:
         return float(value) if value is not None else None
 
     def _list(self, value: Optional[Union[List[str], str]]) -> Union[List[str], None]:
         if value is None:
@@ -103,41 +87,31 @@
             MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY: self.percentage_simulate_failures,
             MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY: self.protected_routing_keys,
         }
 
     def nack_simulation(self, ch: BlockingChannel, method: Basic.Deliver) -> bool:
         routing_key = method.routing_key if method else None
 
-        if (self.percentage_simulate_nack is None) or (
-            random.random() > self.percentage_simulate_nack
-        ):
+        if (self.percentage_simulate_nack is None) or (random.random() > self.percentage_simulate_nack):
             return False
 
-        if (
-            self.protected_routing_keys is None
-            or routing_key not in self.protected_routing_keys
-        ):
+        if self.protected_routing_keys is None or routing_key not in self.protected_routing_keys:
             ch.basic_nack(delivery_tag=method.delivery_tag)
             return True
         else:
             return False
 
     def failure_simulation(self, method: Basic.Deliver) -> bool:
         routing_key = method.routing_key if method else None
 
         if (self.percentage_simulate_failures is None) or (
             random.random() > self.percentage_simulate_failures
         ):
             return False
         else:
-            return (
-                True
-                if self.protected_routing_keys is None
-                or routing_key not in self.protected_routing_keys
-                else False
-            )
+            return bool(self.protected_routing_keys is None or routing_key not in self.protected_routing_keys)
 
     def delay(self) -> None:
         if self.delay_before_even_handler_second is None:
             pass
         else:
             sleep(self.delay_before_even_handler_second)
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     Implementation is based on pika library.
     """
 
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: Union[
-            RabbitMqConnector, RabbitMqConsumerConnector
-        ] = RabbitMqConnector(),
+        connector: Union[RabbitMqConnector, RabbitMqConsumerConnector] = RabbitMqConnector(),
         fallback: Union[CommandBus, None] = None,
     ):
         self.connector = connector
         self.exchange_name = f"{organization}.{service}"
         self.rabbitmq_key = f"publisher-{self.exchange_name}"
         self.configurer = RabbitMqMessageConfigurer(organization, service, connector)
         self.already_configured = False
@@ -50,35 +48,29 @@
         meta = self.get_configured_meta()
         dispatched_commands = []
         commands = self._check_input(command)
 
         try:
             check_chaos_publication()
             channel = self.connector.get_channel(self.rabbitmq_key)
-            for command in commands:
+            for i, command in enumerate(commands):
                 self._check_is_command(command)
                 command = command.update_meta(meta)
-                self.publisher.execute(channel, command)
-                if channel.is_open and not isinstance(
-                    self.connector, RabbitMqConsumerConnector
-                ):
+                self.publisher.execute(channel, command, first_time=i == 0)
+                if channel.is_open and not isinstance(self.connector, RabbitMqConsumerConnector):
                     channel.close()
                 dispatched_commands.append(command)
         except ChannelClosedByBroker:
-            unpublished_commands = [
-                command for command in commands if command not in dispatched_commands
-            ]
+            unpublished_commands = [command for command in commands if command not in dispatched_commands]
             self._retry(unpublished_commands)
         except Exception as exc:  # noqa
             if not self.fallback:
                 raise exc
 
-            unpublished_commands = [
-                command for command in commands if command not in dispatched_commands
-            ]
+            unpublished_commands = [command for command in commands if command not in dispatched_commands]
             self.fallback.dispatch(unpublished_commands)
 
     def _retry(self, command: Union[Command, List[Command]]) -> None:
         # If command queue is not configured, it will be configured and then try to dispatch again.
         if not self.already_configured:
             self.configurer.configure()
             self.already_configured = True
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     Implementation is based on pika library.
     """
 
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: Union[
-            RabbitMqConnector, RabbitMqConsumerConnector
-        ] = RabbitMqConnector(),
+        connector: Union[RabbitMqConnector, RabbitMqConsumerConnector] = RabbitMqConnector(),
         fallback: Union[DomainEventBus, None] = None,
     ):
         self.connector = connector
         self.exchange_name = f"{organization}.{service}"
         self.rabbitmq_key = f"publisher-{self.exchange_name}"
         self.configurer = RabbitMqMessageConfigurer(organization, service, connector)
         self.already_configured = False
@@ -49,22 +47,20 @@
         meta = self.get_configured_meta()
         published_domain_event = []
         domain_events = self._check_input(domain_event)
 
         try:
             check_chaos_publication()
             channel = self.connector.get_channel(self.rabbitmq_key)
-            for domain_event in domain_events:
+            for i, domain_event in enumerate(domain_events):
                 self._check_is_domain_event(domain_event)
                 domain_event = domain_event.update_meta(meta)
-                self.publisher.execute(channel, domain_event)
+                self.publisher.execute(channel, domain_event, first_time=i == 0)
                 published_domain_event.append(domain_event)
-            if channel.is_open and not isinstance(
-                self.connector, RabbitMqConsumerConnector
-            ):
+            if channel.is_open and not isinstance(self.connector, RabbitMqConsumerConnector):
                 channel.close()
         except ChannelClosedByBroker:
             unpublished_domain_events = [
                 event for event in domain_events if event not in published_domain_event
             ]
             self._retry(unpublished_domain_events)
         except Exception as exc:  # noqa
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,20 +15,22 @@
         self._properties = BasicProperties(delivery_mode=2)  # PERSISTENT_TEXT_PLAIN
 
     def execute(
         self,
         channel: BlockingChannel,
         message: Message,
         routing_key: Union[str, None] = None,
+        first_time: bool = False,
     ) -> None:
         if routing_key is None:
-            routing_key = RabbitMqMessageQueueNameFormatter.format(
-                message, exchange_name=self._exchange_name
-            )
+            routing_key = RabbitMqMessageQueueNameFormatter.format(message, exchange_name=self._exchange_name)
 
-        channel.confirm_delivery()
+        if first_time:
+            # Confirm delivery should be enabled just once. Source: https://www.rabbitmq.com/tutorials/tutorial-seven-java#enabling-publisher-confirms-on-a-channel
+            # Otherwise with Pika we get lots of error messages
+            channel.confirm_delivery()
         channel.basic_publish(
             exchange=self._exchange_name,
             routing_key=routing_key,
             body=message.format_json().encode(),
             properties=self._properties,
         )
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,23 @@
     This class configures exchanges, queue bindings and routing keys from defined MessageSubscribers.
     """
 
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: Union[
-            RabbitMqConnector, RabbitMqConsumerConnector
-        ] = RabbitMqConnector(),
+        connector: Union[RabbitMqConnector, RabbitMqConsumerConnector] = RabbitMqConnector(),
         queue_config: QueueConfig = QueueConfig.default(),
         use_store_queues: bool = True,
     ) -> None:
         self._use_store_queues = use_store_queues
         self.subscribers_configurer = RabbitMqMessageSubcribersConfigurer(
             organization, service, connector, queue_config
         )
-        self.store_configurer = RabbitMqMessageStoreConfigurer(
-            organization, service, connector, queue_config
-        )
+        self.store_configurer = RabbitMqMessageStoreConfigurer(organization, service, connector, queue_config)
 
     def configure(self) -> None:
         """
         Define exchanges, queue bindings and routing key with empty subscribers.
         """
         self.configure_subscribers([])
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,20 @@
         organization: str,
         service: str,
         connector: Union[RabbitMqConnector, RabbitMqConsumerConnector],
         queue_config: QueueConfig,
     ) -> None:
         self._connector = connector
         self._exchange_name = f"{organization}.{service}"
-        self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(
-            self._exchange_name
-        )
-        self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(
-            self._exchange_name
-        )
+        self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(self._exchange_name)
+        self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(self._exchange_name)
         self._common_retry_exchange_name = f"retry.{organization}.store"
         self._common_dead_letter_exchange_name = f"dead_letter.{organization}.store"
 
-        self.rabbitmq = RabbitMqDeclarer(
-            connector=self._connector, channel_name=self._exchange_name
-        )
+        self.rabbitmq = RabbitMqDeclarer(connector=self._connector, channel_name=self._exchange_name)
         self.queue_config = queue_config
 
     def execute(self) -> None:
         self._configure_exchanges()
         self._declare_queues(
             self._exchange_name,
             self._retry_exchange_name,
@@ -99,20 +93,16 @@
             )
             self.rabbitmq.bind_queue(
                 exchange_name=dead_letter_exchange_name,
                 queue_name="dead_letter.store",
                 routing_key=f"dead_letter.{routing_key_any_message}",
             )
 
-        self.rabbitmq.bind_queue(
-            exchange_name=exchange_name, queue_name="store", routing_key="retry.store"
-        )
-        self.rabbitmq.bind_queue(
-            exchange_name=exchange_name, queue_name="store", routing_key="store"
-        )
+        self.rabbitmq.bind_queue(exchange_name=exchange_name, queue_name="store", routing_key="retry.store")
+        self.rabbitmq.bind_queue(exchange_name=exchange_name, queue_name="store", routing_key="store")
 
         self.rabbitmq.bind_queue(
             exchange_name=self._common_retry_exchange_name,
             queue_name="store",
             routing_key="store",
         )
         self.rabbitmq.bind_queue(
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,17 @@
         organization: str,
         service: str,
         connector: Union[RabbitMqConnector, RabbitMqConsumerConnector],
         queue_config: QueueConfig,
     ) -> None:
         self._connector = connector
         self._exchange_name = f"{organization}.{service}"
-        self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(
-            self._exchange_name
-        )
-        self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(
-            self._exchange_name
-        )
-        self.rabbitmq = RabbitMqDeclarer(
-            connector=self._connector, channel_name=self._exchange_name
-        )
+        self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(self._exchange_name)
+        self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(self._exchange_name)
+        self.rabbitmq = RabbitMqDeclarer(connector=self._connector, channel_name=self._exchange_name)
         self._configured_subscribers: List[Any] = []
         self.queue_config = queue_config
 
     def execute(self, subscribers: List[Type[MessageSubscriber]]) -> None:
         self._configure_exchanges()
         self._declare_queues(
             self._exchange_name,
@@ -72,23 +66,19 @@
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
                     break
 
                 queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
                     subscriber_info, exchange_name=self._exchange_name
                 )
-                retry_queue_name = (
-                    RabbitMqMessageSubscriberQueueNameFormatter.format_retry(
-                        subscriber_info, exchange_name=self._exchange_name
-                    )
-                )
-                dead_letter_queue_name = (
-                    RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
-                        subscriber_info, exchange_name=self._exchange_name
-                    )
+                retry_queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_retry(
+                    subscriber_info, exchange_name=self._exchange_name
+                )
+                dead_letter_queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
+                    subscriber_info, exchange_name=self._exchange_name
                 )
 
                 suffix = subscriber.get_subscriber_name()
                 name = f"{queue_name}.{suffix}"
                 retry_name = f"{retry_queue_name}.{suffix}"
                 dead_letter_name = f"{dead_letter_queue_name}.{suffix}"
                 self.rabbitmq.delete_queue(name)
@@ -108,23 +98,19 @@
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
                     break
 
                 base_queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
                     subscriber_info, exchange_name=exchange_name
                 )
-                base_retry_queue_name = (
-                    RabbitMqMessageSubscriberQueueNameFormatter.format_retry(
-                        subscriber_info, exchange_name=exchange_name
-                    )
-                )
-                base_dead_letter_queue_name = (
-                    RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
-                        subscriber_info, exchange_name=exchange_name
-                    )
+                base_retry_queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_retry(
+                    subscriber_info, exchange_name=exchange_name
+                )
+                base_dead_letter_queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
+                    subscriber_info, exchange_name=exchange_name
                 )
                 routing_key = base_queue_name
                 suffix = subscriber.get_subscriber_name()
 
                 queue_name = f"{base_queue_name}.{suffix}"
                 retry_queue_name = f"{base_retry_queue_name}.{suffix}"
                 dead_letter_queue_name = f"{base_dead_letter_queue_name}.{suffix}"
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 
 
 class RabbitMqMessageConsumerLogger:
     def __init__(self, logger: Optional[Logger] = NotImplementedLogger()) -> None:
         self.logger = logger
 
     def _get_base_message(self, handler: Callable[..., Any]) -> LogMessage:
-        return LogMessage(
-            layer="rabbitmq_message_consumer", operation=f"{handler.__name__}"
-        )
+        return LogMessage(layer="rabbitmq_message_consumer", operation=f"{handler.__name__}")
 
     def _get_event_handler_name(self, handler: Callable[..., Any]) -> str:
         handler_name = getattr(handler, "__name__", repr(handler))
-        handler_module = getattr(handler, "__module__") + "."
+        handler_module = handler.__module__ + "."
         return f"{handler_module}{handler_name}"
 
     def log_nack_simulation(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from pika.spec import Basic
 
 
 class RabbitMqEventConsumerPrinter:
     def __init__(self, verbose: bool = False):
         self.verbose = verbose
 
-    def print_received_message(
-        self, method: Basic.Deliver, properties: BasicProperties, body: bytes
-    ) -> None:
+    def print_received_message(self, method: Basic.Deliver, properties: BasicProperties, body: bytes) -> None:
         if self.verbose:
             print(
                 "\n#####################################################################################################################"
             )
             print(f" [x] Received {body!r}")
             print(f" [x] Properties {properties!r}")
             print(f" [x] method {method!r}")
@@ -25,21 +23,19 @@
             print(
                 "#####################################################################################################################\n"
             )
 
     def print_context(self, handler: Callable[..., Any], result: AnyResult) -> None:
         if self.verbose:
             handler_name = getattr(handler, "__name__", repr(handler))
-            handler_module = getattr(handler, "__module__") + "."
+            handler_module = handler.__module__ + "."
 
             print(f" [x] event_handler: {handler_module}{handler_name}")
             print(f" [x] result from event_handler: {result}")
 
     def print_action(self, action_name: str) -> None:
         if self.verbose:
             print(f" [>] {action_name}")
 
-    def print_send_message_to(
-        self, exchange_name: str, routing_key: str, headers: Dict[str, Any]
-    ) -> None:
+    def print_send_message_to(self, exchange_name: str, routing_key: str, headers: Dict[str, Any]) -> None:
         if self.verbose:
             print(f" [>] send: [{exchange_name} |{routing_key}] -> {headers}")
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import os
 import threading
 import traceback
 from dataclasses import dataclass
 from time import sleep
 from typing import Any, Callable, Dict, List, NoReturn, Optional, Tuple, Type, Union
 
@@ -55,20 +56,16 @@
     RabbitMqMessageSubscriberQueueNameFormatter,
 )
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 from petisco.extra.rabbitmq.shared.rabbitmq_exchange_name_formatter import (
     RabbitMqExchangeNameFormatter,
 )
 
-MAX_ATTEMPTS_TO_RECONNECT = int(
-    os.getenv("PETISCO_RABBITMQ_MAX_ATTEMPTS_TO_RECONNECT_CONSUMER", "30")
-)
-WAIT_SECONDS_TO_RECONNECT = int(
-    os.getenv("PETISCO_RABBITMQ_WAIT_SECONDS_TO_RECONNECT_CONSUMER", "10")
-)
+MAX_ATTEMPTS_TO_RECONNECT = int(os.getenv("PETISCO_RABBITMQ_MAX_ATTEMPTS_TO_RECONNECT_CONSUMER", "30"))
+WAIT_SECONDS_TO_RECONNECT = int(os.getenv("PETISCO_RABBITMQ_WAIT_SECONDS_TO_RECONNECT_CONSUMER", "10"))
 
 
 @dataclass
 class SubscriberItem:
     queue_name: str
     subscriber: MessageSubscriber
     consumer_tag: str
@@ -141,45 +138,36 @@
 
     def _re_connect(self, attempt: int):
         if attempt >= MAX_ATTEMPTS_TO_RECONNECT:
             raise ConnectionError(
                 f"Impossible to reconnect consumer '{self.rabbitmq_key}' after {attempt} attempts"
             )
 
-        logger.info(
-            f"Trying to reconnect consumer '{self.rabbitmq_key}' (attempt {attempt})"
-        )
+        logger.info(f"Trying to reconnect consumer '{self.rabbitmq_key}' (attempt {attempt})")
 
         try:
             self._channel = self.connector.get_channel(self.rabbitmq_key)
         except ConnectionError:
             sleep(WAIT_SECONDS_TO_RECONNECT)
             attempt += 1
             self._re_connect(attempt=attempt)
         else:
-            subscribers = [
-                item.subscriber.__class__ for item in self.subscribers.values()
-            ]
+            subscribers = [item.subscriber.__class__ for item in self.subscribers.values()]
             self.add_subscribers(subscribers)
             self.start()
-            logger.info(
-                f"Consumer '{self.rabbitmq_key}' reconnected after {attempt} attempts"
-            )
+            logger.info(f"Consumer '{self.rabbitmq_key}' reconnected after {attempt} attempts")
 
     def notify_lost_connection_exception(self, exception: Exception) -> None:
         notifier = Container.get(Notifier)
         error = UnknownError.from_exception(
             exception=exception,
             arguments={
                 "exchange": self.exchange_name,
                 "service": self.service,
-                "subscribers": {
-                    queue: str(item.subscriber)
-                    for queue, item in self.subscribers.items()
-                },
+                "subscribers": {queue: str(item.subscriber) for queue, item in self.subscribers.items()},
             },
         )
         notifier_exception_message = NotifierExceptionMessage.from_unknown_error(
             error, title="Lost connection exception in RabbitMQ consumer"
         )
         notifier.publish_exception(notifier_exception_message)
 
@@ -202,17 +190,15 @@
                     )
                     self._add_subscriber_instance_on_queue(
                         queue_name=f"{queue_name}.{subscriber.get_subscriber_name()}",
                         subscriber=subscriber,
                         message_type_expected=subscriber_info.message_type,
                     )
 
-    def add_subscriber_on_dead_letter(
-        self, subscriber: Type[MessageSubscriber]
-    ) -> None:
+    def add_subscriber_on_dead_letter(self, subscriber: Type[MessageSubscriber]) -> None:
         """
         Add defined subscribers to be connected with the correspondent dead letter.
         """
         instance_subscriber: MessageSubscriber = subscriber()
         for subscriber_info in instance_subscriber.get_message_subscribers_info():
             queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
                 subscriber_info, exchange_name=self.exchange_name
@@ -228,21 +214,17 @@
         queue_name: str,
         subscriber: MessageSubscriber,
         is_store: bool = False,
         message_type_expected: str = "message",
     ) -> None:
         consumer_tag = self._channel.basic_consume(
             queue=queue_name,
-            on_message_callback=self.consumer(
-                subscriber, is_store, message_type_expected
-            ),
-        )
-        self.subscribers[queue_name] = SubscriberItem(
-            queue_name, subscriber, consumer_tag, is_store
+            on_message_callback=self.consumer(subscriber, is_store, message_type_expected),
         )
+        self.subscribers[queue_name] = SubscriberItem(queue_name, subscriber, consumer_tag, is_store)
 
     def add_subscriber_on_queue(
         self,
         queue_name: str,
         subscriber: Type[MessageSubscriber],
         is_store: bool = False,
         message_type_expected: str = "message",
@@ -254,31 +236,23 @@
         self._add_subscriber_instance_on_queue(
             queue_name=queue_name,
             subscriber=subscriber_instance,
             is_store=is_store,
             message_type_expected=message_type_expected,
         )
 
-    def _configure_inner_buses(
-        self, ch: BlockingChannel
-    ) -> Tuple[DomainEventBus, CommandBus]:
+    def _configure_inner_buses(self, ch: BlockingChannel) -> Tuple[DomainEventBus, CommandBus]:
         connector = RabbitMqConsumerConnector(ch)
         bus_organization = (
-            self.organization
-            if self.inner_bus_organization is None
-            else self.inner_bus_organization
-        )
-        bus_service = (
-            self.service if self.inner_bus_service is None else self.inner_bus_service
+            self.organization if self.inner_bus_organization is None else self.inner_bus_organization
         )
+        bus_service = self.service if self.inner_bus_service is None else self.inner_bus_service
 
         if self.domain_event_bus_builder is None:
-            domain_event_bus = RabbitMqDomainEventBus(
-                bus_organization, bus_service, connector
-            )
+            domain_event_bus = RabbitMqDomainEventBus(bus_organization, bus_service, connector)
             logger.warning(
                 "RabbitMqMessageConsumer: using an inner DomainEventBus with hardcoded implementation (RabbitMqDomainEventBus)\n"
             )
         else:
             domain_event_bus = self.domain_event_bus_builder()
             domain_event_bus.connector = connector
 
@@ -304,17 +278,15 @@
             method: Basic.Deliver,
             properties: BasicProperties,
             body: bytes,
         ) -> None:
             self.printer.print_received_message(method, properties, body)
 
             if self.chaos.nack_simulation(ch, method):
-                self.consumer_logger.log_nack_simulation(
-                    method, properties, body, subscriber.handle
-                )
+                self.consumer_logger.log_nack_simulation(method, properties, body, subscriber.handle)
                 return
             else:
                 self.consumer_logger.log(
                     method,
                     properties,
                     body,
                     subscriber.handle,
@@ -324,26 +296,22 @@
                 if message_type_expected == "domain_event":
                     message = DomainEvent.from_format(body)
                 elif message_type_expected == "command":
                     message = Command.from_format(body)
                 else:
                     message = Message.from_format(body)
             except Exception as e:
-                self.consumer_logger.log_parser_error(
-                    method, properties, body, subscriber.handle, e
-                )
+                self.consumer_logger.log_parser_error(method, properties, body, subscriber.handle, e)
                 ch.basic_nack(delivery_tag=method.delivery_tag)
                 return
 
             self.chaos.delay()
 
             if self.chaos.failure_simulation(method):
-                self.consumer_logger.log_failure_simulation(
-                    method, properties, body, subscriber.handle
-                )
+                self.consumer_logger.log_failure_simulation(method, properties, body, subscriber.handle)
                 result = Failure(MessageChaosError())
             else:
                 domain_event_bus, command_bus = self._configure_inner_buses(ch)
 
                 subscriber.set_domain_event_bus(domain_event_bus)
                 subscriber.set_command_bus(command_bus)
                 result = subscriber.handle(message)
@@ -353,20 +321,16 @@
             if result is None:
                 raise MessageHandlerReturnsNoneError(subscriber.handle)
 
             derived_action = ConsumerDerivedAction()
 
             if result.is_failure:
                 if not properties.headers:
-                    properties.headers = {
-                        "queue": f"{method.routing_key}.{subscriber.get_subscriber_name()}"
-                    }
-                derived_action = self.handle_consumption_error(
-                    ch, method, properties, body, is_store
-                )
+                    properties.headers = {"queue": f"{method.routing_key}.{subscriber.get_subscriber_name()}"}
+                derived_action = self.handle_consumption_error(ch, method, properties, body, is_store)
             else:
                 ch.basic_ack(delivery_tag=method.delivery_tag)
 
             self.consumer_logger.log(
                 method,
                 properties,
                 body,
@@ -432,17 +396,15 @@
         if is_store:
             routing_key = "store"
             exchange_name = self._fallback_store_exchange_name
 
         assert isinstance(routing_key, str)
         routing_key = self._get_routing_key(routing_key, "retry.")
 
-        updated_headers = self.send_message_to(
-            exchange_name, ch, routing_key, properties, body
-        )
+        updated_headers = self.send_message_to(exchange_name, ch, routing_key, properties, body)
         return ConsumerDerivedAction(
             action="send_to_retry",
             exchange_name=exchange_name,
             routing_key=routing_key,
             headers=updated_headers,
         )
 
@@ -453,17 +415,15 @@
         properties: BasicProperties,
         body: bytes,
     ) -> ConsumerDerivedAction:
         self.printer.print_action("send_to_dead_letter")
         exchange_name = RabbitMqExchangeNameFormatter.dead_letter(self.exchange_name)
         assert isinstance(method.routing_key, str)
         routing_key = self._get_routing_key(method.routing_key, "dead_letter.")
-        updated_headers = self.send_message_to(
-            exchange_name, ch, routing_key, properties, body
-        )
+        updated_headers = self.send_message_to(exchange_name, ch, routing_key, properties, body)
         return ConsumerDerivedAction(
             action="send_to_dead_letter",
             exchange_name=exchange_name,
             routing_key=routing_key,
             headers=updated_headers,
         )
 
@@ -477,17 +437,15 @@
     ) -> Dict[str, Any]:
         if properties.headers:
             redelivery_count = properties.headers.get("redelivery_count", 0)
             properties.headers["redelivery_count"] = redelivery_count + 1
         else:
             properties.headers = {"redelivery_count": 1}
 
-        self.printer.print_send_message_to(
-            exchange_name, routing_key, dict(properties.headers)
-        )
+        self.printer.print_send_message_to(exchange_name, routing_key, dict(properties.headers))
 
         ch.basic_publish(
             exchange=exchange_name,
             routing_key=routing_key,
             body=body,
             properties=properties,
         )
@@ -496,15 +454,17 @@
 
     def stop(self) -> None:
         """
         Stop the process of consuming messages from RabbitMQ.
         """
 
         def _log_stop_exception(e: Exception) -> None:
-            message = f"Error stopping RabbitMQMessageConsumer: {repr(e.__class__)} {e} | {traceback.format_exc()}"
+            message = (
+                f"Error stopping RabbitMQMessageConsumer: {repr(e.__class__)} {e} | {traceback.format_exc()}"
+            )
             logger.error(message)
 
         if self._thread and self._thread.is_alive():
             self._unsubscribe_all()
             try:
                 self._thread.join()
                 self._thread = None
@@ -518,17 +478,15 @@
                 self._channel.cancel()
             except ValueError:
                 pass
 
         def _await_for_stop_consuming_consumer_channel() -> None:
             sleep(2.0)
 
-        self.connector.get_connection(self.rabbitmq_key).call_later(
-            0, _stop_consuming_consumer_channel
-        )
+        self.connector.get_connection(self.rabbitmq_key).call_later(0, _stop_consuming_consumer_channel)
 
         _await_for_stop_consuming_consumer_channel()
 
     def unsubscribe_subscriber_on_queue(self, queue_name: str) -> None:
         subscriber_item = self.subscribers.get(queue_name)
         if subscriber_item is None:
             raise IndexError(
@@ -548,27 +506,23 @@
                 f"Cannot resume an nonexistent queue ({queue_name}). Please, check configured consumers ({list(self.subscribers.keys())})"
             )
 
         def _resume_handler_on_queue() -> None:
             assert isinstance(subscriber_item, SubscriberItem)
             subscriber_item.consumer_tag = self._channel.basic_consume(
                 queue=subscriber_item.queue_name,
-                on_message_callback=self.consumer(
-                    subscriber_item.subscriber, subscriber_item.is_store
-                ),
+                on_message_callback=self.consumer(subscriber_item.subscriber, subscriber_item.is_store),
             )
 
         self._do_it_in_consumer_thread(_resume_handler_on_queue)
 
     def _do_it_in_consumer_thread(self, action: Callable[..., None]) -> None:
         def _execute_action() -> None:
-            try:
+            with contextlib.suppress(ValueError):
                 action()
-            except ValueError:
-                pass
 
         def _await_for_thread() -> None:
             sleep(2.0)
 
         self.connector.get_connection(self.rabbitmq_key).call_later(0, _execute_action)
 
         _await_for_thread()
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from petisco.base.domain.message.message import Message
 
 
 class RabbitMqMessageQueueNameFormatter:
     @staticmethod
     def format(message: Message, exchange_name: str = None) -> str:
         message_name = message.get_message_name().replace(".", "_")
-        message_type = (
-            message.get_message_type()
-            if message.get_message_type() != "domain_event"
-            else "event"
-        )
-        message_format = (
-            f"{message.get_message_version()}.{message_type}.{message_name}"
-        )
+        message_type = message.get_message_type() if message.get_message_type() != "domain_event" else "event"
+        message_format = f"{message.get_message_version()}.{message_type}.{message_name}"
         return f"{exchange_name}.{message_format}" if exchange_name else message_name
 
     @staticmethod
     def format_retry(message: Message, exchange_name: str = None) -> str:
         queue_name = RabbitMqMessageQueueNameFormatter.format(message, exchange_name)
         return f"retry.{queue_name}"
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,24 @@
 import re
 
 from petisco.base.domain.message.message_subscriber_info import MessageSubscriberInfo
 
 
 class RabbitMqMessageSubscriberQueueNameFormatter:
     @staticmethod
-    def format(
-        subscriber_info: MessageSubscriberInfo, exchange_name: str = None
-    ) -> str:
-        message_name = (
-            re.sub(r"(?<!^)(?=[A-Z])", "_", subscriber_info.message_name)
-            .lower()
-            .replace(".", "_")
-        )
+    def format(subscriber_info: MessageSubscriberInfo, exchange_name: str = None) -> str:
+        message_name = re.sub(r"(?<!^)(?=[A-Z])", "_", subscriber_info.message_name).lower().replace(".", "_")
         message_type = (
-            subscriber_info.message_type
-            if subscriber_info.message_type != "domain_event"
-            else "event"
-        )
-        message_format = (
-            f"{subscriber_info.message_version}.{message_type}.{message_name}"
+            subscriber_info.message_type if subscriber_info.message_type != "domain_event" else "event"
         )
+        message_format = f"{subscriber_info.message_version}.{message_type}.{message_name}"
         return f"{exchange_name}.{message_format}" if exchange_name else message_format
 
     @staticmethod
-    def format_retry(
-        subscriber_info: MessageSubscriberInfo, exchange_name: str = None
-    ) -> str:
-        queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
-            subscriber_info, exchange_name
-        )
+    def format_retry(subscriber_info: MessageSubscriberInfo, exchange_name: str = None) -> str:
+        queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(subscriber_info, exchange_name)
         return f"retry.{queue_name}"
 
     @staticmethod
-    def format_dead_letter(
-        subscriber_info: MessageSubscriberInfo, exchange_name: str = None
-    ) -> str:
-        queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
-            subscriber_info, exchange_name
-        )
+    def format_dead_letter(subscriber_info: MessageSubscriberInfo, exchange_name: str = None) -> str:
+        queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(subscriber_info, exchange_name)
         return f"dead_letter.{queue_name}"
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.1.4/petisco/extra/rabbitmq/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,28 +65,24 @@
     )
 
     return [
         Dependency(
             DomainEventBus,
             alias=alias,
             builders={
-                "default": Builder(
-                    RabbitMqDomainEventBus, organization=organization, service=service
-                ),
+                "default": Builder(RabbitMqDomainEventBus, organization=organization, service=service),
                 "not_implemented": Builder(NotImplementedDomainEventBus),
             },
             envar_modifier="PETISCO_DOMAIN_EVENT_BUS_TYPE",
         ),
         Dependency(
             CommandBus,
             alias=alias,
             builders={
-                "default": Builder(
-                    RabbitMqCommandBus, organization=organization, service=service
-                ),
+                "default": Builder(RabbitMqCommandBus, organization=organization, service=service),
                 "not_implemented": Builder(NotImplementedCommandBus),
             },
             envar_modifier="PETISCO_COMMAND_BUS_TYPE",
         ),
         Dependency(
             MessageConfigurer,
             alias=alias,
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/rabbitmq_configurer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/rabbitmq_configurer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,20 @@
 )
 
 MAX_RETRIES = 5
 
 CLEAR_SUBSCRIBER_BEFORE: bool = os.getenv(
     "PETISCO_RABBITMQ_CONFIGURER_CLEAR_SUBSCRIBER_BEFORE", "false"
 ).lower() in ["true", "1", "yes", "on"]
-CLEAR_STORE_BEFORE: bool = os.getenv(
-    "PETISCO_RABBITMQ_CONFIGURER_CLEAR_STORE_BEFORE", "false"
-).lower() in ["true", "1", "yes", "on"]
+CLEAR_STORE_BEFORE: bool = os.getenv("PETISCO_RABBITMQ_CONFIGURER_CLEAR_STORE_BEFORE", "false").lower() in [
+    "true",
+    "1",
+    "yes",
+    "on",
+]
 
 
 class RabbitMqConfigurer(ApplicationConfigurer):
     def __init__(
         self,
         subscribers: list[type[MessageSubscriber]],
         execute_after_dependencies: bool = True,
@@ -43,36 +46,38 @@
         clear_store_before: bool | None = None,
         use_container_buses: bool = True,
     ):
         """
         Initializes an instance of RabbitMqConfigurer.
 
         Args:
-            subscribers (list[MessageSubscriber]): A list of MessageSubscriber objects representing the message subscribers.
-            execute_after_dependencies (bool, optional): Flag indicating whether to execute after dependencies. Defaults to True.
-            start_consuming (bool, optional): Flag indicating whether to start consuming messages. Defaults to True.
-            alias (str, optional): Alias for the MessageConfigurer and MessageConsumer (Container.get(MessageConfigurer|MessageConsumer, alias=self.alias)). Defaults to None.
-            inner_bus_organization (str, optional): configured organization for inner buses (DomainEventBus and CommandBus). If None will configure consumer organization.
-            inner_bus_service (str, optional): configured service for inner buses (DomainEventBus and CommandBus). If None will configure consumer service.
+            subscribers (list[MessageSubscriber]): A list of MessageSubscriber objects representing
+                the message subscribers.
+            execute_after_dependencies (bool, optional): Flag indicating whether to execute after
+                dependencies. Defaults to True.
+            start_consuming (bool, optional): Flag indicating whether to start consuming messages.
+                Defaults to True.
+            alias (str, optional): Alias for the MessageConfigurer and MessageConsumer
+                (Container.get(MessageConfigurer|MessageConsumer, alias=self.alias)). Defaults to None.
+            inner_bus_organization (str, optional): configured organization for inner buses (DomainEventBus
+                and CommandBus). If None will configure consumer organization.
+            inner_bus_service (str, optional): configured service for inner buses (DomainEventBus
+                and CommandBus). If None will configure consumer service.
             use_container_buses (bool, optional): configure buses from petisco.Container.
         """
         self.subscribers = subscribers
         self.start_consuming = start_consuming
         self.alias = alias
         self.inner_bus_organization = inner_bus_organization
         self.inner_bus_service = inner_bus_service
         self.consumer: MessageConsumer | None = None
         self.clear_subscriber_before = (
-            clear_subscriber_before
-            if clear_subscriber_before
-            else CLEAR_SUBSCRIBER_BEFORE
-        )
-        self.clear_store_before = (
-            clear_store_before if clear_store_before else CLEAR_STORE_BEFORE
+            clear_subscriber_before if clear_subscriber_before else CLEAR_SUBSCRIBER_BEFORE
         )
+        self.clear_store_before = clear_store_before if clear_store_before else CLEAR_STORE_BEFORE
         self.use_container_buses = use_container_buses
 
         super().__init__(execute_after_dependencies)
 
     def execute(self, testing: bool = False) -> None:
         configurer = Container.get(MessageConfigurer, alias=self.alias)
         try:
@@ -82,36 +87,30 @@
                 clear_store_before=self.clear_store_before,
             )
 
             if self.start_consuming:
                 self.consumer = Container.get(MessageConsumer, alias=self.alias)
 
                 if isinstance(self.consumer, RabbitMqMessageConsumer):
-                    self.consumer.set_inner_bus_config(
-                        self.inner_bus_organization, self.inner_bus_service
-                    )
+                    self.consumer.set_inner_bus_config(self.inner_bus_organization, self.inner_bus_service)
                     if self.use_container_buses is True:
 
                         def domain_event_bus_builder() -> DomainEventBus:
                             return Container.get(DomainEventBus)
 
                         def command_bus_builder() -> CommandBus:
                             return Container.get(CommandBus)
 
-                        self.consumer.domain_event_bus_builder = (
-                            domain_event_bus_builder
-                        )
+                        self.consumer.domain_event_bus_builder = domain_event_bus_builder
                         self.consumer.command_bus_builder = command_bus_builder
 
                 self.consumer.add_subscribers(self.subscribers)
                 self.consumer.start()
         except ConnectionError as ex:
-            logger.error(
-                f"Connection error with rabbit when trying to configure it. Message {str(ex)}"
-            )
+            logger.error(f"Connection error with rabbit when trying to configure it. Message {str(ex)}")
             self.notify_connection_error(ex)
 
     def stop(self) -> None:
         if self.consumer:
             self.consumer.stop()
 
     def notify_connection_error(self, exception: Exception) -> None:
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.1.4/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,15 @@
         return QueueConfig(
             default_retry_ttl=default_retry_ttl,
             default_main_ttl=default_main_ttl,
             specific_queue_configs=specific_queue_configs,
         )
 
     @staticmethod
-    def default(
-        default_retry_ttl: int = 5000, default_main_ttl: int = 5000
-    ) -> "QueueConfig":
+    def default(default_retry_ttl: int = 5000, default_main_ttl: int = 5000) -> "QueueConfig":
         return QueueConfig(
             default_retry_ttl=default_retry_ttl,
             default_main_ttl=default_main_ttl,
             specific_queue_configs={},
         )
 
     def __init__(
@@ -39,18 +37,15 @@
         specific_queue_configs: Dict[str, SpecificQueueConfig],
     ) -> None:
         self.default_retry_ttl = default_retry_ttl
         self.default_main_ttl = default_main_ttl
         self.specific_queue_configs = specific_queue_configs
 
     def info(self) -> Dict[str, Any]:
-        return {
-            name: specific_config.info()
-            for name, specific_config in self.specific_queue_configs.items()
-        }
+        return {name: specific_config.info() for name, specific_config in self.specific_queue_configs.items()}
 
     def get_retry_ttl(self, queue_name: str) -> Union[int, None]:
         for queue_config in self.specific_queue_configs.values():
             if queue_config.has_specific_config(queue_name):
                 return queue_config.get_retry_ttl()
         return self.default_retry_ttl
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,22 +17,18 @@
 
     def __init__(self) -> None:
         self.heartbeat = int(os.environ.get("RABBITMQ_HEARTBEAT", 60))
         self.user = os.environ.get("RABBITMQ_USER", "guest")
         self.password = os.environ.get("RABBITMQ_PASSWORD", "guest")
         self.host = os.environ.get("RABBITMQ_HOST", "localhost")
         self.port = os.environ.get("RABBITMQ_PORT", "5672")
-        self.num_max_retries_connection = int(
-            os.environ.get("RABBITMQ_CONNECTION_NUM_MAX_RETRIES", 15)
-        )
-        self.wait_seconds_retry = float(
-            os.environ.get("RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY", 1)
-        )
+        self.num_max_retries_connection = int(os.environ.get("RABBITMQ_CONNECTION_NUM_MAX_RETRIES", 15))
+        self.wait_seconds_retry = float(os.environ.get("RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY", 1))
         self.prefetch_count = int(os.environ.get("RABBITMQ_PREFETCH_COUNT", 1))
-        self.open_connections: Dict[str, BlockingConnection] = dict()
+        self.open_connections: Dict[str, BlockingConnection] = {}
 
     @staticmethod
     def ping() -> None:
         connector = RabbitMqConnector()
         connector.get_connection(key_connection="ping")
         connector.close(key_connection="ping")
 
@@ -81,45 +77,40 @@
 
     def _create_connection(self, key_connection: str) -> BlockingConnection:
         connection = self._create_blocking_connection(key_connection)
 
         self._wait_for_open_connection(connection, key_connection)
 
         if not connection.is_open:
-            time_elapsed = round(
-                (self.wait_seconds_retry * self.num_max_retries_connection), 2
-            )
+            time_elapsed = round((self.wait_seconds_retry * self.num_max_retries_connection), 2)
             raise ConnectionError(
                 f"RabbitMQConnector: Impossible to obtain a open connection with host {self.host}. "
                 f"Retried {self.num_max_retries_connection} in ~{time_elapsed} seconds"
             )
 
         return connection
 
     def _create_blocking_connection(self, connection_name: str) -> BlockingConnection:
         try:
             connection = BlockingConnection(
                 ConnectionParameters(
                     heartbeat=self.heartbeat,
                     host=self.host,
                     port=int(self.port),
-                    credentials=PlainCredentials(
-                        username=self.user, password=self.password
-                    ),
+                    credentials=PlainCredentials(username=self.user, password=self.password),
                     client_properties={"connection_name": connection_name},
                 )
             )
-        except:  # noqa E722
+        except Exception as exc:
             raise ConnectionError(
                 f"RabbitMQConnector: Impossible to connect to host {self.host}. "
-                f"Review the following envars: [RABBITMQ_USER, RABBITMQ_PASSWORD, RABBITMQ_HOST, RABBITMQ_PORT, RABBITMQ_CONNECTION_NUM_MAX_RETRIES, RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY]"
-            )
+                "Review the following envars: [RABBITMQ_USER, RABBITMQ_PASSWORD, RABBITMQ_HOST, "
+                "RABBITMQ_PORT, RABBITMQ_CONNECTION_NUM_MAX_RETRIES, RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY]"
+            ) from exc
         return connection
 
-    def _wait_for_open_connection(
-        self, connection: BlockingConnection, key_connection: str
-    ) -> None:
-        for i in range(self.num_max_retries_connection):
+    def _wait_for_open_connection(self, connection: BlockingConnection, key_connection: str) -> None:
+        for _i in range(self.num_max_retries_connection):
             if connection.is_open:
                 self.open_connections[key_connection] = connection
                 break
             time.sleep(self.wait_seconds_retry)
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,22 @@
 
 
 class RabbitMqDeclarer:
     def __init__(self, connector: RabbitMqConnector, channel_name: str):
         self._connector = connector
         self._channel_name = channel_name
 
-    def declare_exchange(
-        self, exchange_name: str, exchange_type: str = "topic"
-    ) -> None:
+    def declare_exchange(self, exchange_name: str, exchange_type: str = "topic") -> None:
         channel = self._connector.get_channel(self._channel_name)
         try:
-            channel.exchange_declare(
-                exchange=exchange_name, exchange_type=exchange_type, durable=True
-            )
+            channel.exchange_declare(exchange=exchange_name, exchange_type=exchange_type, durable=True)
         except Exception as error:
             raise TypeError(
                 f"RabbitMQEventPublisher: Cannot create the exchange ({exchange_name})\n{error}"
-            )
+            ) from error
         channel.close()
 
     def delete_exchange(self, exchange_name: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
         channel.exchange_delete(exchange_name)
         channel.close()
 
@@ -42,28 +38,24 @@
 
         if dead_letter_routing_key:
             queue_arguments["x-dead-letter-routing-key"] = dead_letter_routing_key
 
         if message_ttl:
             queue_arguments["x-message-ttl"] = message_ttl
 
-        result = channel.queue_declare(
-            queue=queue_name, arguments=queue_arguments, durable=True
-        )
+        result = channel.queue_declare(queue=queue_name, arguments=queue_arguments, durable=True)
         channel.close()
 
         queue_name: str = result.method.queue
 
         return queue_name
 
     def bind_queue(self, exchange_name: str, queue_name: str, routing_key: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
 
-        channel.queue_bind(
-            exchange=exchange_name, queue=queue_name, routing_key=routing_key
-        )
+        channel.queue_bind(exchange=exchange_name, queue=queue_name, routing_key=routing_key)
         channel.close()
 
     def delete_queue(self, queue_name: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
         channel.queue_delete(queue_name)
         channel.close()
```

### Comparing `petisco-2.1.3/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.1.4/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class SpecificQueueConfig:
     @staticmethod
     def from_dict(
         kdict: Dict[str, Any], default_retry_ttl: int, default_main_ttl: int
     ) -> "SpecificQueueConfig":
         return SpecificQueueConfig(
-            wildcard=kdict.get("when_queue_contains", None),
+            wildcard=kdict.get("when_queue_contains"),
             specific_retry_ttl=kdict.get("use", {}).get("retry_ttl", default_retry_ttl),
             specific_main_ttl=kdict.get("use", {}).get("main_ttl", default_main_ttl),
         )
 
     def __init__(
         self,
         wildcard: str,
```

### Comparing `petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_command_bus.py` & `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_command_bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 
 class RedisCommandBus(RedisMessageBus):
     """
     An implementation of CommandBus using Redis infrastructure.
     """
 
-    def __init__(
-        self, organization: str, service: str, redis_database: Redis | RedisCluster
-    ):
+    def __init__(self, organization: str, service: str, redis_database: Redis | RedisCluster):
         super().__init__(organization, service, redis_database, "commands")
 
     def dispatch(self, command: Command | list[Command]) -> None:
         """
         Dispatch one Command
         """
         commands = self._check_input(command)
```

### Comparing `petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py` & `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 
 class RedisDomainEventBus(RedisMessageBus):
     """
     An implementation of DomainEventBus using Redis infrastructure.
     """
 
-    def __init__(
-        self, organization: str, service: str, redis_database: Redis | RedisCluster
-    ):
+    def __init__(self, organization: str, service: str, redis_database: Redis | RedisCluster):
         super().__init__(organization, service, redis_database, "events")
 
     def publish(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
         """
         Publish a DomainEvent or a list of DomainEvent
         """
         domain_events = self._check_input(domain_event)
```

### Comparing `petisco-2.1.3/petisco/extra/redis/application/message/bus/redis_message_bus.py` & `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_message_bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,19 @@
             message = message.update_meta(meta)
             updated_messages.append(message)
         try:
             data = [self._get_formatted_data(message) for message in updated_messages]
             with self.redis_database.pipeline() as pipe:
                 pipe.lpush(self.database_name, *data)
                 pipe.execute()
-        except (TimeoutError, ConnectionError, RedisError) as ex:
+        except (TimeoutError, ConnectionError, RedisError) as exc:
             logger.opt(exception=True).error(
                 f"Error publishing events ({len(messages)} of type {messages[0].get_message_type()}). Exception traceback:"
             )
-            raise BusCannotPublish(additional_info={"error message": str(ex)})
+            raise BusCannotPublish(additional_info={"error message": str(exc)}) from exc
 
     def _get_formatted_data(self, message: Message):
         formatted_data = {
             "organization": self.organization,
             "service": self.service,
             "message": message.format(),
         }
```

### Comparing `petisco-2.1.3/petisco/extra/slack/__init__.py` & `petisco-2.1.4/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.1.4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
             "text": {
                 "type": "plain_text",
                 "text": title,
                 "emoji": True,
             },
         }
 
-    def _create_message_block(
-        self, notifier_message: NotifierMessage
-    ) -> Dict[str, Any]:
+    def _create_message_block(self, notifier_message: NotifierMessage) -> Dict[str, Any]:
         text_message = ""
         if notifier_message.message:
             text_message += f"{notifier_message.message}"
 
         text_meta = create_text_meta(notifier_message.meta)
         if text_meta:
             text_message += text_meta
```

### Comparing `petisco-2.1.3/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.1.4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,34 +26,30 @@
             "text": {
                 "type": "plain_text",
                 "text": title,
                 "emoji": True,
             },
         }
 
-    def _create_message_block(
-        self, notifier_exception_message: NotifierExceptionMessage
-    ):
+    def _create_message_block(self, notifier_exception_message: NotifierExceptionMessage):
         text_meta = create_text_meta(notifier_exception_message.meta)
         message_block = None
         if text_meta:
             message_block = {
                 "type": "section",
                 "text": {
                     "type": "mrkdwn",
                     "text": text_meta,
                 },
             }
             if self.slack_accessory:
                 message_block["accessory"] = self.slack_accessory
         return message_block
 
-    def _create_executor_block(
-        self, notifier_exception_message: NotifierExceptionMessage
-    ):
+    def _create_executor_block(self, notifier_exception_message: NotifierExceptionMessage):
         executor_block = {
             "type": "section",
         }
 
         if self.repository_url:
             url_error = f"{self.repository_url}/{notifier_exception_message.filename}"
             if notifier_exception_message.lineno:
```

### Comparing `petisco-2.1.3/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
 
 class SlackNotifier(Notifier):
     def __init__(
         self,
         token: str,
         channel: str,
-        converter: Optional[
-            SlackNotifierMessageConverter
-        ] = BlocksSlackNotifierMessageConverter(),
+        converter: Optional[SlackNotifierMessageConverter] = BlocksSlackNotifierMessageConverter(),
         exception_converter: Optional[
             SlackNotifierMessageConverter
         ] = ExceptionBlocksSlackNotifierMessageConverter(),
     ):
         self.channel = channel
         self.converter = converter
         self.exception_converter = exception_converter
@@ -42,21 +40,19 @@
     def publish(self, notifier_message: NotifierMessage) -> None:
         try:
             self.client.chat_postMessage(
                 channel=self.channel,
                 blocks=self.converter.convert(notifier_message),
                 text=notifier_message.title,
             )
-        except SlackApiError as e:
-            raise SlackError(e.response["error"])
+        except SlackApiError as err:
+            raise SlackError(err.response["error"]) from err
 
-    def publish_exception(
-        self, notifier_exception_message: NotifierExceptionMessage
-    ) -> None:
+    def publish_exception(self, notifier_exception_message: NotifierExceptionMessage) -> None:
         try:
             self.client.chat_postMessage(
                 channel=self.channel,
                 blocks=self.exception_converter.convert(notifier_exception_message),
                 text=notifier_exception_message.title,
             )
         except SlackApiError as e:
-            raise SlackError(e.response["error"])
+            raise SlackError(e.response["error"]) from e
```

### Comparing `petisco-2.1.3/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,12 @@
 )
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.base.misc.interface import Interface
 
 
 class SlackNotifierMessageConverter(Interface):
     @abstractmethod
-    def convert(
-        self, notifier_message: Union[NotifierMessage, NotifierExceptionMessage]
-    ) -> List[Dict]:
+    def convert(self, notifier_message: Union[NotifierMessage, NotifierExceptionMessage]) -> List[Dict]:
         """
         Should return a list of blocks. See: https://api.slack.com/reference/block-kit/blocks
         """
         raise NotImplementedError
```

### Comparing `petisco-2.1.3/petisco/extra/slack/dependencies.py` & `petisco-2.1.4/petisco/extra/slack/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/async_sql_database.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,29 +38,27 @@
                 await self._async_run_initial_statements(conn)
 
         self.async_session_factory = async_sessionmaker(bind=engine)
 
     async def _async_run_initial_statements(self, conn) -> None:
         if self.initial_statements_filename:
             try:
-                file = open(self.initial_statements_filename)
-                statements = re.split(r";\s*$", file.read(), flags=re.MULTILINE)
+                with open(self.initial_statements_filename) as file:
+                    statements = re.split(r";\s*$", file.read(), flags=re.MULTILINE)
                 for statement in statements:
                     if statement:
                         await conn.execute(text(statement))
             except Exception as exc:  # noqa
                 raise RuntimeError(
                     f"Error loading the initial_statements_filename={self.initial_statements_filename}. {str(exc)}"
-                )
+                ) from exc
 
     def get_session_scope(self) -> Callable[..., AsyncContextManager[AsyncSession]]:
         if self.async_session_factory is None:
-            raise RuntimeError(
-                "AsyncSqlDatabase must run initialize() before get_session_scope()"
-            )
+            raise RuntimeError("AsyncSqlDatabase must run initialize() before get_session_scope()")
 
         if self.use_scoped_session:
             Session = scoped_session(self.async_session_factory)  # noqa
         else:
             Session = self.async_session_factory  # noqa
         return async_sql_session_scope_provider(Session)
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from loguru import logger
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.ext.asyncio import AsyncSession
 
 
 def async_sql_session_scope_provider(
-    async_session_factory: Callable[[], AsyncSession]
+    async_session_factory: Callable[[], AsyncSession],
 ) -> Callable[..., AsyncContextManager[AsyncSession]]:
     @asynccontextmanager
     async def session_scope() -> AsyncContextManager[AsyncSession]:
         session = async_session_factory()
         try:
             yield session
             await session.commit()
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,26 +30,20 @@
         driver: str = "pymysql",
         user: str = "root",
         password: str = "root",
         host: str = "mysql",
         port: str = "3306",
         database_name: str = MYSQL_DATABASE_DEFAULT,
     ) -> "MySqlConnection":
-        url = (
-            f"{server_name}+{driver}://{user}:{password}@{host}:{port}/{database_name}"
-        )
-        return MySqlConnection(
-            server_name, driver, user, password, host, port, database_name, url
-        )
+        url = f"{server_name}+{driver}://{user}:{password}@{host}:{port}/{database_name}"
+        return MySqlConnection(server_name, driver, user, password, host, port, database_name, url)
 
     @staticmethod
     def create_local(database_name: str = MYSQL_DATABASE_DEFAULT) -> "MySqlConnection":
-        return MySqlConnection.create(
-            host="localhost", port="3307", database_name=database_name
-        )
+        return MySqlConnection.create(host="localhost", port="3307", database_name=database_name)
 
     @staticmethod
     def from_environ() -> "MySqlConnection":
         return MySqlConnection.create(
             "mysql",
             "pymysql",
             os.getenv("MYSQL_USER", "root"),
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_base.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 T = TypeVar("T")
 
 
 class SqlBase(DeclarativeBase, Generic[T]):
     def __repr__(self):
         attributes = ", ".join(
-            f"{key}={value}"
-            for key, value in self.__dict__.items()
-            if not key.startswith("_")
+            f"{key}={value}" for key, value in self.__dict__.items() if not key.startswith("_")
         )
         return f"{self.__class__.__name__}({attributes})"
 
     def info(self) -> dict[str, str]:
         return {
             "name": self.__class__.__name__,
             "module": self.__class__.__module__,
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_database.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_database.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,20 +42,16 @@
         self.before_initial_statements = before_initial_statements
         self.initial_statements_filename = initial_statements_filename
         self.after_initial_statements = after_initial_statements
         self._check_connection()
         super().__init__(alias)
 
     def _check_connection(self) -> None:
-        if not self.connection or not isinstance(
-            self.connection, (SqliteConnection, MySqlConnection)
-        ):
-            raise ConnectionError(
-                "SqlDatabase needs a valid SqliteConnection or MySqlConnection connection"
-            )
+        if not self.connection or not isinstance(self.connection, (SqliteConnection, MySqlConnection)):
+            raise ConnectionError("SqlDatabase needs a valid SqliteConnection or MySqlConnection connection")
 
     def initialize(self, base: type[DeclarativeBase] = SqlBase) -> None:
         engine = create_engine(
             self.connection.url,
             pool_pre_ping=True,
             json_serializer=lambda obj: obj,
             json_deserializer=lambda obj: obj,
@@ -72,56 +68,50 @@
                 self.after_initial_statements()
 
         self.session_factory = sessionmaker(bind=engine)
 
     def _run_initial_statements(self, engine) -> None:
         if self.initial_statements_filename:
             try:
-                file = open(self.initial_statements_filename)
-                statements = re.split(r";\s*$", file.read(), flags=re.MULTILINE)
+                with open(self.initial_statements_filename) as file:
+                    statements = re.split(r";\s*$", file.read(), flags=re.MULTILINE)
                 with engine.connect() as conn:
                     for statement in statements:
                         if statement:
                             conn.execute(text(statement))
                     conn.commit()
             except Exception as exc:  # noqa
                 raise RuntimeError(
                     f"Error loading the initial_statements_filename={self.initial_statements_filename}. {str(exc)}"
-                )
+                ) from exc
 
     def delete(self):
         if isinstance(self.connection, SqliteConnection):
             if os.path.exists(self.connection.database_name):
                 os.remove(self.connection.database_name)
         else:
-            logger.warning(
-                "SqlDatabase do not implement delete to mitigate possible problems in production"
-            )
+            logger.warning("SqlDatabase do not implement delete to mitigate possible problems in production")
 
     def clear_data(self, base: DeclarativeBase = SqlBase) -> None:
         if isinstance(self.connection, SqliteConnection):
             session_scope = self.get_session_scope()
             with session_scope() as session:
                 for table in reversed(base.metadata.sorted_tables):
                     session.execute(table.delete())
         else:
             logger.warning(
                 "SqlDatabase do not implement clear_data to mitigate possible problems in production"
             )
 
     def get_session_scope(self) -> Callable[..., ContextManager[Session]]:
         if self.session_factory is None:
-            raise RuntimeError(
-                "SqlDatabase must run initialize() before get_session_scope()"
-            )
+            raise RuntimeError("SqlDatabase must run initialize() before get_session_scope()")
 
         if self.use_scoped_session:
-            Session: Callable[..., Session] = scoped_session(
-                self.session_factory
-            )  # noqa
+            Session: Callable[..., Session] = scoped_session(self.session_factory)  # noqa
         else:
             Session: Callable[..., Session] = self.session_factory  # noqa
         return sql_session_scope_provider(Session)
 
     def is_available(self):
         try:
             context = self.get_session_scope()
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_repository.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,41 +32,29 @@
 
     @classmethod
     def fail_if_aggregate_already_exist(
         cls, model: Any, aggregate_id: Uuid, result_error: Error | None = None
     ) -> BoolResult:
         if model:
             error = (
-                AggregateAlreadyExistError(
-                    aggregate_id, cls.__name__, model.__tablename__
-                )
-                if not result_error
-                else result_error
+                result_error
+                if result_error
+                else AggregateAlreadyExistError(aggregate_id, cls.__name__, model.__tablename__)
             )
             return Failure(error)
         return isSuccess
 
     @classmethod
     def fail_if_aggregate_not_found(
         cls, model: Any, aggregate_id: Uuid, result_error: Error | None = None
     ) -> BoolResult:
         if not model:
-            error = (
-                AggregateNotFoundError(aggregate_id, cls.__name__)
-                if not result_error
-                else result_error
-            )
+            error = result_error if result_error else AggregateNotFoundError(aggregate_id, cls.__name__)
             return Failure(error)
         return isSuccess
 
     @classmethod
-    def fail_if_aggregates_not_found(
-        cls, model: Any, result_error: Error | None = None
-    ) -> BoolResult:
+    def fail_if_aggregates_not_found(cls, model: Any, result_error: Error | None = None) -> BoolResult:
         if not model:
-            error = (
-                AggregatesNotFoundError(cls.__name__)
-                if not result_error
-                else result_error
-            )
+            error = result_error if result_error else AggregatesNotFoundError(cls.__name__)
             return Failure(error)
         return isSuccess
```

### Comparing `petisco-2.1.3/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import Session
 
 from petisco.extra.meiga import WaitingForEarlyReturn
 
 
 def sql_session_scope_provider(
-    session_factory: Callable[[], Session]
+    session_factory: Callable[[], Session],
 ) -> Callable[[], ContextManager[Session]]:
     @contextmanager
     def session_scope() -> Iterator[Session]:
         session = session_factory()
         try:
             yield session
             session.commit()
```

### Comparing `petisco-2.1.3/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.1.4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,40 +26,32 @@
 
 engine = create_engine("sqlite:///database.db", echo=True)
 SQLModel.metadata.create_all(engine)
 
 SQLModelType = TypeVar("SQLModelType", bound=SQLModel)
 
 
-class SQLModelCrudRepository(
-    Generic[SQLModelType, AggregateRootType], CrudRepository[AggregateRootType]
-):
+class SQLModelCrudRepository(Generic[SQLModelType, AggregateRootType], CrudRepository[AggregateRootType]):
     @abstractmethod
-    def get_aggregate_root(
-        self, sql_model: SQLModel
-    ) -> Result[AggregateRootType, Error]:
+    def get_aggregate_root(self, sql_model: SQLModel) -> Result[AggregateRootType, Error]:
         return NotImplementedMethodError
 
     @abstractmethod
-    def get_sql_model(
-        self, aggregate_root: AggregateRootType
-    ) -> Result[SQLModel, Error]:
+    def get_sql_model(self, aggregate_root: AggregateRootType) -> Result[SQLModel, Error]:
         return NotImplementedMethodError
 
     @abstractmethod
     def get_sql_model_type(self) -> SQLModelType:
         return NotImplementedMethodError
 
     @meiga
     def save(self, aggregate_root: AggregateRootType) -> BoolResult:
         with Session(engine) as session:
             model = self.get_sql_model_type()
-            statement = select(model).where(
-                model.aggregate_id == aggregate_root.aggregate_id.value
-            )
+            statement = select(model).where(model.aggregate_id == aggregate_root.aggregate_id.value)
             sql_model = session.exec(statement).first()
             if sql_model:
                 return Failure(AggregateAlreadyExistError(aggregate_root.aggregate_id))
 
             sql_model = self.get_sql_model(aggregate_root).unwrap_or_return()
 
             session.add(sql_model)
@@ -77,17 +69,15 @@
                 return Failure(AggregateNotFoundError(aggregate_id))
             aggregate_root = self.get_aggregate_root(sql_model).unwrap_or_return()
             return Success(aggregate_root)
 
     def update(self, aggregate_root: AggregateRootType) -> BoolResult:
         with Session(engine) as session:
             model = self.get_sql_model_type()
-            statement = select(model).where(
-                model.aggregate_id == aggregate_root.aggregate_id.value
-            )
+            statement = select(model).where(model.aggregate_id == aggregate_root.aggregate_id.value)
             sql_model = session.exec(statement).first()
             if sql_model is None:
                 return Failure(AggregateNotFoundError(aggregate_root.aggregate_id))
 
             sql_model = self.get_sql_model(aggregate_root)
             session.add(sql_model)
             session.commit()
@@ -108,12 +98,9 @@
 
     def retrieve_all(self) -> Result[List[AggregateRootType], Error]:
         with Session(engine) as session:
             model = self.get_sql_model_type()
             statement = select(model)
             sql_models = session.exec(statement)
 
-            all = [
-                self.get_aggregate_root(sql_model).unwrap_or_return()
-                for sql_model in sql_models
-            ]
+            all = [self.get_aggregate_root(sql_model).unwrap_or_return() for sql_model in sql_models]
             return Success(all)
```

### Comparing `petisco-2.1.3/petisco/extra/threading/pool_executor.py` & `petisco-2.1.4/petisco/extra/threading/pool_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 class Executable:
     def __init__(self, func: Callable[[Any], Any], args: Tuple[Any]) -> None:
         self.func = func
         self.args = args
 
 
 class PoolExecutor:
-    def __init__(
-        self, executables: List[Executable], use_multi_threading: bool = True
-    ) -> None:
+    def __init__(self, executables: List[Executable], use_multi_threading: bool = True) -> None:
         self.executables = executables
         self.use_multi_threading = use_multi_threading
 
     def execute(self) -> List[Any]:
         if len(self.executables) < 1:
             return []
```

### Comparing `petisco-2.1.3/petisco/public_api.py` & `petisco-2.1.4/petisco/public_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Public API of Alice Petisco Framework"""
+
 from petisco.base.application.application import Application
 from petisco.base.application.application_configurer import ApplicationConfigurer
 from petisco.base.application.controller.async_controller import AsyncController
 from petisco.base.application.controller.controller import Controller
 from petisco.base.application.controller.error_map import ErrorMap
 from petisco.base.application.controller.handlers import (
     custom_message_handler,
```

### Comparing `petisco-2.1.3/petisco.egg-info/PKG-INFO` & `petisco-2.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7065 7469  : 2.1.Name: peti
 00000020: 7363 6f0a 5665 7273 696f 6e3a 2032 2e31  sco.Version: 2.1
-00000030: 2e33 0a53 756d 6d61 7279 3a20 5065 7469  .3.Summary: Peti
+00000030: 2e34 0a53 756d 6d61 7279 3a20 5065 7469  .4.Summary: Peti
 00000040: 7363 6f20 6973 2061 2066 7261 6d65 776f  sco is a framewo
 00000050: 726b 2066 6f72 2068 656c 7069 6e67 2050  rk for helping P
 00000060: 7974 686f 6e20 6465 7665 6c6f 7065 7273  ython developers
 00000070: 2074 6f20 6275 696c 6420 636c 6561 6e20   to build clean 
 00000080: 4170 706c 6963 6174 696f 6e73 0a48 6f6d  Applications.Hom
 00000090: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 000000a0: 6769 7468 7562 2e63 6f6d 2f61 6c69 6365  github.com/alice
@@ -40,159 +40,172 @@
 00000270: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
 00000280: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
 00000290: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 000002a0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
 000002b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 000002d0: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
-000002e0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
-000002f0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-00000300: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
-00000310: 2d45 7874 7261 3a20 7371 6c61 6c63 6865  -Extra: sqlalche
-00000320: 6d79 0a50 726f 7669 6465 732d 4578 7472  my.Provides-Extr
-00000330: 613a 2072 6564 6973 0a50 726f 7669 6465  a: redis.Provide
-00000340: 732d 4578 7472 613a 2072 6162 6269 746d  s-Extra: rabbitm
-00000350: 710a 5072 6f76 6964 6573 2d45 7874 7261  q.Provides-Extra
-00000360: 3a20 736c 6163 6b0a 5072 6f76 6964 6573  : slack.Provides
-00000370: 2d45 7874 7261 3a20 656c 6173 7469 630a  -Extra: elastic.
-00000380: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000390: 656c 6173 7469 632d 6170 6d0a 5072 6f76  elastic-apm.Prov
-000003a0: 6964 6573 2d45 7874 7261 3a20 6661 7374  ides-Extra: fast
-000003b0: 6170 690a 5072 6f76 6964 6573 2d45 7874  api.Provides-Ext
-000003c0: 7261 3a20 7269 6368 0a50 726f 7669 6465  ra: rich.Provide
-000003d0: 732d 4578 7472 613a 2064 6576 0a4c 6963  s-Extra: dev.Lic
-000003e0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-000003f0: 5345 0a0a 2320 7065 7469 7363 6f20 f09f  SE..# petisco ..
-00000400: 8daa 2020 0a0a 5b21 5b76 6572 7369 6f6e  ..  ..[![version
-00000410: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000420: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000430: 7265 6c65 6173 652f 616c 6963 652d 6269  release/alice-bi
-00000440: 6f6d 6574 7269 6373 2f70 6574 6973 636f  ometrics/petisco
-00000450: 2f61 6c6c 2e73 7667 295d 2868 7474 7073  /all.svg)](https
-00000460: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00000470: 6963 652d 6269 6f6d 6574 7269 6373 2f70  ice-biometrics/p
-00000480: 6574 6973 636f 2f72 656c 6561 7365 7329  etisco/releases)
-00000490: 200a 5b21 5b63 695d 2868 7474 7073 3a2f   .[![ci](https:/
-000004a0: 2f67 6974 6875 622e 636f 6d2f 616c 6963  /github.com/alic
-000004b0: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
-000004c0: 6973 636f 2f77 6f72 6b66 6c6f 7773 2f63  isco/workflows/c
-000004d0: 692f 6261 6467 652e 7376 6729 5d28 6874  i/badge.svg)](ht
-000004e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004f0: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
-00000500: 732f 7065 7469 7363 6f2f 6163 7469 6f6e  s/petisco/action
-00000510: 7329 200a 5b21 5b70 7970 695d 2868 7474  s) .[![pypi](htt
-00000520: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000530: 2e69 6f2f 7079 7069 2f64 6d2f 7065 7469  .io/pypi/dm/peti
-00000540: 7363 6f29 5d28 6874 7470 733a 2f2f 7079  sco)](https://py
-00000550: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-00000560: 6574 6973 636f 2f29 200a 5b21 5b63 6f64  etisco/) .[![cod
-00000570: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
-00000580: 6465 636f 762e 696f 2f67 682f 616c 6963  decov.io/gh/alic
-00000590: 652d 6269 6f6d 6574 7269 6373 2f70 6574  e-biometrics/pet
-000005a0: 6973 636f 2f62 7261 6e63 682f 6d61 696e  isco/branch/main
-000005b0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-000005c0: 3f74 6f6b 656e 3d59 4858 4159 4b58 3056  ?token=YHXAYKX0V
-000005d0: 4f29 5d28 6874 7470 733a 2f2f 636f 6465  O)](https://code
-000005e0: 636f 762e 696f 2f67 682f 616c 6963 652d  cov.io/gh/alice-
-000005f0: 6269 6f6d 6574 7269 6373 2f70 6574 6973  biometrics/petis
-00000600: 636f 290a 5b21 5b43 6f64 6520 7374 796c  co).[![Code styl
-00000610: 653a 2062 6c61 636b 5d28 6874 7470 733a  e: black](https:
-00000620: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000630: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000640: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000650: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000660: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00000670: 6163 6b29 0a5b 215b 496d 706f 7274 733a  ack).[![Imports:
-00000680: 2069 736f 7274 5d28 6874 7470 733a 2f2f   isort](https://
-00000690: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000006a0: 6164 6765 2f25 3230 696d 706f 7274 732d  adge/%20imports-
-000006b0: 6973 6f72 742d 2532 3331 3637 3462 313f  isort-%231674b1?
-000006c0: 7374 796c 653d 666c 6174 266c 6162 656c  style=flat&label
-000006d0: 436f 6c6f 723d 6566 3833 3336 295d 2868  Color=ef8336)](h
-000006e0: 7474 7073 3a2f 2f70 7963 7161 2e67 6974  ttps://pycqa.git
-000006f0: 6875 622e 696f 2f69 736f 7274 2f29 0a5b  hub.io/isort/).[
-00000700: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
-00000710: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000720: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000730: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
-00000740: 732f 7065 7469 7363 6f2e 7376 6729 5d28  s/petisco.svg)](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f61 6c69 6365 2d62 696f 6d65 7472  om/alice-biometr
-00000770: 6963 732f 7065 7469 7363 6f2f 626c 6f62  ics/petisco/blob
-00000780: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a5b  /main/LICENSE).[
-00000790: 215b 7665 7273 696f 6e73 5d28 6874 7470  ![versions](http
-000007a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007b0: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000007c0: 6e73 2f70 6574 6973 636f 2e73 7667 295d  ns/petisco.svg)]
-000007d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007e0: 636f 6d2f 616c 6963 652d 6269 6f6d 6574  com/alice-biomet
-000007f0: 7269 6373 2f70 6574 6973 636f 290a 0a3c  rics/petisco)..<
-00000800: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000810: 2f67 6974 6875 622e 636f 6d2f 616c 6963  /github.com/alic
-00000820: 652d 6269 6f6d 6574 7269 6373 2f63 7573  e-biometrics/cus
-00000830: 746f 6d2d 656d 6f6a 6973 2f62 6c6f 622f  tom-emojis/blob/
-00000840: 6d61 7374 6572 2f69 6d61 6765 732f 616c  master/images/al
-00000850: 6963 655f 6865 6164 6572 2e70 6e67 3f72  ice_header.png?r
-00000860: 6177 3d74 7275 6522 2077 6964 7468 3d61  aw=true" width=a
-00000870: 7574 6f3e 0a0a 2d2d 2d0a 0a2a 2a44 6f63  uto>..---..**Doc
-00000880: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c61  umentation**: <a
-00000890: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
-000008a0: 6c69 6365 2d62 696f 6d65 7472 6963 732e  lice-biometrics.
-000008b0: 6769 7468 7562 2e69 6f2f 7065 7469 7363  github.io/petisc
-000008c0: 6f2f 2220 7461 7267 6574 3d22 5f62 6c61  o/" target="_bla
-000008d0: 6e6b 223e 6874 7470 733a 2f2f 616c 6963  nk">https://alic
-000008e0: 652d 6269 6f6d 6574 7269 6373 2e67 6974  e-biometrics.git
-000008f0: 6875 622e 696f 2f70 6574 6973 636f 2f3c  hub.io/petisco/<
-00000900: 2f61 3e0a 0a2a 2a53 6f75 7263 6520 436f  /a>..**Source Co
-00000910: 6465 2a2a 3a20 3c61 2068 7265 663d 2268  de**: <a href="h
-00000920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000930: 6d2f 616c 6963 652d 6269 6f6d 6574 7269  m/alice-biometri
-00000940: 6373 2f70 6574 6973 636f 2220 7461 7267  cs/petisco" targ
-00000950: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
-00000960: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000970: 6c69 6365 2d62 696f 6d65 7472 6963 732f  lice-biometrics/
-00000980: 7065 7469 7363 6f3c 2f61 3e0a 0a2d 2d2d  petisco</a>..---
-00000990: 0a0a 2323 2057 6861 7420 6973 2070 6574  ..## What is pet
-000009a0: 6973 636f 3f20 f09f 8daa 0a0a 7065 7469  isco? ......peti
-000009b0: 7363 6f20 6973 2061 2066 7261 6d65 776f  sco is a framewo
-000009c0: 726b 2066 6f72 2068 656c 7069 6e67 2050  rk for helping P
-000009d0: 7974 686f 6e20 6465 7665 6c6f 7065 7273  ython developers
-000009e0: 2074 6f20 6275 696c 6420 636c 6561 6e20   to build clean 
-000009f0: 4170 706c 6963 6174 696f 6e73 2069 6e20  Applications in 
-00000a00: 5079 7468 6f6e 2e0a 0a23 2320 486f 7720  Python...## How 
-00000a10: 636f 756c 6420 7065 7469 7363 6f20 6865  could petisco he
-00000a20: 6c70 206d 653f 20f0 9f8d aa0a 0a70 6574  lp me? ......pet
-00000a30: 6973 636f 2070 726f 7669 6465 7320 7365  isco provides se
-00000a40: 7665 7261 6c20 6861 6e64 7920 636c 6173  veral handy clas
-00000a50: 7365 7320 746f 2068 656c 7020 796f 7520  ses to help you 
-00000a60: 6f6e 2064 6566 696e 696e 6720 796f 7572  on defining your
-00000a70: 2064 6f6d 6169 6e20 7769 7468 2068 6578   domain with hex
-00000a80: 6167 6f6e 616c 2061 7263 6869 7465 6374  agonal architect
-00000a90: 7572 652c 2065 7665 6e74 2073 7472 6561  ure, event strea
-00000aa0: 6d69 6e67 2061 6e64 2043 5152 532e 0a0a  ming and CQRS...
-00000ab0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000ac0: 20f0 9f92 bb0a 0a60 6060 636f 6e73 6f6c   ......```consol
-00000ad0: 650a 7069 7020 696e 7374 616c 6c20 7065  e.pip install pe
-00000ae0: 7469 7363 6f0a 6060 600a 0a49 6e73 7461  tisco.```..Insta
-00000af0: 6c6c 6174 696f 6e20 7769 7468 2045 7874  llation with Ext
-00000b00: 7261 7320 0a0a 6060 6063 6f6e 736f 6c65  ras ..```console
-00000b10: 0a70 6970 2069 6e73 7461 6c6c 2070 6574  .pip install pet
-00000b20: 6973 636f 5b66 6173 7461 7069 2c73 716c  isco[fastapi,sql
-00000b30: 616c 6368 656d 792c 656c 6173 7469 632c  alchemy,elastic,
-00000b40: 656c 6173 7469 632d 6170 6d2c 7261 6262  elastic-apm,rabb
-00000b50: 6974 6d71 2c73 6c61 636b 2c72 6564 6973  itmq,slack,redis
-00000b60: 5d0a 6060 600a 0a23 2320 436f 6e74 7269  ].```..## Contri
-00000b70: 6275 7465 200a 0a57 6527 6420 6c6f 7665  bute ..We'd love
-00000b80: 2079 6f75 2074 6f20 636f 6e74 7269 6275   you to contribu
-00000b90: 7465 2074 6f20 2a70 6574 6973 636f 2a20  te to *petisco* 
-00000ba0: f09f a5b3 f09f a5b3 f09f a5b3 f09f a5b3  ................
-00000bb0: f09f a5b3 f09f a5b3 efb8 8fef b88f 210a  ..............!.
-00000bc0: 0a46 6f72 206d 6f72 6520 696e 666f 726d  .For more inform
-00000bd0: 6174 696f 6e2c 2063 6865 636b 206f 7572  ation, check our
-00000be0: 205b 646f 6375 6d65 6e74 6174 696f 6e5d   [documentation]
-00000bf0: 2868 7474 7073 3a2f 2f61 6c69 6365 2d62  (https://alice-b
-00000c00: 696f 6d65 7472 6963 732e 6769 7468 7562  iometrics.github
-00000c10: 2e69 6f2f 7065 7469 7363 6f2f 636f 6e74  .io/petisco/cont
-00000c20: 7269 6275 7469 6e67 2f29 0a0a 2323 2043  ributing/)..## C
-00000c30: 6f6e 7461 6374 20f0 9f93 ac0a 0a73 7570  ontact ......sup
-00000c40: 706f 7274 4061 6c69 6365 6269 6f6d 6574  port@alicebiomet
-00000c50: 7269 6373 2e63 6f6d 0a                   rics.com.
+000002e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000002f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000300: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000310: 3132 0a44 6573 6372 6970 7469 6f6e 2d43  12.Description-C
+00000320: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000330: 742f 6d61 726b 646f 776e 0a50 726f 7669  t/markdown.Provi
+00000340: 6465 732d 4578 7472 613a 2073 716c 616c  des-Extra: sqlal
+00000350: 6368 656d 790a 5072 6f76 6964 6573 2d45  chemy.Provides-E
+00000360: 7874 7261 3a20 7265 6469 730a 5072 6f76  xtra: redis.Prov
+00000370: 6964 6573 2d45 7874 7261 3a20 7261 6262  ides-Extra: rabb
+00000380: 6974 6d71 0a50 726f 7669 6465 732d 4578  itmq.Provides-Ex
+00000390: 7472 613a 2073 6c61 636b 0a50 726f 7669  tra: slack.Provi
+000003a0: 6465 732d 4578 7472 613a 2065 6c61 7374  des-Extra: elast
+000003b0: 6963 0a50 726f 7669 6465 732d 4578 7472  ic.Provides-Extr
+000003c0: 613a 2065 6c61 7374 6963 2d61 706d 0a50  a: elastic-apm.P
+000003d0: 726f 7669 6465 732d 4578 7472 613a 2066  rovides-Extra: f
+000003e0: 6173 7461 7069 0a50 726f 7669 6465 732d  astapi.Provides-
+000003f0: 4578 7472 613a 2072 6963 680a 5072 6f76  Extra: rich.Prov
+00000400: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
+00000410: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000420: 4345 4e53 450a 0a23 2070 6574 6973 636f  CENSE..# petisco
+00000430: 20f0 9f8d aa20 200a 0a0a 0a3c 6469 7620   ....  ....<div 
+00000440: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000450: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000470: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
+00000480: 732f 6375 7374 6f6d 2d65 6d6f 6a69 732f  s/custom-emojis/
+00000490: 626c 6f62 2f6d 6173 7465 722f 696d 6167  blob/master/imag
+000004a0: 6573 2f70 6574 6973 636f 2e70 6e67 3f72  es/petisco.png?r
+000004b0: 6177 3d74 7275 6522 2073 7479 6c65 3d22  aw=true" style="
+000004c0: 7769 6474 683a 2036 3025 223e 0a0a 0a20  width: 60%">... 
+000004d0: 5b41 6c69 6365 5d20 7c20 5b47 6574 7469  [Alice] | [Getti
+000004e0: 6e67 2053 7461 7274 6564 5d20 7c20 5b44  ng Started] | [D
+000004f0: 6f63 756d 656e 7461 7469 6f6e 5d20 7c20  ocumentation] | 
+00000500: 5b53 6f75 7263 6520 436f 6465 5d20 7c20  [Source Code] | 
+00000510: 5b45 7861 6d70 6c65 735d 0a0a 205b 215b  [Examples].. [![
+00000520: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
+00000530: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000540: 6769 7468 7562 2f72 656c 6561 7365 2f61  github/release/a
+00000550: 6c69 6365 2d62 696f 6d65 7472 6963 732f  lice-biometrics/
+00000560: 7065 7469 7363 6f2f 616c 6c2e 7376 6729  petisco/all.svg)
+00000570: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000580: 2e63 6f6d 2f61 6c69 6365 2d62 696f 6d65  .com/alice-biome
+00000590: 7472 6963 732f 7065 7469 7363 6f2f 7265  trics/petisco/re
+000005a0: 6c65 6173 6573 2920 0a5b 215b 6369 5d28  leases) .[![ci](
+000005b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005c0: 6f6d 2f61 6c69 6365 2d62 696f 6d65 7472  om/alice-biometr
+000005d0: 6963 732f 7065 7469 7363 6f2f 776f 726b  ics/petisco/work
+000005e0: 666c 6f77 732f 6369 2f62 6164 6765 2e73  flows/ci/badge.s
+000005f0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000600: 6875 622e 636f 6d2f 616c 6963 652d 6269  hub.com/alice-bi
+00000610: 6f6d 6574 7269 6373 2f70 6574 6973 636f  ometrics/petisco
+00000620: 2f61 6374 696f 6e73 2920 0a5b 215b 7079  /actions) .[![py
+00000630: 7069 5d28 6874 7470 733a 2f2f 696d 672e  pi](https://img.
+00000640: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000650: 646d 2f70 6574 6973 636f 295d 2868 7474  dm/petisco)](htt
+00000660: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000670: 6f6a 6563 742f 7065 7469 7363 6f2f 2920  oject/petisco/) 
+00000680: 0a5b 215b 636f 6465 636f 765d 2868 7474  .[![codecov](htt
+00000690: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+000006a0: 6768 2f61 6c69 6365 2d62 696f 6d65 7472  gh/alice-biometr
+000006b0: 6963 732f 7065 7469 7363 6f2f 6272 616e  ics/petisco/bran
+000006c0: 6368 2f6d 6169 6e2f 6772 6170 682f 6261  ch/main/graph/ba
+000006d0: 6467 652e 7376 673f 746f 6b65 6e3d 5948  dge.svg?token=YH
+000006e0: 5841 594b 5830 564f 295d 2868 7474 7073  XAYKX0VO)](https
+000006f0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000700: 2f61 6c69 6365 2d62 696f 6d65 7472 6963  /alice-biometric
+00000710: 732f 7065 7469 7363 6f29 0a5b 215b 6c69  s/petisco).[![li
+00000720: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
+00000730: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000740: 7468 7562 2f6c 6963 656e 7365 2f61 6c69  thub/license/ali
+00000750: 6365 2d62 696f 6d65 7472 6963 732f 7065  ce-biometrics/pe
+00000760: 7469 7363 6f2e 7376 6729 5d28 6874 7470  tisco.svg)](http
+00000770: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000780: 6c69 6365 2d62 696f 6d65 7472 6963 732f  lice-biometrics/
+00000790: 7065 7469 7363 6f2f 626c 6f62 2f6d 6169  petisco/blob/mai
+000007a0: 6e2f 4c49 4345 4e53 4529 0a5b 215b 7665  n/LICENSE).[![ve
+000007b0: 7273 696f 6e73 5d28 6874 7470 733a 2f2f  rsions](https://
+000007c0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000007d0: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
+000007e0: 6574 6973 636f 2e73 7667 295d 2868 7474  etisco.svg)](htt
+000007f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000800: 616c 6963 652d 6269 6f6d 6574 7269 6373  alice-biometrics
+00000810: 2f70 6574 6973 636f 290a 5b21 5b52 7566  /petisco).[![Ruf
+00000820: 665d 2868 7474 7073 3a2f 2f69 6d67 2e73  f](https://img.s
+00000830: 6869 656c 6473 2e69 6f2f 656e 6470 6f69  hields.io/endpoi
+00000840: 6e74 3f75 726c 3d68 7474 7073 3a2f 2f72  nt?url=https://r
+00000850: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000860: 7465 6e74 2e63 6f6d 2f61 7374 7261 6c2d  tent.com/astral-
+00000870: 7368 2f72 7566 662f 6d61 696e 2f61 7373  sh/ruff/main/ass
+00000880: 6574 732f 6261 6467 652f 7632 2e6a 736f  ets/badge/v2.jso
+00000890: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
+000008a0: 7562 2e63 6f6d 2f61 7374 7261 6c2d 7368  ub.com/astral-sh
+000008b0: 2f72 7566 6629 0a5b 215b 5079 6461 6e74  /ruff).[![Pydant
+000008c0: 6963 2076 325d 2868 7474 7073 3a2f 2f69  ic v2](https://i
+000008d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 656e  mg.shields.io/en
+000008e0: 6470 6f69 6e74 3f75 726c 3d68 7474 7073  dpoint?url=https
+000008f0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000900: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 7964  rcontent.com/pyd
+00000910: 616e 7469 632f 7079 6461 6e74 6963 2f6d  antic/pydantic/m
+00000920: 6169 6e2f 646f 6373 2f62 6164 6765 2f76  ain/docs/badge/v
+00000930: 322e 6a73 6f6e 295d 2868 7474 7073 3a2f  2.json)](https:/
+00000940: 2f64 6f63 732e 7079 6461 6e74 6963 2e64  /docs.pydantic.d
+00000950: 6576 2f6c 6174 6573 742f 636f 6e74 7269  ev/latest/contri
+00000960: 6275 7469 6e67 2f23 6261 6467 6573 290a  buting/#badges).
+00000970: 0a3c 2f64 6976 3e0a 0a5b 416c 6963 655d  .</div>..[Alice]
+00000980: 3a20 6874 7470 733a 2f2f 616c 6963 6562  : https://aliceb
+00000990: 696f 6d65 7472 6963 732e 636f 6d2f 0a5b  iometrics.com/.[
+000009a0: 4765 7474 696e 6720 5374 6172 7465 645d  Getting Started]
+000009b0: 3a20 6874 7470 733a 2f2f 616c 6963 652d  : https://alice-
+000009c0: 6269 6f6d 6574 7269 6373 2e67 6974 6875  biometrics.githu
+000009d0: 622e 696f 2f70 6574 6973 636f 2f67 6574  b.io/petisco/get
+000009e0: 7469 6e67 5f73 7461 7274 6564 2f0a 5b44  ting_started/.[D
+000009f0: 6f63 756d 656e 7461 7469 6f6e 5d3a 2068  ocumentation]: h
+00000a00: 7474 7073 3a2f 2f61 6c69 6365 2d62 696f  ttps://alice-bio
+00000a10: 6d65 7472 6963 732e 6769 7468 7562 2e69  metrics.github.i
+00000a20: 6f2f 7065 7469 7363 6f2f 0a5b 536f 7572  o/petisco/.[Sour
+00000a30: 6365 2043 6f64 655d 3a20 2e2f 7065 7469  ce Code]: ./peti
+00000a40: 7363 6f0a 5b45 7861 6d70 6c65 735d 3a20  sco.[Examples]: 
+00000a50: 2e2f 6578 616d 706c 6573 0a0a 2d2d 2d0a  ./examples..---.
+00000a60: 0a23 2320 5768 6174 2069 7320 7065 7469  .## What is peti
+00000a70: 7363 6f3f 20f0 9f8d aa0a 0a70 6574 6973  sco? ......petis
+00000a80: 636f 2069 7320 6120 6672 616d 6577 6f72  co is a framewor
+00000a90: 6b20 666f 7220 6865 6c70 696e 6720 5079  k for helping Py
+00000aa0: 7468 6f6e 2064 6576 656c 6f70 6572 7320  thon developers 
+00000ab0: 746f 2062 7569 6c64 2063 6c65 616e 2041  to build clean A
+00000ac0: 7070 6c69 6361 7469 6f6e 7320 696e 2050  pplications in P
+00000ad0: 7974 686f 6e2e 0a0a 2323 2048 6f77 2063  ython...## How c
+00000ae0: 6f75 6c64 2070 6574 6973 636f 2068 656c  ould petisco hel
+00000af0: 7020 6d65 3f20 f09f 8daa 0a0a 7065 7469  p me? ......peti
+00000b00: 7363 6f20 7072 6f76 6964 6573 2073 6576  sco provides sev
+00000b10: 6572 616c 2068 616e 6479 2063 6c61 7373  eral handy class
+00000b20: 6573 2074 6f20 6865 6c70 2079 6f75 206f  es to help you o
+00000b30: 6e20 6465 6669 6e69 6e67 2079 6f75 7220  n defining your 
+00000b40: 646f 6d61 696e 2077 6974 6820 6865 7861  domain with hexa
+00000b50: 676f 6e61 6c20 6172 6368 6974 6563 7475  gonal architectu
+00000b60: 7265 2c20 6576 656e 7420 7374 7265 616d  re, event stream
+00000b70: 696e 6720 616e 6420 4351 5253 2e0a 0a23  ing and CQRS...#
+00000b80: 2320 496e 7374 616c 6c61 7469 6f6e 20f0  # Installation .
+00000b90: 9f92 bb0a 0a60 6060 636f 6e73 6f6c 650a  .....```console.
+00000ba0: 7069 7020 696e 7374 616c 6c20 7065 7469  pip install peti
+00000bb0: 7363 6f0a 6060 600a 0a49 6e73 7461 6c6c  sco.```..Install
+00000bc0: 6174 696f 6e20 7769 7468 2045 7874 7261  ation with Extra
+00000bd0: 730a 0a60 6060 636f 6e73 6f6c 650a 7069  s..```console.pi
+00000be0: 7020 696e 7374 616c 6c20 7065 7469 7363  p install petisc
+00000bf0: 6f5b 6661 7374 6170 692c 7371 6c61 6c63  o[fastapi,sqlalc
+00000c00: 6865 6d79 2c65 6c61 7374 6963 2c65 6c61  hemy,elastic,ela
+00000c10: 7374 6963 2d61 706d 2c72 6162 6269 746d  stic-apm,rabbitm
+00000c20: 712c 736c 6163 6b2c 7265 6469 735d 0a60  q,slack,redis].`
+00000c30: 6060 0a0a 2323 2043 6f6e 7472 6962 7574  ``..## Contribut
+00000c40: 650a 0a57 6527 6420 6c6f 7665 2079 6f75  e..We'd love you
+00000c50: 2074 6f20 636f 6e74 7269 6275 7465 2074   to contribute t
+00000c60: 6f20 2a70 6574 6973 636f 2a20 f09f a5b3  o *petisco* ....
+00000c70: f09f a5b3 f09f a5b3 f09f a5b3 f09f a5b3  ................
+00000c80: f09f a5b3 efb8 8fef b88f 210a 0a46 6f72  ..........!..For
+00000c90: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00000ca0: 6e2c 2063 6865 636b 206f 7572 205b 646f  n, check our [do
+00000cb0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000cc0: 7073 3a2f 2f61 6c69 6365 2d62 696f 6d65  ps://alice-biome
+00000cd0: 7472 6963 732e 6769 7468 7562 2e69 6f2f  trics.github.io/
+00000ce0: 7065 7469 7363 6f2f 636f 6e74 7269 6275  petisco/contribu
+00000cf0: 7469 6e67 2f29 0a0a 2323 2043 6f6e 7461  ting/)..## Conta
+00000d00: 6374 20f0 9f93 ac0a 0a3c 7375 7070 6f72  ct ......<suppor
+00000d10: 7440 616c 6963 6562 696f 6d65 7472 6963  t@alicebiometric
+00000d20: 732e 636f 6d3e 0a                        s.com>.
```

### Comparing `petisco-2.1.3/petisco.egg-info/SOURCES.txt` & `petisco-2.1.4/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/setup.cfg` & `petisco-2.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `petisco-2.1.3/setup.py` & `petisco-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     extras_require={
         "sqlalchemy": [
             "sqlalchemy<3.0.0,>=2.0.15",
```

### Comparing `petisco-2.1.3/tests/fixtures.py` & `petisco-2.1.4/tests/fixtures.py`

 * *Files identical despite different names*

