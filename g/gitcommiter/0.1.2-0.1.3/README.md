# Comparing `tmp/gitcommiter-0.1.2.tar.gz` & `tmp/gitcommiter-0.1.3.tar.gz`

## Comparing `gitcommiter-0.1.2.tar` & `gitcommiter-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/banner.tape
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/usage.tape
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.github/labels.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.github/release-drafter.yml
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.github/workflows/Publish.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.github/workflows/draft.yml
--rw-r--r--   0        0        0   120112 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/media/banner.gif
--rw-r--r--   0        0        0   164698 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/media/usecase.gif
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/gitcommiter/__init__.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/gitcommiter/gitcommiter.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/LICENSE
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 gitcommiter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/banner.tape
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/usage.tape
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.github/labels.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.github/workflows/Publish.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.github/workflows/draft.yml
+-rw-r--r--   0        0        0   120112 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/media/banner.gif
+-rw-r--r--   0        0        0   164698 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/media/usecase.gif
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/gitcommiter/__init__.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/gitcommiter/gitcommiter.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 gitcommiter-0.1.3/PKG-INFO
```

### Comparing `gitcommiter-0.1.2/.github/labels.yml` & `gitcommiter-0.1.3/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/.github/release-drafter.yml` & `gitcommiter-0.1.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/.github/workflows/Publish.yml` & `gitcommiter-0.1.3/.github/workflows/Publish.yml`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/media/banner.gif` & `gitcommiter-0.1.3/media/banner.gif`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/media/usecase.gif` & `gitcommiter-0.1.3/media/usecase.gif`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/gitcommiter/gitcommiter.py` & `gitcommiter-0.1.3/gitcommiter/gitcommiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,26 @@
 
 
 @click.command()
 @click.option(
     "-d", "--directory", type=click.Path(exists=True), help="Directory to process"
 )
 @click.option("-p", "--push", is_flag=True, help="Push changes to the remote repository")
+@click.option("-nv", "--no-verify", is_flag=True, help="Ignore pre-commit hooks")
 @click.option("-h", "--help", is_flag=True, help="Print help message")
-def git_add_and_commit(directory, push, help):
+def git_add_and_commit(directory, push, no_verify, help):
     if help:
         print_banner()
         click.echo("Automatically add and commit new, modified, and deleted files to Git and write super cool commit messages")
         click.echo("\nUsage:")
         click.echo("  gitcommiter -d /path/to/your/directory [-p]")
         click.echo("\nOptions:")
         click.echo("  -d, --directory  Directory to process")
         click.echo("  -p, --push       Push changes to the remote repository")
+        click.echo("  -nv, --no-verify Ignore pre-commit hooks")
         click.echo("  -h, --help       Print this message")
         click.get_current_context().exit()
 
     if not directory:
         click.echo("Please provide a directory using the -d/--directory option.")
         click.echo("For example: gitcommiter -d /path/to/your/directory")
         click.get_current_context().exit()
@@ -100,15 +102,18 @@
     # Construct the commit message
     commit_message = construct_commit_message(
         untracked_files, modified_files, deleted_files
     )
 
     # Commit changes
     if commit_message:
-        subprocess.run(["git", "commit", "-m", commit_message])
+        if no_verify:
+            subprocess.run(["git", "commit", "-m", commit_message, "--no-verify"])
+        else:
+            subprocess.run(["git", "commit", "-m", commit_message])
 
     # Push changes if the -p/--push option is passed
     if push:
         subprocess.run(["git", "push"])
```

### Comparing `gitcommiter-0.1.2/.gitignore` & `gitcommiter-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/LICENSE` & `gitcommiter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/README.md` & `gitcommiter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gitcommiter-0.1.2/pyproject.toml` & `gitcommiter-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "gitcommiter"
-version = "0.1.2"
+version = "0.1.3"
 description = "Automatically add and commit new, modified, and deleted files to Git and write super cool commit messages."
-authors = [{ name = "SAIKAT KARMAKAR", email = "saikickkarma@protonmail.com" }]
+authors = [{ name = "SAIKAT KARMAKAR", email = "github.maturity983@passinbox.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
```

### Comparing `gitcommiter-0.1.2/PKG-INFO` & `gitcommiter-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: gitcommiter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically add and commit new, modified, and deleted files to Git and write super cool commit messages.
-Author-email: SAIKAT KARMAKAR <saikickkarma@protonmail.com>
+Author-email: SAIKAT KARMAKAR <github.maturity983@passinbox.com>
 License: Copyright 2023 Saikat Karmakar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

