# Comparing `tmp/transstellar-2.5.0.tar.gz` & `tmp/transstellar-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transstellar-2.5.0.tar", max compression
+gzip compressed data, was "transstellar-2.5.1.tar", max compression
```

## Comparing `transstellar-2.5.0.tar` & `transstellar-2.5.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      396 2024-05-30 07:36:29.906963 transstellar-2.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/__init__.py
--rw-r--r--   0        0        0      333 2024-05-23 08:08:58.028344 transstellar-2.5.0/src/transstellar/api_client/__init__.py
--rw-r--r--   0        0        0      474 2024-05-23 08:50:22.393777 transstellar-2.5.0/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6405 2024-05-23 08:50:22.393777 transstellar-2.5.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
--rw-r--r--   0        0        0     3392 2024-05-27 03:39:07.570292 transstellar-2.5.0/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc
--rw-r--r--   0        0        0     4656 2024-05-23 08:08:58.024343 transstellar-2.5.0/src/transstellar/api_client/api_client.py
--rw-r--r--   0        0        0     2436 2024-05-23 10:30:29.487092 transstellar-2.5.0/src/transstellar/api_client/api_resource.py
--rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/api_client/errors/__init__.py
--rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
--rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
--rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.5.0/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/api_client/errors/client_error.py
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/api_client/errors/server_error.py
--rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/api_client/errors/unauthorized_error.py
--rw-r--r--   0        0        0      905 2024-05-30 07:03:37.204455 transstellar-2.5.0/src/transstellar/framework/__init__.py
--rw-r--r--   0        0        0      971 2024-05-30 07:03:38.472362 transstellar-2.5.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5740 2024-05-22 08:04:44.985764 transstellar-2.5.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc
--rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.5.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
--rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1699 2024-05-30 07:28:21.035505 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
--rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.5.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
--rw-r--r--   0        0        0    12182 2024-05-29 08:58:15.467719 transstellar-2.5.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc
--rw-r--r--   0        0        0      243 2024-05-30 06:59:44.723948 transstellar-2.5.0/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
--rw-r--r--   0        0        0     1111 2024-05-30 07:24:13.244922 transstellar-2.5.0/src/transstellar/framework/__pycache__/handle_page_error.cpython-312.pyc
--rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.5.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
--rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.5.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
--rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.5.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
--rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.5.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
--rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.5.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc
--rw-r--r--   0        0        0      681 2024-05-30 07:24:13.244922 transstellar-2.5.0/src/transstellar/framework/__pycache__/page_decorator_meta.cpython-312.pyc
--rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.5.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc
--rw-r--r--   0        0        0     2467 2024-05-23 06:46:43.216136 transstellar-2.5.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0     3177 2024-05-21 10:39:38.120518 transstellar-2.5.0/src/transstellar/framework/application.py
--rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.5.0/src/transstellar/framework/application_bootstrapper.py
--rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/framework/base_api_test.py
--rw-r--r--   0        0        0      648 2024-05-30 07:34:23.091092 transstellar-2.5.0/src/transstellar/framework/base_page.py
--rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.5.0/src/transstellar/framework/base_test.py
--rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.5.0/src/transstellar/framework/base_ui_test.py
--rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/framework/config_service.py
--rw-r--r--   0        0        0     7714 2024-05-29 03:50:01.743149 transstellar-2.5.0/src/transstellar/framework/element.py
--rw-r--r--   0        0        0      127 2024-05-30 06:57:03.509178 transstellar-2.5.0/src/transstellar/framework/handle_error.py
--rw-r--r--   0        0        0      544 2024-05-30 07:24:08.065177 transstellar-2.5.0/src/transstellar/framework/handle_page_error.py
--rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.5.0/src/transstellar/framework/handle_ui_error.py
--rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/framework/loggable.py
--rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.5.0/src/transstellar/framework/logger.py
--rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.5.0/src/transstellar/framework/main_config.py
--rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.5.0/src/transstellar/framework/module.py
--rw-r--r--   0        0        0      202 2024-05-30 07:22:54.292639 transstellar-2.5.0/src/transstellar/framework/page_decorator_meta.py
--rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.5.0/src/transstellar/framework/router.py
--rw-r--r--   0        0        0     1374 2024-05-23 06:42:34.553784 transstellar-2.5.0/src/transstellar/framework/utils.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      396 2024-05-30 09:34:27.930884 transstellar-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-23 08:08:58.028344 transstellar-2.5.1/src/transstellar/api_client/__init__.py
+-rw-r--r--   0        0        0      474 2024-05-23 08:50:22.393777 transstellar-2.5.1/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6405 2024-05-23 08:50:22.393777 transstellar-2.5.1/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
+-rw-r--r--   0        0        0     3392 2024-05-27 03:39:07.570292 transstellar-2.5.1/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc
+-rw-r--r--   0        0        0     4656 2024-05-23 08:08:58.024343 transstellar-2.5.1/src/transstellar/api_client/api_client.py
+-rw-r--r--   0        0        0     2436 2024-05-23 10:30:29.487092 transstellar-2.5.1/src/transstellar/api_client/api_resource.py
+-rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/api_client/errors/__init__.py
+-rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
+-rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
+-rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.5.1/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/api_client/errors/client_error.py
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/api_client/errors/server_error.py
+-rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/api_client/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      905 2024-05-30 07:03:37.204455 transstellar-2.5.1/src/transstellar/framework/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-30 07:03:38.472362 transstellar-2.5.1/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5740 2024-05-22 08:04:44.985764 transstellar-2.5.1/src/transstellar/framework/__pycache__/application.cpython-312.pyc
+-rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.5.1/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
+-rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1658 2024-05-30 09:25:51.565444 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
+-rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.5.1/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
+-rw-r--r--   0        0        0    12182 2024-05-29 08:58:15.467719 transstellar-2.5.1/src/transstellar/framework/__pycache__/element.cpython-312.pyc
+-rw-r--r--   0        0        0      243 2024-05-30 06:59:44.723948 transstellar-2.5.1/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
+-rw-r--r--   0        0        0     1167 2024-05-30 09:31:02.429628 transstellar-2.5.1/src/transstellar/framework/__pycache__/handle_page_error.cpython-312.pyc
+-rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.5.1/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
+-rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.5.1/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
+-rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.5.1/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
+-rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.5.1/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
+-rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.5.1/src/transstellar/framework/__pycache__/module.cpython-312.pyc
+-rw-r--r--   0        0        0      681 2024-05-30 07:24:13.244922 transstellar-2.5.1/src/transstellar/framework/__pycache__/page_decorator_meta.cpython-312.pyc
+-rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.5.1/src/transstellar/framework/__pycache__/router.cpython-312.pyc
+-rw-r--r--   0        0        0     2467 2024-05-23 06:46:43.216136 transstellar-2.5.1/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0     3177 2024-05-21 10:39:38.120518 transstellar-2.5.1/src/transstellar/framework/application.py
+-rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.5.1/src/transstellar/framework/application_bootstrapper.py
+-rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/framework/base_api_test.py
+-rw-r--r--   0        0        0      648 2024-05-30 09:25:28.333479 transstellar-2.5.1/src/transstellar/framework/base_page.py
+-rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.5.1/src/transstellar/framework/base_test.py
+-rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.5.1/src/transstellar/framework/base_ui_test.py
+-rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/framework/config_service.py
+-rw-r--r--   0        0        0     7714 2024-05-29 03:50:01.743149 transstellar-2.5.1/src/transstellar/framework/element.py
+-rw-r--r--   0        0        0      127 2024-05-30 06:57:03.509178 transstellar-2.5.1/src/transstellar/framework/handle_error.py
+-rw-r--r--   0        0        0      569 2024-05-30 09:31:01.177619 transstellar-2.5.1/src/transstellar/framework/handle_page_error.py
+-rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.5.1/src/transstellar/framework/handle_ui_error.py
+-rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/framework/loggable.py
+-rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.5.1/src/transstellar/framework/logger.py
+-rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.5.1/src/transstellar/framework/main_config.py
+-rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.5.1/src/transstellar/framework/module.py
+-rw-r--r--   0        0        0      202 2024-05-30 07:22:54.292639 transstellar-2.5.1/src/transstellar/framework/page_decorator_meta.py
+-rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.5.1/src/transstellar/framework/router.py
+-rw-r--r--   0        0        0     1374 2024-05-23 06:42:34.553784 transstellar-2.5.1/src/transstellar/framework/utils.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.5.1/PKG-INFO
```

### Comparing `transstellar-2.5.0/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/api_client/api_client.py` & `transstellar-2.5.1/src/transstellar/api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/api_client/api_resource.py` & `transstellar-2.5.1/src/transstellar/api_client/api_resource.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__init__.py` & `transstellar-2.5.1/src/transstellar/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/application.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/application.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu May 30 07:28:17 2024 UTC, .py size: 720 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-00000000: cb0d 0d0a 0000 0000 912a 5866 d002 0000  .........*Xf....
+00000000: cb0d 0d0a 0000 0000 0846 5866 8802 0000  .........FXf....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
-00000020: 0000 0000 00f3 5a00 0000 9700 6400 6401  ......Z.....d.d.
+00000020: 0000 0000 00f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
-00000050: 6404 6405 6c06 6d07 5a07 0100 6404 6406  d.d.l.m.Z...d.d.
-00000060: 6c08 6d08 5a08 0100 0200 4700 6407 8400  l.m.Z.....G.d...
-00000070: 6408 6507 6505 ac09 ab04 0000 0000 0000  d.e.e...........
-00000080: 5a09 7901 290a e900 0000 004e 2902 da0b  Z.y.)......N)...
-00000090: 5061 7273 6552 6573 756c 74da 0875 726c  ParseResult..url
-000000a0: 7061 7273 6529 01da 1150 6167 6544 6563  parse)...PageDec
-000000b0: 6f72 6174 6f72 4d65 7461 e901 0000 0029  oratorMeta.....)
-000000c0: 01da 0745 6c65 6d65 6e74 2901 da11 6861  ...Element)...ha
-000000d0: 6e64 6c65 5f70 6167 655f 6572 726f 7263  ndle_page_errorc
-000000e0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-000000f0: 0000 0000 f334 0000 0097 0065 005a 0164  .....4.....e.Z.d
-00000100: 005a 0264 015a 0364 0265 0466 0264 0384  .Z.d.Z.d.e.f.d..
-00000110: 045a 0564 0484 005a 0664 0584 005a 0764  .Z.d...Z.d...Z.d
-00000120: 0665 0866 0264 0784 045a 0979 0829 09da  .e.f.d...Z.y.)..
-00000130: 0842 6173 6550 6167 657a 062f 2f62 6f64  .BasePagez.//bod
-00000140: 79da 0375 726c 6302 0000 0000 0000 0000  y..urlc.........
-00000150: 0000 0003 0000 0003 0000 00f3 5c00 0000  ............\...
-00000160: 9700 7c00 6a00 0000 0000 0000 0000 0000  ..|.j...........
-00000170: 0000 0000 0000 0000 6a03 0000 0000 0000  ........j.......
-00000180: 0000 0000 0000 0000 0000 0000 7c01 ab01  ............|...
-00000190: 0000 0000 0000 0100 7c00 6a05 0000 0000  ........|.j.....
-000001a0: 0000 0000 0000 0000 0000 0000 0000 6400  ..............d.
-000001b0: ab01 0000 0000 0000 0100 7900 a901 4e29  ..........y...N)
-000001c0: 03da 0664 7269 7665 72da 0367 6574 da17  ...driver..get..
-000001d0: 7365 745f 6375 7272 656e 745f 646f 6d5f  set_current_dom_
-000001e0: 656c 656d 656e 7429 02da 0473 656c 6672  element)...selfr
-000001f0: 0b00 0000 7302 0000 0020 20fa 302f 7072  ....s....  .0/pr
-00000200: 6f6a 6563 742f 7372 632f 7472 616e 7373  oject/src/transs
-00000210: 7465 6c6c 6172 2f66 7261 6d65 776f 726b  tellar/framework
-00000220: 2f62 6173 655f 7061 6765 2e70 79da 0567  /base_page.py..g
-00000230: 6f5f 746f 7a0e 4261 7365 5061 6765 2e67  o_toz.BasePage.g
-00000240: 6f5f 746f 0e00 0000 7320 0000 0080 00d8  o_to....s ......
-00000250: 080c 8f0b 890b 8f0f 890f 9803 d408 1ce0  ................
-00000260: 080c d708 24d1 0824 a054 d508 2af3 0000  ....$..$.T..*...
-00000270: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000280: 0000 0003 0000 00f3 2600 0000 9700 0200  ........&.......
-00000290: 7c01 7c00 6a00 0000 0000 0000 0000 0000  |.|.j...........
-000002a0: 0000 0000 0000 0000 ab01 0000 0000 0000  ................
-000002b0: 5300 720d 0000 0029 01da 0361 7070 2902  S.r....)...app).
-000002c0: 7211 0000 00da 0a70 6167 655f 636c 6173  r......page_clas
-000002d0: 7373 0200 0000 2020 7212 0000 00da 0867  ss....  r......g
-000002e0: 6574 5f70 6167 657a 1142 6173 6550 6167  et_pagez.BasePag
-000002f0: 652e 6765 745f 7061 6765 1300 0000 7311  e.get_page....s.
-00000300: 0000 0080 00d9 0f19 9824 9f28 9928 d30f  .........$.(.(..
-00000310: 23d0 0823 7214 0000 0063 0300 0000 0000  #..#r....c......
-00000320: 0000 0000 0000 0500 0000 0300 0000 f35c  ...............\
-00000330: 0000 0097 0002 0074 0100 0000 0000 0000  .......t........
-00000340: 0074 0200 0000 0000 0000 006a 0400 0000  .t.........j....
-00000350: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00000360: 0119 0000 007c 02ab 0200 0000 0000 007c  .....|.........|
-00000370: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
-00000380: 0000 0000 00ab 0100 0000 0000 0053 0072  .............S.r
-00000390: 0d00 0000 2904 da07 6765 7461 7474 72da  ....)...getattr.
-000003a0: 0373 7973 da07 6d6f 6475 6c65 7372 1600  .sys..modulesr..
-000003b0: 0000 2903 7211 0000 00da 066d 6f64 756c  ..).r......modul
-000003c0: 6572 1700 0000 7303 0000 0020 2020 7212  er....s....   r.
-000003d0: 0000 00da 1467 6574 5f70 6167 655f 6672  .....get_page_fr
-000003e0: 6f6d 5f6d 6f64 756c 657a 1d42 6173 6550  om_modulez.BaseP
-000003f0: 6167 652e 6765 745f 7061 6765 5f66 726f  age.get_page_fro
-00000400: 6d5f 6d6f 6475 6c65 1600 0000 7323 0000  m_module....s#..
-00000410: 0080 00d8 0f37 8c77 9473 977b 917b a036  .....7.w.s.{.{.6
-00000420: d117 2aa8 4ad3 0f37 b804 bf08 b908 d30f  ..*.J..7........
-00000430: 41d0 0841 7214 0000 00da 0672 6574 7572  A..Ar......retur
-00000440: 6e63 0100 0000 0000 0000 0000 0000 0300  nc..............
-00000450: 0000 0300 0000 f354 0000 0097 0074 0100  .......T.....t..
-00000460: 0000 0000 0000 007c 006a 0200 0000 0000  .......|.j......
-00000470: 0000 0000 0000 0000 0000 0000 006a 0400  .............j..
-00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000490: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
-000004a0: 0000 0000 00ab 0100 0000 0000 0053 0072  .............S.r
-000004b0: 0d00 0000 2904 7204 0000 0072 1600 0000  ....).r....r....
-000004c0: 720e 0000 00da 0b63 7572 7265 6e74 5f75  r......current_u
-000004d0: 726c 2901 7211 0000 0073 0100 0000 2072  rl).r....s.... r
-000004e0: 1200 0000 da0f 6765 745f 6375 7272 656e  ......get_curren
-000004f0: 745f 7572 6c7a 1842 6173 6550 6167 652e  t_urlz.BasePage.
-00000500: 6765 745f 6375 7272 656e 745f 7572 6c19  get_current_url.
-00000510: 0000 0073 1b00 0000 8000 dc0f 1798 049f  ...s............
-00000520: 0899 089f 0f99 0fd7 1833 d118 33d3 0f34  .........3..3..4
-00000530: d008 3472 1400 0000 4e29 0ada 085f 5f6e  ..4r....N)...__n
-00000540: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000550: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000560: 0d58 5041 5448 5f43 5552 5245 4e54 da03  .XPATH_CURRENT..
-00000570: 7374 7272 1300 0000 7218 0000 0072 1e00  strr....r....r..
-00000580: 0000 7203 0000 0072 2200 0000 a900 7214  ..r....r".....r.
-00000590: 0000 0072 1200 0000 720a 0000 0072 0a00  ...r....r....r..
-000005a0: 0000 0b00 0000 732a 0000 0084 00d8 141c  ......s*........
-000005b0: 804d f004 0305 2b98 13f3 0003 052b f20a  .M....+......+..
-000005c0: 0105 24f2 0601 0542 01f0 0601 0535 a01b  ..$....B.....5..
-000005d0: f400 0105 3572 1400 0000 720a 0000 0029  ....5r....r....)
-000005e0: 01da 096d 6574 6163 6c61 7373 290a 721b  ...metaclass).r.
-000005f0: 0000 00da 0c75 726c 6c69 622e 7061 7273  .....urllib.pars
-00000600: 6572 0300 0000 7204 0000 00da 2a74 7261  er....r.....*tra
-00000610: 6e73 7374 656c 6c61 722e 6672 616d 6577  nsstellar.framew
-00000620: 6f72 6b2e 7061 6765 5f64 6563 6f72 6174  ork.page_decorat
-00000630: 6f72 5f6d 6574 6172 0500 0000 da07 656c  or_metar......el
-00000640: 656d 656e 7472 0700 0000 7208 0000 0072  ementr....r....r
-00000650: 0a00 0000 7228 0000 0072 1400 0000 7212  ....r(...r....r.
-00000660: 0000 00fa 083c 6d6f 6475 6c65 3e72 2d00  .....<module>r-.
-00000670: 0000 0100 0000 7323 0000 00f0 0301 0101  ......s#........
-00000680: db00 0adf 002e e500 48e5 001c dd00 30f4  ........H.....0.
-00000690: 080f 0135 8877 d022 33f6 000f 0135 7214  ...5.w."3....5r.
-000006a0: 0000 00                                  ...
+00000050: 6404 6405 6c06 6d07 5a07 0100 0200 4700  d.d.l.m.Z.....G.
+00000060: 6406 8400 6407 6507 6505 ac08 ab04 0000  d...d.e.e.......
+00000070: 0000 0000 5a08 7901 2909 e900 0000 004e  ....Z.y.)......N
+00000080: 2902 da0b 5061 7273 6552 6573 756c 74da  )...ParseResult.
+00000090: 0875 726c 7061 7273 6529 01da 1150 6167  .urlparse)...Pag
+000000a0: 6544 6563 6f72 6174 6f72 4d65 7461 e901  eDecoratorMeta..
+000000b0: 0000 0029 01da 0745 6c65 6d65 6e74 6300  ...)...Elementc.
+000000c0: 0000 0000 0000 0000 0000 0002 0000 0000  ................
+000000d0: 0000 00f3 3400 0000 9700 6500 5a01 6400  ....4.....e.Z.d.
+000000e0: 5a02 6401 5a03 6402 6504 6602 6403 8404  Z.d.Z.d.e.f.d...
+000000f0: 5a05 6404 8400 5a06 6405 8400 5a07 6406  Z.d...Z.d...Z.d.
+00000100: 6508 6602 6407 8404 5a09 7908 2909 da08  e.f.d...Z.y.)...
+00000110: 4261 7365 5061 6765 7a06 2f2f 626f 6479  BasePagez.//body
+00000120: da03 7572 6c63 0200 0000 0000 0000 0000  ..urlc..........
+00000130: 0000 0300 0000 0300 0000 f35c 0000 0097  ...........\....
+00000140: 007c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00000150: 0000 0000 0000 006a 0300 0000 0000 0000  .......j........
+00000160: 0000 0000 0000 0000 0000 007c 01ab 0100  ...........|....
+00000170: 0000 0000 0001 007c 006a 0500 0000 0000  .......|.j......
+00000180: 0000 0000 0000 0000 0000 0000 0064 00ab  .............d..
+00000190: 0100 0000 0000 0001 0079 00a9 014e 2903  .........y...N).
+000001a0: da06 6472 6976 6572 da03 6765 74da 1773  ..driver..get..s
+000001b0: 6574 5f63 7572 7265 6e74 5f64 6f6d 5f65  et_current_dom_e
+000001c0: 6c65 6d65 6e74 2902 da04 7365 6c66 720a  lement)...selfr.
+000001d0: 0000 0073 0200 0000 2020 fa30 2f70 726f  ...s....  .0/pro
+000001e0: 6a65 6374 2f73 7263 2f74 7261 6e73 7374  ject/src/transst
+000001f0: 656c 6c61 722f 6672 616d 6577 6f72 6b2f  ellar/framework/
+00000200: 6261 7365 5f70 6167 652e 7079 da05 676f  base_page.py..go
+00000210: 5f74 6f7a 0e42 6173 6550 6167 652e 676f  _toz.BasePage.go
+00000220: 5f74 6f0c 0000 0073 2000 0000 8000 d808  _to....s .......
+00000230: 0c8f 0b89 0b8f 0f89 0f98 03d4 081c e008  ................
+00000240: 0cd7 0824 d108 24a0 54d5 082a f300 0000  ...$..$.T..*....
+00000250: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00000260: 0000 0300 0000 f326 0000 0097 0002 007c  .......&.......|
+00000270: 017c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00000280: 0000 0000 0000 00ab 0100 0000 0000 0053  ...............S
+00000290: 0072 0c00 0000 2901 da03 6170 7029 0272  .r....)...app).r
+000002a0: 1000 0000 da0a 7061 6765 5f63 6c61 7373  ......page_class
+000002b0: 7302 0000 0020 2072 1100 0000 da08 6765  s....  r......ge
+000002c0: 745f 7061 6765 7a11 4261 7365 5061 6765  t_pagez.BasePage
+000002d0: 2e67 6574 5f70 6167 6511 0000 0073 1100  .get_page....s..
+000002e0: 0000 8000 d90f 1998 249f 2899 28d3 0f23  ........$.(.(..#
+000002f0: d008 2372 1300 0000 6303 0000 0000 0000  ..#r....c.......
+00000300: 0000 0000 0005 0000 0003 0000 00f3 5c00  ..............\.
+00000310: 0000 9700 0200 7401 0000 0000 0000 0000  ......t.........
+00000320: 7402 0000 0000 0000 0000 6a04 0000 0000  t.........j.....
+00000330: 0000 0000 0000 0000 0000 0000 0000 7c01  ..............|.
+00000340: 1900 0000 7c02 ab02 0000 0000 0000 7c00  ....|.........|.
+00000350: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+00000360: 0000 0000 ab01 0000 0000 0000 5300 720c  ............S.r.
+00000370: 0000 0029 04da 0767 6574 6174 7472 da03  ...)...getattr..
+00000380: 7379 73da 076d 6f64 756c 6573 7215 0000  sys..modulesr...
+00000390: 0029 0372 1000 0000 da06 6d6f 6475 6c65  .).r......module
+000003a0: 7216 0000 0073 0300 0000 2020 2072 1100  r....s....   r..
+000003b0: 0000 da14 6765 745f 7061 6765 5f66 726f  ....get_page_fro
+000003c0: 6d5f 6d6f 6475 6c65 7a1d 4261 7365 5061  m_modulez.BasePa
+000003d0: 6765 2e67 6574 5f70 6167 655f 6672 6f6d  ge.get_page_from
+000003e0: 5f6d 6f64 756c 6514 0000 0073 2300 0000  _module....s#...
+000003f0: 8000 d80f 378c 7794 7397 7b91 7ba0 36d1  ....7.w.s.{.{.6.
+00000400: 172a a84a d30f 37b8 04bf 08b9 08d3 0f41  .*.J..7........A
+00000410: d008 4172 1300 0000 da06 7265 7475 726e  ..Ar......return
+00000420: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000430: 0003 0000 00f3 5400 0000 9700 7401 0000  ......T.....t...
+00000440: 0000 0000 0000 7c00 6a02 0000 0000 0000  ......|.j.......
+00000450: 0000 0000 0000 0000 0000 0000 6a04 0000  ............j...
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+00000480: 0000 0000 ab01 0000 0000 0000 5300 720c  ............S.r.
+00000490: 0000 0029 0472 0400 0000 7215 0000 0072  ...).r....r....r
+000004a0: 0d00 0000 da0b 6375 7272 656e 745f 7572  ......current_ur
+000004b0: 6c29 0172 1000 0000 7301 0000 0020 7211  l).r....s.... r.
+000004c0: 0000 00da 0f67 6574 5f63 7572 7265 6e74  .....get_current
+000004d0: 5f75 726c 7a18 4261 7365 5061 6765 2e67  _urlz.BasePage.g
+000004e0: 6574 5f63 7572 7265 6e74 5f75 726c 1700  et_current_url..
+000004f0: 0000 731b 0000 0080 00dc 0f17 9804 9f08  ..s.............
+00000500: 9908 9f0f 990f d718 33d1 1833 d30f 34d0  ........3..3..4.
+00000510: 0834 7213 0000 004e 290a da08 5f5f 6e61  .4r....N)...__na
+00000520: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000530: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0d  ..__qualname__..
+00000540: 5850 4154 485f 4355 5252 454e 54da 0373  XPATH_CURRENT..s
+00000550: 7472 7212 0000 0072 1700 0000 721d 0000  trr....r....r...
+00000560: 0072 0300 0000 7221 0000 00a9 0072 1300  .r....r!.....r..
+00000570: 0000 7211 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000580: 0009 0000 0073 2a00 0000 8400 d814 1c80  .....s*.........
+00000590: 4df0 0403 052b 9813 f300 0305 2bf2 0a01  M....+......+...
+000005a0: 0524 f206 0105 4201 f006 0105 35a0 1bf4  .$....B.....5...
+000005b0: 0001 0535 7213 0000 0072 0900 0000 2901  ...5r....r....).
+000005c0: da09 6d65 7461 636c 6173 7329 0972 1a00  ..metaclass).r..
+000005d0: 0000 da0c 7572 6c6c 6962 2e70 6172 7365  ....urllib.parse
+000005e0: 7203 0000 0072 0400 0000 da2a 7472 616e  r....r.....*tran
+000005f0: 7373 7465 6c6c 6172 2e66 7261 6d65 776f  sstellar.framewo
+00000600: 726b 2e70 6167 655f 6465 636f 7261 746f  rk.page_decorato
+00000610: 725f 6d65 7461 7205 0000 00da 0765 6c65  r_metar......ele
+00000620: 6d65 6e74 7207 0000 0072 0900 0000 7227  mentr....r....r'
+00000630: 0000 0072 1300 0000 7211 0000 00fa 083c  ...r....r......<
+00000640: 6d6f 6475 6c65 3e72 2c00 0000 0100 0000  module>r,.......
+00000650: 7320 0000 00f0 0301 0101 db00 0adf 002e  s ..............
+00000660: e500 48e5 001c f406 0f01 3588 77d0 2233  ..H.......5.w."3
+00000670: f600 0f01 3572 1300 0000                 ....5r....
```

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/element.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/handle_page_error.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/handle_page_error.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu May 30 07:24:08 2024 UTC, .py size: 544 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,73 @@
-00000000: cb0d 0d0a 0000 0000 9829 5866 2002 0000  .........)Xf ...
-00000010: e300 0000 0000 0000 0000 0000 0001 0000  ................
-00000020: 0000 0000 00f3 1000 0000 9700 6400 8400  ............d...
-00000030: 5a00 6401 8400 5a01 7902 2903 6301 0000  Z.d...Z.y.).c...
-00000040: 0000 0000 0000 0000 0008 0000 0003 0000  ................
-00000050: 00f3 b000 0000 9700 7401 0000 0000 0000  ........t.......
-00000060: 0000 7c00 ab01 0000 0000 0000 6a03 0000  ..|.........j...
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: ab00 0000 0000 0000 4400 5d39 0000 5c02  ........D.]9..\.
-00000090: 0000 7d01 7d02 7405 0000 0000 0000 0000  ..}.}.t.........
-000000a0: 7c02 ab01 0000 0000 0000 7301 8c12 7c01  |.........s...|.
-000000b0: 6a07 0000 0000 0000 0000 0000 0000 0000  j...............
-000000c0: 0000 0000 6401 ab01 0000 0000 0000 7201  ....d.........r.
-000000d0: 8c24 7409 0000 0000 0000 0000 7c00 7c01  .$t.........|.|.
-000000e0: 740b 0000 0000 0000 0000 7c02 ab01 0000  t.........|.....
-000000f0: 0000 0000 ab03 0000 0000 0000 0100 8c3b  ...............;
-00000100: 0400 7c00 5300 2902 4eda 025f 5f29 06da  ..|.S.).N..__)..
-00000110: 0476 6172 73da 0569 7465 6d73 da08 6361  .vars..items..ca
-00000120: 6c6c 6162 6c65 da0a 7374 6172 7473 7769  llable..startswi
-00000130: 7468 da07 7365 7461 7474 72da 1268 616e  th..setattr..han
-00000140: 646c 655f 7061 6765 5f65 7272 6f72 7329  dle_page_errors)
-00000150: 03da 0363 6c73 da04 6e61 6d65 da06 6d65  ...cls..name..me
-00000160: 7468 6f64 7303 0000 0020 2020 fa38 2f70  thods....   .8/p
-00000170: 726f 6a65 6374 2f73 7263 2f74 7261 6e73  roject/src/trans
-00000180: 7374 656c 6c61 722f 6672 616d 6577 6f72  stellar/framewor
-00000190: 6b2f 6861 6e64 6c65 5f70 6167 655f 6572  k/handle_page_er
-000001a0: 726f 722e 7079 da11 6861 6e64 6c65 5f70  ror.py..handle_p
-000001b0: 6167 655f 6572 726f 7272 0e00 0000 0100  age_errorr......
-000001c0: 0000 7350 0000 0080 00dc 181c 9853 9b09  ..sP.........S..
-000001d0: 9f0f 990f d318 29f2 0006 050e 890c 8804  ......).........
-000001e0: 8866 dc0b 1390 46d5 0b1b a044 a74f a14f  .f....F....D.O.O
-000001f0: b044 d524 39dc 0c13 d810 13d8 1014 dc10  .D.$9...........
-00000200: 22a0 36d3 102a f507 040d 0ef0 0506 050e  ".6..*..........
-00000210: f010 000c 0f80 4af3 0000 0000 6301 0000  ......J.....c...
-00000220: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000230: 00f3 1200 0000 8700 9700 8800 6601 6401  ............f.d.
-00000240: 8408 7d01 7c01 5300 2902 4e63 0000 0000  ..}.|.S.).Nc....
-00000250: 0000 0000 0000 0000 0500 0000 1f00 0000  ................
-00000260: f36e 0000 0095 0197 0009 0002 0089 047c  .n.............|
-00000270: 0069 007c 01a4 018e 017d 027c 0253 0023  .i.|.....}.|.S.#
-00000280: 0074 0000 0000 0000 0000 0024 0072 1e7d  .t.........$.r.}
-00000290: 0374 0300 0000 0000 0000 0064 0189 046a  .t.........d...j
-000002a0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 009b 009d 02ab 0100 0000 0000 007c  ...............|
-000002c0: 0382 0264 007d 037e 0377 0177 0078 0359  ...d.}.~.w.w.x.Y
-000002d0: 0077 0129 024e 7a0d 556e 6162 6c65 2074  .w.).Nz.Unable t
-000002e0: 6f20 646f 2029 03da 0945 7863 6570 7469  o do )...Excepti
-000002f0: 6f6e da0c 5275 6e74 696d 6545 7272 6f72  on..RuntimeError
-00000300: da08 5f5f 6e61 6d65 5f5f 2905 da04 6172  ..__name__)...ar
-00000310: 6773 da06 6b77 6172 6773 da06 7265 7375  gs..kwargs..resu
-00000320: 6c74 da01 6572 0c00 0000 7305 0000 0020  lt..er....s.... 
-00000330: 2020 2080 720d 0000 00da 0777 7261 7070     .r......wrapp
-00000340: 6572 7a23 6861 6e64 6c65 5f70 6167 655f  erz#handle_page_
-00000350: 6572 726f 7273 2e3c 6c6f 6361 6c73 3e2e  errors.<locals>.
-00000360: 7772 6170 7065 720e 0000 0073 4800 0000  wrapper....sH...
-00000370: f880 00f0 0204 0949 01d9 151b 9854 d015  .......I.....T..
-00000380: 2ca0 56d1 152c 8846 d813 1988 4df8 dc0f  ,.V..,.F....M...
-00000390: 18f2 0001 0949 01dc 121e a01d a876 af7f  .....I.......v..
-000003a0: a97f d02e 3fd0 1f40 d312 41c0 71d0 0c48  ....?..@..A.q..H
-000003b0: fbf0 0301 0949 01fa 7310 0000 0083 090d  .....I..s.......
-000003c0: 008d 0934 0396 192f 03af 0534 03a9 0029  ...4.../...4...)
-000003d0: 0272 0c00 0000 7219 0000 0073 0200 0000  .r....r....s....
-000003e0: 6020 720d 0000 0072 0900 0000 7209 0000  ` r....r....r...
-000003f0: 000d 0000 0073 1000 0000 f880 00f4 0205  .....s..........
-00000400: 0549 01f0 0e00 0c13 804e 720f 0000 004e  .I.......Nr....N
-00000410: 2902 720e 0000 0072 0900 0000 721a 0000  ).r....r....r...
-00000420: 0072 0f00 0000 720d 0000 00fa 083c 6d6f  .r....r......<mo
-00000430: 6475 6c65 3e72 1b00 0000 0100 0000 730f  dule>r........s.
-00000440: 0000 00f0 0301 0101 f202 0901 0ff3 1808  ................
-00000450: 0113 720f 0000 00                        ..r....
+00000000: cb0d 0d0a 0000 0000 5547 5866 3902 0000  ........UGXf9...
+00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
+00000020: 0000 0000 00f3 1800 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 6402 8400 5a01 6403 8400 5a02  l.Z.d...Z.d...Z.
+00000040: 7901 2904 e900 0000 004e 6301 0000 0000  y.)......Nc.....
+00000050: 0000 0000 0000 0008 0000 0003 0000 00f3  ................
+00000060: c400 0000 9700 7401 0000 0000 0000 0000  ......t.........
+00000070: 7c00 ab01 0000 0000 0000 6a03 0000 0000  |.........j.....
+00000080: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
+00000090: 0000 0000 0000 4400 5d43 0000 5c02 0000  ......D.]C..\...
+000000a0: 7d01 7d02 7405 0000 0000 0000 0000 6a06  }.}.t.........j.
+000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000c0: 0000 7c02 ab01 0000 0000 0000 7301 8c1c  ..|.........s...
+000000d0: 7c01 6a09 0000 0000 0000 0000 0000 0000  |.j.............
+000000e0: 0000 0000 0000 6401 ab01 0000 0000 0000  ......d.........
+000000f0: 7201 8c2e 740b 0000 0000 0000 0000 7c00  r...t.........|.
+00000100: 7c01 740d 0000 0000 0000 0000 7c02 ab01  |.t.........|...
+00000110: 0000 0000 0000 ab03 0000 0000 0000 0100  ................
+00000120: 8c45 0400 7c00 5300 2902 4eda 025f 5f29  .E..|.S.).N..__)
+00000130: 07da 0476 6172 73da 0569 7465 6d73 da07  ...vars..items..
+00000140: 696e 7370 6563 74da 0869 736d 6574 686f  inspect..ismetho
+00000150: 64da 0a73 7461 7274 7377 6974 68da 0773  d..startswith..s
+00000160: 6574 6174 7472 da12 6861 6e64 6c65 5f70  etattr..handle_p
+00000170: 6167 655f 6572 726f 7273 2903 da03 636c  age_errors)...cl
+00000180: 73da 046e 616d 65da 066d 6574 686f 6473  s..name..methods
+00000190: 0300 0000 2020 20fa 382f 7072 6f6a 6563  ....   .8/projec
+000001a0: 742f 7372 632f 7472 616e 7373 7465 6c6c  t/src/transstell
+000001b0: 6172 2f66 7261 6d65 776f 726b 2f68 616e  ar/framework/han
+000001c0: 646c 655f 7061 6765 5f65 7272 6f72 2e70  dle_page_error.p
+000001d0: 79da 1168 616e 646c 655f 7061 6765 5f65  y..handle_page_e
+000001e0: 7272 6f72 7210 0000 0004 0000 0073 5600  rrorr........sV.
+000001f0: 0000 8000 dc18 1c98 539b 099f 0f99 0fd3  ........S.......
+00000200: 1829 f200 0605 0e89 0c88 0488 66dc 0b12  .)..........f...
+00000210: d70b 1bd1 0b1b 9846 d50b 23a8 44af 4fa9  .......F..#.D.O.
+00000220: 4fb8 44d5 2c41 dc0c 13d8 1013 d810 14dc  O.D.,A..........
+00000230: 1022 a036 d310 2af5 0704 0d0e f005 0605  .".6..*.........
+00000240: 0ef0 1000 0c0f 804a f300 0000 0063 0100  .......J.....c..
+00000250: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000260: 0000 f312 0000 0087 0097 0088 0066 0164  .............f.d
+00000270: 0184 087d 017c 0153 0029 024e 6300 0000  ...}.|.S.).Nc...
+00000280: 0000 0000 0000 0000 0005 0000 001f 0000  ................
+00000290: 00f3 6e00 0000 9501 9700 0900 0200 8904  ..n.............
+000002a0: 7c00 6900 7c01 a401 8e01 7d02 7c02 5300  |.i.|.....}.|.S.
+000002b0: 2300 7400 0000 0000 0000 0000 2400 721e  #.t.........$.r.
+000002c0: 7d03 7403 0000 0000 0000 0000 6401 8904  }.t.........d...
+000002d0: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
+000002e0: 0000 0000 9b00 9d02 ab01 0000 0000 0000  ................
+000002f0: 7c03 8202 6400 7d03 7e03 7701 7700 7803  |...d.}.~.w.w.x.
+00000300: 5900 7701 2902 4e7a 0d55 6e61 626c 6520  Y.w.).Nz.Unable 
+00000310: 746f 2064 6f20 2903 da09 4578 6365 7074  to do )...Except
+00000320: 696f 6eda 0c52 756e 7469 6d65 4572 726f  ion..RuntimeErro
+00000330: 72da 085f 5f6e 616d 655f 5f29 05da 0461  r..__name__)...a
+00000340: 7267 73da 066b 7761 7267 73da 0672 6573  rgs..kwargs..res
+00000350: 756c 74da 0165 720e 0000 0073 0500 0000  ult..er....s....
+00000360: 2020 2020 8072 0f00 0000 da07 7772 6170      .r......wrap
+00000370: 7065 727a 2368 616e 646c 655f 7061 6765  perz#handle_page
+00000380: 5f65 7272 6f72 732e 3c6c 6f63 616c 733e  _errors.<locals>
+00000390: 2e77 7261 7070 6572 1100 0000 7348 0000  .wrapper....sH..
+000003a0: 00f8 8000 f002 0409 4901 d915 1b98 54d0  ........I.....T.
+000003b0: 152c a056 d115 2c88 46d8 1319 884d f8dc  .,.V..,.F....M..
+000003c0: 0f18 f200 0109 4901 dc12 1ea0 1da8 76af  ......I.......v.
+000003d0: 7fa9 7fd0 2e3f d01f 40d3 1241 c071 d00c  .....?..@..A.q..
+000003e0: 48fb f003 0109 4901 fa73 1000 0000 8309  H.....I..s......
+000003f0: 0d00 8d09 3403 9619 2f03 af05 3403 a900  ....4.../...4...
+00000400: 2902 720e 0000 0072 1b00 0000 7302 0000  ).r....r....s...
+00000410: 0060 2072 0f00 0000 720b 0000 0072 0b00  .` r....r....r..
+00000420: 0000 1000 0000 7310 0000 00f8 8000 f402  ......s.........
+00000430: 0505 4901 f00e 000c 1380 4e72 1100 0000  ..I.......Nr....
+00000440: 2903 7207 0000 0072 1000 0000 720b 0000  ).r....r....r...
+00000450: 0072 1c00 0000 7211 0000 0072 0f00 0000  .r....r....r....
+00000460: fa08 3c6d 6f64 756c 653e 721d 0000 0001  ..<module>r.....
+00000470: 0000 0073 1200 0000 f003 0101 01db 000e  ...s............
+00000480: f206 0901 0ff3 1808 0113 7211 0000 00    ..........r....
```

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/logger.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/logger.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/module.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/module.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/page_decorator_meta.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/page_decorator_meta.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/router.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/router.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/__pycache__/utils.cpython-312.pyc` & `transstellar-2.5.1/src/transstellar/framework/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/application.py` & `transstellar-2.5.1/src/transstellar/framework/application.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/base_page.py` & `transstellar-2.5.1/src/transstellar/framework/base_page.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/base_ui_test.py` & `transstellar-2.5.1/src/transstellar/framework/base_ui_test.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/element.py` & `transstellar-2.5.1/src/transstellar/framework/element.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/handle_ui_error.py` & `transstellar-2.5.1/src/transstellar/framework/handle_ui_error.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/logger.py` & `transstellar-2.5.1/src/transstellar/framework/logger.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/router.py` & `transstellar-2.5.1/src/transstellar/framework/router.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/src/transstellar/framework/utils.py` & `transstellar-2.5.1/src/transstellar/framework/utils.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.5.0/PKG-INFO` & `transstellar-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transstellar
-Version: 2.5.0
+Version: 2.5.1
 Summary: A pytest framework
 Author: Onramplab Dev
 Author-email: dev@onramplab.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: injector (>=0.21.0,<0.22.0)
```

