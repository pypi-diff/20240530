# Comparing `tmp/red_utils-0.2.8.tar.gz` & `tmp/red_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_utils-0.2.8.tar", last modified: Sun Dec  3 19:51:43 2023, max compression
+gzip compressed data, was "red_utils-0.2.9.tar", last modified: Fri Dec  8 16:43:12 2023, max compression
```

## Comparing `red_utils-0.2.8.tar` & `red_utils-0.2.9.tar`

### file list

```diff
@@ -1,140 +1,142 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.638915 red_utils-0.2.8/
--rw-r--r--   0 jack      (1000) jack      (1000)     7899 2023-12-03 19:51:43.638915 red_utils-0.2.8/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)     5885 2023-09-20 17:01:44.000000 red_utils-0.2.8/README.md
--rw-rw-r--   0 jack      (1000) jack      (1000)     2476 2023-12-03 19:50:12.000000 red_utils-0.2.8/pyproject.toml
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.618915 red_utils-0.2.8/red_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      160 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      366 2023-09-18 20:55:09.000000 red_utils-0.2.8/red_utils/__main__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.618915 red_utils-0.2.8/red_utils/core/
--rw-rw-r--   0 jack      (1000) jack      (1000)       66 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/core/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.618915 red_utils-0.2.8/red_utils/core/dataclass_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)       87 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/core/dataclass_utils/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.618915 red_utils-0.2.8/red_utils/core/dataclass_utils/mixins/
--rw-rw-r--   0 jack      (1000) jack      (1000)       73 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/core/dataclass_utils/mixins/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      937 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/core/dataclass_utils/mixins/mixin_classes.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.618915 red_utils-0.2.8/red_utils/domain/
--rw-rw-r--   0 jack      (1000) jack      (1000)        0 2023-09-18 20:55:09.000000 red_utils-0.2.8/red_utils/domain/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/exc/
--rw-rw-r--   0 jack      (1000) jack      (1000)       73 2023-09-18 20:55:09.000000 red_utils-0.2.8/red_utils/exc/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      757 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/exc/base.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1534 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/exc/generic.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/ext/
--rw-rw-r--   0 jack      (1000) jack      (1000)      798 2023-09-25 04:34:32.000000 red_utils-0.2.8/red_utils/ext/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/ext/arrow_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      205 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/arrow_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      238 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/arrow_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      126 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/arrow_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3834 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/arrow_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      207 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/arrow_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/ext/context_managers/
--rw-rw-r--   0 jack      (1000) jack      (1000)      159 2023-09-25 04:37:42.000000 red_utils-0.2.8/red_utils/ext/context_managers/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/ext/context_managers/cli_spinners/
--rw-rw-r--   0 jack      (1000) jack      (1000)       95 2023-09-25 04:37:42.000000 red_utils-0.2.8/red_utils/ext/context_managers/cli_spinners/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      512 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/context_managers/cli_spinners/handlers.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.622915 red_utils-0.2.8/red_utils/ext/diskcache_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      933 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      242 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     9847 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/classes.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      874 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     8271 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5296 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/diskcache_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.626915 red_utils-0.2.8/red_utils/ext/fastapi_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      631 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      240 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      761 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      780 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/dependencies.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1149 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/healthcheck.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5349 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1290 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/tag_definitions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1964 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/uvicorn_override.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2185 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/fastapi_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.626915 red_utils-0.2.8/red_utils/ext/httpx_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      297 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/httpx_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      238 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/httpx_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      177 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/httpx_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2953 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/httpx_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1168 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/httpx_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.626915 red_utils-0.2.8/red_utils/ext/loguru_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      951 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      239 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3921 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      518 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/enums.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2602 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     6189 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/sinks.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1963 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/loguru_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.626915 red_utils-0.2.8/red_utils/ext/msgpack_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      374 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      240 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      890 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/classes.py
--rw-rw-r--   0 jack      (1000) jack      (1000)       78 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     6169 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      152 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/msgpack_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/ext/pendulum_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      223 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/pendulum_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      241 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/pendulum_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      312 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/pendulum_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1687 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/pendulum_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      167 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/ext/pendulum_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/ext/pydantic_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      101 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/pydantic_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      241 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/pydantic_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1261 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/pydantic_utils/parsers.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)     1585 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      242 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1552 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/base.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5868 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/connection_models.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      133 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2471 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/custom_types.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5894 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/utils.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/
--rw-rw-r--   0 jack      (1000) jack      (1000)      178 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/std/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/context_managers/
--rw-rw-r--   0 jack      (1000) jack      (1000)      275 2023-09-25 04:11:45.000000 red_utils-0.2.8/red_utils/std/context_managers/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      243 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/context_managers/__main__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/context_managers/benchmarks/
--rw-rw-r--   0 jack      (1000) jack      (1000)      118 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/context_managers/benchmarks/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      967 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/context_managers/benchmarks/fn_benchmarks.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/context_managers/database_managers/
--rw-rw-r--   0 jack      (1000) jack      (1000)      113 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/context_managers/database_managers/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3959 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/context_managers/database_managers/sqlite_managers.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/context_managers/object_managers/
--rw-rw-r--   0 jack      (1000) jack      (1000)      104 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/context_managers/object_managers/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4826 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/context_managers/object_managers/protect.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/dataclass_mixins/
--rw-rw-r--   0 jack      (1000) jack      (1000)       87 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/std/dataclass_mixins/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      944 2023-12-03 19:48:35.000000 red_utils-0.2.8/red_utils/std/dataclass_mixins/mixins.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.630915 red_utils-0.2.8/red_utils/std/dict_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      172 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/dict_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/dict_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1968 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/dict_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      373 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/dict_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/red_utils/std/file_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      180 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/file_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/file_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      298 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/file_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     6108 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/file_utils/operations.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/red_utils/std/hash_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      103 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/hash_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/hash_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1054 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/hash_utils/operations.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/red_utils/std/time_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      194 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/time_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/time_utils/__main__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      126 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/time_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1340 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/time_utils/operations.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/red_utils/std/uuid_utils/
--rw-rw-r--   0 jack      (1000) jack      (1000)      216 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/uuid_utils/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      199 2023-12-03 19:47:57.000000 red_utils-0.2.8/red_utils/std/uuid_utils/classes.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      144 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/uuid_utils/constants.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     8283 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/uuid_utils/operations.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2803 2023-09-20 17:01:44.000000 red_utils-0.2.8/red_utils/std/uuid_utils/validators.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/red_utils.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)     7899 2023-12-03 19:51:43.000000 red_utils-0.2.8/red_utils.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)     4215 2023-12-03 19:51:43.000000 red_utils-0.2.8/red_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-12-03 19:51:43.000000 red_utils-0.2.8/red_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)      573 2023-12-03 19:51:43.000000 red_utils-0.2.8/red_utils.egg-info/requires.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       10 2023-12-03 19:51:43.000000 red_utils-0.2.8/red_utils.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-12-03 19:51:43.638915 red_utils-0.2.8/setup.cfg
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-03 19:51:43.634915 red_utils-0.2.8/tests/
--rw-rw-r--   0 jack      (1000) jack      (1000)      520 2023-09-18 20:55:09.000000 red_utils-0.2.8/tests/test_file_utils.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.231411 red_utils-0.2.9/
+-rw-r--r--   0 jack      (1000) jack      (1000)     7899 2023-12-08 16:43:12.231411 red_utils-0.2.9/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5885 2023-12-08 16:38:36.000000 red_utils-0.2.9/README.md
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2476 2023-12-08 16:41:44.000000 red_utils-0.2.9/pyproject.toml
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.207411 red_utils-0.2.9/red_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      160 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      366 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/__main__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.207411 red_utils-0.2.9/red_utils/core/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      165 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/core/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      243 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/core/constants.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.207411 red_utils-0.2.9/red_utils/core/dataclass_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       87 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/core/dataclass_utils/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.207411 red_utils-0.2.9/red_utils/core/dataclass_utils/mixins/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       73 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/core/dataclass_utils/mixins/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      937 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/core/dataclass_utils/mixins/mixin_classes.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.207411 red_utils-0.2.9/red_utils/domain/
+-rw-rw-r--   0 jack      (1000) jack      (1000)        0 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/domain/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/exc/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       73 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/exc/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      757 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/exc/base.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1534 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/exc/generic.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/ext/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      798 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/ext/arrow_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      205 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/arrow_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      238 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/arrow_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      126 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/arrow_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3834 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/arrow_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      207 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/arrow_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/ext/context_managers/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      159 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/context_managers/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/ext/context_managers/cli_spinners/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       95 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/context_managers/cli_spinners/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      512 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/context_managers/cli_spinners/handlers.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.211411 red_utils-0.2.9/red_utils/ext/diskcache_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      933 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      242 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9847 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/classes.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      874 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8271 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5296 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/diskcache_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.215411 red_utils-0.2.9/red_utils/ext/fastapi_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      631 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      240 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      761 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      780 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/dependencies.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1149 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/healthcheck.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5349 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1290 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/tag_definitions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1964 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/uvicorn_override.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2185 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/fastapi_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.215411 red_utils-0.2.9/red_utils/ext/httpx_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      352 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      238 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1060 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/classes.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      107 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2952 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1649 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/httpx_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.215411 red_utils-0.2.9/red_utils/ext/loguru_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      951 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      239 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3921 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      518 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/enums.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2602 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6189 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/sinks.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1963 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/loguru_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/ext/msgpack_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      374 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      240 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      890 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/classes.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)       78 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6169 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      152 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/msgpack_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/ext/pendulum_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      223 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pendulum_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      241 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pendulum_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      312 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pendulum_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1687 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pendulum_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      167 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pendulum_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/ext/pydantic_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      101 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pydantic_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      241 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pydantic_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1261 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/pydantic_utils/parsers.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1585 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      242 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1552 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/base.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5868 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/connection_models.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      133 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2471 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/custom_types.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5894 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/utils.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/std/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      178 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/std/context_managers/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      275 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      243 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/__main__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/std/context_managers/benchmarks/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      118 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/benchmarks/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      967 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/benchmarks/fn_benchmarks.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.219411 red_utils-0.2.9/red_utils/std/context_managers/database_managers/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      113 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/database_managers/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3959 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/database_managers/sqlite_managers.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/context_managers/object_managers/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      104 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/object_managers/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4826 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/context_managers/object_managers/protect.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/dataclass_mixins/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       87 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dataclass_mixins/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      944 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dataclass_mixins/mixins.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/dict_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      172 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dict_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dict_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1968 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dict_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      373 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/dict_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/hash_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      103 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/hash_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/hash_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1054 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/hash_utils/operations.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/path_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      188 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/path_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/path_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)       35 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/path_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8887 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/path_utils/operations.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/time_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      194 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/time_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      237 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/time_utils/__main__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      126 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/time_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1340 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/time_utils/operations.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/red_utils/std/uuid_utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      216 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/uuid_utils/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      199 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/uuid_utils/classes.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      144 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/uuid_utils/constants.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8283 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/uuid_utils/operations.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2803 2023-12-08 16:38:36.000000 red_utils-0.2.9/red_utils/std/uuid_utils/validators.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.227411 red_utils-0.2.9/red_utils.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)     7899 2023-12-08 16:43:12.000000 red_utils-0.2.9/red_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4280 2023-12-08 16:43:12.000000 red_utils-0.2.9/red_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-12-08 16:43:12.000000 red_utils-0.2.9/red_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)      573 2023-12-08 16:43:12.000000 red_utils-0.2.9/red_utils.egg-info/requires.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       10 2023-12-08 16:43:12.000000 red_utils-0.2.9/red_utils.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-12-08 16:43:12.231411 red_utils-0.2.9/setup.cfg
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-12-08 16:43:12.223411 red_utils-0.2.9/tests/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      520 2023-12-08 16:38:36.000000 red_utils-0.2.9/tests/test_file_utils.py
```

### Comparing `red_utils-0.2.8/PKG-INFO` & `red_utils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red_utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of utility scripts/functions that I use frequently.
 Author-email: redjax <none@none.com>, redjax <jackenyon@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/redjax/red-utils
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: diskcache>=5.6.1
```

### Comparing `red_utils-0.2.8/README.md` & `red_utils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/pyproject.toml` & `red_utils-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "red_utils"
-version = "0.2.8"
+version = "0.2.9"
 description = "Collection of utility scripts/functions that I use frequently."
 authors = [
     { name = "redjax", email = "none@none.com" },
     { name = "redjax", email = "jackenyon@gmail.com" },
 ]
 dependencies = [
     "diskcache>=5.6.1",
```

### Comparing `red_utils-0.2.8/red_utils/core/dataclass_utils/mixins/mixin_classes.py` & `red_utils-0.2.9/red_utils/core/dataclass_utils/mixins/mixin_classes.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/exc/base.py` & `red_utils-0.2.9/red_utils/exc/base.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/exc/generic.py` & `red_utils-0.2.9/red_utils/exc/generic.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/__init__.py` & `red_utils-0.2.9/red_utils/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/arrow_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/arrow_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/context_managers/cli_spinners/handlers.py` & `red_utils-0.2.9/red_utils/ext/context_managers/cli_spinners/handlers.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/diskcache_utils/__init__.py` & `red_utils-0.2.9/red_utils/ext/diskcache_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/diskcache_utils/classes.py` & `red_utils-0.2.9/red_utils/ext/diskcache_utils/classes.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/diskcache_utils/constants.py` & `red_utils-0.2.9/red_utils/ext/diskcache_utils/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/diskcache_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/diskcache_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/diskcache_utils/validators.py` & `red_utils-0.2.9/red_utils/ext/diskcache_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/__init__.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/constants.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/dependencies.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/healthcheck.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/tag_definitions.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/tag_definitions.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/uvicorn_override.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/uvicorn_override.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/fastapi_utils/validators.py` & `red_utils-0.2.9/red_utils/ext/fastapi_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/httpx_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/httpx_utils/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 from .constants import (
     default_headers,
-    valid_methods,
 )
-from .validators import validate_client, validate_headers, validate_method
+from .validators import (
+    validate_client,
+    validate_headers,
+    validate_method,
+)
 
 import httpx
 
 from httpx import Client
 
+
 def merge_headers(
     original_headers: dict[str, str] = default_headers,
     update_vals: dict[str, str] = None,
 ) -> dict[str, str]:
     """Merge header dicts into new headers dict."""
     validate_headers(original_headers)
     validate_headers(update_vals)
```

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/__init__.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/constants.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/enums.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/enums.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/sinks.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/sinks.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/loguru_utils/validators.py` & `red_utils-0.2.9/red_utils/ext/loguru_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/msgpack_utils/classes.py` & `red_utils-0.2.9/red_utils/ext/msgpack_utils/classes.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/msgpack_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/msgpack_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/pendulum_utils/operations.py` & `red_utils-0.2.9/red_utils/ext/pendulum_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/pydantic_utils/parsers.py` & `red_utils-0.2.9/red_utils/ext/pydantic_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/__init__.py` & `red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/base.py` & `red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/base.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/connection_models.py` & `red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/connection_models.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/custom_types.py` & `red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/ext/sqlalchemy_utils/utils.py` & `red_utils-0.2.9/red_utils/ext/sqlalchemy_utils/utils.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/context_managers/benchmarks/fn_benchmarks.py` & `red_utils-0.2.9/red_utils/std/context_managers/benchmarks/fn_benchmarks.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/context_managers/database_managers/sqlite_managers.py` & `red_utils-0.2.9/red_utils/std/context_managers/database_managers/sqlite_managers.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/context_managers/object_managers/protect.py` & `red_utils-0.2.9/red_utils/std/context_managers/object_managers/protect.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/dataclass_mixins/mixins.py` & `red_utils-0.2.9/red_utils/std/dataclass_mixins/mixins.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/dict_utils/operations.py` & `red_utils-0.2.9/red_utils/std/dict_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/hash_utils/operations.py` & `red_utils-0.2.9/red_utils/std/hash_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/time_utils/operations.py` & `red_utils-0.2.9/red_utils/std/time_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/uuid_utils/operations.py` & `red_utils-0.2.9/red_utils/std/uuid_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils/std/uuid_utils/validators.py` & `red_utils-0.2.9/red_utils/std/uuid_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/red_utils.egg-info/PKG-INFO` & `red_utils-0.2.9/red_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of utility scripts/functions that I use frequently.
 Author-email: redjax <none@none.com>, redjax <jackenyon@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/redjax/red-utils
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: diskcache>=5.6.1
```

### Comparing `red_utils-0.2.8/red_utils.egg-info/SOURCES.txt` & `red_utils-0.2.9/red_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 red_utils/__main__.py
 red_utils.egg-info/PKG-INFO
 red_utils.egg-info/SOURCES.txt
 red_utils.egg-info/dependency_links.txt
 red_utils.egg-info/requires.txt
 red_utils.egg-info/top_level.txt
 red_utils/core/__init__.py
+red_utils/core/constants.py
 red_utils/core/dataclass_utils/__init__.py
 red_utils/core/dataclass_utils/mixins/__init__.py
 red_utils/core/dataclass_utils/mixins/mixin_classes.py
 red_utils/domain/__init__.py
 red_utils/exc/__init__.py
 red_utils/exc/base.py
 red_utils/exc/generic.py
@@ -37,14 +38,15 @@
 red_utils/ext/fastapi_utils/healthcheck.py
 red_utils/ext/fastapi_utils/operations.py
 red_utils/ext/fastapi_utils/tag_definitions.py
 red_utils/ext/fastapi_utils/uvicorn_override.py
 red_utils/ext/fastapi_utils/validators.py
 red_utils/ext/httpx_utils/__init__.py
 red_utils/ext/httpx_utils/__main__.py
+red_utils/ext/httpx_utils/classes.py
 red_utils/ext/httpx_utils/constants.py
 red_utils/ext/httpx_utils/operations.py
 red_utils/ext/httpx_utils/validators.py
 red_utils/ext/loguru_utils/__init__.py
 red_utils/ext/loguru_utils/__main__.py
 red_utils/ext/loguru_utils/constants.py
 red_utils/ext/loguru_utils/enums.py
@@ -83,21 +85,21 @@
 red_utils/std/context_managers/object_managers/protect.py
 red_utils/std/dataclass_mixins/__init__.py
 red_utils/std/dataclass_mixins/mixins.py
 red_utils/std/dict_utils/__init__.py
 red_utils/std/dict_utils/__main__.py
 red_utils/std/dict_utils/operations.py
 red_utils/std/dict_utils/validators.py
-red_utils/std/file_utils/__init__.py
-red_utils/std/file_utils/__main__.py
-red_utils/std/file_utils/constants.py
-red_utils/std/file_utils/operations.py
 red_utils/std/hash_utils/__init__.py
 red_utils/std/hash_utils/__main__.py
 red_utils/std/hash_utils/operations.py
+red_utils/std/path_utils/__init__.py
+red_utils/std/path_utils/__main__.py
+red_utils/std/path_utils/constants.py
+red_utils/std/path_utils/operations.py
 red_utils/std/time_utils/__init__.py
 red_utils/std/time_utils/__main__.py
 red_utils/std/time_utils/constants.py
 red_utils/std/time_utils/operations.py
 red_utils/std/uuid_utils/__init__.py
 red_utils/std/uuid_utils/classes.py
 red_utils/std/uuid_utils/constants.py
```

### Comparing `red_utils-0.2.8/red_utils.egg-info/requires.txt` & `red_utils-0.2.9/red_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `red_utils-0.2.8/tests/test_file_utils.py` & `red_utils-0.2.9/tests/test_file_utils.py`

 * *Files identical despite different names*

