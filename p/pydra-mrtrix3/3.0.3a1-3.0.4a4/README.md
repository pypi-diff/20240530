# Comparing `tmp/pydra_mrtrix3-3.0.3a1.tar.gz` & `tmp/pydra_mrtrix3-3.0.4a4.tar.gz`

## Comparing `pydra_mrtrix3-3.0.3a1.tar` & `pydra_mrtrix3-3.0.4a4.tar`

### file list

```diff
@@ -1,46 +1,338 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.gitattributes
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/CHANGELOG.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/codecov.yml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/conftest.py
--rwxr-xr-x   0        0        0    11414 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/generate.py
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/Makefile
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/make.bat
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/.codespell-ignorewords
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/.flake8
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/LICENSE
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/README.rst
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/conftest.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pyproject.toml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pytest.ini
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/track.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/tests/test_mime.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/.codespell-ignorewords
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/.flake8
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/README.rst
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/conftest.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pyproject.toml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pytest.ini
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/gradients.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/_version.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/latest.py
--rw-r--r--   0        0        0    10680 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/manual/mrcalc_.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.gitignore
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/LICENSE
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/README.rst
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pyproject.toml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/.gitattributes
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/CHANGELOG.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/codecov.yml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/conftest.py
+-rwxr-xr-x   0        0        0    12843 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/generate.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/docs/Makefile
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/docs/make.bat
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/docs/requirements.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/mrtrix3_version.txt/mrtrix3_version.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/_version.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/latest.py
+-rw-r--r--   0        0        0    10680 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/manual/mrcalc_.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/__init__.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/afdconnectivity_.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/amp2response_.py
+-rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/amp2sh_.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/connectome2tck_.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/connectomeedit_.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/connectomestats_.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dcmedit_.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dcminfo_.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirflip_.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirgen_.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirmerge_.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirorder_.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirsplit_.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dirstat_.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2adc_.py
+-rw-r--r--   0        0        0    12447 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2fod_.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_3dautomask_.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_ants_.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_b02template_.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_consensus_.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_fslbet_.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_hdbet_.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_legacy_.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_mean_.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_mtnorm_.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_synthstrip_.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2mask_trace_.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_dhollander_.py
+-rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_fa_.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_manual_.py
+-rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_msmt_5tt_.py
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_tax_.py
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2response_tournier_.py
+-rw-r--r--   0        0        0    10395 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwi2tensor_.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_ants_.py
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_fsl_.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_mtnorm_.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwibiasnormmask_.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwicat_.py
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwidenoise_.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwiextract_.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwifslpreproc_.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwigradcheck_.py
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwinormalise_group_.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwinormalise_manual_.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwinormalise_mtnorm_.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/dwishellmath_.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivett2gmwmi_.py
+-rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivett2vis_.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettcheck_.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettedit_.py
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettgen_freesurfer_.py
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettgen_fsl_.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettgen_gif_.py
+-rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fivettgen_hsvs_.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixel2peaks_.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixel2sh_.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixel2tsf_.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixel2voxel_.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelcfestats_.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelconnectivity_.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelconvert_.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelcorrespondence_.py
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelcrop_.py
+-rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelfilter_.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fixelreorient_.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fod2dec_.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/fod2fixel_.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/label2colour_.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/label2mesh_.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/labelconvert_.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/labelsgmfix_.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/labelstats_.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mask2glass_.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/maskdump_.py
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/maskfilter_.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mesh2voxel_.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/meshconvert_.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/meshfilter_.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mraverageheader_.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrcat_.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrcentroid_.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrcheckerboardmask_.py
+-rw-r--r--   0        0        0    11741 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrclusterstats_.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrcolour_.py
+-rw-r--r--   0        0        0    20203 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrconvert_.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrdegibbs_.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrdump_.py
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mredit_.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrfilter_.py
+-rw-r--r--   0        0        0    14536 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrgrid_.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrhistmatch_.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrhistogram_.py
+-rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrinfo_.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrmath_.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrmetric_.py
+-rw-r--r--   0        0        0    31397 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrregister_.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrstats_.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrthreshold_.py
+-rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrtransform_.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mrtrix_cleanup_.py
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/mtnormalise_.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/peaks2amp_.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/peaks2fixel_.py
+-rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/population_template_.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/responsemean_.py
+-rw-r--r--   0        0        0     9643 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/sh2amp_.py
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/sh2peaks_.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/sh2power_.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/sh2response_.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/shbasis_.py
+-rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/shconv_.py
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tck2connectome_.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tck2fixel_.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckconvert_.py
+-rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckdfc_.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckedit_.py
+-rw-r--r--   0        0        0    24149 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckgen_.py
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckglobal_.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckinfo_.py
+-rw-r--r--   0        0        0    15101 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckmap_.py
+-rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckresample_.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tcksample_.py
+-rw-r--r--   0        0        0    13198 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tcksift2_.py
+-rw-r--r--   0        0        0    10238 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tcksift_.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tckstats_.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tcktransform_.py
+-rw-r--r--   0        0        0    11699 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tensor2metric_.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/transformcalc_.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/transformcompose_.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/transformconvert_.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfdivide_.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfinfo_.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfmult_.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfsmooth_.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfthreshold_.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tsfvalidate_.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/vectorstats_.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/voxel2fixel_.py
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/voxel2mesh_.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/warp2metric_.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/warpconvert_.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/warpcorrect_.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/warpinit_.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/warpinvert_.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_afdconnectivity.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_amp2response.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_amp2sh.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_connectome2tck.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_connectomeedit.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_connectomestats.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dcmedit.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dcminfo.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirflip.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirgen.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirmerge.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirorder.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirsplit.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dirstat.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2adc.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2fod.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_3dautomask.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_ants.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_b02template.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_consensus.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_fslbet.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_hdbet.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_legacy.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_mean.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_mtnorm.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_synthstrip.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_trace.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_dhollander.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_fa.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_manual.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_msmt_5tt.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_tax.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_tournier.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2tensor.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_ants.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_fsl.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_mtnorm.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiasnormmask.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwicat.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwidenoise.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwiextract.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwifslpreproc.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwigradcheck.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_group.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_manual.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_mtnorm.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_dwishellmath.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivett2gmwmi.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivett2vis.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettcheck.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettedit.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_freesurfer.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_fsl.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_gif.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_hsvs.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2peaks.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2sh.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2tsf.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2voxel.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcfestats.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelconnectivity.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelconvert.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcorrespondence.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcrop.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelfilter.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fixelreorient.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fod2dec.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_fod2fixel.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_label2colour.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_label2mesh.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_labelconvert.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_labelsgmfix.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_labelstats.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mask2glass.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_maskdump.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_maskfilter.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mesh2voxel.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_meshconvert.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_meshfilter.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mraverageheader.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrcat.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrcentroid.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrcheckerboardmask.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrclusterstats.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrcolour.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrconvert.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrdegibbs.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrdump.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mredit.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrfilter.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrgrid.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrhistmatch.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrhistogram.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrinfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrmath.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrmetric.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrregister.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrstats.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrthreshold.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrtransform.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mrtrix_cleanup.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_mtnormalise.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_peaks2amp.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_peaks2fixel.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_population_template.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_responsemean.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_sh2amp.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_sh2peaks.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_sh2power.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_sh2response.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_shbasis.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_shconv.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tck2connectome.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tck2fixel.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckconvert.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckdfc.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckedit.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckgen.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckglobal.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckinfo.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckmap.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckresample.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tcksample.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tcksift.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tcksift2.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tckstats.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tcktransform.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tensor2metric.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_transformcalc.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_transformcompose.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_transformconvert.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfdivide.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfinfo.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfmult.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfsmooth.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfthreshold.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_tsfvalidate.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_vectorstats.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_voxel2fixel.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_voxel2mesh.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_warp2metric.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_warpconvert.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_warpcorrect.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_warpinit.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/v3_0/tests/test_warpinvert.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/.codespell-ignorewords
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/.flake8
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/conftest.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/pytest.ini
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/dwi.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/in_out.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/track.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/tests/test_mime.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/.codespell-ignorewords
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/.flake8
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/conftest.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/pytest.ini
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/converters.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/gradients.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/tracks.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/.gitignore
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/LICENSE
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/README.rst
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/pyproject.toml
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.4a4/PKG-INFO
```

### Comparing `pydra_mrtrix3-3.0.3a1/CHANGELOG.md` & `pydra_mrtrix3-3.0.4a4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/conftest.py` & `pydra_mrtrix3-3.0.4a4/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/generate.py` & `pydra_mrtrix3-3.0.4a4/generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,14 +58,71 @@
     "voxel",
     "vector",
     "warp",
     "response",
 ]
 
 
+XFAIL = [
+    "dirsplit",
+    "dwi2mask_3dautomask",
+    "dwi2mask_ants",
+    "dwi2mask_b02template",
+    "dwi2mask_consensus",
+    "dwi2mask_fslbet",
+    "dwi2mask_hdbet",
+    "dwi2mask_legacy",
+    "dwi2mask_mean",
+    "dwi2mask_mtnorm",
+    "dwi2mask_synthstrip",
+    "dwi2mask_trace",
+    "dwi2response_dhollander",
+    "dwi2response_fa",
+    "dwi2response_manual",
+    "dwi2response_msmt_5tt",
+    "dwi2response_tax",
+    "dwi2response_tournier",
+    "dwibiascorrect_ants",
+    "dwibiascorrect_fsl",
+    "dwibiascorrect_mtnorm",
+    "dwibiasnormmask",
+    "dwicat",
+    "dwifslpreproc",
+    "dwigradcheck",
+    "dwinormalise_group",
+    "dwinormalise_manual",
+    "dwinormalise_mtnorm",
+    "dwishellmath",
+    "fivettgen_freesurfer",
+    "fivettgen_fsl",
+    "fivettgen_gif",
+    "fivettgen_hsvs",
+    "fixelcfestats",
+    "fixelconnectivity",
+    "fixelconvert",
+    "fixelcorrespondence",
+    "fixelcrop",
+    "fixelfilter",
+    "fixelreorient",
+    "labelsgmfix",
+    "mask2glass",
+    "mrconvert",
+    "mrstats",
+    "mrtransform",
+    "mrtrix_cleanup",
+    "population_template",
+    "responsemean",
+    "tck2fixel",
+    "tckstats",
+    "tsfmult",
+    "voxel2fixel",
+    "warpinvert",
+]
+
+
 @click.command(
     help="""Loops through all MRtrix commands to generate Pydra
 (https://pydra.readthedocs.io) task interfaces for them
 
 CMD_DIR the command directory to list the commands from
 
 OUTPUT_DIR the output directory to write the generated files to
@@ -246,23 +303,30 @@
     tests_dir.mkdir(exist_ok=True)
     module = import_module(f"pydra.tasks.mrtrix3.{pkg_version}.{cmd_name}_")
     interface = getattr(module, pascal_case_task_name(cmd_name))
     task = interface()
 
     code_str = f"""# Auto-generated test for {cmd_name}
 
+import pytest
 from fileformats.generic import File, Directory, FsObject  # noqa
 from fileformats.medimage import Nifti1  # noqa
 from fileformats.medimage_mrtrix3 import ImageFormat, ImageIn, Tracks  # noqa
-from pydra.tasks.mrtrix3.{pkg_version} import {cmd_name}
+from pydra.tasks.mrtrix3.{pkg_version} import {pascal_case_task_name(cmd_name)}
+"""
 
+    if cmd_name in XFAIL:
+        code_str += (
+            f"""@pytest.mark.xfail(reason="Task {cmd_name} is known not pass yet")"""
+        )
 
+    code_str += f"""
 def test_{cmd_name.lower()}(tmp_path, cli_parse_only):
 
-    task = {cmd_name}(
+    task = {pascal_case_task_name(cmd_name)}(
 """
     input_fields = attrs.fields(type(task.inputs))
     output_fields = attrs.fields(make_klass(task.output_spec))
 
     for field in input_fields:
         if field.name in (
             "executable",
```

### Comparing `pydra_mrtrix3-3.0.3a1/docs/Makefile` & `pydra_mrtrix3-3.0.4a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/docs/make.bat` & `pydra_mrtrix3-3.0.4a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/LICENSE` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/README.rst` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/conftest.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pyproject.toml` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/pyproject.toml`

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

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/dwi.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/image.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats/fileformats/medimage_mrtrix3/in_out.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/LICENSE` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/README.rst` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/conftest.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pyproject.toml` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,21 @@
 name = "fileformats-medimage-mrtrix3-extras"
 description = "Classes for representing different file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
     "fileformats >= 0.8",
     "fileformats-medimage-mrtrix3",
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
+    "medimages4tests",
+    "pydra >= 0.22.0",
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
-raw-options = { root = ".." }
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

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from fileformats.medimage_mrtrix3 import (
     ImageFormat as MrtrixImage,
     ImageHeader as MrtrixImageHeader,
 )
 
 try:
-    from pydra.tasks.mrtrix3.utils import MrConvert
+    from pydra.tasks.mrtrix3.v3_0 import MrConvert
 except ImportError:
     from pydra.tasks.mrtrix3.latest import mrconvert as MrConvert
 
     in_out_file_kwargs = {"in_file": "input", "out_file": "output"}
 else:
     in_out_file_kwargs = {}
```

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/image.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/tracks.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py` & `pydra_mrtrix3-3.0.4a4/related-packages/fileformats-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/manual/mrcalc_.py` & `pydra_mrtrix3-3.0.4a4/pydra/tasks/mrtrix3/manual/mrcalc_.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/.gitignore` & `pydra_mrtrix3-3.0.4a4/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -133,8 +133,7 @@
 
 # VS Code
 .vscode/
 
 # Hatchling
 _version.py
 
-/pydra/tasks/mrtrix3/v3_0
```

### Comparing `pydra_mrtrix3-3.0.3a1/LICENSE` & `pydra_mrtrix3-3.0.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/README.rst` & `pydra_mrtrix3-3.0.4a4/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a1/pyproject.toml` & `pydra_mrtrix3-3.0.4a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-mrtrix3"
 description = "pydra-mrtrix3 contains Pydra task specifications for MRtrix3 tools"
 readme = "README.rst"
 requires-python = ">=3.8"
-dependencies = [
-    "pydra >=0.22",
-    "fileformats-medimage_mrtrix3 >=3.0.3a",
-    "pytest"]  # bug in fileformats requires this currently
-license = {file = "LICENSE"}
-authors = [
-    {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
-]
-maintainers = [
-    {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
-]
+dependencies = ["fileformats-medimage_mrtrix3", "numpy", "pydra >=0.23"]
+license = { file = "LICENSE" }
+authors = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
+maintainers = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 keywords = ["pydra"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
@@ -36,15 +29,15 @@
     "black",
     "pre-commit",
     "black >=22.12.0",
     "click >=8.1.3",
     "tqdm",
     "attrs >=23.1.0",
     "fileformats >= 0.8",
-    "fileformats-extras >= 0.2.1"
+    "fileformats-extras >= 0.2.1",
 ]
 doc = [
     "packaging",
     "sphinx >=2.1.2",
     "sphinx_rtd_theme",
     "sphinxcontrib-apidoc ~=0.3.0",
     "sphinxcontrib-napoleon",
@@ -53,14 +46,15 @@
 test = [
     "pytest >= 4.4.0",
     "pytest-cov",
     "pytest-env",
     "pytest-xdist",
     "pytest-rerunfailures",
     "codecov",
+    "fileformats-medimage_mrtrix3-extras",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "pydra/tasks/mrtrix3/_version.py"
@@ -74,13 +68,11 @@
 exclude = "_version.py"
 
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
 extend-ignore = ['E203', 'E501', 'E129', 'W503']
```

### Comparing `pydra_mrtrix3-3.0.3a1/PKG-INFO` & `pydra_mrtrix3-3.0.4a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydra-mrtrix3
-Version: 3.0.3a1
+Version: 3.0.4a4
 Summary: pydra-mrtrix3 contains Pydra task specifications for MRtrix3 tools
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License:    Copyright 2022 Nipype developers
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
@@ -24,17 +24,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: fileformats-medimage-mrtrix3>=3.0.3a
-Requires-Dist: pydra>=0.22
-Requires-Dist: pytest
+Requires-Dist: fileformats-medimage-mrtrix3
+Requires-Dist: numpy
+Requires-Dist: pydra>=0.23
 Provides-Extra: dev
 Requires-Dist: attrs>=23.1.0; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: black>=22.12.0; extra == 'dev'
 Requires-Dist: click>=8.1.3; extra == 'dev'
 Requires-Dist: fileformats-extras>=0.2.1; extra == 'dev'
 Requires-Dist: fileformats>=0.8; extra == 'dev'
@@ -45,14 +45,15 @@
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Requires-Dist: sphinx>=2.1.2; extra == 'doc'
 Requires-Dist: sphinxcontrib-apidoc~=0.3.0; extra == 'doc'
 Requires-Dist: sphinxcontrib-napoleon; extra == 'doc'
 Requires-Dist: sphinxcontrib-versioning; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: codecov; extra == 'test'
+Requires-Dist: fileformats-medimage-mrtrix3-extras; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-env; extra == 'test'
 Requires-Dist: pytest-rerunfailures; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
 Requires-Dist: pytest>=4.4.0; extra == 'test'
 Description-Content-Type: text/x-rst
```

