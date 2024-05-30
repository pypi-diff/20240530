# Comparing `tmp/salve_ipc-0.1.0.tar.gz` & `tmp/salve_ipc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salve_ipc-0.1.0.tar", last modified: Wed May 29 14:20:46 2024, max compression
+gzip compressed data, was "salve_ipc-0.2.1.tar", last modified: Thu May 30 05:26:04 2024, max compression
```

## Comparing `salve_ipc-0.1.0.tar` & `salve_ipc-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:20:46.195655 salve_ipc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-29 14:20:46.195655 salve_ipc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:20:46.195655 salve_ipc-0.1.0/salve_ipc/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/salve_ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/salve_ipc/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/salve_ipc/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/salve_ipc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/salve_ipc/server_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:20:46.195655 salve_ipc-0.1.0/salve_ipc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-29 14:20:46.000000 salve_ipc-0.1.0/salve_ipc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 14:20:46.000000 salve_ipc-0.1.0/salve_ipc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:20:46.000000 salve_ipc-0.1.0/salve_ipc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 14:20:46.000000 salve_ipc-0.1.0/salve_ipc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 14:20:46.000000 salve_ipc-0.1.0/salve_ipc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:20:46.195655 salve_ipc-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 14:20:38.000000 salve_ipc-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/salve_ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/salve_ipc/highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/highlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/highlight/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/salve_ipc/server_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/salve_ipc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-30 05:26:03.000000 salve_ipc-0.2.1/salve_ipc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 05:26:03.000000 salve_ipc-0.2.1/salve_ipc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:26:03.000000 salve_ipc-0.2.1/salve_ipc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 05:26:03.000000 salve_ipc-0.2.1/salve_ipc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 05:26:03.000000 salve_ipc-0.2.1/salve_ipc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:26:04.052316 salve_ipc-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-30 05:25:50.000000 salve_ipc-0.2.1/setup.py
```

### Comparing `salve_ipc-0.1.0/LICENSE` & `salve_ipc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.1.0/PKG-INFO` & `salve_ipc-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,61 @@
-Metadata-Version: 2.1
-Name: salve_ipc
-Version: 0.1.0
-Summary: A module that makes IPC for your code editor easy providing autocompletion and replacement suggestions
-Home-page: https://github.com/Moosems/salve
-Author: Moosems
-Author-email: moosems.j@gmail.com
-License: MIT license
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Typing :: Typed
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">Salve</h1>
+<h1 align="center">Salve v0.2.0</h1>
 
 > **Note**
 > This package does not work on Windows machines as `Selector.select()` does not work on them.
 
 # Installation
 
-In the Command Line, paste the following: `pip install salve_ipc` (NOT YET WORKING).
+In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocomplete and, in the future, syntax highlighting.
+Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
 - "autocomplete"
 - "replacements"
 - "highlight"
 
+### `generic_tokens`
+
+The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
+
 ### `Request` and `Response` TypedDict classes
 
 The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
 
+### `Token` dataclass
+
+The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
+### `tokens_from_result(result: list[str]) -> list[Token]`
+
+The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                              | Arguments                                                                                                                                                                         |
-| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                 | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                            | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                  | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                        | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists                                                                                                           | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                      | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
+| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
 from os import set_blocking
 from selectors import EVENT_READ, DefaultSelector
 from sys import stdin, stdout
@@ -104,20 +100,18 @@
     stdout.flush()
 ```
 
 ## How to run and contribute
 
 ### Running
 
-To run the example, move `examples/example_usage.py` to the root directory and run with python. The project uses only standard library modules, so there are no external dependencies.
+To run the example, move `examples/example_usage.py` to the root directory and run with python.
 
 To test newer features or test code in a Pull Review, do the same but move it back after if you plan to make a PR.
 
 ### Contributing
 
-To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so we can discuss it.
+To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so it can be discussed. Note that whenever and wherever possible you should try to use stdlib modules rather than external ones.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](./LISCENSE).
-
-
```

### Comparing `salve_ipc-0.1.0/README.md` & `salve_ipc-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,77 @@
-<h1 align="center">Salve</h1>
+Metadata-Version: 2.1
+Name: salve_ipc
+Version: 0.2.1
+Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
+Home-page: https://github.com/Moosems/salve
+Author: Moosems
+Author-email: moosems.j@gmail.com
+License: MIT license
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">Salve v0.2.0</h1>
 
 > **Note**
 > This package does not work on Windows machines as `Selector.select()` does not work on them.
 
 # Installation
 
-In the Command Line, paste the following: `pip install salve_ipc` (NOT YET WORKING).
+In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocomplete and, in the future, syntax highlighting.
+Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
 - "autocomplete"
 - "replacements"
 - "highlight"
 
+### `generic_tokens`
+
+The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
+
 ### `Request` and `Response` TypedDict classes
 
 The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
 
+### `Token` dataclass
+
+The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
+### `tokens_from_result(result: list[str]) -> list[Token]`
+
+The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                              | Arguments                                                                                                                                                                         |
-| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                 | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                            | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                  | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                        | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists                                                                                                           | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                      | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
+| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
 from os import set_blocking
 from selectors import EVENT_READ, DefaultSelector
 from sys import stdin, stdout
@@ -88,18 +116,20 @@
     stdout.flush()
 ```
 
 ## How to run and contribute
 
 ### Running
 
-To run the example, move `examples/example_usage.py` to the root directory and run with python. The project uses only standard library modules, so there are no external dependencies.
+To run the example, move `examples/example_usage.py` to the root directory and run with python.
 
 To test newer features or test code in a Pull Review, do the same but move it back after if you plan to make a PR.
 
 ### Contributing
 
-To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so we can discuss it.
+To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so it can be discussed. Note that whenever and wherever possible you should try to use stdlib modules rather than external ones.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](./LISCENSE).
+
+
```

### Comparing `salve_ipc-0.1.0/salve_ipc/server.py` & `salve_ipc-0.2.1/salve_ipc/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from difflib import restore
 from json import dumps, loads
 from os import set_blocking
 from selectors import EVENT_READ, DefaultSelector
 from sys import exit, stdin, stdout
 from time import time
 
+from highlight import Token, get_highlights
 from misc import COMMANDS, Message, Request, Response
-from server_functions import (
-    Token,
-    find_autocompletions,
-    get_highlights,
-    get_replacements,
-)
+from server_functions import find_autocompletions, get_replacements
 
 
 class Handler:
+    """Handles input from the user and returns output from special functions designed to make the job easy. Not an external API."""
+
     def __init__(self) -> None:
         set_blocking(stdin.fileno(), False)
         set_blocking(stdout.fileno(), False)
         self.selector = DefaultSelector()
         self.selector.register(stdin, EVENT_READ)
 
         self.id_list: list[int] = []
@@ -67,15 +65,15 @@
 
     def handle_request(self, request: Request) -> None:
         file: str = request["file"]
         result: list[str] = []
         command: str = request["command"]
         cancelled: bool = False
 
-        if not file in self.files:
+        if file not in self.files:
             response: Response = {
                 "id": request["id"],
                 "type": "response",
                 "cancelled": True,
                 "command": command,
                 "result": result,
             }
```

### Comparing `salve_ipc-0.1.0/salve_ipc.egg-info/PKG-INFO` & `salve_ipc-0.2.1/salve_ipc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 Metadata-Version: 2.1
 Name: salve-ipc
-Version: 0.1.0
-Summary: A module that makes IPC for your code editor easy providing autocompletion and replacement suggestions
+Version: 0.2.1
+Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
 Home-page: https://github.com/Moosems/salve
 Author: Moosems
 Author-email: moosems.j@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">Salve</h1>
+<h1 align="center">Salve v0.2.0</h1>
 
 > **Note**
 > This package does not work on Windows machines as `Selector.select()` does not work on them.
 
 # Installation
 
-In the Command Line, paste the following: `pip install salve_ipc` (NOT YET WORKING).
+In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocomplete and, in the future, syntax highlighting.
+Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
 - "autocomplete"
 - "replacements"
 - "highlight"
 
+### `generic_tokens`
+
+The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
+
 ### `Request` and `Response` TypedDict classes
 
 The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
 
+### `Token` dataclass
+
+The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
+### `tokens_from_result(result: list[str]) -> list[Token]`
+
+The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                              | Arguments                                                                                                                                                                         |
-| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                 | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                            | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                  | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                        | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists                                                                                                           | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                      | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
+| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
 from os import set_blocking
 from selectors import EVENT_READ, DefaultSelector
 from sys import stdin, stdout
@@ -104,20 +116,20 @@
     stdout.flush()
 ```
 
 ## How to run and contribute
 
 ### Running
 
-To run the example, move `examples/example_usage.py` to the root directory and run with python. The project uses only standard library modules, so there are no external dependencies.
+To run the example, move `examples/example_usage.py` to the root directory and run with python.
 
 To test newer features or test code in a Pull Review, do the same but move it back after if you plan to make a PR.
 
 ### Contributing
 
-To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so we can discuss it.
+To contribute, fork the repository, make your changes, and then make a pull request. If you want to add a feature, please open an issue first so it can be discussed. Note that whenever and wherever possible you should try to use stdlib modules rather than external ones.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](./LISCENSE).
```

### Comparing `salve_ipc-0.1.0/setup.py` & `salve_ipc-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# pip install . --break-system-packages --no-build-isolation
+# pip uninstall salve_ipc -y --break-system-packages; pip install . --break-system-packages --no-build-isolation
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="salve_ipc",
-    version="0.1.0",
-    description="A module that makes IPC for your code editor easy providing autocompletion and replacement suggestions",
+    version="0.2.1",
+    description="A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor",
     author="Moosems",
     author_email="moosems.j@gmail.com",
     url="https://github.com/Moosems/salve",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[line for line in open("requirements.txt").readlines()],
     python_requires=">=3.9",
     license="MIT license",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Typing :: Typed",
     ],
     packages=["salve_ipc"],
-    package_data={"salve_ipc": ["./*"]},
+    package_data={"salve_ipc": ["./*", "./highlight/*"]},
 )
```

