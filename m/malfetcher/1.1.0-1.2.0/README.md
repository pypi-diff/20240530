# Comparing `tmp/malfetcher-1.1.0.tar.gz` & `tmp/malfetcher-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malfetcher-1.1.0.tar", last modified: Tue May 14 12:09:59 2024, max compression
+gzip compressed data, was "malfetcher-1.2.0.tar", last modified: Thu May 30 19:31:45 2024, max compression
```

## Comparing `malfetcher-1.1.0.tar` & `malfetcher-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-14 12:09:51.000000 malfetcher-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-14 12:09:59.953037 malfetcher-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-14 12:09:51.000000 malfetcher-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/malfetcher/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/mal_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/mal_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/malfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 12:09:51.000000 malfetcher-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:09:59.953037 malfetcher-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 12:09:51.000000 malfetcher-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:31:45.654020 malfetcher-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-30 19:31:41.000000 malfetcher-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-30 19:31:45.654020 malfetcher-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-30 19:31:41.000000 malfetcher-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:31:45.650020 malfetcher-1.2.0/malfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-30 19:31:41.000000 malfetcher-1.2.0/malfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-30 19:31:41.000000 malfetcher-1.2.0/malfetcher/mal_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20483 2024-05-30 19:31:41.000000 malfetcher-1.2.0/malfetcher/mal_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-30 19:31:41.000000 malfetcher-1.2.0/malfetcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:31:45.654020 malfetcher-1.2.0/malfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-30 19:31:45.000000 malfetcher-1.2.0/malfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 19:31:45.000000 malfetcher-1.2.0/malfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:31:45.000000 malfetcher-1.2.0/malfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 19:31:45.000000 malfetcher-1.2.0/malfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 19:31:45.000000 malfetcher-1.2.0/malfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-30 19:31:41.000000 malfetcher-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:31:45.654020 malfetcher-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-30 19:31:41.000000 malfetcher-1.2.0/setup.py
```

### Comparing `malfetcher-1.1.0/LICENSE` & `malfetcher-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malfetcher-1.1.0/PKG-INFO` & `malfetcher-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malfetcher
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple library to help you fetch data from MyAnimeList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/prochy-exe/malfetcher
 Project-URL: Documentation, https://github.com/prochy-exe/malfetcher/wiki
 Project-URL: Source, https://github.com/prochy-exe/malfetcher
 Keywords: python,mal,myanimelist
@@ -26,14 +26,15 @@
 Requires-Dist: gevent
 
 # malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
+
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
 
 ### Dependencies
 
 * Python(tested on the latest ver.)
@@ -61,47 +62,49 @@
 pip install -e .
 ```
 
 ### Using the library
 
 * To import the library into your code use:
 ```
-import malhelper
+import malfetcher
 ```
 * When importing this library for the first time, you will be taken through the setup process
 
 ### Setting up the MyAnilist developer app
 
 * When the setup process starts, you will be automatically taken to required pages. This process is really simple.
 * When asked for the Client ID, you will be taken to the account developer page.
 * If not logged in, log in first.
 * Then create a new client
 * Choose whatever name you fancy, and for the redirect URL use http://localhost:8888/auth
 * After you save the client, copy the ID and paste it into the terminal
 * After entering the ID you will be taken to an auth page, where you need to allow the app to access your account.
-* Afterwards you will be taken to a redirect page that is momentarily hosted using gevent. (If you have any worries, please see the token_getter.html source code.)
+* Afterwards you will be taken to a redirect page that will automatically send the token to the library.
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.1](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
+* [1.2.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.2.0)
+    * [fix light init](https://github.com/prochy-exe/malfetcher/commit/8f30536fe4f9817eea870cb4d4ea7a248badb0b5)
+* [1.1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
     * [fix typo](https://github.com/prochy-exe/malfetcher/commit/ec8fa79befc1a4190667639920f3b6bd736340f1)
     * [allow some functions to not require user token](https://github.com/prochy-exe/malfetcher/commit/2a3b8c4229984caf7e383072eb5e06af0208c3e3)
     * [use local ip address instead of localhost](https://github.com/prochy-exe/malfetcher/commit/ccb7bfff7d136e9be0204509f18f1646185b5e2c)
     * [print list name when no anime found](https://github.com/prochy-exe/malfetcher/commit/7888e5d7d7100f8e9952210ddbed6705b5dc393b)
     * [drop user list caching](https://github.com/prochy-exe/malfetcher/commit/dd5933434945759bbab8a2fd06ce0511b1ff435e)
     * [allow the mal_to_al_id function to be imported easily](https://github.com/prochy-exe/malfetcher/commit/fbf23bfd384ac53d68dbbe7960d12efa29d88b11)
     * [add function to update progress in users list](https://github.com/prochy-exe/malfetcher/commit/e8fa1dd20054c68f81be4133a9414daa4aad8b29)
     * [regenerate token when expired](https://github.com/prochy-exe/malfetcher/commit/af326c5693fec00c8c90286d63d81782fb90932f)
     * [add state to requests](https://github.com/prochy-exe/malfetcher/commit/76a3e27031ef88d5ba84d7816802647ae55a9e84)
     * [rotate useragents in hopes to avoid captcha](https://github.com/prochy-exe/malfetcher/commit/15ef5a3e866b64cb287264d70946602aa50dea82)
     * [fetch unreleased info all the time](https://github.com/prochy-exe/malfetcher/commit/15d8723dab29a67f0b55f903f8195a47bced6253)
     * [make sure we have a day in the dates](https://github.com/prochy-exe/malfetcher/commit/6ceea01d96ec190b85e0d3950f84a861aa464a73)
     * [Formatting changes](https://github.com/prochy-exe/malfetcher/commit/d06303c44837bc75f788fb29e510dad645c9e801)
-* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+* [1.0.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.1.0/README.md` & `malfetcher-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
+
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
 
 ### Dependencies
 
 * Python(tested on the latest ver.)
@@ -34,47 +35,49 @@
 pip install -e .
 ```
 
 ### Using the library
 
 * To import the library into your code use:
 ```
-import malhelper
+import malfetcher
 ```
 * When importing this library for the first time, you will be taken through the setup process
 
 ### Setting up the MyAnilist developer app
 
 * When the setup process starts, you will be automatically taken to required pages. This process is really simple.
 * When asked for the Client ID, you will be taken to the account developer page.
 * If not logged in, log in first.
 * Then create a new client
 * Choose whatever name you fancy, and for the redirect URL use http://localhost:8888/auth
 * After you save the client, copy the ID and paste it into the terminal
 * After entering the ID you will be taken to an auth page, where you need to allow the app to access your account.
-* Afterwards you will be taken to a redirect page that is momentarily hosted using gevent. (If you have any worries, please see the token_getter.html source code.)
+* Afterwards you will be taken to a redirect page that will automatically send the token to the library.
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.1](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
+* [1.2.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.2.0)
+    * [fix light init](https://github.com/prochy-exe/malfetcher/commit/8f30536fe4f9817eea870cb4d4ea7a248badb0b5)
+* [1.1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
     * [fix typo](https://github.com/prochy-exe/malfetcher/commit/ec8fa79befc1a4190667639920f3b6bd736340f1)
     * [allow some functions to not require user token](https://github.com/prochy-exe/malfetcher/commit/2a3b8c4229984caf7e383072eb5e06af0208c3e3)
     * [use local ip address instead of localhost](https://github.com/prochy-exe/malfetcher/commit/ccb7bfff7d136e9be0204509f18f1646185b5e2c)
     * [print list name when no anime found](https://github.com/prochy-exe/malfetcher/commit/7888e5d7d7100f8e9952210ddbed6705b5dc393b)
     * [drop user list caching](https://github.com/prochy-exe/malfetcher/commit/dd5933434945759bbab8a2fd06ce0511b1ff435e)
     * [allow the mal_to_al_id function to be imported easily](https://github.com/prochy-exe/malfetcher/commit/fbf23bfd384ac53d68dbbe7960d12efa29d88b11)
     * [add function to update progress in users list](https://github.com/prochy-exe/malfetcher/commit/e8fa1dd20054c68f81be4133a9414daa4aad8b29)
     * [regenerate token when expired](https://github.com/prochy-exe/malfetcher/commit/af326c5693fec00c8c90286d63d81782fb90932f)
     * [add state to requests](https://github.com/prochy-exe/malfetcher/commit/76a3e27031ef88d5ba84d7816802647ae55a9e84)
     * [rotate useragents in hopes to avoid captcha](https://github.com/prochy-exe/malfetcher/commit/15ef5a3e866b64cb287264d70946602aa50dea82)
     * [fetch unreleased info all the time](https://github.com/prochy-exe/malfetcher/commit/15d8723dab29a67f0b55f903f8195a47bced6253)
     * [make sure we have a day in the dates](https://github.com/prochy-exe/malfetcher/commit/6ceea01d96ec190b85e0d3950f84a861aa464a73)
     * [Formatting changes](https://github.com/prochy-exe/malfetcher/commit/d06303c44837bc75f788fb29e510dad645c9e801)
-* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+* [1.0.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.1.0/malfetcher/mal_config_utils.py` & `malfetcher-1.2.0/malfetcher/mal_config_utils.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.1.0/malfetcher/mal_fetcher.py` & `malfetcher-1.2.0/malfetcher/mal_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 mal_to_al_status = {v:k for k, v in al_to_mal_status.items()}
 skip_user_statuses = ["REPEATING"]
 
 # Minimal user setup to interact with MyAnimeList API
 config = utils_read_json(config_path)
 if not config or 'myanimelist_client_id' not in config:
     client_id = input("Please input your MyAnimeList API Client ID.\nhttps://myanimelist.net/apiconfig\n")
+    if not config:
+        config = {}
     config['myanimelist_client_id'] = client_id
     utils_save_json(config_path, config)
 else:
     client_id = config['myanimelist_client_id']
 
 # Utils
```

### Comparing `malfetcher-1.1.0/malfetcher/utils.py` & `malfetcher-1.2.0/malfetcher/utils.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.1.0/malfetcher.egg-info/PKG-INFO` & `malfetcher-1.2.0/malfetcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malfetcher
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple library to help you fetch data from MyAnimeList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/prochy-exe/malfetcher
 Project-URL: Documentation, https://github.com/prochy-exe/malfetcher/wiki
 Project-URL: Source, https://github.com/prochy-exe/malfetcher
 Keywords: python,mal,myanimelist
@@ -26,14 +26,15 @@
 Requires-Dist: gevent
 
 # malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
+
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
 
 ### Dependencies
 
 * Python(tested on the latest ver.)
@@ -61,47 +62,49 @@
 pip install -e .
 ```
 
 ### Using the library
 
 * To import the library into your code use:
 ```
-import malhelper
+import malfetcher
 ```
 * When importing this library for the first time, you will be taken through the setup process
 
 ### Setting up the MyAnilist developer app
 
 * When the setup process starts, you will be automatically taken to required pages. This process is really simple.
 * When asked for the Client ID, you will be taken to the account developer page.
 * If not logged in, log in first.
 * Then create a new client
 * Choose whatever name you fancy, and for the redirect URL use http://localhost:8888/auth
 * After you save the client, copy the ID and paste it into the terminal
 * After entering the ID you will be taken to an auth page, where you need to allow the app to access your account.
-* Afterwards you will be taken to a redirect page that is momentarily hosted using gevent. (If you have any worries, please see the token_getter.html source code.)
+* Afterwards you will be taken to a redirect page that will automatically send the token to the library.
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.1](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
+* [1.2.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.2.0)
+    * [fix light init](https://github.com/prochy-exe/malfetcher/commit/8f30536fe4f9817eea870cb4d4ea7a248badb0b5)
+* [1.1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.1.0)
     * [fix typo](https://github.com/prochy-exe/malfetcher/commit/ec8fa79befc1a4190667639920f3b6bd736340f1)
     * [allow some functions to not require user token](https://github.com/prochy-exe/malfetcher/commit/2a3b8c4229984caf7e383072eb5e06af0208c3e3)
     * [use local ip address instead of localhost](https://github.com/prochy-exe/malfetcher/commit/ccb7bfff7d136e9be0204509f18f1646185b5e2c)
     * [print list name when no anime found](https://github.com/prochy-exe/malfetcher/commit/7888e5d7d7100f8e9952210ddbed6705b5dc393b)
     * [drop user list caching](https://github.com/prochy-exe/malfetcher/commit/dd5933434945759bbab8a2fd06ce0511b1ff435e)
     * [allow the mal_to_al_id function to be imported easily](https://github.com/prochy-exe/malfetcher/commit/fbf23bfd384ac53d68dbbe7960d12efa29d88b11)
     * [add function to update progress in users list](https://github.com/prochy-exe/malfetcher/commit/e8fa1dd20054c68f81be4133a9414daa4aad8b29)
     * [regenerate token when expired](https://github.com/prochy-exe/malfetcher/commit/af326c5693fec00c8c90286d63d81782fb90932f)
     * [add state to requests](https://github.com/prochy-exe/malfetcher/commit/76a3e27031ef88d5ba84d7816802647ae55a9e84)
     * [rotate useragents in hopes to avoid captcha](https://github.com/prochy-exe/malfetcher/commit/15ef5a3e866b64cb287264d70946602aa50dea82)
     * [fetch unreleased info all the time](https://github.com/prochy-exe/malfetcher/commit/15d8723dab29a67f0b55f903f8195a47bced6253)
     * [make sure we have a day in the dates](https://github.com/prochy-exe/malfetcher/commit/6ceea01d96ec190b85e0d3950f84a861aa464a73)
     * [Formatting changes](https://github.com/prochy-exe/malfetcher/commit/d06303c44837bc75f788fb29e510dad645c9e801)
-* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+* [1.0.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.1.0/pyproject.toml` & `malfetcher-1.2.0/pyproject.toml`

 * *Files identical despite different names*

