# Comparing `tmp/fileformats_medimage_mrtrix3_extras-0.1.tar.gz` & `tmp/fileformats_medimage_mrtrix3_extras-3.0.4a5.tar.gz`

## Comparing `fileformats_medimage_mrtrix3_extras-0.1.tar` & `fileformats_medimage_mrtrix3_extras-3.0.4a5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/.codespell-ignorewords
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/.flake8
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/conftest.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/pytest.ini
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/_version.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/converters.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/gradients.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/tracks.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/README.rst
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/pyproject.toml
--rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/.codespell-ignorewords
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/.flake8
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/conftest.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/pytest.ini
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/_version.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/converters.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/gradients.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/tracks.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/.gitignore
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/README.rst
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/pyproject.toml
+-rw-r--r--   0        0        0    18242 2020-02-02 00:00:00.000000 fileformats_medimage_mrtrix3_extras-3.0.4a5/PKG-INFO
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/conftest.py` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,13 +34,12 @@
 
 @pytest.fixture
 def work_dir():
     work_dir = tempfile.mkdtemp()
     return Path(work_dir)
 
 
-
 @pytest.fixture(scope="session")
 def dummy_dwi_dicom():
     import medimages4tests.dummy.dicom.mri.dwi.siemens.skyra.syngo_d13c as module
 
     return DicomDir(module.get_image())
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/converters.py` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from fileformats.core import hook
 from fileformats.medimage.base import MedicalImage
 
 from fileformats.medimage_mrtrix3 import (
     ImageFormat as MrtrixImage,
     ImageHeader as MrtrixImageHeader,
 )
+
 try:
-    from pydra.tasks.mrtrix3.utils import MRConvert
+    from pydra.tasks.mrtrix3.v3_0 import MrConvert
 except ImportError:
-    from pydra.tasks.mrtrix3.latest import mrconvert as MRConvert
+    from pydra.tasks.mrtrix3.latest import mrconvert as MrConvert
+
     in_out_file_kwargs = {"in_file": "input", "out_file": "output"}
 else:
     in_out_file_kwargs = {}
 
 
 @hook.converter(
     source_format=MedicalImage,
     target_format=MrtrixImage,
     out_ext=MrtrixImage.ext,
-    **in_out_file_kwargs
+    **in_out_file_kwargs,
 )
 def mrconvert(name, out_ext: str, **kwargs):
     """Initiate an MRConvert task with the output file extension set
 
     Parameters
     ----------
     name : str
@@ -31,22 +33,22 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return MRConvert(name=name, out_file="out" + out_ext, **kwargs)
+    return MrConvert(name=name, out_file="out" + out_ext, **kwargs)
 
 
 @hook.converter(
     source_format=MedicalImage,
     target_format=MrtrixImageHeader,
     out_ext=MrtrixImageHeader.ext,
-    **in_out_file_kwargs
+    **in_out_file_kwargs,
 )
 def mrconvert2(name, out_ext: str, **kwargs):
     """Initiate an MRConvert task with the output file extension set
 
     Parameters
     ----------
     name : str
@@ -55,8 +57,8 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return MRConvert(name=name, out_file="out" + out_ext, **kwargs)
+    return MrConvert(name=name, out_file="out" + out_ext, **kwargs)
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/image.py` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 from unittest import mock
 import typing as ty
 from pathlib import Path
 import numpy as np
-from random import Random
 from medimages4tests.dummy.nifti import get_image as get_dummy_nifti
-from fileformats.core import FileSet
+from fileformats.core import FileSet, SampleFileGenerator
 from fileformats.medimage import MedicalImage, Nifti1
 from fileformats.medimage_mrtrix3 import ImageFormat
 
 
 @FileSet.generate_sample_data.register
-def generate_mrtrix_sample_data(mif: ImageFormat, dest_dir: Path, seed: ty.Union[int, Random] = 0, stem: ty.Optional[str] = None) -> ty.Iterable[Path]:
-    nifti = Nifti1(get_dummy_nifti(dest_dir / "nifti.nii"))
+def generate_mrtrix_sample_data(
+    mif: ImageFormat,
+    generator: SampleFileGenerator,
+) -> ty.Iterable[Path]:
+    nifti = Nifti1(get_dummy_nifti(generator.dest_dir / "nifti.nii"))
     with mock.patch.dict(os.environ, {"MRTRIX_CLI_PARSE_ONLY": "0"}):
         mif = ImageFormat.convert(nifti)
     return mif.fspaths
 
 
 @MedicalImage.read_array.register
 def mrtrix_read_array(mif: ImageFormat) -> np.ndarray:
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/tracks.py` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/tracks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import time
 import struct
 import math
 from pathlib import Path
 import typing as ty
-from random import Random
-from fileformats.core import FileSet
+from fileformats.core import FileSet, SampleFileGenerator
 from fileformats.medimage_mrtrix3 import Tracks
 
 
 @FileSet.generate_sample_data.register
-def generate_tracks_sample_data(tracks: Tracks, dest_dir: Path, seed: ty.Union[int, Random] = 0, stem: ty.Optional[str] = None) -> ty.Iterable[Path]:
+def generate_tracks_sample_data(
+    tracks: Tracks,
+    generator: SampleFileGenerator,
+) -> ty.Iterable[Path]:
     """Generate a tracks file with a single straight track of length 10"""
-    fspath = dest_dir / "tracks.tck"
+    fspath = generator.dest_dir / "tracks.tck"
     timestamp = str(time.time() * 1e9 + time.process_time_ns())
     contents = f"""mrtrix tracks
 datatype: Float32BE
 timestamp: {timestamp}
 count: 1
 total_count: 1
 file: . """
     byte_contents = contents.encode()
     offset = len(byte_contents) + math.ceil(math.log10(len(byte_contents))) + 5
     byte_contents += str(offset).encode() + b"\nEND\n"
     for i in range(10):
         ib = i.to_bytes(32, "big")
         byte_contents += ib + ib + ib
-    nan_bytes = struct.pack('!d', float('nan'))
-    inf_bytes = struct.pack('!d', float('inf'))
+    nan_bytes = struct.pack("!d", float("nan"))
+    inf_bytes = struct.pack("!d", float("inf"))
     byte_contents += nan_bytes + nan_bytes + nan_bytes
     byte_contents += inf_bytes + inf_bytes + inf_bytes
     with open(fspath, "wb") as f:
         f.write(byte_contents)
     return [fspath]
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/fileformats/extras/medimage_mrtrix3/tests/test_converters.py` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/fileformats/extras/medimage_mrtrix3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/LICENSE` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
 To the extent possible, if any provision of this Public License is deemed unenforceable, it shall be automatically reformed to the minimum extent necessary to make it enforceable. If the provision cannot be reformed, it shall be severed from this Public License without affecting the enforceability of the remaining terms and conditions.
 No term or condition of this Public License will be waived and no failure to comply consented to unless expressly agreed to by the Licensor.
 Nothing in this Public License constitutes or may be interpreted as a limitation upon, or waiver of, any privileges and immunities that apply to the Licensor or You, including from the legal processes of any jurisdiction or authority.
 Creative Commons is not a party to its public licenses. Notwithstanding, Creative Commons may elect to apply one of its public licenses to material it publishes and in those instances will be considered the “Licensor.” The text of the Creative Commons public licenses is dedicated to the public domain under the CC0 Public Domain Dedication. Except for the limited purpose of indicating that material is shared under a Creative Commons public license or as otherwise permitted by the Creative Commons policies published at creativecommons.org/policies, Creative Commons does not authorize the use of the trademark “Creative Commons” or any other trademark or logo of Creative Commons without its prior written consent including, without limitation, in connection with any unauthorized modifications to any of its public licenses or any other arrangements, understandings, or agreements concerning use of licensed material. For the avoidance of doubt, this paragraph does not form part of the public licenses.
 
 Creative Commons may be contacted at creativecommons.org.
 
-Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations.
+Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations.
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/README.rst` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/pyproject.toml` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,22 @@
 [project]
 name = "fileformats-medimage-mrtrix3-extras"
 description = "Classes for representing different file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
     "fileformats >= 0.8",
-    "fileformats-medimage-mrtrix3",
-    "pydra >= 0.22.0"
-]
-license = {file = "LICENSE"}
-authors = [
-    {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
-]
-maintainers = [
-    {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
-]
-keywords = [
-    "file formats",
-    "data",
+    "fileformats-medimage-mrtrix3 >=3.0.4a4",
+    "medimages4tests",
+    "pydra >= 0.23.0",
 ]
+license = { file = "LICENSE" }
+authors = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
+maintainers = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
+keywords = ["file formats", "data"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
@@ -36,38 +30,25 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = [
-    "black",
-    "pre-commit",
-    "codespell",
-    "flake8",
-    "flake8-pyproject",
-]
-test = [
-    "pytest >=6.2.5",
-    "pytest-env>=0.6.2",
-    "pytest-cov>=2.12.1",
-    "medimages4tests",
-    "codecov",
-]
+dev = ["black", "pre-commit", "codespell", "flake8", "flake8-pyproject"]
+test = ["pytest >=6.2.5", "pytest-env>=0.6.2", "pytest-cov>=2.12.1", "codecov"]
 
-converters = [
-]
+converters = []
 
 [project.urls]
 repository = "https://github.com/MRtrix3/mrtrix3"
 
 [tool.hatch.version]
 source = "vcs"
-raw-options = { root = "../../" }
+raw-options = { root = "../.." }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "fileformats/extras/medimage_mrtrix3/_version.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["fileformats"]
 
@@ -76,13 +57,11 @@
 exclude = "fileformats/extras/medimage_mrtrix3/_version.py"
 
 [tool.codespell]
 ignore-words = ".codespell-ignorewords"
 
 [tool.flake8]
 doctests = true
-per-file-ignores = [
-    "__init__.py:F401"
-]
+per-file-ignores = ["__init__.py:F401"]
 max-line-length = 88
 select = "C,E,F,W,B,B950"
 extend-ignore = ['E203', 'E501', 'E129']
```

### Comparing `fileformats_medimage_mrtrix3_extras-0.1/PKG-INFO` & `fileformats_medimage_mrtrix3_extras-3.0.4a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fileformats-medimage-mrtrix3-extras
-Version: 0.1
+Version: 3.0.4a5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/MRtrix3/mrtrix3
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -107,27 +107,27 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: fileformats-medimage-mrtrix3
+Requires-Dist: fileformats-medimage-mrtrix3>=3.0.4a4
 Requires-Dist: fileformats>=0.8
-Requires-Dist: pydra>=0.22.0
+Requires-Dist: medimages4tests
+Requires-Dist: pydra>=0.23.0
 Provides-Extra: converters
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: codecov; extra == 'test'
-Requires-Dist: medimages4tests; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats-mrtrix3 Extras
 ==========================
```

