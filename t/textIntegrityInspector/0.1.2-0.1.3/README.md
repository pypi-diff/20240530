# Comparing `tmp/textintegrityinspector-0.1.2.tar.gz` & `tmp/textintegrityinspector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textintegrityinspector-0.1.2.tar", last modified: Wed May 29 08:15:35 2024, max compression
+gzip compressed data, was "textintegrityinspector-0.1.3.tar", last modified: Wed May 29 14:20:14 2024, max compression
```

## Comparing `textintegrityinspector-0.1.2.tar` & `textintegrityinspector-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.843011 textintegrityinspector-0.1.2/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.835011 textintegrityinspector-0.1.2/.github/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.839011 textintegrityinspector-0.1.2/.github/workflows/
--rw-r--r--   0     1001 root         (0)     3226 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/.github/workflows/build.yml
--rw-r--r--   0     1001 root         (0)     3493 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/.gitlab-ci.yml
--rw-r--r--   0     1001 root         (0)      266 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/.textIntegrityInspector.toml
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.839011 textintegrityinspector-0.1.2/.vscode/
--rw-r--r--   0     1001 root         (0)      982 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/.vscode/launch.json
--rw-r--r--   0     1001 root         (0)      498 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/.vscode/settings.json
--rw-r--r--   0     1001 root         (0)       45 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/AUTHORS
--rw-r--r--   0     1001 root         (0)      186 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/ChangeLog
--rw-r--r--   0     1001 root         (0)      465 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/Dockerfile
--rw-r--r--   0     1001 root         (0)     1069 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/LICENSE
--rw-r--r--   0     1001 root         (0)      473 2024-05-29 08:15:35.843011 textintegrityinspector-0.1.2/PKG-INFO
--rw-r--r--   0     1001 root         (0)      281 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/Pipfile
--rw-r--r--   0     1001 root         (0)    34132 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/Pipfile.lock
--rw-r--r--   0     1001 root         (0)     2591 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.835011 textintegrityinspector-0.1.2/doc/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.839011 textintegrityinspector-0.1.2/doc/images/
--rw-r--r--   0     1001 root         (0)   187520 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/doc/images/TextIntegrityLogo180.png
--rw-r--r--   0     1001 root         (0)       90 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/pyprojet.toml
--rw-r--r--   0     1001 root         (0)      446 2024-05-29 08:15:35.843011 textintegrityinspector-0.1.2/setup.cfg
--rw-r--r--   0     1001 root         (0)       75 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/setup.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.839011 textintegrityinspector-0.1.2/tests/
--rw-r--r--   0     1001 root         (0)        0 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/tests/__init__.py
--rw-r--r--   0     1001 root         (0)     3214 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/tests/test_main.py
--rw-r--r--   0     1001 root         (0)    13626 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/tests/test_validator.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.843011 textintegrityinspector-0.1.2/textIntegrityInspector/
--rw-r--r--   0     1001 root         (0)      205 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/textIntegrityInspector/__init__.py
--rw-r--r--   0     1001 root         (0)     4692 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/textIntegrityInspector/__main__.py
--rw-r--r--   0     1001 root         (0)     2715 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/textIntegrityInspector/languageData.py
--rw-r--r--   0     1001 root         (0)     6475 2024-05-29 08:15:07.000000 textintegrityinspector-0.1.2/textIntegrityInspector/validator.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 08:15:35.843011 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/
--rw-r--r--   0     1001 root         (0)      473 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)      820 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)       80 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/entry_points.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/not-zip-safe
--rw-r--r--   0     1001 root         (0)       47 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/pbr.json
--rw-r--r--   0     1001 root         (0)       54 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)       23 2024-05-29 08:15:35.000000 textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/top_level.txt
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.276883 textintegrityinspector-0.1.3/.github/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/.github/workflows/
+-rw-r--r--   0     1001 root         (0)     3226 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0     1001 root         (0)     3493 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.gitlab-ci.yml
+-rw-r--r--   0     1001 root         (0)      266 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.textIntegrityInspector.toml
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/.vscode/
+-rw-r--r--   0     1001 root         (0)      982 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.vscode/launch.json
+-rw-r--r--   0     1001 root         (0)      498 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.vscode/settings.json
+-rw-r--r--   0     1001 root         (0)       45 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/AUTHORS
+-rw-r--r--   0     1001 root         (0)      186 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/ChangeLog
+-rw-r--r--   0     1001 root         (0)      465 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Dockerfile
+-rw-r--r--   0     1001 root         (0)     1069 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/LICENSE
+-rw-r--r--   0     1001 root         (0)      473 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/PKG-INFO
+-rw-r--r--   0     1001 root         (0)      281 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Pipfile
+-rw-r--r--   0     1001 root         (0)    34132 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Pipfile.lock
+-rw-r--r--   0     1001 root         (0)     2591 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.276883 textintegrityinspector-0.1.3/doc/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/doc/images/
+-rw-r--r--   0     1001 root         (0)   187520 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/doc/images/TextIntegrityLogo180.png
+-rw-r--r--   0     1001 root         (0)       90 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/pyprojet.toml
+-rw-r--r--   0     1001 root         (0)      446 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/setup.cfg
+-rw-r--r--   0     1001 root         (0)       75 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/tests/
+-rw-r--r--   0     1001 root         (0)        0 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/__init__.py
+-rw-r--r--   0     1001 root         (0)     3214 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/test_main.py
+-rw-r--r--   0     1001 root         (0)    13626 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/test_validator.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/textIntegrityInspector/
+-rw-r--r--   0     1001 root         (0)      205 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/__init__.py
+-rw-r--r--   0     1001 root         (0)     4692 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/__main__.py
+-rw-r--r--   0     1001 root         (0)     2715 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/languageData.py
+-rw-r--r--   0     1001 root         (0)     6475 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/validator.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/
+-rw-r--r--   0     1001 root         (0)      473 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)      820 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)       80 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/entry_points.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/not-zip-safe
+-rw-r--r--   0     1001 root         (0)       47 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/pbr.json
+-rw-r--r--   0     1001 root         (0)       54 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)       23 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/top_level.txt
```

### Comparing `textintegrityinspector-0.1.2/.github/workflows/build.yml` & `textintegrityinspector-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/.gitlab-ci.yml` & `textintegrityinspector-0.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/.vscode/launch.json` & `textintegrityinspector-0.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/LICENSE` & `textintegrityinspector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/Pipfile.lock` & `textintegrityinspector-0.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/README.md` & `textintegrityinspector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/doc/images/TextIntegrityLogo180.png` & `textintegrityinspector-0.1.3/doc/images/TextIntegrityLogo180.png`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/tests/test_main.py` & `textintegrityinspector-0.1.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/tests/test_validator.py` & `textintegrityinspector-0.1.3/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/textIntegrityInspector/__main__.py` & `textintegrityinspector-0.1.3/textIntegrityInspector/__main__.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/textIntegrityInspector/languageData.py` & `textintegrityinspector-0.1.3/textIntegrityInspector/languageData.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/textIntegrityInspector/validator.py` & `textintegrityinspector-0.1.3/textIntegrityInspector/validator.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.2/textIntegrityInspector.egg-info/SOURCES.txt` & `textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

