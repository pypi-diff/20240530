# Comparing `tmp/petisco-2.1.4.tar.gz` & `tmp/petisco-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-2.1.4.tar", last modified: Thu May 30 05:34:27 2024, max compression
+gzip compressed data, was "petisco-2.1.5.tar", last modified: Thu May 30 13:07:07 2024, max compression
```

## Comparing `petisco-2.1.4.tar` & `petisco-2.1.5.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 05:34:24.000000 petisco-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 05:34:24.000000 petisco-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 05:34:27.383946 petisco-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 05:34:24.000000 petisco-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.355945 petisco-2.1.4/petisco/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/chaos_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/chaos/check_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/async_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/controller/meta_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/dependency_injection/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/handlers/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/async_app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/async_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/meta_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.363945 petisco-2.1.4/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/legacy_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.367945 petisco-2.1.4/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/async_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/persistence/fake_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/domain/value_objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/value_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/domain/value_objects/middleware_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/datetime_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/time_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/async_elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/elastic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic/is_elastic_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/elastic_apm/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/capture_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/elastic_apm/is_elastic_apm_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.371945 petisco-2.1.4/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/add_controller_responses_to_response_mocker_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/ensure_all_routers_are_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/fastapi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/application/response_mocker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/as_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/loguru_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/logger/not_implemented_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/meiga/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/meiga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.375945 petisco-2.1.4/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/rabbitmq_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/redis/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/redis/is_redis_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.379946 petisco-2.1.4/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/extra/threading/pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/public_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/petisco/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.359945 petisco-2.1.4/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 05:34:27.000000 petisco-2.1.4/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 05:34:24.000000 petisco-2.1.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 05:34:27.387946 petisco-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-30 05:34:24.000000 petisco-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:27.383946 petisco-2.1.4/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:34:24.000000 petisco-2.1.4/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.947740 petisco-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 13:07:05.000000 petisco-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 13:07:05.000000 petisco-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 13:07:07.947740 petisco-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 13:07:05.000000 petisco-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.911740 petisco-2.1.5/petisco/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.919740 petisco-2.1.5/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.923740 petisco-2.1.5/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.923740 petisco-2.1.5/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.927740 petisco-2.1.5/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.927740 petisco-2.1.5/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/model/legacy_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.927740 petisco-2.1.5/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/persistence/fake_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.927740 petisco-2.1.5/petisco/base/domain/value_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/value_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/domain/value_objects/middleware_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.927740 petisco-2.1.5/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/datetime_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/time_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/elastic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic/is_elastic_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic_apm/capture_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.931740 petisco-2.1.5/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/application/add_controller_responses_to_response_mocker_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/application/ensure_all_routers_are_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/application/fastapi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/application/response_mocker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/meiga/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/meiga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.935740 petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/rabbitmq_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.939740 petisco-2.1.5/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.943740 petisco-2.1.5/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.947740 petisco-2.1.5/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.915740 petisco-2.1.5/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 13:07:07.000000 petisco-2.1.5/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.947740 petisco-2.1.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 13:07:05.000000 petisco-2.1.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 13:07:07.947740 petisco-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-30 13:07:05.000000 petisco-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.947740 petisco-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 13:07:05.000000 petisco-2.1.5/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:07.947740 petisco-2.1.5/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:07:05.000000 petisco-2.1.5/tests/modules/__init__.py
```

### Comparing `petisco-2.1.4/LICENSE` & `petisco-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/PKG-INFO` & `petisco-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.1.4
+Version: 2.1.5
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petisco-2.1.4/README.md` & `petisco-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/application.py` & `petisco-2.1.5/petisco/base/application/application.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/application_info.py` & `petisco-2.1.5/petisco/base/application/application_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/chaos/chaos_config.py` & `petisco-2.1.5/petisco/base/application/chaos/chaos_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/controller/async_controller.py` & `petisco-2.1.5/petisco/base/application/controller/async_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/controller/controller.py` & `petisco-2.1.5/petisco/base/application/controller/controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/controller/http_error.py` & `petisco-2.1.5/petisco/base/application/controller/http_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/controller/meta_controller.py` & `petisco-2.1.5/petisco/base/application/controller/meta_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/dependency_injection/container.py` & `petisco-2.1.5/petisco/base/application/dependency_injection/container.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/dependency_injection/dependency.py` & `petisco-2.1.5/petisco/base/application/dependency_injection/dependency.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/handlers/message_handler.py` & `petisco-2.1.5/petisco/base/application/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/middleware/middleware.py` & `petisco-2.1.5/petisco/base/application/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.1.5/petisco/base/application/middleware/notifier_middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/notifier/notifier.py` & `petisco-2.1.5/petisco/base/application/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-2.1.5/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/patterns/crud_repository.py` & `petisco-2.1.5/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.1.5/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/application/use_case/meta_use_case.py` & `petisco-2.1.5/petisco/base/application/use_case/meta_use_case.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.1.5/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.1.5/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.1.5/petisco/base/domain/errors/defaults/not_found.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/errors/domain_error.py` & `petisco-2.1.5/petisco/base/domain/errors/domain_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/errors/unknown_error.py` & `petisco-2.1.5/petisco/base/domain/errors/unknown_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-2.1.5/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/command_bus.py` & `petisco-2.1.5/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/command_subscriber.py` & `petisco-2.1.5/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.1.5/petisco/base/domain/message/domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-2.1.5/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message.py` & `petisco-2.1.5/petisco/base/domain/message/message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_bus.py` & `petisco-2.1.5/petisco/base/domain/message/message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_configurer.py` & `petisco-2.1.5/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_consumer.py` & `petisco-2.1.5/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_handler_returns_none_error.py` & `petisco-2.1.5/petisco/base/domain/message/message_handler_returns_none_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_subscriber.py` & `petisco-2.1.5/petisco/base/domain/message/message_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/message_subscriber_info.py` & `petisco-2.1.5/petisco/base/domain/message/message_subscriber_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/not_implemented_command_bus.py` & `petisco-2.1.5/petisco/base/domain/message/not_implemented_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.1.5/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.1.5/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/model/aggregate_root.py` & `petisco-2.1.5/petisco/base/domain/model/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/model/legacy_uuid.py` & `petisco-2.1.5/petisco/base/domain/model/legacy_uuid.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/model/uuid.py` & `petisco-2.1.5/petisco/base/domain/model/uuid.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/model/value_object.py` & `petisco-2.1.5/petisco/base/domain/model/value_object.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/persistence/async_fake_database.py` & `petisco-2.1.5/petisco/base/domain/persistence/async_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/persistence/database.py` & `petisco-2.1.5/petisco/base/domain/persistence/database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/domain/persistence/databases.py` & `petisco-2.1.5/petisco/base/domain/persistence/databases.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/misc/async_wrapper.py` & `petisco-2.1.5/petisco/base/misc/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/misc/builder.py` & `petisco-2.1.5/petisco/base/misc/builder.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/misc/result_mapper.py` & `petisco-2.1.5/petisco/base/misc/result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/misc/singleton.py` & `petisco-2.1.5/petisco/base/misc/singleton.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/base/misc/wrapper.py` & `petisco-2.1.5/petisco/base/misc/wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/cli/petisco.py` & `petisco-2.1.5/petisco/cli/petisco.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/cli/petisco_dev.py` & `petisco-2.1.5/petisco/cli/petisco_dev.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/cli/petisco_rabbitmq.py` & `petisco-2.1.5/petisco/cli/petisco_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/__init__.py` & `petisco-2.1.5/petisco/extra/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/async_elastic_database.py` & `petisco-2.1.5/petisco/extra/elastic/async_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/elastic_connection.py` & `petisco-2.1.5/petisco/extra/elastic/elastic_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/elastic_database.py` & `petisco-2.1.5/petisco/extra/elastic/elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.1.5/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic/elastic_repository.py` & `petisco-2.1.5/petisco/extra/elastic/elastic_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py` & `petisco-2.1.5/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/__init__.py` & `petisco-2.1.5/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/application/ensure_all_routers_are_async.py` & `petisco-2.1.5/petisco/extra/fastapi/application/ensure_all_routers_are_async.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/application/fastapi_application.py` & `petisco-2.1.5/petisco/extra/fastapi/application/fastapi_application.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/application/response_mocker.py` & `petisco-2.1.5/petisco/extra/fastapi/application/response_mocker.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.1.5/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/fastapi/testing/assert_http_exception.py` & `petisco-2.1.5/petisco/extra/fastapi/testing/assert_http_exception.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/logger/__init__.py` & `petisco-2.1.5/petisco/extra/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/logger/log_message.py` & `petisco-2.1.5/petisco/extra/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/logger/logging_based_logger.py` & `petisco-2.1.5/petisco/extra/logger/logging_based_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/logger/loguru_logger.py` & `petisco-2.1.5/petisco/extra/logger/loguru_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/__init__.py` & `petisco-2.1.5/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         meta = self.get_configured_meta()
         dispatched_commands = []
         commands = self._check_input(command)
 
         try:
             check_chaos_publication()
             channel = self.connector.get_channel(self.rabbitmq_key)
-            for i, command in enumerate(commands):
+            for command in commands:
                 self._check_is_command(command)
                 command = command.update_meta(meta)
-                self.publisher.execute(channel, command, first_time=i == 0)
+                self.publisher.execute(channel, command)
                 if channel.is_open and not isinstance(self.connector, RabbitMqConsumerConnector):
                     channel.close()
                 dispatched_commands.append(command)
         except ChannelClosedByBroker:
             unpublished_commands = [command for command in commands if command not in dispatched_commands]
             self._retry(unpublished_commands)
         except Exception as exc:  # noqa
```

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,18 +47,18 @@
         meta = self.get_configured_meta()
         published_domain_event = []
         domain_events = self._check_input(domain_event)
 
         try:
             check_chaos_publication()
             channel = self.connector.get_channel(self.rabbitmq_key)
-            for i, domain_event in enumerate(domain_events):
+            for domain_event in domain_events:
                 self._check_is_domain_event(domain_event)
                 domain_event = domain_event.update_meta(meta)
-                self.publisher.execute(channel, domain_event, first_time=i == 0)
+                self.publisher.execute(channel, domain_event)
                 published_domain_event.append(domain_event)
             if channel.is_open and not isinstance(self.connector, RabbitMqConsumerConnector):
                 channel.close()
         except ChannelClosedByBroker:
             unpublished_domain_events = [
                 event for event in domain_events if event not in published_domain_event
             ]
```

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,36 @@
 )
 
 
 class RabbitMqMessagePublisher:
     def __init__(self, exchange_name: str) -> None:
         self._exchange_name = exchange_name
         self._properties = BasicProperties(delivery_mode=2)  # PERSISTENT_TEXT_PLAIN
+        self.executed_times = 0
+
+    def _confirm_delivery_if_required(self, channel: BlockingChannel) -> bool:
+        """
+        Confirm delivery should be enabled just once. Source: https://www.rabbitmq.com/tutorials/tutorial-seven-java#enabling-publisher-confirms-on-a-channel
+        Otherwise with Pika we get lots of error messages
+        """
+        self.executed_times += 1
+        if self.executed_times == 1:
+            channel.confirm_delivery()
+            return True
+        return False
 
     def execute(
         self,
         channel: BlockingChannel,
         message: Message,
         routing_key: Union[str, None] = None,
-        first_time: bool = False,
     ) -> None:
         if routing_key is None:
             routing_key = RabbitMqMessageQueueNameFormatter.format(message, exchange_name=self._exchange_name)
 
-        if first_time:
-            # Confirm delivery should be enabled just once. Source: https://www.rabbitmq.com/tutorials/tutorial-seven-java#enabling-publisher-confirms-on-a-channel
-            # Otherwise with Pika we get lots of error messages
-            channel.confirm_delivery()
+        self._confirm_delivery_if_required(channel)
         channel.basic_publish(
             exchange=self._exchange_name,
             routing_key=routing_key,
             body=message.format_json().encode(),
             properties=self._properties,
         )
```

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.1.5/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.1.5/petisco/extra/rabbitmq/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/rabbitmq_configurer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/rabbitmq_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.1.5/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.1.5/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.1.5/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_command_bus.py` & `petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py` & `petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/redis/application/message/bus/redis_message_bus.py` & `petisco-2.1.5/petisco/extra/redis/application/message/bus/redis_message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/__init__.py` & `petisco-2.1.5/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.1.5/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.1.5/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.1.5/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-2.1.5/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/slack/dependencies.py` & `petisco-2.1.5/petisco/extra/slack/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_database.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/async_sql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_base.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_base.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_database.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_repository.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.1.5/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.1.5/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/extra/threading/pool_executor.py` & `petisco-2.1.5/petisco/extra/threading/pool_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco/public_api.py` & `petisco-2.1.5/petisco/public_api.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/petisco.egg-info/PKG-INFO` & `petisco-2.1.5/petisco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.1.4
+Version: 2.1.5
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petisco-2.1.4/petisco.egg-info/SOURCES.txt` & `petisco-2.1.5/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/setup.cfg` & `petisco-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/setup.py` & `petisco-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `petisco-2.1.4/tests/fixtures.py` & `petisco-2.1.5/tests/fixtures.py`

 * *Files identical despite different names*

