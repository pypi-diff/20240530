# Comparing `tmp/py4web-1.20240528.2.tar.gz` & `tmp/py4web-1.20240529.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240528.2.tar", last modified: Wed May 29 07:42:41 2024, max compression
+gzip compressed data, was "py4web-1.20240529.1.tar", last modified: Thu May 30 01:47:04 2024, max compression
```

## Comparing `py4web-1.20240528.2.tar` & `py4web-1.20240529.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.308056 py4web-1.20240528.2/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240528.2/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 07:42:41.308056 py4web-1.20240528.2/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240528.2/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.274720 py4web-1.20240528.2/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-29 07:40:41.000000 py4web-1.20240528.2/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.294722 py4web-1.20240528.2/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199956 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-29 07:42:34.000000 py4web-1.20240528.2/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394058 2024-05-29 07:42:35.000000 py4web-1.20240528.2/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74615 2024-05-29 07:39:14.000000 py4web-1.20240528.2/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.301389 py4web-1.20240528.2/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-25 08:37:03.000000 py4web-1.20240528.2/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.304723 py4web-1.20240528.2/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240528.2/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69783 2024-05-24 05:08:52.000000 py4web-1.20240528.2/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240528.2/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240528.2/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240528.2/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-27 07:35:43.000000 py4web-1.20240528.2/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.274720 py4web-1.20240528.2/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-29 07:42:41.000000 py4web-1.20240528.2/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-29 07:40:49.000000 py4web-1.20240528.2/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240528.2/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-29 07:42:41.308056 py4web-1.20240528.2/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-29 07:42:41.308056 py4web-1.20240528.2/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240528.2/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240528.2/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.204552 py4web-1.20240529.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240529.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-30 01:47:04.204552 py4web-1.20240529.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240529.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.171218 py4web-1.20240529.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-30 01:46:37.000000 py4web-1.20240529.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.191218 py4web-1.20240529.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-30 01:46:57.000000 py4web-1.20240529.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199956 2024-05-30 01:46:57.000000 py4web-1.20240529.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-30 01:46:57.000000 py4web-1.20240529.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-30 01:46:57.000000 py4web-1.20240529.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-30 01:46:57.000000 py4web-1.20240529.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394074 2024-05-30 01:46:58.000000 py4web-1.20240529.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74670 2024-05-29 14:13:48.000000 py4web-1.20240529.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.197885 py4web-1.20240529.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-25 08:37:03.000000 py4web-1.20240529.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.201218 py4web-1.20240529.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240529.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69806 2024-05-30 01:44:44.000000 py4web-1.20240529.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240529.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240529.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240529.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-29 14:24:54.000000 py4web-1.20240529.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.174551 py4web-1.20240529.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-30 01:47:04.000000 py4web-1.20240529.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-30 01:46:16.000000 py4web-1.20240529.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240529.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-30 01:47:04.204552 py4web-1.20240529.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 01:47:04.204552 py4web-1.20240529.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240529.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240529.1/tests/test_url.py
```

### Comparing `py4web-1.20240528.2/LICENSE.md` & `py4web-1.20240529.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/PKG-INFO` & `py4web-1.20240529.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240528.2
+Version: 1.20240529.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240528.2/README.rst` & `py4web-1.20240529.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/__init__.py` & `py4web-1.20240529.1/py4web/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240528.2"
+__version__ = "1.20240529.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app._default.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 199956 bytes, number of entries: 6
 -rw-r--r--  3.0 unx      271 tx defN 24-May-29 04:39 __init__.py
 -rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
 -rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
--rw-r--r--  3.0 unx    13883 tx defN 24-May-29 05:17 static/index.html
+-rw-r--r--  3.0 unx    13882 tx defN 24-May-30 01:45 static/index.html
 -rw-r--r--  3.0 unx     1490 tx defN 24-May-29 04:20 static/css/prism.css
 -rw-r--r--  3.0 unx    22341 tx defN 24-May-29 04:20 static/js/prism.js
-6 files, 251448 bytes uncompressed, 198954 bytes compressed:  20.9%
+6 files, 251447 bytes uncompressed, 198954 bytes compressed:  20.9%
```

#### static/index.html

```diff
@@ -51,15 +51,15 @@
 	Install it and start it
 
 <pre class="language-bash"><code>
 $ pip install py4web               # install it (but use a venv or Nix)
 $ py4web setup apps                # answer yes to all questions
 $ py4web set_password              # pick a password for the admin
 $ cp -r apps/_scaffold apps/myapp  # make a new app
-$ py4web run apps                  # starts py4web
+$ py4web run apps                  # start py4web
 </code></pre>
 
 Each subfolder of <tt>apps/</tt> with an <tt>__init__.py</tt> is its own app. One py4web can run multiple apps. You just copy the <tt>_scaffold</tt> app to make a new one.
 	
       </div><div class="section">
 	
 	The basic functions/objects are imported from the py4web module.
```

##### html2text {}

```diff
@@ -8,15 +8,15 @@
 applications. It is the successor of _w_e_b_2_p_y but much improved.
 Install it and start it
 
 $ pip install py4web               # install it (but use a venv or Nix)
 $ py4web setup apps                # answer yes to all questions
 $ py4web set_password              # pick a password for the admin
 $ cp -r apps/_scaffold apps/myapp  # make a new app
-$ py4web run apps                  # starts py4web
+$ py4web run apps                  # start py4web
 Each subfolder of apps/ with an __init__.py is its own app. One py4web can run
 multiple apps. You just copy the _scaffold app to make a new one.
 The basic functions/objects are imported from the py4web module.
 
 from py4web import action, redirect, request, URL, Field
 Use @action to map URLs into functions (aka actions). Actions can return
 strings or dictionaries.
```

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240529.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1394058 bytes, number of entries: 143
+Zip file size: 1394074 bytes, number of entries: 143
 -rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
 -rw-r--r--  3.0 unx     4221 tx defN 24-May-28 00:48 __init__.py
 -rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
 -rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
 -rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
 -rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
 -rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
@@ -43,15 +43,15 @@
 -rw-r--r--  3.0 unx     3031 tx defN 23-May-08 00:39 vue_components_examples/vue_grid_and_forms.py
 -rw-r--r--  3.0 unx     1390 tx defN 23-May-08 00:39 vue_components_examples/models.py
 -rw-r--r--  3.0 unx      324 tx defN 23-May-08 00:39 vue_components_examples/vue_file_uploader.py
 -rw-r--r--  3.0 unx       32 tx stor 23-May-08 00:39 vue_components_examples/common.py
 -rw-r--r--  3.0 unx      302 tx defN 23-May-08 00:39 vue_components_examples/vue_grid.py
 -rw-r--r--  3.0 unx     1597 tx defN 23-May-08 00:39 vue_components_examples/components/fileupload.py
 -rw-r--r--  3.0 unx     2078 tx defN 23-May-08 00:39 vue_components_examples/components/starrater.py
--rw-r--r--  3.0 unx    10333 tx defN 23-May-08 00:39 vue_components_examples/components/vueform.py
+-rw-r--r--  3.0 unx    10374 tx defN 24-May-29 14:21 vue_components_examples/components/vueform.py
 -rw-r--r--  3.0 unx     7777 tx defN 23-May-08 00:39 vue_components_examples/components/grid.py
 -rw-r--r--  3.0 unx     7858 tx defN 23-May-08 00:39 vue_components_examples/components/README.md
 -rw-r--r--  3.0 unx       34 tx stor 23-May-08 00:39 vue_components_examples/settings.py
 -rw-r--r--  3.0 unx     1149 tx defN 23-May-08 00:39 vue_components_examples/vue_view_form.py
 -rw-r--r--  3.0 unx     1124 tx defN 23-May-08 00:39 vue_components_examples/vue_edit_form.py
 -rw-r--r--  3.0 unx     1215 tx defN 23-May-08 00:39 vue_components_examples/vue_star_rater.py
 -rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 translations/it.json
@@ -138,8 +138,8 @@
 -rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
 -rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
 -rw-r--r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
 -rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
 -rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
-143 files, 9352387 bytes uncompressed, 1366902 bytes compressed:  85.4%
+143 files, 9352428 bytes uncompressed, 1366918 bytes compressed:  85.4%
```

#### vue_components_examples/components/vueform.py

```diff
@@ -57,15 +57,15 @@
             set, then the form is not acted upon, and the error is shown to the user.
         """
         assert session is not None, "You must provide a session."
         self.path_form = path + "/form"
         self.path_check = path + "/check"
         self.db = db
         self.signer = signer or URLSigner(session)
-        self.__prerequisites__ = [self.signer]
+        self.__prerequisites__ = [db, self.signer]  # session to be added by the signer
         self.validate = validate
         # Creates entry points for giving the blank form, and processing form submissions.
         # There are three entry points:
         # - Form setup GET: This gets how the form is set up, including the types of the fields.
         # - Form GET: This gets the values of the fields.
         # - Form PUT: This gives the values of the fields, and performs whatever
         #   action needs to be peformed.
```

### Comparing `py4web-1.20240528.2/py4web/core.py` & `py4web-1.20240529.1/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1017,14 +1017,15 @@
                             try:
                                 if context.get("exception"):
                                     call_f(fixture.on_error, context)
                                 else:
                                     call_f(fixture.on_success, context)
                             except Exception as err:
                                 context["exception"] = context.get("exception") or err
+                    for fixture in reversed(fixtures):
                         safely(lambda: Fixture.local_delete(fixture))
                     exception = context.get("exception")
                     if isinstance(exception, Exception):
                         raise exception
                 return context.get("output", "")
 
             return wrapper
```

### Comparing `py4web-1.20240528.2/py4web/server_adapters.py` & `py4web-1.20240529.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth.py` & `py4web-1.20240529.1/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240529.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/cors.py` & `py4web-1.20240529.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/dbstore.py` & `py4web-1.20240529.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/downloader.py` & `py4web-1.20240529.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/factories.py` & `py4web-1.20240529.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/form.py` & `py4web-1.20240529.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/grid.py` & `py4web-1.20240529.1/py4web/utils/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,15 +789,15 @@
 
             select_params["orderby"] = self.param.orderby
             if sort_order:
                 parts = sort_order.lstrip("~").split(".")
                 if (
                     len(parts) == 2
                     and parts[0] in db.tables
-                    and parts[1] in db[parts[p]]
+                    and parts[1] in db[parts[0]]
                 ):
                     orderby = db[parts[0]][parts[1]]
                     if sort_order.startswith("~"):
                         orderby = ~orderby
                     select_params["orderby"] = orderby
 
             if self.param.left:
@@ -1055,14 +1055,15 @@
         sort_order = request.query.get("orderby", "")
 
         thead = THEAD(
             **clean_sc(_class=self.param.grid_class_style.classes.get("grid-thead", ""))
         )
         for index, column in enumerate(self.param.columns):
             col = None
+            key = None
             if isinstance(column, (Field, FieldVirtual)):
                 field = column
                 if field.readable and (field.type != "id" or self.param.show_id):
                     key, col = self._make_field_header(column, index, sort_order)
             elif isinstance(column, Column):
                 key = column.name.lower().replace(" ", "-")
                 col = column.name
```

### Comparing `py4web-1.20240528.2/py4web/utils/jsonrpc.py` & `py4web-1.20240529.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/mailer.py` & `py4web-1.20240529.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/misc.py` & `py4web-1.20240529.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/populate.py` & `py4web-1.20240529.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/publisher.py` & `py4web-1.20240529.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/recaptcha.py` & `py4web-1.20240529.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/security.py` & `py4web-1.20240529.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web/utils/url_signer.py` & `py4web-1.20240529.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/py4web.egg-info/PKG-INFO` & `py4web-1.20240529.1/py4web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240528.2
+Version: 1.20240529.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240528.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20240529.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/pyproject.toml` & `py4web-1.20240529.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py4web"
-version = "1.20240528.2"
+version = "1.20240529.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240528.2/tests/test_action.py` & `py4web-1.20240529.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_auth.py` & `py4web-1.20240529.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_cache.py` & `py4web-1.20240529.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_fixture.py` & `py4web-1.20240529.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_form.py` & `py4web-1.20240529.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_get_error_snapshot.py` & `py4web-1.20240529.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_json.py` & `py4web-1.20240529.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_main.py` & `py4web-1.20240529.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_session.py` & `py4web-1.20240529.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240528.2/tests/test_tags.py` & `py4web-1.20240529.1/tests/test_tags.py`

 * *Files identical despite different names*

