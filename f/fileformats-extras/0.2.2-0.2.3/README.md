# Comparing `tmp/fileformats_extras-0.2.2.tar.gz` & `tmp/fileformats_extras-0.2.3.tar.gz`

## Comparing `fileformats_extras-0.2.2.tar` & `fileformats_extras-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,25 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.codespell-ignorewords
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/medical.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/archive/__init__.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/archive/converters.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/serialization/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/serialization/converters.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/serialization/yaml.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/application/tests/test_medical.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/core/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/core/_version.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/image/__init__.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/image/converters.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/image/readwrite.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/fileformats/extras/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/LICENSE
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/README.rst
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    18267 2020-02-02 00:00:00.000000 fileformats_extras-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/__init__.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/archive.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/medical.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/serialization.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/tests/test_application_archive.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/tests/test_application_medical.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/application/tests/test_application_serialization.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/core/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/core/_version.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/image/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/image/converters.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/image/readwrite.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/fileformats/extras/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/README.rst
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    18267 2020-02-02 00:00:00.000000 fileformats_extras-0.2.3/PKG-INFO
```

### Comparing `fileformats_extras-0.2.2/.pre-commit-config.yaml` & `fileformats_extras-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/conftest.py` & `fileformats_extras-0.2.3/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/.github/workflows/publish.yml` & `fileformats_extras-0.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/.github/workflows/tests.yml` & `fileformats_extras-0.2.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/fileformats/extras/application/medical.py` & `fileformats_extras-0.2.3/fileformats/extras/application/medical.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
         for e in dcm.elements()
         if getattr(e, "keyword", False) and e.keyword != "PixelData"  # type: ignore[union-attr]
     }
     return metadata
 
 
 @FileSet.generate_sample_data.register
-def dicom_dir_generate_sample_data(
+def dicom_generate_sample_data(
     dicom: Dicom, dest_dir: Path, seed: ty.Union[int, Random], stem: ty.Optional[str]
 ):
     return next(
         medimages4tests.dummy.dicom.mri.t1w.siemens.skyra.syngo_d13c.get_image().iterdir()
     )
```

### Comparing `fileformats_extras-0.2.2/fileformats/extras/application/archive/converters.py` & `fileformats_extras-0.2.3/fileformats/extras/application/archive.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/fileformats/extras/application/archive/tests/test_archive_converters.py` & `fileformats_extras-0.2.3/fileformats/extras/application/tests/test_application_archive.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/fileformats/extras/application/serialization/tests/test_serialization_converters.py` & `fileformats_extras-0.2.3/fileformats/extras/application/tests/test_application_serialization.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/fileformats/extras/image/converters.py` & `fileformats_extras-0.2.3/fileformats/extras/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/fileformats/extras/image/tests/test_image_converters.py` & `fileformats_extras-0.2.3/fileformats/extras/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/LICENSE` & `fileformats_extras-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/README.rst` & `fileformats_extras-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/pyproject.toml` & `fileformats_extras-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.2.2/PKG-INFO` & `fileformats_extras-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-extras
-Version: 0.2.2
+Version: 0.2.3
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

