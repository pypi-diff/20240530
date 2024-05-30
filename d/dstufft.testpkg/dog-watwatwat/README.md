# Comparing `tmp/dstufft.testpkg-dog.tar.gz` & `tmp/dstufft.testpkg-watwatwat.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dstufft.testpkg-dog.tar", last modified: Fri Sep  5 02:11:47 2014, max compression
+gzip compressed data, was "dist/dstufft.testpkg-watwatwat.tar", last modified: Fri Sep  5 02:27:53 2014, max compression
```

## Comparing `dstufft.testpkg-dog.tar` & `dstufft.testpkg-watwatwat.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/dstufft.testpkg.egg-info/
--rw-r--r--   0 dstufft    (501) staff       (20)        1 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/dstufft.testpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dstufft    (501) staff       (20)      187 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/dstufft.testpkg.egg-info/PKG-INFO
--rw-r--r--   0 dstufft    (501) staff       (20)      164 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/dstufft.testpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dstufft    (501) staff       (20)        1 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/dstufft.testpkg.egg-info/top_level.txt
--rw-r--r--   0 dstufft    (501) staff       (20)      187 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/PKG-INFO
--rw-r--r--   0 dstufft    (501) staff       (20)       59 2014-09-05 02:11:47.000000 dstufft.testpkg-dog/setup.cfg
--rw-r--r--   0 dstufft    (501) staff       (20)       75 2014-09-05 02:08:15.000000 dstufft.testpkg-dog/setup.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2014-09-05 02:27:53.000000 dstufft.testpkg-watwatwat/
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2014-09-05 02:27:53.000000 dstufft.testpkg-watwatwat/dstufft.testpkg.egg-info/
+-rw-r--r--   0 dstufft    (501) staff       (20)        1 2014-09-05 02:27:52.000000 dstufft.testpkg-watwatwat/dstufft.testpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)      193 2014-09-05 02:27:52.000000 dstufft.testpkg-watwatwat/dstufft.testpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dstufft    (501) staff       (20)      164 2014-09-05 02:27:53.000000 dstufft.testpkg-watwatwat/dstufft.testpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)        1 2014-09-05 02:27:52.000000 dstufft.testpkg-watwatwat/dstufft.testpkg.egg-info/top_level.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)      193 2014-09-05 02:27:53.000000 dstufft.testpkg-watwatwat/PKG-INFO
+-rw-r--r--   0 dstufft    (501) staff       (20)       59 2014-09-05 02:27:53.000000 dstufft.testpkg-watwatwat/setup.cfg
+-rw-r--r--   0 dstufft    (501) staff       (20)       81 2014-09-05 02:27:48.000000 dstufft.testpkg-watwatwat/setup.py
```

