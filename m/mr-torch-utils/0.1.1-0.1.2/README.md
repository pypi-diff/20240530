# Comparing `tmp/mr_torch_utils-0.1.1.tar.gz` & `tmp/mr_torch_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mr_torch_utils-0.1.1.tar", last modified: Wed May 29 10:53:36 2024, max compression
+gzip compressed data, was "mr_torch_utils-0.1.2.tar", last modified: Thu May 30 17:07:53 2024, max compression
```

## Comparing `mr_torch_utils-0.1.1.tar` & `mr_torch_utils-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-27 15:16:52.000000 mr_torch_utils-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      525 2024-05-29 10:53:29.000000 mr_torch_utils-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-29 10:53:36.000000 mr_torch_utils-0.1.1/src/mr_torch_utils.egg-info/top_level.txt
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 10:53:36.249603 mr_torch_utils-0.1.1/src/torch_utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      119 2024-05-27 15:18:38.000000 mr_torch_utils-0.1.1/src/torch_utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-05-29 10:39:55.000000 mr_torch_utils-0.1.1/src/torch_utils/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      856 2024-05-29 10:46:54.000000 mr_torch_utils-0.1.1/src/torch_utils/datasets.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-27 15:16:52.000000 mr_torch_utils-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      525 2024-05-30 17:07:51.000000 mr_torch_utils-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-05-30 17:07:53.000000 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-30 17:07:53.000000 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 17:07:53.000000 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-30 17:07:53.000000 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-30 17:07:53.000000 mr_torch_utils-0.1.2/src/mr_torch_utils.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 17:07:53.087621 mr_torch_utils-0.1.2/src/torch_utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      119 2024-05-27 15:18:38.000000 mr_torch_utils-0.1.2/src/torch_utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-05-29 10:39:55.000000 mr_torch_utils-0.1.2/src/torch_utils/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      872 2024-05-30 15:49:08.000000 mr_torch_utils-0.1.2/src/torch_utils/datasets.py
```

### Comparing `mr_torch_utils-0.1.1/pyproject.toml` & `mr_torch_utils-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mr-torch-utils"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `mr_torch_utils-0.1.1/src/torch_utils/datasets.py` & `mr_torch_utils-0.1.2/src/torch_utils/datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,16 +19,16 @@
       return self.samples[idx]
     else:
       x = self.sample(idx)
       self.samples[idx] = x
       return x
     
 class IterDataset(IterableDataset[T], Generic[T]):
-  def __init__(self, samples: Iterable[T], num_samples: int):
+  def __init__(self, samples: Callable[[], Iterable[T]], num_samples: int):
     self.samples = samples
     self.num_samples = num_samples
 
   def __len__(self):
     return self.num_samples
 
   def __iter__(self):
-    return iter(self.samples)
+    return iter(self.samples())
```

