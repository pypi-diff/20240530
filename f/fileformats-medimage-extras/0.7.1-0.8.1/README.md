# Comparing `tmp/fileformats_medimage_extras-0.7.1.tar.gz` & `tmp/fileformats_medimage_extras-0.8.1.tar.gz`

## Comparing `fileformats_medimage_extras-0.7.1.tar` & `fileformats_medimage_extras-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/_version.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/tests/test_dicom_metadata.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/LICENSE
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/README.rst
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    18942 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/_version.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/tests/test_dicom_metadata.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/tests/test_generators.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/README.rst
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    18951 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.8.1/PKG-INFO
```

### Comparing `fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/converters.py` & `fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,15 @@
     NiftiGzX,
     NiftiXBvec,
     NiftiBvec,
     NiftiGzBvec,
     NiftiGzXBvec,
 )
 
-try:
-    from pydra.tasks.mrtrix3.utils import MRConvert
-except ImportError:
-    from pydra.tasks.mrtrix3.latest import mrconvert as MRConvert
+from pydra.tasks.mrtrix3.latest import MrConvert
 from pydra.tasks.dcm2niix import Dcm2Niix
 
 
 @hook.converter(source_format=MedicalImage, target_format=Analyze, out_ext=Analyze.ext)
 def mrconvert(name, out_ext: str):
     """Initiate an MRConvert task with the output file extension set
 
@@ -39,15 +36,15 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return MRConvert(name=name, out_file="out" + out_ext)
+    return MrConvert(name=name, out_file="out" + out_ext)
 
 
 @pydra.mark.task
 def ensure_dicom_dir(dicom: DicomCollection) -> DicomDir:
     if isinstance(dicom, DicomSeries):
         dicom_dir_fspath = tempfile.mkdtemp()
         dicom.copy(dicom_dir_fspath, mode=DicomDir.CopyMode.link)
@@ -63,17 +60,15 @@
 @hook.converter(source_format=DicomCollection, target_format=Nifti)
 @hook.converter(source_format=DicomCollection, target_format=NiftiGz, compress="y")
 @hook.converter(source_format=DicomCollection, target_format=NiftiX)
 @hook.converter(source_format=DicomCollection, target_format=NiftiGzX, compress="y")
 @hook.converter(source_format=DicomCollection, target_format=NiftiXBvec)
 @hook.converter(source_format=DicomCollection, target_format=NiftiBvec)
 @hook.converter(source_format=DicomCollection, target_format=NiftiGzBvec)
-@hook.converter(
-    source_format=DicomCollection, target_format=NiftiGzXBvec, compress="y"
-)
+@hook.converter(source_format=DicomCollection, target_format=NiftiGzXBvec, compress="y")
 def extended_dcm2niix(
     name,
     compress: str = "n",
     file_postfix: ty.Optional[str] = None,
     side_car_jq: ty.Optional[str] = None,
     extract_volume: ty.Optional[int] = None,
     to_4d: bool = False,
@@ -143,22 +138,23 @@
     )
     out_file = wf.dcm2niix.lzout.out_file
     out_json = wf.dcm2niix.lzout.out_json
     # Add MRConvert step to either select a single volume of a 4D dataset or the inverse,
     # wrap a single volume in a 4D dataset
     if extract_volume is not None or to_4d:
         if extract_volume:
-            coord = [3, extract_volume]
+            coord = (3, extract_volume)
             axes = [0, 1, 2]
         else:  # to_4d
             coord = attrs.NOTHING  # type: ignore
             axes = [0, 1, 2, -1]
         wf.add(
-            MRConvert(
+            MrConvert(
                 in_file=out_file,
+                out_file="out" + NiftiGzX.ext,
                 coord=coord,
                 axes=axes,
                 name="mrconvert",
             )
         )
         out_file = wf.mrconvert.lzout.out_file
     # Add JQ edit of side car to allow manual fixing of any conversion issues
```

### Comparing `fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/dicom.py` & `fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/tests/test_dicom_metadata.py` & `fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/tests/test_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.7.1/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage_extras-0.8.1/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,36 +30,33 @@
 @pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
 def test_dicom_to_nifti_select_suffix(dummy_mixedfmap_dicom):
 
     nifti_gz_x_ph = NiftiGzX.convert(dummy_mixedfmap_dicom, file_postfix="_ph")
     nifti_gz_x_imaginary = NiftiGzX.convert(
         dummy_mixedfmap_dicom, file_postfix="_imaginary"
     )
-    nifti_gz_x_real = NiftiGzX.convert(
-        dummy_mixedfmap_dicom, file_postfix="_real"
-    )
+    nifti_gz_x_real = NiftiGzX.convert(dummy_mixedfmap_dicom, file_postfix="_real")
 
     assert list(nifti_gz_x_ph.dims()) == [256, 256, 60]
     assert list(nifti_gz_x_imaginary.dims()) == [256, 256, 60]
     assert list(nifti_gz_x_real.dims()) == [256, 256, 60]
 
 
-@pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
+# @pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
+@pytest.mark.xfail(reason="Waiting on next Pydra release")
 def test_dicom_to_nifti_with_extract_volume(dummy_dwi_dicom):
 
     nifti_gz_x_e1 = NiftiGzX.convert(dummy_dwi_dicom, extract_volume=30)
     assert nifti_gz_x_e1.metadata["dim"][0] == 3
 
 
 @pytest.mark.xfail(reason="refactoring of side car handling incomplete")
 def test_dicom_to_nifti_with_jq_edit(dummy_t1w_dicom):
 
-    nifti_gz_x = NiftiGzX.convert(
-        dummy_t1w_dicom, side_car_jq=".EchoTime *= 1000"
-    )
+    nifti_gz_x = NiftiGzX.convert(dummy_t1w_dicom, side_car_jq=".EchoTime *= 1000")
     assert nifti_gz_x.metadata["EchoTime"] == 2.07
 
 
 @pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
 def test_dicom_to_niftix_with_fslgrad(dummy_dwi_dicom):
 
     logger.debug("Performing FSL grad conversion")
@@ -73,15 +70,16 @@
     ]
 
     assert all(b in (0.0, 3000.0) for b in nifti_gz_x_fsgrad.encoding.b_values)
     assert len(bvec_mags) == 60
     assert all(abs(1 - m) < 1e5 for m in bvec_mags)
 
 
-@pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
+# @pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
+@pytest.mark.xfail(reason="Waiting on next Pydra release")
 def test_dicom_to_nifti_as_4d(dummy_t1w_dicom):
 
     nifti_gz_x_e1 = NiftiGzX.convert(dummy_t1w_dicom, to_4d=True)
     assert nifti_gz_x_e1.metadata["dim"][0] == 4
 
 
 @pytest.mark.xfail(condition=OLD_MRTRIX_VERSION, reason="Old MRtrix version")
```

### Comparing `fileformats_medimage_extras-0.7.1/LICENSE` & `fileformats_medimage_extras-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.7.1/README.rst` & `fileformats_medimage_extras-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.7.1/pyproject.toml` & `fileformats_medimage_extras-0.8.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,20 @@
     "jq >=1.4.0",
     "nibabel >=5.0.0",
     "numpy >=1.20",
     "medimages4tests >=0.3.0",
     "pydicom >=2.3.1",
     "pydra >= 0.22.0",
     "pydra-dcm2niix",
-    "pydra-mrtrix3",
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
+    "pydra-mrtrix3 >= 3.0.3a0",
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
@@ -44,34 +37,23 @@
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
-    "codecov",
-]
+dev = ["black", "pre-commit", "codespell", "flake8", "flake8-pyproject"]
+test = ["pytest >=6.2.5", "pytest-env>=0.6.2", "pytest-cov>=2.12.1", "codecov"]
 
 [project.urls]
 repository = "https://github.com/ArcanaFramework/fileformats-medimage"
 
 [tool.hatch.version]
 source = "vcs"
-raw-options = {root = ".."}
+raw-options = { root = ".." }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "fileformats/extras/medimage/_version.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["fileformats"]
 
@@ -80,13 +62,11 @@
 exclude = "fileformats/extras/medimage/_version.py"
 
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
 extend-ignore = ['E203', 'E501', 'E129', 'F403']
```

### Comparing `fileformats_medimage_extras-0.7.1/PKG-INFO` & `fileformats_medimage_extras-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage-extras
-Version: 0.7.1
+Version: 0.8.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -116,15 +116,15 @@
 Requires-Dist: fileformats>=0.6
 Requires-Dist: jq>=1.4.0
 Requires-Dist: medimages4tests>=0.3.0
 Requires-Dist: nibabel>=5.0.0
 Requires-Dist: numpy>=1.20
 Requires-Dist: pydicom>=2.3.1
 Requires-Dist: pydra-dcm2niix
-Requires-Dist: pydra-mrtrix3
+Requires-Dist: pydra-mrtrix3>=3.0.3a0
 Requires-Dist: pydra>=0.22.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

