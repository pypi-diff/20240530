# Comparing `tmp/fileformats_medimage_mrtrix3-3.0.3a0.tar.gz` & `tmp/fileformats_medimage_mrtrix3-3.0.4a5.tar.gz`

## Comparing `fileformats_medimage_mrtrix3-3.0.3a0.tar` & `fileformats_medimage_mrtrix3-3.0.4a5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.codespell-ignorewords
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.flake8
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/conftest.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/pytest.ini
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/_version.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/dwi.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/in_out.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/track.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/.gitignore
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/LICENSE
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/README.rst
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/pyproject.toml
--rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/.codespell-ignorewords
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/.flake8
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/conftest.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/pytest.ini
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/_version.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/dwi.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/in_out.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/track.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/tests/test_mime.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/.gitignore
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/README.rst
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/pyproject.toml
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3-3.0.4a5/PKG-INFO
```

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/conftest.py` & `fileformats_medimage_mrtrix3-3.0.4a5/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/dwi.py` & `fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/dwi.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/image.py` & `fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     @property
     def data_file(self):
         return self
 
 
 class ImageFormatGz(Gzip[ImageFormat]):
 
-    iana_mime = None
+    iana_mime = "application/x-image-format-gz"
     ext = ".mif.gz"
 
 
 class ImageHeader(BaseMrtrixImage):
 
     ext = ".mih"
```

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/fileformats/medimage_mrtrix3/in_out.py` & `fileformats_medimage_mrtrix3-3.0.4a5/fileformats/medimage_mrtrix3/in_out.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/.gitignore` & `fileformats_medimage_mrtrix3-3.0.4a5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -133,8 +133,8 @@
 
 # VS Code
 .vscode/
 
 # Hatchling
 _version.py
 
-#/pydra/tasks/mrtrix3/v3_0
+/pydra/tasks/mrtrix3/v3_0
```

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/LICENSE` & `fileformats_medimage_mrtrix3-3.0.4a5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/README.rst` & `fileformats_medimage_mrtrix3-3.0.4a5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/pyproject.toml` & `fileformats_medimage_mrtrix3-3.0.4a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ]
 
 [project.urls]
 repository = "https://github.com/MRtrix3/mrtrix3"
 
 [tool.hatch.version]
 source = "vcs"
-raw-options = { root = ".." }
+raw-options = { root = "../.." }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "fileformats/medimage_mrtrix3/_version.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["fileformats"]
```

### Comparing `fileformats_medimage_mrtrix3-3.0.3a0/PKG-INFO` & `fileformats_medimage_mrtrix3-3.0.4a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage-mrtrix3
-Version: 3.0.3a0
+Version: 3.0.4a5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/MRtrix3/mrtrix3
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

