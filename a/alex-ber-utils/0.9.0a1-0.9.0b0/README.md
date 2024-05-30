# Comparing `tmp/alex_ber_utils-0.9.0a1.tar.gz` & `tmp/alex_ber_utils-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.9.0a1.tar", last modified: Wed May 29 14:44:13 2024, max compression
+gzip compressed data, was "alex_ber_utils-0.9.0b0.tar", last modified: Thu May 30 17:53:08 2024, max compression
```

## Comparing `alex_ber_utils-0.9.0a1.tar` & `alex_ber_utils-0.9.0b0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.983812 alex_ber_utils-0.9.0a1/
--rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.9.0a1/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    31518 2024-05-29 14:44:13.984812 alex_ber_utils-0.9.0a1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3748 2024-05-28 15:27:17.000000 alex_ber_utils-0.9.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.156353 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31518 2024-05-29 14:44:11.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2102 2024-05-29 14:44:12.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:44:11.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 14:44:11.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:44:08.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-29 14:44:11.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-29 14:44:11.000000 alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.166705 alex_ber_utils-0.9.0a1/alexber/
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.458428 alex_ber_utils-0.9.0a1/alexber/utils/
--rwxrwxrwx   0 root         (0) root         (0)      148 2024-05-28 19:28:20.000000 alex_ber_utils-0.9.0a1/alexber/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/_ymlparsers_extra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.477062 alex_ber_utils-0.9.0a1/alexber/utils/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0a1/alexber/utils/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/deploys.py
--rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/emails.py
--rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/fabs.py
--rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/importer.py
--rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/init_app_conf.py
--rwxrwxrwx   0 root         (0) root         (0)     3411 2024-05-29 09:24:38.000000 alex_ber_utils-0.9.0a1/alexber/utils/inspects.py
--rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/mains.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/parsers.py
--rwxrwxrwx   0 root         (0) root         (0)     1804 2024-05-29 09:19:29.000000 alex_ber_utils-0.9.0a1/alexber/utils/pprint.py
--rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/processinvokes.py
--rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/props.py
--rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/setups.py
--rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/stdlogging.py
--rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/thread_locals.py
--rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/uuids.py
--rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/alexber/utils/ymlparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.489124 alex_ber_utils-0.9.0a1/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0a1/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/req-env.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/req-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-28 15:09:21.000000 alex_ber_utils-0.9.0a1/req-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-28 14:48:40.000000 alex_ber_utils-0.9.0a1/req-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/req-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/req.txt
--rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-28 14:53:19.000000 alex_ber_utils-0.9.0a1/requirements-env.txt
--rwxrwxrwx   0 root         (0) root         (0)      670 2024-05-28 14:53:33.000000 alex_ber_utils-0.9.0a1/requirements-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)      601 2024-05-28 15:10:40.000000 alex_ber_utils-0.9.0a1/requirements-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-28 15:10:10.000000 alex_ber_utils-0.9.0a1/requirements-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-05-28 14:54:21.000000 alex_ber_utils-0.9.0a1/requirements-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)      194 2024-05-28 14:53:06.000000 alex_ber_utils-0.9.0a1/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      190 2024-05-29 14:44:13.989812 alex_ber_utils-0.9.0a1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4867 2024-05-29 09:42:25.000000 alex_ber_utils-0.9.0a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.509433 alex_ber_utils-0.9.0a1/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1600 2024-05-28 19:37:45.000000 alex_ber_utils-0.9.0a1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.730052 alex_ber_utils-0.9.0a1/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/deploys_test.py
--rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/emails_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5324 2024-05-28 19:41:58.000000 alex_ber_utils-0.9.0a1/tests/utils/importer_test.py
--rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/init_app_conf_test.py
--rwxrwxrwx   0 root         (0) root         (0)     3656 2024-05-29 00:50:48.000000 alex_ber_utils-0.9.0a1/tests/utils/inspect_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/mains_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5091 2024-05-28 19:34:14.000000 alex_ber_utils-0.9.0a1/tests/utils/parsers_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2712 2024-05-29 09:40:19.000000 alex_ber_utils-0.9.0a1/tests/utils/pprint_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/processinvokes_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/properties_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.765124 alex_ber_utils-0.9.0a1/tests/utils/splitpackage/
--rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/splitpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/splitpackage/mymodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.797357 alex_ber_utils-0.9.0a1/tests/utils/splitpackage_cont/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/splitpackage_cont/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/splitpackage_cont/other_module.py
--rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/threadlocal_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/uuids_test.py
--rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/ymlparsers_extra_test.py
--rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests/utils/ymlparsers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.811356 alex_ber_utils-0.9.0a1/tests_data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.823527 alex_ber_utils-0.9.0a1/tests_data/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.883791 alex_ber_utils-0.9.0a1/tests_data/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/config.properties
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/config2.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.903245 alex_ber_utils-0.9.0a1/tests_data/tests/utils/initappconf/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/initappconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.951060 alex_ber_utils-0.9.0a1/tests_data/tests/utils/parser/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/parser/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/parser/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:44:13.971446 alex_ber_utils-0.9.0a1/tests_data/tests/utils/ymlparsers/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a1/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.654682 alex_ber_utils-0.9.0b0/
+-rwxrwxrwx   0 root         (0) root         (0)    29048 2024-05-30 17:49:09.000000 alex_ber_utils-0.9.0b0/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    33921 2024-05-30 17:53:08.655666 alex_ber_utils-0.9.0b0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3748 2024-05-28 15:27:17.000000 alex_ber_utils-0.9.0b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:07.817966 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    33921 2024-05-30 17:53:06.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-05-30 17:53:07.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 17:53:06.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 17:53:06.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 17:46:18.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-30 17:53:06.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-30 17:53:06.000000 alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:07.829985 alex_ber_utils-0.9.0b0/alexber/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.113602 alex_ber_utils-0.9.0b0/alexber/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      148 2024-05-28 19:28:20.000000 alex_ber_utils-0.9.0b0/alexber/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.132149 alex_ber_utils-0.9.0b0/alexber/utils/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0b0/alexber/utils/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/deploys.py
+-rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/emails.py
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/fabs.py
+-rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/importer.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/init_app_conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     3987 2024-05-30 16:55:40.000000 alex_ber_utils-0.9.0b0/alexber/utils/inspects.py
+-rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/mains.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     2443 2024-05-30 17:47:13.000000 alex_ber_utils-0.9.0b0/alexber/utils/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/processinvokes.py
+-rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/props.py
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/setups.py
+-rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/stdlogging.py
+-rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/thread_locals.py
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/uuids.py
+-rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.143149 alex_ber_utils-0.9.0b0/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0b0/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/req-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/req-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-28 15:09:21.000000 alex_ber_utils-0.9.0b0/req-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-28 14:48:40.000000 alex_ber_utils-0.9.0b0/req-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/req-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-28 14:53:19.000000 alex_ber_utils-0.9.0b0/requirements-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)      670 2024-05-28 14:53:33.000000 alex_ber_utils-0.9.0b0/requirements-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)      601 2024-05-28 15:10:40.000000 alex_ber_utils-0.9.0b0/requirements-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-28 15:10:10.000000 alex_ber_utils-0.9.0b0/requirements-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-05-28 14:54:21.000000 alex_ber_utils-0.9.0b0/requirements-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)      194 2024-05-28 14:53:06.000000 alex_ber_utils-0.9.0b0/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      190 2024-05-30 17:53:08.660665 alex_ber_utils-0.9.0b0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4866 2024-05-30 17:49:09.000000 alex_ber_utils-0.9.0b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.164394 alex_ber_utils-0.9.0b0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1600 2024-05-28 19:37:45.000000 alex_ber_utils-0.9.0b0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.398677 alex_ber_utils-0.9.0b0/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/deploys_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/emails_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5324 2024-05-28 19:41:58.000000 alex_ber_utils-0.9.0b0/tests/utils/importer_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/init_app_conf_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3656 2024-05-29 00:50:48.000000 alex_ber_utils-0.9.0b0/tests/utils/inspect_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/mains_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5091 2024-05-28 19:34:14.000000 alex_ber_utils-0.9.0b0/tests/utils/parsers_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2712 2024-05-29 09:40:19.000000 alex_ber_utils-0.9.0b0/tests/utils/pprint_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/processinvokes_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.434520 alex_ber_utils-0.9.0b0/tests/utils/splitpackage/
+-rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/splitpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.469138 alex_ber_utils-0.9.0b0/tests/utils/splitpackage_cont/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/splitpackage_cont/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/splitpackage_cont/other_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/threadlocal_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/uuids_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/ymlparsers_extra_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.483138 alex_ber_utils-0.9.0b0/tests_data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.496137 alex_ber_utils-0.9.0b0/tests_data/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.557153 alex_ber_utils-0.9.0b0/tests_data/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/config.properties
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.578239 alex_ber_utils-0.9.0b0/tests_data/tests/utils/initappconf/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.618222 alex_ber_utils-0.9.0b0/tests_data/tests/utils/parser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/parser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:53:08.639683 alex_ber_utils-0.9.0b0/tests_data/tests/utils/ymlparsers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0b0/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.9.0a1/CHANGELOG.md` & `alex_ber_utils-0.9.0b0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,77 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
-## [0.8.1a] 04.12.2023
+## [0.9.0b] 30.05.2024
+### Changed
 
+- Minimum library requirement is Python 3.9 now.
+- Dockerfile's base docker image was changed to be based on Python 3.9
+- Some functionality was moved from dropped method_overloading_test.py to importer_test.py
+- Implementation of inspects.ismethod() and inspects.has_method() was changed. 
+- inspect_test.py was changed. inspects.has_method() now expected to return False on property
+(as it should in the first place).
+- In Dockerfile setuptools was **downgraded** from 67.8.0 to 65.6.3. 
+See https://stackoverflow.com/questions/76043689/pkg-resources-is-deprecated-as-an-api#comment136784284_76044568
+- In Dockerfile reference to requirements-md.txt was droped.
+- To requirements.in, req-piptools.txt and req-tests.txt packaging<24.0,>=23.2 was added.
+- All requirements.txt was regenerated, so version has changed:
+- importlib-metadata (and it's dependency zipp) were dropped.
+- bcrypt upgraded from 4.1.1 to 4.1.3.
+- build from 1.0.3 to 1.2.1.
+- cryptography from 41.0.7 to 42.0.7.
+- exceptiongroup from 1.2.0 to 1.2.1.
+- hiyapyco from 0.5.4 to 0.6.0.
+- jinja2 from 3.1.2 to 3.1.4.
+- markupsafe from 2.1.3 to 2.1.5.
+- paramiko from 3.3.1 to 3.4.0
+- pip-tools from 7.3.0 to 7.4.1
+- pluggy from 1.3.0 to 1.5.0
+- pycparser 2.21 to 2.22.
+- pyopenssl from 23.3.0 to 24.1.0.
+- pyproject-hooks from 1.0.0 to 1.1.0.
+- python-dotenv from 1.0.0 to 1.0.1
+- wheel from 0.42.0 to 0.43.0
+ 
+- (minor) Import to dropped enums.py was removed from parsers_test.py 
+
+### Added
+- inspects.resolve_function_args() - maps both explicit and default arguments of a function call by parameter name.
+- inspects.update_function_defaults() - decorator to change and remove default value.
+- pprint.py module. This module effectively changes the default values of the standard `pprint.pprint` module. Intended Usage:
+
+Instead of:
+
+```python
+from pprint import pprint
+```
+use
+```python
+from alexber.utils.pprint import pprint
+```
+
+The defaults are:
+- `indent`: 4
+- `width`: 120
+- `depth`: None
+- `stream`: None
+- `compact`: False
+- `sort_dicts`: False
+- `underscore_numbers`: False
+
+See docstring of pprint.py module for more details.
+
+### Removed
+- Optional dependency alex-ber-utils[md] was removed. Unit-tests for multidispatch was removed.
+Also files req-md.txt and requirements-md.txt was deleted. 
+- Module enums was removed. It does monkey-patching to standard library's enums, that breaks them in Python 3.9+.
 
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
```

### Comparing `alex_ber_utils-0.9.0a1/LICENSE.txt` & `alex_ber_utils-0.9.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/PKG-INFO` & `alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alex_ber_utils
-Version: 0.9.0a1
+Name: alex-ber-utils
+Version: 0.9.0b0
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Education
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: fabric
 Provides-Extra: yaml
 Provides-Extra: yml
 Provides-Extra: env
 Provides-Extra: tests
 Provides-Extra: piptools
@@ -196,16 +196,77 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
-## [0.8.1a] 04.12.2023
+## [0.9.0b] 30.05.2024
+### Changed
 
+- Minimum library requirement is Python 3.9 now.
+- Dockerfile's base docker image was changed to be based on Python 3.9
+- Some functionality was moved from dropped method_overloading_test.py to importer_test.py
+- Implementation of inspects.ismethod() and inspects.has_method() was changed. 
+- inspect_test.py was changed. inspects.has_method() now expected to return False on property
+(as it should in the first place).
+- In Dockerfile setuptools was **downgraded** from 67.8.0 to 65.6.3. 
+See https://stackoverflow.com/questions/76043689/pkg-resources-is-deprecated-as-an-api#comment136784284_76044568
+- In Dockerfile reference to requirements-md.txt was droped.
+- To requirements.in, req-piptools.txt and req-tests.txt packaging<24.0,>=23.2 was added.
+- All requirements.txt was regenerated, so version has changed:
+- importlib-metadata (and it's dependency zipp) were dropped.
+- bcrypt upgraded from 4.1.1 to 4.1.3.
+- build from 1.0.3 to 1.2.1.
+- cryptography from 41.0.7 to 42.0.7.
+- exceptiongroup from 1.2.0 to 1.2.1.
+- hiyapyco from 0.5.4 to 0.6.0.
+- jinja2 from 3.1.2 to 3.1.4.
+- markupsafe from 2.1.3 to 2.1.5.
+- paramiko from 3.3.1 to 3.4.0
+- pip-tools from 7.3.0 to 7.4.1
+- pluggy from 1.3.0 to 1.5.0
+- pycparser 2.21 to 2.22.
+- pyopenssl from 23.3.0 to 24.1.0.
+- pyproject-hooks from 1.0.0 to 1.1.0.
+- python-dotenv from 1.0.0 to 1.0.1
+- wheel from 0.42.0 to 0.43.0
+ 
+- (minor) Import to dropped enums.py was removed from parsers_test.py 
+
+### Added
+- inspects.resolve_function_args() - maps both explicit and default arguments of a function call by parameter name.
+- inspects.update_function_defaults() - decorator to change and remove default value.
+- pprint.py module. This module effectively changes the default values of the standard `pprint.pprint` module. Intended Usage:
+
+Instead of:
+
+```python
+from pprint import pprint
+```
+use
+```python
+from alexber.utils.pprint import pprint
+```
+
+The defaults are:
+- `indent`: 4
+- `width`: 120
+- `depth`: None
+- `stream`: None
+- `compact`: False
+- `sort_dicts`: False
+- `underscore_numbers`: False
+
+See docstring of pprint.py module for more details.
+
+### Removed
+- Optional dependency alex-ber-utils[md] was removed. Unit-tests for multidispatch was removed.
+Also files req-md.txt and requirements-md.txt was deleted. 
+- Module enums was removed. It does monkey-patching to standard library's enums, that breaks them in Python 3.9+.
 
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
```

### Comparing `alex_ber_utils-0.9.0a1/README.md` & `alex_ber_utils-0.9.0b0/README.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/PKG-INFO` & `alex_ber_utils-0.9.0b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alex-ber-utils
-Version: 0.9.0a1
+Name: alex_ber_utils
+Version: 0.9.0b0
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Education
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: fabric
 Provides-Extra: yaml
 Provides-Extra: yml
 Provides-Extra: env
 Provides-Extra: tests
 Provides-Extra: piptools
@@ -196,16 +196,77 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
-## [0.8.1a] 04.12.2023
+## [0.9.0b] 30.05.2024
+### Changed
 
+- Minimum library requirement is Python 3.9 now.
+- Dockerfile's base docker image was changed to be based on Python 3.9
+- Some functionality was moved from dropped method_overloading_test.py to importer_test.py
+- Implementation of inspects.ismethod() and inspects.has_method() was changed. 
+- inspect_test.py was changed. inspects.has_method() now expected to return False on property
+(as it should in the first place).
+- In Dockerfile setuptools was **downgraded** from 67.8.0 to 65.6.3. 
+See https://stackoverflow.com/questions/76043689/pkg-resources-is-deprecated-as-an-api#comment136784284_76044568
+- In Dockerfile reference to requirements-md.txt was droped.
+- To requirements.in, req-piptools.txt and req-tests.txt packaging<24.0,>=23.2 was added.
+- All requirements.txt was regenerated, so version has changed:
+- importlib-metadata (and it's dependency zipp) were dropped.
+- bcrypt upgraded from 4.1.1 to 4.1.3.
+- build from 1.0.3 to 1.2.1.
+- cryptography from 41.0.7 to 42.0.7.
+- exceptiongroup from 1.2.0 to 1.2.1.
+- hiyapyco from 0.5.4 to 0.6.0.
+- jinja2 from 3.1.2 to 3.1.4.
+- markupsafe from 2.1.3 to 2.1.5.
+- paramiko from 3.3.1 to 3.4.0
+- pip-tools from 7.3.0 to 7.4.1
+- pluggy from 1.3.0 to 1.5.0
+- pycparser 2.21 to 2.22.
+- pyopenssl from 23.3.0 to 24.1.0.
+- pyproject-hooks from 1.0.0 to 1.1.0.
+- python-dotenv from 1.0.0 to 1.0.1
+- wheel from 0.42.0 to 0.43.0
+ 
+- (minor) Import to dropped enums.py was removed from parsers_test.py 
+
+### Added
+- inspects.resolve_function_args() - maps both explicit and default arguments of a function call by parameter name.
+- inspects.update_function_defaults() - decorator to change and remove default value.
+- pprint.py module. This module effectively changes the default values of the standard `pprint.pprint` module. Intended Usage:
+
+Instead of:
+
+```python
+from pprint import pprint
+```
+use
+```python
+from alexber.utils.pprint import pprint
+```
+
+The defaults are:
+- `indent`: 4
+- `width`: 120
+- `depth`: None
+- `stream`: None
+- `compact`: False
+- `sort_dicts`: False
+- `underscore_numbers`: False
+
+See docstring of pprint.py module for more details.
+
+### Removed
+- Optional dependency alex-ber-utils[md] was removed. Unit-tests for multidispatch was removed.
+Also files req-md.txt and requirements-md.txt was deleted. 
+- Module enums was removed. It does monkey-patching to standard library's enums, that breaks them in Python 3.9+.
 
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
```

### Comparing `alex_ber_utils-0.9.0a1/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.9.0b0/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.9.0b0/alexber/utils/_ymlparsers_extra.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/deploys.py` & `alex_ber_utils-0.9.0b0/alexber/utils/deploys.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/emails.py` & `alex_ber_utils-0.9.0b0/alexber/utils/emails.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/fabs.py` & `alex_ber_utils-0.9.0b0/alexber/utils/fabs.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/files.py` & `alex_ber_utils-0.9.0b0/alexber/utils/files.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/importer.py` & `alex_ber_utils-0.9.0b0/alexber/utils/importer.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.9.0b0/alexber/utils/init_app_conf.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/inspects.py` & `alex_ber_utils-0.9.0b0/alexber/utils/inspects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from functools import wraps
+import functools
 from typing import Dict, List, Any, Optional, Callable, Type
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 def issetdescriptor(object: Any) -> bool:
@@ -15,16 +15,14 @@
         # mutual exclusion
         return False
     tp = type(object)
 
     return hasattr(tp, "__set__")
 
 
-import inspect
-from typing import Any
 
 
 def ismethod(object: Any) -> bool:
     """Check if the given object is a method.
 
     If the object is a class, return False.
     If the object is not a function or method, return False.
@@ -59,15 +57,15 @@
     :return: Decorated function with modified default values.
     """
     if new_defaults is None:
         new_defaults = {}
     if remove_defaults is None:
         remove_defaults = []
 
-    @wraps(func)
+    @functools.wraps(func)
     def wrapper(*args, **kwargs):
         # Get the signature of the original function
         sig = inspect.signature(func)
 
         # Create a new signature with updated default values
         new_params = []
         for param in sig.parameters.values():
@@ -90,7 +88,26 @@
 
         # Call the original function with the bound arguments
         _bounded_args = bound_args.args
         _bounded_kwargs = bound_args.kwargs
         return func(*_bounded_args, **_bounded_kwargs)
 
     return wrapper
+
+
+def resolve_function_args(func: Callable, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    """
+    Map both explicit and default arguments of a function call by parameter name.
+
+    Parameters:
+    - func: The function whose arguments are to be mapped.
+    - args: Positional arguments passed to the function.
+    - kwargs: Keyword arguments passed to the function.
+
+    Returns:
+    - A dictionary mapping parameter names to their corresponding values.
+    """
+    sig = inspect.signature(func)
+    bound_args = sig.bind_partial(*args, **kwargs)
+    bound_args.apply_defaults()
+    return bound_args.arguments
+
```

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/mains.py` & `alex_ber_utils-0.9.0b0/alexber/utils/mains.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/parsers.py` & `alex_ber_utils-0.9.0b0/alexber/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/processinvokes.py` & `alex_ber_utils-0.9.0b0/alexber/utils/processinvokes.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/props.py` & `alex_ber_utils-0.9.0b0/alexber/utils/props.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/setups.py` & `alex_ber_utils-0.9.0b0/alexber/utils/setups.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/stdlogging.py` & `alex_ber_utils-0.9.0b0/alexber/utils/stdlogging.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/thread_locals.py` & `alex_ber_utils-0.9.0b0/alexber/utils/thread_locals.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/uuids.py` & `alex_ber_utils-0.9.0b0/alexber/utils/uuids.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.9.0b0/alexber/utils/ymlparsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/requirements-fabric.txt` & `alex_ber_utils-0.9.0b0/requirements-fabric.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/requirements-piptools.txt` & `alex_ber_utils-0.9.0b0/requirements-piptools.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/requirements-tests.txt` & `alex_ber_utils-0.9.0b0/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/setup.py` & `alex_ber_utils-0.9.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
 
 #VERSION should be defined before importing UploadCommand
-VERSION = '0.9.0a1'
+VERSION = '0.9.0b'
 from alexber.utils import UploadCommand
 NAME = 'alex_ber_utils'
 SHORT_NAME = 'utils'
 VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
 DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
 AUTHOR = 'Alexander Berkovich'
 
@@ -111,15 +111,15 @@
             'Topic :: Education',
             'Operating System :: OS Independent',
             'Operating System :: Microsoft :: Windows',
             'Operating System :: POSIX',
             'Operating System :: Unix',
             'Natural Language :: English',
         ],
-        python_requires='>=3.6',
+        python_requires='>=3.9',
         zip_safe=False,
 
     )
 
 finally:
     try:
         os.unlink(lnk_data)
```

### Comparing `alex_ber_utils-0.9.0a1/tests/conftest.py` & `alex_ber_utils-0.9.0b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/deploys_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/deploys_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/emails_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/emails_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/importer_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/importer_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/init_app_conf_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/inspect_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/inspect_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/mains_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/mains_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/parsers_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/parsers_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/pprint_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/pprint_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/processinvokes_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/properties_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/properties_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/threadlocal_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/threadlocal_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/uuids_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/uuids_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/ymlparsers_extra_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.9.0a1/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.9.0b0/tests/utils/ymlparsers_test.py`

 * *Files identical despite different names*

