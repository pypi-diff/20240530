# Comparing `tmp/package-tea-two-1.0.0.tar.gz` & `tmp/package-tea-two-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/package-tea-two-1.0.0.tar", last modified: Mon Mar  4 03:16:51 2024, max compression
+gzip compressed data, was "dist/package-tea-two-1.0.1.tar", last modified: Thu May 30 02:30:07 2024, max compression
```

## Comparing `package-tea-two-1.0.0.tar` & `package-tea-two-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:16:51.904053 package-tea-two-1.0.0/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1138 2024-03-04 03:16:51.903450 package-tea-two-1.0.0/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      155 2024-03-04 03:06:01.000000 package-tea-two-1.0.0/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:16:51.900160 package-tea-two-1.0.0/package-tea-two/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      126 2024-03-04 03:06:01.000000 package-tea-two-1.0.0/package-tea-two/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)      505 2024-03-04 03:06:01.000000 package-tea-two-1.0.0/package-tea-two/main.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:16:51.902833 package-tea-two-1.0.0/package_tea_two.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1138 2024-03-04 03:16:51.000000 package-tea-two-1.0.0/package_tea_two.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      265 2024-03-04 03:16:51.000000 package-tea-two-1.0.0/package_tea_two.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 03:16:51.000000 package-tea-two-1.0.0/package_tea_two.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       49 2024-03-04 03:16:51.000000 package-tea-two-1.0.0/package_tea_two.egg-info/requires.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       16 2024-03-04 03:16:51.000000 package-tea-two-1.0.0/package_tea_two.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 03:16:51.904166 package-tea-two-1.0.0/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1455 2024-03-04 03:14:55.000000 package-tea-two-1.0.0/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1169 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      148 2024-05-30 02:28:36.000000 package-tea-two-1.0.1/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package-tea-two/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      126 2024-05-30 02:27:20.000000 package-tea-two-1.0.1/package-tea-two/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)      487 2024-05-30 02:28:36.000000 package-tea-two-1.0.1/package-tea-two/main.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1169 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      265 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       49 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       16 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/package_tea_two.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-05-30 02:30:07.000000 package-tea-two-1.0.1/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1455 2024-05-30 02:28:36.000000 package-tea-two-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `package-tea-two-1.0.0/setup.py` & `package-tea-two-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='package-tea-two',  # 包名
-      version='1.0.0',  # 版本号
+      version='1.0.1',  # 版本号
       description='small package just example',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/package-tea-two.git',
       install_requires=["package-tea-one==1.0.0", "restful-dnspod-log==1.0.1"],
       project_urls={  # Optional
```

