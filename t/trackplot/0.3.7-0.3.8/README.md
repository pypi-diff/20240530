# Comparing `tmp/trackplot-0.3.7.tar.gz` & `tmp/trackplot-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.3.7.tar", max compression
+gzip compressed data, was "trackplot-0.3.8.tar", max compression
```

## Comparing `trackplot-0.3.7.tar` & `trackplot-0.3.8.tar`

### file list

```diff
@@ -1,71 +1,41 @@
--rw-r--r--   0        0        0     1558 2023-11-30 02:11:14.704217 trackplot-0.3.7/LICENSE
--rw-r--r--   0        0        0     8836 2023-11-30 02:11:14.704217 trackplot-0.3.7/README.md
--rw-r--r--   0        0        0     1270 2024-01-23 08:15:41.292546 trackplot-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       38 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/__init__.py
--rw-r--r--   0        0        0      371 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/anno/AxLabel.py
--rw-r--r--   0        0        0        0 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/anno/__init__.py
--rw-r--r--   0        0        0     1545 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/anno/theme.py
--rw-r--r--   0        0        0     7428 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/CoordinateMap.py
--rw-r--r--   0        0        0     4425 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/GenomicLoci.py
--rw-r--r--   0        0        0     3546 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/Junction.py
--rw-r--r--   0        0        0     8881 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/Protein.py
--rw-r--r--   0        0        0     8580 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/ReadDepth.py
--rw-r--r--   0        0        0     8933 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/Readder.py
--rw-r--r--   0        0        0     1368 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/Stroke.py
--rw-r--r--   0        0        0     4254 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/Transcript.py
--rw-r--r--   0        0        0        0 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/__init__.py
--rw-r--r--   0        0        0     7991 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/base/pyUniprot.py
--rw-r--r--   0        0        0    43355 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/cli.py
--rw-r--r--   0        0        0     4745 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/conf/DomainSetting.py
--rw-r--r--   0        0        0        0 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/conf/__init__.py
--rw-r--r--   0        0        0     1342 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/conf/config.py
--rw-r--r--   0        0        0     3803 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/conf/drawing.py
--rw-r--r--   0        0        0    22297 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/conf/ui.py
--rw-r--r--   0        0        0     6341 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/ATAC.py
--rw-r--r--   0        0        0    23683 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Annotation.py
--rw-r--r--   0        0        0    12907 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Bam.py
--rw-r--r--   0        0        0     1481 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/BedGraph.py
--rw-r--r--   0        0        0     1515 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Bigwig.py
--rw-r--r--   0        0        0     3380 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Depth.py
--rw-r--r--   0        0        0     1233 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Fasta.py
--rw-r--r--   0        0        0     3539 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/File.py
--rw-r--r--   0        0        0     6413 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0        0        0      966 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Junction.py
--rw-r--r--   0        0        0     1020 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/Motif.py
--rw-r--r--   0        0        0    20423 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/ReadSegments.py
--rw-r--r--   0        0        0        0 2023-11-30 02:11:15.948219 trackplot-0.3.7/trackplot/file/__init__.py
--rw-r--r--   0        0        0    50302 2024-01-23 08:15:55.848573 trackplot-0.3.7/trackplot/plot.py
--rw-r--r--   0        0        0    52756 2023-11-30 02:11:15.952219 trackplot-0.3.7/trackplot/plot_func.py
--rw-r--r--   0        0        0     6403 2023-11-30 02:11:15.952219 trackplot-0.3.7/trackplot/plot_tests.py
--rw-r--r--   0        0        0    10264 2024-01-23 08:09:43.575919 trackplot-0.3.7/trackplot/server.py
--rw-r--r--   0        0        0     1171 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/Home-2ymNv-_c.js
--rw-r--r--   0        0        0      176 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/Home-I0kdDLBy.css
--rw-r--r--   0        0        0     1171 2024-01-23 07:23:25.318388 trackplot-0.3.7/ui/assets/Home-TBgKVcok.js
--rw-r--r--   0        0        0     1171 2024-01-23 07:42:13.324833 trackplot-0.3.7/ui/assets/Home-Urllcnym.js
--rw-r--r--   0        0        0     1171 2024-01-23 07:34:30.935001 trackplot-0.3.7/ui/assets/Home-XJ7AmKYn.js
--rw-r--r--   0        0        0     1171 2024-01-23 07:18:25.772539 trackplot-0.3.7/ui/assets/Home-xn91KpT-.js
--rw-r--r--   0        0        0   109287 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/Plot-1XGmwhdB.css
--rw-r--r--   0        0        0   276640 2024-01-23 07:42:13.324833 trackplot-0.3.7/ui/assets/Plot-3Au5A8Mh.js
--rw-r--r--   0        0        0   276719 2024-01-23 07:18:25.772539 trackplot-0.3.7/ui/assets/Plot-DoNwQXAX.js
--rw-r--r--   0        0        0   109218 2024-01-23 07:34:30.935001 trackplot-0.3.7/ui/assets/Plot-ODq4tgsg.css
--rw-r--r--   0        0        0   109218 2024-01-23 07:23:25.318388 trackplot-0.3.7/ui/assets/Plot-Rt8tCETk.css
--rw-r--r--   0        0        0   109218 2024-01-23 07:42:13.328833 trackplot-0.3.7/ui/assets/Plot-WuWliOwx.css
--rw-r--r--   0        0        0   109218 2024-01-23 07:18:25.772539 trackplot-0.3.7/ui/assets/Plot-aMhsBEEY.css
--rw-r--r--   0        0        0   276674 2024-01-23 07:23:25.318388 trackplot-0.3.7/ui/assets/Plot-glPweJSy.js
--rw-r--r--   0        0        0   277311 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/Plot-rg_JxZsu.js
--rw-r--r--   0        0        0   276662 2024-01-23 07:34:30.935001 trackplot-0.3.7/ui/assets/Plot-uy0yOMVn.js
--rw-r--r--   0        0        0    47061 2024-01-23 07:18:25.772539 trackplot-0.3.7/ui/assets/el-divider-Fd57SJVn.js
--rw-r--r--   0        0        0    47061 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/el-divider-GFInZ0ZC.js
--rw-r--r--   0        0        0    47061 2024-01-23 07:34:30.935001 trackplot-0.3.7/ui/assets/el-divider-MTfwtyAS.js
--rw-r--r--   0        0        0    47061 2024-01-23 07:42:13.324833 trackplot-0.3.7/ui/assets/el-divider-b4xNR7BF.js
--rw-r--r--   0        0        0    47061 2024-01-23 07:23:25.318388 trackplot-0.3.7/ui/assets/el-divider-qD9PCnRZ.js
--rw-r--r--   0        0        0     6794 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/el-divider-rvYA7bZe.css
--rw-r--r--   0        0        0   101864 2024-01-23 07:42:13.324833 trackplot-0.3.7/ui/assets/index-HgWSTqal.js
--rw-r--r--   0        0        0   101917 2024-01-23 07:23:25.318388 trackplot-0.3.7/ui/assets/index-UJJboihn.js
--rw-r--r--   0        0        0   101917 2024-01-23 07:18:25.772539 trackplot-0.3.7/ui/assets/index-a1mI4l5F.js
--rw-r--r--   0        0        0   101864 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/index-x1fPdXa6.js
--rw-r--r--   0        0        0   101864 2024-01-23 07:34:30.935001 trackplot-0.3.7/ui/assets/index-xxTAchCB.js
--rw-r--r--   0        0        0   314120 2024-01-23 08:07:37.243722 trackplot-0.3.7/ui/assets/index-yWBF9tT_.css
--rw-r--r--   0        0        0      476 2024-01-23 08:07:37.247722 trackplot-0.3.7/ui/index.html
--rw-r--r--   0        0        0     1497 2024-01-23 08:07:36.075720 trackplot-0.3.7/ui/vite.svg
--rw-r--r--   0        0        0    10231 1970-01-01 00:00:00.000000 trackplot-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1558 2024-05-07 11:22:49.784435 trackplot-0.3.8/LICENSE
+-rw-r--r--   0        0        0     8836 2024-05-07 11:22:49.784869 trackplot-0.3.8/README.md
+-rw-r--r--   0        0        0     1270 2024-05-29 03:05:19.663007 trackplot-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-05-07 11:22:50.584300 trackplot-0.3.8/trackplot/__init__.py
+-rw-r--r--   0        0        0      371 2024-05-07 11:22:50.584525 trackplot-0.3.8/trackplot/anno/AxLabel.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:22:50.584591 trackplot-0.3.8/trackplot/anno/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-07 11:22:50.584747 trackplot-0.3.8/trackplot/anno/theme.py
+-rw-r--r--   0        0        0     7428 2024-05-07 11:22:50.585020 trackplot-0.3.8/trackplot/base/CoordinateMap.py
+-rw-r--r--   0        0        0     4425 2024-05-07 11:22:50.585212 trackplot-0.3.8/trackplot/base/GenomicLoci.py
+-rw-r--r--   0        0        0     3546 2024-05-07 11:22:50.585355 trackplot-0.3.8/trackplot/base/Junction.py
+-rw-r--r--   0        0        0     8881 2024-05-07 11:22:50.585596 trackplot-0.3.8/trackplot/base/Protein.py
+-rw-r--r--   0        0        0     8580 2024-05-07 11:22:50.585821 trackplot-0.3.8/trackplot/base/ReadDepth.py
+-rw-r--r--   0        0        0     8933 2024-05-29 02:42:13.180670 trackplot-0.3.8/trackplot/base/Readder.py
+-rw-r--r--   0        0        0     1368 2024-05-07 11:22:50.586209 trackplot-0.3.8/trackplot/base/Stroke.py
+-rw-r--r--   0        0        0     4254 2024-05-07 11:22:50.586376 trackplot-0.3.8/trackplot/base/Transcript.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:22:50.586433 trackplot-0.3.8/trackplot/base/__init__.py
+-rw-r--r--   0        0        0     7991 2024-05-07 11:22:50.586634 trackplot-0.3.8/trackplot/base/pyUniprot.py
+-rw-r--r--   0        0        0    43355 2024-05-07 11:22:50.586964 trackplot-0.3.8/trackplot/cli.py
+-rw-r--r--   0        0        0     4745 2024-05-07 11:22:50.587268 trackplot-0.3.8/trackplot/conf/DomainSetting.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:22:50.587337 trackplot-0.3.8/trackplot/conf/__init__.py
+-rw-r--r--   0        0        0     1342 2024-05-07 11:22:50.587493 trackplot-0.3.8/trackplot/conf/config.py
+-rw-r--r--   0        0        0     3803 2024-05-07 11:22:50.587632 trackplot-0.3.8/trackplot/conf/drawing.py
+-rw-r--r--   0        0        0    22297 2024-05-07 11:22:50.587889 trackplot-0.3.8/trackplot/conf/ui.py
+-rw-r--r--   0        0        0     6341 2024-05-07 11:22:50.588194 trackplot-0.3.8/trackplot/file/ATAC.py
+-rw-r--r--   0        0        0    23683 2024-05-07 11:22:50.588432 trackplot-0.3.8/trackplot/file/Annotation.py
+-rw-r--r--   0        0        0    12907 2024-05-07 11:22:50.588739 trackplot-0.3.8/trackplot/file/Bam.py
+-rw-r--r--   0        0        0     1481 2024-05-07 11:22:50.588883 trackplot-0.3.8/trackplot/file/BedGraph.py
+-rw-r--r--   0        0        0     1515 2024-05-07 11:22:50.589028 trackplot-0.3.8/trackplot/file/Bigwig.py
+-rw-r--r--   0        0        0     3380 2024-05-07 11:22:50.589164 trackplot-0.3.8/trackplot/file/Depth.py
+-rw-r--r--   0        0        0     1233 2024-05-07 11:22:50.589289 trackplot-0.3.8/trackplot/file/Fasta.py
+-rw-r--r--   0        0        0     3539 2024-05-07 11:22:50.589427 trackplot-0.3.8/trackplot/file/File.py
+-rw-r--r--   0        0        0     6413 2024-05-07 11:22:50.589608 trackplot-0.3.8/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0        0        0      966 2024-05-07 11:22:50.589743 trackplot-0.3.8/trackplot/file/Junction.py
+-rw-r--r--   0        0        0     1020 2024-05-29 02:42:18.198181 trackplot-0.3.8/trackplot/file/Motif.py
+-rw-r--r--   0        0        0    20423 2024-05-07 11:22:50.590070 trackplot-0.3.8/trackplot/file/ReadSegments.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:22:50.590151 trackplot-0.3.8/trackplot/file/__init__.py
+-rw-r--r--   0        0        0    50427 2024-05-29 03:11:38.323310 trackplot-0.3.8/trackplot/plot.py
+-rw-r--r--   0        0        0    52821 2024-05-29 03:03:41.582711 trackplot-0.3.8/trackplot/plot_func.py
+-rw-r--r--   0        0        0     6403 2024-05-07 11:22:50.591044 trackplot-0.3.8/trackplot/plot_tests.py
+-rw-r--r--   0        0        0    10264 2024-05-07 11:22:50.591272 trackplot-0.3.8/trackplot/server.py
+-rw-r--r--   0        0        0    10231 1970-01-01 00:00:00.000000 trackplot-0.3.8/PKG-INFO
```

### Comparing `trackplot-0.3.7/LICENSE` & `trackplot-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/README.md` & `trackplot-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/pyproject.toml` & `trackplot-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.3.7"
+version = "0.3.8"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 include = [
     {path="pyproject.toml", format = ["sdist", "wheel"]},
```

### Comparing `trackplot-0.3.7/trackplot/anno/theme.py` & `trackplot-0.3.8/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/CoordinateMap.py` & `trackplot-0.3.8/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/GenomicLoci.py` & `trackplot-0.3.8/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/Junction.py` & `trackplot-0.3.8/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/Protein.py` & `trackplot-0.3.8/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/ReadDepth.py` & `trackplot-0.3.8/trackplot/base/ReadDepth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/Readder.py` & `trackplot-0.3.8/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/Stroke.py` & `trackplot-0.3.8/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/Transcript.py` & `trackplot-0.3.8/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/base/pyUniprot.py` & `trackplot-0.3.8/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/cli.py` & `trackplot-0.3.8/trackplot/cli.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/conf/DomainSetting.py` & `trackplot-0.3.8/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/conf/config.py` & `trackplot-0.3.8/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/conf/drawing.py` & `trackplot-0.3.8/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/conf/ui.py` & `trackplot-0.3.8/trackplot/conf/ui.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/ATAC.py` & `trackplot-0.3.8/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Annotation.py` & `trackplot-0.3.8/trackplot/file/Annotation.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Bam.py` & `trackplot-0.3.8/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/BedGraph.py` & `trackplot-0.3.8/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Bigwig.py` & `trackplot-0.3.8/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Depth.py` & `trackplot-0.3.8/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Fasta.py` & `trackplot-0.3.8/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/File.py` & `trackplot-0.3.8/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.3.8/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Junction.py` & `trackplot-0.3.8/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/Motif.py` & `trackplot-0.3.8/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/file/ReadSegments.py` & `trackplot-0.3.8/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/plot.py` & `trackplot-0.3.8/trackplot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from trackplot.plot_func import *
 
 logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
 faulthandler.enable()
 
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def __load__(args):
     p, args, kwargs = args
     p.load(*args, **kwargs)
@@ -1206,26 +1206,30 @@
             elif kwargs.get("same_y"):
                 max_y_val_, min_y_val_ = max(max_used_y_val.values()), min(min_used_y_val.values())
 
             logger.info(f"plotting {p.type} at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
             if p.type == "density":
                 if isinstance(p.obj[0], Depth):
                     for key, readDepth in p.obj[0].data.items():
+                        temp_params = self.params.get(p, {})
+
+                        if "y_label" not in temp_params:
+                            temp_params["y_label"] = key
+
                         plot_density(
                             ax=ax_var,
                             data=readDepth,
                             region=self.region,
                             graph_coords=self.graph_coords,
                             max_used_y_val=max_y_val_,
                             min_used_y_val=min_y_val_,
                             distance_between_label_axis=distance_between_label_axis,
                             raster=raster,
                             fill_step=fill_step,
-                            y_label=key,
-                            **self.params.get(p, {})
+                            **temp_params
                         )
                         curr_idx += 1
                         ax_var = plt.subplot(gs[curr_idx, 0])
                     curr_idx -= 1
                 else:
                     plot_density(
                         ax=ax_var,
```

### Comparing `trackplot-0.3.7/trackplot/plot_func.py` & `trackplot-0.3.8/trackplot/plot_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,16 +803,15 @@
                 )
 
                 # @2018.12.19 transparent background
                 t.set_bbox(dict(alpha=0))
                 jxn_numbers.append(t)
 
         try:
-            adjust_text(jxn_numbers, force_text=0.2, arrowprops=dict(arrowstyle="-", color='black', lw=1),
-                        autoalign="y")
+            adjust_text(jxn_numbers, force_text=(0.2, 0.2), arrowprops=dict(arrowstyle="-", color='black', lw=1))
         except IndexError as err:
             logger.debug(err)
 
     if obj and obj.title:
         ax.text(max(graph_coords) - len(obj.title), max_used_y_val, obj.title, color=color, fontsize=font_size)
 
     # update the y-axis actually used
@@ -1362,14 +1361,17 @@
         colors = {x: y for x, y in zip(["A", "T", "C", "G"], colors)}
 
     region = obj.region
     if graph_coords is None:
         graph_coords = init_graph_coords(region)
 
     # 在原始坐标轴上画motif
+    if not data:
+        logger.info("there is no any motif information to plot")
+        return
     ymin, ymax, xmin, xmax = 0, 0, \
                              graph_coords[min(data.keys()) - region.start], \
                              graph_coords[max(data.keys()) - region.start] + (1 + width) / 2
 
     # 在放大区画motif
     axin_width = width_per_character * (xmax - xmin) / len(graph_coords)
     bbox_to_left = (xmax * 2 - xmin) / len(graph_coords)
```

### Comparing `trackplot-0.3.7/trackplot/plot_tests.py` & `trackplot-0.3.8/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/trackplot/server.py` & `trackplot-0.3.8/trackplot/server.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.3.7/PKG-INFO` & `trackplot-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.3.7
+Version: 0.3.8
 Summary: The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/
 License: BSD-3
 Author: ygidtu
 Author-email: ygidtu@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

