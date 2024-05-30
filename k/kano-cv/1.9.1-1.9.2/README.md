# Comparing `tmp/kano-cv-1.9.1.tar.gz` & `tmp/kano-cv-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kano-cv-1.9.1.tar", last modified: Sat Feb 17 09:36:01 2024, max compression
+gzip compressed data, was "kano-cv-1.9.2.tar", last modified: Sat Feb 17 09:50:44 2024, max compression
```

## Comparing `kano-cv-1.9.1.tar` & `kano-cv-1.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:36:01.282708 kano-cv-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-17 09:35:40.000000 kano-cv-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-17 09:36:01.282708 kano-cv-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-17 09:35:40.000000 kano-cv-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:36:01.278708 kano-cv-1.9.1/kano/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:36:01.282708 kano-cv-1.9.1/kano/complex/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/complex/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/complex/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/complex/roboflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/complex/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-17 09:35:40.000000 kano-cv-1.9.1/kano/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:36:01.282708 kano-cv-1.9.1/kano_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-17 09:36:01.000000 kano-cv-1.9.1/kano_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-17 09:36:01.000000 kano-cv-1.9.1/kano_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 09:36:01.000000 kano-cv-1.9.1/kano_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-17 09:36:01.000000 kano-cv-1.9.1/kano_cv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-17 09:36:01.000000 kano-cv-1.9.1/kano_cv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-17 09:35:40.000000 kano-cv-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 09:36:01.282708 kano-cv-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:50:44.271867 kano-cv-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-17 09:50:21.000000 kano-cv-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-17 09:50:44.271867 kano-cv-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-17 09:50:21.000000 kano-cv-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:50:44.267867 kano-cv-1.9.2/kano/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:50:44.271867 kano-cv-1.9.2/kano/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/complex/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/complex/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/complex/roboflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/complex/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-17 09:50:21.000000 kano-cv-1.9.2/kano/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 09:50:44.271867 kano-cv-1.9.2/kano_cv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-17 09:50:44.000000 kano-cv-1.9.2/kano_cv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-17 09:50:44.000000 kano-cv-1.9.2/kano_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 09:50:44.000000 kano-cv-1.9.2/kano_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-17 09:50:44.000000 kano-cv-1.9.2/kano_cv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-17 09:50:44.000000 kano-cv-1.9.2/kano_cv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-17 09:50:21.000000 kano-cv-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 09:50:44.271867 kano-cv-1.9.2/setup.cfg
```

### Comparing `kano-cv-1.9.1/LICENSE` & `kano-cv-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/PKG-INFO` & `kano-cv-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kano-cv
-Version: 1.9.1
+Version: 1.9.2
 Summary: Helpful functions for Computer Vision tasks
 Author-email: egliette <leminhtu74@gmail.com>
 License: Copyright (c) 2012-2024 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -40,15 +40,15 @@
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pip-tools>=7.3.0; extra == "dev"
 Requires-Dist: pytest>=8.0.0; extra == "dev"
 Requires-Dist: build>=1.0.3; extra == "dev"
 Requires-Dist: twine>=5.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.6.1; extra == "dev"
-Requires-Dist: python-semantic-release>=9.0.0; extra == "dev"
+Requires-Dist: python-semantic-release>=9.1.0; extra == "dev"
 
 # 🦌 Kano - Tools for Computer Vision Tasks
 
 [![Kano CI](https://github.com/egliette/kano/actions/workflows/python-app.yml/badge.svg)](https://github.com/egliette/kano/actions/workflows/python-app.yml)
 
 **Kano** is a Python package providing utility functions for Computer Vision tasks. Its primary focus is simplifying lengthy functions, allowing developers to concentrate more on the main processes.
```

### Comparing `kano-cv-1.9.1/README.md` & `kano-cv-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano/complex/roboflow.py` & `kano-cv-1.9.2/kano/complex/roboflow.py`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano/complex/segmentation.py` & `kano-cv-1.9.2/kano/complex/segmentation.py`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano/file_utils.py` & `kano-cv-1.9.2/kano/file_utils.py`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano/image_utils.py` & `kano-cv-1.9.2/kano/image_utils.py`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano/video_utils.py` & `kano-cv-1.9.2/kano/video_utils.py`

 * *Files identical despite different names*

### Comparing `kano-cv-1.9.1/kano_cv.egg-info/PKG-INFO` & `kano-cv-1.9.2/kano_cv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kano-cv
-Version: 1.9.1
+Version: 1.9.2
 Summary: Helpful functions for Computer Vision tasks
 Author-email: egliette <leminhtu74@gmail.com>
 License: Copyright (c) 2012-2024 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -40,15 +40,15 @@
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pip-tools>=7.3.0; extra == "dev"
 Requires-Dist: pytest>=8.0.0; extra == "dev"
 Requires-Dist: build>=1.0.3; extra == "dev"
 Requires-Dist: twine>=5.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.6.1; extra == "dev"
-Requires-Dist: python-semantic-release>=9.0.0; extra == "dev"
+Requires-Dist: python-semantic-release>=9.1.0; extra == "dev"
 
 # 🦌 Kano - Tools for Computer Vision Tasks
 
 [![Kano CI](https://github.com/egliette/kano/actions/workflows/python-app.yml/badge.svg)](https://github.com/egliette/kano/actions/workflows/python-app.yml)
 
 **Kano** is a Python package providing utility functions for Computer Vision tasks. Its primary focus is simplifying lengthy functions, allowing developers to concentrate more on the main processes.
```

### Comparing `kano-cv-1.9.1/pyproject.toml` & `kano-cv-1.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kano-cv"
-version = "1.9.1"
+version = "1.9.2"
 description = "Helpful functions for Computer Vision tasks"
 readme = "README.md"
 authors = [{ name = "egliette", email = "leminhtu74@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -28,15 +28,15 @@
     "isort>=5.13.2",
     "flake8>=7.0.0",
     "pip-tools>=7.3.0",
     "pytest>=8.0.0",
     "build>=1.0.3",
     "twine>=5.0.0",
     "pre-commit>=3.6.1",
-    "python-semantic-release>=9.0.0",
+    "python-semantic-release>=9.1.0",
 ]
 
 [project.urls]
 Github = "https://github.com/egliette/kano"
 
 [tool.isort]
 line_length = 79
```

