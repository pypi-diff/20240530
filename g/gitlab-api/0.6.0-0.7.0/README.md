# Comparing `tmp/gitlab_api-0.6.0-py2.py3-none-any.whl.zip` & `tmp/gitlab_api-0.7.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15203 bytes, number of entries: 10
+Zip file size: 15204 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      274 b- defN 23-Sep-21 02:46 gitlab_api/__init__.py
 -rw-r--r--  2.0 unx      517 b- defN 23-Sep-21 02:46 gitlab_api/decorators.py
 -rw-r--r--  2.0 unx      463 b- defN 23-Sep-21 02:46 gitlab_api/exceptions.py
 -rw-r--r--  2.0 unx   128541 b- defN 23-Sep-21 02:46 gitlab_api/gitlab_api.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-15 15:19 gitlab_api/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-15 15:20 gitlab_api-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3804 b- defN 23-Oct-15 15:20 gitlab_api-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-15 15:20 gitlab_api-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Oct-15 15:20 gitlab_api-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      800 b- defN 23-Oct-15 15:20 gitlab_api-0.6.0.dist-info/RECORD
-10 files, 135695 bytes uncompressed, 13843 bytes compressed:  89.8%
+-rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:25 gitlab_api/version.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:25 gitlab_api-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3855 b- defN 23-Oct-28 03:25 gitlab_api-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:25 gitlab_api-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Oct-28 03:25 gitlab_api-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      800 b- defN 23-Oct-28 03:25 gitlab_api-0.7.0.dist-info/RECORD
+10 files, 135746 bytes uncompressed, 13844 bytes compressed:  89.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: gitlab_api/gitlab_api.py
 Comment: 
 
 Filename: gitlab_api/version.py
 Comment: 
 
-Filename: gitlab_api-0.6.0.dist-info/LICENSE
+Filename: gitlab_api-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: gitlab_api-0.6.0.dist-info/METADATA
+Filename: gitlab_api-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: gitlab_api-0.6.0.dist-info/WHEEL
+Filename: gitlab_api-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: gitlab_api-0.6.0.dist-info/top_level.txt
+Filename: gitlab_api-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlab_api-0.6.0.dist-info/RECORD
+Filename: gitlab_api-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlab_api/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.6.0'
+__version__ = '0.7.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `gitlab_api-0.6.0.dist-info/LICENSE` & `gitlab_api-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gitlab_api-0.6.0.dist-info/METADATA` & `gitlab_api-0.7.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gitlab-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: GitLab API Python Wrapper
 Home-page: https://github.com/Knuckles-Team/gitlab-api
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Public Domain
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: urllib3 (>=1.26.13)
 
 # GitLab API
 
@@ -38,15 +39,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/gitlab-api)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/gitlab-api)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/gitlab-api)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/gitlab-api)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/gitlab-api)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/gitlab-api)
 
-*Version: 0.6.0*
+*Version: 0.7.0*
 
 GitLab API Python Wrapper
 
 Includes a large portion of useful API calls to GitLab
 
 This repository is actively maintained - Contributions are welcome!
```

## Comparing `gitlab_api-0.6.0.dist-info/RECORD` & `gitlab_api-0.7.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 gitlab_api/__init__.py,sha256=P50kdKjJkp9yiQ49DJKSwR9uFPE7vBoTmDwvNAf0VTo,274
 gitlab_api/decorators.py,sha256=i4Y1P64ALbNZ-Vt8MxR9fhb_i1evLB0_vKWjO0Bl2Mc,517
 gitlab_api/exceptions.py,sha256=D2wU4uENRLlLldeplf_qcDpYUVFdq_6L8JxNeIU7soU,463
 gitlab_api/gitlab_api.py,sha256=D6Uh8QclJX21S4K2Z--8u4Czcwd5W6-SQADor7x3nrY,128541
-gitlab_api/version.py,sha256=gO8BLKzpTbVdwjtv4mzScee0RMbIoAvk8PCBFoR5gMQ,116
-gitlab_api-0.6.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
-gitlab_api-0.6.0.dist-info/METADATA,sha256=O734PFWS2t6ZC9F0wQUknnO71ukNVYKCkkpTZOiAsko,3804
-gitlab_api-0.6.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-gitlab_api-0.6.0.dist-info/top_level.txt,sha256=nd1ty1-efj5HDc14wL4tzW1k_vF3qni3wPspalPLsR4,11
-gitlab_api-0.6.0.dist-info/RECORD,,
+gitlab_api/version.py,sha256=DEpmsreHKLkk1HePeizyVrVAnG3OvqvP-AFKZPao1lc,116
+gitlab_api-0.7.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
+gitlab_api-0.7.0.dist-info/METADATA,sha256=qL_m_5_fZM5UUgI0vOP092AGJhAEnocQSPSK-d5uGmw,3855
+gitlab_api-0.7.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+gitlab_api-0.7.0.dist-info/top_level.txt,sha256=nd1ty1-efj5HDc14wL4tzW1k_vF3qni3wPspalPLsR4,11
+gitlab_api-0.7.0.dist-info/RECORD,,
```

