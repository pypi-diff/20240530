# Comparing `tmp/batchfetch-1.1.1.tar.gz` & `tmp/batchfetch-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.1.1.tar", last modified: Wed May 15 15:26:01 2024, max compression
+gzip compressed data, was "batchfetch-1.1.2.tar", last modified: Thu May 30 16:51:27 2024, max compression
```

## Comparing `batchfetch-1.1.1.tar` & `batchfetch-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/
--rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-15 15:25:56.000000 batchfetch-1.1.1/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-15 15:25:56.000000 batchfetch-1.1.1/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-15 15:26:01.702767 batchfetch-1.1.1/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-15 15:25:56.000000 batchfetch-1.1.1/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5951 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     9753 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    13709 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/top_level.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-15 15:25:56.000000 batchfetch-1.1.1/run_tests.sh
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-15 15:26:01.702767 batchfetch-1.1.1/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-15 15:25:56.000000 batchfetch-1.1.1/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/tests/
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/tests/data/
--rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/data/test-md5sum.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/data/test-run_simple.sh
--rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/test_helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-30 16:51:27.481080 batchfetch-1.1.2/
+-rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-30 16:51:08.000000 batchfetch-1.1.2/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-30 16:51:08.000000 batchfetch-1.1.2/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-30 16:51:27.481080 batchfetch-1.1.2/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-30 16:51:08.000000 batchfetch-1.1.2/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-30 16:51:27.477746 batchfetch-1.1.2/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-30 16:51:08.000000 batchfetch-1.1.2/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5940 2024-05-30 16:51:08.000000 batchfetch-1.1.2/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9753 2024-05-30 16:51:08.000000 batchfetch-1.1.2/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    14176 2024-05-30 16:51:08.000000 batchfetch-1.1.2/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-30 16:51:08.000000 batchfetch-1.1.2/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-30 16:51:27.481080 batchfetch-1.1.2/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-30 16:51:27.000000 batchfetch-1.1.2/batchfetch.egg-info/top_level.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-30 16:51:08.000000 batchfetch-1.1.2/run_tests.sh
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-30 16:51:27.481080 batchfetch-1.1.2/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-30 16:51:08.000000 batchfetch-1.1.2/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-30 16:51:27.481080 batchfetch-1.1.2/tests/
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-30 16:51:27.481080 batchfetch-1.1.2/tests/data/
+-rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-30 16:51:08.000000 batchfetch-1.1.2/tests/data/test-md5sum.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-30 16:51:08.000000 batchfetch-1.1.2/tests/data/test-run_simple.sh
+-rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-30 16:51:08.000000 batchfetch-1.1.2/tests/test_helpers.py
```

### Comparing `batchfetch-1.1.1/.gitignore` & `batchfetch-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/LICENSE` & `batchfetch-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/PKG-INFO` & `batchfetch-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.1.1/README.md` & `batchfetch-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/batchfetch/__init__.py` & `batchfetch-1.1.2/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/batchfetch/batchfetch_base.py` & `batchfetch-1.1.2/batchfetch/batchfetch_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def _initialize_data(self):
         if self._values_initialized:
             raise DataAlreadyInitialized
 
         # Options
         self.options = {}
-        self.options.update(deepcopy(self.global_options_values))  # Default
+        self.options.update(deepcopy(self.global_options_values))
         self.options.update(deepcopy(self._item_options))
         schema = Schema(self.global_options_schema)
         schema.validate(self.options)
 
         # Data
         self.values = {}
         self.values.update(deepcopy(self.task_default_values))
```

### Comparing `batchfetch-1.1.1/batchfetch/batchfetch_cli.py` & `batchfetch-1.1.2/batchfetch/batchfetch_cli.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/batchfetch/batchfetch_git.py` & `batchfetch-1.1.2/batchfetch/batchfetch_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,29 +223,39 @@
                 commit_ref = self._git_tags(self["reference"] + "^{commit}")[0]
             except GitReferenceDoesNotExist:
                 # The wanted reference does not exist. We should git pull in
                 # case we can get the reference
                 do_git_pull = True
             else:  # The reference exists
                 try:
-                    # If the tag is annotated, it points to a tag object, not
-                    # directly to a commit. You need to resolve it to the
-                    # commit it points to. Using `git rev-parse
-                    # <tagname>^{commit}` allows getting the right reference.
-                    commit_ref_head = self._git_tags("HEAD^{commit}")[0]
-                except GitReferenceDoesNotExist:
-                    # HEAD is detached
-                    commit_ref_head = None
-
-                # The wanted commit reference does not exist
-                # Or the commit ref of HEAD hasn't changed
-                if commit_ref and commit_ref_head == commit_ref:
-                    do_git_pull = False
-                else:
+                    cmd = ["git", "show-ref", "--verify", "--quiet",
+                           f"refs/heads/{self['reference']}"]
+                    run_simple(cmd, env=self.env, cwd=self.git_local_dir)
                     do_git_pull = True
+                except subprocess.CalledProcessError:
+                    pass
+
+                if not do_git_pull:
+                    try:
+                        # If the tag is annotated, it points to a tag object,
+                        # not directly to a commit. You need to resolve it to
+                        # the commit it points to. Using `git rev-parse
+                        # <tagname>^{commit}` allows getting the right
+                        # reference.
+                        commit_ref_head = self._git_tags("HEAD^{commit}")[0]
+                    except GitReferenceDoesNotExist:
+                        # HEAD is detached
+                        commit_ref_head = None
+
+                    # The wanted commit reference does not exist
+                    # Or the commit ref of HEAD hasn't changed
+                    if commit_ref and commit_ref_head == commit_ref:
+                        do_git_pull = False
+                    else:
+                        do_git_pull = True
 
         if not do_git_pull:
             self.add_output(self.indent_spaces + "[INFO] git pull ignored\n")
             return git_merge
 
         # Fetch
         cmd = ["git", "fetch", "origin"]
```

### Comparing `batchfetch-1.1.1/batchfetch/helpers.py` & `batchfetch-1.1.2/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.1.2/batchfetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.1.1/run_tests.sh` & `batchfetch-1.1.2/run_tests.sh`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.1/setup.py` & `batchfetch-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.1.1",
+    version="1.1.2",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

### Comparing `batchfetch-1.1.1/tests/test_helpers.py` & `batchfetch-1.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

