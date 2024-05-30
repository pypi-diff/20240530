# Comparing `tmp/py4web-1.20240528.1.tar.gz` & `tmp/py4web-1.20240528.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240528.1.tar", last modified: Wed May 29 05:04:11 2024, max compression
+gzip compressed data, was "py4web-1.20240528.2.tar", last modified: Wed May 29 07:42:41 2024, max compression
```

## Comparing `py4web-1.20240528.1.tar` & `py4web-1.20240528.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.657328 py4web-1.20240528.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240528.1/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 05:04:11.657328 py4web-1.20240528.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240528.1/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.623994 py4web-1.20240528.1/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-29 04:58:50.000000 py4web-1.20240528.1/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.643995 py4web-1.20240528.1/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199954 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-29 05:04:04.000000 py4web-1.20240528.1/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394058 2024-05-29 05:04:05.000000 py4web-1.20240528.1/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74611 2024-05-28 00:14:10.000000 py4web-1.20240528.1/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.650661 py4web-1.20240528.1/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-25 08:37:03.000000 py4web-1.20240528.1/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.653995 py4web-1.20240528.1/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240528.1/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69783 2024-05-24 05:08:52.000000 py4web-1.20240528.1/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240528.1/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240528.1/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240528.1/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-27 07:35:43.000000 py4web-1.20240528.1/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.627328 py4web-1.20240528.1/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-29 05:04:11.000000 py4web-1.20240528.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-29 04:58:33.000000 py4web-1.20240528.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240528.1/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-29 05:04:11.657328 py4web-1.20240528.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 05:04:11.657328 py4web-1.20240528.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240528.1/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240528.1/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.308056 py4web-1.20240528.2/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240528.2/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 07:42:41.308056 py4web-1.20240528.2/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240528.2/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.274720 py4web-1.20240528.2/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-29 07:40:41.000000 py4web-1.20240528.2/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.294722 py4web-1.20240528.2/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199956 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394058 2024-05-29 07:42:35.000000 py4web-1.20240528.2/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74615 2024-05-29 07:39:14.000000 py4web-1.20240528.2/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.301389 py4web-1.20240528.2/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-25 08:37:03.000000 py4web-1.20240528.2/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.304723 py4web-1.20240528.2/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240528.2/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69783 2024-05-24 05:08:52.000000 py4web-1.20240528.2/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-27 07:35:43.000000 py4web-1.20240528.2/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.274720 py4web-1.20240528.2/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-29 07:40:49.000000 py4web-1.20240528.2/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240528.2/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-29 07:42:41.308056 py4web-1.20240528.2/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.308056 py4web-1.20240528.2/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240528.2/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_url.py
```

### Comparing `py4web-1.20240528.1/LICENSE.md` & `py4web-1.20240528.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/PKG-INFO` & `py4web-1.20240528.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240528.1
+Version: 1.20240528.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240528.1/README.rst` & `py4web-1.20240528.2/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/__init__.py` & `py4web-1.20240528.2/py4web/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240528.1"
+__version__ = "1.20240528.2"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app._default.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 199954 bytes, number of entries: 6
+Zip file size: 199956 bytes, number of entries: 6
 -rw-r--r--  3.0 unx      271 tx defN 24-May-29 04:39 __init__.py
 -rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
 -rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
--rw-r--r--  3.0 unx    13879 tx defN 24-May-29 04:58 static/index.html
+-rw-r--r--  3.0 unx    13883 tx defN 24-May-29 05:17 static/index.html
 -rw-r--r--  3.0 unx     1490 tx defN 24-May-29 04:20 static/css/prism.css
 -rw-r--r--  3.0 unx    22341 tx defN 24-May-29 04:20 static/js/prism.js
-6 files, 251444 bytes uncompressed, 198952 bytes compressed:  20.9%
+6 files, 251448 bytes uncompressed, 198954 bytes compressed:  20.9%
```

#### static/index.html

```diff
@@ -308,15 +308,15 @@
 	<ul>
 	  <li>A built-in <a href="https://py4web.com/_documentation/static/en/chapter-04.html">Web UI</a>.</li>
 	  <li>A built-in ticketing system to track and retrieve bugs in production.</li>
 	  <li>It provides <a href="https://py4web.com/_documentation/static/en/chapter-07.html#record-versioning">full record versioning</a> (remembers all changes to every record).</li>
 	  <li><a href="https://py4web.com/_documentation/static/en/chapter-11.html">internationalization and pluralization</a> with a translation UI.</li>
 	  <li>Automatic generation of <a href="https://py4web.com/_documentation/static/en/chapter-08.html">RESTful APIs</a> for your database.</li>
 	  <li>Built-in logic for <a href="https://py4web.com/_documentation/static/en/chapter-13.html#user-impersonation">user impersonation</a>.</li>
-	  <li>Integrated <a href="https://github.com/web2py/py4web/blob/master/apps/_scaffold/settings.py#L75">SSO support for Google, Github, Facebook, Okta, LDAP, PAM</li>
+	  <li>Integrated <a href="https://github.com/web2py/py4web/blob/master/apps/_scaffold/settings.py#L75">SSO support</a> for Google, Github, Facebook, Okta, LDAP, PAM</li>
 	</ul>
       </div>
 
       <h4>LICENSE</h4>
 
       <a href="https://opensource.org/license/bsd-3-clause">3-clause BSD</a>
```

##### html2text {}

```diff
@@ -196,13 +196,13 @@
     * A built-in _W_e_b_ _U_I.
     * A built-in ticketing system to track and retrieve bugs in production.
     * It provides _f_u_l_l_ _r_e_c_o_r_d_ _v_e_r_s_i_o_n_i_n_g (remembers all changes to every
       record).
     * _i_n_t_e_r_n_a_t_i_o_n_a_l_i_z_a_t_i_o_n_ _a_n_d_ _p_l_u_r_a_l_i_z_a_t_i_o_n with a translation UI.
     * Automatic generation of _R_E_S_T_f_u_l_ _A_P_I_s for your database.
     * Built-in logic for _u_s_e_r_ _i_m_p_e_r_s_o_n_a_t_i_o_n.
-    * Integrated _S_S_O_ _s_u_p_p_o_r_t_ _f_o_r_ _G_o_o_g_l_e_,_ _G_i_t_h_u_b_,_ _F_a_c_e_b_o_o_k_,_ _O_k_t_a_,_ _L_D_A_P_,_ _P_A_M
+    * Integrated _S_S_O_ _s_u_p_p_o_r_t for Google, Github, Facebook, Okta, LDAP, PAM
 ****** LLIICCEENNSSEE ******
 _3_-_c_l_a_u_s_e_ _B_S_D
 ****** UUSSEEFFUULL LLIINNKKSS ******
 _A_ _m_i_n_i_m_a_l_i_s_t_ _F_a_c_e_b_o_o_k_ _c_l_o_n_e
 _A_ _m_i_n_i_m_a_l_i_s_t_ _T_w_i_t_t_e_r_ _c_l_o_n_e_ _(_w_i_t_h_ _V_u_e_)
```

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240528.2/py4web/assets/py4web.app.showcase.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/core.py` & `py4web-1.20240528.2/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1901,15 +1901,15 @@
 )
 def cli():
     """The Command Line Interface"""
 
 
 @cli.command()
 @click.option(
-    "-a", "--all", is_flag=True, default=False, help="List version of all modules"
+    "-v", "--verbose", is_flag=True, default=False, help="List version of all modules"
 )
 def version(verbose=False):
     """Show versions and exit"""
     from . import __version__  # pylint: disable=import-outside-toplevel
 
     click.echo(f"py4web: {__version__}")
     if verbose:
```

### Comparing `py4web-1.20240528.1/py4web/server_adapters.py` & `py4web-1.20240528.2/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth.py` & `py4web-1.20240528.2/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240528.2/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/cors.py` & `py4web-1.20240528.2/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/dbstore.py` & `py4web-1.20240528.2/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/downloader.py` & `py4web-1.20240528.2/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/factories.py` & `py4web-1.20240528.2/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/form.py` & `py4web-1.20240528.2/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/grid.py` & `py4web-1.20240528.2/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/jsonrpc.py` & `py4web-1.20240528.2/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/mailer.py` & `py4web-1.20240528.2/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/misc.py` & `py4web-1.20240528.2/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/populate.py` & `py4web-1.20240528.2/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/publisher.py` & `py4web-1.20240528.2/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/recaptcha.py` & `py4web-1.20240528.2/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/security.py` & `py4web-1.20240528.2/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web/utils/url_signer.py` & `py4web-1.20240528.2/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/py4web.egg-info/PKG-INFO` & `py4web-1.20240528.2/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240528.1
+Version: 1.20240528.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240528.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20240528.2/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/pyproject.toml` & `py4web-1.20240528.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py4web"
-version = "1.20240528.1"
+version = "1.20240528.2"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240528.1/tests/test_action.py` & `py4web-1.20240528.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_auth.py` & `py4web-1.20240528.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_cache.py` & `py4web-1.20240528.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_fixture.py` & `py4web-1.20240528.2/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_form.py` & `py4web-1.20240528.2/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_get_error_snapshot.py` & `py4web-1.20240528.2/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_json.py` & `py4web-1.20240528.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_main.py` & `py4web-1.20240528.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_session.py` & `py4web-1.20240528.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.1/tests/test_tags.py` & `py4web-1.20240528.2/tests/test_tags.py`

 * *Files identical despite different names*

