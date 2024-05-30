# Comparing `tmp/fileformats-0.9.4.tar.gz` & `tmp/fileformats-0.9.5.tar.gz`

## Comparing `fileformats-0.9.4.tar` & `fileformats-0.9.5.tar`

### file list

```diff
@@ -1,57 +1,43 @@
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/archive.py
--rw-r--r--   0        0        0    18033 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/audio.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/document.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/model.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/serialization.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/text.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/video.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/archive.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/document.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/medical.py
--rw-r--r--   0        0        0    83985 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/misc.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/serialization.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/application/tests/test_import.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/_version.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/classifier.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/converter.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/datatype.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/field.py
--rw-r--r--   0        0        0    50014 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/mark.py
--rw-r--r--   0        0        0    28358 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/mixin.py
--rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/utils.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/generic/__init__.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/generic/tests/test_generic.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/raster.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/vector.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/headers.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/magic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/classifiers/file.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fileformats-0.9.4/fileformats/testing/classifiers/generic.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.9.4/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.9.4/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.9.4/LICENSE
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.9.4/README.rst
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 fileformats-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    23242 2020-02-02 00:00:00.000000 fileformats-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/archive.py
+-rw-r--r--   0        0        0    18033 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/audio.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/document.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/model.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/serialization.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/text.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/video.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/archive.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/document.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/medical.py
+-rw-r--r--   0        0        0    83985 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/misc.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/application/serialization.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/_version.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/classifier.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/datatype.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/field.py
+-rw-r--r--   0        0        0    50018 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/mark.py
+-rw-r--r--   0        0        0    28358 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/core/utils.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/field/__init__.py
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/image/raster.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/image/vector.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/headers.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/magic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/classifiers/file.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fileformats-0.9.5/fileformats/testing/classifiers/generic.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fileformats-0.9.5/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.9.5/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.9.5/LICENSE
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fileformats-0.9.5/README.rst
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 fileformats-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    23206 2020-02-02 00:00:00.000000 fileformats-0.9.5/PKG-INFO
```

### Comparing `fileformats-0.9.4/fileformats/audio.py` & `fileformats-0.9.5/fileformats/audio.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/model.py` & `fileformats-0.9.5/fileformats/model.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/text.py` & `fileformats-0.9.5/fileformats/text.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/video.py` & `fileformats-0.9.5/fileformats/video.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/application/__init__.py` & `fileformats-0.9.5/fileformats/application/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/application/archive.py` & `fileformats-0.9.5/fileformats/application/archive.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/application/document.py` & `fileformats-0.9.5/fileformats/application/document.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/application/misc.py` & `fileformats-0.9.5/fileformats/application/misc.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/application/serialization.py` & `fileformats-0.9.5/fileformats/application/serialization.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/classifier.py` & `fileformats-0.9.5/fileformats/core/classifier.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/converter.py` & `fileformats-0.9.5/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/datatype.py` & `fileformats-0.9.5/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/exceptions.py` & `fileformats-0.9.5/fileformats/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/field.py` & `fileformats-0.9.5/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/fileset.py` & `fileformats-0.9.5/fileformats/core/fileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,17 +179,17 @@
         empty metadata array if not"""
         try:
             metadata = self.read_metadata()
         except FileFormatsExtrasPkgUninstalledError:
             raise
         except FileFormatsExtrasPkgNotCheckedError as e:
             logger.warning(str(e))
-            metadata = {}
+            metadata = None
         except FileFormatsExtrasError:
-            metadata = {}
+            metadata = None
         return metadata
 
     @mark.extra
     def read_metadata(self) -> ty.Dict[str, ty.Any]:
         """Reads any metadata associated with the fileset and returns it as a dict"""
         raise NotImplementedError
```

### Comparing `fileformats-0.9.4/fileformats/core/mark.py` & `fileformats-0.9.5/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/mixin.py` & `fileformats-0.9.5/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/core/utils.py` & `fileformats-0.9.5/fileformats/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,19 @@
     Parameters
     ----------
     fspaths : list[Path]
         file-system paths to detect the format of
     candidates: sequence[DataType], optional
         the candidates to select from, by default all file formats
     standard_only : bool, optional
-        If you only want to return matches from the "standard" IANA types, by default False
+        If you only want to return matches from the "standard" IANA types. Only relevant
+        if candidates is None, by default False
     skip_unconstrained : bool, optional
-        skip formats that aren't constrained by extension, magic number or another check
+        skip formats that aren't constrained by extension, magic number or another check.
+        Only relevant if candidates is None
     """
     import fileformats.core.mixin
 
     fspaths = fspaths_converter(fspaths)
     matches = []
     if candidates is None:
         candidates = fileformats.core.FileSet.all_formats
```

### Comparing `fileformats-0.9.4/fileformats/field/__init__.py` & `fileformats-0.9.5/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/generic/__init__.py` & `fileformats-0.9.5/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/image/__init__.py` & `fileformats-0.9.5/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/image/notclassifiedyet.py` & `fileformats-0.9.5/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/image/raster.py` & `fileformats-0.9.5/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/testing/headers.py` & `fileformats-0.9.5/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/testing/classifiers/file.py` & `fileformats-0.9.5/fileformats/testing/classifiers/file.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/fileformats/testing/classifiers/generic.py` & `fileformats-0.9.5/fileformats/testing/classifiers/generic.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/LICENSE` & `fileformats-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.9.4/README.rst` & `fileformats-0.9.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 FileFormats
 ===========
-.. image:: https://github.com/arcanaframework/fileformats/actions/workflows/tests.yml/badge.svg
-   :target: https://github.com/arcanaframework/fileformats/actions/workflows/tests.yml
+.. image:: https://github.com/arcanaframework/fileformats/actions/workflows/ci-cd.yml/badge.svg
+   :target: https://github.com/arcanaframework/fileformats/actions/workflows/ci-cd.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/arcanaframework/fileformats
 .. image:: https://img.shields.io/pypi/pyversions/fileformats.svg
    :target: https://pypi.python.org/pypi/fileformats/
    :alt: Supported Python versions
 .. image:: https://img.shields.io/pypi/v/fileformats.svg
    :target: https://pypi.python.org/pypi/fileformats/
    :alt: Latest Version
-.. image:: https://github.com/ArcanaFramework/fileformats/actions/workflows/docs.yml/badge.svg
+.. image:: https://img.shields.io/badge/docs-built-green
    :target: https://arcanaframework.github.io/fileformats/
    :alt: docs
 
 
 *Fileformats* provides a library of file-format types implemented as Python classes.
 The file-format types are designed to be used in type validation during the construction
 of data workflows (e.g. Pydra_, Fastr_), and also provide some basic data handling methods
@@ -101,29 +101,29 @@
 Format Conversion
 -----------------
 
 While not implemented in the main File-formats itself, file-formats provides hooks for other packages to implement extra behaviour such as format conversion. The `fileformats-extras <https://github.com/ArcanaFramework/fileformats-extras>`__ implements a number of converters between standard file-format types, e.g. archive types to/from generic file/directories, which if installed can be called using the `convert()` method.
 
 .. code-block:: python
 
-    from fileformats.archive import Zip
+    from fileformats.application import Zip
     from fileformats.generic import Directory
 
     zip_file = Zip.convert(Directory("/path/to/a/directory"))
     extracted = Directory.convert(zip_file)
     copied = extracted.copy_to("/path/to/output")
 
 The converters are implemented in the Pydra_ dataflow framework, and can be linked into
 wider Pydra_ workflows by creating a converter task
 
 .. code-block:: python
 
     import pydra
     from pydra.tasks.mypackage import MyTask
-    from fileformats.serialization import Json, Yaml
+    from fileformats.application import Json, Yaml
 
     wf = pydra.Workflow(name="a_workflow", input_spec=["in_json"])
     wf.add(
         Yaml.get_converter(Json, name="json2yaml", in_file=wf.lzin.in_json)
     )
     wf.add(
         MyTask(
```

### Comparing `fileformats-0.9.4/pyproject.toml` & `fileformats-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,18 @@
 allow-direct-references = true
 
 [tool.hatch.build]
 packages = [
     "fileformats",
 ]
 exclude = [
-    "/tests",
+    "tests",
+]
+include = [
+    "./fileformats"
 ]
 
 [tool.black]
 target-version = ['py38']
 exclude = "fileformats/core/_version.py"
 
 [tool.codespell]
```

### Comparing `fileformats-0.9.4/PKG-INFO` & `fileformats-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.9.4
+Version: 0.9.5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -136,25 +136,25 @@
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats
 ===========
-.. image:: https://github.com/arcanaframework/fileformats/actions/workflows/tests.yml/badge.svg
-   :target: https://github.com/arcanaframework/fileformats/actions/workflows/tests.yml
+.. image:: https://github.com/arcanaframework/fileformats/actions/workflows/ci-cd.yml/badge.svg
+   :target: https://github.com/arcanaframework/fileformats/actions/workflows/ci-cd.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/arcanaframework/fileformats
 .. image:: https://img.shields.io/pypi/pyversions/fileformats.svg
    :target: https://pypi.python.org/pypi/fileformats/
    :alt: Supported Python versions
 .. image:: https://img.shields.io/pypi/v/fileformats.svg
    :target: https://pypi.python.org/pypi/fileformats/
    :alt: Latest Version
-.. image:: https://github.com/ArcanaFramework/fileformats/actions/workflows/docs.yml/badge.svg
+.. image:: https://img.shields.io/badge/docs-built-green
    :target: https://arcanaframework.github.io/fileformats/
    :alt: docs
 
 
 *Fileformats* provides a library of file-format types implemented as Python classes.
 The file-format types are designed to be used in type validation during the construction
 of data workflows (e.g. Pydra_, Fastr_), and also provide some basic data handling methods
@@ -241,29 +241,29 @@
 Format Conversion
 -----------------
 
 While not implemented in the main File-formats itself, file-formats provides hooks for other packages to implement extra behaviour such as format conversion. The `fileformats-extras <https://github.com/ArcanaFramework/fileformats-extras>`__ implements a number of converters between standard file-format types, e.g. archive types to/from generic file/directories, which if installed can be called using the `convert()` method.
 
 .. code-block:: python
 
-    from fileformats.archive import Zip
+    from fileformats.application import Zip
     from fileformats.generic import Directory
 
     zip_file = Zip.convert(Directory("/path/to/a/directory"))
     extracted = Directory.convert(zip_file)
     copied = extracted.copy_to("/path/to/output")
 
 The converters are implemented in the Pydra_ dataflow framework, and can be linked into
 wider Pydra_ workflows by creating a converter task
 
 .. code-block:: python
 
     import pydra
     from pydra.tasks.mypackage import MyTask
-    from fileformats.serialization import Json, Yaml
+    from fileformats.application import Json, Yaml
 
     wf = pydra.Workflow(name="a_workflow", input_spec=["in_json"])
     wf.add(
         Yaml.get_converter(Json, name="json2yaml", in_file=wf.lzin.in_json)
     )
     wf.add(
         MyTask(
```

