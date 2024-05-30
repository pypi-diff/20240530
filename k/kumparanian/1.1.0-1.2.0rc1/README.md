# Comparing `tmp/kumparanian-1.1.0.tar.gz` & `tmp/kumparanian-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumparanian-1.1.0.tar", max compression
+gzip compressed data, was "kumparanian-1.2.0rc1.tar", max compression
```

## Comparing `kumparanian-1.1.0.tar` & `kumparanian-1.2.0rc1.tar`

### file list

```diff
@@ -1,14 +1,10 @@
--rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.1.0/LICENSE
--rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.1.0/kumparanian/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 08:24:12.247895 kumparanian-1.1.0/kumparanian/__main__.py
--rw-r--r--   0        0        0     3183 2024-05-29 10:24:09.402664 kumparanian-1.1.0/kumparanian/cli.py
--rw-r--r--   0        0        0      564 2024-05-29 10:24:09.403171 kumparanian-1.1.0/kumparanian/de/__init__.py
--rw-r--r--   0        0        0     2264 2024-05-29 10:24:09.403627 kumparanian-1.1.0/kumparanian/de/dataset.py
--rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.1.0/kumparanian/de/help_text.py
--rw-r--r--   0        0        0     5446 2024-05-29 10:24:09.404362 kumparanian-1.1.0/kumparanian/de/submission.py
--rw-r--r--   0        0        0      392 2024-05-29 10:24:09.404822 kumparanian-1.1.0/kumparanian/ds/__init__.py
--rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.1.0/kumparanian/ds/help_text.py
--rw-r--r--   0        0        0     2322 2024-05-29 10:24:09.405263 kumparanian-1.1.0/kumparanian/ds/model.py
--rw-r--r--   0        0        0      894 2024-05-29 10:24:09.405766 kumparanian-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 kumparanian-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1486 2024-05-15 07:02:16.132381 kumparanian-1.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     2863 2024-05-30 04:46:04.796932 kumparanian-1.2.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 07:02:16.133186 kumparanian-1.2.0rc1/kumparanian/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-15 07:02:16.133323 kumparanian-1.2.0rc1/kumparanian/__main__.py
+-rw-r--r--   0        0        0     1687 2024-05-28 11:10:59.573760 kumparanian-1.2.0rc1/kumparanian/cli.py
+-rw-r--r--   0        0        0      392 2024-05-27 06:29:00.637103 kumparanian-1.2.0rc1/kumparanian/ds/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-22 18:00:54.982713 kumparanian-1.2.0rc1/kumparanian/ds/help_text.py
+-rw-r--r--   0        0        0     9470 2024-05-29 08:10:23.998982 kumparanian-1.2.0rc1/kumparanian/ds/model.py
+-rw-r--r--   0        0        0     1016 2024-05-30 09:55:59.293341 kumparanian-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 kumparanian-1.2.0rc1/PKG-INFO
```

### Comparing `kumparanian-1.1.0/LICENSE` & `kumparanian-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kumparanian-1.1.0/README.md` & `kumparanian-1.2.0rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,24 @@
     Usage: kumparanian ds [OPTIONS] COMMAND [ARGS]...
 
       For Data Scientist role.
 
       Before you submit your trained model, you can verify your trained model
       using the following command:
 
-      $ kumparanian ds verify YOURMODEL.pickle
+      $ kumparanian ds verify YOURMODEL.pickle YOURFILE.pickle
+    
+      YOURMODEL.pickle should contain your trained model, and YOURFILE.pickle
+      should contain the necessary preprocessing components such as the vectorizer, 
+      label encoder, and model type.
 
       Use the following command to evaluate your trained model against your test
       dataset:
 
-      $ kumparanian ds evaluate YOURMODEL.pickle test_file.csv
+      $ kumparanian ds evaluate YOURMODEL.pickle YOURFILE.pickle test_file.csv
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       evaluate  Evaluate the model
       verify    Verify the model
```

### Comparing `kumparanian-1.1.0/kumparanian/cli.py` & `kumparanian-1.2.0rc1/kumparanian/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import multiprocessing
 
 import click
 
-import kumparanian.de as de
 import kumparanian.ds as ds
 
 # Help texts
 epilog = (
     "If you found any issues, feel free report it at: "
     "https://github.com/kumparan/kumparanian/issues"
 )
@@ -20,91 +19,44 @@
 @cli.group(name="ds", help=ds.help_text, epilog=epilog)
 def ds_group():
     pass
 
 
 @ds_group.command(short_help=ds.verify_short_help, help=ds.verify_usage)
 @click.argument("model", type=click.Path(exists=True))
-def verify(model):
+@click.argument("file", type=click.Path(exists=True))
+def verify(model, file):
     try:
-        ds.model.verify(model)
+        ds.model.verify(model, file)
     except Exception as err:
         message = "[INVALID] {}".format(err)
         click.secho(message, fg="red")
         exit(1)
     click.secho("[VALID] Model is valid.", fg="green")
     exit(0)
 
 
 @ds_group.command(short_help=ds.evaluate_short_help, help=ds.evaluate_usage)
 @click.argument("model", type=click.Path(exists=True))
+@click.argument("file", type=click.Path(exists=True))
 @click.argument("testfile", type=click.Path(exists=True))
-def evaluate(model, testfile):
+def evaluate(model, file, testfile):
     # Make sure the model is valid
     try:
-        ds.model.verify(model)
+        ds.model.verify(model, file)
     except Exception:
         message = "Model is invalid, please verify the model"
         click.secho(message, fg="red")
         exit(1)
 
     # Evaluate the model; only shows accuracy
-    acc = ds.model.evaluate(model, testfile, data_type="topic_model")
+    acc = ds.model.evaluate(model, file, testfile, data_type="topic_model")
     click.echo("Accuracy: {}".format(acc))
 
 
-@cli.group(name="de", help=de.help_text, epilog=epilog)
-def de_group():
-    pass
-
-
-@de_group.command(
-    name="generate-dataset", short_help=de.generate_short_help, help=de.generate_usage
-)
-@click.argument("candidate_name", type=str)
-@click.option(
-    "--output-dir",
-    default="data",
-    help="Output directory",
-    type=click.Path(exists=False, file_okay=False, writable=True),
-)
-@click.option("--num-files", default=40, type=int, help="Number of files")
-@click.option("--num-workers", default=4, type=int, help="Number of workers")
-def generate_dataset(candidate_name, output_dir, num_files, num_workers):
-    de.dataset.generate_data(
-        candidate_name=candidate_name,
-        output_dir=output_dir,
-        num_files=num_files,
-        num_workers=num_workers,
-    )
-    click.secho("[kumparanian] Output: " + output_dir + "/", fg="green")
-
-
-@de_group.command(name="verify", short_help=de.verify_short_help, help=de.verify_usage)
-@click.argument("submission_dir", type=click.Path(exists=True))
-def verify_submission(submission_dir):
-    try:
-        de.submission.verify(submission_dir)
-    except Exception as err:
-        message = "[INVALID] {}".format(err)
-        click.secho(message, fg="red")
-        exit(1)
-    click.secho("[VALID] Submission is valid.", fg="green")
-    exit(0)
-
-
-@de_group.command(
-    name="evaluate", short_help=de.evaluate_short_help, help=de.evaluate_usage
-)
-@click.argument("submission_dir", type=str)
-@click.argument("solution_dir", type=str)
-def evaluate_submission(submission_dir, solution_dir):
-    de.submission.evaluate(submission_dir, solution_dir)
-
-
 def main():
     cli()
 
 
 if __name__ == "__main__":
     # handle "Error: No such option: --multiprocessing-fork"
     # read more https://github.com/pyinstaller/pyinstaller/issues/2023
```

### Comparing `kumparanian-1.1.0/pyproject.toml` & `kumparanian-1.2.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 [tool.poetry]
 name = "kumparanian"
-version = "1.1.0"
+version = "1.2.0rc1"
 description = "Kumparanian CLI"
 authors = ["Zavli Juwantara <zavli.juwantara@kumparan.com>"]
 repository = "https://github.com/kumparan/kumparanian"
 maintainers = [
     "Bayu <bayualdiyansyah@gmail.com>",
     "Raden <radenmaharjo@gmail.com>",
     "Aslam <aslam.hadi@kumparan.com>",
+    "Ghefira <ghefira.fatimah@kumparan.com>"
 ]
 license = "kumparan"
 readme = "README.md"
 packages = [
     { include = "kumparanian" },
-    { include = "kumparanian/de" },
     { include = "kumparanian/ds" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-numpy = "^1.26.4"
-dill = "^0.3.8"
+python = ">=3.10,<3.12"
+numpy = "1.24.3"
 click = "^8.1.7"
 colorama = "^0.4.6"
+tensorflow = "2.13.0"
+scikit-learn = "1.4.2"
+dill = "0.3.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 isort = "^5.13.2"
 
+[tool.poetry.scripts]
+kumparanian = "kumparanian.cli:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-pyinstaller-plugin.scripts]
 kumparanian = { source = "kumparanian/cli.py", type = "onedir", bundle = true }
```

### Comparing `kumparanian-1.1.0/PKG-INFO` & `kumparanian-1.2.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: kumparanian
-Version: 1.1.0
+Version: 1.2.0rc1
 Summary: Kumparanian CLI
 Home-page: https://github.com/kumparan/kumparanian
 License: kumparan
 Author: Zavli Juwantara
 Author-email: zavli.juwantara@kumparan.com
 Maintainer: Bayu
 Maintainer-email: bayualdiyansyah@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: dill (==0.3.8)
+Requires-Dist: numpy (==1.24.3)
+Requires-Dist: scikit-learn (==1.4.2)
+Requires-Dist: tensorflow (==2.13.0)
 Project-URL: Repository, https://github.com/kumparan/kumparanian
 Description-Content-Type: text/markdown
 
 # Kumparanian [![Build Status](https://travis-ci.org/kumparan/kumparanian.svg?branch=master)](https://travis-ci.org/kumparan/kumparanian) [![PyPI version](https://badge.fury.io/py/kumparanian.svg)](https://badge.fury.io/py/kumparanian)
 Kumparanian is a set of workflows that optimize Kumparan's data engineering 
 and data scientist hiring process. It cuts down 1-2 working day(s) submission 
 review process to just less than an hour.
@@ -40,20 +41,24 @@
     Usage: kumparanian ds [OPTIONS] COMMAND [ARGS]...
 
       For Data Scientist role.
 
       Before you submit your trained model, you can verify your trained model
       using the following command:
 
-      $ kumparanian ds verify YOURMODEL.pickle
+      $ kumparanian ds verify YOURMODEL.pickle YOURFILE.pickle
+    
+      YOURMODEL.pickle should contain your trained model, and YOURFILE.pickle
+      should contain the necessary preprocessing components such as the vectorizer, 
+      label encoder, and model type.
 
       Use the following command to evaluate your trained model against your test
       dataset:
 
-      $ kumparanian ds evaluate YOURMODEL.pickle test_file.csv
+      $ kumparanian ds evaluate YOURMODEL.pickle YOURFILE.pickle test_file.csv
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       evaluate  Evaluate the model
       verify    Verify the model
```

