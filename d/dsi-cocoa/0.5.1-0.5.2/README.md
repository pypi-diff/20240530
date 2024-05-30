# Comparing `tmp/dsi_cocoa-0.5.1.tar.gz` & `tmp/dsi_cocoa-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.5.1.tar", last modified: Thu May 16 16:51:26 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.5.2.tar", last modified: Thu May 30 17:41:18 2024, max compression
```

## Comparing `dsi_cocoa-0.5.1.tar` & `dsi_cocoa-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/error.badges.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.298008 dsi_cocoa-0.5.1/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 16:51:21.000000 dsi_cocoa-0.5.1/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:26.302008 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 16:51:26.000000 dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.138086 dsi_cocoa-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.github/workflows/error.badges.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.138086 dsi_cocoa-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-30 17:41:13.000000 dsi_cocoa-0.5.2/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:18.142087 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 17:41:18.000000 dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.5.1/.github/workflows/error.badges.yml` & `dsi_cocoa-0.5.2/.github/workflows/error.badges.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.5.2/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.5.2/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/.gitignore` & `dsi_cocoa-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/.pre-commit-config.yaml` & `dsi_cocoa-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/PKG-INFO` & `dsi_cocoa-0.5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.5.1
+Version: 0.5.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
@@ -42,79 +42,89 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
+If files modified/created only after a certain date are to be evaluated then use the date option:
 
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
 ```bash
-cocoa /path/to/repo --date YYYY-MM-DD
+cocoa /path/to/repo --date "YYYY-MM-DD"
+```
+
+Note: Please add date string in "YYYY-MM-DD" format.
+
+All options can be combined like so:
+
+```bash
+cocoa /path/to/repo --lint --verbose --date "YYYY-MM-DD"
 ```
 
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.5.1/README.md` & `dsi_cocoa-0.5.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
@@ -23,79 +23,89 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
+If files modified/created only after a certain date are to be evaluated then use the date option:
 
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
 ```bash
-cocoa /path/to/repo --date YYYY-MM-DD
+cocoa /path/to/repo --date "YYYY-MM-DD"
+```
+
+Note: Please add date string in "YYYY-MM-DD" format.
+
+All options can be combined like so:
+
+```bash
+cocoa /path/to/repo --lint --verbose --date "YYYY-MM-DD"
 ```
 
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.5.1/pyproject.toml` & `dsi_cocoa-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.5.2/src/cocoa/evaluate_repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,19 @@
     check_branch_names,
     clone_repo,
     files_after_date,
     get_current_branch,
     get_remote_branches_info,
     is_git_remote_repo,
     is_git_repo,
+    switch_branches,
 )
 
 
-def walk_and_process(
-    dir_path, lint_flag, start_date=None, verbose=False
-):
+def walk_and_process(dir_path, lint_flag, start_date=None, verbose=False):
     """
     Walk through directory and process all python and jupyter notebook files.
     """
     paths_to_flag = ["__pycache__", "DS_Store", "ipynb_checkpoints"]
     cprint(
         f"Currently analyzing branch {get_current_branch(dir_path)}",
         color="green",
@@ -144,25 +143,32 @@
             for result in results[:5]:
                 print(f"\t  {result}")
             if len(results) > 5:
                 print(f"\t  ...and {len(results) - 5} more issues.")
 
 
 def evaluate_repo(
-    path_or_url, lint_flag, start_date=None, verbose=False, branchinfo=False
+    path_or_url,
+    lint_flag,
+    start_date=None,
+    verbose=False,
+    branchinfo=False,
+    branch_name="main",
 ):
     """
     This is the entry point to running the automated code review.
     """
     cprint(PREAMBLE_TEXT, color="green")
     if os.path.isdir(path_or_url):
         if not is_git_repo(path_or_url):
             print(f"Error: {path_or_url} is not a Git repository.")
             exit(1)
 
+        switch_branches(path_or_url, branch_name)
+
         check_branch_names(path_or_url)
         if branchinfo:
             get_remote_branches_info(path_or_url)
         walk_and_process(
             path_or_url,
             lint_flag=lint_flag,
             start_date=start_date,
@@ -198,21 +204,27 @@
         default=None,
         help="Start date in YYYY-MM-DD format to filter files by commit date",
         type=str,
     )
     parser.add_argument(
         "--branchinfo", help="Report branch information", action="store_true"
     )
-
+    parser.add_argument(
+        "--branch",
+        default="main",
+        help="Specify which branch to evaluate",
+        type=str,
+    )
     args = parser.parse_args()
 
     dir_path = args.repo
     lint_flag = args.lint
     start_date = args.date
     verbose = args.verbose
     branchinfo = args.branchinfo
+    branch = args.branch
 
-    evaluate_repo(dir_path, lint_flag, start_date, verbose, branchinfo)
+    evaluate_repo(dir_path, lint_flag, start_date, verbose, branchinfo, branch)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsi_cocoa-0.5.1/src/cocoa/linting.py` & `dsi_cocoa-0.5.2/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/src/cocoa/notebooks.py` & `dsi_cocoa-0.5.2/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/src/cocoa/repo.py` & `dsi_cocoa-0.5.2/src/cocoa/repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -197,7 +197,26 @@
         response = requests.get(url)
         if response.ok:
             return True
     except requests.RequestException as e:
         print(f"Failed to access {url}: {e}")
 
     return False
+
+
+def switch_branches(repo_path, target_branch):
+    """Switch branches in a repository"""
+    repo = git.Repo(repo_path)
+    # Fetch all branches from remote
+    repo.git.fetch()
+
+    # Check if the target branch exists locally or remotely
+    if target_branch in repo.heads:
+        # Checkout the local branch
+        repo.git.checkout(target_branch)
+        print(f"Switched to local branch: {target_branch}")
+    elif target_branch in repo.remotes.origin.refs:
+        # Checkout the remote branch
+        repo.git.checkout("-b", target_branch, f"origin/{target_branch}")
+        print(f"Switched to remote branch: {target_branch}")
+    else:
+        print(f"Branch '{target_branch}' does not exist locally or remotely.")
```

### Comparing `dsi_cocoa-0.5.1/src/cocoa/spring2024.py` & `dsi_cocoa-0.5.2/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.5.1
+Version: 0.5.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
@@ -42,79 +42,89 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
+If files modified/created only after a certain date are to be evaluated then use the date option:
 
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
 ```bash
-cocoa /path/to/repo --date YYYY-MM-DD
+cocoa /path/to/repo --date "YYYY-MM-DD"
+```
+
+Note: Please add date string in "YYYY-MM-DD" format.
+
+All options can be combined like so:
+
+```bash
+cocoa /path/to/repo --lint --verbose --date "YYYY-MM-DD"
 ```
 
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.5.1/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.5.2/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+.bumpversion.cfg
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
+setup.py
 .github/workflows/error.badges.yml
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
 src/cocoa/evaluate_repo.py
 src/cocoa/linting.py
```

