# Comparing `tmp/pgc-finder-0.0.2.tar.gz` & `tmp/pgc-finder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgc-finder-0.0.2.tar", last modified: Thu May 30 03:46:02 2024, max compression
+gzip compressed data, was "pgc-finder-0.0.3.tar", last modified: Thu May 30 05:01:21 2024, max compression
```

## Comparing `pgc-finder-0.0.2.tar` & `pgc-finder-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 03:46:02.727128 pgc-finder-0.0.2/
--rw-r--r--   0 jrim       (501) staff       (20)      576 2024-05-30 03:46:02.726879 pgc-finder-0.0.2/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)     1831 2024-05-29 17:13:50.000000 pgc-finder-0.0.2/README.md
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 03:46:02.725710 pgc-finder-0.0.2/pgc_finder/
--rw-r--r--   0 jrim       (501) staff       (20)      426 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    13289 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10046 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)     8060 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4297 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     6190 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6514 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     6511 2024-05-29 17:13:40.000000 pgc-finder-0.0.2/pgc_finder/main.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 03:46:02.726672 pgc-finder-0.0.2/pgc_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      576 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      508 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)       27 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)       11 2024-05-30 03:46:02.000000 pgc-finder-0.0.2/pgc_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-30 03:46:02.727195 pgc-finder-0.0.2/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      814 2024-05-30 03:45:55.000000 pgc-finder-0.0.2/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 05:01:21.822585 pgc-finder-0.0.3/
+-rw-r--r--   0 jrim       (501) staff       (20)      621 2024-05-30 05:01:21.822299 pgc-finder-0.0.3/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)     1831 2024-05-29 17:13:50.000000 pgc-finder-0.0.3/README.md
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 05:01:21.820706 pgc-finder-0.0.3/pgc_finder/
+-rw-r--r--   0 jrim       (501) staff       (20)      426 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    13289 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10046 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     8060 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4297 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6190 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6514 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)      509 2024-05-30 04:58:50.000000 pgc-finder-0.0.3/pgc_finder/cli.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6511 2024-05-29 17:13:40.000000 pgc-finder-0.0.3/pgc_finder/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 05:01:21.822038 pgc-finder-0.0.3/pgc_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      621 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      563 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       51 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/entry_points.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)       27 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       11 2024-05-30 05:01:21.000000 pgc-finder-0.0.3/pgc_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-30 05:01:21.822650 pgc-finder-0.0.3/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      950 2024-05-30 05:00:06.000000 pgc-finder-0.0.3/setup.py
```

### Comparing `pgc-finder-0.0.2/README.md` & `pgc-finder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_accessory.py` & `pgc-finder-0.0.3/pgc_finder/_accessory.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_blast.py` & `pgc-finder-0.0.3/pgc_finder/_blast.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_cluster.py` & `pgc-finder-0.0.3/pgc_finder/_cluster.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_count.py` & `pgc-finder-0.0.3/pgc_finder/_count.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_parse.py` & `pgc-finder-0.0.3/pgc_finder/_parse.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_profile.py` & `pgc-finder-0.0.3/pgc_finder/_profile.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_search.py` & `pgc-finder-0.0.3/pgc_finder/_search.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_seqlib.py` & `pgc-finder-0.0.3/pgc_finder/_seqlib.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_target.py` & `pgc-finder-0.0.3/pgc_finder/_target.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_utils.py` & `pgc-finder-0.0.3/pgc_finder/_utils.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/_visualize.py` & `pgc-finder-0.0.3/pgc_finder/_visualize.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/pgc_finder/main.py` & `pgc-finder-0.0.3/pgc_finder/main.py`

 * *Files identical despite different names*

### Comparing `pgc-finder-0.0.2/setup.py` & `pgc-finder-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pgc-finder',
-    version='0.0.2',
+    version='0.0.3',
     description='Python package for probe-based gene cluster finding in large microbial genome database',
     author='jsrim',
     author_email='comfortindex@naver.com',
-    url='https://github.com/jrim42/gene-cluster',
+    url='https://github.com/jrim42/pgc-finder',
     install_requires=['pandas', 'matplotlib', 'requests'],
     packages=find_packages(),
-    keywords=[],
+    keywords=['gene', 'cluster', 'genomics', 'bioinformatics'],
     python_requires='>=3.6',
-    package_data={},
+    entry_points={
+        'console_scripts': [
+            'pgc-finder=pgc_finder.cli:main',
+        ],
+    },
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

