# Comparing `tmp/fileformats_medimage-0.7.1.tar.gz` & `tmp/fileformats_medimage-0.8.1.tar.gz`

## Comparing `fileformats_medimage-0.7.1.tar` & `fileformats_medimage-0.8.1.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/pytest.ini
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/LICENSE
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/README.rst
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/pyproject.toml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/base.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/itk.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/surface.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/anatomical_entity/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/imaging/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/imaging/derivatives.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/contents/imaging/modality.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/raw/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/raw/mri/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/raw/pet/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/raw/pet/base.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/raw/pet/siemens.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/tests/test_dicom.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/fileformats/medimage/tests/test_nifti.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/LICENSE
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/README.rst
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    18984 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/pytest.ini
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/LICENSE
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/README.rst
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/tests/test_generators.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/base.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/itk.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/surface.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/anatomical_entity/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/imaging/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/imaging/derivatives.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/imaging/modality.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/property/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/property/imaging_procedure/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/property/imaging_procedure/cross_sectional_procedure/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/property/imaging_procedure/cross_sectional_procedure/mr_procedure/__init__.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/contents/property/imaging_procedure/cross_sectional_procedure/mr_procedure/tissue_contrast.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/raw/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/raw/mri/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/raw/pet/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/raw/pet/base.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/raw/pet/siemens.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/tests/test_contents.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/README.rst
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    19086 2020-02-02 00:00:00.000000 fileformats_medimage-0.8.1/PKG-INFO
```

### Comparing `fileformats_medimage-0.7.1/.pre-commit-config.yaml` & `fileformats_medimage-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/conftest.py` & `fileformats_medimage-0.8.1/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/.github/workflows/ci-cd.yml` & `fileformats_medimage-0.8.1/.github/workflows/ci-cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,20 @@
     - name: Set up Python ${{ matrix.python-version }} on ${{ matrix.os }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Update build tools
       run: python3 -m pip install --upgrade pip
     - name: Install Package
-      run: python3 -m pip install -e .[test] -e ./extras[test]
+      run: python3 -m pip install .[test] ./extras[test]
     - name: Pytest
-      run: pytest -vvs --cov fileformats --cov-config .coveragerc --cov-report xml .
+      run: |
+        mkdir work-dir
+        cd work-dir
+        pytest -vvs --cov fileformats --cov-config .coveragerc --cov-report xml ..
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v2
       with:
         fail_ci_if_error: true
         token: ${{ secrets.CODECOV_TOKEN }}
 
   build:
```

### Comparing `fileformats_medimage-0.7.1/extras/LICENSE` & `fileformats_medimage-0.8.1/extras/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/extras/README.rst` & `fileformats_medimage-0.8.1/extras/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/extras/pyproject.toml` & `fileformats_medimage-0.8.1/extras/pyproject.toml`

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

### Comparing `fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/converters.py` & `fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/converters.py`

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

### Comparing `fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/dicom.py` & `fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py` & `fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/extras/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage-0.8.1/extras/fileformats/extras/medimage/tests/test_neuro_converters.py`

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

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/__init__.py` & `fileformats_medimage-0.8.1/fileformats/medimage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,33 +71,51 @@
     ScreenFilmRadiography,
     Stereoscopy,
     StereotacticRadiography,
     Spectroscopy,
     Tomography,
     ComputedTomography,
     Ultrasound,
-    MRI,
-    PET,
-    CR,
-    CT,
-    DX,
-    MG,
-    MR,
-    NM,
-    PT,
-    PX,
-    RF,
-    RG,
-    US,
+    Mri,
+    Pet,
+    Dti,
+    Dmri,
+    Fmri,
+    Cr,
+    Ct,
+    Dx,
+    Mg,
+    Mr,
+    Nm,
+    Pt,
+    Px,
+    Rf,
+    Rg,
+    Us,
 )
 from .contents.imaging.derivatives import Derivative, Mask  # noqa: F401
 from .contents.anatomical_entity.material_anatomical_entity.anatomical_structure import (  # noqa: F401
     Brain,
     SpinalCord,
 )
+from .contents.property.imaging_procedure.cross_sectional_procedure.mr_procedure.tissue_contrast import (  # noqa: F401
+    T1w,
+    T2w,
+    T2sw,
+    T1T2w,
+    Flair,
+    Dwi,
+    T2Weighted,
+    T1Weighted,
+    T2StarWeighted,
+    T1T2Weighted,
+    DiffusionWeighted,
+    FluidAttenuatedInversionRecovery,
+    IntermediateWeighted,
+)
 from .itk import (  # noqa: F401
     GDCM,
     GIPL,
     VTK,
     PGM,
     MetaImage,
     Nrrd,
```

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/base.py` & `fileformats_medimage-0.8.1/fileformats/medimage/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 class MedicalImage(WithClassifiers, FileSet):
 
     iana_mime: ty.Optional[str] = None
     INCLUDE_HDR_KEYS = None
     IGNORE_HDR_KEYS = None
     binary = True
+    classifiers_attr_name = "image_contents"
+    image_contents = ()
     allowed_classifiers = (ContentsClassifier,)
+    multiple_classifiers = True
     exclusive_classifiers = (ImagingModality, AnatomicalEntity, Derivative)
 
     @hook.extra
     def read_array(self) -> "numpy.ndarray":  # noqa
         """
         Returns the binary data of the image in a numpy array
         """
```

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/dicom.py` & `fileformats_medimage-0.8.1/fileformats/medimage/dicom.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from .base import MedicalImage
 
 # =====================================================================
 # Custom loader functions for different image types
 # =====================================================================
 
 
+def dicom_sort_key(dicom: Dicom) -> str:
+    """Sorts DICOM objects by SOPInstanceUID"""
+    return dicom.metadata["SOPInstanceUID"]
+
+
 class DicomCollection(MedicalImage):
     """Base class for collections of DICOM files, which can either be stored within a
     directory (DicomDir) or presented as a flat list (DicomSeries)
     """
 
     content_types = (Dicom,)
     iana_mime = None
@@ -23,21 +28,20 @@
     def __len__(self):
         return len(self.contents)
 
     @hook.extra
     def series_number(self) -> str:
         raise NotImplementedError
 
-    @cached_property
-    def contents(self) -> ty.List[Dicom]:
-        return sorted(super().contents, key=lambda d: d.metadata["SOPInstanceUID"])
-
 
 class DicomDir(DicomCollection, DirectoryContaining[Dicom]):
-    pass
+
+    @cached_property
+    def contents(self) -> ty.List[Dicom]:
+        return sorted(super().contents, key=dicom_sort_key)
 
 
 class DicomSeries(DicomCollection, SetOf[Dicom]):
     @classmethod
     def from_paths(
         cls,
         fspaths: ty.Iterable[Path],
@@ -71,14 +75,18 @@
                 (
                     str(dicom.metadata["StudyInstanceUID"]),
                     str(dicom.metadata["SeriesNumber"]),
                 )
             ].append(dicom)
         return set([cls(s) for s in series_dict.values()]), remaining
 
+    @cached_property
+    def contents(self) -> ty.List[Dicom]:
+        return sorted(super().contents, key=dicom_sort_key)
+
 
 @FileSet.read_metadata.register
 def dicom_collection_read_metadata(
     collection: DicomCollection, selected_keys: ty.Optional[ty.Sequence[str]] = None
 ) -> ty.Mapping[str, ty.Any]:
     # Collated DICOM headers across series
     collated = {}
```

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.8.1/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/itk.py` & `fileformats_medimage-0.8.1/fileformats/medimage/itk.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/misc.py` & `fileformats_medimage-0.8.1/fileformats/medimage/misc.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/nifti.py` & `fileformats_medimage-0.8.1/fileformats/medimage/nifti.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 from fileformats.generic import File
 from fileformats.core import hook
-from fileformats.core.mixin import (
-    WithSideCars, WithMagicNumber, WithAdjacentFiles)
+from fileformats.core.mixin import WithSideCars, WithMagicNumber, WithAdjacentFiles
 from fileformats.application import Json
+
 # from fileformats.text import Tsv
 from fileformats.application import Gzip
 from .base import MedicalImage
 
 
 class Nifti(MedicalImage, File):
```

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/contents/imaging/modality.py` & `fileformats_medimage-0.8.1/fileformats/medimage/contents/imaging/modality.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,210 +1,241 @@
 from .. import ContentsClassifier
 
 
 class ImagingModality(ContentsClassifier):
-    ontology_link = 'http://www.radlex.org/RID/RID10311'
-    description = 'Form of imaging that depends on the way the image is produced'
+    ontology_link = "http://www.radlex.org/RID/RID10311"
+    description = "Form of imaging that depends on the way the image is produced"
     dicom_modality = None
 
 
 class CombinedModalities(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID49580'
-    description = 'These are cases where 2 different modalities are ' \
-                  'performed in the same imaging setup without moving the ' \
-                  'patient. These classes were created as sets, with the ' \
-                  'individual modalities as the set members. Any reasoning ' \
-                  'involving modality should accommodate this.'
+    ontology_link = "http://www.radlex.org/RID/RID49580"
+    description = (
+        "These are cases where 2 different modalities are "
+        "performed in the same imaging setup without moving the "
+        "patient. These classes were created as sets, with the "
+        "individual modalities as the set members. Any reasoning "
+        "involving modality should accommodate this."
+    )
 
 
 class DualEnergyXrayAbsorptiometry(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10363'
+    ontology_link = "http://www.radlex.org/RID/RID10363"
     description = None
 
 
 class Fluoroscopy(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10361'
+    ontology_link = "http://www.radlex.org/RID/RID10361"
     description = None
 
 
 class MrFluoroscopy(Fluoroscopy):
-    ontology_link = 'http://www.radlex.org/RID/RID10319'
-    description = 'Non-invasive method of vascular imaging and determination ' \
-                  'of internal anatomy without injection of contrast media or ' \
-                  'radiation exposure. The technique is used especially in ' \
-                  'cerebral angiography as well as for studies of other vascular ' \
-                  'structures. [MeSH]'
+    ontology_link = "http://www.radlex.org/RID/RID10319"
+    description = (
+        "Non-invasive method of vascular imaging and determination "
+        "of internal anatomy without injection of contrast media or "
+        "radiation exposure. The technique is used especially in "
+        "cerebral angiography as well as for studies of other vascular "
+        "structures. [MeSH]"
+    )
 
 
 class RadioFluoroscopy(Fluoroscopy):
-    ontology_link = 'http://www.radlex.org/RID/RID45709'
-    description = 'Production of an image when x-rays strike a fluorescent screen. [MeSH]'
+    ontology_link = "http://www.radlex.org/RID/RID45709"
+    description = (
+        "Production of an image when x-rays strike a fluorescent screen. [MeSH]"
+    )
 
 
 class MagneticResonanceImaging(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10312'
-    description = 'Non-invasive method of demonstrating internal anatomy ' \
-                  'based on the principle that atomic nuclei in a strong ' \
-                  'magnetic field absorb pulses of radiofrequency energy and ' \
-                  'emit them as radiowaves which can be reconstructed into ' \
-                  'computerized images. The concept includes proton spin ' \
-                  'tomographic techniques. [MeSH]'
-    dicom_modality = 'MR'
+    ontology_link = "http://www.radlex.org/RID/RID10312"
+    description = (
+        "Non-invasive method of demonstrating internal anatomy "
+        "based on the principle that atomic nuclei in a strong "
+        "magnetic field absorb pulses of radiofrequency energy and "
+        "emit them as radiowaves which can be reconstructed into "
+        "computerized images. The concept includes proton spin "
+        "tomographic techniques. [MeSH]"
+    )
+    dicom_modality = "MR"
 
 
-class DiffusionTensorImaging(MagneticResonanceImaging):
-    ontology_link = 'http://www.radlex.org/RID/RID38778'
+class DiffusionMagneticResonanceImaging(MagneticResonanceImaging):
+    ontology_link = "http://www.radlex.org/RID/RID38778"
+    description = None
+
+
+class DiffusionTensorImaging(DiffusionMagneticResonanceImaging):
+    ontology_link = "http://www.radlex.org/RID/RID38778"
     description = None
 
 
 class DynamicContrast(MagneticResonanceImaging):
-    ontology_link = 'http://www.radlex.org/RID/RID49531'
-    description = 	'An imaging method with a timed series of T1-weighted ' \
-                     'images used to detect and measure signal intensity ' \
-                     'change (enhancement) over time following administration ' \
-                     'of intravenous contrast agent to noninvasively access ' \
-                     'tissue vascular characteristics.'
+    ontology_link = "http://www.radlex.org/RID/RID49531"
+    description = (
+        "An imaging method with a timed series of T1-weighted "
+        "images used to detect and measure signal intensity "
+        "change (enhancement) over time following administration "
+        "of intravenous contrast agent to noninvasively access "
+        "tissue vascular characteristics."
+    )
 
 
 class EnhancedMagneticResonanceImaging(MagneticResonanceImaging):
     pass
 
 
 class FunctionalMagneticResonanceImaging(MagneticResonanceImaging):
-    ontology_link = 'http://www.radlex.org/RID/RID10317'
+    ontology_link = "http://www.radlex.org/RID/RID10317"
     description = None
 
 
 class MagneticResonanceAngiography(MagneticResonanceImaging):
-    ontology_link = 'http://www.radlex.org/RID/RID10319'
+    ontology_link = "http://www.radlex.org/RID/RID10319"
     description = None
 
 
 class MagneticResonanceSpectroscopy(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10315'
-    description = '	Spectroscopic method of measuring the magnetic moment of ' \
-                  'elementary particles such as atomic nuclei, protons or ' \
-                  'electrons. It is employed in clinical applications such as ' \
-                  'nmr tomography (magnetic resonance imaging). [MeSH]'
+    ontology_link = "http://www.radlex.org/RID/RID10315"
+    description = (
+        "	Spectroscopic method of measuring the magnetic moment of "
+        "elementary particles such as atomic nuclei, protons or "
+        "electrons. It is employed in clinical applications such as "
+        "nmr tomography (magnetic resonance imaging). [MeSH]"
+    )
 
 
 class NuclearMedicineImaging(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10330'
+    ontology_link = "http://www.radlex.org/RID/RID10330"
     description = None
-    dicom_modality = 'NM'
+    dicom_modality = "NM"
 
 
 class PositronEmissionTomography(NuclearMedicineImaging):
-    ontology_link = 'http://www.radlex.org/RID/RID10337'
-    description = 'An imaging technique using compounds labelled with ' \
-                  'short-lived positron-emitting radionuclides (such as ' \
-                  'carbon-11, nitrogen-13, oxygen-15 and fluorine-18) to ' \
-                  'measure cell metabolism. It has been useful in study of ' \
-                  'soft tissues such as cancer; cardiovascular system; and ' \
-                  'brain. SPECT is closely related to PET, but uses isotopes ' \
-                  'with longer half-lives and resolution is lower. [MeSH]'
-    dicom_modality = 'PT'
+    ontology_link = "http://www.radlex.org/RID/RID10337"
+    description = (
+        "An imaging technique using compounds labelled with "
+        "short-lived positron-emitting radionuclides (such as "
+        "carbon-11, nitrogen-13, oxygen-15 and fluorine-18) to "
+        "measure cell metabolism. It has been useful in study of "
+        "soft tissues such as cancer; cardiovascular system; and "
+        "brain. SPECT is closely related to PET, but uses isotopes "
+        "with longer half-lives and resolution is lower. [MeSH]"
+    )
+    dicom_modality = "PT"
+
 
 class PanographicRadiograph(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10360'
+    ontology_link = "http://www.radlex.org/RID/RID10360"
     description = None
-    dicom_modality = 'PX'
+    dicom_modality = "PX"
 
 
 class ProjectionRadiography(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10345'
-    description = 'Examination of any part of the body for diagnostic purposes ' \
-                  'by means of roentgen rays, recording the image on a ' \
-                  'sensitized surface (such as photographic film). [MeSH]'
+    ontology_link = "http://www.radlex.org/RID/RID10345"
+    description = (
+        "Examination of any part of the body for diagnostic purposes "
+        "by means of roentgen rays, recording the image on a "
+        "sensitized surface (such as photographic film). [MeSH]"
+    )
 
 
 class ComputedRadiography(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID10349'
-    dicom_modality = 'CR'
+    ontology_link = "http://www.radlex.org/RID/RID10349"
+    dicom_modality = "CR"
     description = None
 
 
 class DigitalRadiography(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID10351'
-    dicom_modality = 'DR'
+    ontology_link = "http://www.radlex.org/RID/RID10351"
+    dicom_modality = "DR"
     description = None
 
 
 class DualEnergySubtractionRadiograpgy(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID10356'
+    ontology_link = "http://www.radlex.org/RID/RID10356"
     description = None
 
 
 class Mammography(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID10357'
+    ontology_link = "http://www.radlex.org/RID/RID10357"
     description = None
 
 
 class ScreenFilmRadiography(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID10353'
-    description = 'Conventional radiography'
-    dicom_modality = 'RG'
+    ontology_link = "http://www.radlex.org/RID/RID10353"
+    description = "Conventional radiography"
+    dicom_modality = "RG"
 
 
 class Stereoscopy(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID50131'
+    ontology_link = "http://www.radlex.org/RID/RID50131"
     description = None
 
 
 class StereotacticRadiography(ProjectionRadiography):
-    ontology_link = 'http://www.radlex.org/RID/RID50260'
+    ontology_link = "http://www.radlex.org/RID/RID50260"
     description = None
 
 
 class Spectroscopy(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10377'
-    description = 'The measurement of the amplitude of the components of a ' \
-                  'complex waveform throughout the frequency range of the ' \
-                  'waveform. (McGraw-Hill Dictionary of Scientific and ' \
-                  'Technical Terms, 4th ed) [MeSH]'
+    ontology_link = "http://www.radlex.org/RID/RID10377"
+    description = (
+        "The measurement of the amplitude of the components of a "
+        "complex waveform throughout the frequency range of the "
+        "waveform. (McGraw-Hill Dictionary of Scientific and "
+        "Technical Terms, 4th ed) [MeSH]"
+    )
 
 
 class Tomography(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID28840'
+    ontology_link = "http://www.radlex.org/RID/RID28840"
     description = None
 
 
 class ComputedTomography(Tomography):
-    ontology_link = 'http://www.radlex.org/RID/RID10321'
-    description = 'Tomography using x-ray transmission and a computer algorithm ' \
-                  'to reconstruct the image. [MeSH]'
-    dicom_modality = 'CT'
+    ontology_link = "http://www.radlex.org/RID/RID10321"
+    description = (
+        "Tomography using x-ray transmission and a computer algorithm "
+        "to reconstruct the image. [MeSH]"
+    )
+    dicom_modality = "CT"
 
 
 class Ultrasound(ImagingModality):
-    ontology_link = 'http://www.radlex.org/RID/RID10326'
-    description = 'The visualization of deep structures of the body by ' \
-                  'recording the reflections of echoes of pulses of ultrasonic ' \
-                  'waves directed into the tissues. Use of ultrasound for ' \
-                  'imaging or diagnostic purposes employs frequencies ranging ' \
-                  'from 1.6 to 10 megahertz. [MeSH]'
-    dicom_modality = 'US'
+    ontology_link = "http://www.radlex.org/RID/RID10326"
+    description = (
+        "The visualization of deep structures of the body by "
+        "recording the reflections of echoes of pulses of ultrasonic "
+        "waves directed into the tissues. Use of ultrasound for "
+        "imaging or diagnostic purposes employs frequencies ranging "
+        "from 1.6 to 10 megahertz. [MeSH]"
+    )
+    dicom_modality = "US"
 
 
 # Some extra abbreviations
-MRI = MagneticResonanceImaging
-PET = PositronEmissionTomography
+Mri = MagneticResonanceImaging
+Pet = PositronEmissionTomography
+Dmri = DiffusionMagneticResonanceImaging
+Dti = DiffusionTensorImaging
+Fmri = FunctionalMagneticResonanceImaging
 
 # DICOM abbreviations, taken from: https://dicom.nema.org/medical/dicom/current/output/chtml/part16/sect_CID_29.html
-CR = ComputedRadiography
-CT = ComputedTomography
-DX = DigitalRadiography
-MG = Mammography
-MR = MagneticResonanceImaging
-NM = NuclearMedicineImaging
-PT = PositronEmissionTomography
-PX = PanographicRadiograph
-RF = RadioFluoroscopy
-RG = ScreenFilmRadiography
-US = Ultrasound
+Cr = ComputedRadiography
+Ct = ComputedTomography
+Dx = DigitalRadiography
+Mg = Mammography
+Mr = MagneticResonanceImaging
+Nm = NuclearMedicineImaging
+Pt = PositronEmissionTomography
+Px = PanographicRadiograph
+Rf = RadioFluoroscopy
+Rg = ScreenFilmRadiography
+Us = Ultrasound
 # AR = Autorefraction
 # BI = Biomagnetic Imaging
 # BMD = Bone Mineral Densitometry
 # EPS = Cardiac Electrophysiology
 # DMS = Dermoscopy
 # DG = Diaphanography
 # ECG = Electrocardiography
```

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/raw/pet/base.py` & `fileformats_medimage-0.8.1/fileformats/medimage/raw/pet/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/raw/pet/siemens.py` & `fileformats_medimage-0.8.1/fileformats/medimage/raw/pet/siemens.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/fileformats/medimage/tests/test_dicom.py` & `fileformats_medimage-0.8.1/fileformats/medimage/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/LICENSE` & `fileformats_medimage-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/README.rst` & `fileformats_medimage-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.7.1/pyproject.toml` & `fileformats_medimage-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
     "medimages4tests >=0.3",
     "fileformats-medimage-extras",
+    "pydra-dcm2niix",
+    "pydra-mrtrix3 >=3.0.4a4",
 ]
 
 
 [project.urls]
 repository = "https://github.com/ArcanaFramework/fileformats-medimage"
```

### Comparing `fileformats_medimage-0.7.1/PKG-INFO` & `fileformats_medimage-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage
-Version: 0.7.1
+Version: 0.8.1
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -117,14 +117,16 @@
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: fileformats-medimage-extras; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
+Requires-Dist: pydra-dcm2niix; extra == 'test'
+Requires-Dist: pydra-mrtrix3>=3.0.4a4; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats - Medimage
 ======================
```

