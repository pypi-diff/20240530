# Comparing `tmp/celery_starter-1.0.2.tar.gz` & `tmp/celery_starter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_starter-1.0.2.tar", last modified: Thu May  2 17:18:16 2024, max compression
+gzip compressed data, was "celery_starter-1.0.3.tar", last modified: Thu May 30 15:08:38 2024, max compression
```

## Comparing `celery_starter-1.0.2.tar` & `celery_starter-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.428094 celery_starter-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-02 17:18:09.000000 celery_starter-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:18:09.000000 celery_starter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-02 17:18:16.436094 celery_starter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-02 17:18:09.000000 celery_starter-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-05-02 17:18:09.000000 celery_starter-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:18:16.436094 celery_starter-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.428094 celery_starter-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/src/celery_starter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/src/celery_starter/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/src/celery_starter/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/commands/runcelery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/src/celery_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/commands/test_runcelery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.890884 celery_starter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 15:08:34.000000 celery_starter-1.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.882884 celery_starter-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-30 15:08:34.000000 celery_starter-1.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 15:08:34.000000 celery_starter-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 15:08:34.000000 celery_starter-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-30 15:08:34.000000 celery_starter-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 15:08:34.000000 celery_starter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-30 15:08:38.890884 celery_starter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-30 15:08:34.000000 celery_starter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-05-30 15:08:34.000000 celery_starter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 15:08:38.890884 celery_starter-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.882884 celery_starter-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/src/celery_starter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/src/celery_starter/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/src/celery_starter/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-30 15:08:34.000000 celery_starter-1.0.3/src/celery_starter/management/commands/runcelery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/src/celery_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 15:08:38.000000 celery_starter-1.0.3/src/celery_starter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 15:08:34.000000 celery_starter-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:38.886884 celery_starter-1.0.3/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:08:34.000000 celery_starter-1.0.3/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 15:08:34.000000 celery_starter-1.0.3/tests/management/commands/test_runcelery.py
```

### Comparing `celery_starter-1.0.2/.editorconfig` & `celery_starter-1.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/.github/workflows/publish-to-pypi.yml` & `celery_starter-1.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/.pre-commit-config.yaml` & `celery_starter-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/CONTRIBUTING.md` & `celery_starter-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/LICENSE` & `celery_starter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/PKG-INFO` & `celery_starter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery_starter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django command to launch celery worker, beat, flower
 Home-page: https://github.com/Friskes/celery-starter
 Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
```

### Comparing `celery_starter-1.0.2/README.md` & `celery_starter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/pyproject.toml` & `celery_starter-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/src/celery_starter/_localization.py` & `celery_starter-1.0.3/src/celery_starter/_localization.py`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.2/src/celery_starter/management/commands/runcelery.py` & `celery_starter-1.0.3/src/celery_starter/management/commands/runcelery.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,16 +132,21 @@
             for i in range(cmd_len):
                 if cmd[i] == '-A':
                     return cmd[i + 1].strip(), self.args[0]
 
                 if cmd[i].startswith('--app'):
                     return cmd[i].split('=')[-1].strip(), self.args[0]
         else:
-            if os.environ.get('CELERY_APP'):
-                return os.environ['CELERY_APP'], None
+            celery_app = (
+                os.environ.get('CELERY_APP', None)
+                or getattr(settings, 'CELERY_APP', None)
+                or default_app.conf.get('CELERY_APP', 'app')
+            )
+            if celery_app:
+                return celery_app, None
 
             settings_filename = 'settings.py'
             for root, _dirs, files in os.walk(self.BASE_DIR):
                 if settings_filename in files:
                     return root.rsplit('/', 1)[-1], None
 
         raise ValueError(L.celery_app_not_found)
```

### Comparing `celery_starter-1.0.2/src/celery_starter.egg-info/PKG-INFO` & `celery_starter-1.0.3/src/celery_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery_starter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django command to launch celery worker, beat, flower
 Home-page: https://github.com/Friskes/celery-starter
 Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
```

### Comparing `celery_starter-1.0.2/src/celery_starter.egg-info/SOURCES.txt` & `celery_starter-1.0.3/src/celery_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

