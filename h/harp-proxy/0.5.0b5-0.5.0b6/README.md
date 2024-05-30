# Comparing `tmp/harp_proxy-0.5.0b5.tar.gz` & `tmp/harp_proxy-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harp_proxy-0.5.0b5.tar", max compression
+gzip compressed data, was "harp_proxy-0.5.0b6.tar", max compression
```

## Comparing `harp_proxy-0.5.0b5.tar` & `harp_proxy-0.5.0b6.tar`

### file list

```diff
@@ -1,204 +1,208 @@
--rw-r--r--   0        0        0     2001 2024-04-01 15:50:33.825795 harp_proxy-0.5.0b5/LICENSE.rst
--rw-r--r--   0        0        0     3940 2024-04-01 15:50:33.826352 harp_proxy-0.5.0b5/README.rst
--rw-r--r--   0        0        0     2959 2024-04-01 15:50:33.851169 harp_proxy-0.5.0b5/harp/__init__.py
--rw-r--r--   0        0        0       85 2024-04-01 15:50:33.851239 harp_proxy-0.5.0b5/harp/__main__.py
--rw-r--r--   0        0        0     2871 2024-04-01 15:50:33.851305 harp_proxy-0.5.0b5/harp/_logging.py
--rw-r--r--   0        0        0       84 2024-04-01 15:50:33.851390 harp_proxy-0.5.0b5/harp/asgi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.851451 harp_proxy-0.5.0b5/harp/asgi/bridge/__init__.py
--rw-r--r--   0        0        0     2874 2024-04-01 15:50:33.851531 harp_proxy-0.5.0b5/harp/asgi/bridge/requests.py
--rw-r--r--   0        0        0     1313 2024-04-01 15:50:33.851593 harp_proxy-0.5.0b5/harp/asgi/bridge/responses.py
--rw-r--r--   0        0        0     2072 2024-04-01 15:50:33.851658 harp_proxy-0.5.0b5/harp/asgi/events.py
--rw-r--r--   0        0        0     6633 2024-04-01 15:50:33.851734 harp_proxy-0.5.0b5/harp/asgi/kernel.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.851794 harp_proxy-0.5.0b5/harp/asgi/tests/__init__.py
--rw-r--r--   0        0        0     6987 2024-04-01 15:50:33.851874 harp_proxy-0.5.0b5/harp/asgi/tests/test_http_bridge_asgi_request.py
--rw-r--r--   0        0        0     1734 2024-04-01 15:50:33.851974 harp_proxy-0.5.0b5/harp/commandline/__init__.py
--rw-r--r--   0        0        0      352 2024-04-01 15:50:33.852040 harp_proxy-0.5.0b5/harp/commandline/install_dev.py
--rw-r--r--   0        0        0     4305 2024-04-01 15:50:33.852116 harp_proxy-0.5.0b5/harp/commandline/start.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.852179 harp_proxy-0.5.0b5/harp/commandline/utils/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-01 15:50:33.852433 harp_proxy-0.5.0b5/harp/commandline/utils/_hacks.py
--rw-r--r--   0        0        0     4794 2024-04-01 15:50:33.852506 harp_proxy-0.5.0b5/harp/commandline/utils/manager.py
--rw-r--r--   0        0        0      538 2024-04-01 15:50:33.852600 harp_proxy-0.5.0b5/harp/config/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.852658 harp_proxy-0.5.0b5/harp/config/adapters/__init__.py
--rw-r--r--   0        0        0      952 2024-04-01 15:50:33.852725 harp_proxy-0.5.0b5/harp/config/adapters/hypercorn.py
--rw-r--r--   0        0        0     2398 2024-04-01 15:50:33.852789 harp_proxy-0.5.0b5/harp/config/application.py
--rw-r--r--   0        0        0    12157 2024-04-01 15:50:33.853090 harp_proxy-0.5.0b5/harp/config/config.py
--rw-r--r--   0        0        0     1533 2024-04-01 15:50:33.853161 harp_proxy-0.5.0b5/harp/config/events.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.853222 harp_proxy-0.5.0b5/harp/config/factories/__init__.py
--rw-r--r--   0        0        0     4159 2024-04-01 15:50:33.853324 harp_proxy-0.5.0b5/harp/config/factories/kernel_factory.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.853387 harp_proxy-0.5.0b5/harp/config/factories/tests/__init__.py
--rw-r--r--   0        0        0     2026 2024-04-01 15:50:33.853457 harp_proxy-0.5.0b5/harp/config/factories/tests/test_configuration.py
--rw-r--r--   0        0        0     1385 2024-04-01 15:50:33.853518 harp_proxy-0.5.0b5/harp/config/factories/tests/test_settings.py
--rw-r--r--   0        0        0      235 2024-04-01 15:50:33.853605 harp_proxy-0.5.0b5/harp/config/settings/__init__.py
--rw-r--r--   0        0        0      166 2024-04-01 15:50:33.853669 harp_proxy-0.5.0b5/harp/config/settings/base.py
--rw-r--r--   0        0        0      256 2024-04-01 15:50:33.853727 harp_proxy-0.5.0b5/harp/config/settings/disabled.py
--rw-r--r--   0        0        0      626 2024-04-01 15:50:33.853788 harp_proxy-0.5.0b5/harp/config/settings/from_file.py
--rw-r--r--   0        0        0     1381 2024-04-01 15:50:33.854045 harp_proxy-0.5.0b5/harp/controllers/__init__.py
--rw-r--r--   0        0        0      583 2024-04-01 15:50:33.854132 harp_proxy-0.5.0b5/harp/controllers/default.py
--rw-r--r--   0        0        0     1112 2024-04-01 15:50:33.854200 harp_proxy-0.5.0b5/harp/controllers/resolvers.py
--rw-r--r--   0        0        0     3889 2024-04-01 15:50:33.854277 harp_proxy-0.5.0b5/harp/controllers/routing.py
--rw-r--r--   0        0        0      156 2024-04-01 15:50:33.854562 harp_proxy-0.5.0b5/harp/controllers/typing.py
--rw-r--r--   0        0        0      438 2024-04-01 15:50:33.854635 harp_proxy-0.5.0b5/harp/errors.py
--rw-r--r--   0        0        0     1423 2024-04-01 15:50:33.854709 harp_proxy-0.5.0b5/harp/event_dispatcher.py
--rw-r--r--   0        0        0      598 2024-04-01 15:50:33.854812 harp_proxy-0.5.0b5/harp/http/__init__.py
--rw-r--r--   0        0        0      739 2024-04-01 15:50:33.854905 harp_proxy-0.5.0b5/harp/http/errors.py
--rw-r--r--   0        0        0     3907 2024-04-01 15:50:33.854971 harp_proxy-0.5.0b5/harp/http/requests.py
--rw-r--r--   0        0        0     1210 2024-04-01 15:50:33.855026 harp_proxy-0.5.0b5/harp/http/responses.py
--rw-r--r--   0        0        0     3150 2024-04-01 15:50:33.855089 harp_proxy-0.5.0b5/harp/http/serializers.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.855158 harp_proxy-0.5.0b5/harp/http/tests/__init__.py
--rw-r--r--   0        0        0     1671 2024-04-01 15:50:33.855237 harp_proxy-0.5.0b5/harp/http/tests/stubs.py
--rw-r--r--   0        0        0     6125 2024-04-01 15:50:33.855311 harp_proxy-0.5.0b5/harp/http/tests/test_requests.py
--rw-r--r--   0        0        0     3214 2024-04-01 15:50:33.855394 harp_proxy-0.5.0b5/harp/http/tests/test_requests_wrapped.py
--rw-r--r--   0        0        0     3069 2024-04-01 15:50:33.855477 harp_proxy-0.5.0b5/harp/http/tests/test_utils_cookies.py
--rw-r--r--   0        0        0      286 2024-04-01 15:50:33.855583 harp_proxy-0.5.0b5/harp/http/typing/__init__.py
--rw-r--r--   0        0        0      847 2024-04-01 15:50:33.855843 harp_proxy-0.5.0b5/harp/http/typing/bridges.py
--rw-r--r--   0        0        0      591 2024-04-01 15:50:33.855900 harp_proxy-0.5.0b5/harp/http/typing/messages.py
--rw-r--r--   0        0        0      255 2024-04-01 15:50:33.855978 harp_proxy-0.5.0b5/harp/http/typing/serializers.py
--rw-r--r--   0        0        0      123 2024-04-01 15:50:33.856077 harp_proxy-0.5.0b5/harp/http/utils/__init__.py
--rw-r--r--   0        0        0      617 2024-04-01 15:50:33.856138 harp_proxy-0.5.0b5/harp/http/utils/cookies.py
--rw-r--r--   0        0        0     3913 2024-04-01 15:50:33.856204 harp_proxy-0.5.0b5/harp/http/utils/methods.py
--rw-r--r--   0        0        0      794 2024-04-01 15:50:33.856308 harp_proxy-0.5.0b5/harp/meta/__init__.py
--rw-r--r--   0        0        0      470 2024-04-01 15:50:33.856403 harp_proxy-0.5.0b5/harp/models/__init__.py
--rw-r--r--   0        0        0      481 2024-04-01 15:50:33.856499 harp_proxy-0.5.0b5/harp/models/base.py
--rw-r--r--   0        0        0     1732 2024-04-01 15:50:33.856561 harp_proxy-0.5.0b5/harp/models/blobs.py
--rw-r--r--   0        0        0      274 2024-04-01 15:50:33.856625 harp_proxy-0.5.0b5/harp/models/messages.py
--rw-r--r--   0        0        0     1065 2024-04-01 15:50:33.856923 harp_proxy-0.5.0b5/harp/models/transactions.py
--rw-r--r--   0        0        0      365 2024-04-01 15:50:33.856999 harp_proxy-0.5.0b5/harp/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.857068 harp_proxy-0.5.0b5/harp/tests/__init__.py
--rw-r--r--   0        0        0     1684 2024-04-01 15:50:33.857143 harp_proxy-0.5.0b5/harp/tests/test_asgi_kernel.py
--rw-r--r--   0        0        0      988 2024-04-01 15:50:33.857208 harp_proxy-0.5.0b5/harp/tests/test_settings.py
--rw-r--r--   0        0        0      358 2024-04-01 15:50:33.857547 harp_proxy-0.5.0b5/harp/typing/__init__.py
--rw-r--r--   0        0        0      342 2024-04-01 15:50:33.857608 harp_proxy-0.5.0b5/harp/typing/global_settings.py
--rw-r--r--   0        0        0      199 2024-04-01 15:50:33.857713 harp_proxy-0.5.0b5/harp/typing/signs.py
--rw-r--r--   0        0        0     1768 2024-04-01 15:50:33.857957 harp_proxy-0.5.0b5/harp/typing/storage.py
--rw-r--r--   0        0        0      266 2024-04-01 15:50:33.858063 harp_proxy-0.5.0b5/harp/utils/__init__.py
--rw-r--r--   0        0        0      443 2024-04-01 15:50:33.858288 harp_proxy-0.5.0b5/harp/utils/apdex.py
--rw-r--r--   0        0        0      278 2024-04-01 15:50:33.858353 harp_proxy-0.5.0b5/harp/utils/arguments.py
--rw-r--r--   0        0        0     1055 2024-04-01 15:50:33.858428 harp_proxy-0.5.0b5/harp/utils/background.py
--rw-r--r--   0        0        0      188 2024-04-01 15:50:33.858488 harp_proxy-0.5.0b5/harp/utils/bytes.py
--rw-r--r--   0        0        0     2082 2024-04-01 15:50:33.858548 harp_proxy-0.5.0b5/harp/utils/collections.py
--rw-r--r--   0        0        0      739 2024-04-01 15:50:33.858739 harp_proxy-0.5.0b5/harp/utils/dates.py
--rw-r--r--   0        0        0       94 2024-04-01 15:50:33.858900 harp_proxy-0.5.0b5/harp/utils/guids.py
--rw-r--r--   0        0        0      102 2024-04-01 15:50:33.858970 harp_proxy-0.5.0b5/harp/utils/identifiers.py
--rw-r--r--   0        0        0      200 2024-04-01 15:50:33.859037 harp_proxy-0.5.0b5/harp/utils/json.py
--rw-r--r--   0        0        0     1273 2024-04-01 15:50:33.859139 harp_proxy-0.5.0b5/harp/utils/network.py
--rw-r--r--   0        0        0      330 2024-04-01 15:50:33.859207 harp_proxy-0.5.0b5/harp/utils/processes.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.859275 harp_proxy-0.5.0b5/harp/utils/testing/__init__.py
--rw-r--r--   0        0        0      943 2024-04-01 15:50:33.859343 harp_proxy-0.5.0b5/harp/utils/testing/applications.py
--rw-r--r--   0        0        0     2958 2024-04-01 15:50:33.859419 harp_proxy-0.5.0b5/harp/utils/testing/benchmarking.py
--rw-r--r--   0        0        0      217 2024-04-01 15:50:33.859550 harp_proxy-0.5.0b5/harp/utils/testing/communicators/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-01 15:50:33.859623 harp_proxy-0.5.0b5/harp/utils/testing/communicators/asgi.py
--rw-r--r--   0        0        0     2150 2024-04-01 15:50:33.859696 harp_proxy-0.5.0b5/harp/utils/testing/communicators/http.py
--rw-r--r--   0        0        0     4572 2024-04-01 15:50:33.859770 harp_proxy-0.5.0b5/harp/utils/testing/http.py
--rw-r--r--   0        0        0      177 2024-04-01 15:50:33.859881 harp_proxy-0.5.0b5/harp/utils/testing/mixins/__init__.py
--rw-r--r--   0        0        0     2264 2024-04-01 15:50:33.859950 harp_proxy-0.5.0b5/harp/utils/testing/mixins/controllers.py
--rw-r--r--   0        0        0      874 2024-04-01 15:50:33.860052 harp_proxy-0.5.0b5/harp/utils/testing/stub_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.860128 harp_proxy-0.5.0b5/harp/utils/tests/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-01 15:50:33.860211 harp_proxy-0.5.0b5/harp/utils/tests/test_collections.py
--rw-r--r--   0        0        0      691 2024-04-01 15:50:33.860278 harp_proxy-0.5.0b5/harp/utils/tests/test_dates.py
--rw-r--r--   0        0        0      261 2024-04-01 15:50:33.860337 harp_proxy-0.5.0b5/harp/utils/tests/test_urls.py
--rw-r--r--   0        0        0      106 2024-04-01 15:50:33.860394 harp_proxy-0.5.0b5/harp/utils/urls.py
--rw-r--r--   0        0        0      261 2024-04-01 15:50:33.860497 harp_proxy-0.5.0b5/harp/views/__init__.py
--rw-r--r--   0        0        0     1745 2024-04-01 15:50:33.860776 harp_proxy-0.5.0b5/harp/views/json.py
--rw-r--r--   0        0        0      409 2024-04-01 15:50:33.860857 harp_proxy-0.5.0b5/harp/views/strings.py
--rw-r--r--   0        0        0       19 2024-04-01 15:50:33.860964 harp_proxy-0.5.0b5/harp_apps/__init__.py
--rw-r--r--   0        0        0       22 2024-04-01 15:50:33.861067 harp_proxy-0.5.0b5/harp_apps/contrib/__init__.py
--rw-r--r--   0        0        0      728 2024-04-01 15:50:33.861183 harp_proxy-0.5.0b5/harp_apps/contrib/sentry/__app__.py
--rw-r--r--   0        0        0       21 2024-04-01 15:50:33.861248 harp_proxy-0.5.0b5/harp_apps/contrib/sentry/__init__.py
--rw-r--r--   0        0        0       82 2024-04-01 15:50:33.861313 harp_proxy-0.5.0b5/harp_apps/contrib/sentry/settings.py
--rw-r--r--   0        0        0     1248 2024-04-01 15:50:33.861420 harp_proxy-0.5.0b5/harp_apps/dashboard/__app__.py
--rw-r--r--   0        0        0       24 2024-04-01 15:50:33.861481 harp_proxy-0.5.0b5/harp_apps/dashboard/__init__.py
--rw-r--r--   0        0        0     5576 2024-04-01 15:50:33.861806 harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/__init__.py
--rw-r--r--   0        0        0      874 2024-04-01 15:50:33.861892 harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/blobs.py
--rw-r--r--   0        0        0     4732 2024-04-01 15:50:33.862206 harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/overview.py
--rw-r--r--   0        0        0     2757 2024-04-01 15:50:33.862287 harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/system.py
--rw-r--r--   0        0        0     3407 2024-04-01 15:50:33.862373 harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/transactions.py
--rw-r--r--   0        0        0      450 2024-04-01 15:50:33.862745 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/development/index.rst
--rw-r--r--   0        0        0     5487 2024-04-01 15:50:33.862832 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/development/tests_e2e.rst
--rw-r--r--   0        0        0     6937 2024-04-01 15:50:33.862930 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/development/tests_unit.rst
--rw-r--r--   0        0        0      179 2024-04-01 15:50:33.863037 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/examples/auth.basic.yml
--rw-r--r--   0        0        0       99 2024-04-01 15:50:33.863108 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/examples/auth.yml
--rw-r--r--   0        0        0      125 2024-04-01 15:50:33.863177 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/examples/devserver.yml
--rw-r--r--   0        0        0      146 2024-04-01 15:50:33.863245 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/examples/main.yml
--rw-r--r--   0        0        0     2140 2024-04-01 15:50:33.863310 harp_proxy-0.5.0b5/harp_apps/dashboard/docs/index.rst
--rw-r--r--   0        0        0      421 2024-04-01 15:50:33.864370 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/__init__.py
--rw-r--r--   0        0        0      817 2024-04-01 15:50:33.864446 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/base.py
--rw-r--r--   0        0        0      717 2024-04-01 15:50:33.864509 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/transaction_endpoint.py
--rw-r--r--   0        0        0      122 2024-04-01 15:50:33.864573 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/transaction_flag.py
--rw-r--r--   0        0        0      155 2024-04-01 15:50:33.864637 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/transaction_method.py
--rw-r--r--   0        0        0      142 2024-04-01 15:50:33.864695 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/transaction_status.py
--rw-r--r--   0        0        0      168 2024-04-01 15:50:33.864751 harp_proxy-0.5.0b5/harp_apps/dashboard/filters/utils.py
--rw-r--r--   0        0        0       90 2024-04-01 15:50:33.902778 harp_proxy-0.5.0b5/harp_apps/dashboard/schemas/__init__.py
--rw-r--r--   0        0        0      232 2024-04-01 15:50:33.902899 harp_proxy-0.5.0b5/harp_apps/dashboard/schemas/transactions_grouped_by.py
--rw-r--r--   0        0        0     3547 2024-04-01 15:50:33.903573 harp_proxy-0.5.0b5/harp_apps/dashboard/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.903635 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/__init__.py
--rw-r--r--   0        0        0     1752 2024-04-01 15:50:33.903786 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_controllers_blobs.py
--rw-r--r--   0        0        0     2402 2024-04-01 15:50:33.906124 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_controllers_transactions.py
--rw-r--r--   0        0        0      967 2024-04-01 15:50:33.906198 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_settings.py
--rw-r--r--   0        0        0     4039 2024-04-01 15:50:33.906268 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_utils_dependencies.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.906330 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/utils/__init__.py
--rw-r--r--   0        0        0     3101 2024-04-01 15:50:33.906400 harp_proxy-0.5.0b5/harp_apps/dashboard/tests/utils/test_dates.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.906458 harp_proxy-0.5.0b5/harp_apps/dashboard/utils/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-01 15:50:33.907412 harp_proxy-0.5.0b5/harp_apps/dashboard/utils/dates.py
--rw-r--r--   0        0        0     1061 2024-04-01 15:50:33.907475 harp_proxy-0.5.0b5/harp_apps/dashboard/utils/dependencies.py
--rw-r--r--   0        0        0    23255 2024-04-01 15:50:49.759340 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/dateFns-s2EURlY7.js
--rw-r--r--   0        0        0    41267 2024-04-01 15:50:49.759345 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/index-BOfsip6N.css
--rw-r--r--   0        0        0   113735 2024-04-01 15:50:49.759428 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/index-pKJQAlqa.js
--rw-r--r--   0        0        0   141498 2024-04-01 15:50:49.759416 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/react-vbD531y6.js
--rw-r--r--   0        0        0    41176 2024-04-01 15:50:49.759410 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/reactQuery-BTfpiMem.js
--rw-r--r--   0        0        0    55347 2024-04-01 15:50:49.759338 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/reactRouter-iI7EIT1e.js
--rw-r--r--   0        0        0   389875 2024-04-01 15:50:49.759441 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/recharts-9OgIHZXS.js
--rw-r--r--   0        0        0    49465 2024-04-01 15:50:49.759345 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/sentry-B_MfAkLS.js
--rw-r--r--   0        0        0    49075 2024-04-01 15:50:49.759437 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/syntaxHighlighter-D1hpWw2Q.js
--rw-r--r--   0        0        0    37066 2024-04-01 15:50:49.759367 harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/ui-Bo7CIhws.js
--rw-r--r--   0        0        0     2519 2024-04-01 15:50:48.941994 harp_proxy-0.5.0b5/harp_apps/dashboard/web/harp.svg
--rw-r--r--   0        0        0     1089 2024-04-01 15:50:49.759393 harp_proxy-0.5.0b5/harp_apps/dashboard/web/index.html
--rw-r--r--   0        0        0      653 2024-04-01 15:50:33.907577 harp_proxy-0.5.0b5/harp_apps/http_client/__app__.py
--rw-r--r--   0        0        0       26 2024-04-01 15:50:33.907633 harp_proxy-0.5.0b5/harp_apps/http_client/__init__.py
--rw-r--r--   0        0        0      555 2024-04-01 15:50:33.907731 harp_proxy-0.5.0b5/harp_apps/janitor/__app__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.907758 harp_proxy-0.5.0b5/harp_apps/janitor/__init__.py
--rw-r--r--   0        0        0      186 2024-04-01 15:50:33.907820 harp_proxy-0.5.0b5/harp_apps/janitor/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.907878 harp_proxy-0.5.0b5/harp_apps/janitor/tests/__init__.py
--rw-r--r--   0        0        0     3505 2024-04-01 15:50:33.907951 harp_proxy-0.5.0b5/harp_apps/janitor/tests/test_worker.py
--rw-r--r--   0        0        0     3911 2024-04-01 15:50:33.908023 harp_proxy-0.5.0b5/harp_apps/janitor/worker.py
--rw-r--r--   0        0        0     1023 2024-04-01 15:50:33.908352 harp_proxy-0.5.0b5/harp_apps/proxy/__app__.py
--rw-r--r--   0        0        0       20 2024-04-01 15:50:33.908414 harp_proxy-0.5.0b5/harp_apps/proxy/__init__.py
--rw-r--r--   0        0        0     7425 2024-04-01 15:50:33.908696 harp_proxy-0.5.0b5/harp_apps/proxy/controllers.py
--rw-r--r--   0        0        0       88 2024-04-01 15:50:33.908979 harp_proxy-0.5.0b5/harp_apps/proxy/docs/examples/swapi.yml
--rw-r--r--   0        0        0      862 2024-04-01 15:50:33.909039 harp_proxy-0.5.0b5/harp_apps/proxy/docs/index.rst
--rw-r--r--   0        0        0      164 2024-04-01 15:50:33.909092 harp_proxy-0.5.0b5/harp_apps/proxy/events.py
--rw-r--r--   0        0        0      633 2024-04-01 15:50:33.909148 harp_proxy-0.5.0b5/harp_apps/proxy/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.909207 harp_proxy-0.5.0b5/harp_apps/proxy/tests/__init__.py
--rw-r--r--   0        0        0     8497 2024-04-01 15:50:33.909457 harp_proxy-0.5.0b5/harp_apps/proxy/tests/test_controllers_http_proxy.py
--rw-r--r--   0        0        0     1061 2024-04-01 15:50:33.909572 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/__app__.py
--rw-r--r--   0        0        0       33 2024-04-01 15:50:33.909633 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/__init__.py
--rw-r--r--   0        0        0      160 2024-04-01 15:50:33.909706 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/constants.py
--rw-r--r--   0        0        0     1033 2024-04-01 15:50:33.909815 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/docs/index.rst
--rw-r--r--   0        0        0      877 2024-04-01 15:50:33.909915 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/__init__.py
--rw-r--r--   0        0        0     2194 2024-04-01 15:50:33.909987 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/base.py
--rw-r--r--   0        0        0     1928 2024-04-01 15:50:33.910063 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/blobs.py
--rw-r--r--   0        0        0     1082 2024-04-01 15:50:33.910127 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/flags.py
--rw-r--r--   0        0        0     2413 2024-04-01 15:50:33.910209 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/messages.py
--rw-r--r--   0        0        0     1425 2024-04-01 15:50:33.910281 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/metrics.py
--rw-r--r--   0        0        0      934 2024-04-01 15:50:33.910344 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/tags.py
--rw-r--r--   0        0        0     6198 2024-04-01 15:50:33.910605 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/transactions.py
--rw-r--r--   0        0        0      882 2024-04-01 15:50:33.910677 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/users.py
--rw-r--r--   0        0        0      633 2024-04-01 15:50:33.910745 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/settings.py
--rw-r--r--   0        0        0    17727 2024-04-01 15:50:33.911099 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/storage.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.911184 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/__init__.py
--rw-r--r--   0        0        0     1143 2024-04-01 15:50:33.911250 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_application.py
--rw-r--r--   0        0        0     2928 2024-04-01 15:50:33.911314 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_models_base.py
--rw-r--r--   0        0        0      829 2024-04-01 15:50:33.911377 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py
--rw-r--r--   0        0        0     1487 2024-04-01 15:50:33.911435 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py
--rw-r--r--   0        0        0      504 2024-04-01 15:50:33.911501 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_storage_usage.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.911577 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/__init__.py
--rw-r--r--   0        0        0     2920 2024-04-01 15:50:33.911651 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/dates.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.911709 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/testing/__init__.py
--rw-r--r--   0        0        0     1884 2024-04-01 15:50:33.911779 harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/testing/mixins.py
--rw-r--r--   0        0        0     1032 2024-04-01 15:50:33.911911 harp_proxy-0.5.0b5/harp_apps/telemetry/__app__.py
--rw-r--r--   0        0        0       24 2024-04-01 15:50:33.911979 harp_proxy-0.5.0b5/harp_apps/telemetry/__init__.py
--rw-r--r--   0        0        0     2735 2024-04-01 15:50:33.912062 harp_proxy-0.5.0b5/harp_apps/telemetry/manager.py
--rw-r--r--   0        0        0        0 2024-04-01 15:50:33.912149 harp_proxy-0.5.0b5/harp_apps/telemetry/tests/__init__.py
--rw-r--r--   0        0        0      160 2024-04-01 15:50:33.912266 harp_proxy-0.5.0b5/harp_apps/telemetry/tests/test_application.py
--rw-r--r--   0        0        0     1768 2024-04-01 15:50:33.912335 harp_proxy-0.5.0b5/harp_apps/telemetry/tests/test_manager.py
--rw-r--r--   0        0        0     2782 2024-04-01 15:50:33.915737 harp_proxy-0.5.0b5/pyproject.toml
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 harp_proxy-0.5.0b5/PKG-INFO
+-rw-r--r--   0        0        0     2001 2024-05-30 09:59:02.081756 harp_proxy-0.5.0b6/LICENSE.rst
+-rw-r--r--   0        0        0     3940 2024-05-30 09:59:02.082360 harp_proxy-0.5.0b6/README.rst
+-rw-r--r--   0        0        0     2917 2024-05-30 09:59:02.110733 harp_proxy-0.5.0b6/harp/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-30 09:59:02.110788 harp_proxy-0.5.0b6/harp/__main__.py
+-rw-r--r--   0        0        0     3047 2024-05-30 09:59:02.111061 harp_proxy-0.5.0b6/harp/_logging.py
+-rw-r--r--   0        0        0       84 2024-05-30 09:59:02.111149 harp_proxy-0.5.0b6/harp/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.111213 harp_proxy-0.5.0b6/harp/asgi/bridge/__init__.py
+-rw-r--r--   0        0        0     2874 2024-05-30 09:59:02.111287 harp_proxy-0.5.0b6/harp/asgi/bridge/requests.py
+-rw-r--r--   0        0        0     1313 2024-05-30 09:59:02.111347 harp_proxy-0.5.0b6/harp/asgi/bridge/responses.py
+-rw-r--r--   0        0        0     2072 2024-05-30 09:59:02.111409 harp_proxy-0.5.0b6/harp/asgi/events.py
+-rw-r--r--   0        0        0     6824 2024-05-30 09:59:02.111698 harp_proxy-0.5.0b6/harp/asgi/kernel.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.111765 harp_proxy-0.5.0b6/harp/asgi/tests/__init__.py
+-rw-r--r--   0        0        0     6987 2024-05-30 09:59:02.111849 harp_proxy-0.5.0b6/harp/asgi/tests/test_http_bridge_asgi_request.py
+-rw-r--r--   0        0        0     2114 2024-05-30 09:59:02.112141 harp_proxy-0.5.0b6/harp/commandline/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-30 09:59:02.112410 harp_proxy-0.5.0b6/harp/commandline/install_dev.py
+-rw-r--r--   0        0        0     2113 2024-05-30 09:59:02.112618 harp_proxy-0.5.0b6/harp/commandline/server.py
+-rw-r--r--   0        0        0     3765 2024-05-30 09:59:02.112832 harp_proxy-0.5.0b6/harp/commandline/start.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.112892 harp_proxy-0.5.0b6/harp/commandline/tests/__init__.py
+-rw-r--r--   0        0        0      620 2024-05-30 09:59:02.113160 harp_proxy-0.5.0b6/harp/commandline/tests/test_server_options.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.113221 harp_proxy-0.5.0b6/harp/commandline/utils/__init__.py
+-rw-r--r--   0        0        0     1375 2024-05-30 09:59:02.113489 harp_proxy-0.5.0b6/harp/commandline/utils/_hacks.py
+-rw-r--r--   0        0        0     4880 2024-05-30 09:59:02.113772 harp_proxy-0.5.0b6/harp/commandline/utils/manager.py
+-rw-r--r--   0        0        0      538 2024-05-30 09:59:02.113882 harp_proxy-0.5.0b6/harp/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.113950 harp_proxy-0.5.0b6/harp/config/adapters/__init__.py
+-rw-r--r--   0        0        0     1408 2024-05-30 09:59:02.114181 harp_proxy-0.5.0b6/harp/config/adapters/hypercorn.py
+-rw-r--r--   0        0        0     2398 2024-05-30 09:59:02.114264 harp_proxy-0.5.0b6/harp/config/application.py
+-rw-r--r--   0        0        0    12196 2024-05-30 09:59:02.114563 harp_proxy-0.5.0b6/harp/config/config.py
+-rw-r--r--   0        0        0     1533 2024-05-30 09:59:02.114639 harp_proxy-0.5.0b6/harp/config/events.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.114701 harp_proxy-0.5.0b6/harp/config/factories/__init__.py
+-rw-r--r--   0        0        0     4159 2024-05-30 09:59:02.114792 harp_proxy-0.5.0b6/harp/config/factories/kernel_factory.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.114852 harp_proxy-0.5.0b6/harp/config/factories/tests/__init__.py
+-rw-r--r--   0        0        0     2026 2024-05-30 09:59:02.114927 harp_proxy-0.5.0b6/harp/config/factories/tests/test_configuration.py
+-rw-r--r--   0        0        0     1385 2024-05-30 09:59:02.114994 harp_proxy-0.5.0b6/harp/config/factories/tests/test_settings.py
+-rw-r--r--   0        0        0      235 2024-05-30 09:59:02.115100 harp_proxy-0.5.0b6/harp/config/settings/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-30 09:59:02.115164 harp_proxy-0.5.0b6/harp/config/settings/base.py
+-rw-r--r--   0        0        0      256 2024-05-30 09:59:02.115228 harp_proxy-0.5.0b6/harp/config/settings/disabled.py
+-rw-r--r--   0        0        0      626 2024-05-30 09:59:02.115293 harp_proxy-0.5.0b6/harp/config/settings/from_file.py
+-rw-r--r--   0        0        0     1381 2024-05-30 09:59:02.115612 harp_proxy-0.5.0b6/harp/controllers/__init__.py
+-rw-r--r--   0        0        0      583 2024-05-30 09:59:02.115680 harp_proxy-0.5.0b6/harp/controllers/default.py
+-rw-r--r--   0        0        0     1112 2024-05-30 09:59:02.115741 harp_proxy-0.5.0b6/harp/controllers/resolvers.py
+-rw-r--r--   0        0        0     3889 2024-05-30 09:59:02.115963 harp_proxy-0.5.0b6/harp/controllers/routing.py
+-rw-r--r--   0        0        0      156 2024-05-30 09:59:02.116180 harp_proxy-0.5.0b6/harp/controllers/typing.py
+-rw-r--r--   0        0        0      438 2024-05-30 09:59:02.116238 harp_proxy-0.5.0b6/harp/errors.py
+-rw-r--r--   0        0        0     1423 2024-05-30 09:59:02.116302 harp_proxy-0.5.0b6/harp/event_dispatcher.py
+-rw-r--r--   0        0        0      598 2024-05-30 09:59:02.116400 harp_proxy-0.5.0b6/harp/http/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-30 09:59:02.116463 harp_proxy-0.5.0b6/harp/http/errors.py
+-rw-r--r--   0        0        0     3907 2024-05-30 09:59:02.116535 harp_proxy-0.5.0b6/harp/http/requests.py
+-rw-r--r--   0        0        0     1210 2024-05-30 09:59:02.116597 harp_proxy-0.5.0b6/harp/http/responses.py
+-rw-r--r--   0        0        0     3150 2024-05-30 09:59:02.116662 harp_proxy-0.5.0b6/harp/http/serializers.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.116721 harp_proxy-0.5.0b6/harp/http/tests/__init__.py
+-rw-r--r--   0        0        0     1671 2024-05-30 09:59:02.116792 harp_proxy-0.5.0b6/harp/http/tests/stubs.py
+-rw-r--r--   0        0        0     6125 2024-05-30 09:59:02.116861 harp_proxy-0.5.0b6/harp/http/tests/test_requests.py
+-rw-r--r--   0        0        0     3214 2024-05-30 09:59:02.116923 harp_proxy-0.5.0b6/harp/http/tests/test_requests_wrapped.py
+-rw-r--r--   0        0        0     3069 2024-05-30 09:59:02.116989 harp_proxy-0.5.0b6/harp/http/tests/test_utils_cookies.py
+-rw-r--r--   0        0        0      286 2024-05-30 09:59:02.117084 harp_proxy-0.5.0b6/harp/http/typing/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-30 09:59:02.117357 harp_proxy-0.5.0b6/harp/http/typing/bridges.py
+-rw-r--r--   0        0        0      591 2024-05-30 09:59:02.117449 harp_proxy-0.5.0b6/harp/http/typing/messages.py
+-rw-r--r--   0        0        0      255 2024-05-30 09:59:02.117538 harp_proxy-0.5.0b6/harp/http/typing/serializers.py
+-rw-r--r--   0        0        0      123 2024-05-30 09:59:02.117646 harp_proxy-0.5.0b6/harp/http/utils/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-30 09:59:02.117714 harp_proxy-0.5.0b6/harp/http/utils/cookies.py
+-rw-r--r--   0        0        0     3913 2024-05-30 09:59:02.117785 harp_proxy-0.5.0b6/harp/http/utils/methods.py
+-rw-r--r--   0        0        0      794 2024-05-30 09:59:02.117884 harp_proxy-0.5.0b6/harp/meta/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-30 09:59:02.117979 harp_proxy-0.5.0b6/harp/models/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-30 09:59:02.118048 harp_proxy-0.5.0b6/harp/models/base.py
+-rw-r--r--   0        0        0     1732 2024-05-30 09:59:02.118111 harp_proxy-0.5.0b6/harp/models/blobs.py
+-rw-r--r--   0        0        0      274 2024-05-30 09:59:02.118172 harp_proxy-0.5.0b6/harp/models/messages.py
+-rw-r--r--   0        0        0     1065 2024-05-30 09:59:02.118461 harp_proxy-0.5.0b6/harp/models/transactions.py
+-rw-r--r--   0        0        0      604 2024-05-30 09:59:02.118718 harp_proxy-0.5.0b6/harp/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.118782 harp_proxy-0.5.0b6/harp/tests/__init__.py
+-rw-r--r--   0        0        0     1684 2024-05-30 09:59:02.118869 harp_proxy-0.5.0b6/harp/tests/test_asgi_kernel.py
+-rw-r--r--   0        0        0      988 2024-05-30 09:59:02.118931 harp_proxy-0.5.0b6/harp/tests/test_settings.py
+-rw-r--r--   0        0        0      358 2024-05-30 09:59:02.119220 harp_proxy-0.5.0b6/harp/typing/__init__.py
+-rw-r--r--   0        0        0      342 2024-05-30 09:59:02.119280 harp_proxy-0.5.0b6/harp/typing/global_settings.py
+-rw-r--r--   0        0        0      199 2024-05-30 09:59:02.119335 harp_proxy-0.5.0b6/harp/typing/signs.py
+-rw-r--r--   0        0        0     1768 2024-05-30 09:59:02.119538 harp_proxy-0.5.0b6/harp/typing/storage.py
+-rw-r--r--   0        0        0      266 2024-05-30 09:59:02.119633 harp_proxy-0.5.0b6/harp/utils/__init__.py
+-rw-r--r--   0        0        0      443 2024-05-30 09:59:02.119879 harp_proxy-0.5.0b6/harp/utils/apdex.py
+-rw-r--r--   0        0        0      278 2024-05-30 09:59:02.119940 harp_proxy-0.5.0b6/harp/utils/arguments.py
+-rw-r--r--   0        0        0     1055 2024-05-30 09:59:02.119997 harp_proxy-0.5.0b6/harp/utils/background.py
+-rw-r--r--   0        0        0      188 2024-05-30 09:59:02.120050 harp_proxy-0.5.0b6/harp/utils/bytes.py
+-rw-r--r--   0        0        0     2082 2024-05-30 09:59:02.120109 harp_proxy-0.5.0b6/harp/utils/collections.py
+-rw-r--r--   0        0        0      557 2024-05-30 09:59:02.120365 harp_proxy-0.5.0b6/harp/utils/commandline.py
+-rw-r--r--   0        0        0      739 2024-05-30 09:59:02.120431 harp_proxy-0.5.0b6/harp/utils/dates.py
+-rw-r--r--   0        0        0       94 2024-05-30 09:59:02.120493 harp_proxy-0.5.0b6/harp/utils/guids.py
+-rw-r--r--   0        0        0      102 2024-05-30 09:59:02.120549 harp_proxy-0.5.0b6/harp/utils/identifiers.py
+-rw-r--r--   0        0        0      200 2024-05-30 09:59:02.120603 harp_proxy-0.5.0b6/harp/utils/json.py
+-rw-r--r--   0        0        0     1273 2024-05-30 09:59:02.120663 harp_proxy-0.5.0b6/harp/utils/network.py
+-rw-r--r--   0        0        0      330 2024-05-30 09:59:02.120720 harp_proxy-0.5.0b6/harp/utils/processes.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.120785 harp_proxy-0.5.0b6/harp/utils/testing/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-30 09:59:02.120854 harp_proxy-0.5.0b6/harp/utils/testing/applications.py
+-rw-r--r--   0        0        0     2958 2024-05-30 09:59:02.120921 harp_proxy-0.5.0b6/harp/utils/testing/benchmarking.py
+-rw-r--r--   0        0        0      217 2024-05-30 09:59:02.121005 harp_proxy-0.5.0b6/harp/utils/testing/communicators/__init__.py
+-rw-r--r--   0        0        0     2222 2024-05-30 09:59:02.121066 harp_proxy-0.5.0b6/harp/utils/testing/communicators/asgi.py
+-rw-r--r--   0        0        0     2150 2024-05-30 09:59:02.121129 harp_proxy-0.5.0b6/harp/utils/testing/communicators/http.py
+-rw-r--r--   0        0        0     4572 2024-05-30 09:59:02.121197 harp_proxy-0.5.0b6/harp/utils/testing/http.py
+-rw-r--r--   0        0        0      177 2024-05-30 09:59:02.121284 harp_proxy-0.5.0b6/harp/utils/testing/mixins/__init__.py
+-rw-r--r--   0        0        0     2264 2024-05-30 09:59:02.121356 harp_proxy-0.5.0b6/harp/utils/testing/mixins/controllers.py
+-rw-r--r--   0        0        0      874 2024-05-30 09:59:02.121449 harp_proxy-0.5.0b6/harp/utils/testing/stub_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.121509 harp_proxy-0.5.0b6/harp/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-30 09:59:02.121577 harp_proxy-0.5.0b6/harp/utils/tests/test_collections.py
+-rw-r--r--   0        0        0      691 2024-05-30 09:59:02.121632 harp_proxy-0.5.0b6/harp/utils/tests/test_dates.py
+-rw-r--r--   0        0        0      261 2024-05-30 09:59:02.121691 harp_proxy-0.5.0b6/harp/utils/tests/test_urls.py
+-rw-r--r--   0        0        0      106 2024-05-30 09:59:02.121743 harp_proxy-0.5.0b6/harp/utils/urls.py
+-rw-r--r--   0        0        0      261 2024-05-30 09:59:02.121830 harp_proxy-0.5.0b6/harp/views/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-30 09:59:02.122097 harp_proxy-0.5.0b6/harp/views/json.py
+-rw-r--r--   0        0        0      409 2024-05-30 09:59:02.122154 harp_proxy-0.5.0b6/harp/views/strings.py
+-rw-r--r--   0        0        0       19 2024-05-30 09:59:02.122242 harp_proxy-0.5.0b6/harp_apps/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-30 09:59:02.122327 harp_proxy-0.5.0b6/harp_apps/contrib/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-30 09:59:02.122418 harp_proxy-0.5.0b6/harp_apps/contrib/sentry/__app__.py
+-rw-r--r--   0        0        0       21 2024-05-30 09:59:02.122470 harp_proxy-0.5.0b6/harp_apps/contrib/sentry/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-30 09:59:02.122519 harp_proxy-0.5.0b6/harp_apps/contrib/sentry/settings.py
+-rw-r--r--   0        0        0     1248 2024-05-30 09:59:02.122614 harp_proxy-0.5.0b6/harp_apps/dashboard/__app__.py
+-rw-r--r--   0        0        0       24 2024-05-30 09:59:02.122666 harp_proxy-0.5.0b6/harp_apps/dashboard/__init__.py
+-rw-r--r--   0        0        0     5681 2024-05-30 09:59:02.122962 harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-30 09:59:02.123030 harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/blobs.py
+-rw-r--r--   0        0        0     4732 2024-05-30 09:59:02.123298 harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/overview.py
+-rw-r--r--   0        0        0     2757 2024-05-30 09:59:02.123362 harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/system.py
+-rw-r--r--   0        0        0     3407 2024-05-30 09:59:02.123430 harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/transactions.py
+-rw-r--r--   0        0        0      450 2024-05-30 09:59:02.123560 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/development/index.rst
+-rw-r--r--   0        0        0     5487 2024-05-30 09:59:02.123636 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/development/tests_e2e.rst
+-rw-r--r--   0        0        0     6937 2024-05-30 09:59:02.123712 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/development/tests_unit.rst
+-rw-r--r--   0        0        0      179 2024-05-30 09:59:02.123800 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/examples/auth.basic.yml
+-rw-r--r--   0        0        0       99 2024-05-30 09:59:02.123856 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/examples/auth.yml
+-rw-r--r--   0        0        0      125 2024-05-30 09:59:02.123909 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/examples/devserver.yml
+-rw-r--r--   0        0        0      146 2024-05-30 09:59:02.123962 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/examples/main.yml
+-rw-r--r--   0        0        0     2140 2024-05-30 09:59:02.124026 harp_proxy-0.5.0b6/harp_apps/dashboard/docs/index.rst
+-rw-r--r--   0        0        0      421 2024-05-30 09:59:02.124255 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/__init__.py
+-rw-r--r--   0        0        0      817 2024-05-30 09:59:02.124314 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/base.py
+-rw-r--r--   0        0        0      717 2024-05-30 09:59:02.124387 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/transaction_endpoint.py
+-rw-r--r--   0        0        0      122 2024-05-30 09:59:02.124446 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/transaction_flag.py
+-rw-r--r--   0        0        0      155 2024-05-30 09:59:02.124510 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/transaction_method.py
+-rw-r--r--   0        0        0      142 2024-05-30 09:59:02.124604 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/transaction_status.py
+-rw-r--r--   0        0        0      168 2024-05-30 09:59:02.124665 harp_proxy-0.5.0b6/harp_apps/dashboard/filters/utils.py
+-rw-r--r--   0        0        0       90 2024-05-30 09:59:02.162484 harp_proxy-0.5.0b6/harp_apps/dashboard/schemas/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-30 09:59:02.162549 harp_proxy-0.5.0b6/harp_apps/dashboard/schemas/transactions_grouped_by.py
+-rw-r--r--   0        0        0     3547 2024-05-30 09:59:02.162621 harp_proxy-0.5.0b6/harp_apps/dashboard/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.162680 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/__init__.py
+-rw-r--r--   0        0        0     1752 2024-05-30 09:59:02.162751 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_controllers_blobs.py
+-rw-r--r--   0        0        0     2402 2024-05-30 09:59:02.162829 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_controllers_transactions.py
+-rw-r--r--   0        0        0      967 2024-05-30 09:59:02.162899 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_settings.py
+-rw-r--r--   0        0        0     4039 2024-05-30 09:59:02.162970 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_utils_dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.163029 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3101 2024-05-30 09:59:02.163098 harp_proxy-0.5.0b6/harp_apps/dashboard/tests/utils/test_dates.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.163163 harp_proxy-0.5.0b6/harp_apps/dashboard/utils/__init__.py
+-rw-r--r--   0        0        0     2758 2024-05-30 09:59:02.163515 harp_proxy-0.5.0b6/harp_apps/dashboard/utils/dates.py
+-rw-r--r--   0        0        0     1061 2024-05-30 09:59:02.163576 harp_proxy-0.5.0b6/harp_apps/dashboard/utils/dependencies.py
+-rw-r--r--   0        0        0    23255 2024-05-30 09:59:22.418036 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/dateFns-s2EURlY7.js
+-rw-r--r--   0        0        0   113779 2024-05-30 09:59:22.418165 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/index-CKrV6JKW.js
+-rw-r--r--   0        0        0    41290 2024-05-30 09:59:22.417641 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/index-sYClmDC3.css
+-rw-r--r--   0        0        0   141498 2024-05-30 09:59:22.418358 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/react-vbD531y6.js
+-rw-r--r--   0        0        0    41176 2024-05-30 09:59:22.418195 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/reactQuery-BTfpiMem.js
+-rw-r--r--   0        0        0    55347 2024-05-30 09:59:22.417956 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/reactRouter-iI7EIT1e.js
+-rw-r--r--   0        0        0   390040 2024-05-30 09:59:22.418089 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/recharts-BzBtiWsS.js
+-rw-r--r--   0        0        0    49465 2024-05-30 09:59:22.418001 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/sentry-DxJl7iQ9.js
+-rw-r--r--   0        0        0    49075 2024-05-30 09:59:22.418269 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/syntaxHighlighter-CEoW8GyI.js
+-rw-r--r--   0        0        0    37066 2024-05-30 09:59:22.418117 harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/ui-DM1JZie1.js
+-rw-r--r--   0        0        0     2519 2024-05-30 09:59:21.511358 harp_proxy-0.5.0b6/harp_apps/dashboard/web/harp.svg
+-rw-r--r--   0        0        0     1089 2024-05-30 09:59:22.418227 harp_proxy-0.5.0b6/harp_apps/dashboard/web/index.html
+-rw-r--r--   0        0        0      653 2024-05-30 09:59:02.163671 harp_proxy-0.5.0b6/harp_apps/http_client/__app__.py
+-rw-r--r--   0        0        0       26 2024-05-30 09:59:02.163729 harp_proxy-0.5.0b6/harp_apps/http_client/__init__.py
+-rw-r--r--   0        0        0      555 2024-05-30 09:59:02.163824 harp_proxy-0.5.0b6/harp_apps/janitor/__app__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.163851 harp_proxy-0.5.0b6/harp_apps/janitor/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-30 09:59:02.163913 harp_proxy-0.5.0b6/harp_apps/janitor/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.163971 harp_proxy-0.5.0b6/harp_apps/janitor/tests/__init__.py
+-rw-r--r--   0        0        0     3505 2024-05-30 09:59:02.164043 harp_proxy-0.5.0b6/harp_apps/janitor/tests/test_worker.py
+-rw-r--r--   0        0        0     3911 2024-05-30 09:59:02.164113 harp_proxy-0.5.0b6/harp_apps/janitor/worker.py
+-rw-r--r--   0        0        0     1023 2024-05-30 09:59:02.164430 harp_proxy-0.5.0b6/harp_apps/proxy/__app__.py
+-rw-r--r--   0        0        0       20 2024-05-30 09:59:02.164488 harp_proxy-0.5.0b6/harp_apps/proxy/__init__.py
+-rw-r--r--   0        0        0     7425 2024-05-30 09:59:02.164785 harp_proxy-0.5.0b6/harp_apps/proxy/controllers.py
+-rw-r--r--   0        0        0       88 2024-05-30 09:59:02.165128 harp_proxy-0.5.0b6/harp_apps/proxy/docs/examples/swapi.yml
+-rw-r--r--   0        0        0      862 2024-05-30 09:59:02.165195 harp_proxy-0.5.0b6/harp_apps/proxy/docs/index.rst
+-rw-r--r--   0        0        0      164 2024-05-30 09:59:02.165251 harp_proxy-0.5.0b6/harp_apps/proxy/events.py
+-rw-r--r--   0        0        0      633 2024-05-30 09:59:02.165308 harp_proxy-0.5.0b6/harp_apps/proxy/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.165369 harp_proxy-0.5.0b6/harp_apps/proxy/tests/__init__.py
+-rw-r--r--   0        0        0     8497 2024-05-30 09:59:02.165711 harp_proxy-0.5.0b6/harp_apps/proxy/tests/test_controllers_http_proxy.py
+-rw-r--r--   0        0        0     1061 2024-05-30 09:59:02.165820 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/__app__.py
+-rw-r--r--   0        0        0       33 2024-05-30 09:59:02.165874 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-30 09:59:02.165927 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/constants.py
+-rw-r--r--   0        0        0     1033 2024-05-30 09:59:02.166017 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/docs/index.rst
+-rw-r--r--   0        0        0      877 2024-05-30 09:59:02.166105 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-30 09:59:02.166170 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/base.py
+-rw-r--r--   0        0        0     1928 2024-05-30 09:59:02.166234 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/blobs.py
+-rw-r--r--   0        0        0     1082 2024-05-30 09:59:02.166294 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/flags.py
+-rw-r--r--   0        0        0     2413 2024-05-30 09:59:02.166361 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/messages.py
+-rw-r--r--   0        0        0     1425 2024-05-30 09:59:02.166422 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/metrics.py
+-rw-r--r--   0        0        0      934 2024-05-30 09:59:02.166478 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/tags.py
+-rw-r--r--   0        0        0     6198 2024-05-30 09:59:02.166767 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/transactions.py
+-rw-r--r--   0        0        0      882 2024-05-30 09:59:02.166830 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/users.py
+-rw-r--r--   0        0        0      633 2024-05-30 09:59:02.166889 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/settings.py
+-rw-r--r--   0        0        0    17727 2024-05-30 09:59:02.167235 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/storage.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.167312 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-30 09:59:02.167385 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_application.py
+-rw-r--r--   0        0        0     2928 2024-05-30 09:59:02.167455 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_models_base.py
+-rw-r--r--   0        0        0      829 2024-05-30 09:59:02.167518 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py
+-rw-r--r--   0        0        0     1487 2024-05-30 09:59:02.167575 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py
+-rw-r--r--   0        0        0      504 2024-05-30 09:59:02.167630 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_storage_usage.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.167687 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/__init__.py
+-rw-r--r--   0        0        0     2920 2024-05-30 09:59:02.167758 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/dates.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.167818 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/testing/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-30 09:59:02.167896 harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/testing/mixins.py
+-rw-r--r--   0        0        0     1032 2024-05-30 09:59:02.168016 harp_proxy-0.5.0b6/harp_apps/telemetry/__app__.py
+-rw-r--r--   0        0        0       24 2024-05-30 09:59:02.168072 harp_proxy-0.5.0b6/harp_apps/telemetry/__init__.py
+-rw-r--r--   0        0        0     2735 2024-05-30 09:59:02.168138 harp_proxy-0.5.0b6/harp_apps/telemetry/manager.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:59:02.168193 harp_proxy-0.5.0b6/harp_apps/telemetry/tests/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-30 09:59:02.168262 harp_proxy-0.5.0b6/harp_apps/telemetry/tests/test_application.py
+-rw-r--r--   0        0        0     1768 2024-05-30 09:59:02.168321 harp_proxy-0.5.0b6/harp_apps/telemetry/tests/test_manager.py
+-rw-r--r--   0        0        0     2869 2024-05-30 09:59:02.171643 harp_proxy-0.5.0b6/pyproject.toml
+-rw-r--r--   0        0        0     5641 1970-01-01 00:00:00.000000 harp_proxy-0.5.0b6/PKG-INFO
```

### Comparing `harp_proxy-0.5.0b5/LICENSE.rst` & `harp_proxy-0.5.0b6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/README.rst` & `harp_proxy-0.5.0b6/README.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/__init__.py` & `harp_proxy-0.5.0b6/harp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,23 +75,21 @@
     """
     Run the default server using provided configuration.
 
     :param config: Config
     :return:
     """
     import asyncio
-    import sys
 
     from harp.config.adapters.hypercorn import HypercornAdapter
     from harp.config.factories.kernel_factory import KernelFactory
 
-    config.read_env(sys.argv[1:])
     factory = KernelFactory(config)
     server = HypercornAdapter(factory)
-    asyncio.run(server.serve())
+    return asyncio.run(server.serve())
 
 
 __all__ = [
     "Config",
     "ROOT_DIR",
     "__revision__",
     "__version__",
```

### Comparing `harp_proxy-0.5.0b5/harp/_logging.py` & `harp_proxy-0.5.0b6/harp/_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,26 +20,34 @@
 structlog.configure(
     logger_factory=structlog.stdlib.LoggerFactory(),
     wrapper_class=structlog.stdlib.BoundLogger,
     processors=processors,
     cache_logger_on_first_use=True,
 )
 
+try:
+    _exc_formatter_options = {"width": os.get_terminal_size()[0]}
+except OSError:
+    _exc_formatter_options = {}
+
+
 LOGGING_FORMATTERS = {
     "json": {
         "()": structlog.stdlib.ProcessorFormatter,
         "processor": structlog.processors.JSONRenderer(),
     },
     "plain": {
         "()": structlog.stdlib.ProcessorFormatter,
         "processor": structlog.dev.ConsoleRenderer(exception_formatter=structlog.dev.plain_traceback, colors=False),
     },
     "pretty": {
         "()": structlog.stdlib.ProcessorFormatter,
-        "processor": structlog.dev.ConsoleRenderer(exception_formatter=structlog.dev.plain_traceback),
+        "processor": structlog.dev.ConsoleRenderer(
+            exception_formatter=structlog.dev.RichTracebackFormatter(**_exc_formatter_options)
+        ),
     },
     "keyvalue": {
         "()": structlog.stdlib.ProcessorFormatter,
         "processor": structlog.processors.KeyValueRenderer(key_order=["timestamp", "level", "event", "logger"]),
     },
 }
```

### Comparing `harp_proxy-0.5.0b5/harp/asgi/bridge/requests.py` & `harp_proxy-0.5.0b6/harp/asgi/bridge/requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/asgi/bridge/responses.py` & `harp_proxy-0.5.0b6/harp/asgi/bridge/responses.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/asgi/events.py` & `harp_proxy-0.5.0b6/harp/asgi/events.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/asgi/kernel.py` & `harp_proxy-0.5.0b6/harp/asgi/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import traceback
 from inspect import signature
 
 from asgiref.typing import ASGIReceiveCallable, ASGISendCallable, Scope
+from hypercorn.utils import LifespanFailureError
 from whistle import AsyncEventDispatcher, Event, IAsyncEventDispatcher
 
 from harp import get_logger
 from harp.controllers import DefaultControllerResolver
 from harp.http import AlreadyHandledHttpResponse, HttpRequest, HttpResponse
 
 from .bridge.requests import HttpRequestAsgiBridge
@@ -43,15 +44,19 @@
             response = await self.handle_http(scope, receive, send)
             if isinstance(response, AlreadyHandledHttpResponse):
                 return
             return await HttpResponseAsgiBridge(response, send).send()
 
         if asgi_type == "lifespan":
             await receive()
-            await self.dispatcher.adispatch(EVENT_CORE_STARTED, Event())
+            try:
+                await self.dispatcher.adispatch(EVENT_CORE_STARTED, Event())
+            except Exception as exc:
+                raise LifespanFailureError(EVENT_CORE_STARTED, repr(exc)) from exc
+
             self.started = True
             return
 
         if asgi_type == "websocket":
             # NOT IMPLEMENTED YET!
             # This is ignored here to avoid huge errors in the console.
             return
```

### Comparing `harp_proxy-0.5.0b5/harp/asgi/tests/test_http_bridge_asgi_request.py` & `harp_proxy-0.5.0b6/harp/asgi/tests/test_http_bridge_asgi_request.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/commandline/__init__.py` & `harp_proxy-0.5.0b6/harp/commandline/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,33 +31,45 @@
 
 .. click:: harp.commandline:entrypoint
    :prog: harp
    :nested: full
 
 """
 
-import rich_click as click
-
 from harp.commandline.install_dev import install_dev
+from harp.commandline.server import server
 from harp.commandline.start import start
+from harp.settings import HARP_ENV
+from harp.utils.commandline import check_packages, click
 
 __title__ = "Command Line"
 
+IS_DEVELOPMENT_ENVIRONMENT = False
+
+if HARP_ENV == "dev" or check_packages("honcho", "watchfiles"):
+    IS_DEVELOPMENT_ENVIRONMENT = True
+
+if HARP_ENV == "prod":
+    IS_DEVELOPMENT_ENVIRONMENT = False
+
 
 @click.group()
 def entrypoint():
     """HTTP Application Runtime Proxy (HARP)
 
     The following commands are available to help you setup and run your HTTP proxy application.
 
     """
     pass
 
 
-entrypoint.add_command(start)
-entrypoint.add_command(install_dev)
+if IS_DEVELOPMENT_ENVIRONMENT:
+    entrypoint.add_command(start)
+    entrypoint.add_command(install_dev)
+
+entrypoint.add_command(server)
 
 __all__ = [
     "entrypoint",
     "start",
     "install_dev",
 ]
```

### Comparing `harp_proxy-0.5.0b5/harp/commandline/start.py` & `harp_proxy-0.5.0b6/harp/commandline/start.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import importlib.util
 import sys
-from itertools import chain
-
-import rich_click as click
 
+from harp.commandline.server import ServerOptions, add_harp_server_click_options
 from harp.commandline.utils.manager import HARP_DASHBOARD_SERVICE
+from harp.utils.commandline import click
 
 
 def _get_service_name_for_humans(x: str):
     if ":" in x:
         return x.split(":", 1)[1]
     return x
 
@@ -20,31 +19,28 @@
 
 def assert_development_packages_are_available():
     assert_package_is_available("honcho")
     assert_package_is_available("watchfiles")
 
 
 @click.command(short_help="Starts the development environment.")
-@click.option("--set", "options", default=(), multiple=True, help="Set proxy configuration options.")
-@click.option("--file", "-f", "files", default=(), multiple=True, help="Load configuration from file.")
-@click.option("--disable", default=(), multiple=True, help="Disable some applications.")
-@click.option("--with-docs/--no-docs", default=False)
-@click.option("--with-ui/--no-ui", default=False)
+@click.option("--with-docs/--no-docs", default=False, help="Append the sphinx doc process to the default process list.")
+@click.option("--with-ui/--no-ui", default=False, help="Append the storybook process to the default process list.")
 # TODO maybe run reset as a pre-start command, so it does not run on each reload?
-@click.option("--reset", is_flag=True, help="Reset the database (drop and recreate tables).")
 @click.option("--mock", is_flag=True, help="Enable mock data instead of real api data (dashboard).")
 @click.option(
     "--server-subprocess",
     "-XS",
     "server_subprocesses",
     multiple=True,
     help="Add a server subprocess to the list of services to start.",
 )
 @click.argument("services", nargs=-1)
-def start(with_docs, with_ui, options, files, disable, services, server_subprocesses, reset, mock):
+@add_harp_server_click_options
+def start(with_docs, with_ui, services, server_subprocesses, mock, **kwargs):
     try:
         assert_development_packages_are_available()
     except ModuleNotFoundError as exc:
         raise click.UsageError(
             "\n".join(
                 (
                     "You must install development dependencies to start the development environment.",
@@ -62,25 +58,18 @@
     )
 
     more_env = {}
 
     if not mock:
         more_env.setdefault(HARP_DASHBOARD_SERVICE, {})["DISABLE_MOCKS"] = "true"
 
-    options = dict(map(lambda x: x.split("=", 1), options))
+    options = ServerOptions(**kwargs)
+
     manager_factory = HonchoManagerFactory(
-        proxy_options=list(
-            chain(
-                ("--set {key} {value}".format(key=key, value=value) for key, value in options.items()),
-                ("--disable {app}".format(app=app) for app in disable),
-                ("-f " + file for file in files),
-                (("--set storage.drop_tables true",) if reset else ()),
-            )
-        ),
-        dashboard_devserver_port=options.get("dashboard.devserver_port", None),
+        proxy_options=options.as_list(), dashboard_devserver_port=options.get("dashboard.devserver_port", None)
     )
 
     services = {f"harp:{_name}" for _name in services or ()} or set(manager_factory.defaults)
     if with_docs or HARP_DOCS_SERVICE in services:
         services.add(HARP_DOCS_SERVICE)
     if with_ui or HARP_UI_SERVICE in services:
         services.add(HARP_UI_SERVICE)
```

### Comparing `harp_proxy-0.5.0b5/harp/commandline/utils/_hacks.py` & `harp_proxy-0.5.0b6/harp/commandline/utils/_hacks.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/commandline/utils/manager.py` & `harp_proxy-0.5.0b6/harp/commandline/utils/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os
+import shlex
 import sys
 from string import Template
 
 import rich_click as click
 
 from harp import ROOT_DIR
 from harp.utils.network import get_available_network_port
 
 HARP_DASHBOARD_SERVICE = "harp:dashboard"
 HARP_DOCS_SERVICE = "harp:docs"
 HARP_SERVER_SERVICE = "harp:server"
 HARP_UI_SERVICE = "harp:ui"
 
 
+def quote(x):
+    return shlex.quote(str(x))
+
+
 class HonchoManagerFactory:
     names = {HARP_DASHBOARD_SERVICE, HARP_SERVER_SERVICE, HARP_DOCS_SERVICE, HARP_UI_SERVICE}
     defaults = {HARP_DASHBOARD_SERVICE, HARP_SERVER_SERVICE}
     commands = {}
 
     def __init__(self, *, proxy_options=(), dashboard_devserver_port=None):
         self.ports = {HARP_DASHBOARD_SERVICE: dashboard_devserver_port or get_available_network_port()}
@@ -49,23 +54,23 @@
                 ]
             ),
         )
 
     commands[HARP_DASHBOARD_SERVICE] = _get_dashboard_executable
 
     def _get_server_executable(self, processes):
-        cmd = f"{sys.executable} bin/entrypoint"
+        cmd = f"{sys.executable} -m harp server"
         proxy_options = list(self.proxy_options)
 
         if HARP_DASHBOARD_SERVICE in processes:
-            proxy_options.append(f"--set dashboard.devserver_port {self.ports[HARP_DASHBOARD_SERVICE]}")
+            proxy_options.append(f"--set dashboard.devserver_port={quote(self.ports[HARP_DASHBOARD_SERVICE])}")
 
         for _name, _port in self.proxy_ports.items():
-            proxy_options.append(f"--set proxy.endpoints.{_port}.name {_name}")
-            proxy_options.append(f"--set proxy.endpoints.{_port}.url http://localhost:{self.ports[_name]}")
+            proxy_options.append(f"--set proxy.endpoints.{_port}.name={quote(_name)}")
+            proxy_options.append(f"--set proxy.endpoints.{_port}.url={quote(f'http://localhost:{self.ports[_name]}')}")
 
         if proxy_options:
             cmd += " " + " ".join(proxy_options)
 
         return ROOT_DIR, f'watchfiles --filter python "{cmd}" harp harp_apps'
 
     commands[HARP_SERVER_SERVICE] = _get_server_executable
```

### Comparing `harp_proxy-0.5.0b5/harp/config/__init__.py` & `harp_proxy-0.5.0b6/harp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/application.py` & `harp_proxy-0.5.0b6/harp/config/application.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/config.py` & `harp_proxy-0.5.0b6/harp/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Factory configuration, does nothing but can be used to instanciate a server.
 """
 
 import importlib.util
 import os
 import pprint
-from argparse import ArgumentParser
 from copy import deepcopy
 from types import MappingProxyType
 from typing import Self, Type
 
 import orjson
 from config.ini import INIFile
 from config.json import JSONFile
 from config.toml import TOMLFile
 from rodi import Container
 from whistle import IAsyncEventDispatcher
 
 from harp import get_logger
+from harp.commandline.server import ServerOptions
 from harp.config.application import Application
 from harp.utils.identifiers import is_valid_dotted_identifier
 
 logger = get_logger(__name__)
 
 
 def get_application_class_name(name):
@@ -99,72 +99,52 @@
         if not is_valid_dotted_identifier(name):
             raise ValueError(f"Invalid application name: {name}")
         self.reset()
         if name in self._raw_settings["applications"]:
             self._raw_settings["applications"].remove(name)
         self._debug_applications.discard(name)
 
-    def read_env(self, args=None):
+    def read_env(
+        self,
+        options: ServerOptions,
+        /,
+    ):
         """
         Parses sys.argv-like arguments.
 
         :param args:
+        :param files: list of filenames to load in order. Will happen after defaults env and files.
         :return: argparse.Namespace
 
         """
-        if not args:
-            args = []
-
-        parser = ArgumentParser()
-        parser.add_argument(
-            "--set",
-            "-s",
-            action="append",
-            dest="values",
-            nargs=2,
-            metavar=("KEY", "VALUE"),
-            help="Set a configuration value.",
-        )
-        parser.add_argument(
-            "--file",
-            "-f",
-            action="append",
-            dest="files",
-            help="Load configuration from file.",
-        )
-        parser.add_argument(
-            "--disable",
-            "-D",
-            action="append",
-            dest="disabled_applications",
-            help="Disable an application.",
-        )
-        options = parser.parse_args(args)
-
-        for disabled_application in options.disabled_applications or ():
-            self.remove_application(disabled_application)
+        for _enabaled_application in options.enable or ():
+            self.add_application(_enabaled_application)
+        for _disabled_application in options.disable or ():
+            self.remove_application(_disabled_application)
 
         from config.common import ConfigurationBuilder, MapSource
         from config.env import EnvVars
         from config.yaml import YAMLFile
 
         builder = ConfigurationBuilder()
 
         # default config
         builder.add_source(MapSource({}))
         builder.add_source(EnvVars(prefix="DEFAULT__HARP_"))
 
         # current
         builder.add_source(MapSource(self._raw_settings))
 
+        # load default system config (if present)
         if os.path.exists("/etc/harp.yaml"):
             builder.add_source(YAMLFile("/etc/harp.yaml"))
         elif os.path.exists("/etc/harp.yml"):
             builder.add_source(YAMLFile("/etc/harp.yml"))
 
+        # load user config
         for file in options.files or ():
             _, ext = os.path.splitext(file)
             if ext in (".yaml", ".yml"):
                 builder.add_source(YAMLFile(file))
             elif ext in (".json",):
                 builder.add_source(JSONFile(file))
             elif ext in (".ini", ".conf"):
@@ -172,19 +152,32 @@
             elif ext in (".toml",):
                 builder.add_source(TOMLFile(file))
             else:
                 raise ValueError(f"Unknown file extension: {ext}")
 
         builder.add_source(EnvVars(prefix="HARP_"))
 
-        for k, v in options.values or ():
+        for k, v in (options.options or {}).items():
             builder.add_value(k, v)
 
         self._raw_settings = builder.build().values
 
+        self._raw_settings.setdefault("proxy", {})
+        self._raw_settings["proxy"].setdefault("endpoints", [])
+
+        for k, v in (options.endpoints or {}).items():
+            _port, _url = v.split(":", 1)
+            self._raw_settings["proxy"]["endpoints"].append(
+                {
+                    "name": k,
+                    "port": int(_port),
+                    "url": _url,
+                }
+            )
+
     def validate(self):
         if self._validated_settings is None:
             to_be_validated = deepcopy(self._raw_settings)
             application_names = to_be_validated.pop("applications", [])
             validated = {"applications": []}
 
             # round 1: import applications and set defaults before validation
```

### Comparing `harp_proxy-0.5.0b5/harp/config/events.py` & `harp_proxy-0.5.0b6/harp/config/events.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/factories/kernel_factory.py` & `harp_proxy-0.5.0b6/harp/config/factories/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/factories/tests/test_configuration.py` & `harp_proxy-0.5.0b6/harp/config/factories/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/factories/tests/test_settings.py` & `harp_proxy-0.5.0b6/harp/config/factories/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/config/settings/from_file.py` & `harp_proxy-0.5.0b6/harp/config/settings/from_file.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/controllers/__init__.py` & `harp_proxy-0.5.0b6/harp/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/controllers/default.py` & `harp_proxy-0.5.0b6/harp/controllers/default.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/controllers/resolvers.py` & `harp_proxy-0.5.0b6/harp/controllers/resolvers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/controllers/routing.py` & `harp_proxy-0.5.0b6/harp/controllers/routing.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/event_dispatcher.py` & `harp_proxy-0.5.0b6/harp/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/__init__.py` & `harp_proxy-0.5.0b6/harp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/errors.py` & `harp_proxy-0.5.0b6/harp/http/errors.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/requests.py` & `harp_proxy-0.5.0b6/harp/http/requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/responses.py` & `harp_proxy-0.5.0b6/harp/http/responses.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/serializers.py` & `harp_proxy-0.5.0b6/harp/http/serializers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/tests/stubs.py` & `harp_proxy-0.5.0b6/harp/http/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/tests/test_requests.py` & `harp_proxy-0.5.0b6/harp/http/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/tests/test_requests_wrapped.py` & `harp_proxy-0.5.0b6/harp/http/tests/test_requests_wrapped.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/tests/test_utils_cookies.py` & `harp_proxy-0.5.0b6/harp/http/tests/test_utils_cookies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/typing/bridges.py` & `harp_proxy-0.5.0b6/harp/http/typing/bridges.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/typing/messages.py` & `harp_proxy-0.5.0b6/harp/http/typing/messages.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/utils/cookies.py` & `harp_proxy-0.5.0b6/harp/http/utils/cookies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/http/utils/methods.py` & `harp_proxy-0.5.0b6/harp/http/utils/methods.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/meta/__init__.py` & `harp_proxy-0.5.0b6/harp/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/models/blobs.py` & `harp_proxy-0.5.0b6/harp/models/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/models/transactions.py` & `harp_proxy-0.5.0b6/harp/models/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/tests/test_asgi_kernel.py` & `harp_proxy-0.5.0b6/harp/tests/test_asgi_kernel.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/tests/test_settings.py` & `harp_proxy-0.5.0b6/harp/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/typing/storage.py` & `harp_proxy-0.5.0b6/harp/typing/storage.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/background.py` & `harp_proxy-0.5.0b6/harp/utils/background.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/collections.py` & `harp_proxy-0.5.0b6/harp/utils/collections.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/dates.py` & `harp_proxy-0.5.0b6/harp/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/network.py` & `harp_proxy-0.5.0b6/harp/utils/network.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/applications.py` & `harp_proxy-0.5.0b6/harp/utils/testing/applications.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/benchmarking.py` & `harp_proxy-0.5.0b6/harp/utils/testing/benchmarking.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/communicators/asgi.py` & `harp_proxy-0.5.0b6/harp/utils/testing/communicators/asgi.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/communicators/http.py` & `harp_proxy-0.5.0b6/harp/utils/testing/communicators/http.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/http.py` & `harp_proxy-0.5.0b6/harp/utils/testing/http.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/mixins/controllers.py` & `harp_proxy-0.5.0b6/harp/utils/testing/mixins/controllers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/testing/stub_api/__init__.py` & `harp_proxy-0.5.0b6/harp/utils/testing/stub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/tests/test_collections.py` & `harp_proxy-0.5.0b6/harp/utils/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/utils/tests/test_dates.py` & `harp_proxy-0.5.0b6/harp/utils/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp/views/json.py` & `harp_proxy-0.5.0b6/harp/views/json.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/contrib/sentry/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/contrib/sentry/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/__init__.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         self.storage = storage
         self.global_settings = all_settings
         self.settings = local_settings
 
         # create users if they don't exist
         if isinstance(self.settings.auth, DashboardAuthBasicSetting):
             asyncio.create_task(self.storage.create_users_once_ready(self.settings.auth.users))
+        else:
+            asyncio.create_task(self.storage.create_users_once_ready({"anonymous": None}))
 
         # controllers for delegating requests
         if self.settings.devserver_port:
             self._ui_devserver_proxy_controller = self._create_ui_devserver_proxy_controller(
                 port=self.settings.devserver_port
             )
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/blobs.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/overview.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/overview.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/system.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/system.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/controllers/transactions.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/controllers/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/docs/development/tests_e2e.rst` & `harp_proxy-0.5.0b6/harp_apps/dashboard/docs/development/tests_e2e.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/docs/development/tests_unit.rst` & `harp_proxy-0.5.0b6/harp_apps/dashboard/docs/development/tests_unit.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/docs/index.rst` & `harp_proxy-0.5.0b6/harp_apps/dashboard/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/filters/base.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/filters/base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/filters/transaction_endpoint.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/filters/transaction_endpoint.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/settings.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_controllers_blobs.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_controllers_blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_controllers_transactions.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_controllers_transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_settings.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/tests/test_utils_dependencies.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/tests/test_utils_dependencies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/tests/utils/test_dates.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/utils/dates.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/utils/dependencies.py` & `harp_proxy-0.5.0b6/harp_apps/dashboard/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/dateFns-s2EURlY7.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/dateFns-s2EURlY7.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/index-BOfsip6N.css` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/index-sYClmDC3.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:Lato,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}[type=text],input:where(:not([type])),[type=email],[type=url],[type=password],[type=number],[type=date],[type=datetime-local],[type=month],[type=search],[type=tel],[type=time],[type=week],[multiple],textarea,select{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}[type=text]:focus,input:where(:not([type])):focus,[type=email]:focus,[type=url]:focus,[type=password]:focus,[type=number]:focus,[type=date]:focus,[type=datetime-local]:focus,[type=month]:focus,[type=search]:focus,[type=tel]:focus,[type=time]:focus,[type=week]:focus,[multiple]:focus,textarea:focus,select:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}input::-moz-placeholder,textarea::-moz-placeholder{color:#6b7280;opacity:1}input::placeholder,textarea::placeholder{color:#6b7280;opacity:1}::-webkit-datetime-edit-fields-wrapper{padding:0}::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}::-webkit-datetime-edit{display:inline-flex}::-webkit-datetime-edit,::-webkit-datetime-edit-year-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute-field,::-webkit-datetime-edit-second-field,::-webkit-datetime-edit-millisecond-field,::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}select{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 20 20'%3e%3cpath stroke='%236b7280' stroke-linecap='round' stroke-linejoin='round' stroke-width='1.5' d='M6 8l4 4 4-4'/%3e%3c/svg%3e");background-position:right .5rem center;background-repeat:no-repeat;background-size:1.5em 1.5em;padding-right:2.5rem;-webkit-print-color-adjust:exact;print-color-adjust:exact}[multiple],[size]:where(select:not([size="1"])){background-image:initial;background-position:initial;background-repeat:unset;background-size:initial;padding-right:.75rem;-webkit-print-color-adjust:unset;print-color-adjust:unset}[type=checkbox],[type=radio]{-webkit-appearance:none;-moz-appearance:none;appearance:none;padding:0;-webkit-print-color-adjust:exact;print-color-adjust:exact;display:inline-block;vertical-align:middle;background-origin:border-box;-webkit-user-select:none;-moz-user-select:none;user-select:none;flex-shrink:0;height:1rem;width:1rem;color:#2563eb;background-color:#fff;border-color:#6b7280;border-width:1px;--tw-shadow: 0 0 #0000}[type=checkbox]{border-radius:0}[type=radio]{border-radius:100%}[type=checkbox]:focus,[type=radio]:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 2px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow)}[type=checkbox]:checked,[type=radio]:checked{border-color:transparent;background-color:currentColor;background-size:100% 100%;background-position:center;background-repeat:no-repeat}[type=checkbox]:checked{background-image:url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3cpath d='M12.207 4.793a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-2-2a1 1 0 011.414-1.414L6.5 9.086l4.293-4.293a1 1 0 011.414 0z'/%3e%3c/svg%3e")}@media (forced-colors: active){[type=checkbox]:checked{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=radio]:checked{background-image:url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3ccircle cx='8' cy='8' r='3'/%3e%3c/svg%3e")}@media (forced-colors: active){[type=radio]:checked{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=checkbox]:checked:hover,[type=checkbox]:checked:focus,[type=radio]:checked:hover,[type=radio]:checked:focus{border-color:transparent;background-color:currentColor}[type=checkbox]:indeterminate{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 16 16'%3e%3cpath stroke='white' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M4 8h8'/%3e%3c/svg%3e");border-color:transparent;background-color:currentColor;background-size:100% 100%;background-position:center;background-repeat:no-repeat}@media (forced-colors: active){[type=checkbox]:indeterminate{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=checkbox]:indeterminate:hover,[type=checkbox]:indeterminate:focus{border-color:transparent;background-color:currentColor}[type=file]{background:unset;border-color:inherit;border-width:0;border-radius:0;padding:0;font-size:unset;line-height:inherit}[type=file]:focus{outline:1px solid ButtonText;outline:1px auto -webkit-focus-ring-color}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{width:100%}@media (min-width: 640px){.container{max-width:640px}}@media (min-width: 768px){.container{max-width:768px}}@media (min-width: 1024px){.container{max-width:1024px}}@media (min-width: 1280px){.container{max-width:1280px}}@media (min-width: 1536px){.container{max-width:1536px}}.prose{color:var(--tw-prose-body);max-width:65ch}.prose :where(p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where([class~=lead]):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-lead);font-size:1.25em;line-height:1.6;margin-top:1.2em;margin-bottom:1.2em}.prose :where(a):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-links);text-decoration:underline;font-weight:500}.prose :where(strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-bold);font-weight:600}.prose :where(a strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(ol):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal;margin-top:1.25em;margin-bottom:1.25em;padding-inline-start:1.625em}.prose :where(ol[type=A]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=A s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=I]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type=I s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type="1"]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal}.prose :where(ul):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-inline-start:1.625em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{font-weight:400;color:var(--tw-prose-counters)}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{color:var(--tw-prose-bullets)}.prose :where(dt):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.25em}.prose :where(hr):not(:where([class~=not-prose],[class~=not-prose] *)){border-color:var(--tw-prose-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.prose :where(blockquote):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-style:italic;color:var(--tw-prose-quotes);border-inline-start-width:.25rem;border-inline-start-color:var(--tw-prose-quote-borders);quotes:"“""”""‘""’";margin-top:1.6em;margin-bottom:1.6em;padding-inline-start:1em}.prose :where(blockquote p:first-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:open-quote}.prose :where(blockquote p:last-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:close-quote}.prose :where(h1):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.prose :where(h1 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:900;color:inherit}.prose :where(h2):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.prose :where(h2 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:800;color:inherit}.prose :where(h3):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.prose :where(h3 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(h4):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.prose :where(h4 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(picture):not(:where([class~=not-prose],[class~=not-prose] *)){display:block;margin-top:2em;margin-bottom:2em}.prose :where(video):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(kbd):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-family:inherit;color:var(--tw-prose-kbd);box-shadow:0 0 0 1px rgb(var(--tw-prose-kbd-shadows) / 10%),0 3px rgb(var(--tw-prose-kbd-shadows) / 10%);font-size:.875em;border-radius:.3125rem;padding-top:.1875em;padding-inline-end:.375em;padding-bottom:.1875em;padding-inline-start:.375em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-code);font-weight:600;font-size:.875em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:"`"}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:"`"}.prose :where(a code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h1 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h2 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.875em}.prose :where(h3 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.9em}.prose :where(h4 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(pre):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-pre-code);background-color:var(--tw-prose-pre-bg);overflow-x:auto;font-weight:400;font-size:.875em;line-height:1.7142857;margin-top:1.7142857em;margin-bottom:1.7142857em;border-radius:.375rem;padding-top:.8571429em;padding-inline-end:1.1428571em;padding-bottom:.8571429em;padding-inline-start:1.1428571em}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)){background-color:transparent;border-width:0;border-radius:0;padding:0;font-weight:inherit;color:inherit;font-size:inherit;font-family:inherit;line-height:inherit}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:none}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:none}.prose :where(table):not(:where([class~=not-prose],[class~=not-prose] *)){width:100%;table-layout:auto;text-align:start;margin-top:2em;margin-bottom:2em;font-size:.875em;line-height:1.7142857}.prose :where(thead):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-th-borders)}.prose :where(thead th):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;vertical-align:bottom;padding-inline-end:.5714286em;padding-bottom:.5714286em;padding-inline-start:.5714286em}.prose :where(tbody tr):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-td-borders)}.prose :where(tbody tr:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:0}.prose :where(tbody td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:baseline}.prose :where(tfoot):not(:where([class~=not-prose],[class~=not-prose] *)){border-top-width:1px;border-top-color:var(--tw-prose-th-borders)}.prose :where(tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:top}.prose :where(figure>*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(figcaption):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-captions);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.prose{--tw-prose-body: #374151;--tw-prose-headings: #111827;--tw-prose-lead: #4b5563;--tw-prose-links: #111827;--tw-prose-bold: #111827;--tw-prose-counters: #6b7280;--tw-prose-bullets: #d1d5db;--tw-prose-hr: #e5e7eb;--tw-prose-quotes: #111827;--tw-prose-quote-borders: #e5e7eb;--tw-prose-captions: #6b7280;--tw-prose-kbd: #111827;--tw-prose-kbd-shadows: 17 24 39;--tw-prose-code: #111827;--tw-prose-pre-code: #e5e7eb;--tw-prose-pre-bg: #1f2937;--tw-prose-th-borders: #d1d5db;--tw-prose-td-borders: #e5e7eb;--tw-prose-invert-body: #d1d5db;--tw-prose-invert-headings: #fff;--tw-prose-invert-lead: #9ca3af;--tw-prose-invert-links: #fff;--tw-prose-invert-bold: #fff;--tw-prose-invert-counters: #9ca3af;--tw-prose-invert-bullets: #4b5563;--tw-prose-invert-hr: #374151;--tw-prose-invert-quotes: #f3f4f6;--tw-prose-invert-quote-borders: #374151;--tw-prose-invert-captions: #9ca3af;--tw-prose-invert-kbd: #fff;--tw-prose-invert-kbd-shadows: 255 255 255;--tw-prose-invert-code: #fff;--tw-prose-invert-pre-code: #d1d5db;--tw-prose-invert-pre-bg: rgb(0 0 0 / 50%);--tw-prose-invert-th-borders: #4b5563;--tw-prose-invert-td-borders: #374151;font-size:1rem;line-height:1.75}.prose :where(picture>img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(li):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;margin-bottom:.5em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:.375em}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:.375em}.prose :where(.prose>ul>li p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(.prose>ul>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ul>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(.prose>ol>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ol>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(dl):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where(dd):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;padding-inline-start:1.625em}.prose :where(hr+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h2+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h3+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h4+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(thead th:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:0}.prose :where(thead th:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-end:0}.prose :where(tbody td,tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){padding-top:.5714286em;padding-inline-end:.5714286em;padding-bottom:.5714286em;padding-inline-start:.5714286em}.prose :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:0}.prose :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-end:0}.prose :where(figure):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(.prose>:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(.prose>:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:0}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.invisible{visibility:hidden}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.-inset-0{top:-0px;right:-0px;bottom:-0px;left:-0px}.-inset-0\.5{top:-.125rem;right:-.125rem;bottom:-.125rem;left:-.125rem}.inset-y-0{top:0;bottom:0}.left-0{left:0}.right-0{right:0}.top-8{top:2rem}.isolate{isolation:isolate}.z-10{z-index:10}.order-first{order:-9999}.order-last{order:9999}.m-2{margin:.5rem}.m-4{margin:1rem}.mx-1{margin-left:.25rem;margin-right:.25rem}.mx-auto{margin-left:auto;margin-right:auto}.my-2{margin-top:.5rem;margin-bottom:.5rem}.my-5{margin-top:1.25rem;margin-bottom:1.25rem}.\!ml-1{margin-left:.25rem!important}.-ml-px{margin-left:-1px}.mb-2{margin-bottom:.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.ml-10{margin-left:2.5rem}.ml-2{margin-left:.5rem}.ml-24{margin-left:6rem}.ml-3{margin-left:.75rem}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mt-10{margin-top:2.5rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.block{display:block}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.grid{display:grid}.hidden{display:none}.size-5{width:1.25rem;height:1.25rem}.h-12{height:3rem}.h-14{height:3.5rem}.h-3{height:.75rem}.h-32{height:8rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-screen{height:100vh}.max-h-screen{max-height:100vh}.min-h-screen{min-height:100vh}.w-1{width:.25rem}.w-1\/2{width:50%}.w-1\/5{width:20%}.w-2\/5{width:40%}.w-3{width:.75rem}.w-4{width:1rem}.w-5{width:1.25rem}.w-6{width:1.5rem}.w-96{width:24rem}.w-auto{width:auto}.w-fit{width:-moz-fit-content;width:fit-content}.w-full{width:100%}.w-screen{width:100vw}.min-w-4{min-width:1rem}.min-w-40{min-width:10rem}.min-w-96{min-width:24rem}.min-w-fit{min-width:-moz-fit-content;min-width:fit-content}.min-w-full{min-width:100%}.max-w-60{max-width:15rem}.max-w-7xl{max-width:80rem}.max-w-full{max-width:100%}.flex-1{flex:1 1 0%}.flex-shrink-0,.shrink-0{flex-shrink:0}.grow{flex-grow:1}.rotate-90{--tw-rotate: 90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.cursor-pointer{cursor:pointer}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}.grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-end{align-items:flex-end}.items-center{align-items:center}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-4{gap:1rem}.gap-x-3{-moz-column-gap:.75rem;column-gap:.75rem}.gap-x-8{-moz-column-gap:2rem;column-gap:2rem}.-space-x-px>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(-1px * var(--tw-space-x-reverse));margin-left:calc(-1px * calc(1 - var(--tw-space-x-reverse)))}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(.25rem * var(--tw-space-x-reverse));margin-left:calc(.25rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(.5rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(.5rem * var(--tw-space-y-reverse))}.space-y-4>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 0;border-top-width:calc(1px * calc(1 - var(--tw-divide-y-reverse)));border-bottom-width:calc(1px * var(--tw-divide-y-reverse))}.divide-gray-100>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(243 244 246 / var(--tw-divide-opacity))}.divide-gray-200>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(229 231 235 / var(--tw-divide-opacity))}.divide-gray-300>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(209 213 219 / var(--tw-divide-opacity))}.self-center{align-self:center}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-x-auto{overflow-x:auto}.overflow-y-auto{overflow-y:auto}.truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.overflow-ellipsis{text-overflow:ellipsis}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l-md{border-top-left-radius:.375rem;border-bottom-left-radius:.375rem}.rounded-r-md{border-top-right-radius:.375rem;border-bottom-right-radius:.375rem}.rounded-t-sm{border-top-left-radius:.125rem;border-top-right-radius:.125rem}.\!border-0{border-width:0px!important}.border{border-width:1px}.border-0{border-width:0px}.border-b{border-bottom-width:1px}.border-b-0{border-bottom-width:0px}.border-b-4{border-bottom-width:4px}.border-t{border-top-width:1px}.border-t-0{border-top-width:0px}.border-gray-200{--tw-border-opacity: 1;border-color:rgb(229 231 235 / var(--tw-border-opacity))}.border-gray-300{--tw-border-opacity: 1;border-color:rgb(209 213 219 / var(--tw-border-opacity))}.border-primary-900{--tw-border-opacity: 1;border-color:rgb(6 95 159 / var(--tw-border-opacity))}.border-transparent{border-color:transparent}.bg-amber-500{--tw-bg-opacity: 1;background-color:rgb(245 158 11 / var(--tw-bg-opacity))}.bg-blue-50{--tw-bg-opacity: 1;background-color:rgb(239 246 255 / var(--tw-bg-opacity))}.bg-blue-600{--tw-bg-opacity: 1;background-color:rgb(37 99 235 / var(--tw-bg-opacity))}.bg-emerald-400{--tw-bg-opacity: 1;background-color:rgb(52 211 153 / var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity: 1;background-color:rgb(249 250 251 / var(--tw-bg-opacity))}.bg-green-50{--tw-bg-opacity: 1;background-color:rgb(240 253 244 / var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity: 1;background-color:rgb(34 197 94 / var(--tw-bg-opacity))}.bg-lime-500{--tw-bg-opacity: 1;background-color:rgb(132 204 22 / var(--tw-bg-opacity))}.bg-orange-50{--tw-bg-opacity: 1;background-color:rgb(255 247 237 / var(--tw-bg-opacity))}.bg-orange-500{--tw-bg-opacity: 1;background-color:rgb(249 115 22 / var(--tw-bg-opacity))}.bg-primary-600{--tw-bg-opacity: 1;background-color:rgb(21 164 233 / var(--tw-bg-opacity))}.bg-primary-900{--tw-bg-opacity: 1;background-color:rgb(6 95 159 / var(--tw-bg-opacity))}.bg-purple-50{--tw-bg-opacity: 1;background-color:rgb(250 245 255 / var(--tw-bg-opacity))}.bg-red-50{--tw-bg-opacity: 1;background-color:rgb(254 242 242 / var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity: 1;background-color:rgb(239 68 68 / var(--tw-bg-opacity))}.bg-red-700{--tw-bg-opacity: 1;background-color:rgb(185 28 28 / var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity: 1;background-color:rgb(241 245 249 / var(--tw-bg-opacity))}.bg-teal-400{--tw-bg-opacity: 1;background-color:rgb(45 212 191 / var(--tw-bg-opacity))}.bg-transparent{background-color:transparent}.bg-white{--tw-bg-opacity: 1;background-color:rgb(255 255 255 / var(--tw-bg-opacity))}.bg-yellow-50{--tw-bg-opacity: 1;background-color:rgb(254 252 232 / var(--tw-bg-opacity))}.bg-yellow-500{--tw-bg-opacity: 1;background-color:rgb(234 179 8 / var(--tw-bg-opacity))}.fill-current{fill:currentColor}.\!p-0{padding:0!important}.p-2{padding:.5rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-2\.5{padding-left:.625rem;padding-right:.625rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.py-0{padding-top:0;padding-bottom:0}.py-0\.5{padding-top:.125rem;padding-bottom:.125rem}.py-1{padding-top:.25rem;padding-bottom:.25rem}.py-1\.5{padding-top:.375rem;padding-bottom:.375rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-3\.5{padding-top:.875rem;padding-bottom:.875rem}.pb-4{padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pl-1{padding-left:.25rem}.pl-1\.5{padding-left:.375rem}.pr-1{padding-right:.25rem}.pr-1\.5{padding-right:.375rem}.pr-2{padding-right:.5rem}.pr-6{padding-right:1.5rem}.pt-0{padding-top:0}.pt-1{padding-top:.25rem}.text-left{text-align:left}.text-right{text-align:right}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-text-bottom{vertical-align:text-bottom}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:Lato,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji"}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-4xl{font-size:2.25rem;line-height:2.5rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-light{font-weight:300}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.leading-6{line-height:1.5rem}.text-black{--tw-text-opacity: 1;color:rgb(0 0 0 / var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity: 1;color:rgb(59 130 246 / var(--tw-text-opacity))}.text-blue-600{--tw-text-opacity: 1;color:rgb(37 99 235 / var(--tw-text-opacity))}.text-blue-700{--tw-text-opacity: 1;color:rgb(29 78 216 / var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity: 1;color:rgb(209 213 219 / var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity: 1;color:rgb(107 114 128 / var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity: 1;color:rgb(75 85 99 / var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity: 1;color:rgb(55 65 81 / var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity: 1;color:rgb(17 24 39 / var(--tw-text-opacity))}.text-green-500{--tw-text-opacity: 1;color:rgb(34 197 94 / var(--tw-text-opacity))}.text-green-700{--tw-text-opacity: 1;color:rgb(21 128 61 / var(--tw-text-opacity))}.text-indigo-600{--tw-text-opacity: 1;color:rgb(79 70 229 / var(--tw-text-opacity))}.text-orange-700{--tw-text-opacity: 1;color:rgb(194 65 12 / var(--tw-text-opacity))}.text-primary-900{--tw-text-opacity: 1;color:rgb(6 95 159 / var(--tw-text-opacity))}.text-purple-500{--tw-text-opacity: 1;color:rgb(168 85 247 / var(--tw-text-opacity))}.text-purple-700{--tw-text-opacity: 1;color:rgb(126 34 206 / var(--tw-text-opacity))}.text-red-500{--tw-text-opacity: 1;color:rgb(239 68 68 / var(--tw-text-opacity))}.text-red-700{--tw-text-opacity: 1;color:rgb(185 28 28 / var(--tw-text-opacity))}.text-white{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity))}.text-yellow-500{--tw-text-opacity: 1;color:rgb(234 179 8 / var(--tw-text-opacity))}.text-yellow-700{--tw-text-opacity: 1;color:rgb(161 98 7 / var(--tw-text-opacity))}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.shadow-sm{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.ring-1{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-2{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-inset{--tw-ring-inset: inset}.ring-black{--tw-ring-opacity: 1;--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity))}.ring-blue-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(191 219 254 / var(--tw-ring-opacity))}.ring-blue-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(59 130 246 / var(--tw-ring-opacity))}.ring-blue-600\/20{--tw-ring-color: rgb(37 99 235 / .2)}.ring-blue-700{--tw-ring-opacity: 1;--tw-ring-color: rgb(29 78 216 / var(--tw-ring-opacity))}.ring-gray-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(229 231 235 / var(--tw-ring-opacity))}.ring-gray-300{--tw-ring-opacity: 1;--tw-ring-color: rgb(209 213 219 / var(--tw-ring-opacity))}.ring-gray-600\/20{--tw-ring-color: rgb(75 85 99 / .2)}.ring-green-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(34 197 94 / var(--tw-ring-opacity))}.ring-green-600\/20{--tw-ring-color: rgb(22 163 74 / .2)}.ring-orange-600\/20{--tw-ring-color: rgb(234 88 12 / .2)}.ring-purple-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(168 85 247 / var(--tw-ring-opacity))}.ring-purple-600\/20{--tw-ring-color: rgb(147 51 234 / .2)}.ring-red-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(254 202 202 / var(--tw-ring-opacity))}.ring-red-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(239 68 68 / var(--tw-ring-opacity))}.ring-red-600\/20{--tw-ring-color: rgb(220 38 38 / .2)}.ring-white{--tw-ring-opacity: 1;--tw-ring-color: rgb(255 255 255 / var(--tw-ring-opacity))}.ring-yellow-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(234 179 8 / var(--tw-ring-opacity))}.ring-yellow-600\/20{--tw-ring-color: rgb(202 138 4 / .2)}.ring-opacity-5{--tw-ring-opacity: .05}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.debug{outline:1px dot-dash red;border:1px solid red}.placeholder\:text-gray-400::-moz-placeholder{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.placeholder\:text-gray-400::placeholder{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.hover\:cursor-pointer:hover{cursor:pointer}.hover\:border-white:hover{--tw-border-opacity: 1;border-color:rgb(255 255 255 / var(--tw-border-opacity))}.hover\:bg-blue-500:hover{--tw-bg-opacity: 1;background-color:rgb(59 130 246 / var(--tw-bg-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity: 1;background-color:rgb(243 244 246 / var(--tw-bg-opacity))}.hover\:bg-gray-50:hover{--tw-bg-opacity: 1;background-color:rgb(249 250 251 / var(--tw-bg-opacity))}.hover\:bg-slate-50:hover{--tw-bg-opacity: 1;background-color:rgb(248 250 252 / var(--tw-bg-opacity))}.hover\:text-gray-500:hover{--tw-text-opacity: 1;color:rgb(107 114 128 / var(--tw-text-opacity))}.hover\:text-white:hover{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity))}.hover\:text-yellow-500:hover{--tw-text-opacity: 1;color:rgb(234 179 8 / var(--tw-text-opacity))}.focus\:z-10:focus{z-index:10}.focus\:z-20:focus{z-index:20}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:outline-offset-0:focus{outline-offset:0px}.focus\:\!ring-0:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-0:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.focus\:ring-2:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.focus\:ring-inset:focus{--tw-ring-inset: inset}.focus\:ring-indigo-600:focus{--tw-ring-opacity: 1;--tw-ring-color: rgb(79 70 229 / var(--tw-ring-opacity))}.focus\:ring-offset-0:focus{--tw-ring-offset-width: 0px}.focus-visible\:outline:focus-visible{outline-style:solid}.focus-visible\:outline-2:focus-visible{outline-width:2px}.focus-visible\:outline-offset-2:focus-visible{outline-offset:2px}.focus-visible\:outline-blue-500:focus-visible{outline-color:#3b82f6}.focus-visible\:outline-primary-600:focus-visible{outline-color:#15a4e9}@media (min-width: 640px){.sm\:static{position:static}.sm\:inset-auto{inset:auto}.sm\:-mx-6{margin-left:-1.5rem;margin-right:-1.5rem}.sm\:ml-6{margin-left:1.5rem}.sm\:flex{display:flex}.sm\:hidden{display:none}.sm\:flex-1{flex:1 1 0%}.sm\:items-center{align-items:center}.sm\:items-stretch{align-items:stretch}.sm\:justify-start{justify-content:flex-start}.sm\:justify-between{justify-content:space-between}.sm\:space-x-8>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(2rem * var(--tw-space-x-reverse));margin-left:calc(2rem * calc(1 - var(--tw-space-x-reverse)))}.sm\:px-6{padding-left:1.5rem;padding-right:1.5rem}.sm\:pr-0{padding-right:0}.sm\:text-sm{font-size:.875rem;line-height:1.25rem}}@media (min-width: 1024px){.lg\:order-first{order:-9999}.lg\:order-last{order:9999}.lg\:-mx-8{margin-left:-2rem;margin-right:-2rem}.lg\:mt-12{margin-top:3rem}.lg\:block{display:block}.lg\:flex-row{flex-direction:row}.lg\:items-start{align-items:flex-start}.lg\:justify-between{justify-content:space-between}.lg\:px-8{padding-left:2rem;padding-right:2rem}}@media (min-width: 1280px){.xl\:h-40{height:10rem}}@media (min-width: 1536px){.\32xl\:h-48{height:12rem}.\32xl\:min-w-52{min-width:13rem}.\32xl\:max-w-72{max-width:18rem}}
+*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:Lato,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}[type=text],input:where(:not([type])),[type=email],[type=url],[type=password],[type=number],[type=date],[type=datetime-local],[type=month],[type=search],[type=tel],[type=time],[type=week],[multiple],textarea,select{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:#fff;border-color:#6b7280;border-width:1px;border-radius:0;padding:.5rem .75rem;font-size:1rem;line-height:1.5rem;--tw-shadow: 0 0 #0000}[type=text]:focus,input:where(:not([type])):focus,[type=email]:focus,[type=url]:focus,[type=password]:focus,[type=number]:focus,[type=date]:focus,[type=datetime-local]:focus,[type=month]:focus,[type=search]:focus,[type=tel]:focus,[type=time]:focus,[type=week]:focus,[multiple]:focus,textarea:focus,select:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow);border-color:#2563eb}input::-moz-placeholder,textarea::-moz-placeholder{color:#6b7280;opacity:1}input::placeholder,textarea::placeholder{color:#6b7280;opacity:1}::-webkit-datetime-edit-fields-wrapper{padding:0}::-webkit-date-and-time-value{min-height:1.5em;text-align:inherit}::-webkit-datetime-edit{display:inline-flex}::-webkit-datetime-edit,::-webkit-datetime-edit-year-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute-field,::-webkit-datetime-edit-second-field,::-webkit-datetime-edit-millisecond-field,::-webkit-datetime-edit-meridiem-field{padding-top:0;padding-bottom:0}select{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 20 20'%3e%3cpath stroke='%236b7280' stroke-linecap='round' stroke-linejoin='round' stroke-width='1.5' d='M6 8l4 4 4-4'/%3e%3c/svg%3e");background-position:right .5rem center;background-repeat:no-repeat;background-size:1.5em 1.5em;padding-right:2.5rem;-webkit-print-color-adjust:exact;print-color-adjust:exact}[multiple],[size]:where(select:not([size="1"])){background-image:initial;background-position:initial;background-repeat:unset;background-size:initial;padding-right:.75rem;-webkit-print-color-adjust:unset;print-color-adjust:unset}[type=checkbox],[type=radio]{-webkit-appearance:none;-moz-appearance:none;appearance:none;padding:0;-webkit-print-color-adjust:exact;print-color-adjust:exact;display:inline-block;vertical-align:middle;background-origin:border-box;-webkit-user-select:none;-moz-user-select:none;user-select:none;flex-shrink:0;height:1rem;width:1rem;color:#2563eb;background-color:#fff;border-color:#6b7280;border-width:1px;--tw-shadow: 0 0 #0000}[type=checkbox]{border-radius:0}[type=radio]{border-radius:100%}[type=checkbox]:focus,[type=radio]:focus{outline:2px solid transparent;outline-offset:2px;--tw-ring-inset: var(--tw-empty, );--tw-ring-offset-width: 2px;--tw-ring-offset-color: #fff;--tw-ring-color: #2563eb;--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow)}[type=checkbox]:checked,[type=radio]:checked{border-color:transparent;background-color:currentColor;background-size:100% 100%;background-position:center;background-repeat:no-repeat}[type=checkbox]:checked{background-image:url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3cpath d='M12.207 4.793a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-2-2a1 1 0 011.414-1.414L6.5 9.086l4.293-4.293a1 1 0 011.414 0z'/%3e%3c/svg%3e")}@media (forced-colors: active){[type=checkbox]:checked{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=radio]:checked{background-image:url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3ccircle cx='8' cy='8' r='3'/%3e%3c/svg%3e")}@media (forced-colors: active){[type=radio]:checked{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=checkbox]:checked:hover,[type=checkbox]:checked:focus,[type=radio]:checked:hover,[type=radio]:checked:focus{border-color:transparent;background-color:currentColor}[type=checkbox]:indeterminate{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 16 16'%3e%3cpath stroke='white' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M4 8h8'/%3e%3c/svg%3e");border-color:transparent;background-color:currentColor;background-size:100% 100%;background-position:center;background-repeat:no-repeat}@media (forced-colors: active){[type=checkbox]:indeterminate{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}}[type=checkbox]:indeterminate:hover,[type=checkbox]:indeterminate:focus{border-color:transparent;background-color:currentColor}[type=file]{background:unset;border-color:inherit;border-width:0;border-radius:0;padding:0;font-size:unset;line-height:inherit}[type=file]:focus{outline:1px solid ButtonText;outline:1px auto -webkit-focus-ring-color}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{width:100%}@media (min-width: 640px){.container{max-width:640px}}@media (min-width: 768px){.container{max-width:768px}}@media (min-width: 1024px){.container{max-width:1024px}}@media (min-width: 1280px){.container{max-width:1280px}}@media (min-width: 1536px){.container{max-width:1536px}}.prose{color:var(--tw-prose-body);max-width:65ch}.prose :where(p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where([class~=lead]):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-lead);font-size:1.25em;line-height:1.6;margin-top:1.2em;margin-bottom:1.2em}.prose :where(a):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-links);text-decoration:underline;font-weight:500}.prose :where(strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-bold);font-weight:600}.prose :where(a strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th strong):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(ol):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal;margin-top:1.25em;margin-bottom:1.25em;padding-inline-start:1.625em}.prose :where(ol[type=A]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=A s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=I]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type=I s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i s]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type="1"]):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:decimal}.prose :where(ul):not(:where([class~=not-prose],[class~=not-prose] *)){list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-inline-start:1.625em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{font-weight:400;color:var(--tw-prose-counters)}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *))::marker{color:var(--tw-prose-bullets)}.prose :where(dt):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.25em}.prose :where(hr):not(:where([class~=not-prose],[class~=not-prose] *)){border-color:var(--tw-prose-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.prose :where(blockquote):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-style:italic;color:var(--tw-prose-quotes);border-inline-start-width:.25rem;border-inline-start-color:var(--tw-prose-quote-borders);quotes:"“""”""‘""’";margin-top:1.6em;margin-bottom:1.6em;padding-inline-start:1em}.prose :where(blockquote p:first-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:open-quote}.prose :where(blockquote p:last-of-type):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:close-quote}.prose :where(h1):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.prose :where(h1 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:900;color:inherit}.prose :where(h2):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.prose :where(h2 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:800;color:inherit}.prose :where(h3):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.prose :where(h3 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(h4):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.prose :where(h4 strong):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:700;color:inherit}.prose :where(img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(picture):not(:where([class~=not-prose],[class~=not-prose] *)){display:block;margin-top:2em;margin-bottom:2em}.prose :where(video):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(kbd):not(:where([class~=not-prose],[class~=not-prose] *)){font-weight:500;font-family:inherit;color:var(--tw-prose-kbd);box-shadow:0 0 0 1px rgb(var(--tw-prose-kbd-shadows) / 10%),0 3px rgb(var(--tw-prose-kbd-shadows) / 10%);font-size:.875em;border-radius:.3125rem;padding-top:.1875em;padding-inline-end:.375em;padding-bottom:.1875em;padding-inline-start:.375em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-code);font-weight:600;font-size:.875em}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:"`"}.prose :where(code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:"`"}.prose :where(a code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h1 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(h2 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.875em}.prose :where(h3 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit;font-size:.9em}.prose :where(h4 code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(blockquote code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(thead th code):not(:where([class~=not-prose],[class~=not-prose] *)){color:inherit}.prose :where(pre):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-pre-code);background-color:var(--tw-prose-pre-bg);overflow-x:auto;font-weight:400;font-size:.875em;line-height:1.7142857;margin-top:1.7142857em;margin-bottom:1.7142857em;border-radius:.375rem;padding-top:.8571429em;padding-inline-end:1.1428571em;padding-bottom:.8571429em;padding-inline-start:1.1428571em}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)){background-color:transparent;border-width:0;border-radius:0;padding:0;font-weight:inherit;color:inherit;font-size:inherit;font-family:inherit;line-height:inherit}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):before{content:none}.prose :where(pre code):not(:where([class~=not-prose],[class~=not-prose] *)):after{content:none}.prose :where(table):not(:where([class~=not-prose],[class~=not-prose] *)){width:100%;table-layout:auto;text-align:start;margin-top:2em;margin-bottom:2em;font-size:.875em;line-height:1.7142857}.prose :where(thead):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-th-borders)}.prose :where(thead th):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:600;vertical-align:bottom;padding-inline-end:.5714286em;padding-bottom:.5714286em;padding-inline-start:.5714286em}.prose :where(tbody tr):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:1px;border-bottom-color:var(--tw-prose-td-borders)}.prose :where(tbody tr:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){border-bottom-width:0}.prose :where(tbody td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:baseline}.prose :where(tfoot):not(:where([class~=not-prose],[class~=not-prose] *)){border-top-width:1px;border-top-color:var(--tw-prose-th-borders)}.prose :where(tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){vertical-align:top}.prose :where(figure>*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(figcaption):not(:where([class~=not-prose],[class~=not-prose] *)){color:var(--tw-prose-captions);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.prose{--tw-prose-body: #374151;--tw-prose-headings: #111827;--tw-prose-lead: #4b5563;--tw-prose-links: #111827;--tw-prose-bold: #111827;--tw-prose-counters: #6b7280;--tw-prose-bullets: #d1d5db;--tw-prose-hr: #e5e7eb;--tw-prose-quotes: #111827;--tw-prose-quote-borders: #e5e7eb;--tw-prose-captions: #6b7280;--tw-prose-kbd: #111827;--tw-prose-kbd-shadows: 17 24 39;--tw-prose-code: #111827;--tw-prose-pre-code: #e5e7eb;--tw-prose-pre-bg: #1f2937;--tw-prose-th-borders: #d1d5db;--tw-prose-td-borders: #e5e7eb;--tw-prose-invert-body: #d1d5db;--tw-prose-invert-headings: #fff;--tw-prose-invert-lead: #9ca3af;--tw-prose-invert-links: #fff;--tw-prose-invert-bold: #fff;--tw-prose-invert-counters: #9ca3af;--tw-prose-invert-bullets: #4b5563;--tw-prose-invert-hr: #374151;--tw-prose-invert-quotes: #f3f4f6;--tw-prose-invert-quote-borders: #374151;--tw-prose-invert-captions: #9ca3af;--tw-prose-invert-kbd: #fff;--tw-prose-invert-kbd-shadows: 255 255 255;--tw-prose-invert-code: #fff;--tw-prose-invert-pre-code: #d1d5db;--tw-prose-invert-pre-bg: rgb(0 0 0 / 50%);--tw-prose-invert-th-borders: #4b5563;--tw-prose-invert-td-borders: #374151;font-size:1rem;line-height:1.75}.prose :where(picture>img):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose :where(li):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;margin-bottom:.5em}.prose :where(ol>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:.375em}.prose :where(ul>li):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:.375em}.prose :where(.prose>ul>li p):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(.prose>ul>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ul>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(.prose>ol>li>*:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ol>li>*:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:1.25em}.prose :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.75em;margin-bottom:.75em}.prose :where(dl):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:1.25em;margin-bottom:1.25em}.prose :where(dd):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:.5em;padding-inline-start:1.625em}.prose :where(hr+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h2+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h3+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(h4+*):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(thead th:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:0}.prose :where(thead th:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-end:0}.prose :where(tbody td,tfoot td):not(:where([class~=not-prose],[class~=not-prose] *)){padding-top:.5714286em;padding-inline-end:.5714286em;padding-bottom:.5714286em;padding-inline-start:.5714286em}.prose :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-start:0}.prose :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){padding-inline-end:0}.prose :where(figure):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:2em;margin-bottom:2em}.prose :where(.prose>:first-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-top:0}.prose :where(.prose>:last-child):not(:where([class~=not-prose],[class~=not-prose] *)){margin-bottom:0}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.invisible{visibility:hidden}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.-inset-0{top:-0px;right:-0px;bottom:-0px;left:-0px}.-inset-0\.5{top:-.125rem;right:-.125rem;bottom:-.125rem;left:-.125rem}.inset-y-0{top:0;bottom:0}.left-0{left:0}.right-0{right:0}.top-8{top:2rem}.isolate{isolation:isolate}.z-10{z-index:10}.order-first{order:-9999}.order-last{order:9999}.m-2{margin:.5rem}.m-4{margin:1rem}.mx-1{margin-left:.25rem;margin-right:.25rem}.mx-auto{margin-left:auto;margin-right:auto}.my-2{margin-top:.5rem;margin-bottom:.5rem}.my-5{margin-top:1.25rem;margin-bottom:1.25rem}.\!ml-1{margin-left:.25rem!important}.-ml-px{margin-left:-1px}.mb-2{margin-bottom:.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.ml-10{margin-left:2.5rem}.ml-2{margin-left:.5rem}.ml-24{margin-left:6rem}.ml-3{margin-left:.75rem}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mt-10{margin-top:2.5rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.block{display:block}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.grid{display:grid}.hidden{display:none}.size-5{width:1.25rem;height:1.25rem}.h-12{height:3rem}.h-14{height:3.5rem}.h-3{height:.75rem}.h-32{height:8rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-screen{height:100vh}.max-h-screen{max-height:100vh}.min-h-screen{min-height:100vh}.w-1{width:.25rem}.w-1\/2{width:50%}.w-1\/5{width:20%}.w-2\/5{width:40%}.w-3{width:.75rem}.w-4{width:1rem}.w-5{width:1.25rem}.w-6{width:1.5rem}.w-96{width:24rem}.w-auto{width:auto}.w-fit{width:-moz-fit-content;width:fit-content}.w-full{width:100%}.w-screen{width:100vw}.min-w-4{min-width:1rem}.min-w-40{min-width:10rem}.min-w-96{min-width:24rem}.min-w-fit{min-width:-moz-fit-content;min-width:fit-content}.min-w-full{min-width:100%}.max-w-0{max-width:0px}.max-w-60{max-width:15rem}.max-w-7xl{max-width:80rem}.max-w-full{max-width:100%}.flex-1{flex:1 1 0%}.flex-shrink-0,.shrink-0{flex-shrink:0}.grow{flex-grow:1}.rotate-90{--tw-rotate: 90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.cursor-pointer{cursor:pointer}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}.grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-end{align-items:flex-end}.items-center{align-items:center}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-4{gap:1rem}.gap-x-3{-moz-column-gap:.75rem;column-gap:.75rem}.gap-x-8{-moz-column-gap:2rem;column-gap:2rem}.-space-x-px>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(-1px * var(--tw-space-x-reverse));margin-left:calc(-1px * calc(1 - var(--tw-space-x-reverse)))}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(.25rem * var(--tw-space-x-reverse));margin-left:calc(.25rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(.5rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(.5rem * var(--tw-space-y-reverse))}.space-y-4>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 0;border-top-width:calc(1px * calc(1 - var(--tw-divide-y-reverse)));border-bottom-width:calc(1px * var(--tw-divide-y-reverse))}.divide-gray-100>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(243 244 246 / var(--tw-divide-opacity))}.divide-gray-200>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(229 231 235 / var(--tw-divide-opacity))}.divide-gray-300>:not([hidden])~:not([hidden]){--tw-divide-opacity: 1;border-color:rgb(209 213 219 / var(--tw-divide-opacity))}.self-center{align-self:center}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-x-auto{overflow-x:auto}.overflow-y-auto{overflow-y:auto}.truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.overflow-ellipsis{text-overflow:ellipsis}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l-md{border-top-left-radius:.375rem;border-bottom-left-radius:.375rem}.rounded-r-md{border-top-right-radius:.375rem;border-bottom-right-radius:.375rem}.rounded-t-sm{border-top-left-radius:.125rem;border-top-right-radius:.125rem}.\!border-0{border-width:0px!important}.border{border-width:1px}.border-0{border-width:0px}.border-b{border-bottom-width:1px}.border-b-0{border-bottom-width:0px}.border-b-4{border-bottom-width:4px}.border-t{border-top-width:1px}.border-t-0{border-top-width:0px}.border-gray-200{--tw-border-opacity: 1;border-color:rgb(229 231 235 / var(--tw-border-opacity))}.border-gray-300{--tw-border-opacity: 1;border-color:rgb(209 213 219 / var(--tw-border-opacity))}.border-primary-900{--tw-border-opacity: 1;border-color:rgb(6 95 159 / var(--tw-border-opacity))}.border-transparent{border-color:transparent}.bg-amber-500{--tw-bg-opacity: 1;background-color:rgb(245 158 11 / var(--tw-bg-opacity))}.bg-blue-50{--tw-bg-opacity: 1;background-color:rgb(239 246 255 / var(--tw-bg-opacity))}.bg-blue-600{--tw-bg-opacity: 1;background-color:rgb(37 99 235 / var(--tw-bg-opacity))}.bg-emerald-400{--tw-bg-opacity: 1;background-color:rgb(52 211 153 / var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity: 1;background-color:rgb(249 250 251 / var(--tw-bg-opacity))}.bg-green-50{--tw-bg-opacity: 1;background-color:rgb(240 253 244 / var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity: 1;background-color:rgb(34 197 94 / var(--tw-bg-opacity))}.bg-lime-500{--tw-bg-opacity: 1;background-color:rgb(132 204 22 / var(--tw-bg-opacity))}.bg-orange-50{--tw-bg-opacity: 1;background-color:rgb(255 247 237 / var(--tw-bg-opacity))}.bg-orange-500{--tw-bg-opacity: 1;background-color:rgb(249 115 22 / var(--tw-bg-opacity))}.bg-primary-600{--tw-bg-opacity: 1;background-color:rgb(21 164 233 / var(--tw-bg-opacity))}.bg-primary-900{--tw-bg-opacity: 1;background-color:rgb(6 95 159 / var(--tw-bg-opacity))}.bg-purple-50{--tw-bg-opacity: 1;background-color:rgb(250 245 255 / var(--tw-bg-opacity))}.bg-red-50{--tw-bg-opacity: 1;background-color:rgb(254 242 242 / var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity: 1;background-color:rgb(239 68 68 / var(--tw-bg-opacity))}.bg-red-700{--tw-bg-opacity: 1;background-color:rgb(185 28 28 / var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity: 1;background-color:rgb(241 245 249 / var(--tw-bg-opacity))}.bg-teal-400{--tw-bg-opacity: 1;background-color:rgb(45 212 191 / var(--tw-bg-opacity))}.bg-transparent{background-color:transparent}.bg-white{--tw-bg-opacity: 1;background-color:rgb(255 255 255 / var(--tw-bg-opacity))}.bg-yellow-50{--tw-bg-opacity: 1;background-color:rgb(254 252 232 / var(--tw-bg-opacity))}.bg-yellow-500{--tw-bg-opacity: 1;background-color:rgb(234 179 8 / var(--tw-bg-opacity))}.fill-current{fill:currentColor}.\!p-0{padding:0!important}.p-2{padding:.5rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-2\.5{padding-left:.625rem;padding-right:.625rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.py-0{padding-top:0;padding-bottom:0}.py-0\.5{padding-top:.125rem;padding-bottom:.125rem}.py-1{padding-top:.25rem;padding-bottom:.25rem}.py-1\.5{padding-top:.375rem;padding-bottom:.375rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-3\.5{padding-top:.875rem;padding-bottom:.875rem}.pb-4{padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pl-1{padding-left:.25rem}.pl-1\.5{padding-left:.375rem}.pr-1{padding-right:.25rem}.pr-1\.5{padding-right:.375rem}.pr-2{padding-right:.5rem}.pr-6{padding-right:1.5rem}.pt-0{padding-top:0}.pt-1{padding-top:.25rem}.text-left{text-align:left}.text-right{text-align:right}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-text-bottom{vertical-align:text-bottom}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:Lato,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji"}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-4xl{font-size:2.25rem;line-height:2.5rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-light{font-weight:300}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.leading-6{line-height:1.5rem}.text-black{--tw-text-opacity: 1;color:rgb(0 0 0 / var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity: 1;color:rgb(59 130 246 / var(--tw-text-opacity))}.text-blue-600{--tw-text-opacity: 1;color:rgb(37 99 235 / var(--tw-text-opacity))}.text-blue-700{--tw-text-opacity: 1;color:rgb(29 78 216 / var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity: 1;color:rgb(209 213 219 / var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity: 1;color:rgb(107 114 128 / var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity: 1;color:rgb(75 85 99 / var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity: 1;color:rgb(55 65 81 / var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity: 1;color:rgb(17 24 39 / var(--tw-text-opacity))}.text-green-500{--tw-text-opacity: 1;color:rgb(34 197 94 / var(--tw-text-opacity))}.text-green-700{--tw-text-opacity: 1;color:rgb(21 128 61 / var(--tw-text-opacity))}.text-indigo-600{--tw-text-opacity: 1;color:rgb(79 70 229 / var(--tw-text-opacity))}.text-orange-700{--tw-text-opacity: 1;color:rgb(194 65 12 / var(--tw-text-opacity))}.text-primary-900{--tw-text-opacity: 1;color:rgb(6 95 159 / var(--tw-text-opacity))}.text-purple-500{--tw-text-opacity: 1;color:rgb(168 85 247 / var(--tw-text-opacity))}.text-purple-700{--tw-text-opacity: 1;color:rgb(126 34 206 / var(--tw-text-opacity))}.text-red-500{--tw-text-opacity: 1;color:rgb(239 68 68 / var(--tw-text-opacity))}.text-red-700{--tw-text-opacity: 1;color:rgb(185 28 28 / var(--tw-text-opacity))}.text-white{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity))}.text-yellow-500{--tw-text-opacity: 1;color:rgb(234 179 8 / var(--tw-text-opacity))}.text-yellow-700{--tw-text-opacity: 1;color:rgb(161 98 7 / var(--tw-text-opacity))}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.shadow-sm{--tw-shadow: 0 1px 2px 0 rgb(0 0 0 / .05);--tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.ring-1{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-2{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-inset{--tw-ring-inset: inset}.ring-black{--tw-ring-opacity: 1;--tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity))}.ring-blue-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(191 219 254 / var(--tw-ring-opacity))}.ring-blue-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(59 130 246 / var(--tw-ring-opacity))}.ring-blue-600\/20{--tw-ring-color: rgb(37 99 235 / .2)}.ring-blue-700{--tw-ring-opacity: 1;--tw-ring-color: rgb(29 78 216 / var(--tw-ring-opacity))}.ring-gray-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(229 231 235 / var(--tw-ring-opacity))}.ring-gray-300{--tw-ring-opacity: 1;--tw-ring-color: rgb(209 213 219 / var(--tw-ring-opacity))}.ring-gray-600\/20{--tw-ring-color: rgb(75 85 99 / .2)}.ring-green-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(34 197 94 / var(--tw-ring-opacity))}.ring-green-600\/20{--tw-ring-color: rgb(22 163 74 / .2)}.ring-orange-600\/20{--tw-ring-color: rgb(234 88 12 / .2)}.ring-purple-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(168 85 247 / var(--tw-ring-opacity))}.ring-purple-600\/20{--tw-ring-color: rgb(147 51 234 / .2)}.ring-red-200{--tw-ring-opacity: 1;--tw-ring-color: rgb(254 202 202 / var(--tw-ring-opacity))}.ring-red-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(239 68 68 / var(--tw-ring-opacity))}.ring-red-600\/20{--tw-ring-color: rgb(220 38 38 / .2)}.ring-white{--tw-ring-opacity: 1;--tw-ring-color: rgb(255 255 255 / var(--tw-ring-opacity))}.ring-yellow-500{--tw-ring-opacity: 1;--tw-ring-color: rgb(234 179 8 / var(--tw-ring-opacity))}.ring-yellow-600\/20{--tw-ring-color: rgb(202 138 4 / .2)}.ring-opacity-5{--tw-ring-opacity: .05}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.debug{outline:1px dot-dash red;border:1px solid red}.placeholder\:text-gray-400::-moz-placeholder{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.placeholder\:text-gray-400::placeholder{--tw-text-opacity: 1;color:rgb(156 163 175 / var(--tw-text-opacity))}.hover\:cursor-pointer:hover{cursor:pointer}.hover\:border-white:hover{--tw-border-opacity: 1;border-color:rgb(255 255 255 / var(--tw-border-opacity))}.hover\:bg-blue-500:hover{--tw-bg-opacity: 1;background-color:rgb(59 130 246 / var(--tw-bg-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity: 1;background-color:rgb(243 244 246 / var(--tw-bg-opacity))}.hover\:bg-gray-50:hover{--tw-bg-opacity: 1;background-color:rgb(249 250 251 / var(--tw-bg-opacity))}.hover\:bg-slate-50:hover{--tw-bg-opacity: 1;background-color:rgb(248 250 252 / var(--tw-bg-opacity))}.hover\:text-gray-500:hover{--tw-text-opacity: 1;color:rgb(107 114 128 / var(--tw-text-opacity))}.hover\:text-white:hover{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity))}.hover\:text-yellow-500:hover{--tw-text-opacity: 1;color:rgb(234 179 8 / var(--tw-text-opacity))}.focus\:z-10:focus{z-index:10}.focus\:z-20:focus{z-index:20}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:outline-offset-0:focus{outline-offset:0px}.focus\:\!ring-0:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color) !important;--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)!important}.focus\:ring-0:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.focus\:ring-2:focus{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.focus\:ring-inset:focus{--tw-ring-inset: inset}.focus\:ring-indigo-600:focus{--tw-ring-opacity: 1;--tw-ring-color: rgb(79 70 229 / var(--tw-ring-opacity))}.focus\:ring-offset-0:focus{--tw-ring-offset-width: 0px}.focus-visible\:outline:focus-visible{outline-style:solid}.focus-visible\:outline-2:focus-visible{outline-width:2px}.focus-visible\:outline-offset-2:focus-visible{outline-offset:2px}.focus-visible\:outline-blue-500:focus-visible{outline-color:#3b82f6}.focus-visible\:outline-primary-600:focus-visible{outline-color:#15a4e9}@media (min-width: 640px){.sm\:static{position:static}.sm\:inset-auto{inset:auto}.sm\:-mx-6{margin-left:-1.5rem;margin-right:-1.5rem}.sm\:ml-6{margin-left:1.5rem}.sm\:flex{display:flex}.sm\:hidden{display:none}.sm\:flex-1{flex:1 1 0%}.sm\:items-center{align-items:center}.sm\:items-stretch{align-items:stretch}.sm\:justify-start{justify-content:flex-start}.sm\:justify-between{justify-content:space-between}.sm\:space-x-8>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(2rem * var(--tw-space-x-reverse));margin-left:calc(2rem * calc(1 - var(--tw-space-x-reverse)))}.sm\:px-6{padding-left:1.5rem;padding-right:1.5rem}.sm\:pr-0{padding-right:0}.sm\:text-sm{font-size:.875rem;line-height:1.25rem}}@media (min-width: 1024px){.lg\:order-first{order:-9999}.lg\:order-last{order:9999}.lg\:-mx-8{margin-left:-2rem;margin-right:-2rem}.lg\:mt-12{margin-top:3rem}.lg\:block{display:block}.lg\:flex-row{flex-direction:row}.lg\:items-start{align-items:flex-start}.lg\:justify-between{justify-content:space-between}.lg\:px-8{padding-left:2rem;padding-right:2rem}}@media (min-width: 1280px){.xl\:h-40{height:10rem}}@media (min-width: 1536px){.\32xl\:h-48{height:12rem}.\32xl\:min-w-52{min-width:13rem}.\32xl\:max-w-72{max-width:18rem}}
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/index-pKJQAlqa.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/index-CKrV6JKW.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -30,37 +30,37 @@
     b as Tt,
     i as Et,
     A as Qe,
     j as r,
     $ as fe,
     c as Ge,
     G as Ze
-} from "./ui-Bo7CIhws.js";
+} from "./ui-DM1JZie1.js";
 import {
     s as Rt
-} from "./sentry-B_MfAkLS.js";
+} from "./sentry-DxJl7iQ9.js";
 import {
     C as Ot,
-    a as Pt,
-    X as Nt,
+    a as Nt,
+    X as Pt,
     T as Ct,
     L as Mt,
     B as Lt,
     b as _t,
     Y as jt,
     R as Ft
-} from "./recharts-9OgIHZXS.js";
+} from "./recharts-BzBtiWsS.js";
 import {
     f as Bt,
     a as Dt,
     b as zt
 } from "./dateFns-s2EURlY7.js";
 import {
     S as At
-} from "./syntaxHighlighter-D1hpWw2Q.js";
+} from "./syntaxHighlighter-CEoW8GyI.js";
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const i of document.querySelectorAll('link[rel="modulepreload"]')) a(i);
     new MutationObserver(i => {
         for (const o of i)
             if (o.type === "childList")
@@ -259,17 +259,17 @@
                     y = {};
                     for (var T in x) y[T] = x[T];
                     y.theme = v.useContext(xt)
                 }
                 typeof x.className == "string" ? d = kt(p.registered, c, x.className) : x.className != null && (d = x.className + " ");
                 var O = Qt(h.concat(c), p.registered, y);
                 d += p.key + "-" + O.name, l !== void 0 && (d += " " + l);
-                var P = m && u === void 0 ? Be(w) : f,
+                var N = m && u === void 0 ? Be(w) : f,
                     M = {};
-                for (var q in x) m && q === "as" || P(q) && (M[q] = x[q]);
+                for (var q in x) m && q === "as" || N(q) && (M[q] = x[q]);
                 return M.className = d, M.ref = s, v.createElement(v.Fragment, null, v.createElement(Vt, {
                     cache: p,
                     serialized: O,
                     isStringTag: typeof w == "string"
                 }), v.createElement(w, M))
             });
             return S.displayName = o !== void 0 ? o : "Styled(" + (typeof i == "string" ? i : i.displayName || i.name || "Component") + ")", S.defaultProps = t.defaultProps, S.__emotion_real = S, S.__emotion_base = i, S.__emotion_styles = h, S.__emotion_forwardProp = u, Object.defineProperty(S, "toString", {
@@ -598,15 +598,15 @@
         strokeLinejoin: "round",
         d: "M11.48 3.499a.562.562 0 0 1 1.04 0l2.125 5.111a.563.563 0 0 0 .475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 0 0-.182.557l1.285 5.385a.562.562 0 0 1-.84.61l-4.725-2.885a.562.562 0 0 0-.586 0L6.982 20.54a.562.562 0 0 1-.84-.61l1.285-5.386a.562.562 0 0 0-.182-.557l-4.204-3.602a.562.562 0 0 1 .321-.988l5.518-.442a.563.563 0 0 0 .475-.345L11.48 3.5Z"
     }))
 }
 const Rr = v.forwardRef(Er),
     Or = Rr;
 
-function Pr({
+function Nr({
     title: e,
     titleId: t,
     ...n
 }, a) {
     return v.createElement("svg", Object.assign({
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
@@ -621,16 +621,16 @@
         id: t
     }, e) : null, v.createElement("path", {
         strokeLinecap: "round",
         strokeLinejoin: "round",
         d: "M6 18 18 6M6 6l12 12"
     }))
 }
-const Nr = v.forwardRef(Pr),
-    Ne = Nr,
+const Pr = v.forwardRef(Nr),
+    Pe = Pr,
     Cr = "data:image/svg+xml,%3csvg%20xmlns='http://www.w3.org/2000/svg'%20width='195'%20height='249'%3e%3cg%20fill='%23fff'%20fill-rule='nonzero'%3e%3cpath%20d='M181%20179.8c0%2010.2-7.1%2018.6-16.5%2020.9-1.8.3-3.6.3-5.1.5-27%203.3-50.6%2014-71.5%2032.3-3.3%203.1-6.1%206.1-8.9%209.7-.5.8-1.3%201.3-1.5%202-1.8%201.8-4.6%203.1-7.4%203.1-5.9%200-10.4-4.6-10.4-10.4%200-1%20.3-2%20.5-3.1.3-.3.3-.8.5-1%206.4-17%2015.5-31.3%2027.7-42.5%2018.8-16.5%2040.2-27%2064.1-31.3%203.1-.5%206.1-1%209.2-1.3%2010.7.8%2019.3%209.9%2019.3%2021.1M170.1%20108.3c-.3.3-.5.8-.8%201l-.3.3c-5.1%205.1-10.9%208.7-17%2010.4-9.7%202.8-19.1%202.8-28.2.3-1.3-.3-2.3-.8-3.6-1-4.1-2.3-5.6-7.1-3.6-11.2%201.8-3.6%205.6-5.3%209.4-4.6.8.3%201.3.5%202%20.8%2010.2%203.3%2020.6%203.6%2031%20.5%201.8-.5%203.3-1.3%204.8-1.8.3-.3.8-.3%201-.5%201-.3%202-.3%203.1.3%202.2.9%203.2%203.5%202.2%205.5m-11.5-87.5c-10.7-5.9-22.6-10.4-35.9-13.5-13.2-2.8-27.2-4.6-42-4.8-14.5-.3-29-.5-43-.5S11.5%201.2.8%200v33.8c2%2037.1%2013%2065.1%2032.8%2083.7%2020.9%2018.3%2045.3%2028%2073.3%2029h4.6c24.7-.8%2043.5-6.4%2057-17%2017.3-12%2026-28.8%2026-49.9-1.3-27-13.2-46.6-35.9-58.8'/%3e%3c/g%3e%3c/svg%3e";
 
 function ie(...e) {
     return e.filter(Boolean).join(" ")
 }
 const Mr = I(Qe)(() => [{
         "--tw-bg-opacity": "1",
@@ -683,15 +683,15 @@
         className: "absolute inset-y-0 left-0 flex items-center sm:hidden"
     }, r(Qe.Button, {
         className: "relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-primary"
     }, r("span", {
         className: "absolute -inset-0.5"
     }), r("span", {
         className: "sr-only"
-    }, "Open main menu"), l ? r(Ne, {
+    }, "Open main menu"), l ? r(Pe, {
         className: "block h-6 w-6",
         "aria-hidden": "true"
     }) : r(br, {
         className: "block h-6 w-6",
         "aria-hidden": "true"
     }))), r("div", {
         className: "flex flex-1 items-center justify-center sm:items-stretch sm:justify-start"
@@ -1371,22 +1371,22 @@
         }, function(a, i, o) {
             a.exports = o(13)
         }, function(a, i, o) {
             Object.defineProperty(i, "__esModule", {
                 value: !0
             }), i.SparklinesText = i.SparklinesNormalBand = i.SparklinesReferenceLine = i.SparklinesSpots = i.SparklinesBars = i.SparklinesCurve = i.SparklinesLine = i.Sparklines = void 0;
             var l = function() {
-                    function D(N, W) {
+                    function D(P, W) {
                         for (var C = 0; C < W.length; C++) {
                             var Q = W[C];
-                            Q.enumerable = Q.enumerable || !1, Q.configurable = !0, "value" in Q && (Q.writable = !0), Object.defineProperty(N, Q.key, Q)
+                            Q.enumerable = Q.enumerable || !1, Q.configurable = !0, "value" in Q && (Q.writable = !0), Object.defineProperty(P, Q.key, Q)
                         }
                     }
-                    return function(N, W, C) {
-                        return W && D(N.prototype, W), C && D(N, C), N
+                    return function(P, W, C) {
+                        return W && D(P.prototype, W), C && D(P, C), P
                     }
                 }(),
                 u = o(0),
                 f = L(u),
                 m = o(1),
                 g = L(m),
                 h = o(17),
@@ -1398,51 +1398,51 @@
                 s = o(20),
                 w = L(s),
                 d = o(21),
                 c = L(d),
                 y = o(22),
                 T = L(y),
                 O = o(27),
-                P = L(O),
+                N = L(O),
                 M = o(28),
                 q = L(M);
 
             function L(D) {
                 return D && D.__esModule ? D : {
                     default: D
                 }
             }
 
-            function Z(D, N) {
-                if (!(D instanceof N)) throw new TypeError("Cannot call a class as a function")
+            function Z(D, P) {
+                if (!(D instanceof P)) throw new TypeError("Cannot call a class as a function")
             }
 
-            function G(D, N) {
+            function G(D, P) {
                 if (!D) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                return N && (typeof N == "object" || typeof N == "function") ? N : D
+                return P && (typeof P == "object" || typeof P == "function") ? P : D
             }
 
-            function V(D, N) {
-                if (typeof N != "function" && N !== null) throw new TypeError("Super expression must either be null or a function, not " + typeof N);
-                D.prototype = Object.create(N && N.prototype, {
+            function V(D, P) {
+                if (typeof P != "function" && P !== null) throw new TypeError("Super expression must either be null or a function, not " + typeof P);
+                D.prototype = Object.create(P && P.prototype, {
                     constructor: {
                         value: D,
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
-                }), N && (Object.setPrototypeOf ? Object.setPrototypeOf(D, N) : D.__proto__ = N)
+                }), P && (Object.setPrototypeOf ? Object.setPrototypeOf(D, P) : D.__proto__ = P)
             }
             var Y = function(D) {
-                V(N, D);
+                V(P, D);
 
-                function N(W) {
-                    return Z(this, N), G(this, (N.__proto__ || Object.getPrototypeOf(N)).call(this, W))
+                function P(W) {
+                    return Z(this, P), G(this, (P.__proto__ || Object.getPrototypeOf(P)).call(this, W))
                 }
-                return l(N, [{
+                return l(P, [{
                     key: "render",
                     value: function() {
                         var C = this.props,
                             Q = C.data,
                             le = C.limit,
                             b = C.width,
                             E = C.height,
@@ -1474,15 +1474,15 @@
                                 points: H,
                                 width: b,
                                 height: E,
                                 margin: $
                             })
                         }))
                     }
-                }]), N
+                }]), P
             }(m.PureComponent);
             Y.propTypes = {
                 data: f.default.array,
                 limit: f.default.number,
                 width: f.default.number,
                 height: f.default.number,
                 svgWidth: f.default.number,
@@ -1495,15 +1495,15 @@
                 onMouseMove: f.default.func
             }, Y.defaultProps = {
                 data: [],
                 width: 240,
                 height: 60,
                 preserveAspectRatio: "none",
                 margin: 2
-            }, i.Sparklines = Y, i.SparklinesLine = S.default, i.SparklinesCurve = p.default, i.SparklinesBars = w.default, i.SparklinesSpots = c.default, i.SparklinesReferenceLine = T.default, i.SparklinesNormalBand = P.default, i.SparklinesText = k.default
+            }, i.Sparklines = Y, i.SparklinesLine = S.default, i.SparklinesCurve = p.default, i.SparklinesBars = w.default, i.SparklinesSpots = c.default, i.SparklinesReferenceLine = T.default, i.SparklinesNormalBand = N.default, i.SparklinesText = k.default
         }, function(a, i, o) {
             (function(l) {
                 var u = o(4),
                     f = o(5),
                     m = o(8),
                     g = o(6),
                     h = o(15);
@@ -1521,15 +1521,15 @@
                             bool: T("boolean"),
                             func: T("function"),
                             number: T("number"),
                             object: T("object"),
                             string: T("string"),
                             symbol: T("symbol"),
                             any: O(),
-                            arrayOf: P,
+                            arrayOf: N,
                             element: M(),
                             instanceOf: q,
                             node: V(),
                             objectOf: Z,
                             oneOf: L,
                             oneOfType: G,
                             shape: Y
@@ -1575,15 +1575,15 @@
                         return y(E)
                     }
 
                     function O() {
                         return y(u.thatReturnsNull)
                     }
 
-                    function P(b) {
+                    function N(b) {
                         function E(z, F, j, $, A) {
                             if (typeof b != "function") return new c("Property `" + A + "` of component `" + j + "` has invalid PropType notation inside arrayOf.");
                             var _ = z[F];
                             if (!Array.isArray(_)) {
                                 var B = W(_);
                                 return new c("Invalid " + $ + " `" + A + "` of type " + ("`" + B + "` supplied to `" + j + "`, expected an array."))
                             }
@@ -1714,21 +1714,21 @@
                                 } else return !1;
                                 return !0;
                             default:
                                 return !1
                         }
                     }
 
-                    function N(b, E) {
+                    function P(b, E) {
                         return b === "symbol" || E["@@toStringTag"] === "Symbol" || typeof Symbol == "function" && E instanceof Symbol
                     }
 
                     function W(b) {
                         var E = typeof b;
-                        return Array.isArray(b) ? "array" : b instanceof RegExp ? "object" : N(E, b) ? "symbol" : E
+                        return Array.isArray(b) ? "array" : b instanceof RegExp ? "object" : P(E, b) ? "symbol" : E
                     }
 
                     function C(b) {
                         if (typeof b > "u" || b === null) return "" + b;
                         var E = W(b);
                         if (E === "object") {
                             if (b instanceof Date) return "date";
@@ -1874,18 +1874,18 @@
                     key: "render",
                     value: function() {
                         var d = this.props,
                             c = d.point,
                             y = d.text,
                             T = d.fontSize,
                             O = d.fontFamily,
-                            P = c.x,
+                            N = c.x,
                             M = c.y;
                         return g.default.createElement("g", null, g.default.createElement("text", {
-                            x: P,
+                            x: N,
                             y: M,
                             fontFamily: O || "Verdana",
                             fontSize: T || 10
                         }, y))
                     }
                 }]), s
             }(g.default.Component);
@@ -1958,50 +1958,50 @@
                     value: function() {
                         var d = this.props,
                             c = d.data,
                             y = d.points;
                         d.width;
                         var T = d.height,
                             O = d.margin,
-                            P = d.color,
+                            N = d.color,
                             M = d.style,
                             q = d.onMouseMove,
-                            L = y.map(function(N) {
-                                return [N.x, N.y]
-                            }).reduce(function(N, W) {
-                                return N.concat(W)
+                            L = y.map(function(P) {
+                                return [P.x, P.y]
+                            }).reduce(function(P, W) {
+                                return P.concat(W)
                             }),
                             Z = [y[y.length - 1].x, T - O, O, T - O, O, y[0].y],
                             G = L.concat(Z),
                             V = {
-                                stroke: P || M.stroke || "slategray",
+                                stroke: N || M.stroke || "slategray",
                                 strokeWidth: M.strokeWidth || "1",
                                 strokeLinejoin: M.strokeLinejoin || "round",
                                 strokeLinecap: M.strokeLinecap || "round",
                                 fill: "none"
                             },
                             Y = {
                                 stroke: M.stroke || "none",
                                 strokeWidth: "0",
                                 fillOpacity: M.fillOpacity || ".1",
-                                fill: M.fill || P || "slategray",
+                                fill: M.fill || N || "slategray",
                                 pointerEvents: "auto"
                             },
-                            D = y.map(function(N, W) {
+                            D = y.map(function(P, W) {
                                 return g.default.createElement("circle", {
                                     key: W,
-                                    cx: N.x,
-                                    cy: N.y,
+                                    cx: P.x,
+                                    cy: P.y,
                                     r: 2,
                                     style: Y,
                                     onMouseEnter: function(Q) {
-                                        return q("enter", c[W], N)
+                                        return q("enter", c[W], P)
                                     },
                                     onClick: function(Q) {
-                                        return q("click", c[W], N)
+                                        return q("click", c[W], P)
                                     }
                                 })
                             });
                         return g.default.createElement("g", null, D, g.default.createElement("polyline", {
                             points: G.join(" "),
                             style: Y
                         }), g.default.createElement("polyline", {
@@ -2075,15 +2075,15 @@
                     value: function() {
                         var d = this.props,
                             c = d.points;
                         d.width;
                         var y = d.height,
                             T = d.margin,
                             O = d.color,
-                            P = d.style,
+                            N = d.style,
                             M = d.divisor,
                             q = M === void 0 ? .25 : M,
                             L = void 0,
                             Z = function(C) {
                                 var Q = void 0;
                                 if (!L) Q = [C.x, C.y];
                                 else {
@@ -2096,29 +2096,29 @@
                                 return Z(W)
                             }).reduce(function(W, C) {
                                 return W.concat(C)
                             }),
                             V = ["L" + c[c.length - 1].x, y - T, T, y - T, T, c[0].y],
                             Y = G.concat(V),
                             D = {
-                                stroke: O || P.stroke || "slategray",
-                                strokeWidth: P.strokeWidth || "1",
-                                strokeLinejoin: P.strokeLinejoin || "round",
-                                strokeLinecap: P.strokeLinecap || "round",
+                                stroke: O || N.stroke || "slategray",
+                                strokeWidth: N.strokeWidth || "1",
+                                strokeLinejoin: N.strokeLinejoin || "round",
+                                strokeLinecap: N.strokeLinecap || "round",
                                 fill: "none"
                             },
-                            N = {
-                                stroke: P.stroke || "none",
+                            P = {
+                                stroke: N.stroke || "none",
                                 strokeWidth: "0",
-                                fillOpacity: P.fillOpacity || ".1",
-                                fill: P.fill || O || "slategray"
+                                fillOpacity: N.fillOpacity || ".1",
+                                fill: N.fill || O || "slategray"
                             };
                         return g.default.createElement("g", null, g.default.createElement("path", {
                             d: "M" + Y.join(" "),
-                            style: N
+                            style: P
                         }), g.default.createElement("path", {
                             d: "M" + G.join(" "),
                             style: D
                         }))
                     }
                 }]), s
             }(g.default.Component);
@@ -2184,20 +2184,20 @@
                     key: "render",
                     value: function() {
                         var d = this,
                             c = this.props,
                             y = c.points,
                             T = c.height,
                             O = c.style,
-                            P = c.barWidth,
+                            N = c.barWidth,
                             M = c.margin,
                             q = c.onMouseMove,
                             L = 1 * (O && O.strokeWidth || 0),
                             Z = M ? 2 * M : 0,
-                            G = P || (y && y.length >= 2 ? Math.max(0, y[1].x - y[0].x - L - Z) : 0);
+                            G = N || (y && y.length >= 2 ? Math.max(0, y[1].x - y[0].x - L - Z) : 0);
                         return g.default.createElement("g", {
                             transform: "scale(1,-1)"
                         }, y.map(function(V, Y) {
                             return g.default.createElement("rect", {
                                 key: Y,
                                 x: V.x - (G + L) / 2,
                                 y: -T,
@@ -2286,29 +2286,29 @@
                     value: function() {
                         var d = this.props,
                             c = d.points;
                         d.width, d.height;
                         var y = d.size,
                             T = d.style,
                             O = d.spotColors,
-                            P = g.default.createElement("circle", {
+                            N = g.default.createElement("circle", {
                                 cx: c[0].x,
                                 cy: c[0].y,
                                 r: y,
                                 style: T
                             }),
                             M = g.default.createElement("circle", {
                                 cx: c[c.length - 1].x,
                                 cy: c[c.length - 1].y,
                                 r: y,
                                 style: T || {
                                     fill: O[this.lastDirection(c)]
                                 }
                             });
-                        return g.default.createElement("g", null, T && P, M)
+                        return g.default.createElement("g", null, T && N, M)
                     }
                 }]), s
             }(g.default.Component);
             x.propTypes = {
                 size: f.default.number,
                 style: f.default.object,
                 spotColors: f.default.object
@@ -2383,27 +2383,27 @@
                     return x(this, c), p(this, (c.__proto__ || Object.getPrototypeOf(c)).apply(this, arguments))
                 }
                 return l(c, [{
                     key: "render",
                     value: function() {
                         var T = this.props,
                             O = T.points,
-                            P = T.margin,
+                            N = T.margin,
                             M = T.type,
                             q = T.style,
                             L = T.value,
                             Z = O.map(function(V) {
                                 return V.y
                             }),
                             G = M == "custom" ? L : k[M](Z);
                         return g.default.createElement("line", {
                             x1: O[0].x,
-                            y1: G + P,
+                            y1: G + N,
                             x2: O[O.length - 1].x,
-                            y2: G + P,
+                            y2: G + N,
                             style: q
                         })
                     }
                 }]), c
             }(g.default.Component);
             w.propTypes = {
                 type: f.default.oneOf(["max", "min", "mean", "avg", "median", "custom"]),
@@ -2487,16 +2487,16 @@
         }, function(a, i, o) {
             Object.defineProperty(i, "__esModule", {
                 value: !0
             });
             var l = function() {
                     function c(y, T) {
                         for (var O = 0; O < T.length; O++) {
-                            var P = T[O];
-                            P.enumerable = P.enumerable || !1, P.configurable = !0, "value" in P && (P.writable = !0), Object.defineProperty(y, P.key, P)
+                            var N = T[O];
+                            N.enumerable = N.enumerable || !1, N.configurable = !0, "value" in N && (N.writable = !0), Object.defineProperty(y, N.key, N)
                         }
                     }
                     return function(y, T, O) {
                         return T && c(y.prototype, T), O && c(y, O), y
                     }
                 }(),
                 u = o(0),
@@ -2540,26 +2540,26 @@
                 function y() {
                     return p(this, y), s(this, (y.__proto__ || Object.getPrototypeOf(y)).apply(this, arguments))
                 }
                 return l(y, [{
                     key: "render",
                     value: function() {
                         var O = this.props,
-                            P = O.points,
+                            N = O.points,
                             M = O.margin,
                             q = O.style,
-                            L = P.map(function(V) {
+                            L = N.map(function(V) {
                                 return V.y
                             }),
                             Z = (0, k.default)(L),
                             G = (0, S.default)(L);
                         return g.default.createElement("rect", {
-                            x: P[0].x,
+                            x: N[0].x,
                             y: Z - G + M,
-                            width: P[P.length - 1].x - P[0].x,
+                            width: N[N.length - 1].x - N[0].x,
                             height: S.default * 2,
                             style: q
                         })
                     }
                 }]), y
             }(g.default.Component);
             d.propTypes = {
@@ -2593,18 +2593,18 @@
                     s = p === void 0 ? 1 : p,
                     w = h.margin,
                     d = w === void 0 ? 0 : w,
                     c = h.max,
                     y = c === void 0 ? (0, m.default)(k) : c,
                     T = h.min,
                     O = T === void 0 ? (0, u.default)(k) : T,
-                    P = k.length;
-                R && R < P && (k = k.slice(P - R));
+                    N = k.length;
+                R && R < N && (k = k.slice(N - R));
                 var M = (s - d * 2) / (y - O || 2),
-                    q = (x - d * 2) / ((R || P) - (P > 1 ? 1 : 0));
+                    q = (x - d * 2) / ((R || N) - (N > 1 ? 1 : 0));
                 return k.map(function(L, Z) {
                     return {
                         x: Z * q + d,
                         y: (y === O ? 1 : y - L) * M + d
                     }
                 })
             }
@@ -2844,18 +2844,18 @@
             data: e,
             margin: {
                 top: 0,
                 right: 30,
                 left: 0,
                 bottom: 0
             }
-        }, r(Pt, {
+        }, r(Nt, {
             stroke: "#f5f5f5",
             vertical: !1
-        }), r(Nt, {
+        }), r(Pt, {
             dataKey: "datetime",
             tickLine: !1,
             axisLine: {
                 stroke: "#f5f5f5"
             },
             interval: "equidistantPreserveStart",
             fontSize: 12,
@@ -3110,27 +3110,27 @@
     Group: fe.Group,
     List: ye.List,
     Panels: ye.Panels,
     Panel: ye.Panel
 });
 
 function on() {
-    return r(X.Fragment, null, r(Ne, {
+    return r(X.Fragment, null, r(Pe, {
         className: "w-3 inline mr-1"
     }), "null")
 }
 
 function ln() {
     return r(X.Fragment, null, r(er, {
         className: "w-3 inline mr-1"
     }), "true")
 }
 
 function sn() {
-    return r(X.Fragment, null, r(Ne, {
+    return r(X.Fragment, null, r(Pe, {
         className: "w-3 inline mr-1"
     }), "false")
 }
 
 function cn({
     value: e
 }) {
@@ -3849,15 +3849,15 @@
         d: "M3.22 7.595a.75.75 0 0 0 0 1.06l3.25 3.25a.75.75 0 0 0 1.06-1.06l-2.72-2.72 2.72-2.72a.75.75 0 0 0-1.06-1.06l-3.25 3.25Zm8.25-3.25-3.25 3.25a.75.75 0 0 0 0 1.06l3.25 3.25a.75.75 0 1 0 1.06-1.06l-2.72-2.72 2.72-2.72a.75.75 0 0 0-1.06-1.06Z",
         clipRule: "evenodd"
     }))
 }
 const Rn = v.forwardRef(En),
     On = Rn;
 
-function Pn({
+function Nn({
     title: e,
     titleId: t,
     ...n
 }, a) {
     return v.createElement("svg", Object.assign({
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 16 16",
@@ -3870,16 +3870,16 @@
         id: t
     }, e) : null, v.createElement("path", {
         fillRule: "evenodd",
         d: "M12.78 7.595a.75.75 0 0 1 0 1.06l-3.25 3.25a.75.75 0 0 1-1.06-1.06l2.72-2.72-2.72-2.72a.75.75 0 0 1 1.06-1.06l3.25 3.25Zm-8.25-3.25 3.25 3.25a.75.75 0 0 1 0 1.06l-3.25 3.25a.75.75 0 0 1-1.06-1.06l2.72-2.72-2.72-2.72a.75.75 0 0 1 1.06-1.06Z",
         clipRule: "evenodd"
     }))
 }
-const Nn = v.forwardRef(Pn),
-    Cn = Nn;
+const Pn = v.forwardRef(Nn),
+    Cn = Pn;
 
 function Mn({
     title: e,
     titleId: t,
     ...n
 }, a) {
     return v.createElement("svg", Object.assign({
@@ -3987,22 +3987,22 @@
         return {
             response: ((t = e.messages) == null ? void 0 : t.find(a => a.kind === "response")) ?? void 0,
             error: ((n = e.messages) == null ? void 0 : n.find(a => a.kind === "error")) ?? void 0,
             endpoint: e.endpoint ?? void 0
         }
     };
 
-function Pe() {
-    return Pe = Object.assign ? Object.assign.bind() : function(e) {
+function Ne() {
+    return Ne = Object.assign ? Object.assign.bind() : function(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = arguments[t];
             for (var a in n) Object.prototype.hasOwnProperty.call(n, a) && (e[a] = n[a])
         }
         return e
-    }, Pe.apply(this, arguments)
+    }, Ne.apply(this, arguments)
 }
 const $n = I.table(() => [{
         minWidth: "100%",
         "> :not([hidden]) ~ :not([hidden])": {
             "--tw-divide-y-reverse": "0",
             borderTopWidth: "calc(1px * calc(1 - var(--tw-divide-y-reverse)))",
             borderBottomWidth: "calc(1px * var(--tw-divide-y-reverse))",
@@ -4077,15 +4077,15 @@
         const g = f,
             h = a[g],
             k = {};
         if (h.onClick !== void 0) {
             const R = h.onClick;
             k.onClick = () => R(l)
         }
-        return r(qn, Pe({
+        return r(qn, Ne({
             key: m,
             className: h.className ?? ""
         }, k), Qn(h, l, g))
     })))))
 }
 const re = I.span(({
         color: e = "default"
@@ -4273,15 +4273,16 @@
         return r("span", {
             className: "font-normal"
         }, r(Zn, {
             method: a
         }), n ? r("span", {
             className: "inline-flex items-center bg-gray-50 px-1 ml-2 py-0.5 text-xs font-medium text-gray-700 ring-1 ring-inset ring-gray-600/20"
         }, n) : null, r("span", {
-            className: "text-gray-500 font-mono text-xs"
+            className: "text-gray-500 font-mono text-xs",
+            title: i
         }, i))
     }
     if (e == "response") {
         const a = t.split(" ");
         return r("span", {
             className: "font-normal"
         }, r(Kn, {
@@ -4331,15 +4332,16 @@
             format: ({
                 request: e,
                 endpoint: t
             }) => e ? r(de, {
                 kind: e.kind,
                 summary: e.summary,
                 endpoint: t
-            }) : null
+            }) : null,
+            className: "truncate max-w-0 w-full"
         },
         response: {
             label: "Response",
             get: e => Hn(e) ?? null,
             format: ({
                 response: e,
                 error: t,
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/react-vbD531y6.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/react-vbD531y6.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/reactQuery-BTfpiMem.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/reactQuery-BTfpiMem.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/reactRouter-iI7EIT1e.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/reactRouter-iI7EIT1e.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/recharts-9OgIHZXS.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/recharts-BzBtiWsS.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     c as Si,
     g as se,
-    r as B,
+    r as R,
     a as S
 } from "./react-vbD531y6.js";
 var Ep = {
         exports: {}
     },
     ae = {};
 /** @license React v16.13.1
@@ -32,15 +32,15 @@
     Ua = Se ? Symbol.for("react.memo") : 60115,
     Ka = Se ? Symbol.for("react.lazy") : 60116,
     Vy = Se ? Symbol.for("react.block") : 60121,
     Yy = Se ? Symbol.for("react.fundamental") : 60117,
     Zy = Se ? Symbol.for("react.responder") : 60118,
     Jy = Se ? Symbol.for("react.scope") : 60119;
 
-function Ue(e) {
+function Ke(e) {
     if (typeof e == "object" && e !== null) {
         var t = e.$$typeof;
         switch (t) {
             case bc:
                 switch (e = e.type, e) {
                     case wc:
                     case Fa:
@@ -64,15 +64,15 @@
             case xc:
                 return t
         }
     }
 }
 
 function jp(e) {
-    return Ue(e) === Fa
+    return Ke(e) === Fa
 }
 ae.AsyncMode = wc;
 ae.ConcurrentMode = Fa;
 ae.ContextConsumer = Ra;
 ae.ContextProvider = Ba;
 ae.Element = bc;
 ae.ForwardRef = za;
@@ -80,54 +80,54 @@
 ae.Lazy = Ka;
 ae.Memo = Ua;
 ae.Portal = xc;
 ae.Profiler = La;
 ae.StrictMode = Na;
 ae.Suspense = Wa;
 ae.isAsyncMode = function(e) {
-    return jp(e) || Ue(e) === wc
+    return jp(e) || Ke(e) === wc
 };
 ae.isConcurrentMode = jp;
 ae.isContextConsumer = function(e) {
-    return Ue(e) === Ra
+    return Ke(e) === Ra
 };
 ae.isContextProvider = function(e) {
-    return Ue(e) === Ba
+    return Ke(e) === Ba
 };
 ae.isElement = function(e) {
     return typeof e == "object" && e !== null && e.$$typeof === bc
 };
 ae.isForwardRef = function(e) {
-    return Ue(e) === za
+    return Ke(e) === za
 };
 ae.isFragment = function(e) {
-    return Ue(e) === Da
+    return Ke(e) === Da
 };
 ae.isLazy = function(e) {
-    return Ue(e) === Ka
+    return Ke(e) === Ka
 };
 ae.isMemo = function(e) {
-    return Ue(e) === Ua
+    return Ke(e) === Ua
 };
 ae.isPortal = function(e) {
-    return Ue(e) === xc
+    return Ke(e) === xc
 };
 ae.isProfiler = function(e) {
-    return Ue(e) === La
+    return Ke(e) === La
 };
 ae.isStrictMode = function(e) {
-    return Ue(e) === Na
+    return Ke(e) === Na
 };
 ae.isSuspense = function(e) {
-    return Ue(e) === Wa
+    return Ke(e) === Wa
 };
 ae.isValidElementType = function(e) {
     return typeof e == "string" || typeof e == "function" || e === Da || e === Fa || e === La || e === Na || e === Wa || e === Xy || typeof e == "object" && e !== null && (e.$$typeof === Ka || e.$$typeof === Ua || e.$$typeof === Ba || e.$$typeof === Ra || e.$$typeof === za || e.$$typeof === Yy || e.$$typeof === Zy || e.$$typeof === Jy || e.$$typeof === Vy)
 };
-ae.typeOf = Ue;
+ae.typeOf = Ke;
 Ep.exports = ae;
 var Jo = Ep.exports;
 
 function Mp(e) {
     var t, r, n = "";
     if (typeof e == "string" || typeof e == "number") n += e;
     else if (typeof e == "object")
@@ -135,20 +135,20 @@
             var i = e.length;
             for (t = 0; t < i; t++) e[t] && (r = Mp(e[t])) && (n && (n += " "), n += r)
         } else
             for (r in e) e[r] && (n && (n += " "), n += r);
     return n
 }
 
-function re() {
+function ee() {
     for (var e, t, r = 0, n = "", i = arguments.length; r < i; r++)(e = arguments[r]) && (t = Mp(e)) && (n && (n += " "), n += t);
     return n
 }
 var Qy = Array.isArray,
-    Le = Qy,
+    Be = Qy,
     em = typeof Si == "object" && Si && Si.Object === Object && Si,
     Cp = em,
     tm = Cp,
     rm = typeof self == "object" && self && self.Object === Object && self,
     nm = tm || rm || Function("return this")(),
     vt = nm,
     im = vt,
@@ -198,15 +198,15 @@
     wm = Et,
     Om = "[object Symbol]";
 
 function Am(e) {
     return typeof e == "symbol" || wm(e) && xm(e) == Om
 }
 var Ur = Am,
-    Sm = Le,
+    Sm = Be,
     Pm = Ur,
     _m = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
     $m = /^\w*$/;
 
 function Tm(e, t) {
     if (Sm(e)) return !1;
     var r = typeof e;
@@ -288,16 +288,16 @@
     og = ng,
     ug = ag;
 
 function cg(e, t) {
     var r = ug(e, t);
     return og(r) ? r : void 0
 }
-var sr = cg,
-    sg = sr,
+var lr = cg,
+    sg = lr,
     lg = sg(Object, "create"),
     qa = lg,
     Is = qa;
 
 function fg() {
     this.__data__ = Is ? Is(null) : {}, this.size = 0
 }
@@ -427,15 +427,15 @@
 }
 Hr.prototype.clear = tb;
 Hr.prototype.delete = rb;
 Hr.prototype.get = nb;
 Hr.prototype.has = ib;
 Hr.prototype.set = ab;
 var Ga = Hr,
-    ob = sr,
+    ob = lr,
     ub = vt,
     cb = ob(ub, "Map"),
     Pc = cb,
     ks = Dg,
     sb = Ga,
     lb = Pc;
 
@@ -550,15 +550,15 @@
 function qb(e, t) {
     for (var r = -1, n = e == null ? 0 : e.length, i = Array(n); ++r < n;) i[r] = t(e[r], r, e);
     return i
 }
 var Tc = qb,
     Ds = di,
     Hb = Tc,
-    Gb = Le,
+    Gb = Be,
     Xb = Ur,
     Vb = 1 / 0,
     Ns = Ds ? Ds.prototype : void 0,
     Ls = Ns ? Ns.toString : void 0;
 
 function Lp(e) {
     if (typeof e == "string") return e;
@@ -570,15 +570,15 @@
 var Yb = Lp,
     Zb = Yb;
 
 function Jb(e) {
     return e == null ? "" : Zb(e)
 }
 var Bp = Jb,
-    Qb = Le,
+    Qb = Be,
     e0 = Oc,
     t0 = Kb,
     r0 = Bp;
 
 function n0(e, t) {
     return Qb(e) ? e : e0(e, t) ? [e] : t0(r0(e))
 }
@@ -610,17 +610,17 @@
 var Fp = f0;
 const Ze = se(Fp);
 
 function h0(e) {
     return e == null
 }
 var p0 = h0;
-const X = se(p0);
+const G = se(p0);
 var d0 = Tt,
-    v0 = Le,
+    v0 = Be,
     y0 = Et,
     m0 = "[object String]";
 
 function g0(e) {
     return typeof e == "string" || !v0(e) && y0(e) && d0(e) == m0
 }
 var b0 = g0;
@@ -650,19 +650,19 @@
     N = function(t) {
         return S0(t) && !Xr(t)
     },
     be = function(t) {
         return N(t) || vi(t)
     },
     T0 = 0,
-    lr = function(t) {
+    fr = function(t) {
         var r = ++T0;
         return "".concat(t || "").concat(r)
     },
-    Ar = function(t, r) {
+    ar = function(t, r) {
         var n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 0,
             i = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : !1;
         if (!N(t) && !vi(t)) return n;
         var a;
         if (Zt(t)) {
             var o = t.indexOf("%");
             a = r * parseFloat(t.slice(0, o)) / 100
@@ -702,15 +702,15 @@
         xmin: u,
         xmax: c,
         a: h,
         b: (i - h * n) / r
     }
 };
 
-function xr(e, t) {
+function wr(e, t) {
     for (var r in e)
         if ({}.hasOwnProperty.call(e, r) && (!{}.hasOwnProperty.call(t, r) || e[r] !== t[r])) return !1;
     for (var n in t)
         if ({}.hasOwnProperty.call(t, n) && !{}.hasOwnProperty.call(e, n)) return !1;
     return !0
 }
 
@@ -730,15 +730,15 @@
         polygon: Bs,
         polyline: Bs
     },
     jc = ["dangerouslySetInnerHTML", "onCopy", "onCopyCapture", "onCut", "onCutCapture", "onPaste", "onPasteCapture", "onCompositionEnd", "onCompositionEndCapture", "onCompositionStart", "onCompositionStartCapture", "onCompositionUpdate", "onCompositionUpdateCapture", "onFocus", "onFocusCapture", "onBlur", "onBlurCapture", "onChange", "onChangeCapture", "onBeforeInput", "onBeforeInputCapture", "onInput", "onInputCapture", "onReset", "onResetCapture", "onSubmit", "onSubmitCapture", "onInvalid", "onInvalidCapture", "onLoad", "onLoadCapture", "onError", "onErrorCapture", "onKeyDown", "onKeyDownCapture", "onKeyPress", "onKeyPressCapture", "onKeyUp", "onKeyUpCapture", "onAbort", "onAbortCapture", "onCanPlay", "onCanPlayCapture", "onCanPlayThrough", "onCanPlayThroughCapture", "onDurationChange", "onDurationChangeCapture", "onEmptied", "onEmptiedCapture", "onEncrypted", "onEncryptedCapture", "onEnded", "onEndedCapture", "onLoadedData", "onLoadedDataCapture", "onLoadedMetadata", "onLoadedMetadataCapture", "onLoadStart", "onLoadStartCapture", "onPause", "onPauseCapture", "onPlay", "onPlayCapture", "onPlaying", "onPlayingCapture", "onProgress", "onProgressCapture", "onRateChange", "onRateChangeCapture", "onSeeked", "onSeekedCapture", "onSeeking", "onSeekingCapture", "onStalled", "onStalledCapture", "onSuspend", "onSuspendCapture", "onTimeUpdate", "onTimeUpdateCapture", "onVolumeChange", "onVolumeChangeCapture", "onWaiting", "onWaitingCapture", "onAuxClick", "onAuxClickCapture", "onClick", "onClickCapture", "onContextMenu", "onContextMenuCapture", "onDoubleClick", "onDoubleClickCapture", "onDrag", "onDragCapture", "onDragEnd", "onDragEndCapture", "onDragEnter", "onDragEnterCapture", "onDragExit", "onDragExitCapture", "onDragLeave", "onDragLeaveCapture", "onDragOver", "onDragOverCapture", "onDragStart", "onDragStartCapture", "onDrop", "onDropCapture", "onMouseDown", "onMouseDownCapture", "onMouseEnter", "onMouseLeave", "onMouseMove", "onMouseMoveCapture", "onMouseOut", "onMouseOutCapture", "onMouseOver", "onMouseOverCapture", "onMouseUp", "onMouseUpCapture", "onSelect", "onSelectCapture", "onTouchCancel", "onTouchCancelCapture", "onTouchEnd", "onTouchEndCapture", "onTouchMove", "onTouchMoveCapture", "onTouchStart", "onTouchStartCapture", "onPointerDown", "onPointerDownCapture", "onPointerMove", "onPointerMoveCapture", "onPointerUp", "onPointerUpCapture", "onPointerCancel", "onPointerCancelCapture", "onPointerEnter", "onPointerEnterCapture", "onPointerLeave", "onPointerLeaveCapture", "onPointerOver", "onPointerOverCapture", "onPointerOut", "onPointerOutCapture", "onGotPointerCapture", "onGotPointerCaptureCapture", "onLostPointerCapture", "onLostPointerCaptureCapture", "onScroll", "onScrollCapture", "onWheel", "onWheelCapture", "onAnimationStart", "onAnimationStartCapture", "onAnimationEnd", "onAnimationEndCapture", "onAnimationIteration", "onAnimationIterationCapture", "onTransitionEnd", "onTransitionEndCapture"],
     Wi = function(t, r) {
         if (!t || typeof t == "function" || typeof t == "boolean") return null;
         var n = t;
-        if (B.isValidElement(t) && (n = t.props), !Kr(n)) return null;
+        if (R.isValidElement(t) && (n = t.props), !Kr(n)) return null;
         var i = {};
         return Object.keys(n).forEach(function(a) {
             jc.includes(a) && (i[a] = r || function(o) {
                 return n[a](n, o)
             })
         }), i
     },
@@ -804,32 +804,32 @@
         return typeof t == "string" ? t : t ? t.displayName || t.name || "Component" : ""
     },
     zs = null,
     Po = null,
     Mc = function e(t) {
         if (t === zs && Array.isArray(Po)) return Po;
         var r = [];
-        return B.Children.forEach(t, function(n) {
-            X(n) || (Jo.isFragment(n) ? r = r.concat(e(n.props.children)) : r.push(n))
+        return R.Children.forEach(t, function(n) {
+            G(n) || (Jo.isFragment(n) ? r = r.concat(e(n.props.children)) : r.push(n))
         }), Po = r, zs = t, r
     };
 
-function Ne(e, t) {
+function Le(e, t) {
     var r = [],
         n = [];
     return Array.isArray(t) ? n = t.map(function(i) {
         return Ot(i)
     }) : n = [Ot(t)], Mc(e).forEach(function(i) {
         var a = Ze(i, "type.displayName") || Ze(i, "type.name");
         n.indexOf(a) !== -1 && r.push(i)
     }), r
 }
 
-function ze(e, t) {
-    var r = Ne(e, t);
+function We(e, t) {
+    var r = Le(e, t);
     return r && r[0]
 }
 var Ws = function(t) {
         if (!t || !t.props) return !1;
         var r = t.props,
             n = r.width,
             i = r.height;
@@ -842,49 +842,49 @@
     Wp = function(t) {
         return t && eu(t) === "object" && "cx" in t && "cy" in t && "r" in t
     },
     R0 = function(t, r, n, i) {
         var a, o = (a = So == null ? void 0 : So[i]) !== null && a !== void 0 ? a : [];
         return !Y(t) && (i && o.includes(r) || C0.includes(r)) || n && jc.includes(r)
     },
-    G = function(t, r, n) {
+    H = function(t, r, n) {
         if (!t || typeof t == "function" || typeof t == "boolean") return null;
         var i = t;
-        if (B.isValidElement(t) && (i = t.props), !Kr(i)) return null;
+        if (R.isValidElement(t) && (i = t.props), !Kr(i)) return null;
         var a = {};
         return Object.keys(i).forEach(function(o) {
             var u;
             R0((u = i) === null || u === void 0 ? void 0 : u[o], o, r, n) && (a[o] = i[o])
         }), a
     },
     tu = function e(t, r) {
         if (t === r) return !0;
-        var n = B.Children.count(t);
-        if (n !== B.Children.count(r)) return !1;
+        var n = R.Children.count(t);
+        if (n !== R.Children.count(r)) return !1;
         if (n === 0) return !0;
         if (n === 1) return Us(Array.isArray(t) ? t[0] : t, Array.isArray(r) ? r[0] : r);
         for (var i = 0; i < n; i++) {
             var a = t[i],
                 o = r[i];
             if (Array.isArray(a) || Array.isArray(o)) {
                 if (!e(a, o)) return !1
             } else if (!Us(a, o)) return !1
         }
         return !0
     },
     Us = function(t, r) {
-        if (X(t) && X(r)) return !0;
-        if (!X(t) && !X(r)) {
+        if (G(t) && G(r)) return !0;
+        if (!G(t) && !G(r)) {
             var n = t.props || {},
                 i = n.children,
                 a = Rs(n, k0),
                 o = r.props || {},
                 u = o.children,
                 c = Rs(o, D0);
-            return i && u ? xr(a, c) && tu(i, u) : !i && !u ? xr(a, c) : !1
+            return i && u ? wr(a, c) && tu(i, u) : !i && !u ? wr(a, c) : !1
         }
         return !1
     },
     Ks = function(t, r) {
         var n = [],
             i = {};
         return Mc(t).forEach(function(a, o) {
@@ -952,16 +952,16 @@
         s = U0(e, W0),
         f = i || {
             width: r,
             height: n,
             x: 0,
             y: 0
         },
-        l = re("recharts-surface", a);
-    return S.createElement("svg", ru({}, G(s, !0, "svg"), {
+        l = ee("recharts-surface", a);
+    return S.createElement("svg", ru({}, H(s, !0, "svg"), {
         className: l,
         width: r,
         height: n,
         style: o,
         viewBox: "".concat(f.x, " ").concat(f.y, " ").concat(f.width, " ").concat(f.height)
     }), S.createElement("title", null, u), S.createElement("desc", null, c), t)
 }
@@ -996,18 +996,18 @@
     for (a = 0; a < n.length; a++) i = n[a], !(t.indexOf(i) >= 0) && (r[i] = e[i]);
     return r
 }
 var ie = S.forwardRef(function(e, t) {
         var r = e.children,
             n = e.className,
             i = H0(e, q0),
-            a = re("recharts-layer", n);
+            a = ee("recharts-layer", n);
         return S.createElement("g", iu({
             className: a
-        }, G(i, !0), {
+        }, H(i, !0), {
             ref: t
         }), r)
     }),
     At = function(t, r) {
         for (var n = arguments.length, i = new Array(n > 2 ? n - 2 : 0), a = 2; a < n; a++) i[a - 2] = arguments[a]
     };
 
@@ -2047,17 +2047,17 @@
                 var d = Sw(n),
                     w = ew().type(d).size(Pw(a, u, n));
                 return w()
             },
             l = s.className,
             h = s.cx,
             p = s.cy,
-            y = G(s, !0);
+            y = H(s, !0);
         return h === +h && p === +p && a === +a ? S.createElement("path", fu({}, y, {
-            className: re("recharts-symbols", l),
+            className: ee("recharts-symbols", l),
             transform: "translate(".concat(h, ", ").concat(p, ")"),
             d: f()
         })) : null
     };
 eo.registerSymbol = _w;
 
 function Pr(e) {
@@ -2270,15 +2270,15 @@
                     h = {
                         display: "inline-block",
                         verticalAlign: "middle",
                         marginRight: 4
                     };
                 return a.map(function(p, y) {
                     var v = p.formatter || c,
-                        d = re(jn(jn({
+                        d = ee(jn(jn({
                             "recharts-legend-item": !0
                         }, "legend-item-".concat(y), !0), "inactive", p.inactive));
                     if (p.type === "none") return null;
                     var w = Y(p.value) ? null : p.value;
                     At(!Y(p.value), `The name property is also required when using a function for the dataKey of a chart's cartesian components. Ex: <Bar name="Name of my Data"/>`);
                     var b = p.inactive ? s : p.color;
                     return S.createElement("li", hu({
@@ -2313,15 +2313,15 @@
                 };
                 return S.createElement("ul", {
                     className: "recharts-default-legend",
                     style: u
                 }, this.renderItems())
             }
         }]), t
-    }(B.PureComponent);
+    }(R.PureComponent);
 jn(Dc, "displayName", "Legend");
 jn(Dc, "defaultProps", {
     iconSize: 14,
     layout: "horizontal",
     align: "center",
     verticalAlign: "middle",
     inactiveColor: "#ccc"
@@ -2535,15 +2535,15 @@
 
 function U1(e, t) {
     for (var r = -1, n = t.length, i = e.length; ++r < n;) e[i + r] = t[r];
     return e
 }
 var xd = U1,
     K1 = xd,
-    q1 = Le;
+    q1 = Be;
 
 function H1(e, t, r) {
     var n = t(e);
     return q1(e) ? n : K1(n, r(e))
 }
 var G1 = H1;
 
@@ -2696,15 +2696,15 @@
     eA = Ad,
     il = JO,
     al = il && il.isTypedArray,
     tA = al ? eA(al) : QO,
     Sd = tA,
     rA = aO,
     nA = Lc,
-    iA = Le,
+    iA = Be,
     aA = Od,
     oA = Bc,
     uA = Sd,
     cA = Object.prototype,
     sA = cA.hasOwnProperty;
 
 function lA(e, t) {
@@ -2808,27 +2808,27 @@
         var m = e.constructor,
             g = t.constructor;
         m != g && "constructor" in e && "constructor" in t && !(typeof m == "function" && m instanceof m && typeof g == "function" && g instanceof g) && (v = !1)
     }
     return a.delete(e), a.delete(t), v
 }
 var zA = FA,
-    WA = sr,
+    WA = lr,
     UA = vt,
     KA = WA(UA, "DataView"),
     qA = KA,
-    HA = sr,
+    HA = lr,
     GA = vt,
     XA = HA(GA, "Promise"),
     VA = XA,
-    YA = sr,
+    YA = lr,
     ZA = vt,
     JA = YA(ZA, "Set"),
     _d = JA,
-    QA = sr,
+    QA = lr,
     eS = vt,
     tS = QA(eS, "WeakMap"),
     rS = tS,
     du = qA,
     vu = Pc,
     yu = VA,
     mu = _d,
@@ -2867,15 +2867,15 @@
 });
 var sS = Vt,
     Eo = vd,
     lS = bd,
     fS = W1,
     hS = zA,
     hl = sS,
-    pl = Le,
+    pl = Be,
     dl = Od,
     pS = Sd,
     dS = 1,
     vl = "[object Arguments]",
     yl = "[object Array]",
     _i = "[object Object]",
     vS = Object.prototype,
@@ -2983,15 +2983,15 @@
 
 function LS(e, t) {
     return e != null && t in Object(e)
 }
 var BS = LS,
     RS = Rp,
     FS = Lc,
-    zS = Le,
+    zS = Be,
     WS = Bc,
     US = Rc,
     KS = Va;
 
 function qS(e, t, r) {
     t = RS(t, e);
     for (var n = -1, i = t.length, a = !1; ++n < i;) {
@@ -3054,15 +3054,15 @@
 function gP(e) {
     return yP(e) ? dP(mP(e)) : vP(e)
 }
 var bP = gP,
     xP = NS,
     wP = uP,
     OP = Zr,
-    AP = Le,
+    AP = Be,
     SP = bP;
 
 function PP(e) {
     return typeof e == "function" ? e : e == null ? OP : typeof e == "object" ? AP(e) ? wP(e[0], e[1]) : xP(e) : SP(e)
 }
 var Ft = PP;
 
@@ -3433,25 +3433,25 @@
                 return a === "vertical" && N(n.props.height) ? {
                     height: n.props.height
                 } : a === "horizontal" ? {
                     width: n.props.width || i
                 } : null
             }
         }]), t
-    }(B.PureComponent);
+    }(R.PureComponent);
 ro(Mn, "displayName", "Legend");
 ro(Mn, "defaultProps", {
     iconSize: 14,
     layout: "horizontal",
     align: "center",
     verticalAlign: "bottom"
 });
 var Al = di,
     g_ = Lc,
-    b_ = Le,
+    b_ = Be,
     Sl = Al ? Al.isConcatSpreadable : void 0;
 
 function x_(e) {
     return b_(e) || g_(e) || !!(Sl && e && e[Sl])
 }
 var w_ = x_,
     O_ = xd,
@@ -3558,15 +3558,15 @@
     X_ = Ec,
     V_ = Ft,
     Y_ = Rd,
     Z_ = W_,
     J_ = Ad,
     Q_ = G_,
     e$ = Zr,
-    t$ = Le;
+    t$ = Be;
 
 function r$(e, t, r) {
     t.length ? t = Mo(t, function(a) {
         return t$(a) ? function(o) {
             return X_(o, a.length === 1 ? a[0] : a)
         } : a
     }) : t = [e$];
@@ -3618,15 +3618,15 @@
 
 function s$(e) {
     return function() {
         return e
     }
 }
 var l$ = s$,
-    f$ = sr,
+    f$ = lr,
     h$ = function() {
         try {
             var e = f$(Object, "defineProperty");
             return e({}, "", {}), e
         } catch {}
     }(),
     Fd = h$,
@@ -3837,37 +3837,37 @@
         b = w === void 0 ? !1 : w,
         x = function() {
             if (f && f.length) {
                 var _ = {
                         padding: 0,
                         margin: 0
                     },
-                    M = (h ? Wc(f, h) : f).map(function(j, k) {
+                    M = (h ? Wc(f, h) : f).map(function(j, D) {
                         if (j.type === "none") return null;
                         var C = Co({
                                 display: "block",
                                 paddingTop: 4,
                                 paddingBottom: 4,
                                 color: j.color || "#000"
                             }, u),
                             L = j.formatter || l || V$,
-                            R = j.value,
-                            F = j.name,
-                            q = R,
-                            Z = F;
+                            B = j.value,
+                            W = j.name,
+                            q = B,
+                            Z = W;
                         if (L && q != null && Z != null) {
-                            var U = L(R, F, j, k, f);
+                            var U = L(B, W, j, D, f);
                             if (Array.isArray(U)) {
-                                var ee = z$(U, 2);
-                                q = ee[0], Z = ee[1]
+                                var Q = z$(U, 2);
+                                q = Q[0], Z = Q[1]
                             } else q = U
                         }
                         return S.createElement("li", {
                             className: "recharts-tooltip-item",
-                            key: "tooltip-item-".concat(k),
+                            key: "tooltip-item-".concat(D),
                             style: C
                         }, be(Z) ? S.createElement("span", {
                             className: "recharts-tooltip-item-name"
                         }, Z) : null, be(Z) ? S.createElement("span", {
                             className: "recharts-tooltip-item-separator"
                         }, n) : null, S.createElement("span", {
                             className: "recharts-tooltip-item-value"
@@ -3888,28 +3888,28 @@
             backgroundColor: "#fff",
             border: "1px solid #ccc",
             whiteSpace: "nowrap"
         }, a),
         g = Co({
             margin: 0
         }, s),
-        O = !X(v),
+        O = !G(v),
         A = O ? v : "",
-        P = re("recharts-default-tooltip", p),
-        T = re("recharts-tooltip-label", y);
+        P = ee("recharts-default-tooltip", p),
+        E = ee("recharts-tooltip-label", y);
     O && d && f !== void 0 && f !== null && (A = d(v, f));
-    var E = b ? {
+    var T = b ? {
         role: "status",
         "aria-live": "assertive"
     } : {};
     return S.createElement("div", xu({
         className: P,
         style: m
-    }, E), S.createElement("p", {
-        className: T,
+    }, T), S.createElement("p", {
+        className: E,
         style: g
     }, S.isValidElement(A) ? A : "".concat(A)), x())
 };
 
 function In(e) {
     "@babel/helpers - typeof";
     return In = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
@@ -3948,15 +3948,15 @@
         visibility: "hidden"
     };
 
 function eT(e) {
     var t = e.coordinate,
         r = e.translateX,
         n = e.translateY;
-    return re(un, $i($i($i($i({}, "".concat(un, "-right"), N(r) && t && N(t.x) && r >= t.x), "".concat(un, "-left"), N(r) && t && N(t.x) && r < t.x), "".concat(un, "-bottom"), N(n) && t && N(t.y) && n >= t.y), "".concat(un, "-top"), N(n) && t && N(t.y) && n < t.y))
+    return ee(un, $i($i($i($i({}, "".concat(un, "-right"), N(r) && t && N(t.x) && r >= t.x), "".concat(un, "-left"), N(r) && t && N(t.x) && r < t.x), "".concat(un, "-bottom"), N(n) && t && N(t.y) && n >= t.y), "".concat(un, "-top"), N(n) && t && N(t.y) && n < t.y))
 }
 
 function Ml(e) {
     var t = e.allowEscapeViewBox,
         r = e.coordinate,
         n = e.key,
         i = e.offsetTopLeft,
@@ -4257,15 +4257,15 @@
                     style: O,
                     ref: function(P) {
                         n.wrapperNode = P
                     }
                 }, s)
             }
         }]), t
-    }(B.PureComponent),
+    }(R.PureComponent),
     lT = function() {
         return !(typeof window < "u" && window.document && window.document.createElement && window.setTimeout)
     },
     at = {
         isSsr: lT(),
         get: function(t) {
             return at[t]
@@ -4458,15 +4458,15 @@
                 viewBox: x,
                 wrapperStyle: m
             }, bT(s, Ll(Ll({}, this.props), {}, {
                 payload: g
             })))
         }
     }]), t
-}(B.PureComponent);
+}(R.PureComponent);
 Uc(gt, "displayName", "Tooltip");
 Uc(gt, "defaultProps", {
     accessibilityLayer: !1,
     allowEscapeViewBox: {
         x: !1,
         y: !1
     },
@@ -4564,16 +4564,16 @@
     function y(O) {
         return s = O, u = setTimeout(w, t), f ? p(O) : o
     }
 
     function v(O) {
         var A = O - c,
             P = O - s,
-            T = t - A;
-        return l ? FT(T, a - P) : T
+            E = t - A;
+        return l ? FT(E, a - P) : E
     }
 
     function d(O) {
         var A = O - c,
             P = O - s;
         return c === void 0 || A >= t || A < 0 || l && P >= a
     }
@@ -4730,15 +4730,15 @@
         return u
     }
 }
 
 function tE(e) {
     if (Array.isArray(e)) return e
 }
-var qF = B.forwardRef(function(e, t) {
+var HF = R.forwardRef(function(e, t) {
         var r = e.aspect,
             n = e.initialDimension,
             i = n === void 0 ? {
                 width: -1,
                 height: -1
             } : n,
             a = e.width,
@@ -4753,91 +4753,91 @@
             y = e.debounce,
             v = y === void 0 ? 0 : y,
             d = e.id,
             w = e.className,
             b = e.onResize,
             x = e.style,
             m = x === void 0 ? {} : x,
-            g = B.useRef(null),
-            O = B.useRef();
-        O.current = b, B.useImperativeHandle(t, function() {
+            g = R.useRef(null),
+            O = R.useRef();
+        O.current = b, R.useImperativeHandle(t, function() {
             return Object.defineProperty(g.current, "current", {
                 get: function() {
                     return console.warn("The usage of ref.current.current is deprecated and will no longer be supported."), g.current
                 },
                 configurable: !0
             })
         });
-        var A = B.useState({
+        var A = R.useState({
                 containerWidth: i.width,
                 containerHeight: i.height
             }),
             P = ZT(A, 2),
-            T = P[0],
-            E = P[1],
-            $ = B.useCallback(function(M, j) {
-                E(function(k) {
+            E = P[0],
+            T = P[1],
+            $ = R.useCallback(function(M, j) {
+                T(function(D) {
                     var C = Math.round(M),
                         L = Math.round(j);
-                    return k.containerWidth === C && k.containerHeight === L ? k : {
+                    return D.containerWidth === C && D.containerHeight === L ? D : {
                         containerWidth: C,
                         containerHeight: L
                     }
                 })
             }, []);
-        B.useEffect(function() {
-            var M = function(F) {
-                var q, Z = F[0].contentRect,
+        R.useEffect(function() {
+            var M = function(W) {
+                var q, Z = W[0].contentRect,
                     U = Z.width,
-                    ee = Z.height;
-                $(U, ee), (q = O.current) === null || q === void 0 || q.call(O, U, ee)
+                    Q = Z.height;
+                $(U, Q), (q = O.current) === null || q === void 0 || q.call(O, U, Q)
             };
             v > 0 && (M = Hd(M, v, {
                 trailing: !0,
                 leading: !1
             }));
             var j = new ResizeObserver(M),
-                k = g.current.getBoundingClientRect(),
-                C = k.width,
-                L = k.height;
+                D = g.current.getBoundingClientRect(),
+                C = D.width,
+                L = D.height;
             return $(C, L), j.observe(g.current),
                 function() {
                     j.disconnect()
                 }
         }, [$, v]);
-        var _ = B.useMemo(function() {
-            var M = T.containerWidth,
-                j = T.containerHeight;
+        var _ = R.useMemo(function() {
+            var M = E.containerWidth,
+                j = E.containerHeight;
             if (M < 0 || j < 0) return null;
             At(Zt(o) || Zt(c), `The width(%s) and height(%s) are both fixed numbers,
        maybe you don't need to use a ResponsiveContainer.`, o, c), At(!r || r > 0, "The aspect(%s) must be greater than zero.", r);
-            var k = Zt(o) ? M : o,
+            var D = Zt(o) ? M : o,
                 C = Zt(c) ? j : c;
-            r && r > 0 && (k ? C = k / r : C && (k = C * r), h && C > h && (C = h)), At(k > 0 || C > 0, `The width(%s) and height(%s) of chart should be greater than 0,
+            r && r > 0 && (D ? C = D / r : C && (D = C * r), h && C > h && (C = h)), At(D > 0 || C > 0, `The width(%s) and height(%s) of chart should be greater than 0,
        please check the style of container, or the props width(%s) and height(%s),
        or add a minWidth(%s) or minHeight(%s) or use aspect(%s) to control the
-       height and width.`, k, C, o, c, f, l, r);
+       height and width.`, D, C, o, c, f, l, r);
             var L = !Array.isArray(p) && Jo.isElement(p) && Ot(p.type).endsWith("Chart");
-            return S.Children.map(p, function(R) {
-                return Jo.isElement(R) ? B.cloneElement(R, Ti({
-                    width: k,
+            return S.Children.map(p, function(B) {
+                return Jo.isElement(B) ? R.cloneElement(B, Ti({
+                    width: D,
                     height: C
                 }, L ? {
                     style: Ti({
                         height: "100%",
                         width: "100%",
                         maxHeight: C,
-                        maxWidth: k
-                    }, R.props.style)
-                } : {})) : R
+                        maxWidth: D
+                    }, B.props.style)
+                } : {})) : B
             })
-        }, [r, p, c, h, l, f, T, o]);
+        }, [r, p, c, h, l, f, E, o]);
         return S.createElement("div", {
             id: d ? "".concat(d) : void 0,
-            className: re("recharts-responsive-container", w),
+            className: ee("recharts-responsive-container", w),
             style: Ti(Ti({}, m), {}, {
                 width: o,
                 height: c,
                 minWidth: f,
                 minHeight: l,
                 maxHeight: h
             }),
@@ -4901,15 +4901,15 @@
     if (r !== void 0) {
         var n = r.call(e, t || "default");
         if (Dn(n) != "object") return n;
         throw new TypeError("@@toPrimitive must return a primitive value.")
     }
     return (t === "string" ? String : Number)(e)
 }
-var dr = {
+var vr = {
         widthCache: {},
         cacheCount: 0
     },
     aE = 2e3,
     oE = {
         position: "absolute",
         top: "-20000px",
@@ -4934,26 +4934,26 @@
             height: 0
         };
         var n = uE(r),
             i = JSON.stringify({
                 text: t,
                 copyStyle: n
             });
-        if (dr.widthCache[i]) return dr.widthCache[i];
+        if (vr.widthCache[i]) return vr.widthCache[i];
         try {
             var a = document.getElementById(ql);
             a || (a = document.createElement("span"), a.setAttribute("id", ql), a.setAttribute("aria-hidden", "true"), document.body.appendChild(a));
             var o = Au(Au({}, oE), n);
             Object.assign(a.style, o), a.textContent = "".concat(t);
             var u = a.getBoundingClientRect(),
                 c = {
                     width: u.width,
                     height: u.height
                 };
-            return dr.widthCache[i] = c, ++dr.cacheCount > aE && (dr.cacheCount = 0, dr.widthCache = {}), c
+            return vr.widthCache[i] = c, ++vr.cacheCount > aE && (vr.cacheCount = 0, vr.widthCache = {}), c
         } catch {
             return {
                 width: 0,
                 height: 0
             }
         }
     },
@@ -5068,15 +5068,15 @@
         pt: 96 / 72,
         pc: 96 / 6,
         in: 96,
         Q: 96 / (2.54 * 40),
         px: 1
     },
     bE = Object.keys(Gd),
-    gr = "NaN";
+    br = "NaN";
 
 function xE(e, t) {
     return e * Gd[t]
 }
 var Ei = function() {
     function e(t, r) {
         pE(this, e), this.num = t, this.unit = r, this.num = t, this.unit = r, Number.isNaN(t) && (this.unit = ""), r !== "" && !mE.test(r) && (this.num = NaN, this.unit = ""), bE.includes(r) && (this.num = xE(t, r), this.unit = "px")
@@ -5120,37 +5120,37 @@
                 u = a[2];
             return new e(parseFloat(o), u ?? "")
         }
     }]), e
 }();
 
 function Xd(e) {
-    if (e.includes(gr)) return gr;
+    if (e.includes(br)) return br;
     for (var t = e; t.includes("*") || t.includes("/");) {
         var r, n = (r = Xl.exec(t)) !== null && r !== void 0 ? r : [],
             i = ta(n, 4),
             a = i[1],
             o = i[2],
             u = i[3],
             c = Ei.parse(a ?? ""),
             s = Ei.parse(u ?? ""),
             f = o === "*" ? c.multiply(s) : c.divide(s);
-        if (f.isNaN()) return gr;
+        if (f.isNaN()) return br;
         t = t.replace(Xl, f.toString())
     }
     for (; t.includes("+") || /.-\d+(?:\.\d+)?/.test(t);) {
         var l, h = (l = Vl.exec(t)) !== null && l !== void 0 ? l : [],
             p = ta(h, 4),
             y = p[1],
             v = p[2],
             d = p[3],
             w = Ei.parse(y ?? ""),
             b = Ei.parse(d ?? ""),
             x = v === "+" ? w.add(b) : w.subtract(b);
-        if (x.isNaN()) return gr;
+        if (x.isNaN()) return br;
         t = t.replace(Vl, x.toString())
     }
     return t
 }
 var Yl = /\(([^()]*)\)/;
 
 function wE(e) {
@@ -5168,21 +5168,21 @@
     return t = wE(t), t = Xd(t), t
 }
 
 function AE(e) {
     try {
         return OE(e)
     } catch {
-        return gr
+        return br
     }
 }
 
 function ko(e) {
     var t = AE(e.slice(5, -1));
-    return t === gr ? "" : t
+    return t === br ? "" : t
 }
 var SE = ["x", "y", "lineHeight", "capHeight", "scaleToFit", "textAnchor", "verticalAnchor", "fill"],
     PE = ["dx", "dy", "angle", "className", "breakAll"];
 
 function Su() {
     return Su = Object.assign ? Object.assign.bind() : function(e) {
         for (var t = 1; t < arguments.length; t++) {
@@ -5268,15 +5268,15 @@
 var Vd = /[ \f\n\r\t\v\u2028\u2029]+/,
     Yd = function(t) {
         var r = t.children,
             n = t.breakAll,
             i = t.style;
         try {
             var a = [];
-            X(r) || (n ? a = r.toString().split("") : a = r.toString().split(Vd));
+            G(r) || (n ? a = r.toString().split("") : a = r.toString().split(Vd));
             var o = a.map(function(c) {
                     return {
                         word: c,
                         width: xn(c, i).width
                     }
                 }),
                 u = n ? 0 : xn(" ", i).width;
@@ -5292,67 +5292,67 @@
         var o = t.maxLines,
             u = t.children,
             c = t.style,
             s = t.breakAll,
             f = N(o),
             l = u,
             h = function() {
-                var k = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : [];
-                return k.reduce(function(C, L) {
-                    var R = L.word,
-                        F = L.width,
+                var D = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : [];
+                return D.reduce(function(C, L) {
+                    var B = L.word,
+                        W = L.width,
                         q = C[C.length - 1];
-                    if (q && (i == null || a || q.width + F + n < Number(i))) q.words.push(R), q.width += F + n;
+                    if (q && (i == null || a || q.width + W + n < Number(i))) q.words.push(B), q.width += W + n;
                     else {
                         var Z = {
-                            words: [R],
-                            width: F
+                            words: [B],
+                            width: W
                         };
                         C.push(Z)
                     }
                     return C
                 }, [])
             },
             p = h(r),
-            y = function(k) {
-                return k.reduce(function(C, L) {
+            y = function(D) {
+                return D.reduce(function(C, L) {
                     return C.width > L.width ? C : L
                 })
             };
         if (!f) return p;
-        for (var v = "…", d = function(k) {
-                var C = l.slice(0, k),
+        for (var v = "…", d = function(D) {
+                var C = l.slice(0, D),
                     L = Yd({
                         breakAll: s,
                         style: c,
                         children: C + v
                     }).wordsWithComputedWidth,
-                    R = h(L),
-                    F = R.length > o || y(R).width > Number(i);
-                return [F, R]
+                    B = h(L),
+                    W = B.length > o || y(B).width > Number(i);
+                return [W, B]
             }, w = 0, b = l.length - 1, x = 0, m; w <= b && x <= l.length - 1;) {
             var g = Math.floor((w + b) / 2),
                 O = g - 1,
                 A = d(O),
                 P = Jl(A, 2),
-                T = P[0],
-                E = P[1],
+                E = P[0],
+                T = P[1],
                 $ = d(g),
                 _ = Jl($, 1),
                 M = _[0];
-            if (!T && !M && (w = g + 1), T && M && (b = g - 1), !T && M) {
-                m = E;
+            if (!E && !M && (w = g + 1), E && M && (b = g - 1), !E && M) {
+                m = T;
                 break
             }
             x++
         }
         return m || p
     },
     ef = function(t) {
-        var r = X(t) ? [] : t.toString().split(Vd);
+        var r = G(t) ? [] : t.toString().split(Vd);
         return [{
             words: r
         }]
     },
     CE = function(t) {
         var r = t.width,
             n = t.scaleToFit,
@@ -5395,32 +5395,32 @@
             h = t.textAnchor,
             p = h === void 0 ? "start" : h,
             y = t.verticalAnchor,
             v = y === void 0 ? "end" : y,
             d = t.fill,
             w = d === void 0 ? tf : d,
             b = Zl(t, SE),
-            x = B.useMemo(function() {
+            x = R.useMemo(function() {
                 return CE({
                     breakAll: b.breakAll,
                     children: b.children,
                     maxLines: b.maxLines,
                     scaleToFit: l,
                     style: b.style,
                     width: b.width
                 })
             }, [b.breakAll, b.children, b.maxLines, l, b.style, b.width]),
             m = b.dx,
             g = b.dy,
             O = b.angle,
             A = b.className,
             P = b.breakAll,
-            T = Zl(b, PE);
+            E = Zl(b, PE);
         if (!be(n) || !be(a)) return null;
-        var E = n + (N(m) ? m : 0),
+        var T = n + (N(m) ? m : 0),
             $ = a + (N(g) ? g : 0),
             _;
         switch (v) {
             case "start":
                 _ = ko("calc(".concat(s, ")"));
                 break;
             case "middle":
@@ -5429,30 +5429,30 @@
             default:
                 _ = ko("calc(".concat(x.length - 1, " * -").concat(u, ")"));
                 break
         }
         var M = [];
         if (l) {
             var j = x[0].width,
-                k = b.width;
-            M.push("scale(".concat((N(k) ? k / j : 1) / j, ")"))
+                D = b.width;
+            M.push("scale(".concat((N(D) ? D / j : 1) / j, ")"))
         }
-        return O && M.push("rotate(".concat(O, ", ").concat(E, ", ").concat($, ")")), M.length && (T.transform = M.join(" ")), S.createElement("text", Su({}, G(T, !0), {
-            x: E,
+        return O && M.push("rotate(".concat(O, ", ").concat(T, ", ").concat($, ")")), M.length && (E.transform = M.join(" ")), S.createElement("text", Su({}, H(E, !0), {
+            x: T,
             y: $,
-            className: re("recharts-text", A),
+            className: ee("recharts-text", A),
             textAnchor: p,
             fill: w.includes("url") ? tf : w
         }), x.map(function(C, L) {
-            var R = C.words.join(P ? "" : " ");
+            var B = C.words.join(P ? "" : " ");
             return S.createElement("tspan", {
-                x: E,
+                x: T,
                 dy: L === 0 ? _ : u,
-                key: R
-            }, R)
+                key: B
+            }, B)
         }))
     };
 
 function Bt(e, t) {
     return e == null || t == null ? NaN : e < t ? -1 : e > t ? 1 : e >= t ? 0 : NaN
 }
 
@@ -5835,21 +5835,21 @@
     for (var n in t) r[n] = t[n];
     return r
 }
 
 function gi() {}
 var Bn = .7,
     ia = 1 / Bn,
-    wr = "\\s*([+-]?\\d+)\\s*",
+    Or = "\\s*([+-]?\\d+)\\s*",
     Rn = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
     ft = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
     GE = /^#([0-9a-f]{3,8})$/,
-    XE = new RegExp(`^rgb\\(${wr},${wr},${wr}\\)$`),
+    XE = new RegExp(`^rgb\\(${Or},${Or},${Or}\\)$`),
     VE = new RegExp(`^rgb\\(${ft},${ft},${ft}\\)$`),
-    YE = new RegExp(`^rgba\\(${wr},${wr},${wr},${Rn}\\)$`),
+    YE = new RegExp(`^rgba\\(${Or},${Or},${Or},${Rn}\\)$`),
     ZE = new RegExp(`^rgba\\(${ft},${ft},${ft},${Rn}\\)$`),
     JE = new RegExp(`^hsl\\(${Rn},${ft},${ft}\\)$`),
     QE = new RegExp(`^hsla\\(${Rn},${ft},${ft},${Rn}\\)$`),
     uf = {
         aliceblue: 15792383,
         antiquewhite: 16444375,
         aqua: 65535,
@@ -6028,48 +6028,48 @@
 
 function sf() {
     return this.rgb().formatRgb()
 }
 
 function Fn(e) {
     var t, r;
-    return e = (e + "").trim().toLowerCase(), (t = GE.exec(e)) ? (r = t[1].length, t = parseInt(t[1], 16), r === 6 ? lf(t) : r === 3 ? new De(t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | t & 240, (t & 15) << 4 | t & 15, 1) : r === 8 ? ji(t >> 24 & 255, t >> 16 & 255, t >> 8 & 255, (t & 255) / 255) : r === 4 ? ji(t >> 12 & 15 | t >> 8 & 240, t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | t & 240, ((t & 15) << 4 | t & 15) / 255) : null) : (t = XE.exec(e)) ? new De(t[1], t[2], t[3], 1) : (t = VE.exec(e)) ? new De(t[1] * 255 / 100, t[2] * 255 / 100, t[3] * 255 / 100, 1) : (t = YE.exec(e)) ? ji(t[1], t[2], t[3], t[4]) : (t = ZE.exec(e)) ? ji(t[1] * 255 / 100, t[2] * 255 / 100, t[3] * 255 / 100, t[4]) : (t = JE.exec(e)) ? pf(t[1], t[2] / 100, t[3] / 100, 1) : (t = QE.exec(e)) ? pf(t[1], t[2] / 100, t[3] / 100, t[4]) : uf.hasOwnProperty(e) ? lf(uf[e]) : e === "transparent" ? new De(NaN, NaN, NaN, 0) : null
+    return e = (e + "").trim().toLowerCase(), (t = GE.exec(e)) ? (r = t[1].length, t = parseInt(t[1], 16), r === 6 ? lf(t) : r === 3 ? new Ne(t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | t & 240, (t & 15) << 4 | t & 15, 1) : r === 8 ? ji(t >> 24 & 255, t >> 16 & 255, t >> 8 & 255, (t & 255) / 255) : r === 4 ? ji(t >> 12 & 15 | t >> 8 & 240, t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | t & 240, ((t & 15) << 4 | t & 15) / 255) : null) : (t = XE.exec(e)) ? new Ne(t[1], t[2], t[3], 1) : (t = VE.exec(e)) ? new Ne(t[1] * 255 / 100, t[2] * 255 / 100, t[3] * 255 / 100, 1) : (t = YE.exec(e)) ? ji(t[1], t[2], t[3], t[4]) : (t = ZE.exec(e)) ? ji(t[1] * 255 / 100, t[2] * 255 / 100, t[3] * 255 / 100, t[4]) : (t = JE.exec(e)) ? pf(t[1], t[2] / 100, t[3] / 100, 1) : (t = QE.exec(e)) ? pf(t[1], t[2] / 100, t[3] / 100, t[4]) : uf.hasOwnProperty(e) ? lf(uf[e]) : e === "transparent" ? new Ne(NaN, NaN, NaN, 0) : null
 }
 
 function lf(e) {
-    return new De(e >> 16 & 255, e >> 8 & 255, e & 255, 1)
+    return new Ne(e >> 16 & 255, e >> 8 & 255, e & 255, 1)
 }
 
 function ji(e, t, r, n) {
-    return n <= 0 && (e = t = r = NaN), new De(e, t, r, n)
+    return n <= 0 && (e = t = r = NaN), new Ne(e, t, r, n)
 }
 
 function rj(e) {
-    return e instanceof gi || (e = Fn(e)), e ? (e = e.rgb(), new De(e.r, e.g, e.b, e.opacity)) : new De
+    return e instanceof gi || (e = Fn(e)), e ? (e = e.rgb(), new Ne(e.r, e.g, e.b, e.opacity)) : new Ne
 }
 
 function Eu(e, t, r, n) {
-    return arguments.length === 1 ? rj(e) : new De(e, t, r, n ?? 1)
+    return arguments.length === 1 ? rj(e) : new Ne(e, t, r, n ?? 1)
 }
 
-function De(e, t, r, n) {
+function Ne(e, t, r, n) {
     this.r = +e, this.g = +t, this.b = +r, this.opacity = +n
 }
-Gc(De, Eu, tv(gi, {
+Gc(Ne, Eu, tv(gi, {
     brighter(e) {
-        return e = e == null ? ia : Math.pow(ia, e), new De(this.r * e, this.g * e, this.b * e, this.opacity)
+        return e = e == null ? ia : Math.pow(ia, e), new Ne(this.r * e, this.g * e, this.b * e, this.opacity)
     },
     darker(e) {
-        return e = e == null ? Bn : Math.pow(Bn, e), new De(this.r * e, this.g * e, this.b * e, this.opacity)
+        return e = e == null ? Bn : Math.pow(Bn, e), new Ne(this.r * e, this.g * e, this.b * e, this.opacity)
     },
     rgb() {
         return this
     },
     clamp() {
-        return new De(rr(this.r), rr(this.g), rr(this.b), aa(this.opacity))
+        return new Ne(rr(this.r), rr(this.g), rr(this.b), aa(this.opacity))
     },
     displayable() {
         return -.5 <= this.r && this.r < 255.5 && -.5 <= this.g && this.g < 255.5 && -.5 <= this.b && this.b < 255.5 && 0 <= this.opacity && this.opacity <= 1
     },
     hex: ff,
     formatHex: ff,
     formatHex8: nj,
@@ -6138,15 +6138,15 @@
     },
     rgb() {
         var e = this.h % 360 + (this.h < 0) * 360,
             t = isNaN(e) || isNaN(this.s) ? 0 : this.s,
             r = this.l,
             n = r + (r < .5 ? r : 1 - r) * t,
             i = 2 * r - n;
-        return new De(Do(e >= 240 ? e - 240 : e + 120, i, n), Do(e, i, n), Do(e < 120 ? e + 240 : e - 120, i, n), this.opacity)
+        return new Ne(Do(e >= 240 ? e - 240 : e + 120, i, n), Do(e, i, n), Do(e < 120 ? e + 240 : e - 120, i, n), this.opacity)
     },
     clamp() {
         return new nt(df(this.h), Mi(this.s), Mi(this.l), aa(this.opacity))
     },
     displayable() {
         return (0 <= this.s && this.s <= 1 || isNaN(this.s)) && 0 <= this.l && this.l <= 1 && 0 <= this.opacity && this.opacity <= 1
     },
@@ -6322,15 +6322,15 @@
 }
 
 function ua(e) {
     return +e
 }
 var yf = [0, 1];
 
-function ke(e) {
+function Ie(e) {
     return e
 }
 
 function Mu(e, t) {
     return (t -= e = +e) ? function(r) {
         return (r - e) / t
     } : mj(isNaN(t) ? NaN : .5)
@@ -6371,47 +6371,47 @@
     return t.domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown())
 }
 
 function io() {
     var e = yf,
         t = yf,
         r = Jr,
-        n, i, a, o = ke,
+        n, i, a, o = Ie,
         u, c, s;
 
     function f() {
         var h = Math.min(e.length, t.length);
-        return o !== ke && (o = gj(e[0], e[h - 1])), u = h > 2 ? xj : bj, c = s = null, l
+        return o !== Ie && (o = gj(e[0], e[h - 1])), u = h > 2 ? xj : bj, c = s = null, l
     }
 
     function l(h) {
         return h == null || isNaN(h = +h) ? a : (c || (c = u(e.map(n), t, r)))(n(o(h)))
     }
     return l.invert = function(h) {
             return o(i((s || (s = u(t, e.map(n), oa)))(h)))
         }, l.domain = function(h) {
             return arguments.length ? (e = Array.from(h, ua), f()) : e.slice()
         }, l.range = function(h) {
             return arguments.length ? (t = Array.from(h), f()) : t.slice()
         }, l.rangeRound = function(h) {
             return t = Array.from(h), r = Vc, f()
         }, l.clamp = function(h) {
-            return arguments.length ? (o = h ? !0 : ke, f()) : o !== ke
+            return arguments.length ? (o = h ? !0 : Ie, f()) : o !== Ie
         }, l.interpolate = function(h) {
             return arguments.length ? (r = h, f()) : r
         }, l.unknown = function(h) {
             return arguments.length ? (a = h, l) : a
         },
         function(h, p) {
             return n = h, i = p, f()
         }
 }
 
 function Yc() {
-    return io()(ke, ke)
+    return io()(Ie, Ie)
 }
 
 function wj(e) {
     return Math.abs(e = Math.round(e)) >= 1e21 ? e.toLocaleString("en").replace(/,/g, "") : e.toString(10)
 }
 
 function ca(e, t) {
@@ -6543,55 +6543,55 @@
             x = l.precision,
             m = l.trim,
             g = l.type;
         g === "n" ? (b = !0, g = "g") : gf[g] || (x === void 0 && (x = 12), m = !0, g = "g"), (d || h === "0" && p === "=") && (d = !0, h = "0", p = "=");
         var O = v === "$" ? r : v === "#" && /[boxX]/.test(g) ? "0" + g.toLowerCase() : "",
             A = v === "$" ? n : /[%p]/.test(g) ? o : "",
             P = gf[g],
-            T = /[defgprs%]/.test(g);
+            E = /[defgprs%]/.test(g);
         x = x === void 0 ? 6 : /[gprs]/.test(g) ? Math.max(1, Math.min(21, x)) : Math.max(0, Math.min(20, x));
 
-        function E($) {
+        function T($) {
             var _ = O,
                 M = A,
-                j, k, C;
+                j, D, C;
             if (g === "c") M = P($) + M, $ = "";
             else {
                 $ = +$;
                 var L = $ < 0 || 1 / $ < 0;
-                if ($ = isNaN($) ? c : P(Math.abs($), x), m && ($ = Pj($)), L && +$ == 0 && y !== "+" && (L = !1), _ = (L ? y === "(" ? y : u : y === "-" || y === "(" ? "" : y) + _, M = (g === "s" ? wf[8 + iv / 3] : "") + M + (L && y === "(" ? ")" : ""), T) {
-                    for (j = -1, k = $.length; ++j < k;)
+                if ($ = isNaN($) ? c : P(Math.abs($), x), m && ($ = Pj($)), L && +$ == 0 && y !== "+" && (L = !1), _ = (L ? y === "(" ? y : u : y === "-" || y === "(" ? "" : y) + _, M = (g === "s" ? wf[8 + iv / 3] : "") + M + (L && y === "(" ? ")" : ""), E) {
+                    for (j = -1, D = $.length; ++j < D;)
                         if (C = $.charCodeAt(j), 48 > C || C > 57) {
                             M = (C === 46 ? i + $.slice(j + 1) : $.slice(j)) + M, $ = $.slice(0, j);
                             break
                         }
                 }
             }
             b && !d && ($ = t($, 1 / 0));
-            var R = _.length + $.length + M.length,
-                F = R < w ? new Array(w - R + 1).join(h) : "";
-            switch (b && d && ($ = t(F + $, F.length ? w - M.length : 1 / 0), F = ""), p) {
+            var B = _.length + $.length + M.length,
+                W = B < w ? new Array(w - B + 1).join(h) : "";
+            switch (b && d && ($ = t(W + $, W.length ? w - M.length : 1 / 0), W = ""), p) {
                 case "<":
-                    $ = _ + $ + M + F;
+                    $ = _ + $ + M + W;
                     break;
                 case "=":
-                    $ = _ + F + $ + M;
+                    $ = _ + W + $ + M;
                     break;
                 case "^":
-                    $ = F.slice(0, R = F.length >> 1) + _ + $ + M + F.slice(R);
+                    $ = W.slice(0, B = W.length >> 1) + _ + $ + M + W.slice(B);
                     break;
                 default:
-                    $ = F + _ + $ + M;
+                    $ = W + _ + $ + M;
                     break
             }
             return a($)
         }
-        return E.toString = function() {
+        return T.toString = function() {
             return l + ""
-        }, E
+        }, T
     }
 
     function f(l, h) {
         var p = s((l = zn(l), l.type = "f", l)),
             y = Math.max(-8, Math.min(8, Math.floor(Er(h) / 3))) * 3,
             v = Math.pow(10, -y),
             d = wf[8 + y / 3];
@@ -6840,19 +6840,19 @@
 }
 
 function Bj(e) {
     return e < 0 ? -e * e : e * e
 }
 
 function ts(e) {
-    var t = e(ke, ke),
+    var t = e(Ie, Ie),
         r = 1;
 
     function n() {
-        return r === 1 ? e(ke, ke) : r === .5 ? e(Lj, Bj) : e($f(r), $f(1 / r))
+        return r === 1 ? e(Ie, Ie) : r === .5 ? e(Lj, Bj) : e($f(r), $f(1 / r))
     }
     return t.exponent = function(i) {
         return arguments.length ? (r = +i, n()) : r
     }, zt(t)
 }
 
 function rs() {
@@ -7079,50 +7079,50 @@
 const vv = we(e => {
     e.setUTCHours(0, 0, 0, 0)
 }, (e, t) => {
     e.setUTCDate(e.getUTCDate() + t)
 }, (e, t) => (t - e) / Pt, e => Math.floor(e / Pt));
 vv.range;
 
-function fr(e) {
+function hr(e) {
     return we(t => {
         t.setDate(t.getDate() - (t.getDay() + 7 - e) % 7), t.setHours(0, 0, 0, 0)
     }, (t, r) => {
         t.setDate(t.getDate() + r * 7)
     }, (t, r) => (r - t - (r.getTimezoneOffset() - t.getTimezoneOffset()) * Ye) / ns)
 }
-const oo = fr(0),
-    fa = fr(1),
-    zj = fr(2),
-    Wj = fr(3),
-    jr = fr(4),
-    Uj = fr(5),
-    Kj = fr(6);
+const oo = hr(0),
+    fa = hr(1),
+    zj = hr(2),
+    Wj = hr(3),
+    jr = hr(4),
+    Uj = hr(5),
+    Kj = hr(6);
 oo.range;
 fa.range;
 zj.range;
 Wj.range;
 jr.range;
 Uj.range;
 Kj.range;
 
-function hr(e) {
+function pr(e) {
     return we(t => {
         t.setUTCDate(t.getUTCDate() - (t.getUTCDay() + 7 - e) % 7), t.setUTCHours(0, 0, 0, 0)
     }, (t, r) => {
         t.setUTCDate(t.getUTCDate() + r * 7)
     }, (t, r) => (r - t) / ns)
 }
-const uo = hr(0),
-    ha = hr(1),
-    qj = hr(2),
-    Hj = hr(3),
-    Mr = hr(4),
-    Gj = hr(5),
-    Xj = hr(6);
+const uo = pr(0),
+    ha = pr(1),
+    qj = pr(2),
+    Hj = pr(3),
+    Mr = pr(4),
+    Gj = pr(5),
+    Xj = pr(6);
 uo.range;
 ha.range;
 qj.range;
 Hj.range;
 Mr.range;
 Gj.range;
 Xj.range;
@@ -7248,16 +7248,16 @@
         y = fn(o),
         v = ln(u),
         d = fn(u),
         w = ln(c),
         b = fn(c),
         x = {
             a: L,
-            A: R,
-            b: F,
+            A: B,
+            b: W,
             B: q,
             c: null,
             d: Df,
             e: Df,
             f: OM,
             g: CM,
             G: kM,
@@ -7281,32 +7281,32 @@
             X: null,
             y: MM,
             Y: IM,
             Z: DM,
             "%": Lf
         },
         m = {
-            a: ee,
-            A: Te,
-            b: Ee,
+            a: Q,
+            A: _e,
+            b: ke,
             B: Kt,
             c: null,
             d: Nf,
             e: Nf,
             f: RM,
             g: VM,
             G: ZM,
             H: NM,
             I: LM,
             j: BM,
             L: bv,
             m: FM,
             M: zM,
-            p: yt,
-            q: Ke,
+            p: De,
+            q: yt,
             Q: Bf,
             s: Rf,
             S: WM,
             u: UM,
             U: KM,
             V: qM,
             w: HM,
@@ -7315,15 +7315,15 @@
             X: null,
             y: XM,
             Y: YM,
             Z: JM,
             "%": Lf
         },
         g = {
-            a: E,
+            a: T,
             A: $,
             b: _,
             B: M,
             c: j,
             d: If,
             e: If,
             f: vM,
@@ -7331,179 +7331,179 @@
             G: Mf,
             H: kf,
             I: kf,
             j: fM,
             L: dM,
             m: lM,
             M: hM,
-            p: T,
+            p: E,
             q: sM,
             Q: mM,
             s: gM,
             S: pM,
             u: iM,
             U: aM,
             V: oM,
             w: nM,
             W: uM,
-            x: k,
+            x: D,
             X: C,
             y: Cf,
             Y: Mf,
             Z: cM,
             "%": yM
         };
     x.x = O(r, x), x.X = O(n, x), x.c = O(t, x), m.x = O(r, m), m.X = O(n, m), m.c = O(t, m);
 
-    function O(z, H) {
+    function O(F, X) {
         return function(J) {
-            var D = [],
+            var k = [],
                 pe = -1,
-                Q = 0,
-                me = z.length,
-                ve, Be, mt;
-            for (J instanceof Date || (J = new Date(+J)); ++pe < me;) z.charCodeAt(pe) === 37 && (D.push(z.slice(Q, pe)), (Be = jf[ve = z.charAt(++pe)]) != null ? ve = z.charAt(++pe) : Be = ve === "e" ? " " : "0", (mt = H[ve]) && (ve = mt(J, Be)), D.push(ve), Q = pe + 1);
-            return D.push(z.slice(Q, pe)), D.join("")
+                re = 0,
+                me = F.length,
+                ve, Re, mt;
+            for (J instanceof Date || (J = new Date(+J)); ++pe < me;) F.charCodeAt(pe) === 37 && (k.push(F.slice(re, pe)), (Re = jf[ve = F.charAt(++pe)]) != null ? ve = F.charAt(++pe) : Re = ve === "e" ? " " : "0", (mt = X[ve]) && (ve = mt(J, Re)), k.push(ve), re = pe + 1);
+            return k.push(F.slice(re, pe)), k.join("")
         }
     }
 
-    function A(z, H) {
+    function A(F, X) {
         return function(J) {
-            var D = sn(1900, void 0, 1),
-                pe = P(D, z, J += "", 0),
-                Q, me;
+            var k = sn(1900, void 0, 1),
+                pe = P(k, F, J += "", 0),
+                re, me;
             if (pe != J.length) return null;
-            if ("Q" in D) return new Date(D.Q);
-            if ("s" in D) return new Date(D.s * 1e3 + ("L" in D ? D.L : 0));
-            if (H && !("Z" in D) && (D.Z = 0), "p" in D && (D.H = D.H % 12 + D.p * 12), D.m === void 0 && (D.m = "q" in D ? D.q : 0), "V" in D) {
-                if (D.V < 1 || D.V > 53) return null;
-                "w" in D || (D.w = 1), "Z" in D ? (Q = zo(sn(D.y, 0, 1)), me = Q.getUTCDay(), Q = me > 4 || me === 0 ? ha.ceil(Q) : ha(Q), Q = ao.offset(Q, (D.V - 1) * 7), D.y = Q.getUTCFullYear(), D.m = Q.getUTCMonth(), D.d = Q.getUTCDate() + (D.w + 6) % 7) : (Q = Fo(sn(D.y, 0, 1)), me = Q.getDay(), Q = me > 4 || me === 0 ? fa.ceil(Q) : fa(Q), Q = xi.offset(Q, (D.V - 1) * 7), D.y = Q.getFullYear(), D.m = Q.getMonth(), D.d = Q.getDate() + (D.w + 6) % 7)
-            } else("W" in D || "U" in D) && ("w" in D || (D.w = "u" in D ? D.u % 7 : "W" in D ? 1 : 0), me = "Z" in D ? zo(sn(D.y, 0, 1)).getUTCDay() : Fo(sn(D.y, 0, 1)).getDay(), D.m = 0, D.d = "W" in D ? (D.w + 6) % 7 + D.W * 7 - (me + 5) % 7 : D.w + D.U * 7 - (me + 6) % 7);
-            return "Z" in D ? (D.H += D.Z / 100 | 0, D.M += D.Z % 100, zo(D)) : Fo(D)
+            if ("Q" in k) return new Date(k.Q);
+            if ("s" in k) return new Date(k.s * 1e3 + ("L" in k ? k.L : 0));
+            if (X && !("Z" in k) && (k.Z = 0), "p" in k && (k.H = k.H % 12 + k.p * 12), k.m === void 0 && (k.m = "q" in k ? k.q : 0), "V" in k) {
+                if (k.V < 1 || k.V > 53) return null;
+                "w" in k || (k.w = 1), "Z" in k ? (re = zo(sn(k.y, 0, 1)), me = re.getUTCDay(), re = me > 4 || me === 0 ? ha.ceil(re) : ha(re), re = ao.offset(re, (k.V - 1) * 7), k.y = re.getUTCFullYear(), k.m = re.getUTCMonth(), k.d = re.getUTCDate() + (k.w + 6) % 7) : (re = Fo(sn(k.y, 0, 1)), me = re.getDay(), re = me > 4 || me === 0 ? fa.ceil(re) : fa(re), re = xi.offset(re, (k.V - 1) * 7), k.y = re.getFullYear(), k.m = re.getMonth(), k.d = re.getDate() + (k.w + 6) % 7)
+            } else("W" in k || "U" in k) && ("w" in k || (k.w = "u" in k ? k.u % 7 : "W" in k ? 1 : 0), me = "Z" in k ? zo(sn(k.y, 0, 1)).getUTCDay() : Fo(sn(k.y, 0, 1)).getDay(), k.m = 0, k.d = "W" in k ? (k.w + 6) % 7 + k.W * 7 - (me + 5) % 7 : k.w + k.U * 7 - (me + 6) % 7);
+            return "Z" in k ? (k.H += k.Z / 100 | 0, k.M += k.Z % 100, zo(k)) : Fo(k)
         }
     }
 
-    function P(z, H, J, D) {
-        for (var pe = 0, Q = H.length, me = J.length, ve, Be; pe < Q;) {
-            if (D >= me) return -1;
-            if (ve = H.charCodeAt(pe++), ve === 37) {
-                if (ve = H.charAt(pe++), Be = g[ve in jf ? H.charAt(pe++) : ve], !Be || (D = Be(z, J, D)) < 0) return -1
-            } else if (ve != J.charCodeAt(D++)) return -1
+    function P(F, X, J, k) {
+        for (var pe = 0, re = X.length, me = J.length, ve, Re; pe < re;) {
+            if (k >= me) return -1;
+            if (ve = X.charCodeAt(pe++), ve === 37) {
+                if (ve = X.charAt(pe++), Re = g[ve in jf ? X.charAt(pe++) : ve], !Re || (k = Re(F, J, k)) < 0) return -1
+            } else if (ve != J.charCodeAt(k++)) return -1
         }
-        return D
+        return k
     }
 
-    function T(z, H, J) {
-        var D = s.exec(H.slice(J));
-        return D ? (z.p = f.get(D[0].toLowerCase()), J + D[0].length) : -1
+    function E(F, X, J) {
+        var k = s.exec(X.slice(J));
+        return k ? (F.p = f.get(k[0].toLowerCase()), J + k[0].length) : -1
     }
 
-    function E(z, H, J) {
-        var D = p.exec(H.slice(J));
-        return D ? (z.w = y.get(D[0].toLowerCase()), J + D[0].length) : -1
+    function T(F, X, J) {
+        var k = p.exec(X.slice(J));
+        return k ? (F.w = y.get(k[0].toLowerCase()), J + k[0].length) : -1
     }
 
-    function $(z, H, J) {
-        var D = l.exec(H.slice(J));
-        return D ? (z.w = h.get(D[0].toLowerCase()), J + D[0].length) : -1
+    function $(F, X, J) {
+        var k = l.exec(X.slice(J));
+        return k ? (F.w = h.get(k[0].toLowerCase()), J + k[0].length) : -1
     }
 
-    function _(z, H, J) {
-        var D = w.exec(H.slice(J));
-        return D ? (z.m = b.get(D[0].toLowerCase()), J + D[0].length) : -1
+    function _(F, X, J) {
+        var k = w.exec(X.slice(J));
+        return k ? (F.m = b.get(k[0].toLowerCase()), J + k[0].length) : -1
     }
 
-    function M(z, H, J) {
-        var D = v.exec(H.slice(J));
-        return D ? (z.m = d.get(D[0].toLowerCase()), J + D[0].length) : -1
+    function M(F, X, J) {
+        var k = v.exec(X.slice(J));
+        return k ? (F.m = d.get(k[0].toLowerCase()), J + k[0].length) : -1
     }
 
-    function j(z, H, J) {
-        return P(z, t, H, J)
+    function j(F, X, J) {
+        return P(F, t, X, J)
     }
 
-    function k(z, H, J) {
-        return P(z, r, H, J)
+    function D(F, X, J) {
+        return P(F, r, X, J)
     }
 
-    function C(z, H, J) {
-        return P(z, n, H, J)
+    function C(F, X, J) {
+        return P(F, n, X, J)
     }
 
-    function L(z) {
-        return o[z.getDay()]
+    function L(F) {
+        return o[F.getDay()]
     }
 
-    function R(z) {
-        return a[z.getDay()]
+    function B(F) {
+        return a[F.getDay()]
     }
 
-    function F(z) {
-        return c[z.getMonth()]
+    function W(F) {
+        return c[F.getMonth()]
     }
 
-    function q(z) {
-        return u[z.getMonth()]
+    function q(F) {
+        return u[F.getMonth()]
     }
 
-    function Z(z) {
-        return i[+(z.getHours() >= 12)]
+    function Z(F) {
+        return i[+(F.getHours() >= 12)]
     }
 
-    function U(z) {
-        return 1 + ~~(z.getMonth() / 3)
+    function U(F) {
+        return 1 + ~~(F.getMonth() / 3)
     }
 
-    function ee(z) {
-        return o[z.getUTCDay()]
+    function Q(F) {
+        return o[F.getUTCDay()]
     }
 
-    function Te(z) {
-        return a[z.getUTCDay()]
+    function _e(F) {
+        return a[F.getUTCDay()]
     }
 
-    function Ee(z) {
-        return c[z.getUTCMonth()]
+    function ke(F) {
+        return c[F.getUTCMonth()]
     }
 
-    function Kt(z) {
-        return u[z.getUTCMonth()]
+    function Kt(F) {
+        return u[F.getUTCMonth()]
     }
 
-    function yt(z) {
-        return i[+(z.getUTCHours() >= 12)]
+    function De(F) {
+        return i[+(F.getUTCHours() >= 12)]
     }
 
-    function Ke(z) {
-        return 1 + ~~(z.getUTCMonth() / 3)
+    function yt(F) {
+        return 1 + ~~(F.getUTCMonth() / 3)
     }
     return {
-        format: function(z) {
-            var H = O(z += "", x);
-            return H.toString = function() {
-                return z
-            }, H
+        format: function(F) {
+            var X = O(F += "", x);
+            return X.toString = function() {
+                return F
+            }, X
         },
-        parse: function(z) {
-            var H = A(z += "", !1);
-            return H.toString = function() {
-                return z
-            }, H
+        parse: function(F) {
+            var X = A(F += "", !1);
+            return X.toString = function() {
+                return F
+            }, X
         },
-        utcFormat: function(z) {
-            var H = O(z += "", m);
-            return H.toString = function() {
-                return z
-            }, H
+        utcFormat: function(F) {
+            var X = O(F += "", m);
+            return X.toString = function() {
+                return F
+            }, X
         },
-        utcParse: function(z) {
-            var H = A(z += "", !0);
-            return H.toString = function() {
-                return z
-            }, H
+        utcParse: function(F) {
+            var X = A(F += "", !0);
+            return X.toString = function() {
+                return F
+            }, X
         }
     }
 }
 var jf = {
         "-": "",
         _: " ",
         0: "0"
@@ -7805,28 +7805,28 @@
 function Bf(e) {
     return +e
 }
 
 function Rf(e) {
     return Math.floor(+e / 1e3)
 }
-var vr, wv, Ov;
+var yr, wv, Ov;
 QM({
     dateTime: "%x, %X",
     date: "%-m/%-d/%Y",
     time: "%-I:%M:%S %p",
     periods: ["AM", "PM"],
     days: ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"],
     shortDays: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
     months: ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"],
     shortMonths: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
 });
 
 function QM(e) {
-    return vr = Qj(e), wv = vr.format, vr.parse, Ov = vr.utcFormat, vr.utcParse, vr
+    return yr = Qj(e), wv = yr.format, yr.parse, Ov = yr.utcFormat, yr.utcParse, yr
 }
 
 function eC(e) {
     return new Date(e)
 }
 
 function tC(e) {
@@ -7873,15 +7873,15 @@
 function nC() {
     return Qe.apply(ls(Vj, Yj, $t, ss, uo, ao, us, as, Qt, Ov).domain([Date.UTC(2e3, 0, 1), Date.UTC(2e3, 0, 2)]), arguments)
 }
 
 function co() {
     var e = 0,
         t = 1,
-        r, n, i, a, o = ke,
+        r, n, i, a, o = Ie,
         u = !1,
         c;
 
     function s(l) {
         return l == null || isNaN(l = +l) ? c : o(i === 0 ? .5 : (l = (a(l) - r) * i, u ? Math.max(0, Math.min(1, l)) : l))
     }
     s.domain = function(l) {
@@ -7907,15 +7907,15 @@
 }
 
 function Wt(e, t) {
     return t.domain(e.domain()).interpolator(e.interpolator()).clamp(e.clamp()).unknown(e.unknown())
 }
 
 function Av() {
-    var e = zt(co()(ke));
+    var e = zt(co()(Ie));
     return e.copy = function() {
         return Wt(e, Av())
     }, jt.apply(e, arguments)
 }
 
 function Sv() {
     var e = Qc(co()).domain([1, 10]);
@@ -7940,15 +7940,15 @@
 
 function iC() {
     return fs.apply(null, arguments).exponent(.5)
 }
 
 function _v() {
     var e = [],
-        t = ke;
+        t = Ie;
 
     function r(n) {
         if (n != null && !isNaN(n = +n)) return t((mi(e, n, 1) - 1) / (e.length - 1))
     }
     return r.domain = function(n) {
         if (!arguments.length) return e.slice();
         e = [];
@@ -7968,15 +7968,15 @@
 }
 
 function so() {
     var e = 0,
         t = .5,
         r = 1,
         n = 1,
-        i, a, o, u, c, s = ke,
+        i, a, o, u, c, s = Ie,
         f, l = !1,
         h;
 
     function p(v) {
         return isNaN(v = +v) ? h : (v = .5 + ((v = +f(v)) - a) * (n * v < n * a ? u : c), s(l ? Math.max(0, Math.min(1, v)) : v))
     }
     p.domain = function(v) {
@@ -7998,15 +7998,15 @@
         },
         function(v) {
             return f = v, i = v(e), a = v(t), o = v(r), u = i === a ? 0 : .5 / (a - i), c = a === o ? 0 : .5 / (o - a), n = a < i ? -1 : 1, p
         }
 }
 
 function $v() {
-    var e = zt(so()(ke));
+    var e = zt(so()(Ie));
     return e.copy = function() {
         return Wt(e, $v())
     }, jt.apply(e, arguments)
 }
 
 function Tv() {
     var e = Qc(so()).domain([.1, 1, 10]);
@@ -8104,15 +8104,15 @@
     return e && e.length ? mC(e, bC, gC) : void 0
 }
 var wC = xC;
 const lo = se(wC);
 var OC = Tc,
     AC = Ft,
     SC = Rd,
-    PC = Le;
+    PC = Be;
 
 function _C(e, t) {
     var r = PC(e) ? OC : SC;
     return r(e, AC(t))
 }
 var $C = _C,
     TC = Ld,
@@ -8125,15 +8125,15 @@
 const CC = se(MC);
 var IC = Fc;
 
 function kC(e, t) {
     return IC(e, t)
 }
 var DC = kC;
-const ar = se(DC);
+const or = se(DC);
 var Qr = 1e9,
     NC = {
         precision: 20,
         rounding: 4,
         toExpNeg: -7,
         toExpPos: 21,
         LN10: "2.302585092994045684017991454684364207601101488628772976033327900967572609677352480235997205089598298341967784042286"
@@ -8141,122 +8141,122 @@
     ds, he = !0,
     Je = "[DecimalError] ",
     nr = Je + "Invalid argument: ",
     ps = Je + "Exponent out of range: ",
     en = Math.floor,
     Yt = Math.pow,
     LC = /^(\d+(\.\d*)?|\.\d+)(e[+-]?\d+)?$/i,
-    We, Ae = 1e7,
+    Ue, Ae = 1e7,
     fe = 7,
     Mv = 9007199254740991,
     pa = en(Mv / fe),
-    W = {};
-W.absoluteValue = W.abs = function() {
+    z = {};
+z.absoluteValue = z.abs = function() {
     var e = new this.constructor(this);
     return e.s && (e.s = 1), e
 };
-W.comparedTo = W.cmp = function(e) {
+z.comparedTo = z.cmp = function(e) {
     var t, r, n, i, a = this;
     if (e = new a.constructor(e), a.s !== e.s) return a.s || -e.s;
     if (a.e !== e.e) return a.e > e.e ^ a.s < 0 ? 1 : -1;
     for (n = a.d.length, i = e.d.length, t = 0, r = n < i ? n : i; t < r; ++t)
         if (a.d[t] !== e.d[t]) return a.d[t] > e.d[t] ^ a.s < 0 ? 1 : -1;
     return n === i ? 0 : n > i ^ a.s < 0 ? 1 : -1
 };
-W.decimalPlaces = W.dp = function() {
+z.decimalPlaces = z.dp = function() {
     var e = this,
         t = e.d.length - 1,
         r = (t - e.e) * fe;
     if (t = e.d[t], t)
         for (; t % 10 == 0; t /= 10) r--;
     return r < 0 ? 0 : r
 };
-W.dividedBy = W.div = function(e) {
+z.dividedBy = z.div = function(e) {
     return St(this, new this.constructor(e))
 };
-W.dividedToIntegerBy = W.idiv = function(e) {
+z.dividedToIntegerBy = z.idiv = function(e) {
     var t = this,
         r = t.constructor;
     return ue(St(t, new r(e), 0, 1), r.precision)
 };
-W.equals = W.eq = function(e) {
+z.equals = z.eq = function(e) {
     return !this.cmp(e)
 };
-W.exponent = function() {
+z.exponent = function() {
     return ye(this)
 };
-W.greaterThan = W.gt = function(e) {
+z.greaterThan = z.gt = function(e) {
     return this.cmp(e) > 0
 };
-W.greaterThanOrEqualTo = W.gte = function(e) {
+z.greaterThanOrEqualTo = z.gte = function(e) {
     return this.cmp(e) >= 0
 };
-W.isInteger = W.isint = function() {
+z.isInteger = z.isint = function() {
     return this.e > this.d.length - 2
 };
-W.isNegative = W.isneg = function() {
+z.isNegative = z.isneg = function() {
     return this.s < 0
 };
-W.isPositive = W.ispos = function() {
+z.isPositive = z.ispos = function() {
     return this.s > 0
 };
-W.isZero = function() {
+z.isZero = function() {
     return this.s === 0
 };
-W.lessThan = W.lt = function(e) {
+z.lessThan = z.lt = function(e) {
     return this.cmp(e) < 0
 };
-W.lessThanOrEqualTo = W.lte = function(e) {
+z.lessThanOrEqualTo = z.lte = function(e) {
     return this.cmp(e) < 1
 };
-W.logarithm = W.log = function(e) {
+z.logarithm = z.log = function(e) {
     var t, r = this,
         n = r.constructor,
         i = n.precision,
         a = i + 5;
     if (e === void 0) e = new n(10);
-    else if (e = new n(e), e.s < 1 || e.eq(We)) throw Error(Je + "NaN");
+    else if (e = new n(e), e.s < 1 || e.eq(Ue)) throw Error(Je + "NaN");
     if (r.s < 1) throw Error(Je + (r.s ? "NaN" : "-Infinity"));
-    return r.eq(We) ? new n(0) : (he = !1, t = St(Wn(r, a), Wn(e, a), a), he = !0, ue(t, i))
+    return r.eq(Ue) ? new n(0) : (he = !1, t = St(Wn(r, a), Wn(e, a), a), he = !0, ue(t, i))
 };
-W.minus = W.sub = function(e) {
+z.minus = z.sub = function(e) {
     var t = this;
     return e = new t.constructor(e), t.s == e.s ? kv(t, e) : Cv(t, (e.s = -e.s, e))
 };
-W.modulo = W.mod = function(e) {
+z.modulo = z.mod = function(e) {
     var t, r = this,
         n = r.constructor,
         i = n.precision;
     if (e = new n(e), !e.s) throw Error(Je + "NaN");
     return r.s ? (he = !1, t = St(r, e, 0, 1).times(e), he = !0, r.minus(t)) : ue(new n(r), i)
 };
-W.naturalExponential = W.exp = function() {
+z.naturalExponential = z.exp = function() {
     return Iv(this)
 };
-W.naturalLogarithm = W.ln = function() {
+z.naturalLogarithm = z.ln = function() {
     return Wn(this)
 };
-W.negated = W.neg = function() {
+z.negated = z.neg = function() {
     var e = new this.constructor(this);
     return e.s = -e.s || 0, e
 };
-W.plus = W.add = function(e) {
+z.plus = z.add = function(e) {
     var t = this;
     return e = new t.constructor(e), t.s == e.s ? Cv(t, e) : kv(t, (e.s = -e.s, e))
 };
-W.precision = W.sd = function(e) {
+z.precision = z.sd = function(e) {
     var t, r, n, i = this;
     if (e !== void 0 && e !== !!e && e !== 1 && e !== 0) throw Error(nr + e);
     if (t = ye(i) + 1, n = i.d.length - 1, r = n * fe + 1, n = i.d[n], n) {
         for (; n % 10 == 0; n /= 10) r--;
         for (n = i.d[0]; n >= 10; n /= 10) r++
     }
     return e && t > r ? t : r
 };
-W.squareRoot = W.sqrt = function() {
+z.squareRoot = z.sqrt = function() {
     var e, t, r, n, i, a, o, u = this,
         c = u.constructor;
     if (u.s < 1) {
         if (!u.s) return new c(0);
         throw Error(Je + "NaN")
     }
     for (e = ye(u), he = !1, i = Math.sqrt(+u), i == 0 || i == 1 / 0 ? (t = st(u.d), (t.length + e) % 2 == 0 && (t += "0"), i = Math.sqrt(t), e = en((e + 1) / 2) - (e < 0 || e % 2), i == 1 / 0 ? t = "5e" + e : (t = i.toExponential(), t = t.slice(0, t.indexOf("e") + 1) + e), n = new c(t)) : n = new c(i.toString()), r = c.precision, i = o = r + 3;;)
@@ -8266,86 +8266,86 @@
                     n = a;
                     break
                 }
             } else if (t != "9999") break;
             o += 4
         } return he = !0, ue(n, r)
 };
-W.times = W.mul = function(e) {
+z.times = z.mul = function(e) {
     var t, r, n, i, a, o, u, c, s, f = this,
         l = f.constructor,
         h = f.d,
         p = (e = new l(e)).d;
     if (!f.s || !e.s) return new l(0);
     for (e.s *= f.s, r = f.e + e.e, c = h.length, s = p.length, c < s && (a = h, h = p, p = a, o = c, c = s, s = o), a = [], o = c + s, n = o; n--;) a.push(0);
     for (n = s; --n >= 0;) {
         for (t = 0, i = c + n; i > n;) u = a[i] + p[n] * h[i - n - 1] + t, a[i--] = u % Ae | 0, t = u / Ae | 0;
         a[i] = (a[i] + t) % Ae | 0
     }
     for (; !a[--o];) a.pop();
     return t ? ++r : a.shift(), e.d = a, e.e = r, he ? ue(e, l.precision) : e
 };
-W.toDecimalPlaces = W.todp = function(e, t) {
+z.toDecimalPlaces = z.todp = function(e, t) {
     var r = this,
         n = r.constructor;
     return r = new n(r), e === void 0 ? r : (dt(e, 0, Qr), t === void 0 ? t = n.rounding : dt(t, 0, 8), ue(r, e + ye(r) + 1, t))
 };
-W.toExponential = function(e, t) {
+z.toExponential = function(e, t) {
     var r, n = this,
         i = n.constructor;
-    return e === void 0 ? r = or(n, !0) : (dt(e, 0, Qr), t === void 0 ? t = i.rounding : dt(t, 0, 8), n = ue(new i(n), e + 1, t), r = or(n, !0, e + 1)), r
+    return e === void 0 ? r = ur(n, !0) : (dt(e, 0, Qr), t === void 0 ? t = i.rounding : dt(t, 0, 8), n = ue(new i(n), e + 1, t), r = ur(n, !0, e + 1)), r
 };
-W.toFixed = function(e, t) {
+z.toFixed = function(e, t) {
     var r, n, i = this,
         a = i.constructor;
-    return e === void 0 ? or(i) : (dt(e, 0, Qr), t === void 0 ? t = a.rounding : dt(t, 0, 8), n = ue(new a(i), e + ye(i) + 1, t), r = or(n.abs(), !1, e + ye(n) + 1), i.isneg() && !i.isZero() ? "-" + r : r)
+    return e === void 0 ? ur(i) : (dt(e, 0, Qr), t === void 0 ? t = a.rounding : dt(t, 0, 8), n = ue(new a(i), e + ye(i) + 1, t), r = ur(n.abs(), !1, e + ye(n) + 1), i.isneg() && !i.isZero() ? "-" + r : r)
 };
-W.toInteger = W.toint = function() {
+z.toInteger = z.toint = function() {
     var e = this,
         t = e.constructor;
     return ue(new t(e), ye(e) + 1, t.rounding)
 };
-W.toNumber = function() {
+z.toNumber = function() {
     return +this
 };
-W.toPower = W.pow = function(e) {
+z.toPower = z.pow = function(e) {
     var t, r, n, i, a, o, u = this,
         c = u.constructor,
         s = 12,
         f = +(e = new c(e));
-    if (!e.s) return new c(We);
+    if (!e.s) return new c(Ue);
     if (u = new c(u), !u.s) {
         if (e.s < 1) throw Error(Je + "Infinity");
         return u
     }
-    if (u.eq(We)) return u;
-    if (n = c.precision, e.eq(We)) return ue(u, n);
+    if (u.eq(Ue)) return u;
+    if (n = c.precision, e.eq(Ue)) return ue(u, n);
     if (t = e.e, r = e.d.length - 1, o = t >= r, a = u.s, o) {
         if ((r = f < 0 ? -f : f) <= Mv) {
-            for (i = new c(We), t = Math.ceil(n / fe + 4), he = !1; r % 2 && (i = i.times(u), Wf(i.d, t)), r = en(r / 2), r !== 0;) u = u.times(u), Wf(u.d, t);
-            return he = !0, e.s < 0 ? new c(We).div(i) : ue(i, n)
+            for (i = new c(Ue), t = Math.ceil(n / fe + 4), he = !1; r % 2 && (i = i.times(u), Wf(i.d, t)), r = en(r / 2), r !== 0;) u = u.times(u), Wf(u.d, t);
+            return he = !0, e.s < 0 ? new c(Ue).div(i) : ue(i, n)
         }
     } else if (a < 0) throw Error(Je + "NaN");
     return a = a < 0 && e.d[Math.max(t, r)] & 1 ? -1 : 1, u.s = 1, he = !1, i = e.times(Wn(u, n + s)), he = !0, i = Iv(i), i.s = a, i
 };
-W.toPrecision = function(e, t) {
+z.toPrecision = function(e, t) {
     var r, n, i = this,
         a = i.constructor;
-    return e === void 0 ? (r = ye(i), n = or(i, r <= a.toExpNeg || r >= a.toExpPos)) : (dt(e, 1, Qr), t === void 0 ? t = a.rounding : dt(t, 0, 8), i = ue(new a(i), e, t), r = ye(i), n = or(i, e <= r || r <= a.toExpNeg, e)), n
+    return e === void 0 ? (r = ye(i), n = ur(i, r <= a.toExpNeg || r >= a.toExpPos)) : (dt(e, 1, Qr), t === void 0 ? t = a.rounding : dt(t, 0, 8), i = ue(new a(i), e, t), r = ye(i), n = ur(i, e <= r || r <= a.toExpNeg, e)), n
 };
-W.toSignificantDigits = W.tosd = function(e, t) {
+z.toSignificantDigits = z.tosd = function(e, t) {
     var r = this,
         n = r.constructor;
     return e === void 0 ? (e = n.precision, t = n.rounding) : (dt(e, 1, Qr), t === void 0 ? t = n.rounding : dt(t, 0, 8)), ue(new n(r), e, t)
 };
-W.toString = W.valueOf = W.val = W.toJSON = W[Symbol.for("nodejs.util.inspect.custom")] = function() {
+z.toString = z.valueOf = z.val = z.toJSON = z[Symbol.for("nodejs.util.inspect.custom")] = function() {
     var e = this,
         t = ye(e),
         r = e.constructor;
-    return or(e, t <= r.toExpNeg || t >= r.toExpPos)
+    return ur(e, t <= r.toExpNeg || t >= r.toExpPos)
 };
 
 function Cv(e, t) {
     var r, n, i, a, o, u, c, s, f = e.constructor,
         l = f.precision;
     if (!e.s || !t.s) return t.s || (t = new f(e)), he ? ue(t, l) : t;
     if (c = e.d, s = t.d, o = e.e, i = t.e, c = c.slice(), a = o - i, a) {
@@ -8392,22 +8392,22 @@
     }
 
     function r(n, i, a) {
         for (var o = 0; a--;) n[a] -= o, o = n[a] < i[a] ? 1 : 0, n[a] = o * Ae + n[a] - i[a];
         for (; !n[0] && n.length > 1;) n.shift()
     }
     return function(n, i, a, o) {
-        var u, c, s, f, l, h, p, y, v, d, w, b, x, m, g, O, A, P, T = n.constructor,
-            E = n.s == i.s ? 1 : -1,
+        var u, c, s, f, l, h, p, y, v, d, w, b, x, m, g, O, A, P, E = n.constructor,
+            T = n.s == i.s ? 1 : -1,
             $ = n.d,
             _ = i.d;
-        if (!n.s) return new T(n);
+        if (!n.s) return new E(n);
         if (!i.s) throw Error(Je + "Division by zero");
-        for (c = n.e - i.e, A = _.length, g = $.length, p = new T(E), y = p.d = [], s = 0; _[s] == ($[s] || 0);) ++s;
-        if (_[s] > ($[s] || 0) && --c, a == null ? b = a = T.precision : o ? b = a + (ye(n) - ye(i)) + 1 : b = a, b < 0) return new T(0);
+        for (c = n.e - i.e, A = _.length, g = $.length, p = new E(T), y = p.d = [], s = 0; _[s] == ($[s] || 0);) ++s;
+        if (_[s] > ($[s] || 0) && --c, a == null ? b = a = E.precision : o ? b = a + (ye(n) - ye(i)) + 1 : b = a, b < 0) return new E(0);
         if (b = b / fe + 2 | 0, s = 0, A == 1)
             for (f = 0, _ = _[0], b++;
                 (s < g || f) && b--; s++) x = f * Ae + ($[s] || 0), y[s] = x / _ | 0, f = x % _ | 0;
         else {
             for (f = Ae / (_[0] + 1) | 0, f > 1 && (_ = e(_, f), $ = e($, f), A = _.length, g = $.length), m = A, v = $.slice(0, A), d = v.length; d < A;) v[d++] = 0;
             P = _.slice(), P.unshift(0), O = _[0], _[1] >= Ae / 2 && ++O;
             do f = 0, u = t(_, v, A, d), u < 0 ? (w = v[0], A != d && (w = w * Ae + (v[1] || 0)), f = w / O | 0, f > 1 ? (f >= Ae && (f = Ae - 1), l = e(_, f), h = l.length, d = v.length, u = t(l, v, h, d), u == 1 && (f--, r(l, A < h ? P : _, h))) : (f == 0 && (u = f = 1), l = _.slice()), h = l.length, h < d && l.unshift(0), r(v, l, d), u == -1 && (d = v.length, u = t(_, v, A, d), u < 1 && (f++, r(v, A < d ? P : _, d))), d = v.length) : u === 0 && (f++, v = [0]), y[s++] = f, u && v[0] ? v[d++] = $[m] || 0 : (v = [$[m]], d = 1); while ((m++ < g || v[0] !== void 0) && b--)
@@ -8418,17 +8418,17 @@
 
 function Iv(e, t) {
     var r, n, i, a, o, u, c = 0,
         s = 0,
         f = e.constructor,
         l = f.precision;
     if (ye(e) > 16) throw Error(ps + ye(e));
-    if (!e.s) return new f(We);
+    if (!e.s) return new f(Ue);
     for (t == null ? (he = !1, u = l) : u = t, o = new f(.03125); e.abs().gte(.1);) e = e.times(o), s += 5;
-    for (n = Math.log(Yt(2, s)) / Math.LN10 * 2 + 5 | 0, u += n, r = i = a = new f(We), f.precision = u;;) {
+    for (n = Math.log(Yt(2, s)) / Math.LN10 * 2 + 5 | 0, u += n, r = i = a = new f(Ue), f.precision = u;;) {
         if (i = ue(i.times(e), u), r = r.times(++c), o = a.plus(St(i, r, u)), st(o.d).slice(0, u) === st(a.d).slice(0, u)) {
             for (; s--;) a = ue(a.times(a), u);
             return f.precision = l, t == null ? (he = !0, ue(a, l)) : a
         }
         a = o
     }
 }
@@ -8452,21 +8452,21 @@
     var r, n, i, a, o, u, c, s, f, l = 1,
         h = 10,
         p = e,
         y = p.d,
         v = p.constructor,
         d = v.precision;
     if (p.s < 1) throw Error(Je + (p.s ? "NaN" : "-Infinity"));
-    if (p.eq(We)) return new v(0);
+    if (p.eq(Ue)) return new v(0);
     if (t == null ? (he = !1, s = d) : s = t, p.eq(10)) return t == null && (he = !0), Wo(v, s);
     if (s += h, v.precision = s, r = st(y), n = r.charAt(0), a = ye(p), Math.abs(a) < 15e14) {
         for (; n < 7 && n != 1 || n == 1 && r.charAt(1) > 3;) p = p.times(e), r = st(p.d), n = r.charAt(0), l++;
         a = ye(p), n > 1 ? (p = new v("0." + r), a++) : p = new v(n + "." + r.slice(1))
     } else return c = Wo(v, s + 2, d).times(a + ""), p = Wn(new v(n + "." + r.slice(1)), s - h).plus(c), v.precision = d, t == null ? (he = !0, ue(p, d)) : p;
-    for (u = o = p = St(p.minus(We), p.plus(We), s), f = ue(p.times(p), s), i = 3;;) {
+    for (u = o = p = St(p.minus(Ue), p.plus(Ue), s), f = ue(p.times(p), s), i = 3;;) {
         if (o = ue(o.times(f), s), c = u.plus(St(o, new v(i), s)), st(c.d).slice(0, s) === st(u.d).slice(0, s)) return u = u.times(2), a !== 0 && (u = u.plus(Wo(v, s + 2, d).times(a + ""))), u = St(u, new v(l), s), v.precision = d, t == null ? (he = !0, ue(u, d)) : u;
         u = c, i += 2
     }
 }
 
 function zf(e, t) {
     var r, n, i;
@@ -8529,15 +8529,15 @@
         c[i] -= l[i]
     }
     for (; c[--u] === 0;) c.pop();
     for (; c[0] === 0; c.shift()) --n;
     return c[0] ? (t.d = c, t.e = n, he ? ue(t, p) : t) : new h(0)
 }
 
-function or(e, t, r) {
+function ur(e, t, r) {
     var n, i = ye(e),
         a = st(e.d),
         o = a.length;
     return t ? (r && (n = r - o) > 0 ? a = a.charAt(0) + "." + a.slice(1) + It(n) : o > 1 && (a = a.charAt(0) + "." + a.slice(1)), a = a + (i < 0 ? "e" : "e+") + i) : i < 0 ? (a = "0." + It(-i - 1) + a, r && (n = r - o) > 0 && (a += It(n))) : i >= o ? (a += It(i + 1 - o), r && (n = r - i - 1) > 0 && (a = a + "." + It(n))) : ((n = i + 1) < o && (a = a.slice(0, n) + "." + a.slice(n)), r && (n = r - o) > 0 && (i + 1 === o && (a += "."), a += It(n))), e.s < 0 ? "-" + a : a
 }
 
 function Wf(e, t) {
@@ -8567,15 +8567,15 @@
                 return
             }
             return zf(o, a.toString())
         } else if (typeof a != "string") throw Error(nr + a);
         if (a.charCodeAt(0) === 45 ? (a = a.slice(1), o.s = -1) : o.s = 1, LC.test(a)) zf(o, a);
         else throw Error(nr + a)
     }
-    if (i.prototype = W, i.ROUND_UP = 0, i.ROUND_DOWN = 1, i.ROUND_CEIL = 2, i.ROUND_FLOOR = 3, i.ROUND_HALF_UP = 4, i.ROUND_HALF_DOWN = 5, i.ROUND_HALF_EVEN = 6, i.ROUND_HALF_CEIL = 7, i.ROUND_HALF_FLOOR = 8, i.clone = Dv, i.config = i.set = BC, e === void 0 && (e = {}), e)
+    if (i.prototype = z, i.ROUND_UP = 0, i.ROUND_DOWN = 1, i.ROUND_CEIL = 2, i.ROUND_FLOOR = 3, i.ROUND_HALF_UP = 4, i.ROUND_HALF_DOWN = 5, i.ROUND_HALF_EVEN = 6, i.ROUND_HALF_CEIL = 7, i.ROUND_HALF_FLOOR = 8, i.clone = Dv, i.config = i.set = BC, e === void 0 && (e = {}), e)
         for (n = ["precision", "rounding", "toExpNeg", "toExpPos", "LN10"], t = 0; t < n.length;) e.hasOwnProperty(r = n[t++]) || (e[r] = this[r]);
     return i.config(e), i
 }
 
 function BC(e) {
     if (!e || typeof e != "object") throw Error(Je + "Object expected");
     var t, r, n, i = ["precision", 1, Qr, "rounding", 0, 8, "toExpNeg", -1 / 0, 0, "toExpPos", 0, 1 / 0];
@@ -8585,15 +8585,15 @@
             else throw Error(nr + r + ": " + n);
     if ((n = e[r = "LN10"]) !== void 0)
         if (n == Math.LN10) this[r] = new this(n);
         else throw Error(nr + r + ": " + n);
     return this
 }
 var ds = Dv(NC);
-We = new ds(1);
+Ue = new ds(1);
 const oe = ds;
 
 function RC(e) {
     return UC(e) || WC(e) || zC(e) || FC()
 }
 
 function FC() {
@@ -8884,15 +8884,15 @@
         h = [].concat(Du(ho.rangeStep(new oe(c), new oe(s).sub(new oe(.99).mul(l)), l)), [s]);
     return n > i ? ku(h) : h
 }
 var cI = Bv(oI),
     sI = Bv(uI),
     lI = "Invariant failed";
 
-function ur(e, t) {
+function cr(e, t) {
     if (!e) throw new Error(lI)
 }
 var fI = ["offset", "layout", "width", "dataKey", "data", "dataPointFormatter", "xAxis", "yAxis"];
 
 function da() {
     return da = Object.assign ? Object.assign.bind() : function(e) {
         for (var t = 1; t < arguments.length; t++) {
@@ -8982,16 +8982,16 @@
         n = e.width,
         i = e.dataKey,
         a = e.data,
         o = e.dataPointFormatter,
         u = e.xAxis,
         c = e.yAxis,
         s = mI(e, fI),
-        f = G(s, !1);
-    e.direction === "x" && u.type !== "number" && ur(!1);
+        f = H(s, !1);
+    e.direction === "x" && u.type !== "number" && cr(!1);
     var l = a.map(function(h) {
         var p = o(h, i),
             y = p.x,
             v = p.y,
             d = p.value,
             w = p.errorVal;
         if (!w) return null;
@@ -9001,65 +9001,65 @@
             var g = hI(w, 2);
             x = g[0], m = g[1]
         } else x = m = w;
         if (r === "vertical") {
             var O = u.scale,
                 A = v + t,
                 P = A + n,
-                T = A - n,
-                E = O(d - x),
+                E = A - n,
+                T = O(d - x),
                 $ = O(d + m);
             b.push({
                 x1: $,
                 y1: P,
                 x2: $,
-                y2: T
+                y2: E
             }), b.push({
-                x1: E,
+                x1: T,
                 y1: A,
                 x2: $,
                 y2: A
             }), b.push({
-                x1: E,
+                x1: T,
                 y1: P,
-                x2: E,
-                y2: T
+                x2: T,
+                y2: E
             })
         } else if (r === "horizontal") {
             var _ = c.scale,
                 M = y + t,
                 j = M - n,
-                k = M + n,
+                D = M + n,
                 C = _(d - x),
                 L = _(d + m);
             b.push({
                 x1: j,
                 y1: L,
-                x2: k,
+                x2: D,
                 y2: L
             }), b.push({
                 x1: M,
                 y1: C,
                 x2: M,
                 y2: L
             }), b.push({
                 x1: j,
                 y1: C,
-                x2: k,
+                x2: D,
                 y2: C
             })
         }
         return S.createElement(ie, da({
             className: "recharts-errorBar",
-            key: "bar-".concat(b.map(function(R) {
-                return "".concat(R.x1, "-").concat(R.x2, "-").concat(R.y1, "-").concat(R.y2)
+            key: "bar-".concat(b.map(function(B) {
+                return "".concat(B.x1, "-").concat(B.x2, "-").concat(B.y1, "-").concat(B.y2)
             }))
-        }, f), b.map(function(R) {
-            return S.createElement("line", da({}, R, {
-                key: "line-".concat(R.x1, "-").concat(R.x2, "-").concat(R.y1, "-").concat(R.y2)
+        }, f), b.map(function(B) {
+            return S.createElement("line", da({}, B, {
+                key: "line-".concat(B.x1, "-").concat(B.x2, "-").concat(B.y1, "-").concat(B.y2)
             }))
         }))
     });
     return S.createElement(ie, {
         className: "recharts-errorBars"
     }, l)
 }
@@ -9129,15 +9129,15 @@
     return (t === "string" ? String : Number)(e)
 }
 var Uv = function(t) {
     var r = t.children,
         n = t.formattedGraphicalItems,
         i = t.legendWidth,
         a = t.legendContent,
-        o = ze(r, Mn);
+        o = We(r, Mn);
     if (!o) return null;
     var u;
     return o.props && o.props.payload ? u = o.props && o.props.payload : a === "children" ? u = (n || []).reduce(function(c, s) {
         var f = s.item,
             l = s.props,
             h = l.sectors || l.data || [];
         return c.concat(h.map(function(p) {
@@ -9189,23 +9189,23 @@
     return r
 }
 
 function Ve(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? Hf(Object(r), !0).forEach(function(n) {
-            Or(e, n, r[n])
+            Ar(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : Hf(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
     }
     return e
 }
 
-function Or(e, t, r) {
+function Ar(e, t, r) {
     return t = OI(t), t in e ? Object.defineProperty(e, t, {
         value: r,
         enumerable: !0,
         configurable: !0,
         writable: !0
     }) : e[t] = r, e
 }
@@ -9255,29 +9255,29 @@
 function Lu(e, t) {
     (t == null || t > e.length) && (t = e.length);
     for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
     return n
 }
 
 function xe(e, t, r) {
-    return X(e) || X(t) ? r : be(t) ? Ze(e, t, r) : Y(t) ? t(e) : r
+    return G(e) || G(t) ? r : be(t) ? Ze(e, t, r) : Y(t) ? t(e) : r
 }
 
 function On(e, t, r, n) {
     var i = CC(e, function(u) {
         return xe(u, t)
     });
     if (r === "number") {
         var a = i.filter(function(u) {
             return N(u) || parseFloat(u)
         });
         return a.length ? [lo(a), Dt(a)] : [1 / 0, -1 / 0]
     }
     var o = n ? i.filter(function(u) {
-        return !X(u)
+        return !G(u)
     }) : i;
     return o.map(function(u) {
         return be(u) || u instanceof Date ? u : ""
     })
 }
 var TI = function(t) {
         var r, n = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : [],
@@ -9342,47 +9342,50 @@
                 u = o;
                 break
         }
         return u
     },
     EI = function(t) {
         var r = t.barSize,
-            n = t.stackGroups,
-            i = n === void 0 ? {} : n;
-        if (!i) return {};
-        for (var a = {}, o = Object.keys(i), u = 0, c = o.length; u < c; u++)
-            for (var s = i[o[u]].stackGroups, f = Object.keys(s), l = 0, h = f.length; l < h; l++) {
-                var p = s[f[l]],
-                    y = p.items,
-                    v = p.cateAxisId,
-                    d = y.filter(function(x) {
-                        return Ot(x.type).indexOf("Bar") >= 0
+            n = t.totalSize,
+            i = t.stackGroups,
+            a = i === void 0 ? {} : i;
+        if (!a) return {};
+        for (var o = {}, u = Object.keys(a), c = 0, s = u.length; c < s; c++)
+            for (var f = a[u[c]].stackGroups, l = Object.keys(f), h = 0, p = l.length; h < p; h++) {
+                var y = f[l[h]],
+                    v = y.items,
+                    d = y.cateAxisId,
+                    w = v.filter(function(g) {
+                        return Ot(g.type).indexOf("Bar") >= 0
                     });
-                if (d && d.length) {
-                    var w = d[0].props.barSize,
-                        b = d[0].props[v];
-                    a[b] || (a[b] = []), a[b].push({
-                        item: d[0],
-                        stackList: d.slice(1),
-                        barSize: X(w) ? r : w
+                if (w && w.length) {
+                    var b = w[0].props.barSize,
+                        x = w[0].props[d];
+                    o[x] || (o[x] = []);
+                    var m = G(b) ? r : b;
+                    o[x].push({
+                        item: w[0],
+                        stackList: w.slice(1),
+                        barSize: G(m) ? void 0 : ar(m, n, 0)
                     })
                 }
             }
-        return a
+        return o
     },
     jI = function(t) {
         var r = t.barGap,
             n = t.barCategoryGap,
             i = t.bandSize,
             a = t.sizeList,
             o = a === void 0 ? [] : a,
             u = t.maxBarSize,
             c = o.length;
         if (c < 1) return null;
-        var s = Ar(r, i, 0, !0),
+        var s = ar(r, i, 0, !0),
             f, l = [];
         if (o[0].barSize === +o[0].barSize) {
             var h = !1,
                 p = i / c,
                 y = o.reduce(function(m, g) {
                     return m + g.barSize || 0
                 }, 0);
@@ -9405,15 +9408,15 @@
                     A.push({
                         item: P,
                         position: d
                     })
                 }), A
             }, l)
         } else {
-            var w = Ar(n, i, 0, !0);
+            var w = ar(n, i, 0, !0);
             i - 2 * w - (c - 1) * s <= 0 && (s = 0);
             var b = (i - 2 * w - (c - 1) * s) / c;
             b > 1 && (b >>= 0);
             var x = u === +u ? Math.min(b, u) : b;
             f = o.reduce(function(m, g, O) {
                 var A = [].concat(Gf(m), [{
                     item: g.item,
@@ -9444,34 +9447,34 @@
         if (s) {
             var f = i || {},
                 l = f.width,
                 h = f.height,
                 p = s.align,
                 y = s.verticalAlign,
                 v = s.layout;
-            if ((v === "vertical" || v === "horizontal" && y === "middle") && p !== "center" && N(t[p])) return Ve(Ve({}, t), {}, Or({}, p, t[p] + (l || 0)));
-            if ((v === "horizontal" || v === "vertical" && p === "center") && y !== "middle" && N(t[y])) return Ve(Ve({}, t), {}, Or({}, y, t[y] + (h || 0)))
+            if ((v === "vertical" || v === "horizontal" && y === "middle") && p !== "center" && N(t[p])) return Ve(Ve({}, t), {}, Ar({}, p, t[p] + (l || 0)));
+            if ((v === "horizontal" || v === "vertical" && p === "center") && y !== "middle" && N(t[y])) return Ve(Ve({}, t), {}, Ar({}, y, t[y] + (h || 0)))
         }
         return t
     },
     CI = function(t, r, n) {
-        return X(r) ? !0 : t === "horizontal" ? r === "yAxis" : t === "vertical" || n === "x" ? r === "xAxis" : n === "y" ? r === "yAxis" : !0
+        return G(r) ? !0 : t === "horizontal" ? r === "yAxis" : t === "vertical" || n === "x" ? r === "xAxis" : n === "y" ? r === "yAxis" : !0
     },
     Kv = function(t, r, n, i, a) {
         var o = r.props.children,
-            u = Ne(o, tn).filter(function(s) {
+            u = Le(o, tn).filter(function(s) {
                 return CI(i, a, s.props.direction)
             });
         if (u && u.length) {
             var c = u.map(function(s) {
                 return s.props.dataKey
             });
             return t.reduce(function(s, f) {
                 var l = xe(f, n);
-                if (X(l)) return s;
+                if (G(l)) return s;
                 var h = Array.isArray(l) ? [lo(l), Dt(l)] : [l, l],
                     p = c.reduce(function(y, v) {
                         var d = xe(f, v, 0),
                             w = h[0] - Math.abs(Array.isArray(d) ? d[0] : d),
                             b = h[1] + Math.abs(Array.isArray(d) ? d[1] : d);
                         return [Math.min(w, y[0]), Math.max(b, y[1])]
                     }, [1 / 0, -1 / 0]);
@@ -9480,15 +9483,15 @@
         }
         return null
     },
     II = function(t, r, n, i, a) {
         var o = r.map(function(u) {
             return Kv(t, u, n, a, i)
         }).filter(function(u) {
-            return !X(u)
+            return !G(u)
         });
         return o && o.length ? o.reduce(function(u, c) {
             return [Math.min(u[0], c[0]), Math.max(u[1], c[1])]
         }, [1 / 0, -1 / 0]) : null
     },
     qv = function(t, r, n, i, a) {
         var o = r.map(function(c) {
@@ -9684,37 +9687,37 @@
                 if (be(y)) {
                     var b = w.stackGroups[y] || {
                         numericAxisId: n,
                         cateAxisId: i,
                         items: []
                     };
                     b.items.push(h), w.hasStack = !0, w.stackGroups[y] = b
-                } else w.stackGroups[lr("_stackId_")] = {
+                } else w.stackGroups[fr("_stackId_")] = {
                     numericAxisId: n,
                     cateAxisId: i,
                     items: [h]
                 };
-                return Ve(Ve({}, l), {}, Or({}, d, w))
+                return Ve(Ve({}, l), {}, Ar({}, d, w))
             }, c),
             f = {};
         return Object.keys(s).reduce(function(l, h) {
             var p = s[h];
             if (p.hasStack) {
                 var y = {};
                 p.stackGroups = Object.keys(p.stackGroups).reduce(function(v, d) {
                     var w = p.stackGroups[d];
-                    return Ve(Ve({}, v), {}, Or({}, d, {
+                    return Ve(Ve({}, v), {}, Ar({}, d, {
                         numericAxisId: n,
                         cateAxisId: i,
                         items: w.items,
                         stackedData: zI(t, w.items, a)
                     }))
                 }, y)
             }
-            return Ve(Ve({}, l), {}, Or({}, h, p))
+            return Ve(Ve({}, l), {}, Ar({}, h, p))
         }, f)
     },
     UI = function(t, r) {
         var n = r.realScaleType,
             i = r.type,
             a = r.tickCount,
             o = r.originalDomain,
@@ -9743,33 +9746,33 @@
     var t = e.axis,
         r = e.ticks,
         n = e.bandSize,
         i = e.entry,
         a = e.index,
         o = e.dataKey;
     if (t.type === "category") {
-        if (!t.allowDuplicatedCategory && t.dataKey && !X(i[t.dataKey])) {
+        if (!t.allowDuplicatedCategory && t.dataKey && !G(i[t.dataKey])) {
             var u = zi(r, "value", i[t.dataKey]);
             if (u) return u.coordinate + n / 2
         }
         return r[a] ? r[a].coordinate + n / 2 : null
     }
-    var c = xe(i, X(o) ? t.dataKey : o);
-    return X(c) ? null : t.scale(c)
+    var c = xe(i, G(o) ? t.dataKey : o);
+    return G(c) ? null : t.scale(c)
 }
 var Vf = function(t) {
         var r = t.axis,
             n = t.ticks,
             i = t.offset,
             a = t.bandSize,
             o = t.entry,
             u = t.index;
         if (r.type === "category") return n[u] ? n[u].coordinate + i : null;
         var c = xe(o, r.dataKey, r.domain[u]);
-        return X(c) ? null : r.scale(c) - a / 2 + i
+        return G(c) ? null : r.scale(c) - a / 2 + i
     },
     KI = function(t) {
         var r = t.numericAxis,
             n = r.scale.domain();
         if (r.type === "number") {
             var i = Math.min(n[0], n[1]),
                 a = Math.max(n[0], n[1]);
@@ -9838,26 +9841,26 @@
                 o = Math.min((s.coordinate || 0) - (f.coordinate || 0), o)
             }
             return o === 1 / 0 ? 0 : o
         }
         return n ? void 0 : 0
     },
     Jf = function(t, r, n) {
-        return !t || !t.length || ar(t, Ze(n, "type.defaultProps.domain")) ? r : t
+        return !t || !t.length || or(t, Ze(n, "type.defaultProps.domain")) ? r : t
     },
     Vv = function(t, r) {
         var n = t.props,
             i = n.dataKey,
             a = n.name,
             o = n.unit,
             u = n.formatter,
             c = n.tooltipType,
             s = n.chartType,
             f = n.hide;
-        return Ve(Ve({}, G(t, !1)), {}, {
+        return Ve(Ve({}, H(t, !1)), {}, {
             dataKey: i,
             unit: o,
             formatter: u,
             name: a || i,
             color: vs(t),
             value: xe(r, i),
             type: c,
@@ -9923,15 +9926,15 @@
     }
     return (t === "string" ? String : Number)(e)
 }
 var ya = Math.PI / 180,
     YI = function(t) {
         return t * 180 / Math.PI
     },
-    $e = function(t, r, n, i) {
+    Te = function(t, r, n, i) {
         return {
             x: t + Math.cos(-ya * i) * n,
             y: r + Math.sin(-ya * i) * n
         }
     },
     ZI = function(t, r) {
         var n = t.x,
@@ -10133,15 +10136,15 @@
         }
         return e
     }, Xn.apply(this, arguments)
 }
 var hk = function(t) {
         var r = t.value,
             n = t.formatter,
-            i = X(t.children) ? r : t.children;
+            i = G(t.children) ? r : t.children;
         return Y(n) ? n(i) : i
     },
     pk = function(t, r) {
         var n = it(r - t),
             i = Math.min(Math.abs(r - t), 360);
         return n * i
     },
@@ -10159,23 +10162,23 @@
             y = c.endAngle,
             v = c.clockWise,
             d = (l + h) / 2,
             w = pk(p, y),
             b = w >= 0 ? 1 : -1,
             x, m;
         i === "insideStart" ? (x = p + b * o, m = v) : i === "insideEnd" ? (x = y - b * o, m = !v) : i === "end" && (x = y + b * o, m = v), m = w <= 0 ? m : !m;
-        var g = $e(s, f, d, x),
-            O = $e(s, f, d, x + (m ? 1 : -1) * 359),
+        var g = Te(s, f, d, x),
+            O = Te(s, f, d, x + (m ? 1 : -1) * 359),
             A = "M".concat(g.x, ",").concat(g.y, `
     A`).concat(d, ",").concat(d, ",0,1,").concat(m ? 0 : 1, `,
     `).concat(O.x, ",").concat(O.y),
-            P = X(t.id) ? lr("recharts-radial-line-") : t.id;
+            P = G(t.id) ? fr("recharts-radial-line-") : t.id;
         return S.createElement("text", Xn({}, n, {
             dominantBaseline: "central",
-            className: re("recharts-radial-bar-label", u)
+            className: ee("recharts-radial-bar-label", u)
         }), S.createElement("defs", null, S.createElement("path", {
             id: P,
             d: A
         })), S.createElement("textPath", {
             xlinkHref: "#".concat(P)
         }, r))
     },
@@ -10188,15 +10191,15 @@
             u = a.cy,
             c = a.innerRadius,
             s = a.outerRadius,
             f = a.startAngle,
             l = a.endAngle,
             h = (f + l) / 2;
         if (i === "outside") {
-            var p = $e(o, u, s + n, h),
+            var p = Te(o, u, s + n, h),
                 y = p.x,
                 v = p.y;
             return {
                 x: y,
                 y: v,
                 textAnchor: y >= o ? "start" : "end",
                 verticalAnchor: "middle"
@@ -10217,15 +10220,15 @@
         if (i === "centerBottom") return {
             x: o,
             y: u,
             textAnchor: "middle",
             verticalAnchor: "end"
         };
         var d = (c + s) / 2,
-            w = $e(o, u, d, h),
+            w = Te(o, u, d, h),
             b = w.x,
             x = w.y;
         return {
             x: b,
             y: x,
             textAnchor: "middle",
             verticalAnchor: "middle"
@@ -10338,61 +10341,61 @@
             verticalAnchor: p
         }, A) : a === "insideBottomRight" ? ge({
             x: u + s - d,
             y: c + f - h,
             textAnchor: w,
             verticalAnchor: p
         }, A) : Kr(a) && (N(a.x) || Zt(a.x)) && (N(a.y) || Zt(a.y)) ? ge({
-            x: u + Ar(a.x, s),
-            y: c + Ar(a.y, f),
+            x: u + ar(a.x, s),
+            y: c + ar(a.y, f),
             textAnchor: "end",
             verticalAnchor: "end"
         }, A) : ge({
             x: u + s / 2,
             y: c + f / 2,
             textAnchor: "middle",
             verticalAnchor: "middle"
         }, A)
     },
     mk = function(t) {
         return "cx" in t && N(t.cx)
     };
 
-function Me(e) {
+function je(e) {
     var t = e.offset,
         r = t === void 0 ? 5 : t,
         n = uk(e, tk),
         i = ge({
             offset: r
         }, n),
         a = i.viewBox,
         o = i.position,
         u = i.value,
         c = i.children,
         s = i.content,
         f = i.className,
         l = f === void 0 ? "" : f,
         h = i.textBreakAll;
-    if (!a || X(u) && X(c) && !B.isValidElement(s) && !Y(s)) return null;
-    if (B.isValidElement(s)) return B.cloneElement(s, i);
+    if (!a || G(u) && G(c) && !R.isValidElement(s) && !Y(s)) return null;
+    if (R.isValidElement(s)) return R.cloneElement(s, i);
     var p;
     if (Y(s)) {
-        if (p = B.createElement(s, i), B.isValidElement(p)) return p
+        if (p = R.createElement(s, i), R.isValidElement(p)) return p
     } else p = hk(i);
     var y = mk(a),
-        v = G(i, !0);
+        v = H(i, !0);
     if (y && (o === "insideStart" || o === "insideEnd" || o === "end")) return dk(i, p, v);
     var d = y ? vk(i) : yk(i);
     return S.createElement(ra, Xn({
-        className: re("recharts-label", l)
+        className: ee("recharts-label", l)
     }, v, d, {
         breakAll: h
     }), p)
 }
-Me.displayName = "Label";
+je.displayName = "Label";
 var Yv = function(t) {
         var r = t.cx,
             n = t.cy,
             i = t.angle,
             a = t.startAngle,
             o = t.endAngle,
             u = t.r,
@@ -10434,55 +10437,55 @@
             endAngle: o || i || 0,
             innerRadius: s || 0,
             outerRadius: f || c || u || 0,
             clockWise: w
         } : t.viewBox ? t.viewBox : {}
     },
     gk = function(t, r) {
-        return t ? t === !0 ? S.createElement(Me, {
+        return t ? t === !0 ? S.createElement(je, {
             key: "label-implicit",
             viewBox: r
-        }) : be(t) ? S.createElement(Me, {
+        }) : be(t) ? S.createElement(je, {
             key: "label-implicit",
             viewBox: r,
             value: t
-        }) : B.isValidElement(t) ? t.type === Me ? B.cloneElement(t, {
+        }) : R.isValidElement(t) ? t.type === je ? R.cloneElement(t, {
             key: "label-implicit",
             viewBox: r
-        }) : S.createElement(Me, {
+        }) : S.createElement(je, {
             key: "label-implicit",
             content: t,
             viewBox: r
-        }) : Y(t) ? S.createElement(Me, {
+        }) : Y(t) ? S.createElement(je, {
             key: "label-implicit",
             content: t,
             viewBox: r
-        }) : Kr(t) ? S.createElement(Me, Xn({
+        }) : Kr(t) ? S.createElement(je, Xn({
             viewBox: r
         }, t, {
             key: "label-implicit"
         })) : null : null
     },
     bk = function(t, r) {
         var n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !0;
         if (!t || !t.children && n && !t.label) return null;
         var i = t.children,
             a = Yv(t),
-            o = Ne(i, Me).map(function(c, s) {
-                return B.cloneElement(c, {
+            o = Le(i, je).map(function(c, s) {
+                return R.cloneElement(c, {
                     viewBox: r || a,
                     key: "label-".concat(s)
                 })
             });
         if (!n) return o;
         var u = gk(t.label, r || a);
         return [u].concat(rk(o))
     };
-Me.parseViewBox = Yv;
-Me.renderCallByParent = bk;
+je.parseViewBox = Yv;
+je.renderCallByParent = bk;
 
 function xk(e) {
     var t = e == null ? 0 : e.length;
     return t ? e[t - 1] : void 0
 }
 var wk = xk;
 const Ok = se(wk);
@@ -10620,23 +10623,23 @@
         o = n.clockWise,
         u = n.id,
         c = n.textBreakAll,
         s = ah(n, Sk);
     return !i || !i.length ? null : S.createElement(ie, {
         className: "recharts-label-list"
     }, i.map(function(f, l) {
-        var h = X(a) ? r(f, l) : xe(f && f.payload, a),
-            p = X(u) ? {} : {
+        var h = G(a) ? r(f, l) : xe(f && f.payload, a),
+            p = G(u) ? {} : {
                 id: "".concat(u, "-").concat(l)
             };
-        return S.createElement(Me, ma({}, G(f, !0), s, p, {
+        return S.createElement(je, ma({}, H(f, !0), s, p, {
             parentViewBox: f.parentViewBox,
             value: h,
             textBreakAll: c,
-            viewBox: Me.parseViewBox(X(o) ? f : ih(ih({}, f), {}, {
+            viewBox: je.parseViewBox(G(o) ? f : ih(ih({}, f), {}, {
                 clockWise: o
             })),
             key: "label-".concat(l),
             index: l
         }))
     }))
 }
@@ -10657,16 +10660,16 @@
     })) : null : null
 }
 
 function Nk(e, t) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !0;
     if (!e || !e.children && r && !e.label) return null;
     var n = e.children,
-        i = Ne(n, ht).map(function(o, u) {
-            return B.cloneElement(o, {
+        i = Le(n, ht).map(function(o, u) {
+            return R.cloneElement(o, {
                 data: t,
                 key: "labelList-".concat(u)
             })
         });
     if (!r) return i;
     var a = Dk(e.label, t);
     return [a].concat(Pk(i))
@@ -10752,18 +10755,18 @@
             o = t.sign,
             u = t.isExternal,
             c = t.cornerRadius,
             s = t.cornerIsExternal,
             f = c * (u ? 1 : -1) + i,
             l = Math.asin(c / f) / ya,
             h = s ? a : a + o * l,
-            p = $e(r, n, f, h),
-            y = $e(r, n, i, h),
+            p = Te(r, n, f, h),
+            y = Te(r, n, i, h),
             v = s ? a - o * l : a,
-            d = $e(r, n, f * Math.cos(l * ya), v);
+            d = Te(r, n, f * Math.cos(l * ya), v);
         return {
             center: p,
             circleTangency: y,
             lineTangency: d,
             theta: l
         }
     },
@@ -10772,24 +10775,24 @@
             n = t.cy,
             i = t.innerRadius,
             a = t.outerRadius,
             o = t.startAngle,
             u = t.endAngle,
             c = Fk(o, u),
             s = o + c,
-            f = $e(r, n, a, o),
-            l = $e(r, n, a, s),
+            f = Te(r, n, a, o),
+            l = Te(r, n, a, s),
             h = "M ".concat(f.x, ",").concat(f.y, `
     A `).concat(a, ",").concat(a, `,0,
     `).concat(+(Math.abs(c) > 180), ",").concat(+(o > s), `,
     `).concat(l.x, ",").concat(l.y, `
   `);
         if (i > 0) {
-            var p = $e(r, n, i, o),
-                y = $e(r, n, i, s);
+            var p = Te(r, n, i, o),
+                y = Te(r, n, i, s);
             h += "L ".concat(y.x, ",").concat(y.y, `
             A `).concat(i, ",").concat(i, `,0,
             `).concat(+(Math.abs(c) > 180), ",").concat(+(o <= s), `,
             `).concat(p.x, ",").concat(p.y, " Z")
         } else h += "L ".concat(r, ",").concat(n, " Z");
         return h
     },
@@ -10854,29 +10857,29 @@
                     sign: l,
                     isExternal: !0,
                     cornerRadius: o,
                     cornerIsExternal: c
                 }),
                 A = O.circleTangency,
                 P = O.lineTangency,
-                T = O.theta,
-                E = ki({
+                E = O.theta,
+                T = ki({
                     cx: r,
                     cy: n,
                     radius: i,
                     angle: f,
                     sign: -l,
                     isExternal: !0,
                     cornerRadius: o,
                     cornerIsExternal: c
                 }),
-                $ = E.circleTangency,
-                _ = E.lineTangency,
-                M = E.theta,
-                j = c ? Math.abs(s - f) : Math.abs(s - f) - T - M;
+                $ = T.circleTangency,
+                _ = T.lineTangency,
+                M = T.theta,
+                j = c ? Math.abs(s - f) : Math.abs(s - f) - E - M;
             if (j < 0 && o === 0) return "".concat(g, "L").concat(r, ",").concat(n, "Z");
             g += "L".concat(_.x, ",").concat(_.y, `
       A`).concat(o, ",").concat(o, ",0,0,").concat(+(l < 0), ",").concat($.x, ",").concat($.y, `
       A`).concat(i, ",").concat(i, ",0,").concat(+(j > 180), ",").concat(+(l > 0), ",").concat(A.x, ",").concat(A.y, `
       A`).concat(o, ",").concat(o, ",0,0,").concat(+(l < 0), ",").concat(P.x, ",").concat(P.y, "Z")
         } else g += "L".concat(r, ",").concat(n, "Z");
         return g
@@ -10901,17 +10904,17 @@
             u = r.cornerRadius,
             c = r.forceCornerRadius,
             s = r.cornerIsExternal,
             f = r.startAngle,
             l = r.endAngle,
             h = r.className;
         if (o < a || f === l) return null;
-        var p = re("recharts-sector", h),
+        var p = ee("recharts-sector", h),
             y = o - a,
-            v = Ar(u, y, 0, !0),
+            v = ar(u, y, 0, !0),
             d;
         return v > 0 && Math.abs(f - l) < 360 ? d = zk({
             cx: n,
             cy: i,
             innerRadius: a,
             outerRadius: o,
             cornerRadius: Math.min(v, y / 2),
@@ -10922,15 +10925,15 @@
         }) : d = Zv({
             cx: n,
             cy: i,
             innerRadius: a,
             outerRadius: o,
             startAngle: f,
             endAngle: l
-        }), S.createElement("path", zu({}, G(r, !0), {
+        }), S.createElement("path", zu({}, H(r, !0), {
             className: p,
             d,
             role: "img"
         }))
     };
 
 function Zn(e) {
@@ -11062,16 +11065,16 @@
     ir = function(t) {
         var r = t.className,
             n = t.points,
             i = t.path,
             a = t.pathRef;
         if ((!n || !n.length) && !i) return null;
         var o = n && n.length ? Gk(t) : i;
-        return S.createElement("path", Wu({}, G(t, !1), Wi(t), {
-            className: re("recharts-curve", r),
+        return S.createElement("path", Wu({}, H(t, !1), Wi(t), {
+            className: ee("recharts-curve", r),
             d: o,
             ref: a
         }))
     },
     Qv = {
         exports: {}
     },
@@ -11794,15 +11797,15 @@
         t && (n = n.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function _e(e) {
+function $e(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? $h(Object(r), !0).forEach(function(n) {
             qu(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : $h(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
@@ -11898,35 +11901,35 @@
     rD = function e(t, r, n) {
         var i = An(function(a, o) {
             if (Gu(o)) {
                 var u = t(o.from, o.to, o.velocity),
                     c = J2(u, 2),
                     s = c[0],
                     f = c[1];
-                return _e(_e({}, o), {}, {
+                return $e($e({}, o), {}, {
                     from: s,
                     velocity: f
                 })
             }
             return o
         }, r);
         return n < 1 ? An(function(a, o) {
-            return Gu(o) ? _e(_e({}, o), {}, {
+            return Gu(o) ? $e($e({}, o), {}, {
                 velocity: ba(o.velocity, i[a].velocity, n),
                 from: ba(o.from, i[a].from, n)
             }) : o
         }, r) : e(t, i, n - 1)
     };
 const nD = function(e, t, r, n, i) {
     var a = I2(e, t),
         o = a.reduce(function(d, w) {
-            return _e(_e({}, d), {}, qu({}, w, [e[w], t[w]]))
+            return $e($e({}, d), {}, qu({}, w, [e[w], t[w]]))
         }, {}),
         u = a.reduce(function(d, w) {
-            return _e(_e({}, d), {}, qu({}, w, {
+            return $e($e({}, d), {}, qu({}, w, {
                 from: e[w],
                 velocity: 0,
                 to: t[w]
             }))
         }, {}),
         c = -1,
         s, f, l = function() {
@@ -11940,28 +11943,28 @@
         p = function() {
             return !Object.values(u).filter(Gu).length
         },
         y = function(w) {
             s || (s = w);
             var b = w - s,
                 x = b / r.dt;
-            u = rD(r, u, x), i(_e(_e(_e({}, e), t), h())), s = w, p() || (c = requestAnimationFrame(l))
+            u = rD(r, u, x), i($e($e($e({}, e), t), h())), s = w, p() || (c = requestAnimationFrame(l))
         },
         v = function(w) {
             f || (f = w);
             var b = (w - f) / n,
                 x = An(function(g, O) {
                     return ba.apply(void 0, _h(O).concat([r(b)]))
                 }, o);
-            if (i(_e(_e(_e({}, e), t), x)), b < 1) c = requestAnimationFrame(l);
+            if (i($e($e($e({}, e), t), x)), b < 1) c = requestAnimationFrame(l);
             else {
                 var m = An(function(g, O) {
                     return ba.apply(void 0, _h(O).concat([r(1)]))
                 }, o);
-                i(_e(_e(_e({}, e), t), m))
+                i($e($e($e({}, e), t), m))
             }
         };
     return l = r.isStepper ? y : v,
         function() {
             return requestAnimationFrame(l),
                 function() {
                     cancelAnimationFrame(c)
@@ -12285,24 +12288,24 @@
                     var b = d.duration,
                         x = d.easing,
                         m = x === void 0 ? "ease" : x,
                         g = d.style,
                         O = d.properties,
                         A = d.onAnimationEnd,
                         P = w > 0 ? o[w - 1] : d,
-                        T = O || Object.keys(g);
+                        E = O || Object.keys(g);
                     if (typeof m == "function" || m === "spring") return [].concat(qo(v), [a.runJSAnimation.bind(a, {
                         from: P.style,
                         to: g,
                         duration: b,
                         easing: m
                     }), b]);
-                    var E = Ah(T, b, m),
+                    var T = Ah(E, b, m),
                         $ = et(et(et({}, P.style), g), {}, {
-                            transition: E
+                            transition: T
                         });
                     return [].concat(qo(v), [$, b, A]).filter(k2)
                 };
             return this.manager.start([c].concat(qo(o.reduce(p, [f, Math.max(h, u)])), [i.onAnimationEnd]))
         }
     }, {
         key: "runAnimation",
@@ -12339,35 +12342,35 @@
                 a = i.children;
             i.begin;
             var o = i.duration;
             i.attributeName, i.easing;
             var u = i.isActive;
             i.steps, i.from, i.to, i.canBegin, i.onAnimationEnd, i.shouldReAnimate, i.onAnimationReStart;
             var c = aD(i, iD),
-                s = B.Children.count(a),
+                s = R.Children.count(a),
                 f = this.state.style;
             if (typeof a == "function") return a(f);
             if (!u || s === 0 || o <= 0) return a;
             var l = function(p) {
                 var y = p.props,
                     v = y.style,
                     d = v === void 0 ? {} : v,
                     w = y.className,
-                    b = B.cloneElement(p, et(et({}, c), {}, {
+                    b = R.cloneElement(p, et(et({}, c), {}, {
                         style: et(et({}, d), f),
                         className: w
                     }));
                 return b
             };
-            return s === 1 ? l(B.Children.only(a)) : S.createElement("div", null, B.Children.map(a, function(h) {
+            return s === 1 ? l(R.Children.only(a)) : S.createElement("div", null, R.Children.map(a, function(h) {
                 return l(h)
             }))
         }
     }]), r
-}(B.PureComponent);
+}(R.PureComponent);
 ot.displayName = "Animate";
 ot.defaultProps = {
     begin: 0,
     duration: 1e3,
     from: "",
     to: "",
     attributeName: "",
@@ -12397,15 +12400,15 @@
     canBegin: V.bool,
     onAnimationEnd: V.func,
     shouldReAnimate: V.bool,
     onAnimationStart: V.func,
     onAnimationReStart: V.func
 };
 
-function HF(e, t) {
+function GF(e, t) {
     if (e == null) return {};
     var r = {},
         n = Object.keys(e),
         i, a;
     for (a = 0; a < n.length; a++) i = n[a], !(t.indexOf(i) >= 0) && (r[i] = e[i]);
     return r
 }
@@ -12583,20 +12586,20 @@
         isUpdateAnimationActive: !1,
         animationBegin: 0,
         animationDuration: 1500,
         animationEasing: "ease"
     },
     ys = function(t) {
         var r = Ch(Ch({}, _D), t),
-            n = B.useRef(),
-            i = B.useState(-1),
+            n = R.useRef(),
+            i = R.useState(-1),
             a = mD(i, 2),
             o = a[0],
             u = a[1];
-        B.useEffect(function() {
+        R.useEffect(function() {
             if (n.current && n.current.getTotalLength) try {
                 var m = n.current.getTotalLength();
                 m && u(m)
             } catch {}
         }, []);
         var c = r.x,
             s = r.y,
@@ -12606,15 +12609,15 @@
             p = r.className,
             y = r.animationEasing,
             v = r.animationDuration,
             d = r.animationBegin,
             w = r.isAnimationActive,
             b = r.isUpdateAnimationActive;
         if (c !== +c || s !== +s || f !== +f || l !== +l || f === 0 || l === 0) return null;
-        var x = re("recharts-rectangle", p);
+        var x = ee("recharts-rectangle", p);
         return b ? S.createElement(ot, {
             canBegin: o > 0,
             from: {
                 width: f,
                 height: l,
                 x: c,
                 y: s
@@ -12638,20 +12641,20 @@
                 from: "0px ".concat(o === -1 ? 1 : o, "px"),
                 to: "".concat(o, "px 0px"),
                 attributeName: "strokeDasharray",
                 begin: d,
                 duration: v,
                 isActive: w,
                 easing: y
-            }, S.createElement("path", wa({}, G(r, !0), {
+            }, S.createElement("path", wa({}, H(r, !0), {
                 className: x,
                 d: Ih(A, P, g, O, h),
                 ref: n
             })))
-        }) : S.createElement("path", wa({}, G(r, !0), {
+        }) : S.createElement("path", wa({}, H(r, !0), {
             className: x,
             d: Ih(c, s, f, l, h)
         }))
     };
 
 function Ju() {
     return Ju = Object.assign ? Object.assign.bind() : function(e) {
@@ -12663,16 +12666,16 @@
     }, Ju.apply(this, arguments)
 }
 var po = function(t) {
     var r = t.cx,
         n = t.cy,
         i = t.r,
         a = t.className,
-        o = re("recharts-dot", a);
-    return r === +r && n === +n && i === +i ? S.createElement("circle", Ju({}, G(t, !1), Wi(t), {
+        o = ee("recharts-dot", a);
+    return r === +r && n === +n && i === +i ? S.createElement("circle", Ju({}, H(t, !1), Wi(t), {
         className: o,
         cx: r,
         cy: n,
         r: i
     })) : null
 };
 
@@ -12785,16 +12788,16 @@
                 x: n,
                 y: a,
                 top: u,
                 left: s,
                 width: l,
                 height: p
             }, v);
-        return !N(n) || !N(a) || !N(l) || !N(p) || !N(u) || !N(s) ? null : S.createElement("path", Qu({}, G(d, !0), {
-            className: re("recharts-cross", y),
+        return !N(n) || !N(a) || !N(l) || !N(p) || !N(u) || !N(s) ? null : S.createElement("path", Qu({}, H(d, !0), {
+            className: ee("recharts-cross", y),
             d: kD(n, a, l, p, u, s)
         }))
     },
     ND = Pd,
     LD = ND(Object.getPrototypeOf, Object),
     BD = LD,
     RD = Tt,
@@ -12959,20 +12962,20 @@
         isUpdateAnimationActive: !1,
         animationBegin: 0,
         animationDuration: 1500,
         animationEasing: "ease"
     },
     fN = function(t) {
         var r = Lh(Lh({}, lN), t),
-            n = B.useRef(),
-            i = B.useState(-1),
+            n = R.useRef(),
+            i = R.useState(-1),
             a = rN(i, 2),
             o = a[0],
             u = a[1];
-        B.useEffect(function() {
+        R.useEffect(function() {
             if (n.current && n.current.getTotalLength) try {
                 var x = n.current.getTotalLength();
                 x && u(x)
             } catch {}
         }, []);
         var c = r.x,
             s = r.y,
@@ -12981,15 +12984,15 @@
             h = r.height,
             p = r.className,
             y = r.animationEasing,
             v = r.animationDuration,
             d = r.animationBegin,
             w = r.isUpdateAnimationActive;
         if (c !== +c || s !== +s || f !== +f || l !== +l || h !== +h || f === 0 && l === 0 || h === 0) return null;
-        var b = re("recharts-trapezoid", p);
+        var b = ee("recharts-trapezoid", p);
         return w ? S.createElement(ot, {
             canBegin: o > 0,
             from: {
                 upperWidth: 0,
                 lowerWidth: 0,
                 height: h,
                 x: c,
@@ -13015,20 +13018,20 @@
                 canBegin: o > 0,
                 from: "0px ".concat(o === -1 ? 1 : o, "px"),
                 to: "".concat(o, "px 0px"),
                 attributeName: "strokeDasharray",
                 begin: d,
                 duration: v,
                 easing: y
-            }, S.createElement("path", Oa({}, G(r, !0), {
+            }, S.createElement("path", Oa({}, H(r, !0), {
                 className: b,
                 d: Bh(A, P, m, g, O),
                 ref: n
             })))
-        }) : S.createElement("g", null, S.createElement("path", Oa({}, G(r, !0), {
+        }) : S.createElement("g", null, S.createElement("path", Oa({}, H(r, !0), {
             className: b,
             d: Bh(c, s, f, l, h)
         })))
     },
     hN = ["option", "shapeType", "propTransformer", "activeClassName", "isActive"];
 
 function ni(e) {
@@ -13131,28 +13134,28 @@
             break;
         default:
             return null
     }
 }
 
 function xN(e) {
-    return B.isValidElement(e) ? e.props : e
+    return R.isValidElement(e) ? e.props : e
 }
 
 function ec(e) {
     var t = e.option,
         r = e.shapeType,
         n = e.propTransformer,
         i = n === void 0 ? gN : n,
         a = e.activeClassName,
         o = a === void 0 ? "recharts-active-shape" : a,
         u = e.isActive,
         c = pN(e, hN),
         s;
-    if (B.isValidElement(t)) s = B.cloneElement(t, Aa(Aa({}, c), xN(t)));
+    if (R.isValidElement(t)) s = R.cloneElement(t, Aa(Aa({}, c), xN(t)));
     else if (Y(t)) s = t(c);
     else if (VD(t) && !tN(t)) {
         var f = i(t, c);
         s = S.createElement(Fh, {
             shapeType: r,
             elementProps: f
         })
@@ -13224,15 +13227,15 @@
 function $N(e) {
     var t = e.activeTooltipItem,
         r = e.graphicalItem,
         n = e.itemData,
         i = PN(r, t),
         a = _N(r, t),
         o = n.filter(function(c, s) {
-            var f = ar(a, c),
+            var f = or(a, c),
                 l = r.props[i].filter(function(y) {
                     var v = SN(r, t);
                     return v(y, t)
                 }),
                 h = r.props[i].indexOf(l[l.length - 1]),
                 p = s === h;
             return f && p
@@ -13374,15 +13377,15 @@
     return r
 }
 
 function Go(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? Kh(Object(r), !0).forEach(function(n) {
-            Fe(e, n, r[n])
+            ze(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : Kh(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
     }
     return e
 }
 
@@ -13448,15 +13451,15 @@
 
 function tc(e, t) {
     return tc = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(n, i) {
         return n.__proto__ = i, n
     }, tc(e, t)
 }
 
-function Fe(e, t, r) {
+function ze(e, t, r) {
     return t = dy(t), t in e ? Object.defineProperty(e, t, {
         value: r,
         enumerable: !0,
         configurable: !0,
         writable: !0
     }) : e[t] = r, e
 }
@@ -13504,43 +13507,43 @@
         return t.changedTouches && !!t.changedTouches.length
     },
     Dr = function(e) {
         YN(t, e);
 
         function t(r) {
             var n;
-            return HN(this, t), n = XN(this, t, [r]), Fe(ct(n), "handleDrag", function(i) {
+            return HN(this, t), n = XN(this, t, [r]), ze(ct(n), "handleDrag", function(i) {
                 n.leaveTimer && (clearTimeout(n.leaveTimer), n.leaveTimer = null), n.state.isTravellerMoving ? n.handleTravellerMove(i) : n.state.isSlideMoving && n.handleSlideDrag(i)
-            }), Fe(ct(n), "handleTouchMove", function(i) {
+            }), ze(ct(n), "handleTouchMove", function(i) {
                 i.changedTouches != null && i.changedTouches.length > 0 && n.handleDrag(i.changedTouches[0])
-            }), Fe(ct(n), "handleDragEnd", function() {
+            }), ze(ct(n), "handleDragEnd", function() {
                 n.setState({
                     isTravellerMoving: !1,
                     isSlideMoving: !1
                 }, function() {
                     var i = n.props,
                         a = i.endIndex,
                         o = i.onDragEnd,
                         u = i.startIndex;
                     o == null || o({
                         endIndex: a,
                         startIndex: u
                     })
                 }), n.detachDragEndListener()
-            }), Fe(ct(n), "handleLeaveWrapper", function() {
+            }), ze(ct(n), "handleLeaveWrapper", function() {
                 (n.state.isTravellerMoving || n.state.isSlideMoving) && (n.leaveTimer = window.setTimeout(n.handleDragEnd, n.props.leaveTimeOut))
-            }), Fe(ct(n), "handleEnterSlideOrTraveller", function() {
+            }), ze(ct(n), "handleEnterSlideOrTraveller", function() {
                 n.setState({
                     isTextActive: !0
                 })
-            }), Fe(ct(n), "handleLeaveSlideOrTraveller", function() {
+            }), ze(ct(n), "handleLeaveSlideOrTraveller", function() {
                 n.setState({
                     isTextActive: !1
                 })
-            }), Fe(ct(n), "handleSlideDragStart", function(i) {
+            }), ze(ct(n), "handleSlideDragStart", function(i) {
                 var a = Hh(i) ? i.changedTouches[0] : i;
                 n.setState({
                     isTravellerMoving: !1,
                     isSlideMoving: !0,
                     slideMoveStartX: a.pageX
                 }), n.attachDragEndListener()
             }), n.travellerDragStartHandlers = {
@@ -13654,15 +13657,15 @@
                 var x = this.getIndex(w),
                     m = x.startIndex,
                     g = x.endIndex,
                     O = function() {
                         var P = d.length - 1;
                         return o === "startX" && (u > c ? m % v === 0 : g % v === 0) || u < c && g === P || o === "endX" && (u > c ? g % v === 0 : m % v === 0) || u > c && g === P
                     };
-                this.setState(Fe(Fe({}, o, s + b), "brushMoveStartX", n.pageX), function() {
+                this.setState(ze(ze({}, o, s + b), "brushMoveStartX", n.pageX), function() {
                     y && O() && y(x)
                 })
             }
         }, {
             key: "handleTravellerMoveKeyboard",
             value: function(n, i) {
                 var a = this,
@@ -13672,15 +13675,15 @@
                     s = o.endX,
                     f = this.state[i],
                     l = u.indexOf(f);
                 if (l !== -1) {
                     var h = l + n;
                     if (!(h === -1 || h >= u.length)) {
                         var p = u[h];
-                        i === "startX" && p >= s || i === "endX" && p <= c || this.setState(Fe({}, i, p), function() {
+                        i === "startX" && p >= s || i === "endX" && p <= c || this.setState(ze({}, i, p), function() {
                             a.props.onChange(a.getIndex({
                                 startX: a.state.startX,
                                 endX: a.state.endX
                             }))
                         })
                     }
                 }
@@ -13711,15 +13714,15 @@
                     i = n.x,
                     a = n.y,
                     o = n.width,
                     u = n.height,
                     c = n.data,
                     s = n.children,
                     f = n.padding,
-                    l = B.Children.only(s);
+                    l = R.Children.only(s);
                 return l ? S.cloneElement(l, {
                     x: i,
                     y: a,
                     width: o,
                     height: u,
                     margin: f,
                     compact: !0,
@@ -13736,15 +13739,15 @@
                     s = o.height,
                     f = o.traveller,
                     l = o.ariaLabel,
                     h = o.data,
                     p = o.startIndex,
                     y = o.endIndex,
                     v = Math.max(n, this.props.x),
-                    d = Go(Go({}, G(this.props, !1)), {}, {
+                    d = Go(Go({}, H(this.props, !1)), {}, {
                         x: v,
                         y: u,
                         width: c,
                         height: s
                     }),
                     w = l || "Min value: ".concat(h[p].name, ", Max value: ").concat(h[y].name);
                 return S.createElement(ie, {
@@ -13851,15 +13854,15 @@
                     p = h.startX,
                     y = h.endX,
                     v = h.isTextActive,
                     d = h.isSlideMoving,
                     w = h.isTravellerMoving,
                     b = h.isTravellerFocused;
                 if (!i || !i.length || !N(u) || !N(c) || !N(s) || !N(f) || s <= 0 || f <= 0) return null;
-                var x = re("recharts-brush", a),
+                var x = ee("recharts-brush", a),
                     m = S.Children.count(o) === 1,
                     g = qN("userSelect", "none");
                 return S.createElement(ie, {
                     className: x,
                     onMouseLeave: this.handleLeaveWrapper,
                     onTouchMove: this.handleTouchMove,
                     style: g
@@ -13954,17 +13957,17 @@
                 for (var a = n.length, o = 0, u = a - 1; u - o > 1;) {
                     var c = Math.floor((o + u) / 2);
                     n[c] > i ? u = c : o = c
                 }
                 return i >= n[u] ? u : o
             }
         }]), t
-    }(B.PureComponent);
-Fe(Dr, "displayName", "Brush");
-Fe(Dr, "defaultProps", {
+    }(R.PureComponent);
+ze(Dr, "displayName", "Brush");
+ze(Dr, "defaultProps", {
     height: 40,
     travellerWidth: 5,
     gap: 1,
     fill: "#fff",
     stroke: "#666",
     padding: {
         top: 1,
@@ -13983,15 +13986,15 @@
         return r = t(n, i, a), !r
     }), !!r
 }
 var tL = eL,
     rL = md,
     nL = Ft,
     iL = tL,
-    aL = Le,
+    aL = Be,
     oL = no;
 
 function uL(e, t, r) {
     var n = aL(e) ? rL : iL;
     return r && oL(e, t, r) && (t = void 0), n(e, nL(t))
 }
 var cL = uL;
@@ -14039,15 +14042,15 @@
         return r = !!t(n, i, a), r
     }), r
 }
 var OL = wL,
     AL = bL,
     SL = OL,
     PL = Ft,
-    _L = Le,
+    _L = Be,
     $L = no;
 
 function TL(e, t, r) {
     var n = _L(e) ? AL : SL;
     return r && $L(e, t, r) && (t = void 0), n(e, PL(t))
 }
 var EL = TL;
@@ -14173,15 +14176,15 @@
     }, e))
 }
 var LL = function(t) {
         var r = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         return function(n, i) {
             if (typeof t == "number") return t;
             var a = typeof n == "number";
-            return a ? t(n, i) : (a || ur(!1), r)
+            return a ? t(n, i) : (a || cr(!1), r)
         }
     },
     BL = ["value", "background"],
     yy;
 
 function Nr(e) {
     "@babel/helpers - typeof";
@@ -14340,15 +14343,15 @@
 
     function t() {
         var r;
         zL(this, t);
         for (var n = arguments.length, i = new Array(n), a = 0; a < n; a++) i[a] = arguments[a];
         return r = UL(this, t, [].concat(i)), Nt(mn(r), "state", {
             isAnimationFinished: !1
-        }), Nt(mn(r), "id", lr("recharts-bar-")), Nt(mn(r), "handleAnimationEnd", function() {
+        }), Nt(mn(r), "id", fr("recharts-bar-")), Nt(mn(r), "handleAnimationEnd", function() {
             var o = r.props.onAnimationEnd;
             r.setState({
                 isAnimationFinished: !0
             }), o && o()
         }), Nt(mn(r), "handleAnimationStart", function() {
             var o = r.props.onAnimationStart;
             r.setState({
@@ -14361,15 +14364,15 @@
         value: function(n) {
             var i = this,
                 a = this.props,
                 o = a.shape,
                 u = a.dataKey,
                 c = a.activeIndex,
                 s = a.activeBar,
-                f = G(this.props, !1);
+                f = H(this.props, !1);
             return n && n.map(function(l, h) {
                 var p = h === c,
                     y = p ? s : o,
                     v = Oe(Oe(Oe({}, f), l), {}, {
                         isActive: p,
                         option: y,
                         index: h,
@@ -14431,41 +14434,41 @@
                             var A = de(0, d.height),
                                 P = A(y);
                             return Oe(Oe({}, d), {}, {
                                 y: d.y + d.height - P,
                                 height: P
                             })
                         }
-                        var T = de(0, d.width),
-                            E = T(y);
+                        var E = de(0, d.width),
+                            T = E(y);
                         return Oe(Oe({}, d), {}, {
-                            width: E
+                            width: T
                         })
                     });
                 return S.createElement(ie, null, n.renderRectanglesStatically(v))
             })
         }
     }, {
         key: "renderRectangles",
         value: function() {
             var n = this.props,
                 i = n.data,
                 a = n.isAnimationActive,
                 o = this.state.prevData;
-            return a && i && i.length && (!o || !ar(o, i)) ? this.renderRectanglesWithAnimation() : this.renderRectanglesStatically(i)
+            return a && i && i.length && (!o || !or(o, i)) ? this.renderRectanglesWithAnimation() : this.renderRectanglesStatically(i)
         }
     }, {
         key: "renderBackground",
         value: function() {
             var n = this,
                 i = this.props,
                 a = i.data,
                 o = i.dataKey,
                 u = i.activeIndex,
-                c = G(this.props.background, !1);
+                c = H(this.props.background, !1);
             return a.map(function(s, f) {
                 s.value;
                 var l = s.background,
                     h = RL(s, BL);
                 if (!l) return null;
                 var p = Oe(Oe(Oe(Oe(Oe({}, h), {}, {
                     fill: "#eee"
@@ -14489,15 +14492,15 @@
             if (this.props.isAnimationActive && !this.state.isAnimationFinished) return null;
             var a = this.props,
                 o = a.data,
                 u = a.xAxis,
                 c = a.yAxis,
                 s = a.layout,
                 f = a.children,
-                l = Ne(f, tn);
+                l = Le(f, tn);
             if (!l) return null;
             var h = s === "vertical" ? o[0].height / 2 : o[0].width / 2,
                 p = function(d, w) {
                     var b = Array.isArray(d.value) ? d.value[1] : d.value;
                     return {
                         x: d.x,
                         y: d.y,
@@ -14534,19 +14537,19 @@
                 l = n.width,
                 h = n.height,
                 p = n.isAnimationActive,
                 y = n.background,
                 v = n.id;
             if (i || !a || !a.length) return null;
             var d = this.state.isAnimationFinished,
-                w = re("recharts-bar", o),
+                w = ee("recharts-bar", o),
                 b = u && u.allowDataOverflow,
                 x = c && c.allowDataOverflow,
                 m = b || x,
-                g = X(v) ? this.id : v;
+                g = G(v) ? this.id : v;
             return S.createElement(ie, {
                 className: w
             }, b || x ? S.createElement("defs", null, S.createElement("clipPath", {
                 id: "clipPath-".concat(g)
             }, S.createElement("rect", {
                 x: b ? s : s - l / 2,
                 y: x ? f : f - h / 2,
@@ -14565,15 +14568,15 @@
                 curData: n.data,
                 prevData: i.curData
             } : n.data !== i.curData ? {
                 curData: n.data
             } : null
         }
     }]), t
-}(B.PureComponent);
+}(R.PureComponent);
 yy = nn;
 Nt(nn, "displayName", "Bar");
 Nt(nn, "defaultProps", {
     xAxisId: 0,
     yAxisId: 0,
     legendType: "rect",
     minPointSize: 0,
@@ -14607,71 +14610,71 @@
         w = v.children,
         b = v.minPointSize,
         x = y === "horizontal" ? o : a,
         m = s ? x.scale.domain() : null,
         g = KI({
             numericAxis: x
         }),
-        O = Ne(w, Kc),
-        A = l.map(function(P, T) {
-            var E, $, _, M, j, k;
-            s ? E = LI(s[f + T], m) : (E = xe(P, d), Array.isArray(E) || (E = [g, E]));
-            var C = LL(b, yy.defaultProps.minPointSize)(E[1], T);
+        O = Le(w, Kc),
+        A = l.map(function(P, E) {
+            var T, $, _, M, j, D;
+            s ? T = LI(s[f + E], m) : (T = xe(P, d), Array.isArray(T) || (T = [g, T]));
+            var C = LL(b, yy.defaultProps.minPointSize)(T[1], E);
             if (y === "horizontal") {
-                var L, R = [o.scale(E[0]), o.scale(E[1])],
-                    F = R[0],
-                    q = R[1];
+                var L, B = [o.scale(T[0]), o.scale(T[1])],
+                    W = B[0],
+                    q = B[1];
                 $ = Vf({
                     axis: a,
                     ticks: u,
                     bandSize: i,
                     offset: p.offset,
                     entry: P,
-                    index: T
-                }), _ = (L = q ?? F) !== null && L !== void 0 ? L : void 0, M = p.size;
-                var Z = F - q;
-                if (j = Number.isNaN(Z) ? 0 : Z, k = {
+                    index: E
+                }), _ = (L = q ?? W) !== null && L !== void 0 ? L : void 0, M = p.size;
+                var Z = W - q;
+                if (j = Number.isNaN(Z) ? 0 : Z, D = {
                         x: $,
                         y: o.y,
                         width: M,
                         height: o.height
                     }, Math.abs(C) > 0 && Math.abs(j) < Math.abs(C)) {
                     var U = it(j || C) * (Math.abs(C) - Math.abs(j));
                     _ -= U, j += U
                 }
             } else {
-                var ee = [a.scale(E[0]), a.scale(E[1])],
-                    Te = ee[0],
-                    Ee = ee[1];
-                if ($ = Te, _ = Vf({
+                var Q = [a.scale(T[0]), a.scale(T[1])],
+                    _e = Q[0],
+                    ke = Q[1];
+                if ($ = _e, _ = Vf({
                         axis: o,
                         ticks: c,
                         bandSize: i,
                         offset: p.offset,
                         entry: P,
-                        index: T
-                    }), M = Ee - Te, j = p.size, k = {
+                        index: E
+                    }), M = ke - _e, j = p.size, D = {
                         x: a.x,
                         y: _,
                         width: a.width,
                         height: j
                     }, Math.abs(C) > 0 && Math.abs(M) < Math.abs(C)) {
                     var Kt = it(M || C) * (Math.abs(C) - Math.abs(M));
                     M += Kt
                 }
             }
             return Oe(Oe(Oe({}, P), {}, {
                 x: $,
                 y: _,
                 width: M,
                 height: j,
-                value: s ? E : E[1],
+                value: s ? T : T[1],
                 payload: P,
-                background: k
-            }, O && O[T] && O[T].props), {}, {
+                background: D
+            }, O && O[E] && O[E].props), {}, {
                 tooltipPayload: [Vv(r, P)],
                 tooltipPosition: {
                     x: $ + M / 2,
                     y: _ + j / 2
                 }
             })
         });
@@ -14766,58 +14769,59 @@
                 right: o - n.right,
                 rightMirror: o - n.right,
                 top: n.top,
                 topMirror: n.top,
                 bottom: u - n.bottom,
                 bottomMirror: u - n.bottom
             },
-            h = !!ze(s, nn);
+            h = !!We(s, nn);
         return f.reduce(function(p, y) {
             var v = r[y],
                 d = v.orientation,
                 w = v.domain,
                 b = v.padding,
                 x = b === void 0 ? {} : b,
                 m = v.mirror,
                 g = v.reversed,
                 O = "".concat(d).concat(m ? "Mirror" : ""),
-                A, P, T, E, $;
+                A, P, E, T, $;
             if (v.type === "number" && (v.padding === "gap" || v.padding === "no-gap")) {
                 var _ = w[1] - w[0],
                     M = 1 / 0,
                     j = v.categoricalDomain.sort();
-                j.forEach(function(Te, Ee) {
-                    Ee > 0 && (M = Math.min((Te || 0) - (j[Ee - 1] || 0), M))
-                });
-                var k = M / _,
-                    C = v.layout === "vertical" ? n.height : n.width;
-                if (v.padding === "gap" && (A = k * C / 2), v.padding === "no-gap") {
-                    var L = Ar(t.barCategoryGap, k * C),
-                        R = k * C / 2;
-                    A = R - L - (R - L) / C * L
+                if (j.forEach(function(_e, ke) {
+                        ke > 0 && (M = Math.min((_e || 0) - (j[ke - 1] || 0), M))
+                    }), Number.isFinite(M)) {
+                    var D = M / _,
+                        C = v.layout === "vertical" ? n.height : n.width;
+                    if (v.padding === "gap" && (A = D * C / 2), v.padding === "no-gap") {
+                        var L = ar(t.barCategoryGap, D * C),
+                            B = D * C / 2;
+                        A = B - L - (B - L) / C * L
+                    }
                 }
             }
             i === "xAxis" ? P = [n.left + (x.left || 0) + (A || 0), n.left + n.width - (x.right || 0) - (A || 0)] : i === "yAxis" ? P = c === "horizontal" ? [n.top + n.height - (x.bottom || 0), n.top + (x.top || 0)] : [n.top + (x.top || 0) + (A || 0), n.top + n.height - (x.bottom || 0) - (A || 0)] : P = v.range, g && (P = [P[1], P[0]]);
-            var F = kI(v, a, h),
-                q = F.scale,
-                Z = F.realScaleType;
+            var W = kI(v, a, h),
+                q = W.scale,
+                Z = W.realScaleType;
             q.domain(w).range(P), DI(q);
             var U = UI(q, tt(tt({}, v), {}, {
                 realScaleType: Z
             }));
-            i === "xAxis" ? ($ = d === "top" && !m || d === "bottom" && m, T = n.left, E = l[O] - $ * v.height) : i === "yAxis" && ($ = d === "left" && !m || d === "right" && m, T = l[O] - $ * v.width, E = n.top);
-            var ee = tt(tt(tt({}, v), U), {}, {
+            i === "xAxis" ? ($ = d === "top" && !m || d === "bottom" && m, E = n.left, T = l[O] - $ * v.height) : i === "yAxis" && ($ = d === "left" && !m || d === "right" && m, E = l[O] - $ * v.width, T = n.top);
+            var Q = tt(tt(tt({}, v), U), {}, {
                 realScaleType: Z,
-                x: T,
-                y: E,
+                x: E,
+                y: T,
                 scale: q,
                 width: i === "xAxis" ? n.width : v.width,
                 height: i === "yAxis" ? n.height : v.height
             });
-            return ee.bandSize = va(ee, U), !v.hide && i === "xAxis" ? l[O] += ($ ? -1 : 1) * ee.height : v.hide || (l[O] += ($ ? -1 : 1) * ee.width), tt(tt({}, p), {}, mo({}, y, ee))
+            return Q.bandSize = va(Q, U), !v.hide && i === "xAxis" ? l[O] += ($ ? -1 : 1) * Q.height : v.hide || (l[O] += ($ ? -1 : 1) * Q.width), tt(tt({}, p), {}, mo({}, y, Q))
         }, {})
     },
     xy = function(t, r) {
         var n = t.x,
             i = t.y,
             a = r.x,
             o = r.y;
@@ -15000,21 +15004,21 @@
             y: e.top,
             width: e.width,
             height: e.height
         }
     }, function(e) {
         return ["l", e.left, "t", e.top, "w", e.width, "h", e.height].join("")
     }),
-    gs = B.createContext(void 0),
-    bs = B.createContext(void 0),
-    Oy = B.createContext(void 0),
-    Ay = B.createContext({}),
-    Sy = B.createContext(void 0),
-    Py = B.createContext(0),
-    _y = B.createContext(0),
+    gs = R.createContext(void 0),
+    bs = R.createContext(void 0),
+    Oy = R.createContext(void 0),
+    Ay = R.createContext({}),
+    Sy = R.createContext(void 0),
+    Py = R.createContext(0),
+    _y = R.createContext(0),
     ep = function(t) {
         var r = t.state,
             n = r.xAxisMap,
             i = r.yAxisMap,
             a = r.offset,
             o = t.clipPathId,
             u = t.children,
@@ -15034,51 +15038,51 @@
         }, S.createElement(Py.Provider, {
             value: s
         }, S.createElement(_y.Provider, {
             value: c
         }, u)))))))
     },
     xB = function() {
-        return B.useContext(Sy)
+        return R.useContext(Sy)
     },
     $y = function(t) {
-        var r = B.useContext(gs);
-        r == null && ur(!1);
+        var r = R.useContext(gs);
+        r == null && cr(!1);
         var n = r[t];
-        return n == null && ur(!1), n
+        return n == null && cr(!1), n
     },
     wB = function() {
-        var t = B.useContext(gs);
+        var t = R.useContext(gs);
         return kt(t)
     },
     OB = function() {
-        var t = B.useContext(bs),
+        var t = R.useContext(bs),
             r = gB(t, function(n) {
                 return vy(n.domain, Number.isFinite)
             });
         return r || kt(t)
     },
     Ty = function(t) {
-        var r = B.useContext(bs);
-        r == null && ur(!1);
+        var r = R.useContext(bs);
+        r == null && cr(!1);
         var n = r[t];
-        return n == null && ur(!1), n
+        return n == null && cr(!1), n
     },
     AB = function() {
-        var t = B.useContext(Oy);
+        var t = R.useContext(Oy);
         return t
     },
     SB = function() {
-        return B.useContext(Ay)
+        return R.useContext(Ay)
     },
     xs = function() {
-        return B.useContext(_y)
+        return R.useContext(_y)
     },
     ws = function() {
-        return B.useContext(Py)
+        return R.useContext(Py)
     };
 
 function ci(e) {
     "@babel/helpers - typeof";
     return ci = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
         return typeof t
     } : function(t) {
@@ -15278,26 +15282,26 @@
     var b = TB(w, 2),
         x = b[0],
         m = x.x,
         g = x.y,
         O = b[1],
         A = O.x,
         P = O.y,
-        T = pt(e, "hidden") ? "url(#".concat(s, ")") : void 0,
-        E = rp(rp({
-            clipPath: T
-        }, G(e, !0)), {}, {
+        E = pt(e, "hidden") ? "url(#".concat(s, ")") : void 0,
+        T = rp(rp({
+            clipPath: E
+        }, H(e, !0)), {}, {
             x1: m,
             y1: g,
             x2: A,
             y2: P
         });
     return S.createElement(ie, {
-        className: re("recharts-reference-line", u)
-    }, IB(o, E), Me.renderCallByParent(e, ZL({
+        className: ee("recharts-reference-line", u)
+    }, IB(o, T), je.renderCallByParent(e, ZL({
         x1: m,
         y1: g,
         x2: A,
         y2: P
     })))
 }
 Os.displayName = "ReferenceLine";
@@ -15411,21 +15415,21 @@
     var s = c.x,
         f = c.y,
         l = e.shape,
         h = e.className,
         p = pt(e, "hidden") ? "url(#".concat(a, ")") : void 0,
         y = ap(ap({
             clipPath: p
-        }, G(e, !0)), {}, {
+        }, H(e, !0)), {}, {
             cx: s,
             cy: f
         });
     return S.createElement(ie, {
-        className: re("recharts-reference-dot", h)
-    }, wi.renderDot(l, y), Me.renderCallByParent(e, {
+        className: ee("recharts-reference-dot", h)
+    }, wi.renderDot(l, y), je.renderCallByParent(e, {
         x: s - n,
         y: f - n,
         width: 2 * n,
         height: 2 * n
     }))
 }
 wi.displayName = "ReferenceDot";
@@ -15561,18 +15565,18 @@
         l = be(i),
         h = e.shape;
     if (!c && !s && !f && !l && !h) return null;
     var p = WB(c, s, f, l, e);
     if (!p && !h) return null;
     var y = pt(e, "hidden") ? "url(#".concat(u, ")") : void 0;
     return S.createElement(ie, {
-        className: re("recharts-reference-area", a)
+        className: ee("recharts-reference-area", a)
     }, Oi.renderRect(h, up(up({
         clipPath: y
-    }, G(e, !0)), p)), Me.renderCallByParent(e, p))
+    }, H(e, !0)), p)), je.renderCallByParent(e, p))
 }
 Oi.displayName = "ReferenceArea";
 Oi.defaultProps = {
     isFront: !1,
     ifOverflow: "discard",
     xAxisId: 0,
     yAxisId: 0,
@@ -15665,15 +15669,15 @@
         t && (n = n.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function je(e) {
+function Ee(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? cp(Object(r), !0).forEach(function(n) {
             GB(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : cp(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
@@ -15710,22 +15714,22 @@
     for (var a = (n || []).slice(), o = a.length, u = t.start, c = t.end, s = function(h) {
             var p = a[h],
                 y, v = function() {
                     return y === void 0 && (y = r(p, h)), y
                 };
             if (h === o - 1) {
                 var d = e * (p.coordinate + e * v() / 2 - c);
-                a[h] = p = je(je({}, p), {}, {
+                a[h] = p = Ee(Ee({}, p), {}, {
                     tickCoord: d > 0 ? p.coordinate - d * e : p.coordinate
                 })
-            } else a[h] = p = je(je({}, p), {}, {
+            } else a[h] = p = Ee(Ee({}, p), {}, {
                 tickCoord: p.coordinate
             });
             var w = Ea(e, p.tickCoord, v, u, c);
-            w && (c = p.tickCoord - e * (v() / 2 + i), a[h] = je(je({}, p), {}, {
+            w && (c = p.tickCoord - e * (v() / 2 + i), a[h] = Ee(Ee({}, p), {}, {
                 isShow: !0
             }))
         }, f = o - 1; f >= 0; f--) s(f);
     return a
 }
 
 function ZB(e, t, r, n, i, a) {
@@ -15733,39 +15737,39 @@
         u = o.length,
         c = t.start,
         s = t.end;
     if (a) {
         var f = n[u - 1],
             l = r(f, u - 1),
             h = e * (f.coordinate + e * l / 2 - s);
-        o[u - 1] = f = je(je({}, f), {}, {
+        o[u - 1] = f = Ee(Ee({}, f), {}, {
             tickCoord: h > 0 ? f.coordinate - h * e : f.coordinate
         });
         var p = Ea(e, f.tickCoord, function() {
             return l
         }, c, s);
-        p && (s = f.tickCoord - e * (l / 2 + i), o[u - 1] = je(je({}, f), {}, {
+        p && (s = f.tickCoord - e * (l / 2 + i), o[u - 1] = Ee(Ee({}, f), {}, {
             isShow: !0
         }))
     }
     for (var y = a ? u - 1 : u, v = function(b) {
             var x = o[b],
                 m, g = function() {
                     return m === void 0 && (m = r(x, b)), m
                 };
             if (b === 0) {
                 var O = e * (x.coordinate - e * g() / 2 - c);
-                o[b] = x = je(je({}, x), {}, {
+                o[b] = x = Ee(Ee({}, x), {}, {
                     tickCoord: O < 0 ? x.coordinate - O * e : x.coordinate
                 })
-            } else o[b] = x = je(je({}, x), {}, {
+            } else o[b] = x = Ee(Ee({}, x), {}, {
                 tickCoord: x.coordinate
             });
             var A = Ea(e, x.tickCoord, g, c, s);
-            A && (c = x.tickCoord + e * (g() / 2 + i), o[b] = je(je({}, x), {}, {
+            A && (c = x.tickCoord + e * (g() / 2 + i), o[b] = Ee(Ee({}, x), {}, {
                 isShow: !0
             }))
         }, d = 0; d < y; d++) v(d);
     return o
 }
 
 function As(e, t, r) {
@@ -15814,36 +15818,36 @@
     return Lr = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
         return typeof t
     } : function(t) {
         return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
     }, Lr(e)
 }
 
-function br() {
-    return br = Object.assign ? Object.assign.bind() : function(e) {
+function xr() {
+    return xr = Object.assign ? Object.assign.bind() : function(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t];
             for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
         }
         return e
-    }, br.apply(this, arguments)
+    }, xr.apply(this, arguments)
 }
 
 function sp(e, t) {
     var r = Object.keys(e);
     if (Object.getOwnPropertySymbols) {
         var n = Object.getOwnPropertySymbols(e);
         t && (n = n.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function Ie(e) {
+function Ce(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? sp(Object(r), !0).forEach(function(n) {
             Ss(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : sp(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
@@ -15975,15 +15979,15 @@
         key: "shouldComponentUpdate",
         value: function(n, i) {
             var a = n.viewBox,
                 o = Xo(n, JB),
                 u = this.props,
                 c = u.viewBox,
                 s = Xo(u, QB);
-            return !xr(a, c) || !xr(o, s) || !xr(i, this.state)
+            return !wr(a, c) || !wr(o, s) || !wr(i, this.state)
         }
     }, {
         key: "componentDidMount",
         value: function() {
             var n = this.layerReference;
             if (n) {
                 var i = n.getElementsByClassName("recharts-cartesian-axis-tick-value")[0];
@@ -16083,80 +16087,80 @@
                 i = n.x,
                 a = n.y,
                 o = n.width,
                 u = n.height,
                 c = n.orientation,
                 s = n.mirror,
                 f = n.axisLine,
-                l = Ie(Ie(Ie({}, G(this.props, !1)), G(f, !1)), {}, {
+                l = Ce(Ce(Ce({}, H(this.props, !1)), H(f, !1)), {}, {
                     fill: "none"
                 });
             if (c === "top" || c === "bottom") {
                 var h = +(c === "top" && !s || c === "bottom" && s);
-                l = Ie(Ie({}, l), {}, {
+                l = Ce(Ce({}, l), {}, {
                     x1: i,
                     y1: a + h * u,
                     x2: i + o,
                     y2: a + h * u
                 })
             } else {
                 var p = +(c === "left" && !s || c === "right" && s);
-                l = Ie(Ie({}, l), {}, {
+                l = Ce(Ce({}, l), {}, {
                     x1: i + p * o,
                     y1: a,
                     x2: i + p * o,
                     y2: a + u
                 })
             }
-            return S.createElement("line", br({}, l, {
-                className: re("recharts-cartesian-axis-line", Ze(f, "className"))
+            return S.createElement("line", xr({}, l, {
+                className: ee("recharts-cartesian-axis-line", Ze(f, "className"))
             }))
         }
     }, {
         key: "renderTicks",
         value: function(n, i, a) {
             var o = this,
                 u = this.props,
                 c = u.tickLine,
                 s = u.stroke,
                 f = u.tick,
                 l = u.tickFormatter,
                 h = u.unit,
-                p = As(Ie(Ie({}, this.props), {}, {
+                p = As(Ce(Ce({}, this.props), {}, {
                     ticks: n
                 }), i, a),
                 y = this.getTickTextAnchor(),
                 v = this.getTickVerticalAnchor(),
-                d = G(this.props, !1),
-                w = G(f, !1),
-                b = Ie(Ie({}, d), {}, {
+                d = H(this.props, !1),
+                w = H(f, !1),
+                b = Ce(Ce({}, d), {}, {
                     fill: "none"
-                }, G(c, !1)),
+                }, H(c, !1)),
                 x = p.map(function(m, g) {
                     var O = o.getTickLineCoord(m),
                         A = O.line,
                         P = O.tick,
-                        T = Ie(Ie(Ie(Ie({
+                        E = Ce(Ce(Ce(Ce({
                             textAnchor: y,
                             verticalAnchor: v
                         }, d), {}, {
                             stroke: "none",
                             fill: s
                         }, w), P), {}, {
                             index: g,
                             payload: m,
                             visibleTicksCount: p.length,
                             tickFormatter: l
                         });
-                    return S.createElement(ie, br({
+                    return S.createElement(ie, xr({
                         className: "recharts-cartesian-axis-tick",
                         key: "tick-".concat(m.value, "-").concat(m.coordinate, "-").concat(m.tickCoord)
-                    }, Tn(o.props, m, g)), c && S.createElement("line", br({}, b, A, {
-                        className: re("recharts-cartesian-axis-tick-line", Ze(c, "className"))
-                    })), f && t.renderTickItem(f, T, "".concat(Y(l) ? l(m.value, g) : m.value).concat(h || "")))
+                    }, Tn(o.props, m, g)), c && S.createElement("line", xr({}, b, A, {
+                        className: ee("recharts-cartesian-axis-tick-line", Ze(c, "className"))
+                    })), f && t.renderTickItem(f, E, "".concat(Y(l) ? l(m.value, g) : m.value).concat(h || "")))
                 });
             return S.createElement("g", {
                 className: "recharts-cartesian-axis-ticks"
             }, x)
         }
     }, {
         key: "render",
@@ -16171,30 +16175,30 @@
                 f = i.hide;
             if (f) return null;
             var l = this.props,
                 h = l.ticks,
                 p = Xo(l, eR),
                 y = h;
             return Y(c) && (y = h && h.length > 0 ? c(this.props) : c(p)), o <= 0 || u <= 0 || !y || !y.length ? null : S.createElement(ie, {
-                className: re("recharts-cartesian-axis", s),
+                className: ee("recharts-cartesian-axis", s),
                 ref: function(d) {
                     n.layerReference = d
                 }
-            }, a && this.renderAxisLine(), this.renderTicks(y, this.state.fontSize, this.state.letterSpacing), Me.renderCallByParent(this.props))
+            }, a && this.renderAxisLine(), this.renderTicks(y, this.state.fontSize, this.state.letterSpacing), je.renderCallByParent(this.props))
         }
     }], [{
         key: "renderTickItem",
         value: function(n, i, a) {
             var o;
-            return S.isValidElement(n) ? o = S.cloneElement(n, i) : Y(n) ? o = n(i) : o = S.createElement(ra, br({}, i, {
+            return S.isValidElement(n) ? o = S.cloneElement(n, i) : Y(n) ? o = n(i) : o = S.createElement(ra, xr({}, i, {
                 className: "recharts-cartesian-axis-tick-value"
             }), a), o
         }
     }]), t
-}(B.Component);
+}(R.Component);
 Ss(an, "displayName", "CartesianAxis");
 Ss(an, "defaultProps", {
     x: 0,
     y: 0,
     width: 0,
     height: 0,
     viewBox: {
@@ -16214,35 +16218,35 @@
     tickSize: 6,
     tickMargin: 2,
     interval: "preserveEnd"
 });
 var sR = ["x1", "y1", "x2", "y2", "key"],
     lR = ["offset"];
 
-function cr(e) {
+function sr(e) {
     "@babel/helpers - typeof";
-    return cr = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
+    return sr = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
         return typeof t
     } : function(t) {
         return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-    }, cr(e)
+    }, sr(e)
 }
 
 function fp(e, t) {
     var r = Object.keys(e);
     if (Object.getOwnPropertySymbols) {
         var n = Object.getOwnPropertySymbols(e);
         t && (n = n.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function Ce(e) {
+function Me(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? fp(Object(r), !0).forEach(function(n) {
             fR(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : fp(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
@@ -16257,23 +16261,23 @@
         configurable: !0,
         writable: !0
     }) : e[t] = r, e
 }
 
 function hR(e) {
     var t = pR(e, "string");
-    return cr(t) == "symbol" ? t : String(t)
+    return sr(t) == "symbol" ? t : String(t)
 }
 
 function pR(e, t) {
-    if (cr(e) != "object" || !e) return e;
+    if (sr(e) != "object" || !e) return e;
     var r = e[Symbol.toPrimitive];
     if (r !== void 0) {
         var n = r.call(e, t || "default");
-        if (cr(n) != "object") return n;
+        if (sr(n) != "object") return n;
         throw new TypeError("@@toPrimitive must return a primitive value.")
     }
     return (t === "string" ? String : Number)(e)
 }
 
 function er() {
     return er = Object.assign ? Object.assign.bind() : function(e) {
@@ -16331,15 +16335,15 @@
     else {
         var n = t.x1,
             i = t.y1,
             a = t.x2,
             o = t.y2,
             u = t.key,
             c = hp(t, sR),
-            s = G(c, !1);
+            s = H(c, !1);
         s.offset;
         var f = hp(s, lR);
         r = S.createElement("line", er({}, f, {
             x1: n,
             y1: i,
             x2: a,
             y2: o,
@@ -16354,15 +16358,15 @@
     var t = e.x,
         r = e.width,
         n = e.horizontal,
         i = n === void 0 ? !0 : n,
         a = e.horizontalPoints;
     if (!i || !a || !a.length) return null;
     var o = a.map(function(u, c) {
-        var s = Ce(Ce({}, e), {}, {
+        var s = Me(Me({}, e), {}, {
             x1: t,
             y1: u,
             x2: t + r,
             y2: u,
             key: "line-".concat(c),
             index: c
         });
@@ -16377,15 +16381,15 @@
     var t = e.y,
         r = e.height,
         n = e.vertical,
         i = n === void 0 ? !0 : n,
         a = e.verticalPoints;
     if (!i || !a || !a.length) return null;
     var o = a.map(function(u, c) {
-        var s = Ce(Ce({}, e), {}, {
+        var s = Me(Me({}, e), {}, {
             x1: u,
             y1: t,
             x2: u,
             y2: t + r,
             key: "line-".concat(c),
             index: c
         });
@@ -16474,61 +16478,61 @@
     }, l)
 }
 var xR = function(t, r) {
         var n = t.xAxis,
             i = t.width,
             a = t.height,
             o = t.offset;
-        return Gv(As(Ce(Ce(Ce({}, an.defaultProps), n), {}, {
+        return Gv(As(Me(Me(Me({}, an.defaultProps), n), {}, {
             ticks: wt(n, !0),
             viewBox: {
                 x: 0,
                 y: 0,
                 width: i,
                 height: a
             }
         })), o.left, o.left + o.width, r)
     },
     wR = function(t, r) {
         var n = t.yAxis,
             i = t.width,
             a = t.height,
             o = t.offset;
-        return Gv(As(Ce(Ce(Ce({}, an.defaultProps), n), {}, {
+        return Gv(As(Me(Me(Me({}, an.defaultProps), n), {}, {
             ticks: wt(n, !0),
             viewBox: {
                 x: 0,
                 y: 0,
                 width: i,
                 height: a
             }
         })), o.top, o.top + o.height, r)
     },
-    yr = {
+    mr = {
         horizontal: !0,
         vertical: !0,
         horizontalPoints: [],
         verticalPoints: [],
         stroke: "#ccc",
         fill: "none",
         verticalFill: [],
         horizontalFill: []
     };
 
 function OR(e) {
     var t, r, n, i, a, o, u = xs(),
         c = ws(),
         s = SB(),
-        f = Ce(Ce({}, e), {}, {
-            stroke: (t = e.stroke) !== null && t !== void 0 ? t : yr.stroke,
-            fill: (r = e.fill) !== null && r !== void 0 ? r : yr.fill,
-            horizontal: (n = e.horizontal) !== null && n !== void 0 ? n : yr.horizontal,
-            horizontalFill: (i = e.horizontalFill) !== null && i !== void 0 ? i : yr.horizontalFill,
-            vertical: (a = e.vertical) !== null && a !== void 0 ? a : yr.vertical,
-            verticalFill: (o = e.verticalFill) !== null && o !== void 0 ? o : yr.verticalFill,
+        f = Me(Me({}, e), {}, {
+            stroke: (t = e.stroke) !== null && t !== void 0 ? t : mr.stroke,
+            fill: (r = e.fill) !== null && r !== void 0 ? r : mr.fill,
+            horizontal: (n = e.horizontal) !== null && n !== void 0 ? n : mr.horizontal,
+            horizontalFill: (i = e.horizontalFill) !== null && i !== void 0 ? i : mr.horizontalFill,
+            vertical: (a = e.vertical) !== null && a !== void 0 ? a : mr.vertical,
+            verticalFill: (o = e.verticalFill) !== null && o !== void 0 ? o : mr.verticalFill,
             x: N(e.x) ? e.x : s.left,
             y: N(e.y) ? e.y : s.top,
             width: N(e.width) ? e.width : s.width,
             height: N(e.height) ? e.height : s.height
         }),
         l = f.x,
         h = f.y,
@@ -16542,35 +16546,35 @@
     if (!N(p) || p <= 0 || !N(y) || y <= 0 || !N(l) || l !== +l || !N(h) || h !== +h) return null;
     var m = f.verticalCoordinatesGenerator || xR,
         g = f.horizontalCoordinatesGenerator || wR,
         O = f.horizontalPoints,
         A = f.verticalPoints;
     if ((!O || !O.length) && Y(g)) {
         var P = d && d.length,
-            T = g({
-                yAxis: x ? Ce(Ce({}, x), {}, {
+            E = g({
+                yAxis: x ? Me(Me({}, x), {}, {
                     ticks: P ? d : x.ticks
                 }) : void 0,
                 width: u,
                 height: c,
                 offset: s
             }, P ? !0 : v);
-        At(Array.isArray(T), "horizontalCoordinatesGenerator should return Array but instead it returned [".concat(cr(T), "]")), Array.isArray(T) && (O = T)
+        At(Array.isArray(E), "horizontalCoordinatesGenerator should return Array but instead it returned [".concat(sr(E), "]")), Array.isArray(E) && (O = E)
     }
     if ((!A || !A.length) && Y(m)) {
-        var E = w && w.length,
+        var T = w && w.length,
             $ = m({
-                xAxis: b ? Ce(Ce({}, b), {}, {
-                    ticks: E ? w : b.ticks
+                xAxis: b ? Me(Me({}, b), {}, {
+                    ticks: T ? w : b.ticks
                 }) : void 0,
                 width: u,
                 height: c,
                 offset: s
-            }, E ? !0 : v);
-        At(Array.isArray($), "verticalCoordinatesGenerator should return Array but instead it returned [".concat(cr($), "]")), Array.isArray($) && (A = $)
+            }, T ? !0 : v);
+        At(Array.isArray($), "verticalCoordinatesGenerator should return Array but instead it returned [".concat(sr($), "]")), Array.isArray($) && (A = $)
     }
     return S.createElement("g", {
         className: "recharts-cartesian-grid"
     }, S.createElement(vR, {
         fill: f.fill,
         fillOpacity: f.fillOpacity,
         x: f.x,
@@ -16642,27 +16646,27 @@
         t && (n = n.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function Re(e) {
+function Fe(e) {
     for (var t = 1; t < arguments.length; t++) {
         var r = arguments[t] != null ? arguments[t] : {};
         t % 2 ? pp(Object(r), !0).forEach(function(n) {
             rt(e, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : pp(Object(r)).forEach(function(n) {
             Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
         })
     }
     return e
 }
 
-function mr(e) {
+function gr(e) {
     return ER(e) || TR(e) || $R(e) || _R()
 }
 
 function _R() {
     throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
@@ -16795,21 +16799,21 @@
         }), rt(Mt(r), "getStrokeDasharray", function(o, u, c) {
             var s = c.reduce(function(w, b) {
                 return w + b
             });
             if (!s) return r.generateSimpleStrokeDasharray(u, o);
             for (var f = Math.floor(o / s), l = o % s, h = u - o, p = [], y = 0, v = 0; y < c.length; v += c[y], ++y)
                 if (v + c[y] > l) {
-                    p = [].concat(mr(c.slice(0, y)), [l - v]);
+                    p = [].concat(gr(c.slice(0, y)), [l - v]);
                     break
                 } var d = p.length % 2 === 0 ? [0, h] : [h];
-            return [].concat(mr(t.repeat(c, f)), mr(p), d).map(function(w) {
+            return [].concat(gr(t.repeat(c, f)), gr(p), d).map(function(w) {
                 return "".concat(w, "px")
             }).join(", ")
-        }), rt(Mt(r), "id", lr("recharts-line-")), rt(Mt(r), "pathRef", function(o) {
+        }), rt(Mt(r), "id", fr("recharts-line-")), rt(Mt(r), "pathRef", function(o) {
             r.mainCurve = o
         }), rt(Mt(r), "handleAnimationEnd", function() {
             r.setState({
                 isAnimationFinished: !0
             }), r.props.onAnimationEnd && r.props.onAnimationEnd()
         }), rt(Mt(r), "handleAnimationStart", function() {
             r.setState({
@@ -16853,15 +16857,15 @@
             if (this.props.isAnimationActive && !this.state.isAnimationFinished) return null;
             var a = this.props,
                 o = a.points,
                 u = a.xAxis,
                 c = a.yAxis,
                 s = a.layout,
                 f = a.children,
-                l = Ne(f, tn);
+                l = Le(f, tn);
             if (!l) return null;
             var h = function(v, d) {
                     return {
                         x: v.x,
                         y: v.y,
                         value: v.value,
                         errorVal: xe(v.payload, d)
@@ -16886,18 +16890,18 @@
         value: function(n, i, a) {
             var o = this.props.isAnimationActive;
             if (o && !this.state.isAnimationFinished) return null;
             var u = this.props,
                 c = u.dot,
                 s = u.points,
                 f = u.dataKey,
-                l = G(this.props, !1),
-                h = G(c, !0),
+                l = H(this.props, !1),
+                h = H(c, !0),
                 p = s.map(function(v, d) {
-                    var w = Re(Re(Re({
+                    var w = Fe(Fe(Fe({
                         key: "dot-".concat(d),
                         r: 3
                     }, l), h), {}, {
                         value: v.value,
                         dataKey: f,
                         cx: v.x,
                         cy: v.y,
@@ -16919,15 +16923,15 @@
         value: function(n, i, a, o) {
             var u = this.props,
                 c = u.type,
                 s = u.layout,
                 f = u.connectNulls;
             u.ref;
             var l = SR(u, AR),
-                h = Re(Re(Re({}, G(l, !0)), {}, {
+                h = Fe(Fe(Fe({}, H(l, !0)), {}, {
                     fill: "none",
                     className: "recharts-line-curve",
                     clipPath: i ? "url(#clipPath-".concat(a, ")") : null,
                     points: n
                 }, o), {}, {
                     type: c,
                     layout: s,
@@ -16972,61 +16976,61 @@
             }, function(m) {
                 var g = m.t;
                 if (b) {
                     var O = b.length / u.length,
                         A = u.map(function(_, M) {
                             var j = Math.floor(M * O);
                             if (b[j]) {
-                                var k = b[j],
-                                    C = de(k.x, _.x),
-                                    L = de(k.y, _.y);
-                                return Re(Re({}, _), {}, {
+                                var D = b[j],
+                                    C = de(D.x, _.x),
+                                    L = de(D.y, _.y);
+                                return Fe(Fe({}, _), {}, {
                                     x: C(g),
                                     y: L(g)
                                 })
                             }
                             if (y) {
-                                var R = de(v * 2, _.x),
-                                    F = de(d / 2, _.y);
-                                return Re(Re({}, _), {}, {
-                                    x: R(g),
-                                    y: F(g)
+                                var B = de(v * 2, _.x),
+                                    W = de(d / 2, _.y);
+                                return Fe(Fe({}, _), {}, {
+                                    x: B(g),
+                                    y: W(g)
                                 })
                             }
-                            return Re(Re({}, _), {}, {
+                            return Fe(Fe({}, _), {}, {
                                 x: _.x,
                                 y: _.y
                             })
                         });
                     return a.renderCurveStatically(A, n, i)
                 }
                 var P = de(0, x),
-                    T = P(g),
-                    E;
+                    E = P(g),
+                    T;
                 if (c) {
                     var $ = "".concat(c).split(/[,\s]+/gim).map(function(_) {
                         return parseFloat(_)
                     });
-                    E = a.getStrokeDasharray(T, x, $)
-                } else E = a.generateSimpleStrokeDasharray(x, T);
+                    T = a.getStrokeDasharray(E, x, $)
+                } else T = a.generateSimpleStrokeDasharray(x, E);
                 return a.renderCurveStatically(u, n, i, {
-                    strokeDasharray: E
+                    strokeDasharray: T
                 })
             })
         }
     }, {
         key: "renderCurve",
         value: function(n, i) {
             var a = this.props,
                 o = a.points,
                 u = a.isAnimationActive,
                 c = this.state,
                 s = c.prevPoints,
                 f = c.totalLength;
-            return u && o && o.length && (!s && f > 0 || !ar(s, o)) ? this.renderCurveWithAnimation(n, i) : this.renderCurveStatically(o, n, i)
+            return u && o && o.length && (!s && f > 0 || !or(s, o)) ? this.renderCurveWithAnimation(n, i) : this.renderCurveStatically(o, n, i)
         }
     }, {
         key: "render",
         value: function() {
             var n, i = this.props,
                 a = i.hide,
                 o = i.dot,
@@ -17039,48 +17043,48 @@
                 p = i.width,
                 y = i.height,
                 v = i.isAnimationActive,
                 d = i.id;
             if (a || !u || !u.length) return null;
             var w = this.state.isAnimationFinished,
                 b = u.length === 1,
-                x = re("recharts-line", c),
+                x = ee("recharts-line", c),
                 m = s && s.allowDataOverflow,
                 g = f && f.allowDataOverflow,
                 O = m || g,
-                A = X(d) ? this.id : d,
-                P = (n = G(o, !1)) !== null && n !== void 0 ? n : {
+                A = G(d) ? this.id : d,
+                P = (n = H(o, !1)) !== null && n !== void 0 ? n : {
                     r: 3,
                     strokeWidth: 2
                 },
-                T = P.r,
-                E = T === void 0 ? 3 : T,
+                E = P.r,
+                T = E === void 0 ? 3 : E,
                 $ = P.strokeWidth,
                 _ = $ === void 0 ? 2 : $,
                 M = Wp(o) ? o : {},
                 j = M.clipDot,
-                k = j === void 0 ? !0 : j,
-                C = E * 2 + _;
+                D = j === void 0 ? !0 : j,
+                C = T * 2 + _;
             return S.createElement(ie, {
                 className: x
             }, m || g ? S.createElement("defs", null, S.createElement("clipPath", {
                 id: "clipPath-".concat(A)
             }, S.createElement("rect", {
                 x: m ? h : h - p / 2,
                 y: g ? l : l - y / 2,
                 width: m ? p : p * 2,
                 height: g ? y : y * 2
-            })), !k && S.createElement("clipPath", {
+            })), !D && S.createElement("clipPath", {
                 id: "clipPath-dots-".concat(A)
             }, S.createElement("rect", {
                 x: h - C / 2,
                 y: l - C / 2,
                 width: p + C,
                 height: y + C
-            }))) : null, !b && this.renderCurve(O, A), this.renderErrorBar(O, A), (b || o) && this.renderDots(O, k, A), (!v || w) && ht.renderCallByParent(this.props, u))
+            }))) : null, !b && this.renderCurve(O, A), this.renderErrorBar(O, A), (b || o) && this.renderDots(O, D, A), (!v || w) && ht.renderCallByParent(this.props, u))
         }
     }], [{
         key: "getDerivedStateFromProps",
         value: function(n, i) {
             return n.animationId !== i.prevAnimationId ? {
                 prevAnimationId: n.animationId,
                 curPoints: n.points,
@@ -17088,33 +17092,33 @@
             } : n.points !== i.curPoints ? {
                 curPoints: n.points
             } : null
         }
     }, {
         key: "repeat",
         value: function(n, i) {
-            for (var a = n.length % 2 !== 0 ? [].concat(mr(n), [0]) : n, o = [], u = 0; u < i; ++u) o = [].concat(mr(o), mr(a));
+            for (var a = n.length % 2 !== 0 ? [].concat(gr(n), [0]) : n, o = [], u = 0; u < i; ++u) o = [].concat(gr(o), gr(a));
             return o
         }
     }, {
         key: "renderDotItem",
         value: function(n, i) {
             var a;
             if (S.isValidElement(n)) a = S.cloneElement(n, i);
             else if (Y(n)) a = n(i);
             else {
-                var o = re("recharts-line-dot", typeof n != "boolean" ? n.className : "");
+                var o = ee("recharts-line-dot", typeof n != "boolean" ? n.className : "");
                 a = S.createElement(po, Sn({}, i, {
                     className: o
                 }))
             }
             return a
         }
     }]), t
-}(B.PureComponent);
+}(R.PureComponent);
 rt(go, "displayName", "Line");
 rt(go, "defaultProps", {
     xAxisId: 0,
     yAxisId: 0,
     connectNulls: !1,
     activeDot: !0,
     dot: !0,
@@ -17148,31 +17152,31 @@
                 x: Cr({
                     axis: r,
                     ticks: i,
                     bandSize: u,
                     entry: h,
                     index: p
                 }),
-                y: X(y) ? null : n.scale(y),
+                y: G(y) ? null : n.scale(y),
                 value: y,
                 payload: h
             } : {
-                x: X(y) ? null : r.scale(y),
+                x: G(y) ? null : r.scale(y),
                 y: Cr({
                     axis: n,
                     ticks: a,
                     bandSize: u,
                     entry: h,
                     index: p
                 }),
                 value: y,
                 payload: h
             }
         });
-    return Re({
+    return Fe({
         points: l,
         layout: f
     }, s)
 });
 var NR = ["layout", "type", "stroke", "connectNulls", "isRange", "ref"],
     Dy;
 
@@ -17324,24 +17328,24 @@
     if (r !== void 0) {
         var n = r.call(e, t || "default");
         if (Rr(n) != "object") return n;
         throw new TypeError("@@toPrimitive must return a primitive value.")
     }
     return (t === "string" ? String : Number)(e)
 }
-var pr = function(e) {
+var dr = function(e) {
     UR(t, e);
 
     function t() {
         var r;
         RR(this, t);
         for (var n = arguments.length, i = new Array(n), a = 0; a < n; a++) i[a] = arguments[a];
         return r = zR(this, t, [].concat(i)), lt(gn(r), "state", {
             isAnimationFinished: !0
-        }), lt(gn(r), "id", lr("recharts-area-")), lt(gn(r), "handleAnimationEnd", function() {
+        }), lt(gn(r), "id", fr("recharts-area-")), lt(gn(r), "handleAnimationEnd", function() {
             var o = r.props.onAnimationEnd;
             r.setState({
                 isAnimationFinished: !0
             }), Y(o) && o()
         }), lt(gn(r), "handleAnimationStart", function() {
             var o = r.props.onAnimationStart;
             r.setState({
@@ -17355,16 +17359,16 @@
             var o = this.props.isAnimationActive,
                 u = this.state.isAnimationFinished;
             if (o && !u) return null;
             var c = this.props,
                 s = c.dot,
                 f = c.points,
                 l = c.dataKey,
-                h = G(this.props, !1),
-                p = G(s, !0),
+                h = H(this.props, !1),
+                p = H(s, !0),
                 y = f.map(function(d, w) {
                     var b = Ct(Ct(Ct({
                         key: "dot-".concat(w),
                         r: 3
                     }, h), p), {}, {
                         dataKey: l,
                         cx: d.x,
@@ -17441,30 +17445,30 @@
                 f = u.stroke,
                 l = u.connectNulls,
                 h = u.isRange;
             u.ref;
             var p = LR(u, NR);
             return S.createElement(ie, {
                 clipPath: a ? "url(#clipPath-".concat(o, ")") : null
-            }, S.createElement(ir, tr({}, G(p, !0), {
+            }, S.createElement(ir, tr({}, H(p, !0), {
                 points: n,
                 connectNulls: l,
                 type: s,
                 baseLine: i,
                 layout: c,
                 stroke: "none",
                 className: "recharts-area-area"
-            })), f !== "none" && S.createElement(ir, tr({}, G(this.props, !1), {
+            })), f !== "none" && S.createElement(ir, tr({}, H(this.props, !1), {
                 className: "recharts-area-curve",
                 layout: c,
                 type: s,
                 connectNulls: l,
                 fill: "none",
                 points: n
-            })), f !== "none" && h && S.createElement(ir, tr({}, G(this.props, !1), {
+            })), f !== "none" && h && S.createElement(ir, tr({}, H(this.props, !1), {
                 className: "recharts-area-curve",
                 layout: c,
                 type: s,
                 connectNulls: l,
                 fill: "none",
                 points: i
             })))
@@ -17498,38 +17502,38 @@
                 key: "area-".concat(p),
                 onAnimationEnd: this.handleAnimationEnd,
                 onAnimationStart: this.handleAnimationStart
             }, function(w) {
                 var b = w.t;
                 if (v) {
                     var x = v.length / u.length,
-                        m = u.map(function(P, T) {
-                            var E = Math.floor(T * x);
-                            if (v[E]) {
-                                var $ = v[E],
+                        m = u.map(function(P, E) {
+                            var T = Math.floor(E * x);
+                            if (v[T]) {
+                                var $ = v[T],
                                     _ = de($.x, P.x),
                                     M = de($.y, P.y);
                                 return Ct(Ct({}, P), {}, {
                                     x: _(b),
                                     y: M(b)
                                 })
                             }
                             return P
                         }),
                         g;
                     if (N(c) && typeof c == "number") {
                         var O = de(d, c);
                         g = O(b)
-                    } else if (X(c) || Xr(c)) {
+                    } else if (G(c) || Xr(c)) {
                         var A = de(d, 0);
                         g = A(b)
-                    } else g = c.map(function(P, T) {
-                        var E = Math.floor(T * x);
-                        if (d[E]) {
-                            var $ = d[E],
+                    } else g = c.map(function(P, E) {
+                        var T = Math.floor(E * x);
+                        if (d[T]) {
+                            var $ = d[T],
                                 _ = de($.x, P.x),
                                 M = de($.y, P.y);
                             return Ct(Ct({}, P), {}, {
                                 x: _(b),
                                 y: M(b)
                             })
                         }
@@ -17551,15 +17555,15 @@
                 o = a.points,
                 u = a.baseLine,
                 c = a.isAnimationActive,
                 s = this.state,
                 f = s.prevPoints,
                 l = s.prevBaseLine,
                 h = s.totalLength;
-            return c && o && o.length && (!f && h > 0 || !ar(f, o) || !ar(l, u)) ? this.renderAreaWithAnimation(n, i) : this.renderAreaStatically(o, u, n, i)
+            return c && o && o.length && (!f && h > 0 || !or(f, o) || !or(l, u)) ? this.renderAreaWithAnimation(n, i) : this.renderAreaStatically(o, u, n, i)
         }
     }, {
         key: "render",
         value: function() {
             var n, i = this.props,
                 a = i.hide,
                 o = i.dot,
@@ -17572,48 +17576,48 @@
                 p = i.width,
                 y = i.height,
                 v = i.isAnimationActive,
                 d = i.id;
             if (a || !u || !u.length) return null;
             var w = this.state.isAnimationFinished,
                 b = u.length === 1,
-                x = re("recharts-area", c),
+                x = ee("recharts-area", c),
                 m = l && l.allowDataOverflow,
                 g = h && h.allowDataOverflow,
                 O = m || g,
-                A = X(d) ? this.id : d,
-                P = (n = G(o, !1)) !== null && n !== void 0 ? n : {
+                A = G(d) ? this.id : d,
+                P = (n = H(o, !1)) !== null && n !== void 0 ? n : {
                     r: 3,
                     strokeWidth: 2
                 },
-                T = P.r,
-                E = T === void 0 ? 3 : T,
+                E = P.r,
+                T = E === void 0 ? 3 : E,
                 $ = P.strokeWidth,
                 _ = $ === void 0 ? 2 : $,
                 M = Wp(o) ? o : {},
                 j = M.clipDot,
-                k = j === void 0 ? !0 : j,
-                C = E * 2 + _;
+                D = j === void 0 ? !0 : j,
+                C = T * 2 + _;
             return S.createElement(ie, {
                 className: x
             }, m || g ? S.createElement("defs", null, S.createElement("clipPath", {
                 id: "clipPath-".concat(A)
             }, S.createElement("rect", {
                 x: m ? f : f - p / 2,
                 y: g ? s : s - y / 2,
                 width: m ? p : p * 2,
                 height: g ? y : y * 2
-            })), !k && S.createElement("clipPath", {
+            })), !D && S.createElement("clipPath", {
                 id: "clipPath-dots-".concat(A)
             }, S.createElement("rect", {
                 x: f - C / 2,
                 y: s - C / 2,
                 width: p + C,
                 height: y + C
-            }))) : null, b ? null : this.renderArea(O, A), (o || b) && this.renderDots(O, k, A), (!v || w) && ht.renderCallByParent(this.props, u))
+            }))) : null, b ? null : this.renderArea(O, A), (o || b) && this.renderDots(O, D, A), (!v || w) && ht.renderCallByParent(this.props, u))
         }
     }], [{
         key: "getDerivedStateFromProps",
         value: function(n, i) {
             return n.animationId !== i.prevAnimationId ? {
                 prevAnimationId: n.animationId,
                 curPoints: n.points,
@@ -17622,18 +17626,18 @@
                 prevBaseLine: i.curBaseLine
             } : n.points !== i.curPoints || n.baseLine !== i.curBaseLine ? {
                 curPoints: n.points,
                 curBaseLine: n.baseLine
             } : null
         }
     }]), t
-}(B.PureComponent);
-Dy = pr;
-lt(pr, "displayName", "Area");
-lt(pr, "defaultProps", {
+}(R.PureComponent);
+Dy = dr;
+lt(dr, "displayName", "Area");
+lt(dr, "defaultProps", {
     stroke: "#3182bd",
     fill: "#3182bd",
     fillOpacity: .6,
     xAxisId: 0,
     yAxisId: 0,
     legendType: "line",
     connectNulls: !1,
@@ -17642,30 +17646,30 @@
     activeDot: !0,
     hide: !1,
     isAnimationActive: !at.isSsr,
     animationBegin: 0,
     animationDuration: 1500,
     animationEasing: "ease"
 });
-lt(pr, "getBaseValue", function(e, t, r, n) {
+lt(dr, "getBaseValue", function(e, t, r, n) {
     var i = e.layout,
         a = e.baseValue,
         o = t.props.baseValue,
         u = o ?? a;
     if (N(u) && typeof u == "number") return u;
     var c = i === "horizontal" ? n : r,
         s = c.scale.domain();
     if (c.type === "number") {
         var f = Math.max(s[0], s[1]),
             l = Math.min(s[0], s[1]);
         return u === "dataMin" ? l : u === "dataMax" || f < 0 ? f : Math.max(Math.min(s[0], s[1]), 0)
     }
     return u === "dataMin" ? s[0] : u === "dataMax" ? s[1] : s[0]
 });
-lt(pr, "getComposedData", function(e) {
+lt(dr, "getComposedData", function(e) {
     var t = e.props,
         r = e.item,
         n = e.xAxis,
         i = e.yAxis,
         a = e.xAxisTicks,
         o = e.yAxisTicks,
         u = e.bandSize,
@@ -17720,20 +17724,20 @@
     }) : x = d ? i.scale(v) : n.scale(v), Ct({
         points: b,
         baseLine: x,
         layout: p,
         isRange: w
     }, h)
 });
-lt(pr, "renderDotItem", function(e, t) {
+lt(dr, "renderDotItem", function(e, t) {
     var r;
     if (S.isValidElement(e)) r = S.cloneElement(e, t);
     else if (Y(e)) r = e(t);
     else {
-        var n = re("recharts-area-dot", typeof e != "boolean" ? e.className : "");
+        var n = ee("recharts-area-dot", typeof e != "boolean" ? e.className : "");
         r = S.createElement(po, tr({}, t, {
             className: n
         }))
     }
     return r
 });
 var bo = function() {
@@ -17940,25 +17944,25 @@
             r.setState({
                 isAnimationFinished: !0
             })
         }), Lt(bn(r), "handleAnimationStart", function() {
             r.setState({
                 isAnimationFinished: !1
             })
-        }), Lt(bn(r), "id", lr("recharts-scatter-")), r
+        }), Lt(bn(r), "id", fr("recharts-scatter-")), r
     }
     return YR(t, [{
         key: "renderSymbolsStatically",
         value: function(n) {
             var i = this,
                 a = this.props,
                 o = a.shape,
                 u = a.activeShape,
                 c = a.activeIndex,
-                s = G(this.props, !1);
+                s = H(this.props, !1);
             return n.map(function(f, l) {
                 var h = c === l,
                     p = h ? u : o,
                     y = Xe(Xe({
                         key: "symbol-".concat(l)
                     }, s), f);
                 return S.createElement(ie, _n({
@@ -18023,27 +18027,27 @@
     }, {
         key: "renderSymbols",
         value: function() {
             var n = this.props,
                 i = n.points,
                 a = n.isAnimationActive,
                 o = this.state.prevPoints;
-            return a && i && i.length && (!o || !ar(o, i)) ? this.renderSymbolsWithAnimation() : this.renderSymbolsStatically(i)
+            return a && i && i.length && (!o || !or(o, i)) ? this.renderSymbolsWithAnimation() : this.renderSymbolsStatically(i)
         }
     }, {
         key: "renderErrorBar",
         value: function() {
             var n = this.props.isAnimationActive;
             if (n && !this.state.isAnimationFinished) return null;
             var i = this.props,
                 a = i.points,
                 o = i.xAxis,
                 u = i.yAxis,
                 c = i.children,
-                s = Ne(c, tn);
+                s = Le(c, tn);
             return s ? s.map(function(f, l) {
                 var h = f.props,
                     p = h.direction,
                     y = h.dataKey;
                 return S.cloneElement(f, {
                     key: "".concat(p, "-").concat(y, "-").concat(a[l]),
                     data: a,
@@ -18065,16 +18069,16 @@
         key: "renderLine",
         value: function() {
             var n = this.props,
                 i = n.points,
                 a = n.line,
                 o = n.lineType,
                 u = n.lineJointType,
-                c = G(this.props, !1),
-                s = G(a, !1),
+                c = H(this.props, !1),
+                s = H(a, !1),
                 f, l;
             if (o === "joint") f = i.map(function(x) {
                 return {
                     x: x.cx,
                     y: x.cy
                 }
             });
@@ -18122,19 +18126,19 @@
                 l = n.top,
                 h = n.width,
                 p = n.height,
                 y = n.id,
                 v = n.isAnimationActive;
             if (i || !a || !a.length) return null;
             var d = this.state.isAnimationFinished,
-                w = re("recharts-scatter", u),
+                w = ee("recharts-scatter", u),
                 b = c && c.allowDataOverflow,
                 x = s && s.allowDataOverflow,
                 m = b || x,
-                g = X(y) ? this.id : y;
+                g = G(y) ? this.id : y;
             return S.createElement(ie, {
                 className: w,
                 clipPath: m ? "url(#clipPath-".concat(g, ")") : null
             }, b || x ? S.createElement("defs", null, S.createElement("clipPath", {
                 id: "clipPath-".concat(g)
             }, S.createElement("rect", {
                 x: b ? f : f - h / 2,
@@ -18153,15 +18157,15 @@
                 curPoints: n.points,
                 prevPoints: i.curPoints
             } : n.points !== i.curPoints ? {
                 curPoints: n.points
             } : null
         }
     }]), t
-}(B.PureComponent);
+}(R.PureComponent);
 Lt(xo, "displayName", "Scatter");
 Lt(xo, "defaultProps", {
     xAxisId: 0,
     yAxisId: 0,
     zAxisId: 0,
     legendType: "circle",
     lineType: "joint",
@@ -18180,87 +18184,87 @@
         n = e.zAxis,
         i = e.item,
         a = e.displayedData,
         o = e.xAxisTicks,
         u = e.yAxisTicks,
         c = e.offset,
         s = i.props.tooltipType,
-        f = Ne(i.props.children, Kc),
-        l = X(t.dataKey) ? i.props.dataKey : t.dataKey,
-        h = X(r.dataKey) ? i.props.dataKey : r.dataKey,
+        f = Le(i.props.children, Kc),
+        l = G(t.dataKey) ? i.props.dataKey : t.dataKey,
+        h = G(r.dataKey) ? i.props.dataKey : r.dataKey,
         p = n && n.dataKey,
         y = n ? n.range : bo.defaultProps.range,
         v = y && y[0],
         d = t.scale.bandwidth ? t.scale.bandwidth() : 0,
         w = r.scale.bandwidth ? r.scale.bandwidth() : 0,
         b = a.map(function(x, m) {
             var g = xe(x, l),
                 O = xe(x, h),
-                A = !X(p) && xe(x, p) || "-",
+                A = !G(p) && xe(x, p) || "-",
                 P = [{
-                    name: X(t.dataKey) ? i.props.name : t.name || t.dataKey,
+                    name: G(t.dataKey) ? i.props.name : t.name || t.dataKey,
                     unit: t.unit || "",
                     value: g,
                     payload: x,
                     dataKey: l,
                     type: s
                 }, {
-                    name: X(r.dataKey) ? i.props.name : r.name || r.dataKey,
+                    name: G(r.dataKey) ? i.props.name : r.name || r.dataKey,
                     unit: r.unit || "",
                     value: O,
                     payload: x,
                     dataKey: h,
                     type: s
                 }];
             A !== "-" && P.push({
                 name: n.name || n.dataKey,
                 unit: n.unit || "",
                 value: A,
                 payload: x,
                 dataKey: p,
                 type: s
             });
-            var T = Cr({
+            var E = Cr({
                     axis: t,
                     ticks: o,
                     bandSize: d,
                     entry: x,
                     index: m,
                     dataKey: l
                 }),
-                E = Cr({
+                T = Cr({
                     axis: r,
                     ticks: u,
                     bandSize: w,
                     entry: x,
                     index: m,
                     dataKey: h
                 }),
                 $ = A !== "-" ? n.scale(A) : v,
                 _ = Math.sqrt(Math.max($, 0) / Math.PI);
             return Xe(Xe({}, x), {}, {
-                cx: T,
-                cy: E,
-                x: T - _,
-                y: E - _,
+                cx: E,
+                cy: T,
+                x: E - _,
+                y: T - _,
                 xAxis: t,
                 yAxis: r,
                 zAxis: n,
                 width: 2 * _,
                 height: 2 * _,
                 size: $,
                 node: {
                     x: g,
                     y: O,
                     z: A
                 },
                 tooltipPayload: P,
                 tooltipPosition: {
-                    x: T,
-                    y: E
+                    x: E,
+                    y: T
                 },
                 payload: x
             }, f && f[m] && f[m].props)
         });
     return Xe({
         points: b
     }, c)
@@ -18277,15 +18281,15 @@
 }
 var Ps = function(t) {
     var r = t.xAxisId,
         n = xs(),
         i = ws(),
         a = $y(r);
     return a == null ? null : S.createElement(an, hc({}, a, {
-        className: re("recharts-".concat(a.axisType, " ").concat(a.axisType), a.className),
+        className: ee("recharts-".concat(a.axisType, " ").concat(a.axisType), a.className),
         viewBox: {
             x: 0,
             y: 0,
             width: n,
             height: i
         },
         ticksGenerator: function(u) {
@@ -18325,15 +18329,15 @@
 }
 var _s = function(t) {
     var r = t.yAxisId,
         n = xs(),
         i = ws(),
         a = Ty(r);
     return a == null ? null : S.createElement(an, pc({}, a, {
-        className: re("recharts-".concat(a.axisType, " ").concat(a.axisType), a.className),
+        className: ee("recharts-".concat(a.axisType, " ").concat(a.axisType), a.className),
         viewBox: {
             x: 0,
             y: 0,
             width: n,
             height: i
         },
         ticksGenerator: function(u) {
@@ -18390,18 +18394,18 @@
 
 function dc(e, t) {
     (t == null || t > e.length) && (t = e.length);
     for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
     return n
 }
 var vc = function(t, r, n, i, a) {
-        var o = Ne(t, Os),
-            u = Ne(t, wi),
+        var o = Le(t, Os),
+            u = Le(t, wi),
             c = [].concat(bp(o), bp(u)),
-            s = Ne(t, Oi),
+            s = Le(t, Oi),
             f = "".concat(i, "Id"),
             l = i[0],
             h = r;
         if (c.length && (h = c.reduce(function(v, d) {
                 if (d.props[f] === n && pt(d.props, "extendDomain") && N(d.props[l])) {
                     var w = d.props[l];
                     return [Math.min(v[0], w), Math.max(v[1], w)]
@@ -18680,16 +18684,16 @@
 
 function Wy(e) {
     var t = e.cx,
         r = e.cy,
         n = e.radius,
         i = e.startAngle,
         a = e.endAngle,
-        o = $e(t, r, n, i),
-        u = $e(t, r, n, a);
+        o = Te(t, r, n, i),
+        u = Te(t, r, n, a);
     return {
         points: [o, u],
         cx: t,
         cy: r,
         radius: n,
         startAngle: i,
         endAngle: a
@@ -18703,16 +18707,16 @@
     else if (t.cx != null && t.cy != null)
         if (e === "centric") {
             var u = t.cx,
                 c = t.cy,
                 s = t.innerRadius,
                 f = t.outerRadius,
                 l = t.angle,
-                h = $e(u, c, s, l),
-                p = $e(u, c, f, l);
+                h = Te(u, c, s, l),
+                p = Te(u, c, f, l);
             n = h.x, i = h.y, a = p.x, o = p.y
         } else return Wy(t);
     return [{
         x: n,
         y: i
     }, {
         x: a,
@@ -18809,20 +18813,20 @@
         }, h = Jv
     } else l = {
         points: pF(s, i, o)
     }, h = ir;
     var x = Li(Li(Li(Li({
         stroke: "#ccc",
         pointerEvents: "none"
-    }, o), l), G(t.props.cursor, !1)), {}, {
+    }, o), l), H(t.props.cursor, !1)), {}, {
         payload: a,
         payloadIndex: u,
-        className: "recharts-tooltip-cursor"
+        className: ee("recharts-tooltip-cursor", t.props.cursor.className)
     });
-    return B.isValidElement(t.props.cursor) ? B.cloneElement(t.props.cursor, x) : B.createElement(h, x)
+    return R.isValidElement(t.props.cursor) ? R.cloneElement(t.props.cursor, x) : R.createElement(h, x)
 }
 var gF = ["item"],
     bF = ["children", "className", "width", "height", "style", "compact", "title", "desc"];
 
 function zr(e) {
     "@babel/helpers - typeof";
     return zr = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
@@ -19076,22 +19080,22 @@
             if (t === "vertical") return {
                 x: i.x,
                 y: a.coordinate
             };
             if (t === "centric") {
                 var o = a.coordinate,
                     u = i.radius;
-                return I(I(I({}, i), $e(i.cx, i.cy, u, o)), {}, {
+                return I(I(I({}, i), Te(i.cx, i.cy, u, o)), {}, {
                     angle: o,
                     radius: u
                 })
             }
             var c = a.coordinate,
                 s = i.angle;
-            return I(I(I({}, i), $e(i.cx, i.cy, c, s)), {}, {
+            return I(I(I({}, i), Te(i.cx, i.cy, c, s)), {}, {
                 angle: s,
                 radius: c
             })
         }
         return Hy
     },
     wo = function(t, r) {
@@ -19163,65 +19167,65 @@
                 b = w.type,
                 x = w.dataKey,
                 m = w.allowDataOverflow,
                 g = w.allowDuplicatedCategory,
                 O = w.scale,
                 A = w.ticks,
                 P = w.includeHidden,
-                T = v.props[o];
-            if (y[T]) return y;
-            var E = wo(t.data, {
+                E = v.props[o];
+            if (y[E]) return y;
+            var T = wo(t.data, {
                     graphicalItems: i.filter(function(U) {
-                        return U.props[o] === T
+                        return U.props[o] === E
                     }),
                     dataStartIndex: c,
                     dataEndIndex: s
                 }),
-                $ = E.length,
+                $ = T.length,
                 _, M, j;
-            fF(v.props.domain, m, b) && (_ = Bu(v.props.domain, null, m), p && (b === "number" || O !== "auto") && (j = On(E, x, "category")));
-            var k = Gy(b);
+            fF(v.props.domain, m, b) && (_ = Bu(v.props.domain, null, m), p && (b === "number" || O !== "auto") && (j = On(T, x, "category")));
+            var D = Gy(b);
             if (!_ || _.length === 0) {
-                var C, L = (C = v.props.domain) !== null && C !== void 0 ? C : k;
+                var C, L = (C = v.props.domain) !== null && C !== void 0 ? C : D;
                 if (x) {
-                    if (_ = On(E, x, b), b === "category" && p) {
-                        var R = E0(_);
-                        g && R ? (M = _, _ = Sa(0, $)) : g || (_ = Jf(L, _, v).reduce(function(U, ee) {
-                            return U.indexOf(ee) >= 0 ? U : [].concat(Wr(U), [ee])
+                    if (_ = On(T, x, b), b === "category" && p) {
+                        var B = E0(_);
+                        g && B ? (M = _, _ = Sa(0, $)) : g || (_ = Jf(L, _, v).reduce(function(U, Q) {
+                            return U.indexOf(Q) >= 0 ? U : [].concat(Wr(U), [Q])
                         }, []))
                     } else if (b === "category") g ? _ = _.filter(function(U) {
-                        return U !== "" && !X(U)
-                    }) : _ = Jf(L, _, v).reduce(function(U, ee) {
-                        return U.indexOf(ee) >= 0 || ee === "" || X(ee) ? U : [].concat(Wr(U), [ee])
+                        return U !== "" && !G(U)
+                    }) : _ = Jf(L, _, v).reduce(function(U, Q) {
+                        return U.indexOf(Q) >= 0 || Q === "" || G(Q) ? U : [].concat(Wr(U), [Q])
                     }, []);
                     else if (b === "number") {
-                        var F = II(E, i.filter(function(U) {
-                            return U.props[o] === T && (P || !U.props.hide)
+                        var W = II(T, i.filter(function(U) {
+                            return U.props[o] === E && (P || !U.props.hide)
                         }), x, a, f);
-                        F && (_ = F)
+                        W && (_ = W)
                     }
-                    p && (b === "number" || O !== "auto") && (j = On(E, x, "category"))
-                } else p ? _ = Sa(0, $) : u && u[T] && u[T].hasStack && b === "number" ? _ = h === "expand" ? [0, 1] : Xv(u[T].stackGroups, c, s) : _ = qv(E, i.filter(function(U) {
-                    return U.props[o] === T && (P || !U.props.hide)
+                    p && (b === "number" || O !== "auto") && (j = On(T, x, "category"))
+                } else p ? _ = Sa(0, $) : u && u[E] && u[E].hasStack && b === "number" ? _ = h === "expand" ? [0, 1] : Xv(u[E].stackGroups, c, s) : _ = qv(T, i.filter(function(U) {
+                    return U.props[o] === E && (P || !U.props.hide)
                 }), b, f, !0);
-                if (b === "number") _ = vc(l, _, T, a, A), L && (_ = Bu(L, _, m));
+                if (b === "number") _ = vc(l, _, E, a, A), L && (_ = Bu(L, _, m));
                 else if (b === "category" && L) {
                     var q = L,
                         Z = _.every(function(U) {
                             return q.indexOf(U) >= 0
                         });
                     Z && (_ = q)
                 }
             }
-            return I(I({}, y), {}, K({}, T, I(I({}, v.props), {}, {
+            return I(I({}, y), {}, K({}, E, I(I({}, v.props), {}, {
                 axisType: a,
                 domain: _,
                 categoricalDomain: j,
                 duplicateDomain: M,
-                originalDomain: (d = v.props.domain) !== null && d !== void 0 ? d : k,
+                originalDomain: (d = v.props.domain) !== null && d !== void 0 ? d : D,
                 isCategorical: p,
                 layout: f
             })))
         }, {})
     },
     BF = function(t, r) {
         var n = r.graphicalItems,
@@ -19269,15 +19273,15 @@
             a = r.AxisComp,
             o = r.graphicalItems,
             u = r.stackGroups,
             c = r.dataStartIndex,
             s = r.dataEndIndex,
             f = t.children,
             l = "".concat(i, "Id"),
-            h = Ne(f, a),
+            h = Le(f, a),
             p = {};
         return h && h.length ? p = LF(t, {
             axes: h,
             graphicalItems: o,
             axisType: i,
             axisIdKey: l,
             stackGroups: u,
@@ -19304,15 +19308,15 @@
             tooltipAxis: r,
             tooltipAxisBandSize: va(r, n)
         }
     },
     $p = function(t) {
         var r = t.children,
             n = t.defaultShowTooltip,
-            i = ze(r, Dr),
+            i = We(r, Dr),
             a = 0,
             o = 0;
         return t.data && t.data.length !== 0 && (o = t.data.length - 1), i && i.props && (i.props.startIndex >= 0 && (a = i.props.startIndex), i.props.endIndex >= 0 && (o = i.props.endIndex)), {
             chartX: 0,
             chartY: 0,
             dataStartIndex: a,
             dataEndIndex: o,
@@ -19348,16 +19352,16 @@
             o = a === void 0 ? {} : a,
             u = t.yAxisMap,
             c = u === void 0 ? {} : u,
             s = n.width,
             f = n.height,
             l = n.children,
             h = n.margin || {},
-            p = ze(l, Dr),
-            y = ze(l, Mn),
+            p = We(l, Dr),
+            y = We(l, Mn),
             v = Object.keys(c).reduce(function(g, O) {
                 var A = c[O],
                     P = A.orientation;
                 return !A.mirror && !A.hide ? I(I({}, g), {}, K({}, P, g[P] + A.width)) : g
             }, {
                 left: h.left || 0,
                 right: h.right || 0
@@ -19378,15 +19382,19 @@
         return I(I({
             brushBottom: b
         }, w), {}, {
             width: Math.max(x, 0),
             height: Math.max(m, 0)
         })
     },
-    UF = function(t) {
+    UF = function(t, r) {
+        if (r === "xAxis") return t[r].width;
+        if (r === "yAxis") return t[r].height
+    },
+    KF = function(t) {
         var r, n = t.chartName,
             i = t.GraphicalChild,
             a = t.defaultTooltipEventType,
             o = a === void 0 ? "axis" : a,
             u = t.validateTooltipEventTypes,
             c = u === void 0 ? ["axis"] : u,
             s = t.axisComponents,
@@ -19397,160 +19405,161 @@
                 var b = w.graphicalItems,
                     x = w.stackGroups,
                     m = w.offset,
                     g = w.updateId,
                     O = w.dataStartIndex,
                     A = w.dataEndIndex,
                     P = d.barSize,
-                    T = d.layout,
-                    E = d.barGap,
+                    E = d.layout,
+                    T = d.barGap,
                     $ = d.barCategoryGap,
                     _ = d.maxBarSize,
-                    M = Tp(T),
+                    M = Tp(E),
                     j = M.numericAxisName,
-                    k = M.cateAxisName,
+                    D = M.cateAxisName,
                     C = zF(b),
-                    L = C && EI({
-                        barSize: P,
-                        stackGroups: x
-                    }),
-                    R = [];
-                return b.forEach(function(F, q) {
-                    var Z = wo(d.data, {
-                            graphicalItems: [F],
+                    L = [];
+                return b.forEach(function(B, W) {
+                    var q = wo(d.data, {
+                            graphicalItems: [B],
                             dataStartIndex: O,
                             dataEndIndex: A
                         }),
-                        U = F.props,
-                        ee = U.dataKey,
-                        Te = U.maxBarSize,
-                        Ee = F.props["".concat(j, "Id")],
-                        Kt = F.props["".concat(k, "Id")],
-                        yt = {},
-                        Ke = s.reduce(function(qt, Ht) {
+                        Z = B.props,
+                        U = Z.dataKey,
+                        Q = Z.maxBarSize,
+                        _e = B.props["".concat(j, "Id")],
+                        ke = B.props["".concat(D, "Id")],
+                        Kt = {},
+                        De = s.reduce(function(qt, Ht) {
                             var Oo = w["".concat(Ht.axisType, "Map")],
-                                $s = F.props["".concat(Ht.axisType, "Id")];
-                            Oo && Oo[$s] || Ht.axisType === "zAxis" || ur(!1);
+                                $s = B.props["".concat(Ht.axisType, "Id")];
+                            Oo && Oo[$s] || Ht.axisType === "zAxis" || cr(!1);
                             var Ts = Oo[$s];
                             return I(I({}, qt), {}, K(K({}, Ht.axisType, Ts), "".concat(Ht.axisType, "Ticks"), wt(Ts)))
-                        }, yt),
-                        z = Ke[k],
-                        H = Ke["".concat(k, "Ticks")],
-                        J = x && x[Ee] && x[Ee].hasStack && qI(F, x[Ee].stackGroups),
-                        D = Ot(F.type).indexOf("Bar") >= 0,
-                        pe = va(z, H),
-                        Q = [];
-                    if (D) {
-                        var me, ve, Be = X(Te) ? _ : Te,
-                            mt = (me = (ve = va(z, H, !0)) !== null && ve !== void 0 ? ve : Be) !== null && me !== void 0 ? me : 0;
-                        Q = jI({
-                            barGap: E,
+                        }, Kt),
+                        yt = De[D],
+                        F = De["".concat(D, "Ticks")],
+                        X = x && x[_e] && x[_e].hasStack && qI(B, x[_e].stackGroups),
+                        J = Ot(B.type).indexOf("Bar") >= 0,
+                        k = va(yt, F),
+                        pe = [],
+                        re = C && EI({
+                            barSize: P,
+                            stackGroups: x,
+                            totalSize: UF(De, D)
+                        });
+                    if (J) {
+                        var me, ve, Re = G(Q) ? _ : Q,
+                            mt = (me = (ve = va(yt, F, !0)) !== null && ve !== void 0 ? ve : Re) !== null && me !== void 0 ? me : 0;
+                        pe = jI({
+                            barGap: T,
                             barCategoryGap: $,
-                            bandSize: mt !== pe ? mt : pe,
-                            sizeList: L[Kt],
-                            maxBarSize: Be
-                        }), mt !== pe && (Q = Q.map(function(qt) {
+                            bandSize: mt !== k ? mt : k,
+                            sizeList: re[ke],
+                            maxBarSize: Re
+                        }), mt !== k && (pe = pe.map(function(qt) {
                             return I(I({}, qt), {}, {
                                 position: I(I({}, qt.position), {}, {
                                     offset: qt.position.offset - mt / 2
                                 })
                             })
                         }))
                     }
-                    var Ai = F && F.type && F.type.getComposedData;
-                    Ai && R.push({
-                        props: I(I({}, Ai(I(I({}, Ke), {}, {
-                            displayedData: Z,
+                    var Ai = B && B.type && B.type.getComposedData;
+                    Ai && L.push({
+                        props: I(I({}, Ai(I(I({}, De), {}, {
+                            displayedData: q,
                             props: d,
-                            dataKey: ee,
-                            item: F,
-                            bandSize: pe,
-                            barPosition: Q,
+                            dataKey: U,
+                            item: B,
+                            bandSize: k,
+                            barPosition: pe,
                             offset: m,
-                            stackedData: J,
-                            layout: T,
+                            stackedData: X,
+                            layout: E,
                             dataStartIndex: O,
                             dataEndIndex: A
                         }))), {}, K(K(K({
-                            key: F.key || "item-".concat(q)
-                        }, j, Ke[j]), k, Ke[k]), "animationId", g)),
-                        childIndex: z0(F, d.children),
-                        item: F
+                            key: B.key || "item-".concat(W)
+                        }, j, De[j]), D, De[D]), "animationId", g)),
+                        childIndex: z0(B, d.children),
+                        item: B
                     })
-                }), R
+                }), L
             },
             y = function(d, w) {
                 var b = d.props,
                     x = d.dataStartIndex,
                     m = d.dataEndIndex,
                     g = d.updateId;
                 if (!Ws({
                         props: b
                     })) return null;
                 var O = b.children,
                     A = b.layout,
                     P = b.stackOffset,
-                    T = b.data,
-                    E = b.reverseStackOrder,
+                    E = b.data,
+                    T = b.reverseStackOrder,
                     $ = Tp(A),
                     _ = $.numericAxisName,
                     M = $.cateAxisName,
-                    j = Ne(O, i),
-                    k = WI(T, j, "".concat(_, "Id"), "".concat(M, "Id"), P, E),
+                    j = Le(O, i),
+                    D = WI(E, j, "".concat(_, "Id"), "".concat(M, "Id"), P, T),
                     C = s.reduce(function(Z, U) {
-                        var ee = "".concat(U.axisType, "Map");
-                        return I(I({}, Z), {}, K({}, ee, RF(b, I(I({}, U), {}, {
+                        var Q = "".concat(U.axisType, "Map");
+                        return I(I({}, Z), {}, K({}, Q, RF(b, I(I({}, U), {}, {
                             graphicalItems: j,
-                            stackGroups: U.axisType === _ && k,
+                            stackGroups: U.axisType === _ && D,
                             dataStartIndex: x,
                             dataEndIndex: m
                         }))))
                     }, {}),
                     L = WF(I(I({}, C), {}, {
                         props: b,
                         graphicalItems: j
                     }), w == null ? void 0 : w.legendBBox);
                 Object.keys(C).forEach(function(Z) {
                     C[Z] = l(b, C[Z], L, Z.replace("Map", ""), n)
                 });
-                var R = C["".concat(M, "Map")],
-                    F = FF(R),
+                var B = C["".concat(M, "Map")],
+                    W = FF(B),
                     q = p(b, I(I({}, C), {}, {
                         dataStartIndex: x,
                         dataEndIndex: m,
                         updateId: g,
                         graphicalItems: j,
-                        stackGroups: k,
+                        stackGroups: D,
                         offset: L
                     }));
                 return I(I({
                     formattedGraphicalItems: q,
                     graphicalItems: j,
                     offset: L,
-                    stackGroups: k
-                }, F), C)
+                    stackGroups: D
+                }, W), C)
             };
         return r = function(v) {
             TF(d, v);
 
             function d(w) {
                 var b, x, m;
                 return SF(this, d), m = _F(this, d, [w]), K(te(m), "eventEmitterSymbol", Symbol("rechartsEventEmitter")), K(te(m), "accessibilityManager", new lF), K(te(m), "handleLegendBBoxUpdate", function(g) {
                     if (g) {
                         var O = m.state,
                             A = O.dataStartIndex,
                             P = O.dataEndIndex,
-                            T = O.updateId;
+                            E = O.updateId;
                         m.setState(I({
                             legendBBox: g
                         }, y({
                             props: m.props,
                             dataStartIndex: A,
                             dataEndIndex: P,
-                            updateId: T
+                            updateId: E
                         }, I(I({}, m.state), {}, {
                             legendBBox: g
                         }))))
                     }
                 }), K(te(m), "handleReceiveSyncEvent", function(g, O, A) {
                     if (m.props.syncId === g) {
                         if (A === m.eventEmitterSymbol && typeof m.props.syncMethod != "function") return;
@@ -19624,16 +19633,16 @@
                     m.setState(O), m.triggerSyncEvent(O);
                     var A = m.props.onMouseLeave;
                     Y(A) && A(O, g)
                 }), K(te(m), "handleOuterEvent", function(g) {
                     var O = F0(g),
                         A = Ze(m.props, "".concat(O));
                     if (O && Y(A)) {
-                        var P, T;
-                        /.*touch.*/i.test(O) ? T = m.getMouseInfo(g.changedTouches[0]) : T = m.getMouseInfo(g), A((P = T) !== null && P !== void 0 ? P : {}, g)
+                        var P, E;
+                        /.*touch.*/i.test(O) ? E = m.getMouseInfo(g.changedTouches[0]) : E = m.getMouseInfo(g), A((P = E) !== null && P !== void 0 ? P : {}, g)
                     }
                 }), K(te(m), "handleClick", function(g) {
                     var O = m.getMouseInfo(g);
                     if (O) {
                         var A = I(I({}, O), {}, {
                             isTooltipActive: !0
                         });
@@ -19661,311 +19670,311 @@
                     g.changedTouches != null && g.changedTouches.length > 0 && m.handleMouseUp(g.changedTouches[0])
                 }), K(te(m), "triggerSyncEvent", function(g) {
                     m.props.syncId !== void 0 && Vo.emit(Yo, m.props.syncId, g, m.eventEmitterSymbol)
                 }), K(te(m), "applySyncEvent", function(g) {
                     var O = m.props,
                         A = O.layout,
                         P = O.syncMethod,
-                        T = m.state.updateId,
-                        E = g.dataStartIndex,
+                        E = m.state.updateId,
+                        T = g.dataStartIndex,
                         $ = g.dataEndIndex;
                     if (g.dataStartIndex !== void 0 || g.dataEndIndex !== void 0) m.setState(I({
-                        dataStartIndex: E,
+                        dataStartIndex: T,
                         dataEndIndex: $
                     }, y({
                         props: m.props,
-                        dataStartIndex: E,
+                        dataStartIndex: T,
                         dataEndIndex: $,
-                        updateId: T
+                        updateId: E
                     }, m.state)));
                     else if (g.activeTooltipIndex !== void 0) {
                         var _ = g.chartX,
                             M = g.chartY,
                             j = g.activeTooltipIndex,
-                            k = m.state,
-                            C = k.offset,
-                            L = k.tooltipTicks;
+                            D = m.state,
+                            C = D.offset,
+                            L = D.tooltipTicks;
                         if (!C) return;
                         if (typeof P == "function") j = P(L, g);
                         else if (P === "value") {
                             j = -1;
-                            for (var R = 0; R < L.length; R++)
-                                if (L[R].value === g.activeLabel) {
-                                    j = R;
+                            for (var B = 0; B < L.length; B++)
+                                if (L[B].value === g.activeLabel) {
+                                    j = B;
                                     break
                                 }
                         }
-                        var F = I(I({}, C), {}, {
+                        var W = I(I({}, C), {}, {
                                 x: C.left,
                                 y: C.top
                             }),
-                            q = Math.min(_, F.x + F.width),
-                            Z = Math.min(M, F.y + F.height),
+                            q = Math.min(_, W.x + W.width),
+                            Z = Math.min(M, W.y + W.height),
                             U = L[j] && L[j].value,
-                            ee = gc(m.state, m.props.data, j),
-                            Te = L[j] ? {
+                            Q = gc(m.state, m.props.data, j),
+                            _e = L[j] ? {
                                 x: A === "horizontal" ? L[j].coordinate : q,
                                 y: A === "horizontal" ? Z : L[j].coordinate
                             } : Hy;
                         m.setState(I(I({}, g), {}, {
                             activeLabel: U,
-                            activeCoordinate: Te,
-                            activePayload: ee,
+                            activeCoordinate: _e,
+                            activePayload: Q,
                             activeTooltipIndex: j
                         }))
                     } else m.setState(g)
                 }), K(te(m), "renderCursor", function(g) {
                     var O, A = m.state,
                         P = A.isTooltipActive,
-                        T = A.activeCoordinate,
-                        E = A.activePayload,
+                        E = A.activeCoordinate,
+                        T = A.activePayload,
                         $ = A.offset,
                         _ = A.activeTooltipIndex,
                         M = A.tooltipAxisBandSize,
                         j = m.getTooltipEventType(),
-                        k = (O = g.props.active) !== null && O !== void 0 ? O : P,
+                        D = (O = g.props.active) !== null && O !== void 0 ? O : P,
                         C = m.props.layout,
                         L = g.key || "_recharts-cursor";
                     return S.createElement(mF, {
                         key: L,
-                        activeCoordinate: T,
-                        activePayload: E,
+                        activeCoordinate: E,
+                        activePayload: T,
                         activeTooltipIndex: _,
                         chartName: n,
                         element: g,
-                        isActive: k,
+                        isActive: D,
                         layout: C,
                         offset: $,
                         tooltipAxisBandSize: M,
                         tooltipEventType: j
                     })
                 }), K(te(m), "renderPolarAxis", function(g, O, A) {
                     var P = Ze(g, "type.axisType"),
-                        T = Ze(m.state, "".concat(P, "Map")),
-                        E = T && T[g.props["".concat(P, "Id")]];
-                    return B.cloneElement(g, I(I({}, E), {}, {
-                        className: P,
+                        E = Ze(m.state, "".concat(P, "Map")),
+                        T = E && E[g.props["".concat(P, "Id")]];
+                    return R.cloneElement(g, I(I({}, T), {}, {
+                        className: ee(P, T.className),
                         key: g.key || "".concat(O, "-").concat(A),
-                        ticks: wt(E, !0)
+                        ticks: wt(T, !0)
                     }))
                 }), K(te(m), "renderPolarGrid", function(g) {
                     var O = g.props,
                         A = O.radialLines,
                         P = O.polarAngles,
-                        T = O.polarRadius,
-                        E = m.state,
-                        $ = E.radiusAxisMap,
-                        _ = E.angleAxisMap,
+                        E = O.polarRadius,
+                        T = m.state,
+                        $ = T.radiusAxisMap,
+                        _ = T.angleAxisMap,
                         M = kt($),
                         j = kt(_),
-                        k = j.cx,
+                        D = j.cx,
                         C = j.cy,
                         L = j.innerRadius,
-                        R = j.outerRadius;
-                    return B.cloneElement(g, {
-                        polarAngles: Array.isArray(P) ? P : wt(j, !0).map(function(F) {
-                            return F.coordinate
+                        B = j.outerRadius;
+                    return R.cloneElement(g, {
+                        polarAngles: Array.isArray(P) ? P : wt(j, !0).map(function(W) {
+                            return W.coordinate
                         }),
-                        polarRadius: Array.isArray(T) ? T : wt(M, !0).map(function(F) {
-                            return F.coordinate
+                        polarRadius: Array.isArray(E) ? E : wt(M, !0).map(function(W) {
+                            return W.coordinate
                         }),
-                        cx: k,
+                        cx: D,
                         cy: C,
                         innerRadius: L,
-                        outerRadius: R,
+                        outerRadius: B,
                         key: g.key || "polar-grid",
                         radialLines: A
                     })
                 }), K(te(m), "renderLegend", function() {
                     var g = m.state.formattedGraphicalItems,
                         O = m.props,
                         A = O.children,
                         P = O.width,
-                        T = O.height,
-                        E = m.props.margin || {},
-                        $ = P - (E.left || 0) - (E.right || 0),
+                        E = O.height,
+                        T = m.props.margin || {},
+                        $ = P - (T.left || 0) - (T.right || 0),
                         _ = Uv({
                             children: A,
                             formattedGraphicalItems: g,
                             legendWidth: $,
                             legendContent: f
                         });
                     if (!_) return null;
                     var M = _.item,
                         j = Ap(_, gF);
-                    return B.cloneElement(M, I(I({}, j), {}, {
+                    return R.cloneElement(M, I(I({}, j), {}, {
                         chartWidth: P,
-                        chartHeight: T,
-                        margin: E,
+                        chartHeight: E,
+                        margin: T,
                         onBBoxUpdate: m.handleLegendBBoxUpdate
                     }))
                 }), K(te(m), "renderTooltip", function() {
                     var g, O = m.props,
                         A = O.children,
                         P = O.accessibilityLayer,
-                        T = ze(A, gt);
-                    if (!T) return null;
-                    var E = m.state,
-                        $ = E.isTooltipActive,
-                        _ = E.activeCoordinate,
-                        M = E.activePayload,
-                        j = E.activeLabel,
-                        k = E.offset,
-                        C = (g = T.props.active) !== null && g !== void 0 ? g : $;
-                    return B.cloneElement(T, {
-                        viewBox: I(I({}, k), {}, {
-                            x: k.left,
-                            y: k.top
+                        E = We(A, gt);
+                    if (!E) return null;
+                    var T = m.state,
+                        $ = T.isTooltipActive,
+                        _ = T.activeCoordinate,
+                        M = T.activePayload,
+                        j = T.activeLabel,
+                        D = T.offset,
+                        C = (g = E.props.active) !== null && g !== void 0 ? g : $;
+                    return R.cloneElement(E, {
+                        viewBox: I(I({}, D), {}, {
+                            x: D.left,
+                            y: D.top
                         }),
                         active: C,
                         label: j,
                         payload: C ? M : [],
                         coordinate: _,
                         accessibilityLayer: P
                     })
                 }), K(te(m), "renderBrush", function(g) {
                     var O = m.props,
                         A = O.margin,
                         P = O.data,
-                        T = m.state,
-                        E = T.offset,
-                        $ = T.dataStartIndex,
-                        _ = T.dataEndIndex,
-                        M = T.updateId;
-                    return B.cloneElement(g, {
+                        E = m.state,
+                        T = E.offset,
+                        $ = E.dataStartIndex,
+                        _ = E.dataEndIndex,
+                        M = E.updateId;
+                    return R.cloneElement(g, {
                         key: g.key || "_recharts-brush",
                         onChange: Ii(m.handleBrushChange, g.props.onChange),
                         data: P,
-                        x: N(g.props.x) ? g.props.x : E.left,
-                        y: N(g.props.y) ? g.props.y : E.top + E.height + E.brushBottom - (A.bottom || 0),
-                        width: N(g.props.width) ? g.props.width : E.width,
+                        x: N(g.props.x) ? g.props.x : T.left,
+                        y: N(g.props.y) ? g.props.y : T.top + T.height + T.brushBottom - (A.bottom || 0),
+                        width: N(g.props.width) ? g.props.width : T.width,
                         startIndex: $,
                         endIndex: _,
                         updateId: "brush-".concat(M)
                     })
                 }), K(te(m), "renderReferenceElement", function(g, O, A) {
                     if (!g) return null;
                     var P = te(m),
-                        T = P.clipPathId,
-                        E = m.state,
-                        $ = E.xAxisMap,
-                        _ = E.yAxisMap,
-                        M = E.offset,
+                        E = P.clipPathId,
+                        T = m.state,
+                        $ = T.xAxisMap,
+                        _ = T.yAxisMap,
+                        M = T.offset,
                         j = g.props,
-                        k = j.xAxisId,
+                        D = j.xAxisId,
                         C = j.yAxisId;
-                    return B.cloneElement(g, {
+                    return R.cloneElement(g, {
                         key: g.key || "".concat(O, "-").concat(A),
-                        xAxis: $[k],
+                        xAxis: $[D],
                         yAxis: _[C],
                         viewBox: {
                             x: M.left,
                             y: M.top,
                             width: M.width,
                             height: M.height
                         },
-                        clipPathId: T
+                        clipPathId: E
                     })
                 }), K(te(m), "renderActivePoints", function(g) {
                     var O = g.item,
                         A = g.activePoint,
                         P = g.basePoint,
-                        T = g.childIndex,
-                        E = g.isRange,
+                        E = g.childIndex,
+                        T = g.isRange,
                         $ = [],
                         _ = O.props.key,
                         M = O.item.props,
                         j = M.activeDot,
-                        k = M.dataKey,
+                        D = M.dataKey,
                         C = I(I({
-                            index: T,
-                            dataKey: k,
+                            index: E,
+                            dataKey: D,
                             cx: A.x,
                             cy: A.y,
                             r: 4,
                             fill: vs(O.item),
                             strokeWidth: 2,
                             stroke: "#fff",
                             payload: A.payload,
                             value: A.value,
-                            key: "".concat(_, "-activePoint-").concat(T)
-                        }, G(j, !1)), Wi(j));
+                            key: "".concat(_, "-activePoint-").concat(E)
+                        }, H(j, !1)), Wi(j));
                     return $.push(d.renderActiveDot(j, C)), P ? $.push(d.renderActiveDot(j, I(I({}, C), {}, {
                         cx: P.x,
                         cy: P.y,
-                        key: "".concat(_, "-basePoint-").concat(T)
-                    }))) : E && $.push(null), $
+                        key: "".concat(_, "-basePoint-").concat(E)
+                    }))) : T && $.push(null), $
                 }), K(te(m), "renderGraphicChild", function(g, O, A) {
                     var P = m.filterFormatItem(g, O, A);
                     if (!P) return null;
-                    var T = m.getTooltipEventType(),
-                        E = m.state,
-                        $ = E.isTooltipActive,
-                        _ = E.tooltipAxis,
-                        M = E.activeTooltipIndex,
-                        j = E.activeLabel,
-                        k = m.props.children,
-                        C = ze(k, gt),
+                    var E = m.getTooltipEventType(),
+                        T = m.state,
+                        $ = T.isTooltipActive,
+                        _ = T.tooltipAxis,
+                        M = T.activeTooltipIndex,
+                        j = T.activeLabel,
+                        D = m.props.children,
+                        C = We(D, gt),
                         L = P.props,
-                        R = L.points,
-                        F = L.isRange,
+                        B = L.points,
+                        W = L.isRange,
                         q = L.baseLine,
                         Z = P.item.props,
                         U = Z.activeDot,
-                        ee = Z.hide,
-                        Te = Z.activeBar,
-                        Ee = Z.activeShape,
-                        Kt = !!(!ee && $ && C && (U || Te || Ee)),
-                        yt = {};
-                    T !== "axis" && C && C.props.trigger === "click" ? yt = {
+                        Q = Z.hide,
+                        _e = Z.activeBar,
+                        ke = Z.activeShape,
+                        Kt = !!(!Q && $ && C && (U || _e || ke)),
+                        De = {};
+                    E !== "axis" && C && C.props.trigger === "click" ? De = {
                         onClick: Ii(m.handleItemMouseEnter, g.props.onClick)
-                    } : T !== "axis" && (yt = {
+                    } : E !== "axis" && (De = {
                         onMouseLeave: Ii(m.handleItemMouseLeave, g.props.onMouseLeave),
                         onMouseEnter: Ii(m.handleItemMouseEnter, g.props.onMouseEnter)
                     });
-                    var Ke = B.cloneElement(g, I(I({}, P.props), yt));
+                    var yt = R.cloneElement(g, I(I({}, P.props), De));
 
-                    function z(Ht) {
+                    function F(Ht) {
                         return typeof _.dataKey == "function" ? _.dataKey(Ht.payload) : null
                     }
                     if (Kt)
                         if (M >= 0) {
-                            var H, J;
+                            var X, J;
                             if (_.dataKey && !_.allowDuplicatedCategory) {
-                                var D = typeof _.dataKey == "function" ? z : "payload.".concat(_.dataKey.toString());
-                                H = zi(R, D, j), J = F && q && zi(q, D, j)
-                            } else H = R == null ? void 0 : R[M], J = F && q && q[M];
-                            if (Ee || Te) {
+                                var k = typeof _.dataKey == "function" ? F : "payload.".concat(_.dataKey.toString());
+                                X = zi(B, k, j), J = W && q && zi(q, k, j)
+                            } else X = B == null ? void 0 : B[M], J = W && q && q[M];
+                            if (ke || _e) {
                                 var pe = g.props.activeIndex !== void 0 ? g.props.activeIndex : M;
-                                return [B.cloneElement(g, I(I(I({}, P.props), yt), {}, {
+                                return [R.cloneElement(g, I(I(I({}, P.props), De), {}, {
                                     activeIndex: pe
                                 })), null, null]
                             }
-                            if (!X(H)) return [Ke].concat(Wr(m.renderActivePoints({
+                            if (!G(X)) return [yt].concat(Wr(m.renderActivePoints({
                                 item: P,
-                                activePoint: H,
+                                activePoint: X,
                                 basePoint: J,
                                 childIndex: M,
-                                isRange: F
+                                isRange: W
                             })))
                         } else {
-                            var Q, me = (Q = m.getItemByXY(m.state.activeCoordinate)) !== null && Q !== void 0 ? Q : {
-                                    graphicalItem: Ke
+                            var re, me = (re = m.getItemByXY(m.state.activeCoordinate)) !== null && re !== void 0 ? re : {
+                                    graphicalItem: yt
                                 },
                                 ve = me.graphicalItem,
-                                Be = ve.item,
-                                mt = Be === void 0 ? g : Be,
+                                Re = ve.item,
+                                mt = Re === void 0 ? g : Re,
                                 Ai = ve.childIndex,
-                                qt = I(I(I({}, P.props), yt), {}, {
+                                qt = I(I(I({}, P.props), De), {}, {
                                     activeIndex: Ai
                                 });
-                            return [B.cloneElement(mt, qt), null, null]
-                        } return F ? [Ke, null, null] : [Ke, null]
+                            return [R.cloneElement(mt, qt), null, null]
+                        } return W ? [yt, null, null] : [yt, null]
                 }), K(te(m), "renderCustomized", function(g, O, A) {
-                    return B.cloneElement(g, I(I({
+                    return R.cloneElement(g, I(I({
                         key: "recharts-customized-".concat(A)
                     }, m.props), m.state))
                 }), K(te(m), "renderMap", {
                     CartesianGrid: {
                         handler: Bi,
                         once: !0
                     },
@@ -20025,15 +20034,15 @@
                     },
                     PolarRadiusAxis: {
                         handler: m.renderPolarAxis
                     },
                     Customized: {
                         handler: m.renderCustomized
                     }
-                }), m.clipPathId = "".concat((b = w.id) !== null && b !== void 0 ? b : lr("recharts"), "-clip"), m.throttleTriggeredAfterMouseMove = Hd(m.triggeredAfterMouseMove, (x = w.throttleDelay) !== null && x !== void 0 ? x : 1e3 / 60), m.state = {}, m
+                }), m.clipPathId = "".concat((b = w.id) !== null && b !== void 0 ? b : fr("recharts"), "-clip"), m.throttleTriggeredAfterMouseMove = Hd(m.triggeredAfterMouseMove, (x = w.throttleDelay) !== null && x !== void 0 ? x : 1e3 / 60), m.state = {}, m
             }
             return PF(d, [{
                 key: "componentDidMount",
                 value: function() {
                     var b, x;
                     this.addListener(), this.accessibilityManager.setDetails({
                         container: this.container,
@@ -20050,40 +20059,40 @@
                 key: "displayDefaultTooltip",
                 value: function() {
                     var b = this.props,
                         x = b.children,
                         m = b.data,
                         g = b.height,
                         O = b.layout,
-                        A = ze(x, gt);
+                        A = We(x, gt);
                     if (A) {
                         var P = A.props.defaultIndex;
                         if (!(typeof P != "number" || P < 0 || P > this.state.tooltipTicks.length)) {
-                            var T = this.state.tooltipTicks[P] && this.state.tooltipTicks[P].value,
-                                E = gc(this.state, m, P, T),
+                            var E = this.state.tooltipTicks[P] && this.state.tooltipTicks[P].value,
+                                T = gc(this.state, m, P, E),
                                 $ = this.state.tooltipTicks[P].coordinate,
                                 _ = (this.state.offset.top + g) / 2,
                                 M = O === "horizontal",
                                 j = M ? {
                                     x: $,
                                     y: _
                                 } : {
                                     y: $,
                                     x: _
                                 },
-                                k = this.state.formattedGraphicalItems.find(function(L) {
-                                    var R = L.item;
-                                    return R.type.name === "Scatter"
+                                D = this.state.formattedGraphicalItems.find(function(L) {
+                                    var B = L.item;
+                                    return B.type.name === "Scatter"
                                 });
-                            k && (j = I(I({}, j), k.props.points[P].tooltipPosition), E = k.props.points[P].tooltipPayload);
+                            D && (j = I(I({}, j), D.props.points[P].tooltipPosition), T = D.props.points[P].tooltipPayload);
                             var C = {
                                 activeTooltipIndex: P,
                                 isTooltipActive: !0,
-                                activeLabel: T,
-                                activePayload: E,
+                                activeLabel: E,
+                                activePayload: T,
                                 activeCoordinate: j
                             };
                             this.setState(C), this.renderCursor(A), this.accessibilityManager.setIndex(P)
                         }
                     }
                 }
             }, {
@@ -20104,25 +20113,25 @@
                         })
                     }
                     return null
                 }
             }, {
                 key: "componentDidUpdate",
                 value: function(b) {
-                    tu([ze(b.children, gt)], [ze(this.props.children, gt)]) || this.displayDefaultTooltip()
+                    tu([We(b.children, gt)], [We(this.props.children, gt)]) || this.displayDefaultTooltip()
                 }
             }, {
                 key: "componentWillUnmount",
                 value: function() {
                     this.removeListener(), this.throttleTriggeredAfterMouseMove.cancel()
                 }
             }, {
                 key: "getTooltipEventType",
                 value: function() {
-                    var b = ze(this.props.children, gt);
+                    var b = We(this.props.children, gt);
                     if (b && typeof b.props.shared == "boolean") {
                         var x = b.props.shared ? "axis" : "item";
                         return c.indexOf(x) >= 0 ? x : o
                     }
                     return o
                 }
             }, {
@@ -20135,25 +20144,25 @@
                         O = {
                             chartX: Math.round(b.pageX - g.left),
                             chartY: Math.round(b.pageY - g.top)
                         },
                         A = m.width / x.offsetWidth || 1,
                         P = this.inRange(O.chartX, O.chartY, A);
                     if (!P) return null;
-                    var T = this.state,
-                        E = T.xAxisMap,
-                        $ = T.yAxisMap,
+                    var E = this.state,
+                        T = E.xAxisMap,
+                        $ = E.yAxisMap,
                         _ = this.getTooltipEventType();
-                    if (_ !== "axis" && E && $) {
-                        var M = kt(E).scale,
+                    if (_ !== "axis" && T && $) {
+                        var M = kt(T).scale,
                             j = kt($).scale,
-                            k = M && M.invert ? M.invert(O.chartX) : null,
+                            D = M && M.invert ? M.invert(O.chartX) : null,
                             C = j && j.invert ? j.invert(O.chartY) : null;
                         return I(I({}, O), {}, {
-                            xValue: k,
+                            xValue: D,
                             yValue: C
                         })
                     }
                     var L = _p(this.state, this.props.data, this.props.layout, P);
                     return L ? I(I({}, O), L) : null
                 }
             }, {
@@ -20161,38 +20170,38 @@
                 value: function(b, x) {
                     var m = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1,
                         g = this.props.layout,
                         O = b / m,
                         A = x / m;
                     if (g === "horizontal" || g === "vertical") {
                         var P = this.state.offset,
-                            T = O >= P.left && O <= P.left + P.width && A >= P.top && A <= P.top + P.height;
-                        return T ? {
+                            E = O >= P.left && O <= P.left + P.width && A >= P.top && A <= P.top + P.height;
+                        return E ? {
                             x: O,
                             y: A
                         } : null
                     }
-                    var E = this.state,
-                        $ = E.angleAxisMap,
-                        _ = E.radiusAxisMap;
+                    var T = this.state,
+                        $ = T.angleAxisMap,
+                        _ = T.radiusAxisMap;
                     if ($ && _) {
                         var M = kt($);
                         return th({
                             x: O,
                             y: A
                         }, M)
                     }
                     return null
                 }
             }, {
                 key: "parseEventsOfWrapper",
                 value: function() {
                     var b = this.props.children,
                         x = this.getTooltipEventType(),
-                        m = ze(b, gt),
+                        m = We(b, gt),
                         g = {};
                     m && x === "axis" && (m.props.trigger === "click" ? g = {
                         onClick: this.handleClick
                     } : g = {
                         onMouseEnter: this.handleMouseEnter,
                         onMouseMove: this.handleMouseMove,
                         onMouseLeave: this.handleMouseLeave,
@@ -20279,115 +20288,113 @@
                 value: function(b) {
                     var x = this.state,
                         m = x.formattedGraphicalItems,
                         g = x.activeItem;
                     if (m && m.length)
                         for (var O = 0, A = m.length; O < A; O++) {
                             var P = m[O],
-                                T = P.props,
-                                E = P.item,
-                                $ = Ot(E.type);
+                                E = P.props,
+                                T = P.item,
+                                $ = Ot(T.type);
                             if ($ === "Bar") {
-                                var _ = (T.data || []).find(function(C) {
+                                var _ = (E.data || []).find(function(C) {
                                     return PD(b, C)
                                 });
                                 if (_) return {
                                     graphicalItem: P,
                                     payload: _
                                 }
                             } else if ($ === "RadialBar") {
-                                var M = (T.data || []).find(function(C) {
+                                var M = (E.data || []).find(function(C) {
                                     return th(b, C)
                                 });
                                 if (M) return {
                                     graphicalItem: P,
                                     payload: M
                                 }
                             } else if (vo(P, g) || yo(P, g) || ii(P, g)) {
                                 var j = $N({
                                         graphicalItem: P,
                                         activeTooltipItem: g,
-                                        itemData: E.props.data
+                                        itemData: T.props.data
                                     }),
-                                    k = E.props.activeIndex === void 0 ? j : E.props.activeIndex;
+                                    D = T.props.activeIndex === void 0 ? j : T.props.activeIndex;
                                 return {
                                     graphicalItem: I(I({}, P), {}, {
-                                        childIndex: k
+                                        childIndex: D
                                     }),
-                                    payload: ii(P, g) ? E.props.data[j] : P.props.data[j]
+                                    payload: ii(P, g) ? T.props.data[j] : P.props.data[j]
                                 }
                             }
                         }
                     return null
                 }
             }, {
                 key: "render",
                 value: function() {
-                    var b = this,
-                        x;
+                    var b = this;
                     if (!Ws(this)) return null;
-                    var m = this.props,
-                        g = m.children,
-                        O = m.className,
-                        A = m.width,
-                        P = m.height,
-                        T = m.style,
-                        E = m.compact,
-                        $ = m.title,
-                        _ = m.desc,
-                        M = Ap(m, bF),
-                        j = G(M, !1);
+                    var x = this.props,
+                        m = x.children,
+                        g = x.className,
+                        O = x.width,
+                        A = x.height,
+                        P = x.style,
+                        E = x.compact,
+                        T = x.title,
+                        $ = x.desc,
+                        _ = Ap(x, bF),
+                        M = H(_, !1);
                     if (E) return S.createElement(ep, {
                         state: this.state,
                         width: this.props.width,
                         height: this.props.height,
                         clipPathId: this.clipPathId
-                    }, S.createElement(nu, $n({}, j, {
-                        width: A,
-                        height: P,
-                        title: $,
-                        desc: _
-                    }), this.renderClipPath(), Ks(g, this.renderMap)));
+                    }, S.createElement(nu, $n({}, M, {
+                        width: O,
+                        height: A,
+                        title: T,
+                        desc: $
+                    }), this.renderClipPath(), Ks(m, this.renderMap)));
                     if (this.props.accessibilityLayer) {
-                        var k, C;
-                        j.tabIndex = (k = this.props.tabIndex) !== null && k !== void 0 ? k : 0, j.role = (C = this.props.role) !== null && C !== void 0 ? C : "application", j.onKeyDown = function(R) {
-                            b.accessibilityManager.keyboardEvent(R)
-                        }, j.onFocus = function() {
+                        var j, D;
+                        M.tabIndex = (j = this.props.tabIndex) !== null && j !== void 0 ? j : 0, M.role = (D = this.props.role) !== null && D !== void 0 ? D : "application", M.onKeyDown = function(L) {
+                            b.accessibilityManager.keyboardEvent(L)
+                        }, M.onFocus = function() {
                             b.accessibilityManager.focus()
                         }
                     }
-                    var L = this.parseEventsOfWrapper();
+                    var C = this.parseEventsOfWrapper();
                     return S.createElement(ep, {
                         state: this.state,
                         width: this.props.width,
                         height: this.props.height,
                         clipPathId: this.clipPathId
                     }, S.createElement("div", $n({
-                        className: re("recharts-wrapper", O),
+                        className: ee("recharts-wrapper", g),
                         style: I({
                             position: "relative",
                             cursor: "default",
-                            width: A,
-                            height: P
-                        }, T)
-                    }, L, {
-                        ref: function(F) {
-                            b.container = F
-                        },
-                        role: (x = j.role) !== null && x !== void 0 ? x : "region"
-                    }), S.createElement(nu, $n({}, j, {
-                        width: A,
-                        height: P,
-                        title: $,
-                        desc: _,
+                            width: O,
+                            height: A
+                        }, P)
+                    }, C, {
+                        ref: function(B) {
+                            b.container = B
+                        }
+                    }), S.createElement(nu, $n({}, M, {
+                        width: O,
+                        height: A,
+                        title: T,
+                        desc: $,
                         style: kF
-                    }), this.renderClipPath(), Ks(g, this.renderMap)), this.renderLegend(), this.renderTooltip()))
+                    }), this.renderClipPath(), Ks(m, this.renderMap)), this.renderLegend(), this.renderTooltip()))
                 }
             }]), d
-        }(B.Component), K(r, "displayName", n), K(r, "defaultProps", I({
+        }(R.Component), K(r, "displayName", n), K(r, "defaultProps", I({
             layout: "horizontal",
             stackOffset: "none",
             barCategoryGap: "10%",
             barGap: 4,
             margin: {
                 top: 5,
                 right: 5,
@@ -20401,16 +20408,16 @@
                 b = v.data,
                 x = v.children,
                 m = v.width,
                 g = v.height,
                 O = v.layout,
                 A = v.stackOffset,
                 P = v.margin,
-                T = d.dataStartIndex,
-                E = d.dataEndIndex;
+                E = d.dataStartIndex,
+                T = d.dataEndIndex;
             if (d.updateId === void 0) {
                 var $ = $p(v);
                 return I(I(I({}, $), {}, {
                     updateId: 0
                 }, y(I(I({
                     props: v
                 }, $), {}, {
@@ -20422,79 +20429,79 @@
                     prevHeight: g,
                     prevLayout: O,
                     prevStackOffset: A,
                     prevMargin: P,
                     prevChildren: x
                 })
             }
-            if (w !== d.prevDataKey || b !== d.prevData || m !== d.prevWidth || g !== d.prevHeight || O !== d.prevLayout || A !== d.prevStackOffset || !xr(P, d.prevMargin)) {
+            if (w !== d.prevDataKey || b !== d.prevData || m !== d.prevWidth || g !== d.prevHeight || O !== d.prevLayout || A !== d.prevStackOffset || !wr(P, d.prevMargin)) {
                 var _ = $p(v),
                     M = {
                         chartX: d.chartX,
                         chartY: d.chartY,
                         isTooltipActive: d.isTooltipActive
                     },
                     j = I(I({}, _p(d, b, O)), {}, {
                         updateId: d.updateId + 1
                     }),
-                    k = I(I(I({}, _), M), j);
-                return I(I(I({}, k), y(I({
+                    D = I(I(I({}, _), M), j);
+                return I(I(I({}, D), y(I({
                     props: v
-                }, k), d)), {}, {
+                }, D), d)), {}, {
                     prevDataKey: w,
                     prevData: b,
                     prevWidth: m,
                     prevHeight: g,
                     prevLayout: O,
                     prevStackOffset: A,
                     prevMargin: P,
                     prevChildren: x
                 })
             }
             if (!tu(x, d.prevChildren)) {
-                var C, L, R, F, q = ze(x, Dr),
-                    Z = q && (C = (L = q.props) === null || L === void 0 ? void 0 : L.startIndex) !== null && C !== void 0 ? C : T,
-                    U = q && (R = (F = q.props) === null || F === void 0 ? void 0 : F.endIndex) !== null && R !== void 0 ? R : E,
-                    ee = Z !== T || U !== E,
-                    Te = !X(b),
-                    Ee = Te && !ee ? d.updateId : d.updateId + 1;
+                var C, L, B, W, q = We(x, Dr),
+                    Z = q && (C = (L = q.props) === null || L === void 0 ? void 0 : L.startIndex) !== null && C !== void 0 ? C : E,
+                    U = q && (B = (W = q.props) === null || W === void 0 ? void 0 : W.endIndex) !== null && B !== void 0 ? B : T,
+                    Q = Z !== E || U !== T,
+                    _e = !G(b),
+                    ke = _e && !Q ? d.updateId : d.updateId + 1;
                 return I(I({
-                    updateId: Ee
+                    updateId: ke
                 }, y(I(I({
                     props: v
                 }, d), {}, {
-                    updateId: Ee,
+                    updateId: ke,
                     dataStartIndex: Z,
                     dataEndIndex: U
                 }), d)), {}, {
                     prevChildren: x,
                     dataStartIndex: Z,
                     dataEndIndex: U
                 })
             }
             return null
         }), K(r, "renderActiveDot", function(v, d) {
             var w;
-            return B.isValidElement(v) ? w = B.cloneElement(v, d) : Y(v) ? w = v(d) : w = S.createElement(po, d), S.createElement(ie, {
+            return R.isValidElement(v) ? w = R.cloneElement(v, d) : Y(v) ? w = v(d) : w = S.createElement(po, d), S.createElement(ie, {
                 className: "recharts-active-dot",
                 key: d.key
             }, w)
         }), r
     },
-    GF = UF({
+    XF = KF({
         chartName: "ComposedChart",
-        GraphicalChild: [go, pr, nn, xo],
+        GraphicalChild: [go, dr, nn, xo],
         axisComponents: [{
             axisType: "xAxis",
             AxisComp: Ps
         }, {
             axisType: "yAxis",
             AxisComp: _s
         }, {
             axisType: "zAxis",
             AxisComp: bo
         }],
         formatAxisMap: YL
     });
 export {
-    nn as B, GF as C, Mn as L, qF as R, gt as T, Ps as X, _s as Y, HF as _, OR as a, go as b, Jo as r
+    nn as B, XF as C, Mn as L, HF as R, gt as T, Ps as X, _s as Y, GF as _, OR as a, go as b, Jo as r
 };
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/sentry-B_MfAkLS.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/sentry-DxJl7iQ9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1658,15 +1658,15 @@
 
 function Ft() {
     return {
         traceId: E(),
         spanId: E().substring(16)
     }
 }
-const dr = "7.109.0",
+const dr = "7.110.0",
     de = parseFloat(dr),
     pr = 100;
 class pe {
     constructor(t, n, r, o = de) {
         this._version = o;
         let i;
         n ? i = n : (i = new R, i.setClient(t));
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/syntaxHighlighter-D1hpWw2Q.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/syntaxHighlighter-CEoW8GyI.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as _n
-} from "./recharts-9OgIHZXS.js";
+} from "./recharts-BzBtiWsS.js";
 import {
     a as J,
     c as ye,
     g as zn
 } from "./react-vbD531y6.js";
 import {
     _ as Un
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/assets/ui-Bo7CIhws.js` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/assets/ui-DM1JZie1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     r as It
-} from "./recharts-9OgIHZXS.js";
+} from "./recharts-BzBtiWsS.js";
 import {
     r as u,
     e as be,
     a as O
 } from "./react-vbD531y6.js";
 
 function kt(e) {
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/harp.svg` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/harp.svg`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/dashboard/web/index.html` & `harp_proxy-0.5.0b6/harp_apps/dashboard/web/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 <html lang="en">
   <head>
     <meta charset="UTF-8" />
 
     <link rel="icon" type="image/svg+xml" href="/harp.svg" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Harp UI</title>
-    <script type="module" crossorigin src="/assets/index-pKJQAlqa.js"></script>
+    <script type="module" crossorigin src="/assets/index-CKrV6JKW.js"></script>
     <link rel="modulepreload" crossorigin href="/assets/react-vbD531y6.js">
     <link rel="modulepreload" crossorigin href="/assets/reactQuery-BTfpiMem.js">
     <link rel="modulepreload" crossorigin href="/assets/reactRouter-iI7EIT1e.js">
-    <link rel="modulepreload" crossorigin href="/assets/recharts-9OgIHZXS.js">
-    <link rel="modulepreload" crossorigin href="/assets/ui-Bo7CIhws.js">
-    <link rel="modulepreload" crossorigin href="/assets/sentry-B_MfAkLS.js">
+    <link rel="modulepreload" crossorigin href="/assets/recharts-BzBtiWsS.js">
+    <link rel="modulepreload" crossorigin href="/assets/ui-DM1JZie1.js">
+    <link rel="modulepreload" crossorigin href="/assets/sentry-DxJl7iQ9.js">
     <link rel="modulepreload" crossorigin href="/assets/dateFns-s2EURlY7.js">
-    <link rel="modulepreload" crossorigin href="/assets/syntaxHighlighter-D1hpWw2Q.js">
-    <link rel="stylesheet" crossorigin href="/assets/index-BOfsip6N.css">
+    <link rel="modulepreload" crossorigin href="/assets/syntaxHighlighter-CEoW8GyI.js">
+    <link rel="stylesheet" crossorigin href="/assets/index-sYClmDC3.css">
   </head>
   <body>
     <div id="root"></div>
   </body>
 </html>
```

### Comparing `harp_proxy-0.5.0b5/harp_apps/http_client/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/http_client/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/janitor/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/janitor/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/janitor/tests/test_worker.py` & `harp_proxy-0.5.0b6/harp_apps/janitor/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/janitor/worker.py` & `harp_proxy-0.5.0b6/harp_apps/janitor/worker.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/proxy/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/proxy/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/proxy/controllers.py` & `harp_proxy-0.5.0b6/harp_apps/proxy/controllers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/proxy/docs/index.rst` & `harp_proxy-0.5.0b6/harp_apps/proxy/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/proxy/settings.py` & `harp_proxy-0.5.0b6/harp_apps/proxy/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/proxy/tests/test_controllers_http_proxy.py` & `harp_proxy-0.5.0b6/harp_apps/proxy/tests/test_controllers_http_proxy.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/docs/index.rst` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/__init__.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/base.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/blobs.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/flags.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/flags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/messages.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/messages.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/metrics.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/metrics.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/tags.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/tags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/transactions.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/models/users.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/models/users.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/settings.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/storage.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/storage.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_application.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_models_base.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_models_base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/dates.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/sqlalchemy_storage/utils/testing/mixins.py` & `harp_proxy-0.5.0b6/harp_apps/sqlalchemy_storage/utils/testing/mixins.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/telemetry/__app__.py` & `harp_proxy-0.5.0b6/harp_apps/telemetry/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/telemetry/manager.py` & `harp_proxy-0.5.0b6/harp_apps/telemetry/manager.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/harp_apps/telemetry/tests/test_manager.py` & `harp_proxy-0.5.0b6/harp_apps/telemetry/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b5/pyproject.toml` & `harp_proxy-0.5.0b6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "harp-proxy"
-version = "0.5.0b5"
+version = "0.5.0b6"
 description = "Harp is an API Runtime Proxy – A toolkit for Fast, Reliable and Observable external APIs"
 authors = ["Romain Dorgueil <romain@makersquad.fr>"]
 readme = "README.rst"
 packages = [
     { include = "harp" },
     { include = "harp_apps" },
 ]
+exclude = ["**/node_modules/", "harp_apps/dashboard/frontend", ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-aiohttp = "^3.9.3"
+python = "^3.12"
+aiohttp = "^3.9.4"
 aiosqlite = ">=0.19,<0.21"
-anyio = "^4.3.0"
+anyio = "^4.4.0"
 asgimiddlewarestaticfile = "^0.6.0"
 asgiref = "^3.8.1"
 asyncpg = "^0.29.0"
 dataclasses-json = "^0.6.3"
 dataclasses-jsonschema = "^2.16.0"
 essentials-configuration = "^2.0.4"
-hishel = ">=0.0.21,<0.0.26"
+hishel = ">=0.0.21,<0.0.27"
 honcho = { version = "^1.1.0", optional = true }
 http-router = "^4.1.2"
 httpx = ">=0.26,<0.28"
-hypercorn = "^0.16.0"
+hypercorn = "^0.17.2"
 multidict = "^6.0.5"
 orjson = "^3.10.0"
 passlib = "^1.7.4"
 psycopg2-binary = "^2.9.9"
 pyyaml = "^6.0.1"
 rich = "^13.7.1"
 rich-click = "^1.7.4"
 rodi = "^2.0.6"
-sentry-sdk = "^1.44.0"
+sentry-sdk = "^2.3.1"
 sqlalchemy = { extras = ["asyncio"], version = "^2.0.29" }
 sqlalchemy-utils = "^0.41.1"
-structlog = "^24.1.0"
+structlog = "^24.2.0"
 svix-ksuid = "^0.6.2"
-watchfiles = { version = "^0.21.0", optional = true }
+watchfiles = { version = "^0.22.0", optional = true }
 whistle = { version = "2.0.0a1", allow-prereleases = true }
 
 
 [tool.poetry.group.dev.dependencies]
 asgi-tools = "^0.76.0"
 black = ">=23.12,<25.0"
 furo = ">=2023.9.10,<2025.0.0"
 isort = "^5.13.2"
 pre-commit = "^3.7.0"
 pytest = ">=7.4.3,<9.0.0"
-pytest-asyncio = "^0.21.1" # 0.23 breaks the test suite (https://github.com/pytest-dev/pytest-asyncio/releases/tag/v0.23.0)
+pytest-asyncio = ">=0.21.1,<0.23.0" # 0.23 breaks the test suite (https://github.com/pytest-dev/pytest-asyncio/releases/tag/v0.23.0)
 respx = ">=0.20.2,<0.22.0"
 sphinx = "^7.2.6"
 sphinx-autobuild = ">=2021.3.14,<2025.0.0"
 sphinx-design = "^0.5.0"
 sphinxcontrib-jquery = "^4.1"
 pytest-benchmark = { extras = ["histogram"], version = "^4.0.0" }
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 sphinx-copybutton = "^0.5.2"
 sphinx-sitemap = "^2.5.1"
-ruff = "^0.1.9"
-pytest-xdist = {version = "^3.5.0", extras = ["psutil"]}
+ruff = ">=0.1.9,<0.4.0"
+pytest-xdist = { version = "^3.5.0", extras = ["psutil"] }
 freezegun = "^1.4.0"
-testcontainers = {extras = ["postgres"], version = ">=3.7.1,<5.0.0"}
+testcontainers = { extras = ["postgres"], version = ">=4.3.0,<4.4" }
 sphinx-click = "^5.1.0"
 
 
 [tool.poetry.group.mysql.dependencies]
 asyncmy = "^0.2.9"
 aiomysql = "^0.2.0"
 cryptography = ">=41.0.7,<43.0.0"
```

### Comparing `harp_proxy-0.5.0b5/PKG-INFO` & `harp_proxy-0.5.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: harp-proxy
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Harp is an API Runtime Proxy – A toolkit for Fast, Reliable and Observable external APIs
 Author: Romain Dorgueil
 Author-email: romain@makersquad.fr
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
-Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiosqlite (>=0.19,<0.21)
-Requires-Dist: anyio (>=4.3.0,<5.0.0)
+Requires-Dist: anyio (>=4.4.0,<5.0.0)
 Requires-Dist: asgimiddlewarestaticfile (>=0.6.0,<0.7.0)
 Requires-Dist: asgiref (>=3.8.1,<4.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
 Requires-Dist: dataclasses-jsonschema (>=2.16.0,<3.0.0)
 Requires-Dist: essentials-configuration (>=2.0.4,<3.0.0)
-Requires-Dist: hishel (>=0.0.21,<0.0.26)
+Requires-Dist: hishel (>=0.0.21,<0.0.27)
 Requires-Dist: honcho (>=1.1.0,<2.0.0) ; extra == "dev"
 Requires-Dist: http-router (>=4.1.2,<5.0.0)
 Requires-Dist: httpx (>=0.26,<0.28)
-Requires-Dist: hypercorn (>=0.16.0,<0.17.0)
+Requires-Dist: hypercorn (>=0.17.2,<0.18.0)
 Requires-Dist: multidict (>=6.0.5,<7.0.0)
 Requires-Dist: orjson (>=3.10.0,<4.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rich-click (>=1.7.4,<2.0.0)
 Requires-Dist: rodi (>=2.0.6,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.44.0,<2.0.0)
+Requires-Dist: sentry-sdk (>=2.3.1,<3.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.29,<3.0.0)
-Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Requires-Dist: structlog (>=24.2.0,<25.0.0)
 Requires-Dist: svix-ksuid (>=0.6.2,<0.7.0)
-Requires-Dist: watchfiles (>=0.21.0,<0.22.0) ; extra == "dev"
+Requires-Dist: watchfiles (>=0.22.0,<0.23.0) ; extra == "dev"
 Requires-Dist: whistle (==2.0.0a1)
 Description-Content-Type: text/x-rst
 
 HARP – Harp, an API Runtime Proxy
 =================================
 
 HARP is a powerful sidecar proxy service designed to elevate the reliability, performance, security, and observability
```

