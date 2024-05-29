# Comparing `tmp/gpt_automation-0.1.6.tar.gz` & `tmp/gpt_automation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_automation-0.1.6.tar", last modified: Wed Mar  6 16:45:43 2024, max compression
+gzip compressed data, was "gpt_automation-0.1.7.tar", last modified: Wed Mar  6 17:52:52 2024, max compression
```

## Comparing `gpt_automation-0.1.6.tar` & `gpt_automation-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 16:45:43.867735 gpt_automation-0.1.6/
--rw-rw-rw-   0        0        0    11560 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       61 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    17151 2024-03-06 16:45:43.867735 gpt_automation-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3559 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-06 16:45:43.823743 gpt_automation-0.1.6/gpt_automation/
--rw-rw-rw-   0        0        0        0 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/gpt_automation/__init__.py
--rw-rw-rw-   0        0        0      925 2024-03-06 13:44:54.000000 gpt_automation-0.1.6/gpt_automation/git_tools.py
--rw-rw-rw-   0        0        0     4310 2024-03-06 16:37:55.000000 gpt_automation-0.1.6/gpt_automation/ignore_walk.py
--rw-rw-rw-   0        0        0     5461 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/gpt_automation/main.py
--rw-rw-rw-   0        0        0     1613 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/gpt_automation/project_info.py
-drwxrwxrwx   0        0        0        0 2024-03-06 16:45:43.863736 gpt_automation-0.1.6/gpt_automation/sample_config/
--rw-rw-rw-   0        0        0      132 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/gpt_automation/sample_config/black_list.txt
--rw-rw-rw-   0        0        0       36 2024-03-06 12:25:49.000000 gpt_automation-0.1.6/gpt_automation/sample_config/white_list.txt
-drwxrwxrwx   0        0        0        0 2024-03-06 16:45:43.861735 gpt_automation-0.1.6/gpt_automation.egg-info/
--rw-rw-rw-   0        0        0    17151 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-03-06 16:45:43.000000 gpt_automation-0.1.6/gpt_automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2024-03-06 16:43:23.000000 gpt_automation-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      432 2024-03-06 16:45:43.875269 gpt_automation-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      258 2024-03-06 16:43:35.000000 gpt_automation-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-06 16:45:43.866735 gpt_automation-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-03-06 13:02:58.000000 gpt_automation-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-06 14:12:08.000000 gpt_automation-0.1.6/tests/ignore_walk_extras_test.py
--rw-rw-rw-   0        0        0     7023 2024-03-06 13:02:58.000000 gpt_automation-0.1.6/tests/ignore_walk_test.py
--rw-rw-rw-   0        0        0     1065 2024-03-06 13:02:58.000000 gpt_automation-0.1.6/tests/main_run.py
--rw-rw-rw-   0        0        0     5028 2024-03-06 16:26:36.000000 gpt_automation-0.1.6/tests/main_test.py
+drwxrwxrwx   0        0        0        0 2024-03-06 17:52:52.443514 gpt_automation-0.1.7/
+-rw-rw-rw-   0        0        0    11560 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    17606 2024-03-06 17:52:52.443514 gpt_automation-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4014 2024-03-06 17:50:53.000000 gpt_automation-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-03-06 17:52:52.408644 gpt_automation-0.1.7/gpt_automation/
+-rw-rw-rw-   0        0        0        0 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/gpt_automation/__init__.py
+-rw-rw-rw-   0        0        0      925 2024-03-06 13:44:54.000000 gpt_automation-0.1.7/gpt_automation/git_tools.py
+-rw-rw-rw-   0        0        0     4765 2024-03-06 17:40:25.000000 gpt_automation-0.1.7/gpt_automation/ignore_walk.py
+-rw-rw-rw-   0        0        0     5461 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/gpt_automation/main.py
+-rw-rw-rw-   0        0        0     1613 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/gpt_automation/project_info.py
+drwxrwxrwx   0        0        0        0 2024-03-06 17:52:52.437511 gpt_automation-0.1.7/gpt_automation/sample_config/
+-rw-rw-rw-   0        0        0      132 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/gpt_automation/sample_config/black_list.txt
+-rw-rw-rw-   0        0        0       36 2024-03-06 12:25:49.000000 gpt_automation-0.1.7/gpt_automation/sample_config/white_list.txt
+drwxrwxrwx   0        0        0        0 2024-03-06 17:52:52.435509 gpt_automation-0.1.7/gpt_automation.egg-info/
+-rw-rw-rw-   0        0        0    17606 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-03-06 17:52:52.000000 gpt_automation-0.1.7/gpt_automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2024-03-06 17:52:26.000000 gpt_automation-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      432 2024-03-06 17:52:52.446506 gpt_automation-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      258 2024-03-06 17:52:09.000000 gpt_automation-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-06 17:52:52.440509 gpt_automation-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-06 13:02:58.000000 gpt_automation-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-06 14:12:08.000000 gpt_automation-0.1.7/tests/ignore_walk_extras_test.py
+-rw-rw-rw-   0        0        0     7023 2024-03-06 13:02:58.000000 gpt_automation-0.1.7/tests/ignore_walk_test.py
+-rw-rw-rw-   0        0        0     1065 2024-03-06 13:02:58.000000 gpt_automation-0.1.7/tests/main_run.py
+-rw-rw-rw-   0        0        0     5028 2024-03-06 16:26:36.000000 gpt_automation-0.1.7/tests/main_test.py
```

### Comparing `gpt_automation-0.1.6/LICENSE` & `gpt_automation-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/PKG-INFO` & `gpt_automation-0.1.7/gpt_automation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gpt_automation
-Version: 0.1.6
+Name: gpt-automation
+Version: 0.1.7
 Summary: GPT directory structure and file contents prompt generator
 Home-page: https://github.com/vrocky/gpt-automation/
 Author: Vinit
 Author-email: Vinit <author@example.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -210,72 +210,81 @@
         
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: gitignore_parser==0.1.11
 
+<h1>GPT Automation</h1>
 
-# GPT Automation
+This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist or a .gptignore file. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
 
-This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
+<h2>Installation</h2>
 
-## Installation
-
-### Pipx Installation
+<h3>Pipx Installation</h3>
 
 We recommend installing GPT Automation through pipx, a package manager for running applications written in Python. If you haven't installed pipx, first install it by running:
 
 ```bash
 python3 -m pip install --user pipx
 python3 -m pipx ensurepath
 ```
 
 Next, install the GPT Automation package with:
 
 ```bash
 pipx install gpt-automation
 ```
 
-Manual InstallationTo manually install the project, run the following command from the project's root directory:
+<h3>Manual Installation</h3>
+
+To manually install the project, run the following command from the project's root directory:
 
 ```bash
 python setup.py install
 ```
 
 This will install the project as a package, making the main module accessible from the command line.
 
-InitializationTo initialize the .gpt directory with sample blacklist and whitelist files, run:
+<h3>Initialization</h3>
+
+To initialize the .gpt directory with sample blacklist, whitelist, and .gptignore files, run:
 
 ```bash
 autogpt init [--profile PROFILE_NAME]
 ```
 
-This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt and sample_config/white_list.txt into this directory.
+This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt, sample_config/white_list.txt, and a sample .gptignore file into this directory.
 
-Prompt GenerationGPT Automation provides two types of prompts:
+<h3>Prompt Generation</h3>
 
-Full PromptIncludes both the directory structure and the contents of all files. To generate a full prompt, use:
+GPT Automation provides two types of prompts:
+
+- Full Prompt: Includes both the directory structure and the contents of all files. To generate a full prompt, use:
 
 ```bash
 autogpt prompt-all [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
-Directory-Only PromptOnly includes the directory structure. To generate a directory-only prompt, use:
+- Directory-Only Prompt: Only includes the directory structure. To generate a directory-only prompt, use:
 
 ```bash
 autogpt prompt-dir [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
 In both cases, the generated prompt is automatically copied to the clipboard.
 
-Options- --path: Specifies the path to your project's root directory. Defaults to the current directory.
+<h3>Options</h3>
+
+- --path: Specifies the path to your project's root directory. Defaults to the current directory.
 - --profile: Specifies the name of the profile to use. This allows for different configurations for different projects or use cases.
 
-Blacklists and WhitelistsThe blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. If a file matches patterns in both lists, it will be included in the prompt.
+<h3>Blacklists, Whitelists, and .gptignore</h3>
+
+The blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. The .gptignore file functions similarly to a blacklist, offering a more flexible and familiar way to specify files and directories to ignore. If a file matches patterns in both lists, it will be included in the prompt.
 
 Sample Blacklist (black_list.txt)```plaintext
 *prompts*
 *.idea*
 *__pycache__*
 *.xml
 *.gitignore*
@@ -295,17 +304,30 @@
 *.groovy
 *.java
 *.py
 *.ini
 *.txt
 ```
 
-OutputThe generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
+Sample .gptignore
+
+```plaintext
+# Ignore all markdown files
+*.md
+
+# Ignore specific directories
+node_modules/
+build/
+```
+
+<h3>Output</h3>
+
+The generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
 
-```python
+```dir
 Directory Structure:
 ./
     file_1.py
     file_2.py
     dir_1/
         file_1.py
 
@@ -316,10 +338,10 @@
 ==========file_2.py:
 # Code for file_2.py
 
 ==========dir_1/file_1.py:
 # Code for dir_1/file_1.py
 ```
 
-This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the `init`, `prompt-all`, and `prompt-dir` commands with their respective options. It also explains the purpose of the blacklist and whitelist files, and how the output will be formatted and copied to the clipboard.
+This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the init, prompt-all, and prompt-dir commands with their respective options. It also explains the purpose of the blacklist, whitelist, and .gptignore files, and how the output will be formatted and copied to the clipboard.
```

### Comparing `gpt_automation-0.1.6/README.md` & `gpt_automation-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,74 @@
+<h1>GPT Automation</h1>
 
-# GPT Automation
+This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist or a .gptignore file. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
 
-This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
+<h2>Installation</h2>
 
-## Installation
-
-### Pipx Installation
+<h3>Pipx Installation</h3>
 
 We recommend installing GPT Automation through pipx, a package manager for running applications written in Python. If you haven't installed pipx, first install it by running:
 
 ```bash
 python3 -m pip install --user pipx
 python3 -m pipx ensurepath
 ```
 
 Next, install the GPT Automation package with:
 
 ```bash
 pipx install gpt-automation
 ```
 
-Manual InstallationTo manually install the project, run the following command from the project's root directory:
+<h3>Manual Installation</h3>
+
+To manually install the project, run the following command from the project's root directory:
 
 ```bash
 python setup.py install
 ```
 
 This will install the project as a package, making the main module accessible from the command line.
 
-InitializationTo initialize the .gpt directory with sample blacklist and whitelist files, run:
+<h3>Initialization</h3>
+
+To initialize the .gpt directory with sample blacklist, whitelist, and .gptignore files, run:
 
 ```bash
 autogpt init [--profile PROFILE_NAME]
 ```
 
-This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt and sample_config/white_list.txt into this directory.
+This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt, sample_config/white_list.txt, and a sample .gptignore file into this directory.
 
-Prompt GenerationGPT Automation provides two types of prompts:
+<h3>Prompt Generation</h3>
 
-Full PromptIncludes both the directory structure and the contents of all files. To generate a full prompt, use:
+GPT Automation provides two types of prompts:
+
+- Full Prompt: Includes both the directory structure and the contents of all files. To generate a full prompt, use:
 
 ```bash
 autogpt prompt-all [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
-Directory-Only PromptOnly includes the directory structure. To generate a directory-only prompt, use:
+- Directory-Only Prompt: Only includes the directory structure. To generate a directory-only prompt, use:
 
 ```bash
 autogpt prompt-dir [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
 In both cases, the generated prompt is automatically copied to the clipboard.
 
-Options- --path: Specifies the path to your project's root directory. Defaults to the current directory.
+<h3>Options</h3>
+
+- --path: Specifies the path to your project's root directory. Defaults to the current directory.
 - --profile: Specifies the name of the profile to use. This allows for different configurations for different projects or use cases.
 
-Blacklists and WhitelistsThe blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. If a file matches patterns in both lists, it will be included in the prompt.
+<h3>Blacklists, Whitelists, and .gptignore</h3>
+
+The blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. The .gptignore file functions similarly to a blacklist, offering a more flexible and familiar way to specify files and directories to ignore. If a file matches patterns in both lists, it will be included in the prompt.
 
 Sample Blacklist (black_list.txt)```plaintext
 *prompts*
 *.idea*
 *__pycache__*
 *.xml
 *.gitignore*
@@ -79,17 +88,30 @@
 *.groovy
 *.java
 *.py
 *.ini
 *.txt
 ```
 
-OutputThe generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
+Sample .gptignore
+
+```plaintext
+# Ignore all markdown files
+*.md
+
+# Ignore specific directories
+node_modules/
+build/
+```
+
+<h3>Output</h3>
+
+The generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
 
-```python
+```dir
 Directory Structure:
 ./
     file_1.py
     file_2.py
     dir_1/
         file_1.py
 
@@ -100,10 +122,10 @@
 ==========file_2.py:
 # Code for file_2.py
 
 ==========dir_1/file_1.py:
 # Code for dir_1/file_1.py
 ```
 
-This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the `init`, `prompt-all`, and `prompt-dir` commands with their respective options. It also explains the purpose of the blacklist and whitelist files, and how the output will be formatted and copied to the clipboard.
+This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the init, prompt-all, and prompt-dir commands with their respective options. It also explains the purpose of the blacklist, whitelist, and .gptignore files, and how the output will be formatted and copied to the clipboard.
```

### Comparing `gpt_automation-0.1.6/gpt_automation/git_tools.py` & `gpt_automation-0.1.7/gpt_automation/git_tools.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/gpt_automation/ignore_walk.py` & `gpt_automation-0.1.7/gpt_automation/ignore_walk.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 import pathlib
 import gitignore_parser
 import re
 
 from gpt_automation.git_tools import find_git_root  # Ensure this is defined somewhere in your code
 
 class IgnoreMatch:
-    def __init__(self, gitignore_path):
-        self.gitignore_path = gitignore_path
-        self.match = gitignore_parser.parse_gitignore(gitignore_path)
-
-def load_gitignore(gitignore_path):
-    if gitignore_path is not None:
-        return IgnoreMatch(gitignore_path)
+    def __init__(self, ignore_paths):
+        # Changed to support multiple ignore paths
+        self.ignore_paths = ignore_paths
+        self.matches = [gitignore_parser.parse_gitignore(path) for path in ignore_paths]
+
+    def match(self, file_path):
+        # Check against all provided ignore files
+        return any(match(file_path) for match in self.matches)
+
+def load_ignore_matches(ignore_paths):
+    if ignore_paths:
+        return IgnoreMatch(ignore_paths)
     else:
         return None
 
-def matches_any_pattern(file_path, gitignore_match_collection):
-    for match in gitignore_match_collection:
+def matches_any_pattern(file_path, ignore_match_collection):
+    for match in ignore_match_collection:
         if match.match(file_path):
             return True
     return False
 
 def compile_patterns(patterns_list):
     compiled_patterns = [re.compile(fnmatch.translate(pattern)) for pattern in patterns_list]
     return compiled_patterns
@@ -31,81 +36,85 @@
     file_path = file_path.replace("\\", "/")
     file_path = file_path.lstrip("/")
     for pattern in patterns:
         if pattern.fullmatch(file_path):
             return True
     return False
 
-def should_ignore_by_git(file_path, gitignore_matches_stack):
-    for gitignore_path in reversed(gitignore_matches_stack):
-        if gitignore_path is not None:
-            ignore_match = load_gitignore(gitignore_path)
+def should_ignore_by_ignore_files(file_path, ignore_matches_stack):
+    for ignore_paths in reversed(ignore_matches_stack):
+        if ignore_paths:
+            ignore_match = load_ignore_matches(ignore_paths)
             if ignore_match and ignore_match.match(file_path):
                 return True
     return False
 
 def should_ignore_by_black_list(file_path, black_list_patterns):
     return matches_list_pattern(file_path, black_list_patterns)
 
 def filter_with_white_list(filtered_filenames, white_list_patterns):
     if white_list_patterns:
         return [filename for filename in filtered_filenames if matches_list_pattern(filename, white_list_patterns)]
     else:
         return filtered_filenames
 
-def ignore_walk(path, black_list, white_list):
+def ignore_walk(path, black_list, white_list, ignore_file_names=['.gitignore',".gptignore"]):
     black_list_patterns = compile_patterns(black_list)
     white_list_patterns = compile_patterns(white_list) if white_list else None
 
     visited = set()
-    gitignore_match_stack = init_gitignore_stack(path)
+    ignore_matches_stack = init_ignore_stack(path, ignore_file_names)
 
     def walk(dirpath, depth):
         if dirpath in visited:
             return
         visited.add(dirpath)
 
-        local_gitignore_path = os.path.join(dirpath, '.gitignore')
-        if os.path.exists(local_gitignore_path):
-            gitignore_match_stack.append(local_gitignore_path)
-        else:
-            gitignore_match_stack.append(None)
+        local_ignore_paths = find_ignore_files(dirpath, ignore_file_names)
+        ignore_matches_stack.append(local_ignore_paths if local_ignore_paths else None)
 
         dirnames, filenames = [], []
         for entry in os.scandir(dirpath):
             if entry.is_dir(follow_symlinks=False):
                 dirnames.append(entry.name)
             elif entry.is_file():
                 filenames.append(entry.name)
 
-        # Filter filenames based on gitignore and blacklist
-        filtered_filenames = [filename for filename in filenames if not should_ignore_by_git(os.path.join(dirpath, filename), gitignore_match_stack) and not should_ignore_by_black_list(os.path.join(dirpath, filename), black_list_patterns)]
-        # Filter filenames with white list patterns
+        # Filter filenames based on ignore files, blacklist, and whitelist
+        filtered_filenames = [filename for filename in filenames if not should_ignore_by_ignore_files(os.path.join(dirpath, filename), ignore_matches_stack) and not should_ignore_by_black_list(os.path.join(dirpath, filename), black_list_patterns)]
         filtered_filenames = filter_with_white_list(filtered_filenames, white_list_patterns)
 
         yield dirpath, dirnames, filtered_filenames
 
         for dirname in dirnames:
             full_dir_path = os.path.join(dirpath, dirname)
-            if not should_ignore_by_git(full_dir_path, gitignore_match_stack) and not should_ignore_by_black_list(full_dir_path, black_list_patterns):
+            if not should_ignore_by_ignore_files(full_dir_path, ignore_matches_stack) and not should_ignore_by_black_list(full_dir_path, black_list_patterns):
                 yield from walk(full_dir_path, depth + 1)
 
-        gitignore_match_stack.pop()
+        ignore_matches_stack.pop()
 
     return walk(path, 0)
 
-def init_gitignore_stack(start_path):
+def find_ignore_files(dirpath, ignore_file_names):
+    ignore_paths = []
+    for ignore_file_name in ignore_file_names:
+        for entry in os.scandir(dirpath):
+            if entry.is_file() and entry.name in ignore_file_names:
+                ignore_paths.append(entry.path)
+    return ignore_paths
+
+def init_ignore_stack(start_path, ignore_file_names):
     git_root = find_git_root(start_path)
-    gitignore_match_stack = []
+    ignore_matches_stack = []
     if git_root:
         relative_path = os.path.relpath(start_path, git_root)
         current_path = git_root
         for part in pathlib.Path(relative_path).parts:
             current_path = os.path.join(current_path, part)
-            gitignore_path = os.path.join(current_path, '.gitignore')
-            if os.path.exists(gitignore_path):
-                gitignore_match_stack.append(gitignore_path)
+            ignore_paths = find_ignore_files(current_path, ignore_file_names)
+            if ignore_paths:
+                ignore_matches_stack.append(ignore_paths)
             else:
-                gitignore_match_stack.append(None)
+                ignore_matches_stack.append(None)
     else:
-        gitignore_match_stack.append(None)
-    return gitignore_match_stack
+        ignore_matches_stack.append(None)
+    return ignore_matches_stack
```

### Comparing `gpt_automation-0.1.6/gpt_automation/main.py` & `gpt_automation-0.1.7/gpt_automation/main.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/gpt_automation/project_info.py` & `gpt_automation-0.1.7/gpt_automation/project_info.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/gpt_automation.egg-info/PKG-INFO` & `gpt_automation-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gpt-automation
-Version: 0.1.6
+Name: gpt_automation
+Version: 0.1.7
 Summary: GPT directory structure and file contents prompt generator
 Home-page: https://github.com/vrocky/gpt-automation/
 Author: Vinit
 Author-email: Vinit <author@example.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -210,72 +210,81 @@
         
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: gitignore_parser==0.1.11
 
+<h1>GPT Automation</h1>
 
-# GPT Automation
+This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist or a .gptignore file. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
 
-This Python-based project provides a way to automatically generate a project structure, including all directories and files, while ignoring certain unwanted files or directories as specified in a blacklist. It also offers the capability to generate file contents, allowing users to copy either the entire project structure or just the directory structure to the clipboard.
+<h2>Installation</h2>
 
-## Installation
-
-### Pipx Installation
+<h3>Pipx Installation</h3>
 
 We recommend installing GPT Automation through pipx, a package manager for running applications written in Python. If you haven't installed pipx, first install it by running:
 
 ```bash
 python3 -m pip install --user pipx
 python3 -m pipx ensurepath
 ```
 
 Next, install the GPT Automation package with:
 
 ```bash
 pipx install gpt-automation
 ```
 
-Manual InstallationTo manually install the project, run the following command from the project's root directory:
+<h3>Manual Installation</h3>
+
+To manually install the project, run the following command from the project's root directory:
 
 ```bash
 python setup.py install
 ```
 
 This will install the project as a package, making the main module accessible from the command line.
 
-InitializationTo initialize the .gpt directory with sample blacklist and whitelist files, run:
+<h3>Initialization</h3>
+
+To initialize the .gpt directory with sample blacklist, whitelist, and .gptignore files, run:
 
 ```bash
 autogpt init [--profile PROFILE_NAME]
 ```
 
-This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt and sample_config/white_list.txt into this directory.
+This creates a .gpt directory (or a profile-specific directory under .gpt/other_profiles/ if --profile is specified) if it doesn't already exist, copying sample_config/black_list.txt, sample_config/white_list.txt, and a sample .gptignore file into this directory.
 
-Prompt GenerationGPT Automation provides two types of prompts:
+<h3>Prompt Generation</h3>
 
-Full PromptIncludes both the directory structure and the contents of all files. To generate a full prompt, use:
+GPT Automation provides two types of prompts:
+
+- Full Prompt: Includes both the directory structure and the contents of all files. To generate a full prompt, use:
 
 ```bash
 autogpt prompt-all [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
-Directory-Only PromptOnly includes the directory structure. To generate a directory-only prompt, use:
+- Directory-Only Prompt: Only includes the directory structure. To generate a directory-only prompt, use:
 
 ```bash
 autogpt prompt-dir [--path PROJECT_PATH] [--profile PROFILE_NAME]
 ```
 
 In both cases, the generated prompt is automatically copied to the clipboard.
 
-Options- --path: Specifies the path to your project's root directory. Defaults to the current directory.
+<h3>Options</h3>
+
+- --path: Specifies the path to your project's root directory. Defaults to the current directory.
 - --profile: Specifies the name of the profile to use. This allows for different configurations for different projects or use cases.
 
-Blacklists and WhitelistsThe blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. If a file matches patterns in both lists, it will be included in the prompt.
+<h3>Blacklists, Whitelists, and .gptignore</h3>
+
+The blacklist file contains patterns of files and directories to ignore during prompt generation, whereas the whitelist file contains patterns of files and directories to include. The .gptignore file functions similarly to a blacklist, offering a more flexible and familiar way to specify files and directories to ignore. If a file matches patterns in both lists, it will be included in the prompt.
 
 Sample Blacklist (black_list.txt)```plaintext
 *prompts*
 *.idea*
 *__pycache__*
 *.xml
 *.gitignore*
@@ -295,17 +304,30 @@
 *.groovy
 *.java
 *.py
 *.ini
 *.txt
 ```
 
-OutputThe generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
+Sample .gptignore
+
+```plaintext
+# Ignore all markdown files
+*.md
+
+# Ignore specific directories
+node_modules/
+build/
+```
+
+<h3>Output</h3>
+
+The generated code, including the directory structure and file contents, will be copied to the clipboard in the following format:
 
-```python
+```dir
 Directory Structure:
 ./
     file_1.py
     file_2.py
     dir_1/
         file_1.py
 
@@ -316,10 +338,10 @@
 ==========file_2.py:
 # Code for file_2.py
 
 ==========dir_1/file_1.py:
 # Code for dir_1/file_1.py
 ```
 
-This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the `init`, `prompt-all`, and `prompt-dir` commands with their respective options. It also explains the purpose of the blacklist and whitelist files, and how the output will be formatted and copied to the clipboard.
+This README provides detailed instructions for installing and using the GPT Automation tool, including how to use the init, prompt-all, and prompt-dir commands with their respective options. It also explains the purpose of the blacklist, whitelist, and .gptignore files, and how the output will be formatted and copied to the clipboard.
```

### Comparing `gpt_automation-0.1.6/gpt_automation.egg-info/SOURCES.txt` & `gpt_automation-0.1.7/gpt_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/tests/ignore_walk_extras_test.py` & `gpt_automation-0.1.7/tests/ignore_walk_extras_test.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/tests/ignore_walk_test.py` & `gpt_automation-0.1.7/tests/ignore_walk_test.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/tests/main_run.py` & `gpt_automation-0.1.7/tests/main_run.py`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.6/tests/main_test.py` & `gpt_automation-0.1.7/tests/main_test.py`

 * *Files identical despite different names*

