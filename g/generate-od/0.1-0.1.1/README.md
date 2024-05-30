# Comparing `tmp/generate_od-0.1.tar.gz` & `tmp/generate-od-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_od-0.1.tar", last modified: Fri May 10 07:58:46 2024, max compression
+gzip compressed data, was "generate-od-0.1.1.tar", last modified: Thu May 30 03:00:23 2024, max compression
```

## Comparing `generate_od-0.1.tar` & `generate-od-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 07:58:46.864597 generate_od-0.1/
--rw-rw-rw-   0        0        0     1085 2024-04-26 08:21:28.000000 generate_od-0.1/LICENSE
--rw-rw-rw-   0        0        0     1080 2024-05-10 07:58:46.864597 generate_od-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-26 08:37:14.000000 generate_od-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 07:58:46.858595 generate_od-0.1/generate_od/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:45:14.000000 generate_od-0.1/generate_od/__init__.py
--rw-rw-rw-   0        0        0     9835 2024-05-10 04:04:27.000000 generate_od-0.1/generate_od/generator.py
--rw-rw-rw-   0        0        0    30182 2024-05-07 03:24:01.000000 generate_od-0.1/generate_od/model.py
--rw-rw-rw-   0        0        0    12858 2024-05-10 04:03:59.000000 generate_od-0.1/generate_od/sateimgs.py
--rw-rw-rw-   0        0        0    10036 2024-05-08 03:32:36.000000 generate_od-0.1/generate_od/utils.py
--rw-rw-rw-   0        0        0     3537 2024-05-10 07:31:02.000000 generate_od-0.1/generate_od/worldpop.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:58:46.863600 generate_od-0.1/generate_od.egg-info/
--rw-rw-rw-   0        0        0     1080 2024-05-10 07:58:46.000000 generate_od-0.1/generate_od.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-05-10 07:58:46.000000 generate_od-0.1/generate_od.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 07:58:46.000000 generate_od-0.1/generate_od.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-10 07:58:46.000000 generate_od-0.1/generate_od.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-10 07:58:46.000000 generate_od-0.1/generate_od.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 07:58:46.864597 generate_od-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-10 07:58:20.000000 generate_od-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:00:23.000900 generate-od-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-04-26 08:21:28.000000 generate-od-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      756 2024-05-30 03:00:23.000900 generate-od-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:37:14.000000 generate-od-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 03:00:22.982901 generate-od-0.1.1/generate_od/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:45:14.000000 generate-od-0.1.1/generate_od/__init__.py
+-rw-rw-rw-   0        0        0     9835 2024-05-10 04:04:27.000000 generate-od-0.1.1/generate_od/generator.py
+-rw-rw-rw-   0        0        0    30182 2024-05-07 03:24:01.000000 generate-od-0.1.1/generate_od/model.py
+-rw-rw-rw-   0        0        0    12858 2024-05-10 04:03:59.000000 generate-od-0.1.1/generate_od/sateimgs.py
+-rw-rw-rw-   0        0        0    10036 2024-05-08 03:32:36.000000 generate-od-0.1.1/generate_od/utils.py
+-rw-rw-rw-   0        0        0     3537 2024-05-10 07:31:02.000000 generate-od-0.1.1/generate_od/worldpop.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:00:23.000900 generate-od-0.1.1/generate_od.egg-info/
+-rw-rw-rw-   0        0        0      756 2024-05-30 03:00:22.000000 generate-od-0.1.1/generate_od.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-30 03:00:22.000000 generate-od-0.1.1/generate_od.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 03:00:22.000000 generate-od-0.1.1/generate_od.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-05-30 03:00:22.000000 generate-od-0.1.1/generate_od.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 03:00:22.000000 generate-od-0.1.1/generate_od.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 03:00:23.002375 generate-od-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2024-05-30 03:00:02.000000 generate-od-0.1.1/setup.py
```

### Comparing `generate_od-0.1/LICENSE` & `generate-od-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/generate_od/generator.py` & `generate-od-0.1.1/generate_od/generator.py`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/generate_od/model.py` & `generate-od-0.1.1/generate_od/model.py`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/generate_od/sateimgs.py` & `generate-od-0.1.1/generate_od/sateimgs.py`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/generate_od/utils.py` & `generate-od-0.1.1/generate_od/utils.py`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/generate_od/worldpop.py` & `generate-od-0.1.1/generate_od/worldpop.py`

 * *Files identical despite different names*

### Comparing `generate_od-0.1/setup.py` & `generate-od-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="generate-od",
-    version="0.1",
+    version="0.1.1",
     author="Can Rong",
     author_email="276413973@qq.com",
     description="A tool to generate origin-destination matrix for any given area.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tsinghua-fib-lab/generate-od-pubtools",
     packages=setuptools.find_packages(),
@@ -33,14 +33,14 @@
         'open-clip-torch>=2.23.0',
         'huggingface-hub',
         'numpy',
         'torch>=2.1.0',
         'Pillow',
         'scipy',
         'shapely',
-        'scikit-learn',
+        'scikit-learn==1.3.0',
         'contextily',
         'matplotlib',
         'rasterio'
     ],
     python_requires='>=3.8',
 )
```

