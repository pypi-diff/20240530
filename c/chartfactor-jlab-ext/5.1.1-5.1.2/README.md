# Comparing `tmp/chartfactor_jlab_ext-5.1.1.tar.gz` & `tmp/chartfactor_jlab_ext-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartfactor_jlab_ext-5.1.1.tar", last modified: Wed May 29 13:42:50 2024, max compression
+gzip compressed data, was "chartfactor_jlab_ext-5.1.2.tar", last modified: Thu May 30 21:00:02 2024, max compression
```

## Comparing `chartfactor_jlab_ext-5.1.1.tar` & `chartfactor_jlab_ext-5.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.404198 chartfactor_jlab_ext-5.1.1/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/LICENSE
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.1.1/MANIFEST.in
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-29 13:42:50.403962 chartfactor_jlab_ext-5.1.1/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/README.md
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.399411 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/.DS_Store
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/_version.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.399639 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/package.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.401132 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/remoteEntry.4c8d261cdf4e51bc6f2a.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-05-29 13:42:48.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/style.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-05-29 13:42:49.000000 chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.403782 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-29 13:42:50.000000 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-05-29 13:42:50.000000 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-29 13:42:50.000000 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-29 13:42:39.000000 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-05-29 13:42:50.000000 chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/top_level.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/install.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.403236 chartfactor_jlab_ext-5.1.1/lib/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor_jlab_ext-5.1.1/lib/cfs.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.1.1/lib/commons.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.1.1/lib/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor_jlab_ext-5.1.1/lib/model.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.1.1/lib/runner.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.1.1/lib/storage-utils.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-05-29 13:42:07.000000 chartfactor_jlab_ext-5.1.1/package.json
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/pyproject.toml
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-05-29 13:42:50.404239 chartfactor_jlab_ext-5.1.1/setup.cfg
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.1.1/setup.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:42:50.403629 chartfactor_jlab_ext-5.1.1/style/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/style/base.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/style/index.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.1/style/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor_jlab_ext-5.1.1/yarn.lock
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.481883 chartfactor_jlab_ext-5.1.2/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/LICENSE
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.1.2/MANIFEST.in
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-30 21:00:02.481664 chartfactor_jlab_ext-5.1.2/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/README.md
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.477869 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/.DS_Store
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/_version.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.478098 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/package.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.479609 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/remoteEntry.d122a8a71c8f1d57f05b.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-05-30 21:00:00.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/style.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.481466 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-30 20:59:49.000000 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-05-30 21:00:02.000000 chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/install.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.480818 chartfactor_jlab_ext-5.1.2/lib/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor_jlab_ext-5.1.2/lib/cfs.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.1.2/lib/commons.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.1.2/lib/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor_jlab_ext-5.1.2/lib/model.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.1.2/lib/runner.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.1.2/lib/storage-utils.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-05-30 20:59:27.000000 chartfactor_jlab_ext-5.1.2/package.json
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/pyproject.toml
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-05-30 21:00:02.481918 chartfactor_jlab_ext-5.1.2/setup.cfg
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.1.2/setup.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 21:00:02.481290 chartfactor_jlab_ext-5.1.2/style/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/style/base.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/style/index.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.1.2/style/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor_jlab_ext-5.1.2/yarn.lock
```

### Comparing `chartfactor_jlab_ext-5.1.1/LICENSE` & `chartfactor_jlab_ext-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/PKG-INFO` & `chartfactor_jlab_ext-5.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.1.1
+Version: 5.1.2
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor_jlab_ext-5.1.1/README.md` & `chartfactor_jlab_ext-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/.DS_Store` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/package.json` & `chartfactor_jlab_ext-5.1.2/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649122807017543%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'5.1.2'"}*

```diff
@@ -24,19 +24,14 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Aktiun/chartfactor-jlab-ext",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.4c8d261cdf4e51bc6f2a.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "chartfactor-jlab-ext/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -69,9 +64,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.1.1"
+    "version": "5.1.2"
 }
```

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/remoteEntry.4c8d261cdf4e51bc6f2a.js` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/remoteEntry.d122a8a71c8f1d57f05b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.1.1", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.1.2", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor-jlab-ext/labextension/static/third-party-licenses.json` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/PKG-INFO` & `chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.1.1
+Version: 5.1.2
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor_jlab_ext-5.1.1/chartfactor_jlab_ext.egg-info/SOURCES.txt` & `chartfactor_jlab_ext-5.1.2/chartfactor_jlab_ext.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
 chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
 chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
-chartfactor-jlab-ext/labextension/static/remoteEntry.4c8d261cdf4e51bc6f2a.js
+chartfactor-jlab-ext/labextension/static/remoteEntry.d122a8a71c8f1d57f05b.js
 chartfactor-jlab-ext/labextension/static/style.js
 chartfactor-jlab-ext/labextension/static/third-party-licenses.json
 chartfactor_jlab_ext.egg-info/PKG-INFO
 chartfactor_jlab_ext.egg-info/SOURCES.txt
 chartfactor_jlab_ext.egg-info/dependency_links.txt
 chartfactor_jlab_ext.egg-info/not-zip-safe
 chartfactor_jlab_ext.egg-info/top_level.txt
```

### Comparing `chartfactor_jlab_ext-5.1.1/lib/cfs.js` & `chartfactor_jlab_ext-5.1.2/lib/cfs.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/lib/commons.js` & `chartfactor_jlab_ext-5.1.2/lib/commons.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/lib/index.js` & `chartfactor_jlab_ext-5.1.2/lib/index.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/lib/model.js` & `chartfactor_jlab_ext-5.1.2/lib/model.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/lib/runner.js` & `chartfactor_jlab_ext-5.1.2/lib/runner.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/lib/storage-utils.js` & `chartfactor_jlab_ext-5.1.2/lib/storage-utils.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/package.json` & `chartfactor_jlab_ext-5.1.2/chartfactor-jlab-ext/labextension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649122807017543%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.d122a8a71c8f1d57f05b.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'5.1.2'"}*

```diff
@@ -24,14 +24,19 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Aktiun/chartfactor-jlab-ext",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.d122a8a71c8f1d57f05b.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "chartfactor-jlab-ext/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -64,9 +69,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.1.1"
+    "version": "5.1.2"
 }
```

### Comparing `chartfactor_jlab_ext-5.1.1/setup.py` & `chartfactor_jlab_ext-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.1.1/yarn.lock` & `chartfactor_jlab_ext-5.1.2/yarn.lock`

 * *Files identical despite different names*

