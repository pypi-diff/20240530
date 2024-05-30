# Comparing `tmp/apimatic-core-0.2.8.tar.gz` & `tmp/apimatic_core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-core-0.2.8.tar", last modified: Sat Feb  3 17:34:13 2024, max compression
+gzip compressed data, was "apimatic_core-0.2.9.tar", last modified: Mon Apr 22 11:23:48 2024, max compression
```

## Comparing `apimatic-core-0.2.8.tar` & `apimatic_core-0.2.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.415277 apimatic-core-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-02-03 17:34:13.415277 apimatic-core-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.391277 apimatic-core-0.2.8/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.391277 apimatic-core-0.2.8/apimatic_core/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/header_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/authentication/multiple/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/multiple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/multiple/and_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/multiple/auth_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/multiple/or_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/multiple/single_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/authentication/query_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/configurations/endpoint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/configurations/global_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/decorators/lazy_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/exceptions/anyof_validation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/exceptions/auth_validation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/exceptions/oneof_validation_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/factories/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/factories/http_response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/http/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/http/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/configurations/http_client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/http_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.395277 apimatic-core-0.2.8/apimatic_core/http/request/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/request/http_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.399277 apimatic-core-0.2.8/apimatic_core/http/response/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/response/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/http/response/http_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.399277 apimatic-core-0.2.8/apimatic_core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/logger/endpoint_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.399277 apimatic-core-0.2.8/apimatic_core/types/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/array_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/datetime_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/error_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/file_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.399277 apimatic-core-0.2.8/apimatic_core/types/union_types/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/union_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/union_types/any_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/union_types/leaf_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/union_types/one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/union_types/union_type_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/types/xml_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/apimatic_core/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/datetime_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/file_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/union_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/apimatic_core/utilities/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.415277 apimatic-core-0.2.8/apimatic_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-02-03 17:34:13.000000 apimatic-core-0.2.8/apimatic_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-03 17:34:13.000000 apimatic-core-0.2.8/apimatic_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 17:34:13.000000 apimatic-core-0.2.8/apimatic_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-03 17:34:13.000000 apimatic-core-0.2.8/apimatic_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-03 17:34:13.000000 apimatic-core-0.2.8/apimatic_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 17:34:13.415277 apimatic-core-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/api_call_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/api_call_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/api_call_tests/test_api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/api_logger_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/api_logger_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/api_logger_tests/test_api_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.403277 apimatic-core-0.2.8/tests/apimatic_core/mocks/callables/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/callables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/callables/base_uri_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.407277 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/global_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/local_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.407277 apimatic-core-0.2.8/tests/apimatic_core/mocks/http/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/http/http_response_catcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.407277 apimatic-core-0.2.8/tests/apimatic_core/mocks/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/logger/api_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.411277 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/cat_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/complex_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/deer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/dog_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/grand_parent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/inner_complex_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/months.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/one_of_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/orbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/union_type_scalar_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/wolf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/models/xml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/mocks/union_type_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.411277 apimatic-core-0.2.8/tests/apimatic_core/request_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/request_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45088 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/request_builder_tests/test_request_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.411277 apimatic-core-0.2.8/tests/apimatic_core/response_handler_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/response_handler_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/response_handler_tests/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.411277 apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59508 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/test_any_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    59974 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/test_one_of.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 17:34:13.415277 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62058 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   126287 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_datetime_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_file_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    34274 2024-02-03 17:33:56.000000 apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/header_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/authentication/multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/multiple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/multiple/and_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/multiple/auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/multiple/or_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/multiple/single_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/authentication/query_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/configurations/endpoint_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/configurations/global_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/decorators/lazy_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.471814 apimatic_core-0.2.9/apimatic_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/exceptions/anyof_validation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/exceptions/auth_validation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/exceptions/oneof_validation_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/factories/http_response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/http/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/configurations/http_client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/http_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/http/request/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/request/http_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/http/response/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/response/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/http/response/http_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/logger/endpoint_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/array_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/datetime_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/error_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/file_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.475814 apimatic_core-0.2.9/apimatic_core/types/union_types/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/union_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/union_types/any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/union_types/leaf_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/union_types/one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/union_types/union_type_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/types/xml_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/apimatic_core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/datetime_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/union_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/apimatic_core/utilities/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/apimatic_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-04-22 11:23:48.000000 apimatic_core-0.2.9/apimatic_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-22 11:23:48.000000 apimatic_core-0.2.9/apimatic_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:23:48.000000 apimatic_core-0.2.9/apimatic_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-22 11:23:48.000000 apimatic_core-0.2.9/apimatic_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 11:23:48.000000 apimatic_core-0.2.9/apimatic_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/api_call_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/api_call_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/api_call_tests/test_api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/api_logger_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/api_logger_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/api_logger_tests/test_api_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.479814 apimatic_core-0.2.9/tests/apimatic_core/mocks/callables/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/callables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/callables/base_uri_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.483814 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/global_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/local_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.483814 apimatic_core-0.2.9/tests/apimatic_core/mocks/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/http/http_response_catcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.483814 apimatic_core-0.2.9/tests/apimatic_core/mocks/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/logger/api_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/cat_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/deer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/dog_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/grand_parent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/inner_complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/months.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/one_of_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/union_type_scalar_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/wolf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/models/xml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/mocks/union_type_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/tests/apimatic_core/request_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/request_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45088 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/request_builder_tests/test_request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/tests/apimatic_core/response_handler_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/response_handler_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/response_handler_tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59508 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/test_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59974 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/test_one_of.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:23:48.487814 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62058 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126287 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_datetime_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34274 2024-04-22 11:23:40.000000 apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_xml_helper.py
```

### Comparing `apimatic-core-0.2.8/LICENSE` & `apimatic_core-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/PKG-INFO` & `apimatic_core-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
 Home-page: https://github.com/apimatic/core-lib-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apimatic-core-0.2.8/README.md` & `apimatic_core-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/api_call.py` & `apimatic_core-0.2.9/apimatic_core/api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/authentication/multiple/and_auth_group.py` & `apimatic_core-0.2.9/apimatic_core/authentication/multiple/and_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/authentication/multiple/auth_group.py` & `apimatic_core-0.2.9/apimatic_core/authentication/multiple/auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/authentication/multiple/or_auth_group.py` & `apimatic_core-0.2.9/apimatic_core/authentication/multiple/or_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/authentication/multiple/single_auth.py` & `apimatic_core-0.2.9/apimatic_core/authentication/multiple/single_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/configurations/endpoint_configuration.py` & `apimatic_core-0.2.9/apimatic_core/configurations/endpoint_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/configurations/global_configuration.py` & `apimatic_core-0.2.9/apimatic_core/configurations/global_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/http/configurations/http_client_configuration.py` & `apimatic_core-0.2.9/apimatic_core/http/configurations/http_client_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/http/http_callback.py` & `apimatic_core-0.2.9/apimatic_core/http/http_callback.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/http/request/http_request.py` & `apimatic_core-0.2.9/apimatic_core/http/request/http_request.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/http/response/api_response.py` & `apimatic_core-0.2.9/apimatic_core/http/response/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/http/response/http_response.py` & `apimatic_core-0.2.9/apimatic_core/http/response/http_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/request_builder.py` & `apimatic_core-0.2.9/apimatic_core/request_builder.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/response_handler.py` & `apimatic_core-0.2.9/apimatic_core/response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/array_serialization_format.py` & `apimatic_core-0.2.9/apimatic_core/types/array_serialization_format.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/error_case.py` & `apimatic_core-0.2.9/apimatic_core/types/error_case.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/parameter.py` & `apimatic_core-0.2.9/apimatic_core/types/parameter.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/union_types/any_of.py` & `apimatic_core-0.2.9/apimatic_core/types/union_types/any_of.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/union_types/leaf_type.py` & `apimatic_core-0.2.9/apimatic_core/types/union_types/leaf_type.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/union_types/one_of.py` & `apimatic_core-0.2.9/apimatic_core/types/union_types/one_of.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/union_types/union_type_context.py` & `apimatic_core-0.2.9/apimatic_core/types/union_types/union_type_context.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/types/xml_attributes.py` & `apimatic_core-0.2.9/apimatic_core/types/xml_attributes.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/api_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/api_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/auth_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/auth_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 
 
 class AuthHelper:
 
     @staticmethod
     def get_base64_encoded_value(*props, delimiter=':'):
-        if props:
+        if props.__len__() > 0 and not any(prop is None for prop in props):
             joined = delimiter.join(props)
             encoded = base64.b64encode(str.encode(joined)).decode('iso-8859-1')
             return encoded
 
     @staticmethod
     def get_token_expiry(current_timestamp, expires_in):
         return current_timestamp + int(expires_in)
```

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/comparison_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/datetime_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/file_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/union_type_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/union_type_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core/utilities/xml_helper.py` & `apimatic_core-0.2.9/apimatic_core/utilities/xml_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/apimatic_core.egg-info/PKG-INFO` & `apimatic_core-0.2.9/apimatic_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
 Home-page: https://github.com/apimatic/core-lib-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apimatic-core-0.2.8/apimatic_core.egg-info/SOURCES.txt` & `apimatic_core-0.2.9/apimatic_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/setup.py` & `apimatic_core-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-core',
-    version='0.2.8',
+    version='0.2.9',
     description='A library that contains core logic and utilities for '
                 'consuming REST APIs using Python SDKs generated by APIMatic.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
```

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/api_call_tests/test_api_call.py` & `apimatic_core-0.2.9/tests/apimatic_core/api_call_tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/api_logger_tests/test_api_logger.py` & `apimatic_core-0.2.9/tests/apimatic_core/api_logger_tests/test_api_logger.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/base.py` & `apimatic_core-0.2.9/tests/apimatic_core/base.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/basic_auth.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/basic_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/bearer_auth.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/authentications/custom_query_authentication.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/authentications/custom_query_authentication.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/callables/base_uri_callable.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/callables/base_uri_callable.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/api_exception.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/global_test_exception.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/global_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/local_test_exception.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/local_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/exceptions/nested_model_exception.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/exceptions/nested_model_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/http/http_client.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/http/http_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/api_response.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/atom.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/atom.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/cat_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/cat_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/complex_type.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/complex_type.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/days.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/days.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/deer.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/deer.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/dog_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/dog_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/grand_parent_class_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/grand_parent_class_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/inner_complex_type.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/inner_complex_type.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/lion.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/lion.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/months.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/months.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/one_of_xml.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/one_of_xml.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/orbit.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/orbit.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/person.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/person.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/rabbit.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/rabbit.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/union_type_scalar_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/union_type_scalar_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/validate.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/validate.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/wolf_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/wolf_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/models/xml_model.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/models/xml_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/mocks/union_type_lookup.py` & `apimatic_core-0.2.9/tests/apimatic_core/mocks/union_type_lookup.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/request_builder_tests/test_request_builder.py` & `apimatic_core-0.2.9/tests/apimatic_core/request_builder_tests/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/response_handler_tests/test_response_handler.py` & `apimatic_core-0.2.9/tests/apimatic_core/response_handler_tests/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/test_any_of.py` & `apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/test_any_of.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/union_type_tests/test_one_of.py` & `apimatic_core-0.2.9/tests/apimatic_core/union_type_tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_api_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_auth_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_auth_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 class TestAuthHelper:
 
     def test_base64_encoded_none_value(self):
         actual_base64_encoded_value = AuthHelper.get_base64_encoded_value()
         expected_base64_encoded_value = None
         assert actual_base64_encoded_value == expected_base64_encoded_value
 
+    def test_base64_encoded_provided_none_values(self):
+        actual_base64_encoded_value = AuthHelper.get_base64_encoded_value(None, None)
+        expected_base64_encoded_value = None
+        assert actual_base64_encoded_value == expected_base64_encoded_value
+
+        actual_base64_encoded_value = AuthHelper.get_base64_encoded_value('test_username', None)
+        expected_base64_encoded_value = None
+        assert actual_base64_encoded_value == expected_base64_encoded_value
+
     def test_base64_encoded_value(self):
         actual_base64_encoded_value = AuthHelper.get_base64_encoded_value('test_username', 'test_password')
         expected_base64_encoded_value = 'dGVzdF91c2VybmFtZTp0ZXN0X3Bhc3N3b3Jk'
         assert actual_base64_encoded_value == expected_base64_encoded_value
 
     def test_token_expiry(self):
         current_utc_timestamp = AuthHelper.get_current_utc_timestamp()
```

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_comparison_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_datetime_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_datetime_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_file_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.8/tests/apimatic_core/utility_tests/test_xml_helper.py` & `apimatic_core-0.2.9/tests/apimatic_core/utility_tests/test_xml_helper.py`

 * *Files identical despite different names*

