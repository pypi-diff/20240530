# Comparing `tmp/dyff_storage-0.9.0.tar.gz` & `tmp/dyff_storage-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.9.0.tar", last modified: Fri May 24 22:48:42 2024, max compression
+gzip compressed data, was "dyff_storage-0.9.1.tar", last modified: Thu May 30 18:07:27 2024, max compression
```

## Comparing `dyff_storage-0.9.0.tar` & `dyff_storage-0.9.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.635452 dyff_storage-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.622452 dyff_storage-0.9.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.628452 dyff_storage-0.9.0/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.628452 dyff_storage-0.9.0/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.630452 dyff_storage-0.9.0/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2584 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.630452 dyff_storage-0.9.0/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.631452 dyff_storage-0.9.0/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.631452 dyff_storage-0.9.0/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.632452 dyff_storage-0.9.0/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7252 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    24465 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.632452 dyff_storage-0.9.0/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15691 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 22:48:42.635452 dyff_storage-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.591077 dyff_storage-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-30 18:07:27.590077 dyff_storage-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.578077 dyff_storage-0.9.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.584077 dyff_storage-0.9.1/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.584077 dyff_storage-0.9.1/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.585077 dyff_storage-0.9.1/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.586077 dyff_storage-0.9.1/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.586077 dyff_storage-0.9.1/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.587077 dyff_storage-0.9.1/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.588077 dyff_storage-0.9.1/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7252 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23851 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.588077 dyff_storage-0.9.1/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15691 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.590077 dyff_storage-0.9.1/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-30 18:07:27.000000 dyff_storage-0.9.1/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-30 18:07:27.000000 dyff_storage-0.9.1/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 18:07:27.000000 dyff_storage-0.9.1/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-30 18:07:27.000000 dyff_storage-0.9.1/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-30 18:07:27.000000 dyff_storage-0.9.1/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 18:07:27.591077 dyff_storage-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:07:27.590077 dyff_storage-0.9.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-30 18:07:21.000000 dyff_storage-0.9.1/tests/test_import.py
```

### Comparing `dyff_storage-0.9.0/.gitignore` & `dyff_storage-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/.gitlab-ci.yml` & `dyff_storage-0.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/.licenserc.yaml` & `dyff_storage-0.9.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/.pre-commit-config.yaml` & `dyff_storage-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/.secrets.baseline` & `dyff_storage-0.9.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/CODE_OF_CONDUCT.md` & `dyff_storage-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/LICENSE` & `dyff_storage-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/PKG-INFO` & `dyff_storage-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.9.0/README.md` & `dyff_storage-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/__init__.py` & `dyff_storage-0.9.1/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/base/auth.py` & `dyff_storage-0.9.1/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/base/command.py` & `dyff_storage-0.9.1/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/base/query.py` & `dyff_storage-0.9.1/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/base/storage.py` & `dyff_storage-0.9.1/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.9.1/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.9.1/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/mock/command.py` & `dyff_storage-0.9.1/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.9.1/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.9.1/dyff/storage/backend/mongodb/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,53 @@
 )
 from dyff.storage import timestamp
 from dyff.storage.backend.base.query import QueryBackend, Whitelist
 from dyff.storage.config import config
 
 
 class MongoDBQueryBackend(QueryBackend):
+    # Mapping of query keys in the API to the corresponding DB fields
+    query_key_map = {
+        Entities.Evaluation: {
+            "inferenceService": "inferenceSession.inferenceService.id",
+            "inferenceServiceName": "inferenceSession.inferenceService.name",
+            "model": "inferenceSession.inferenceService.model.id",
+            "modelName": "inferenceSession.inferenceService.model.name",
+        },
+        Entities.InferenceService: {
+            "model": "model.id",
+            "modelName": "model.name",
+        },
+        Entities.InferenceSession: {
+            "inferenceService": "inferenceService.id",
+            "inferenceServiceName": "inferenceService.name",
+            "model": "inferenceService.model.id",
+            "modelName": "inferenceService.model.name",
+        },
+        Entities.Measurement: {
+            "method": "method.id",
+            "methodName": "method.name",
+            "dataset": "scope.dataset",
+            "evaluation": "scope.evaluation",
+            "inferenceService": "scope.inferenceService",
+            "model": "scope.model",
+        },
+        Entities.Method: {
+            "outputKind": "output.kind",
+        },
+        Entities.SafetyCase: {
+            "method": "method.id",
+            "methodName": "method.name",
+            "dataset": "scope.dataset",
+            "evaluation": "scope.evaluation",
+            "inferenceService": "scope.inferenceService",
+            "model": "scope.model",
+        },
+    }
+
     def __init__(self):
         connection_string = config.api.query.mongodb.connection_string
         self._client = pymongo.MongoClient(connection_string.get_secret_value())
         self._workflows_db = self._client.get_database(
             config.api.query.mongodb.database
         )
 
@@ -95,21 +134,25 @@
 
         def json_decode(k: str, v: str):
             try:
                 return json.loads(v)
             except json.decoder.JSONDecodeError:
                 raise ClientError(f"{k}: json decode failed")
 
-        def build_query(query: dict) -> list:
+        def build_query(query: dict, key_map: dict[str, str]) -> list:
             conjunction: list = []
             for k, v in query.items():
                 if v is None:
                     continue
+
                 if k == "id":
                     k = "_id"
+                else:
+                    # Map query key to DB key, if mapping exists
+                    k = key_map.get(k, k)
 
                 if k == "labels":
                     if isinstance(v, dict):
                         labels = v
                     else:
                         labels = json_decode(k, v)
                     labeled = Labeled(labels=labels)  # validate
@@ -142,46 +185,40 @@
                     )
                 elif isinstance(v, list):
                     conjunction.append({k: {"$in": list(v)}})
                 else:
                     conjunction.append({k: v})
             return conjunction
 
+        key_map = MongoDBQueryBackend.query_key_map.get(kind, {})
+
         json_query_string = query.pop("query", None)
         if json_query_string is not None:
             json_query_object = json_decode("query", json_query_string)
             if isinstance(json_query_object, list):
                 for item in json_query_object:
-                    mongo_conjunction.extend(build_query(item))
+                    mongo_conjunction.extend(build_query(item, key_map))
             elif isinstance(json_query_object, dict):
-                mongo_conjunction.extend(build_query(json_query_object))
+                mongo_conjunction.extend(build_query(json_query_object, key_map))
             else:
                 raise ClientError(
                     f"query: must parse as dict or list[dict]; got {type(json_query_object)}"
                 )
 
-        mongo_conjunction.extend(build_query(query))
+        mongo_conjunction.extend(build_query(query, key_map))
 
         mongo_query = {"$and": mongo_conjunction} if mongo_conjunction else {}
         print(f"query: {mongo_query}")
         collection_name = Resources.for_kind(kind)
         collection = self._workflows_db[collection_name]
         results = collection.find(mongo_query)
 
         for result in results:
             yield self._convert_entity_response(result)
 
-    def _rename_query_key(self, query_dict: dict, old_key: str, new_key: str) -> None:
-        """If query_dict contains a value for old_key, pop the value and add it back at
-        new_key."""
-        unset = object()
-        value = query_dict.pop(old_key, unset)
-        if value is not unset:
-            query_dict[new_key] = value
-
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
         :param id: The unique key of the Audit.
         :returns: The Audit, or None if no Audit with the specified key exists.
         """
         result = self._get_entity(Entities.Audit, id)
@@ -194,16 +231,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Audit entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        results = self._query_entities(Entities.Audit, whitelist, qdict)
+        results = self._query_entities(Entities.Audit, whitelist, query.dict())
         return [Audit.parse_obj(result) for result in results]
 
     def get_data_source(self, id: str) -> Optional[DataSource]:
         """Retrieve a DataSource entity.
 
         :param id: The unique key of the DataSource.
         :returns: The DataSource, or None if no DataSource with the specified key
@@ -242,16 +278,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Dataset entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        results = self._query_entities(Entities.Dataset, whitelist, qdict)
+        results = self._query_entities(Entities.Dataset, whitelist, query.dict())
         return [Dataset.parse_obj(result) for result in results]
 
     def edit_documentation(
         self, id: str, edit: DocumentationEditRequest
     ) -> Optional[Documentation]:
         """Edit the Documentation entity associated with a resource.
 
@@ -305,28 +340,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Evaluation entity. The
             returned entities satisfy 'entity.field==value' for all items 'field: value'
             in kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(
-            qdict, "inferenceService", "inferenceSession.inferenceService.id"
-        )
-        self._rename_query_key(
-            qdict, "inferenceServiceName", "inferenceSession.inferenceService.name"
-        )
-        self._rename_query_key(
-            qdict, "model", "inferenceSession.inferenceService.model.id"
-        )
-        self._rename_query_key(
-            qdict, "modelName", "inferenceSession.inferenceService.model.name"
-        )
-        results = self._query_entities(Entities.Evaluation, whitelist, qdict)
+        results = self._query_entities(Entities.Evaluation, whitelist, query.dict())
         return [Evaluation.parse_obj(result) for result in results]
 
     def get_family(self, id: str) -> Optional[Family]:
         """Retrieve a Family entity.
 
         :param id: The unique ID of the Family.
         :returns: The Family, or None if no Family with the specified ID exists.
@@ -351,18 +373,17 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the InferenceService entity. The
             returned entities satisfy 'entity.field==value' for all items 'field: value'
             in kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "model", "model.id")
-        self._rename_query_key(qdict, "modelName", "model.name")
-        results = self._query_entities(Entities.InferenceService, whitelist, qdict)
+        results = self._query_entities(
+            Entities.InferenceService, whitelist, query.dict()
+        )
         return [InferenceService.parse_obj(result) for result in results]
 
     def get_inference_session(self, id: str) -> Optional[InferenceSession]:
         """Retrieve an InferenceSession entity.
 
         :param id: The unique key of the InferenceSession.
         :returns: The InferenceSession, or None if no InferenceSession with the
@@ -378,20 +399,17 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the InferenceSession entity. The
             returned entities satisfy 'entity.field==value' for all items 'field: value'
             in kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "inferenceService", "inferenceService.id")
-        self._rename_query_key(qdict, "inferenceServiceName", "inferenceService.name")
-        self._rename_query_key(qdict, "model", "inferenceService.model.id")
-        self._rename_query_key(qdict, "modelName", "inferenceService.model.name")
-        results = self._query_entities(Entities.InferenceSession, whitelist, qdict)
+        results = self._query_entities(
+            Entities.InferenceSession, whitelist, query.dict()
+        )
         return [InferenceSession.parse_obj(result) for result in results]
 
     def get_measurement(self, id: str) -> Optional[Measurement]:
         """Retrieve a Measurement entity.
 
         :param id: The unique key of the Measurement.
         :returns: The Measurement, or None if no Measurement with the specified key
@@ -407,22 +425,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Measurement entity. The
             returned entities satisfy 'entity.field==value' for all items 'field: value'
             in kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "method", "method.id")
-        self._rename_query_key(qdict, "methodName", "method.name")
-        self._rename_query_key(qdict, "dataset", "scope.dataset")
-        self._rename_query_key(qdict, "evaluation", "scope.evaluation")
-        self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
-        self._rename_query_key(qdict, "model", "scope.model")
-        results = self._query_entities(Entities.Measurement, whitelist, qdict)
+        results = self._query_entities(Entities.Measurement, whitelist, query.dict())
         return [Measurement.parse_obj(result) for result in results]
 
     def get_method(self, id: str) -> Optional[Method]:
         """Retrieve a Method entity.
 
         :param id: The unique key of the Method.
         :returns: The Method, or None if no Method with the specified key exists.
@@ -437,17 +448,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Method entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "outputKind", "output.kind")
-        results = self._query_entities(Entities.Method, whitelist, qdict)
+        results = self._query_entities(Entities.Method, whitelist, query.dict())
         return [Method.parse_obj(result) for result in results]
 
     def get_model(self, id: str) -> Optional[Model]:
         """Retrieve a Model entity.
 
         :param id: The unique key of the Model.
         :returns: The Model, or None if no Model with the specified key exists.
@@ -462,16 +471,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Model entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        results = self._query_entities(Entities.Model, whitelist, qdict)
+        results = self._query_entities(Entities.Model, whitelist, query.dict())
         return [Model.parse_obj(result) for result in results]
 
     def get_module(self, id: str) -> Optional[Module]:
         """Retrieve a Module entity.
 
         :param id: The unique key of the Module.
         :returns: The Module, or None if no Module with the specified key exists.
@@ -486,16 +494,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Module entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        results = self._query_entities(Entities.Module, whitelist, qdict)
+        results = self._query_entities(Entities.Module, whitelist, query.dict())
         return [Module.parse_obj(result) for result in results]
 
     def get_report(self, id: str) -> Optional[Report]:
         """Retrieve a Report entity.
 
         :param id: The unique key of the Report.
         :returns: The Report, or None if no Report with the specified key exists.
@@ -510,16 +517,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the Report entity. The returned
             entities satisfy 'entity.field==value' for all items 'field: value' in
             kwargs.
         """
-        qdict = query.dict()
-        results = self._query_entities(Entities.Report, whitelist, qdict)
+        results = self._query_entities(Entities.Report, whitelist, query.dict())
         return [Report.parse_obj(result) for result in results]
 
     def get_safetycase(self, id: str) -> Optional[SafetyCase]:
         """Retrieve a SafetyCase entity.
 
         :param id: The unique key of the SafetyCase.
         :returns: The SafetyCase, or None if no SafetyCase with the specified key
@@ -535,22 +541,15 @@
 
         :param whitelist: The set of accounts and entities that the caller has been
             granted access to.
         :param query: Equality constraints on fields of the SafetyCase entity. The
             returned entities satisfy 'entity.field==value' for all items 'field: value'
             in kwargs.
         """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "method", "method.id")
-        self._rename_query_key(qdict, "methodName", "method.name")
-        self._rename_query_key(qdict, "dataset", "scope.dataset")
-        self._rename_query_key(qdict, "evaluation", "scope.evaluation")
-        self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
-        self._rename_query_key(qdict, "model", "scope.model")
-        results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
+        results = self._query_entities(Entities.SafetyCase, whitelist, query.dict())
         return [SafetyCase.parse_obj(result) for result in results]
 
     def get_tag(self, id: str) -> Optional[Tag]:
         """Retrieve a Tag entity.
 
         :param id: The unique ID of the Tag.
         :returns: The Tag, or None if no Tag with the specified ID exists.
```

### Comparing `dyff_storage-0.9.0/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.9.1/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/config.py` & `dyff_storage-0.9.1/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/paths.py` & `dyff_storage-0.9.1/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff/storage/timestamp.py` & `dyff_storage-0.9.1/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.9.1/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.9.0/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.9.1/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/makefile` & `dyff_storage-0.9.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/pyproject.toml` & `dyff_storage-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.9.0/tests/test_import.py` & `dyff_storage-0.9.1/tests/test_import.py`

 * *Files identical despite different names*

