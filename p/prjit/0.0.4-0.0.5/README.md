# Comparing `tmp/prjit-0.0.4.tar.gz` & `tmp/prjit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prjit-0.0.4.tar", last modified: Wed May 29 08:22:27 2024, max compression
+gzip compressed data, was "prjit-0.0.5.tar", last modified: Wed May 29 08:25:49 2024, max compression
```

## Comparing `prjit-0.0.4.tar` & `prjit-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.202182 prjit-0.0.4/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:22:27.201989 prjit-0.0.4/PKG-INFO
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.200244 prjit-0.0.4/bin/
--rwxr-xr-x   0 archiba    (501) staff       (20)    18214 2024-05-29 08:19:19.000000 prjit-0.0.4/bin/prjit
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.201781 prjit-0.0.4/prjit.egg-info/
--rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/PKG-INFO
--rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/SOURCES.txt
--rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/dependency_links.txt
--rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/requires.txt
--rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-29 08:22:27.000000 prjit-0.0.4/prjit.egg-info/top_level.txt
-drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:22:27.201595 prjit-0.0.4/prjitter/
--rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-29 08:22:20.000000 prjit-0.0.4/prjitter/__init__.py
--rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.4/prjitter/bundles.py
--rw-r--r--   0 archiba    (501) staff       (20)     4422 2024-05-29 08:22:15.000000 prjit-0.0.4/prjitter/config.py
--rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.4/prjitter/state.py
--rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.4/prjitter/switcher.py
--rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-29 08:22:27.202219 prjit-0.0.4/setup.cfg
--rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-29 08:22:23.000000 prjit-0.0.4/setup.py
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:25:49.034917 prjit-0.0.5/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:25:49.034575 prjit-0.0.5/PKG-INFO
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:25:49.032810 prjit-0.0.5/bin/
+-rwxr-xr-x   0 archiba    (501) staff       (20)    18218 2024-05-29 08:24:56.000000 prjit-0.0.5/bin/prjit
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:25:49.034314 prjit-0.0.5/prjit.egg-info/
+-rw-r--r--   0 archiba    (501) staff       (20)      410 2024-05-29 08:25:49.000000 prjit-0.0.5/prjit.egg-info/PKG-INFO
+-rw-r--r--   0 archiba    (501) staff       (20)      261 2024-05-29 08:25:49.000000 prjit-0.0.5/prjit.egg-info/SOURCES.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        1 2024-05-29 08:25:49.000000 prjit-0.0.5/prjit.egg-info/dependency_links.txt
+-rw-r--r--   0 archiba    (501) staff       (20)       75 2024-05-29 08:25:49.000000 prjit-0.0.5/prjit.egg-info/requires.txt
+-rw-r--r--   0 archiba    (501) staff       (20)        9 2024-05-29 08:25:49.000000 prjit-0.0.5/prjit.egg-info/top_level.txt
+drwxr-xr-x   0 archiba    (501) staff       (20)        0 2024-05-29 08:25:49.034132 prjit-0.0.5/prjitter/
+-rw-r--r--   0 archiba    (501) staff       (20)       22 2024-05-29 08:25:45.000000 prjit-0.0.5/prjitter/__init__.py
+-rw-r--r--   0 archiba    (501) staff       (20)     1962 2024-05-27 07:05:22.000000 prjit-0.0.5/prjitter/bundles.py
+-rw-r--r--   0 archiba    (501) staff       (20)     4422 2024-05-29 08:22:15.000000 prjit-0.0.5/prjitter/config.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3794 2024-05-27 07:27:41.000000 prjit-0.0.5/prjitter/state.py
+-rw-r--r--   0 archiba    (501) staff       (20)     3958 2024-05-27 08:10:10.000000 prjit-0.0.5/prjitter/switcher.py
+-rw-r--r--   0 archiba    (501) staff       (20)       38 2024-05-29 08:25:49.034988 prjit-0.0.5/setup.cfg
+-rw-r--r--   0 archiba    (501) staff       (20)      609 2024-05-29 08:25:34.000000 prjit-0.0.5/setup.py
```

### Comparing `prjit-0.0.4/bin/prjit` & `prjit-0.0.5/bin/prjit`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 print('Executing:', ' '.join(command))
                 if not dry_run:
                     subprocess.run(command)
             state.current_project = project_name
             state.bound_bundle_ids = []
             state.save_current()
             switch_log_path = global_config.switch_log_path()
-            if old_project is None:
+            if old_project is not None:
                 switch_log_path.open('a').write(f'Action:exit,ProjectName:{old_project},Time:{datetime.now().isoformat()}\n')
             switch_log_path.open('a').write(f'Action:switch,ProjectName:{project_name},Time:{datetime.now().isoformat()}\n')
         else:
             print('Switching cancelled')
 
     def exit(self, dry_run: bool = False):
         global_config = GlobalConfig.load_from_env()
```

### Comparing `prjit-0.0.4/prjitter/bundles.py` & `prjit-0.0.5/prjitter/bundles.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.4/prjitter/config.py` & `prjit-0.0.5/prjitter/config.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.4/prjitter/state.py` & `prjit-0.0.5/prjitter/state.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.4/prjitter/switcher.py` & `prjit-0.0.5/prjitter/switcher.py`

 * *Files identical despite different names*

### Comparing `prjit-0.0.4/setup.py` & `prjit-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='prjit',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(include=['prjitter', 'prjitter.*']),
     url='https://github.com/archiba/prjit',
     license='',
     author='archiba',
     author_email='yuki-chiba@outlook.jp',
     description='Define a project workspace and switch files and applications',
     python_requirems='>=3.9',
```

