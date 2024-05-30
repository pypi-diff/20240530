# Comparing `tmp/glbuild-0.1.2.tar.gz` & `tmp/glbuild-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glbuild-0.1.2.tar", max compression
+gzip compressed data, was "glbuild-0.1.3.tar", max compression
```

## Comparing `glbuild-0.1.2.tar` & `glbuild-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2024-05-16 20:24:48.931510 glbuild-0.1.2/LICENSE
--rw-r--r--   0        0        0      907 2024-05-16 20:24:48.931510 glbuild-0.1.2/README.md
--rw-r--r--   0        0        0       77 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/__init__.py
--rw-r--r--   0        0        0       23 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/cli/__init__.py
--rw-r--r--   0        0        0      935 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/cli/main.py
--rw-r--r--   0        0        0       39 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/collector/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/collector/progress.py
--rw-r--r--   0        0        0      124 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/constants.py
--rw-r--r--   0        0        0     6781 2024-05-16 20:24:48.931510 glbuild-0.1.2/glbuild/glbuild.py
--rw-r--r--   0        0        0       23 2024-05-16 20:24:48.932510 glbuild-0.1.2/glbuild/utils/__init__.py
--rw-r--r--   0        0        0    32235 2024-05-16 20:24:48.932510 glbuild-0.1.2/glbuild/utils/tempfile.py
--rw-r--r--   0        0        0     2180 2024-05-16 20:24:48.932510 glbuild-0.1.2/glbuild/utils/utils.py
--rw-r--r--   0        0        0      932 2024-05-16 20:24:48.933510 glbuild-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 glbuild-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-30 13:28:15.046874 glbuild-0.1.3/LICENSE
+-rw-r--r--   0        0        0      907 2024-05-30 13:28:15.046874 glbuild-0.1.3/README.md
+-rw-r--r--   0        0        0       77 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/cli/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/cli/main.py
+-rw-r--r--   0        0        0       39 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/collector/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/collector/progress.py
+-rw-r--r--   0        0        0      124 2024-05-30 13:28:15.046874 glbuild-0.1.3/glbuild/constants.py
+-rw-r--r--   0        0        0     7391 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/glbuild.py
+-rw-r--r--   0        0        0       23 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/__init__.py
+-rw-r--r--   0        0        0    32235 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/tempfile.py
+-rw-r--r--   0        0        0     2180 2024-05-30 13:28:15.047874 glbuild-0.1.3/glbuild/utils/utils.py
+-rw-r--r--   0        0        0      932 2024-05-30 13:28:15.048874 glbuild-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 glbuild-0.1.3/PKG-INFO
```

### Comparing `glbuild-0.1.2/LICENSE` & `glbuild-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.2/README.md` & `glbuild-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.2/glbuild/cli/main.py` & `glbuild-0.1.3/glbuild/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import click
 from glbuild import GitLabBuild
 
 
 @click.group(invoke_without_command=True)
 @click.option("--token", "-t", type=str, required=True)
 @click.option("--project", "-p", type=int, required=True, multiple=True)
+@click.option("--last", "-n", required=False, help="Get last n jobs only")
 @click.option("--output", "-o", required=True, help="Output directory")
 @click.option("--base-url", "-b", type=str, default="https://gitlab.com")
 @click.option("--api-version", type=int, default=4)
 @click.option("--ssl-verify", type=bool, default=False)
-def cli(token, projects, output, base_url, api_version, ssl_verify):
+def cli(token, projects, last, output, base_url, api_version, ssl_verify):
     """Glbuild CLI.
 
     Collect historical GitLab build data easily.
     """
     glb = GitLabBuild(
         base_url=base_url,
         token=token,
         projects=list(projects),
         api_version=api_version,
         ssl_verify=ssl_verify,
     )
-    glb.start(output=output)
+    glb.start(n=last, output=output)
 
 
 if __name__ == "__main__":
     # pylint: disable=no-value-for-parameter
     cli()
```

### Comparing `glbuild-0.1.2/glbuild/collector/progress.py` & `glbuild-0.1.3/glbuild/collector/progress.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.2/glbuild/glbuild.py` & `glbuild-0.1.3/glbuild/glbuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Main Class for GitLab Builds data collection"""
 
+import math
 import os
 import time
 import json
 import gitlab
 import requests
 import pandas as pd
 from typing import Optional
@@ -31,14 +32,15 @@
         api_version: int = 4,
         ssl_verify: bool = False,
     ) -> None:
         """Constructor.
 
         Params
         ------
+            projects(list[int]|int): Single of List of projects ID.
             base_url(str): GitLab instance base URL. Defaults to https://gitlab.com
             token(str): GitLab Personal Access Token.
         """
         self.base_url: str = base_url
         self.token: str = token
         self.api_version: int = api_version
         self.ssl_verify: bool = ssl_verify
@@ -47,47 +49,51 @@
             url=base_url,
             private_token=token,
             api_version=api_version,
             ssl_verify=ssl_verify,
         )
         self.progress = progress.Progress(projects=projects)
 
-    def start(self, output: str = "./data") -> bool:
+    def start(self, n: Optional[int] = None, output: str = "./data") -> bool:
         """Get historical build jobs metadata and logs from projects into path.
 
         Params
         ------
-            projects(list[int]|int): Single of List of projects ID.
+            n (None|int): Get only n last jobs.
             path(str): Directory for output. Defaults to ./data/
         """
         # Create directories if necessary
         for path in [output, f"{output}/logs/"]:
             utils.ensure_path(path)
 
         for path in [f"{output}/logs/{id}" for id in self.projects]:
             utils.ensure_path(path)
 
         for project_id in self.progress.load_unprocessed():
-            self.__get_project_data(project_id, output)
+            self.__get_project_data(project_id, output, last=n)
             self.progress.set_processed(project_id)
             time.sleep(1)
         return True
 
     ###################################
     #         Project Methods         #
     ###################################
 
     def __get_project_data(
-        self, project_id: int, datapath: str, only_failures: bool = True
+        self,
+        project_id: int,
+        datapath: str,
+        only_failures: bool = True,
+        last: Optional[int] = None,
     ):
         """Collect jobs metadata and logs for a GitLab project."""
         print(f"\nProcessing project with id {project_id}")
 
         # get all metadata of jobs.
-        jobs = self.__get_jobs_metadata(project_id, datapath=datapath)
+        jobs = self.__get_jobs_metadata(project_id, datapath=datapath, last=last)
         print(f"{len(jobs)} jobs found for collection.")
 
         # download the logs
         progress_bar = tqdm(jobs, ncols=120)
         for job in progress_bar:
             if only_failures:
                 if job["status"] != "failed":
@@ -104,28 +110,31 @@
         # close progress bar
         progress_bar.close()
 
     ###################################
     #           Job Methods           #
     ###################################
 
-    def __get_jobs_metadata(self, project_id: int, datapath: str):
+    def __get_jobs_metadata(
+        self, project_id: int, datapath: str, last: Optional[int] = None
+    ):
         """Get jobs for project (or download) and save to datapath.
 
         project_id(int): ID of the project.
         datapath(str): Base directory where to save the collected data.
+        last (None|int): Get only n last jobs.
         """
         jobs_filepath = f"{datapath}/jobs_{project_id}.json"
         project = self.gl.projects.get(int(project_id), lazy=True)
 
         # read already collected json jobs
         old_jobs = utils.json_to_list(jobs_filepath)
         if old_jobs is None:
             # read entire history records
-            jobs = self.__get_all_jobs(project)
+            jobs = self.__get_all_jobs(project, last=last)
         else:
             # read new records efficiently
             old_jobs = pd.DataFrame(old_jobs)
             last_collected_job_id: int = old_jobs["id"].max()
 
             page: int = 1
             jobs_df: pd.DataFrame = pd.DataFrame(
@@ -152,16 +161,25 @@
             jobs = jobs_df.to_dict(orient="records")
 
         # save jobs json data
         with open(jobs_filepath, mode="w", encoding="utf-8") as f:
             json.dump(jobs, f)
         return jobs
 
-    def __get_all_jobs(self, project) -> list[dict]:
+    def __get_all_jobs(self, project, last: Optional[int]) -> list[dict]:
         """Get list of all jobs for a project using python-gitlab."""
+        if last is not None:
+            nb_pages = math.ceil(last / constants.JOBS_PER_PAGE)
+            jobs = []
+            for page in range(nb_pages):
+                jobs.extend(
+                    self.__get_jobs_by_page(project, page + 1, constants.JOBS_PER_PAGE)
+                )
+            return jobs[:last]
+
         return [
             json.loads(job.to_json())
             for job in project.jobs.list(all=True, retry_transient_errors=True)
         ]
 
     def __get_jobs_by_page(
         self, project, page: int, per_page: int = constants.JOBS_PER_PAGE
```

### Comparing `glbuild-0.1.2/glbuild/utils/tempfile.py` & `glbuild-0.1.3/glbuild/utils/tempfile.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.2/glbuild/utils/utils.py` & `glbuild-0.1.3/glbuild/utils/utils.py`

 * *Files identical despite different names*

### Comparing `glbuild-0.1.2/pyproject.toml` & `glbuild-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "glbuild"
-version = "0.1.2"
+version = "0.1.3"
 description = "Gitlab build jobs data collector. CLI tool and Python package."
 authors = [ "Henri Aïdasso <ahenrij@gmail.com>",]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,23 +18,23 @@
 tqdm = "^4.66.4"
 python-gitlab = "^4.5.0"
 pandas = "^2.2.2"
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240406"
 types-toml = "^0.10.8.20240310"
 
+[tool.poetry.scripts]
+glbuild = "glbuild.cli.main:cli"
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
 pytest-datadir = "^1.5.0"
 pytest-timeout = "^2.3.1"
 pre-commit = "^3.7.1"
 black = "^24.4.2"
 fire = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies.prospector]
 extras = [ "with_everything",]
 version = "^1.3.1"
-
-[tool.poetry.scripts]
-glbuild = "glbuild.cli.main:cli"
```

### Comparing `glbuild-0.1.2/PKG-INFO` & `glbuild-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glbuild
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gitlab build jobs data collector. CLI tool and Python package.
 License: LICENSE
 Author: Henri Aïdasso
 Author-email: ahenrij@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

