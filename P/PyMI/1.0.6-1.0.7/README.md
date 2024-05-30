# Comparing `tmp/PyMI-1.0.6.tar.gz` & `tmp/PyMI-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyMI-1.0.6.tar", last modified: Mon May 25 12:21:00 2020, max compression
+gzip compressed data, was "PyMI-1.0.7.tar", last modified: Thu May 30 12:38:52 2024, max compression
```

## Comparing `PyMI-1.0.6.tar` & `PyMI-1.0.7.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.620130 PyMI-1.0.6/
--rw-rw-rw-   0        0        0       14 2020-05-20 11:59:25.000000 PyMI-1.0.6/.gitattributes
--rw-rw-rw-   0        0        0      239 2020-05-25 12:20:59.000000 PyMI-1.0.6/AUTHORS
--rw-rw-rw-   0        0        0     7632 2020-05-25 12:20:59.000000 PyMI-1.0.6/ChangeLog
--rw-rw-rw-   0        0        0    10143 2020-05-20 11:59:25.000000 PyMI-1.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.404128 PyMI-1.0.6/MI/
--rw-rw-rw-   0        0        0    41018 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MI++.cpp
--rw-rw-rw-   0        0        0    13244 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MI++.h
--rw-rw-rw-   0        0        0    29397 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MI.vcxproj
--rw-rw-rw-   0        0        0     1753 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MI.vcxproj.filters
--rw-rw-rw-   0        0        0     2028 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MIExceptions.cpp
--rw-rw-rw-   0        0        0     1588 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MIExceptions.h
--rw-rw-rw-   0        0        0     6853 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MIValue.cpp
--rw-rw-rw-   0        0        0     2070 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/MIValue.h
--rw-rw-rw-   0        0        0      281 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/PythonDir.props
--rw-rw-rw-   0        0        0     1564 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/ReadMe.txt
--rw-rw-rw-   0        0        0      281 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/stdafx.cpp
--rw-rw-rw-   0        0        0      397 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/stdafx.h
--rw-rw-rw-   0        0        0      306 2020-05-20 11:59:25.000000 PyMI-1.0.6/MI/targetver.h
--rw-rw-rw-   0        0        0     8256 2020-05-25 12:21:00.620130 PyMI-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.525130 PyMI-1.0.6/PyMI/
--rw-rw-rw-   0        0        0     9808 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Application.cpp
--rw-rw-rw-   0        0        0      266 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Application.h
--rw-rw-rw-   0        0        0     2119 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Callbacks.cpp
--rw-rw-rw-   0        0        0      682 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Callbacks.h
--rw-rw-rw-   0        0        0     5795 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Class.cpp
--rw-rw-rw-   0        0        0      307 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Class.h
--rw-rw-rw-   0        0        0     8711 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/DestinationOptions.cpp
--rw-rw-rw-   0        0        0      408 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/DestinationOptions.h
--rw-rw-rw-   0        0        0     8732 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Instance.cpp
--rw-rw-rw-   0        0        0      327 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Instance.h
--rw-rw-rw-   0        0        0      754 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/MiError.cpp
--rw-rw-rw-   0        0        0      335 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/MiError.h
--rw-rw-rw-   0        0        0     6330 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Operation.cpp
--rw-rw-rw-   0        0        0      335 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Operation.h
--rw-rw-rw-   0        0        0     6026 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/OperationOptions.cpp
--rw-rw-rw-   0        0        0      392 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/OperationOptions.h
--rw-rw-rw-   0        0        0     8422 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/PyMI.cpp
--rw-rw-rw-   0        0        0       98 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/PyMI.h
--rw-rw-rw-   0        0        0    50059 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/PyMI.vcxproj
--rw-rw-rw-   0        0        0     3733 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/PyMI.vcxproj.filters
--rw-rw-rw-   0        0        0     2109 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/PythonDir.props
--rw-rw-rw-   0        0        0     5501 2020-05-25 12:11:25.000000 PyMI-1.0.6/PyMI/README.rst
--rw-rw-rw-   0        0        0     5563 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Serializer.cpp
--rw-rw-rw-   0        0        0      343 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Serializer.h
--rw-rw-rw-   0        0        0    16442 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Session.cpp
--rw-rw-rw-   0        0        0      422 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Session.h
--rw-rw-rw-   0        0        0    15615 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Utils.cpp
--rw-rw-rw-   0        0        0      940 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/Utils.h
--rw-rw-rw-   0        0        0     1600 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/setup_vs.py
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.265136 PyMI-1.0.6/PyMI/src/
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.594134 PyMI-1.0.6/PyMI/src/mi/
--rw-rw-rw-   0        0        0       28 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/src/mi/__init__.py
--rw-rw-rw-   0        0        0      302 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/stdafx.cpp
--rw-rw-rw-   0        0        0      989 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/stdafx.h
--rw-rw-rw-   0        0        0      306 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI/targetver.h
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.586134 PyMI-1.0.6/PyMI.egg-info/
--rw-rw-rw-   0        0        0     8256 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-05-20 12:12:42.000000 PyMI-1.0.6/PyMI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/pbr.json
--rw-rw-rw-   0        0        0       31 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-05-25 12:20:59.000000 PyMI-1.0.6/PyMI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8100 2020-05-20 11:59:25.000000 PyMI-1.0.6/PyMI.sln
--rw-rw-rw-   0        0        0      255 2020-05-20 11:59:25.000000 PyMI-1.0.6/README.rst
--rw-rw-rw-   0        0        0       50 2020-05-20 11:59:25.000000 PyMI-1.0.6/requirements.txt
--rw-rw-rw-   0        0        0     1006 2020-05-25 12:21:00.623136 PyMI-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2462 2020-05-25 12:11:25.000000 PyMI-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.598165 PyMI-1.0.6/wmi/
--rw-rw-rw-   0        0        0    32275 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/__init__.py
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.606164 PyMI-1.0.6/wmi/samples/
--rw-rw-rw-   0        0        0      767 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/samples/benchmark.py
--rw-rw-rw-   0        0        0     3874 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/samples/benchmark2.py
--rw-rw-rw-   0        0        0     2492 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/samples/benchmark3.py
--rw-rw-rw-   0        0        0      708 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/samples/custom_operation_options.py
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.609161 PyMI-1.0.6/wmi/tests/
--rw-rw-rw-   0        0        0        0 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2020-05-25 12:21:00.617132 PyMI-1.0.6/wmi/tests/functional/
--rw-rw-rw-   0        0        0        0 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/tests/functional/__init__.py
--rw-rw-rw-   0        0        0     1511 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/tests/functional/test_base.py
--rw-rw-rw-   0        0        0     2282 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/tests/functional/test_basic_ops.py
--rw-rw-rw-   0        0        0     2633 2020-05-20 11:59:25.000000 PyMI-1.0.6/wmi/tests/functional/test_timeouts.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.422917 PyMI-1.0.7/
+-rw-rw-rw-   0        0        0       14 2023-11-03 13:15:41.000000 PyMI-1.0.7/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:51.899183 PyMI-1.0.7/.github/
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:51.962849 PyMI-1.0.7/.github/workflows/
+-rw-rw-rw-   0        0        0      846 2023-11-03 13:18:35.000000 PyMI-1.0.7/.github/workflows/pymi-cd.yml
+-rw-rw-rw-   0        0        0      317 2024-05-30 12:38:51.000000 PyMI-1.0.7/AUTHORS
+-rw-rw-rw-   0        0        0     7800 2024-05-30 12:38:51.000000 PyMI-1.0.7/ChangeLog
+-rw-rw-rw-   0        0        0    10143 2023-11-03 13:15:41.000000 PyMI-1.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.063533 PyMI-1.0.7/MI/
+-rw-rw-rw-   0        0        0    41024 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MI++.cpp
+-rw-rw-rw-   0        0        0    13244 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MI++.h
+-rw-rw-rw-   0        0        0    29397 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MI.vcxproj
+-rw-rw-rw-   0        0        0     1753 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MI.vcxproj.filters
+-rw-rw-rw-   0        0        0     2028 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MIExceptions.cpp
+-rw-rw-rw-   0        0        0     1588 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MIExceptions.h
+-rw-rw-rw-   0        0        0     6853 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MIValue.cpp
+-rw-rw-rw-   0        0        0     2070 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/MIValue.h
+-rw-rw-rw-   0        0        0      281 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/PythonDir.props
+-rw-rw-rw-   0        0        0     1564 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/ReadMe.txt
+-rw-rw-rw-   0        0        0      281 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/stdafx.cpp
+-rw-rw-rw-   0        0        0      397 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/stdafx.h
+-rw-rw-rw-   0        0        0      335 2023-11-03 13:15:41.000000 PyMI-1.0.7/MI/targetver.h
+-rw-rw-rw-   0        0        0     7031 2024-05-30 12:38:52.422917 PyMI-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.282198 PyMI-1.0.7/PyMI/
+-rw-rw-rw-   0        0        0     9901 2024-05-30 12:37:25.000000 PyMI-1.0.7/PyMI/Application.cpp
+-rw-rw-rw-   0        0        0      266 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Application.h
+-rw-rw-rw-   0        0        0     2119 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Callbacks.cpp
+-rw-rw-rw-   0        0        0      682 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Callbacks.h
+-rw-rw-rw-   0        0        0     5792 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Class.cpp
+-rw-rw-rw-   0        0        0      307 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Class.h
+-rw-rw-rw-   0        0        0     8880 2024-05-30 12:37:25.000000 PyMI-1.0.7/PyMI/DestinationOptions.cpp
+-rw-rw-rw-   0        0        0      408 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/DestinationOptions.h
+-rw-rw-rw-   0        0        0     8729 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Instance.cpp
+-rw-rw-rw-   0        0        0      327 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Instance.h
+-rw-rw-rw-   0        0        0      754 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/MiError.cpp
+-rw-rw-rw-   0        0        0      335 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/MiError.h
+-rw-rw-rw-   0        0        0     6330 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Operation.cpp
+-rw-rw-rw-   0        0        0      335 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Operation.h
+-rw-rw-rw-   0        0        0     6042 2024-05-30 12:37:25.000000 PyMI-1.0.7/PyMI/OperationOptions.cpp
+-rw-rw-rw-   0        0        0      392 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/OperationOptions.h
+-rw-rw-rw-   0        0        0     8422 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/PyMI.cpp
+-rw-rw-rw-   0        0        0       98 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/PyMI.h
+-rw-rw-rw-   0        0        0    50059 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/PyMI.vcxproj
+-rw-rw-rw-   0        0        0     3733 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/PyMI.vcxproj.filters
+-rw-rw-rw-   0        0        0     2109 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/PythonDir.props
+-rw-rw-rw-   0        0        0     5501 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/README.rst
+-rw-rw-rw-   0        0        0     5563 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Serializer.cpp
+-rw-rw-rw-   0        0        0      343 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Serializer.h
+-rw-rw-rw-   0        0        0    16743 2024-05-30 12:37:25.000000 PyMI-1.0.7/PyMI/Session.cpp
+-rw-rw-rw-   0        0        0      422 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/Session.h
+-rw-rw-rw-   0        0        0    16426 2024-05-30 12:37:25.000000 PyMI-1.0.7/PyMI/Utils.cpp
+-rw-rw-rw-   0        0        0      992 2023-11-03 15:00:25.000000 PyMI-1.0.7/PyMI/Utils.h
+-rw-rw-rw-   0        0        0     1600 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/setup_vs.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:51.899183 PyMI-1.0.7/PyMI/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.343773 PyMI-1.0.7/PyMI/src/mi/
+-rw-rw-rw-   0        0        0       28 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/src/mi/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/stdafx.cpp
+-rw-rw-rw-   0        0        0      989 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/stdafx.h
+-rw-rw-rw-   0        0        0      335 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI/targetver.h
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.328093 PyMI-1.0.7/PyMI.egg-info/
+-rw-rw-rw-   0        0        0     7031 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/pbr.json
+-rw-rw-rw-   0        0        0       31 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:38:51.000000 PyMI-1.0.7/PyMI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8100 2023-11-03 13:15:41.000000 PyMI-1.0.7/PyMI.sln
+-rw-rw-rw-   0        0        0      255 2023-11-03 13:15:41.000000 PyMI-1.0.7/README.rst
+-rw-rw-rw-   0        0        0       50 2023-11-03 13:15:41.000000 PyMI-1.0.7/requirements.txt
+-rw-rw-rw-   0        0        0     1209 2024-05-30 12:38:52.422917 PyMI-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2502 2023-11-03 13:15:41.000000 PyMI-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.344816 PyMI-1.0.7/wmi/
+-rw-rw-rw-   0        0        0    32275 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.391655 PyMI-1.0.7/wmi/samples/
+-rw-rw-rw-   0        0        0      767 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/samples/benchmark.py
+-rw-rw-rw-   0        0        0     3874 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/samples/benchmark2.py
+-rw-rw-rw-   0        0        0     2492 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/samples/benchmark3.py
+-rw-rw-rw-   0        0        0      708 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/samples/custom_operation_options.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.391655 PyMI-1.0.7/wmi/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:38:52.422917 PyMI-1.0.7/wmi/tests/functional/
+-rw-rw-rw-   0        0        0        0 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/tests/functional/__init__.py
+-rw-rw-rw-   0        0        0     1511 2023-11-03 13:15:41.000000 PyMI-1.0.7/wmi/tests/functional/test_base.py
+-rw-rw-rw-   0        0        0     2528 2023-11-03 13:18:35.000000 PyMI-1.0.7/wmi/tests/functional/test_basic_ops.py
+-rw-rw-rw-   0        0        0     2760 2023-11-03 13:18:35.000000 PyMI-1.0.7/wmi/tests/functional/test_timeouts.py
```

### Comparing `PyMI-1.0.6/ChangeLog` & `PyMI-1.0.7/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+1.0.7
+-----
+
+* Add py 3.12 unicode fixes
+* Add support for Python up to 3.12
+* Fix building with mingw-w64
+* Added github workflow to test/build/publish wheel
+
 1.0.6
 -----
 
 * Statically link the VC runtime
 
 1.0.5
 -----
```

### Comparing `PyMI-1.0.6/LICENSE` & `PyMI-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MI++.cpp` & `PyMI-1.0.7/MI/MI++.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     if (result != MI_RESULT_OK)
     {
         if (extError)
         {
             Instance instance((MI_Instance*)extError, false);
             if(IsInstanceOf(instance, L"MSFT_WmiError"))
             {
-                MI_Char* message = instance[L"Message"]->m_value.string;
+                const MI_Char* message = instance[L"Message"]->m_value.string;
                 message = message ? message : L"";
 
                 auto errorCode = instance[L"error_code"]->m_value.uint32;
 
                 switch(errorCode)
                 {
                 case WMI_ERR_TIMEOUT:
```

### Comparing `PyMI-1.0.6/MI/MI++.h` & `PyMI-1.0.7/MI/MI++.h`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MI.vcxproj` & `PyMI-1.0.7/MI/MI.vcxproj`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MI.vcxproj.filters` & `PyMI-1.0.7/MI/MI.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MIExceptions.cpp` & `PyMI-1.0.7/MI/MIExceptions.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MIExceptions.h` & `PyMI-1.0.7/MI/MIExceptions.h`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MIValue.cpp` & `PyMI-1.0.7/MI/MIValue.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/MIValue.h` & `PyMI-1.0.7/MI/MIValue.h`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/MI/ReadMe.txt` & `PyMI-1.0.7/MI/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PKG-INFO` & `PyMI-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,209 +1,213 @@
 Metadata-Version: 2.1
 Name: PyMI
-Version: 1.0.6
+Version: 1.0.7
 Summary: Windows Management Infrastructure API for Python.
 Home-page: https://github.com/cloudbase/PyMI
 Author: Alessandro Pilotti
 Author-email: info@cloudbasesolutions.com
-License: UNKNOWN
-Description: PyMI - Windows Management Infrastructure API for Python
-        =======================================================
-        
-        This project provides a Python native module wrapper over the Windows
-        Management Infrastructure (MI) API [#miapi]_.
-        
-        Works with Python 2.7 and 3.x on any Windows version which supports the MI API,
-        both x86 and x64.
-        
-        It includes also a drop-in replacement for the Python WMI [#pywmi]_ module,
-        proving much faster execution times and no dependency on pywin32.
-        
-        Installation
-        ------------
-        
-        Pip is the preferred way to install PyMI. Pre-compiled binary wheels are
-        available on Pypi [#pymipypi]_:
-        
-        .. code-block:: powershell
-        
-            pip install PyMI
-        
-        Usage
-        -----
-        
-        This project can be used either with a lower level interface that reflects the
-        underlying MI API structure or with the higher level (and slightly slower)
-        WMI module replacement.
-        
-        MI module basic usage
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        Here's a simple example which enumerates all processes and kills any instance of
-        "KillerRabbitOfCaerbannog.exe".
-        
-        .. code-block:: python
-        
-            import mi
-        
-            with mi.Application() as a:
-                with a.create_session(protocol=mi.PROTOCOL_WMIDCOM) as s:
-                    proc_name = u'notepad.exe'
-                    with s.exec_query(
-                            u"root\\cimv2", u"select * from Win32_Process") as q:
-                        i = q.get_next_instance()
-                        while i is not None:
-                            if i[u'name'].lower() == u"KillerRabbitOfCaerbannog.exe":
-                                cls = i.get_class()
-                                # Prepare parameters
-                                params = a.create_method_params(cls, u"Terminate")
-                                # Exit code
-                                params['reason'] = 10
-                                # Invoke method
-                                with s.invoke_method(i, u"Terminate", params) as op:
-                                    op.get_next_instance()
-                            i = q.get_next_instance()
-        
-        WMI module basic usage
-        ^^^^^^^^^^^^^^^^^^^^^^
-        
-        And here's the same example written using the *WMI* module replacement,
-        which provides a simpler and higher level interface over the *mi* API:
-        
-        .. code-block:: python
-        
-            import wmi
-        
-            conn = wmi.WMI()
-            for p in conn.Win32_Process():
-                if p.Name == u"KillerRabbitOfCaerbannog.exe":
-                    p.Terminate(reason=10)
-        
-        
-        Build
-        -----
-        
-        Use the following to build Python 3 wheels. Those will be copied to the build
-        dir.
-        
-        .. code-block:: powershell
-        
-            python setup.py bdist_wheel
-        
-        The best way to build PyMI for Python 2.7 or 3.4 and below is to use the
-        Visual Studio solution (described below). This will statically link the
-        vc140 runtime, which is required by PyMI.
-        
-        Custom VS env vars
-        ^^^^^^^^^^^^^^^^^^
-        
-        distutils will automatically locate your Visual Studio and Windows SDK
-        installation. If you'd like to call vcvarsall.bat yourself and use a specific
-        version, use the following:
-        
-        .. code-block:: powershell
-        
-            function SetVCVars($vcvarsdir, $platform="amd64")
-            {
-                pushd $vcvarsdir
-                try
-                {
-                    cmd /c "vcvarsall.bat $platform & set" |
-                    foreach {
-                      if ($_ -match "=") {
-                        $v = $_.split("="); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
-                      }
-                    }
-                }
-                finally
-                {
-                    popd
-                }
-            }
-        
-            # Replace this folder with the one in which the vcvarsall.bat script is
-            # located (the exact location depends on the Visual Studio version).
-            # SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\VC\Auxiliary\Build"
-            SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC"
-        
-            $env:DISTUTILS_USE_SDK=1
-            $env:MSSdk=1
-        
-            python setup.py bdist_wheel
-        
-        Make sure to use the Visual Studio toolset that matches the Python version
-        that you're targetting: https://wiki.python.org/moin/WindowsCompilers.
-        
-        By default, we're statically linking the VC runtime. To enable dynamic
-        linking, set ``$env:PYMI_VCRUNTIME_DYNAMIC_LINKING="y"``.
-        
-        Debug builds
-        ^^^^^^^^^^^^
-        
-        The easiest way to do a debug build is to set the following in setup.cfg:
-        
-        .. code-block::
-        
-            [build]
-            debug = 1
-        
-        This will be honored regardless of the build type (e.g. stdist, wheel, etc).
-        
-        To enable distutils debug logging, you may set the following:
-        
-        .. code-block:: powershell
-        
-            $env:DISTUTILS_DEBUG = 1
-        
-        Before doing a debug build, you may wish to clean the build dir.
-        
-        Using the Visual Studio Solution
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Open the provided *PyMI.sln* solution in Visual Studio 2015 [#VS2015]_, choose
-        your target Python version / platform and build. Wheel packages are
-        automatically generated in the *dist* folder for release builds.
-        
-        Note: the target Python version must be present. The Python path can be
-        customized by setting the corresponding PythonDir* user macro,
-        e.g. *PythonDir_34_x64*. The *wheel* and *GitPython* packages are required during the build process:
-        
-        .. code-block:: powershell
-        
-            pip install wheel
-            pip install GitPython
-        
-        As an alternative, you can use the MSBuild CLI tool:
-        
-        .. code-block:: powershell
-        
-            $env:MSBuildEmitSolution="TRUE"
-            MSBuild.exe .\PyMI.sln /p:Configuration="Release (Python 3.7)"
-        
-        
-        References
-        ----------
-        
-        .. [#miapi] MI API https://msdn.microsoft.com/en-us/library/hh404805(v=vs.85).aspx
-        .. [#pywmi] Python WMI module https://pypi.python.org/pypi/WMI
-        .. [#pymipypi] PyMI on Pypi https://pypi.python.org/pypi/PyMI
-        .. [#vs2015] Visual Studio 2015 download https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx
-        
-        
 Keywords: wmi mi windows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Systems Administration
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+PyMI - Windows Management Infrastructure API for Python
+=======================================================
+
+This project provides a Python native module wrapper over the Windows
+Management Infrastructure (MI) API [#miapi]_.
+
+Works with Python 2.7 and 3.x on any Windows version which supports the MI API,
+both x86 and x64.
+
+It includes also a drop-in replacement for the Python WMI [#pywmi]_ module,
+proving much faster execution times and no dependency on pywin32.
+
+Installation
+------------
+
+Pip is the preferred way to install PyMI. Pre-compiled binary wheels are
+available on Pypi [#pymipypi]_:
+
+.. code-block:: powershell
+
+    pip install PyMI
+
+Usage
+-----
+
+This project can be used either with a lower level interface that reflects the
+underlying MI API structure or with the higher level (and slightly slower)
+WMI module replacement.
+
+MI module basic usage
+^^^^^^^^^^^^^^^^^^^^^
+
+Here's a simple example which enumerates all processes and kills any instance of
+"KillerRabbitOfCaerbannog.exe".
+
+.. code-block:: python
+
+    import mi
+
+    with mi.Application() as a:
+        with a.create_session(protocol=mi.PROTOCOL_WMIDCOM) as s:
+            proc_name = u'notepad.exe'
+            with s.exec_query(
+                    u"root\\cimv2", u"select * from Win32_Process") as q:
+                i = q.get_next_instance()
+                while i is not None:
+                    if i[u'name'].lower() == u"KillerRabbitOfCaerbannog.exe":
+                        cls = i.get_class()
+                        # Prepare parameters
+                        params = a.create_method_params(cls, u"Terminate")
+                        # Exit code
+                        params['reason'] = 10
+                        # Invoke method
+                        with s.invoke_method(i, u"Terminate", params) as op:
+                            op.get_next_instance()
+                    i = q.get_next_instance()
+
+WMI module basic usage
+^^^^^^^^^^^^^^^^^^^^^^
+
+And here's the same example written using the *WMI* module replacement,
+which provides a simpler and higher level interface over the *mi* API:
+
+.. code-block:: python
+
+    import wmi
+
+    conn = wmi.WMI()
+    for p in conn.Win32_Process():
+        if p.Name == u"KillerRabbitOfCaerbannog.exe":
+            p.Terminate(reason=10)
+
+
+Build
+-----
+
+Use the following to build Python 3 wheels. Those will be copied to the build
+dir.
+
+.. code-block:: powershell
+
+    python setup.py bdist_wheel
+
+The best way to build PyMI for Python 2.7 or 3.4 and below is to use the
+Visual Studio solution (described below). This will statically link the
+vc140 runtime, which is required by PyMI.
+
+Custom VS env vars
+^^^^^^^^^^^^^^^^^^
+
+distutils will automatically locate your Visual Studio and Windows SDK
+installation. If you'd like to call vcvarsall.bat yourself and use a specific
+version, use the following:
+
+.. code-block:: powershell
+
+    function SetVCVars($vcvarsdir, $platform="amd64")
+    {
+        pushd $vcvarsdir
+        try
+        {
+            cmd /c "vcvarsall.bat $platform & set" |
+            foreach {
+              if ($_ -match "=") {
+                $v = $_.split("="); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
+              }
+            }
+        }
+        finally
+        {
+            popd
+        }
+    }
+
+    # Replace this folder with the one in which the vcvarsall.bat script is
+    # located (the exact location depends on the Visual Studio version).
+    # SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\VC\Auxiliary\Build"
+    SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC"
+
+    $env:DISTUTILS_USE_SDK=1
+    $env:MSSdk=1
+
+    python setup.py bdist_wheel
+
+Make sure to use the Visual Studio toolset that matches the Python version
+that you're targetting: https://wiki.python.org/moin/WindowsCompilers.
+
+By default, we're statically linking the VC runtime. To enable dynamic
+linking, set ``$env:PYMI_VCRUNTIME_DYNAMIC_LINKING="y"``.
+
+Debug builds
+^^^^^^^^^^^^
+
+The easiest way to do a debug build is to set the following in setup.cfg:
+
+.. code-block::
+
+    [build]
+    debug = 1
+
+This will be honored regardless of the build type (e.g. stdist, wheel, etc).
+
+To enable distutils debug logging, you may set the following:
+
+.. code-block:: powershell
+
+    $env:DISTUTILS_DEBUG = 1
+
+Before doing a debug build, you may wish to clean the build dir.
+
+Using the Visual Studio Solution
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Open the provided *PyMI.sln* solution in Visual Studio 2015 [#VS2015]_, choose
+your target Python version / platform and build. Wheel packages are
+automatically generated in the *dist* folder for release builds.
+
+Note: the target Python version must be present. The Python path can be
+customized by setting the corresponding PythonDir* user macro,
+e.g. *PythonDir_34_x64*. The *wheel* and *GitPython* packages are required during the build process:
+
+.. code-block:: powershell
+
+    pip install wheel
+    pip install GitPython
+
+As an alternative, you can use the MSBuild CLI tool:
+
+.. code-block:: powershell
+
+    $env:MSBuildEmitSolution="TRUE"
+    MSBuild.exe .\PyMI.sln /p:Configuration="Release (Python 3.7)"
+
+
+References
+----------
+
+.. [#miapi] MI API https://msdn.microsoft.com/en-us/library/hh404805(v=vs.85).aspx
+.. [#pywmi] Python WMI module https://pypi.python.org/pypi/WMI
+.. [#pymipypi] PyMI on Pypi https://pypi.python.org/pypi/PyMI
+.. [#vs2015] Visual Studio 2015 download https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx
+
```

### Comparing `PyMI-1.0.6/PyMI/Application.cpp` & `PyMI-1.0.7/PyMI/Application.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -15,53 +15,53 @@
     self = (Application*)type->tp_alloc(type, 0);
     ::InitializeCriticalSection(&self->cs);
     return (PyObject *)self;
 }
 
 static int Application_init(Application *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* appId = L"";
+    char* appId = "";
     static char *kwlist[] = { "app_id", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "|u", kwlist, &appId))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "|s", kwlist, &appId))
         return -1;
 
     try
     {
         AllowThreads(&self->cs, [&]() {
-            self->app = std::make_shared<MI::Application>(appId);
+            self->app = std::make_shared<MI::Application>(ToWstring(appId).c_str());
         });
         return 0;
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return -1;
     }
 }
 
 static PyObject* Application_NewSession(Application *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* protocol = L"";
-    wchar_t* computerName = L".";
+    char* protocol = "";
+    char* computerName = ".";
     PyObject* destinationOptions = NULL;
 
     static char *kwlist[] = { "protocol", "computer_name", "destination_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "|uuO", kwlist, &protocol, &computerName, &destinationOptions))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "|ssO", kwlist, &protocol, &computerName, &destinationOptions))
         return NULL;
 
     try
     {
         if (!CheckPyNone(destinationOptions) && !PyObject_IsInstance(destinationOptions, reinterpret_cast<PyObject*>(&DestinationOptionsType)))
         {
             throw MI::TypeConversionException(L"\"destination_options\" must have type DestinationOptions");
         }
 
         std::shared_ptr<MI::Session> session;
         AllowThreads(&self->cs, [&]() {
-            session = self->app->NewSession(protocol, computerName,
+            session = self->app->NewSession(ToWstring(protocol).c_str(), ToWstring(computerName).c_str(),
                 !CheckPyNone(destinationOptions) ? ((DestinationOptions*)destinationOptions)->destinationOptions : NULL);
         });
         return (PyObject*)Session_New(session);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
@@ -80,76 +80,76 @@
     ::DeleteCriticalSection(&self->cs);
     Py_TYPE(self)->tp_free((PyObject*)self);
 }
 
 static PyObject* Application_NewMethodInboundParameters(Application *self, PyObject *args, PyObject *kwds)
 {
     PyObject* pyClass = NULL;
-    wchar_t* methodName = NULL;
+    char* methodName = NULL;
 
     static char *kwlist[] = { "mi_class", "method_name", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "Ou", kwlist, &pyClass, &methodName))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "Os", kwlist, &pyClass, &methodName))
         return NULL;
 
     try
     {
         if (!PyObject_IsInstance(pyClass, reinterpret_cast<PyObject*>(&ClassType)))
             throw MI::TypeConversionException(L"\"mi_class\" must have type Class");
 
         std::shared_ptr<MI::Instance> instance;
         AllowThreads(&self->cs, [&]() {
-            instance = self->app->NewMethodParamsInstance(*((Class*)pyClass)->miClass, methodName);
+            instance = self->app->NewMethodParamsInstance(*((Class*)pyClass)->miClass, ToWstring(methodName).c_str());
         });
         return (PyObject*)Instance_New(instance);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Application_NewInstance(Application *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* className = NULL;
+    char* className = NULL;
     static char *kwlist[] = { "class_name", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "u", kwlist, &className))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "s", kwlist, &className))
         return NULL;
 
     try
     {
         std::shared_ptr<MI::Instance> instance;
         AllowThreads(&self->cs, [&]() {
-            instance = self->app->NewInstance(className);
+            instance = self->app->NewInstance(ToWstring(className).c_str());
         });
         return (PyObject*)Instance_New(instance);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Application_NewInstanceFromClass(Application *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* className = NULL;
+    char* className = NULL;
     PyObject* miClass = NULL;
     static char *kwlist[] = { "class_name", "mi_class", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO", kwlist, &className, &miClass))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO", kwlist, &className, &miClass))
         return NULL;
 
     try
     {
         if (!PyObject_IsInstance(miClass, reinterpret_cast<PyObject*>(&ClassType)))
             throw MI::TypeConversionException(L"\"mi_class\" must have type Class");
 
         std::shared_ptr<MI::Instance> instance;
         AllowThreads(&self->cs, [&]() {
-            instance = self->app->NewInstanceFromClass(className, *((Class*)miClass)->miClass);
+            instance = self->app->NewInstanceFromClass(ToWstring(className).c_str(), *((Class*)miClass)->miClass);
         });
         return (PyObject*)Instance_New(instance);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
```

### Comparing `PyMI-1.0.6/PyMI/Callbacks.cpp` & `PyMI-1.0.7/PyMI/Callbacks.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/Callbacks.h` & `PyMI-1.0.7/PyMI/Callbacks.h`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/Class.cpp` & `PyMI-1.0.7/PyMI/Class.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -108,43 +108,43 @@
     }
 }
 
 static PyObject* Class_GetClassName(Class* self, PyObject*)
 {
     try
     {
-        std::wstring& className = self->miClass->GetClassName();
+        std::wstring className = self->miClass->GetClassName();
         return PyUnicode_FromWideChar(className.c_str(), className.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Class_GetNameSpace(Class* self, PyObject*)
 {
     try
     {
-        std::wstring& nameSpace = self->miClass->GetNameSpace();
+        std::wstring nameSpace = self->miClass->GetNameSpace();
         return PyUnicode_FromWideChar(nameSpace.c_str(), nameSpace.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Class_GetServerName(Class* self, PyObject*)
 {
     try
     {
-        std::wstring& serverName = self->miClass->GetServerName();
+        std::wstring serverName = self->miClass->GetServerName();
         return PyUnicode_FromWideChar(serverName.c_str(), serverName.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
```

### Comparing `PyMI-1.0.6/PyMI/DestinationOptions.cpp` & `PyMI-1.0.7/PyMI/DestinationOptions.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -71,23 +71,23 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* DestinationOptions_SetUILocale(DestinationOptions* self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* locale = NULL;
+    char* locale = NULL;
     static char *kwlist[] = { "locale_name", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "u", kwlist, &locale))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "s", kwlist, &locale))
         return NULL;
 
     try
     {
         AllowThreads(&self->cs, [&]() {
-            self->destinationOptions->SetUILocale(locale);
+            self->destinationOptions->SetUILocale(ToWstring(locale).c_str());
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
@@ -135,23 +135,23 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* DestinationOptions_SetTransport(DestinationOptions* self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* transport = NULL;
+    char* transport = NULL;
     static char *kwlist[] = { "transport", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "u", kwlist, &transport))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "s", kwlist, &transport))
         return NULL;
 
     try
     {
         AllowThreads(&self->cs, [&]() {
-            self->destinationOptions->SetTransport(transport);
+            self->destinationOptions->SetTransport(ToWstring(transport).c_str());
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
@@ -174,34 +174,34 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* DestinationOptions_AddCredentials(DestinationOptions* self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* authType = NULL;
-    wchar_t* domain = NULL;
-    wchar_t* username = NULL;
-    wchar_t* password = NULL;
-    wchar_t* certThumbprint = NULL;
+    char* authType = NULL;
+    char* domain = NULL;
+    char* username = NULL;
+    char* password = NULL;
+    char* certThumbprint = NULL;
 
     static char *kwlist[] = { "auth_type", "domain", "username", "password", "cert_thumbprint", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "u|uuuu", kwlist,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "s|ssss", kwlist,
                                      &authType, &domain, &username, &password, &certThumbprint))
         return NULL;
 
     try
     {
-        if (certThumbprint && wcslen(certThumbprint))
+        if (ToWstring(certThumbprint).c_str() && wcslen(ToWstring(certThumbprint).c_str()))
             AllowThreads(&self->cs, [&]() {
-                self->destinationOptions->AddCredentials(authType, certThumbprint);
+                self->destinationOptions->AddCredentials(ToWstring(authType).c_str(), ToWstring(certThumbprint).c_str());
             });
         else
             AllowThreads(&self->cs, [&]() {
-                self->destinationOptions->AddCredentials(authType, domain, username, password);
+                self->destinationOptions->AddCredentials(ToWstring(authType).c_str(), ToWstring(domain).c_str(), ToWstring(username).c_str(), ToWstring(password).c_str());
             });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
```

### Comparing `PyMI-1.0.6/PyMI/Instance.cpp` & `PyMI-1.0.7/PyMI/Instance.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -208,43 +208,43 @@
     }
 }
 
 static PyObject* Instance_GetClassName(Instance *self, PyObject*)
 {
     try
     {
-        std::wstring& className = self->instance->GetClassName();
+        std::wstring className = self->instance->GetClassName();
         return PyUnicode_FromWideChar(className.c_str(), className.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Instance_GetNameSpace(Instance* self, PyObject*)
 {
     try
     {
-        std::wstring& nameSpace = self->instance->GetNameSpace();
+        std::wstring nameSpace = self->instance->GetNameSpace();
         return PyUnicode_FromWideChar(nameSpace.c_str(), nameSpace.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Instance_GetServerName(Instance* self, PyObject*)
 {
     try
     {
-        std::wstring& serverName = self->instance->GetServerName();
+        std::wstring serverName = self->instance->GetServerName();
         return PyUnicode_FromWideChar(serverName.c_str(), serverName.length());
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
```

### Comparing `PyMI-1.0.6/PyMI/MiError.cpp` & `PyMI-1.0.7/PyMI/MiError.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/Operation.cpp` & `PyMI-1.0.7/PyMI/Operation.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/OperationOptions.cpp` & `PyMI-1.0.7/PyMI/OperationOptions.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -97,30 +97,30 @@
         return NULL;
     }
 }
 
 
 static PyObject* OperationOptions_SetCustomOption(OperationOptions* self,  PyObject *args, PyObject *kwds)
 {
-    wchar_t* optionName = NULL;
+    char* optionName = NULL;
     unsigned int optionValueType = 0;
     PyObject* optionValue = NULL;
     PyObject* mustComply = NULL;
 
     static char *kwlist[] = { "name", "value_type", "value", "must_comply", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uIO|O", kwlist,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sIO|O", kwlist,
                                      &optionName, &optionValueType,
                                      &optionValue, &mustComply))
         return NULL;
 
     try
     {
         auto miValue = Py2MI(optionValue, (MI_Type)optionValueType);
         AllowThreads(&self->cs, [&]() {
-            self->operationOptions->SetCustomOption(optionName, (MI_Type)optionValueType,
+            self->operationOptions->SetCustomOption(ToWstring(optionName).c_str(), (MI_Type)optionValueType,
                                                     *miValue, PyObject_IsTrue(mustComply));
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
```

### Comparing `PyMI-1.0.6/PyMI/PyMI.cpp` & `PyMI-1.0.7/PyMI/PyMI.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/PyMI.vcxproj` & `PyMI-1.0.7/PyMI/PyMI.vcxproj`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/PyMI.vcxproj.filters` & `PyMI-1.0.7/PyMI/PyMI.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/PythonDir.props` & `PyMI-1.0.7/PyMI/PythonDir.props`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/README.rst` & `PyMI-1.0.7/PyMI/README.rst`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/Serializer.cpp` & `PyMI-1.0.7/PyMI/Serializer.cpp`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/Session.cpp` & `PyMI-1.0.7/PyMI/Session.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -35,32 +35,32 @@
     ::DeleteCriticalSection(&self->cs);
     Py_TYPE(self)->tp_free((PyObject*)self);
 }
 
 
 static PyObject* Session_ExecQuery(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
-    wchar_t* query = NULL;
-    wchar_t* dialect = L"WQL";
+    char* ns = NULL;
+    char* query = NULL;
+    char* dialect = "WQL";
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "ns", "query", "dialect", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uu|uO", kwlist, &ns, &query,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "ss|sO", kwlist, &ns, &query,
                                      &dialect, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(operationOptions, L"operation_options",
                              &OperationOptionsType, L"OperationOptions");
         std::shared_ptr<MI::Operation> op;
         AllowThreads(&self->cs, [&]() {
             op = self->session->ExecQuery(
-                ns, query, dialect,
+                ToWstring(ns).c_str(), ToWstring(query).c_str(), ToWstring(dialect).c_str(),
                 !CheckPyNone(operationOptions)
                     ? ((OperationOptions*)operationOptions)->operationOptions
                     : NULL);
         });
         return (PyObject*)Operation_New(op);
     }
     catch (std::exception& ex)
@@ -69,25 +69,25 @@
         return NULL;
     }
 }
 
 static PyObject* Session_GetAssociators(Session *self, PyObject *args, PyObject *kwds)
 {
     PyObject* instance = NULL;
-    wchar_t* ns = NULL;
-    wchar_t* assocClass = L"";
-    wchar_t* resultClass = L"";
-    wchar_t* role = L"";
-    wchar_t* resultRole = L"";
+    char* ns = NULL;
+    char* assocClass = "";
+    char* resultClass = "";
+    char* role = "";
+    char* resultRole = "";
     PyObject* keysOnlyObj = NULL;
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "ns", "instance", "assoc_class", "result_class",
                               "role", "result_role", "keys_only", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO|uuuuOO", kwlist, &ns, &instance,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO|ssssOO", kwlist, &ns, &instance,
                                      &assocClass, &resultClass, &role, &resultRole,
                                      &keysOnlyObj, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(instance, L"instance", &InstanceType, L"Instance", false);
@@ -95,16 +95,16 @@
                              &OperationOptionsType, L"OperationOptions");
 
         bool keysOnly = keysOnlyObj && PyObject_IsTrue(keysOnlyObj);
 
         std::shared_ptr<MI::Operation> op;
         AllowThreads(&self->cs, [&]() {
             op = self->session->GetAssociators(
-                ns, *((Instance*)instance)->instance, assocClass,
-                resultClass, role, resultRole, keysOnly,
+                ToWstring(ns).c_str(), *((Instance*)instance)->instance, ToWstring(assocClass).c_str(),
+                ToWstring(resultClass).c_str(), ToWstring(role).c_str(), ToWstring(resultRole).c_str(), keysOnly,
                 !CheckPyNone(operationOptions)
                     ? ((OperationOptions*)operationOptions)->operationOptions
                     : NULL);
         });
         return (PyObject*)Operation_New(op);
     }
     catch (std::exception& ex)
@@ -146,32 +146,32 @@
     });
 
     Py_RETURN_NONE;
 }
 
 static PyObject* Session_CreateInstance(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
+    char* ns = NULL;
     PyObject* instance = NULL;
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "ns", "instance", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO|O", kwlist, &ns,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO|O", kwlist, &ns,
                                      &instance, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(instance, L"instance", &InstanceType, L"Instance", false);
         ValidatePyObjectType(operationOptions, L"operation_options",
                              &OperationOptionsType, L"OperationOptions");
 
         AllowThreads(&self->cs, [&]() {
             self->session->CreateInstance(
-                ns, *((Instance*)instance)->instance,
+                ToWstring(ns).c_str(), *((Instance*)instance)->instance,
                 !CheckPyNone(operationOptions)
                     ? ((OperationOptions*)operationOptions)->operationOptions
                     : NULL);
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
@@ -179,32 +179,32 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Session_ModifyInstance(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
+    char* ns = NULL;
     PyObject* instance = NULL;
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "ns", "instance", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO|O", kwlist, &ns,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO|O", kwlist, &ns,
                                      &instance, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(instance, L"instance", &InstanceType, L"Instance", false);
         ValidatePyObjectType(operationOptions, L"operation_options",
                              &OperationOptionsType, L"OperationOptions");
 
         AllowThreads(&self->cs, [&]() {
             self->session->ModifyInstance(
-                ns, *((Instance*)instance)->instance,
+                ToWstring(ns).c_str(), *((Instance*)instance)->instance,
                 !CheckPyNone(operationOptions)
                     ? ((OperationOptions*)operationOptions)->operationOptions
                     : NULL);
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
@@ -212,32 +212,32 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Session_DeleteInstance(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
+    char* ns = NULL;
     PyObject* instance = NULL;
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "ns", "instance", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO|O", kwlist, &ns,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO|O", kwlist, &ns,
                                      &instance, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(instance, L"instance", &InstanceType, L"Instance", false);
         ValidatePyObjectType(operationOptions, L"operation_options",
                              &OperationOptionsType, L"OperationOptions");
 
         AllowThreads(&self->cs, [&]() {
             self->session->DeleteInstance(
-                ns, *((Instance*)instance)->instance,
+                ToWstring(ns).c_str(), *((Instance*)instance)->instance,
                 !CheckPyNone(operationOptions)
                     ? ((OperationOptions*)operationOptions)->operationOptions
                     : NULL);
         });
         Py_RETURN_NONE;
     }
     catch (std::exception& ex)
@@ -245,73 +245,73 @@
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Session_GetClass(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
-    wchar_t* className = NULL;
+    char* ns = NULL;
+    char* className = NULL;
 
     static char *kwlist[] = { "ns", "class_name", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uu", kwlist, &ns, &className))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "ss", kwlist, &ns, &className))
         return NULL;
 
     try
     {
         std::shared_ptr<MI::Operation> op;
         AllowThreads(&self->cs, [&]() {
-            op = self->session->GetClass(ns, className);
+            op = self->session->GetClass(ToWstring(ns).c_str(), ToWstring(className).c_str());
         });
         return (PyObject*)Operation_New(op);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Session_GetInstance(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
+    char* ns = NULL;
     PyObject* keyInstance = NULL;
 
     static char *kwlist[] = { "ns", "key_instance", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uO", kwlist, &ns, &keyInstance))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "sO", kwlist, &ns, &keyInstance))
         return NULL;
 
     try
     {
         if (!PyObject_IsInstance(keyInstance, reinterpret_cast<PyObject*>(&InstanceType)))
             throw MI::TypeConversionException(L"\"instance\" must have type Instance");
 
         std::shared_ptr<MI::Operation> op;
         AllowThreads(&self->cs, [&]() {
-            op = self->session->GetInstance(ns, *((Instance*)keyInstance)->instance);
+            op = self->session->GetInstance(ToWstring(ns).c_str(), *((Instance*)keyInstance)->instance);
         });
         return (PyObject*)Operation_New(op);
     }
     catch (std::exception& ex)
     {
         SetPyException(ex);
         return NULL;
     }
 }
 
 static PyObject* Session_Subscribe(Session *self, PyObject *args, PyObject *kwds)
 {
-    wchar_t* ns = NULL;
-    wchar_t* query = NULL;
+    char* ns = NULL;
+    char* query = NULL;
     PyObject* indicationResultCallback = NULL;
     PyObject* operationOptions = NULL;
-    wchar_t* dialect = L"WQL";
+    char* dialect = "WQL";
 
     static char *kwlist[] = { "ns", "query", "indication_result", "operation_options", "dialect", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "uu|OOu", kwlist, &ns, &query, &indicationResultCallback, &operationOptions, &dialect))
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "ss|OOs", kwlist, &ns, &query, &indicationResultCallback, &operationOptions, &dialect))
         return NULL;
 
     try
     {
         if (!CheckPyNone(indicationResultCallback) && !PyCallable_Check(indicationResultCallback))
         {
             throw MI::TypeConversionException(L"\"indication_result\" must be callable");
@@ -321,17 +321,17 @@
             throw MI::TypeConversionException(L"\"operation_options\" must have type OperationOptions");
         }
 
         auto callbacks = !CheckPyNone(indicationResultCallback) ? std::make_shared<PythonMICallbacks>(indicationResultCallback) : NULL;
 
         std::shared_ptr<MI::Operation> op;
         AllowThreads(&self->cs, [&]() {
-            op = self->session->Subscribe(ns, query, callbacks,
+            op = self->session->Subscribe(ToWstring(ns).c_str(), ToWstring(query).c_str(), callbacks,
                 !CheckPyNone(operationOptions) ? ((OperationOptions*)operationOptions)->operationOptions : NULL,
-                dialect);
+                ToWstring(dialect).c_str());
         });
         PyObject* obj = (PyObject*)Operation_New(op);
         if (callbacks)
         {
             self->operationCallbacks->push_back(callbacks);
         }
         return obj;
@@ -342,45 +342,45 @@
         return NULL;
     }
 }
 
 static PyObject* Session_InvokeMethod(Session *self, PyObject *args, PyObject *kwds)
 {
     PyObject* target = NULL;
-    wchar_t* methodName = NULL;
+    char* methodName = NULL;
     PyObject* inboundParams = NULL;
     PyObject* operationOptions = NULL;
 
     static char *kwlist[] = { "target", "method_name", "inbound_params", "operation_options", NULL };
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "Ou|OO", kwlist,
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "Os|OO", kwlist,
                                      &target, &methodName, &inboundParams, &operationOptions))
         return NULL;
 
     try
     {
         ValidatePyObjectType(inboundParams, L"inbound_params", &InstanceType, L"Instance");
         ValidatePyObjectType(operationOptions, L"operation_options",
                              &OperationOptionsType, L"OperationOptions");
 
         std::shared_ptr<MI::Operation> op;
         if (PyObject_IsInstance(target, reinterpret_cast<PyObject*>(&InstanceType)))
         {
             AllowThreads(&self->cs, [&]() {
-                op = self->session->InvokeMethod(*((Instance*)target)->instance, methodName,
+                op = self->session->InvokeMethod(*((Instance*)target)->instance, ToWstring(methodName).c_str(),
                     !CheckPyNone(inboundParams) ? ((Instance*)inboundParams)->instance : NULL,
                     !CheckPyNone(operationOptions)
                         ? ((OperationOptions*)operationOptions)->operationOptions
                         : NULL);
             });
         }
         else if (PyObject_IsInstance(target, reinterpret_cast<PyObject*>(&ClassType)))
         {
             AllowThreads(&self->cs, [&]() {
                 auto miClass = ((Class*)target)->miClass;
-                op = self->session->InvokeMethod(miClass->GetNameSpace(), miClass->GetClassName(), methodName,
+                op = self->session->InvokeMethod(miClass->GetNameSpace(), miClass->GetClassName(), ToWstring(methodName).c_str(),
                     !CheckPyNone(inboundParams) ? ((Instance*)inboundParams)->instance : NULL,
                     !CheckPyNone(operationOptions)
                         ? ((OperationOptions*)operationOptions)->operationOptions
                         : NULL);
             });
         }
         else
```

### Comparing `PyMI-1.0.6/PyMI/Utils.cpp` & `PyMI-1.0.7/PyMI/Utils.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "stdafx.h"
 #include "PyMI.h"
 #include "Utils.h"
 #include "instance.h"
 #include <codecvt>
+#include <locale>
 
 #include <datetime.h>
 
 bool CheckPyNone(PyObject* obj)
 {
     return !obj || obj == Py_None;
 }
@@ -115,15 +116,15 @@
         name.assign(w, len);
         delete[] w;
     }
     else
 #endif
     if (PyUnicode_Check(item))
     {
-        Py_ssize_t len = PyUnicode_GetSize(item) + 1;
+        Py_ssize_t len = PyUnicode_GetLength(item) + 1;
         wchar_t* w = new wchar_t[len];
 
         if (PyUnicode_AsWideChar((PYUNICODEASVARCHARARG1TYPE*)item, w, len) < 0)
         {
             delete[] w;
             throw MI::Exception(L"PyUnicode_AsWideChar failed");
         }
@@ -138,24 +139,24 @@
     }
     else
         throw MI::Exception(L"Invalid name or index");
 }
 
 std::wstring Py2WString(PyObject* pyValue)
 {
-    auto len = PyUnicode_GetSize(pyValue) + 1;
+    auto len = PyUnicode_GetLength(pyValue) + 1;
     wchar_t* w = new wchar_t[len];
 
     if (PyUnicode_AsWideChar((PYUNICODEASVARCHARARG1TYPE*)pyValue, w, len) < 0)
     {
         delete[] w;
         throw MI::Exception(L"PyUnicode_AsWideChar failed");
     }
 
-    auto& value = std::wstring(w, len);
+    auto value = std::wstring(w, len);
     delete[] w;
     return value;
 }
 
 std::shared_ptr<MI::MIValue> Py2StrMIValue(PyObject* pyValue)
 {
     PyObject* pyStrValue = PyObject_CallMethod(pyValue, "__str__", NULL);
@@ -163,17 +164,17 @@
     {
         throw MI::Exception(L"PyObject_CallMethod failed for __str__");
     }
 
     try
     {
 #ifdef IS_PY3K
-        auto& value = Py2WString(pyStrValue);
+        auto value = Py2WString(pyStrValue);
 #else
-        auto& value = std::string(PyString_AsString(pyStrValue));
+        auto value = std::string(PyString_AsString(pyStrValue));
 #endif
         Py_DECREF(pyStrValue);
         return MI::MIValue::FromString(value);
     }
     catch (std::exception&)
     {
         Py_DECREF(pyStrValue);
@@ -368,15 +369,15 @@
                 pyObj = PyTuple_GetItem(pyValue, i);
             }
             else
             {
                 pyObj = PyList_GetItem(pyValue, i);
             }
 
-            auto& tmpValue = Py2MI(pyObj, itemType);
+            auto tmpValue = Py2MI(pyObj, itemType);
             value->SetArrayItem(*tmpValue, (unsigned)i);
         }
         return value;
     }
     else
     {
         switch (valueType)
@@ -511,7 +512,35 @@
 
     if ((isNone && !allowNone) ||
         (!isNone && !PyObject_IsInstance(obj,
                                          reinterpret_cast<PyObject*>(expectedType))))
         throw MI::TypeConversionException(
             L"\"" + objName + L"\"must have type " + expectedTypeName);
 }
+
+std::wstring ToWstring(const std::string& inString)
+{
+    if (inString.empty())
+    {
+        return L"";
+    }
+
+    int sizeNeeded = MultiByteToWideChar(CP_UTF8, 0, &inString.at(0), (int)inString.size(), nullptr, 0);
+    if (sizeNeeded <= 0)
+    {
+        DWORD err = GetLastError();
+        throw MI::TypeConversionException(
+            L"wstring conversion failed. Error: " + std::to_wstring(err));
+    }
+
+    std::wstring result(sizeNeeded, 0);
+    sizeNeeded = MultiByteToWideChar(
+        CP_UTF8, 0, &inString.at(0), (int)inString.size(),
+        &result.at(0), sizeNeeded);
+    if (sizeNeeded <= 0) {
+        DWORD err = GetLastError();
+        throw MI::TypeConversionException(
+            L"wstring conversion failed. Error: " + std::to_wstring(err));
+    }
+
+    return result;
+}
```

### Comparing `PyMI-1.0.6/PyMI/Utils.h` & `PyMI-1.0.7/PyMI/Utils.h`

 * *Files 7% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 void CallPythonCallback(PyObject* callable, const char* format, ...);
 void MIIntervalFromPyDelta(PyObject* pyDelta, MI_Interval& interval);
 PyObject* PyDeltaFromMIInterval(const MI_Interval& interval);
 bool CheckPyNone(PyObject* obj);
 void ValidatePyObjectType(PyObject* obj, const std::wstring& objName,
                           PyTypeObject* expectedType, const std::wstring& expectedTypeName,
                           bool allowNone = true);
+std::wstring ToWstring(const std::string& inString);
```

### Comparing `PyMI-1.0.6/PyMI/setup_vs.py` & `PyMI-1.0.7/PyMI/setup_vs.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI/stdafx.h` & `PyMI-1.0.7/PyMI/stdafx.h`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/PyMI.egg-info/PKG-INFO` & `PyMI-1.0.7/PyMI.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,209 +1,213 @@
 Metadata-Version: 2.1
 Name: PyMI
-Version: 1.0.6
+Version: 1.0.7
 Summary: Windows Management Infrastructure API for Python.
 Home-page: https://github.com/cloudbase/PyMI
 Author: Alessandro Pilotti
 Author-email: info@cloudbasesolutions.com
-License: UNKNOWN
-Description: PyMI - Windows Management Infrastructure API for Python
-        =======================================================
-        
-        This project provides a Python native module wrapper over the Windows
-        Management Infrastructure (MI) API [#miapi]_.
-        
-        Works with Python 2.7 and 3.x on any Windows version which supports the MI API,
-        both x86 and x64.
-        
-        It includes also a drop-in replacement for the Python WMI [#pywmi]_ module,
-        proving much faster execution times and no dependency on pywin32.
-        
-        Installation
-        ------------
-        
-        Pip is the preferred way to install PyMI. Pre-compiled binary wheels are
-        available on Pypi [#pymipypi]_:
-        
-        .. code-block:: powershell
-        
-            pip install PyMI
-        
-        Usage
-        -----
-        
-        This project can be used either with a lower level interface that reflects the
-        underlying MI API structure or with the higher level (and slightly slower)
-        WMI module replacement.
-        
-        MI module basic usage
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        Here's a simple example which enumerates all processes and kills any instance of
-        "KillerRabbitOfCaerbannog.exe".
-        
-        .. code-block:: python
-        
-            import mi
-        
-            with mi.Application() as a:
-                with a.create_session(protocol=mi.PROTOCOL_WMIDCOM) as s:
-                    proc_name = u'notepad.exe'
-                    with s.exec_query(
-                            u"root\\cimv2", u"select * from Win32_Process") as q:
-                        i = q.get_next_instance()
-                        while i is not None:
-                            if i[u'name'].lower() == u"KillerRabbitOfCaerbannog.exe":
-                                cls = i.get_class()
-                                # Prepare parameters
-                                params = a.create_method_params(cls, u"Terminate")
-                                # Exit code
-                                params['reason'] = 10
-                                # Invoke method
-                                with s.invoke_method(i, u"Terminate", params) as op:
-                                    op.get_next_instance()
-                            i = q.get_next_instance()
-        
-        WMI module basic usage
-        ^^^^^^^^^^^^^^^^^^^^^^
-        
-        And here's the same example written using the *WMI* module replacement,
-        which provides a simpler and higher level interface over the *mi* API:
-        
-        .. code-block:: python
-        
-            import wmi
-        
-            conn = wmi.WMI()
-            for p in conn.Win32_Process():
-                if p.Name == u"KillerRabbitOfCaerbannog.exe":
-                    p.Terminate(reason=10)
-        
-        
-        Build
-        -----
-        
-        Use the following to build Python 3 wheels. Those will be copied to the build
-        dir.
-        
-        .. code-block:: powershell
-        
-            python setup.py bdist_wheel
-        
-        The best way to build PyMI for Python 2.7 or 3.4 and below is to use the
-        Visual Studio solution (described below). This will statically link the
-        vc140 runtime, which is required by PyMI.
-        
-        Custom VS env vars
-        ^^^^^^^^^^^^^^^^^^
-        
-        distutils will automatically locate your Visual Studio and Windows SDK
-        installation. If you'd like to call vcvarsall.bat yourself and use a specific
-        version, use the following:
-        
-        .. code-block:: powershell
-        
-            function SetVCVars($vcvarsdir, $platform="amd64")
-            {
-                pushd $vcvarsdir
-                try
-                {
-                    cmd /c "vcvarsall.bat $platform & set" |
-                    foreach {
-                      if ($_ -match "=") {
-                        $v = $_.split("="); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
-                      }
-                    }
-                }
-                finally
-                {
-                    popd
-                }
-            }
-        
-            # Replace this folder with the one in which the vcvarsall.bat script is
-            # located (the exact location depends on the Visual Studio version).
-            # SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\VC\Auxiliary\Build"
-            SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC"
-        
-            $env:DISTUTILS_USE_SDK=1
-            $env:MSSdk=1
-        
-            python setup.py bdist_wheel
-        
-        Make sure to use the Visual Studio toolset that matches the Python version
-        that you're targetting: https://wiki.python.org/moin/WindowsCompilers.
-        
-        By default, we're statically linking the VC runtime. To enable dynamic
-        linking, set ``$env:PYMI_VCRUNTIME_DYNAMIC_LINKING="y"``.
-        
-        Debug builds
-        ^^^^^^^^^^^^
-        
-        The easiest way to do a debug build is to set the following in setup.cfg:
-        
-        .. code-block::
-        
-            [build]
-            debug = 1
-        
-        This will be honored regardless of the build type (e.g. stdist, wheel, etc).
-        
-        To enable distutils debug logging, you may set the following:
-        
-        .. code-block:: powershell
-        
-            $env:DISTUTILS_DEBUG = 1
-        
-        Before doing a debug build, you may wish to clean the build dir.
-        
-        Using the Visual Studio Solution
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Open the provided *PyMI.sln* solution in Visual Studio 2015 [#VS2015]_, choose
-        your target Python version / platform and build. Wheel packages are
-        automatically generated in the *dist* folder for release builds.
-        
-        Note: the target Python version must be present. The Python path can be
-        customized by setting the corresponding PythonDir* user macro,
-        e.g. *PythonDir_34_x64*. The *wheel* and *GitPython* packages are required during the build process:
-        
-        .. code-block:: powershell
-        
-            pip install wheel
-            pip install GitPython
-        
-        As an alternative, you can use the MSBuild CLI tool:
-        
-        .. code-block:: powershell
-        
-            $env:MSBuildEmitSolution="TRUE"
-            MSBuild.exe .\PyMI.sln /p:Configuration="Release (Python 3.7)"
-        
-        
-        References
-        ----------
-        
-        .. [#miapi] MI API https://msdn.microsoft.com/en-us/library/hh404805(v=vs.85).aspx
-        .. [#pywmi] Python WMI module https://pypi.python.org/pypi/WMI
-        .. [#pymipypi] PyMI on Pypi https://pypi.python.org/pypi/PyMI
-        .. [#vs2015] Visual Studio 2015 download https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx
-        
-        
 Keywords: wmi mi windows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Systems Administration
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+PyMI - Windows Management Infrastructure API for Python
+=======================================================
+
+This project provides a Python native module wrapper over the Windows
+Management Infrastructure (MI) API [#miapi]_.
+
+Works with Python 2.7 and 3.x on any Windows version which supports the MI API,
+both x86 and x64.
+
+It includes also a drop-in replacement for the Python WMI [#pywmi]_ module,
+proving much faster execution times and no dependency on pywin32.
+
+Installation
+------------
+
+Pip is the preferred way to install PyMI. Pre-compiled binary wheels are
+available on Pypi [#pymipypi]_:
+
+.. code-block:: powershell
+
+    pip install PyMI
+
+Usage
+-----
+
+This project can be used either with a lower level interface that reflects the
+underlying MI API structure or with the higher level (and slightly slower)
+WMI module replacement.
+
+MI module basic usage
+^^^^^^^^^^^^^^^^^^^^^
+
+Here's a simple example which enumerates all processes and kills any instance of
+"KillerRabbitOfCaerbannog.exe".
+
+.. code-block:: python
+
+    import mi
+
+    with mi.Application() as a:
+        with a.create_session(protocol=mi.PROTOCOL_WMIDCOM) as s:
+            proc_name = u'notepad.exe'
+            with s.exec_query(
+                    u"root\\cimv2", u"select * from Win32_Process") as q:
+                i = q.get_next_instance()
+                while i is not None:
+                    if i[u'name'].lower() == u"KillerRabbitOfCaerbannog.exe":
+                        cls = i.get_class()
+                        # Prepare parameters
+                        params = a.create_method_params(cls, u"Terminate")
+                        # Exit code
+                        params['reason'] = 10
+                        # Invoke method
+                        with s.invoke_method(i, u"Terminate", params) as op:
+                            op.get_next_instance()
+                    i = q.get_next_instance()
+
+WMI module basic usage
+^^^^^^^^^^^^^^^^^^^^^^
+
+And here's the same example written using the *WMI* module replacement,
+which provides a simpler and higher level interface over the *mi* API:
+
+.. code-block:: python
+
+    import wmi
+
+    conn = wmi.WMI()
+    for p in conn.Win32_Process():
+        if p.Name == u"KillerRabbitOfCaerbannog.exe":
+            p.Terminate(reason=10)
+
+
+Build
+-----
+
+Use the following to build Python 3 wheels. Those will be copied to the build
+dir.
+
+.. code-block:: powershell
+
+    python setup.py bdist_wheel
+
+The best way to build PyMI for Python 2.7 or 3.4 and below is to use the
+Visual Studio solution (described below). This will statically link the
+vc140 runtime, which is required by PyMI.
+
+Custom VS env vars
+^^^^^^^^^^^^^^^^^^
+
+distutils will automatically locate your Visual Studio and Windows SDK
+installation. If you'd like to call vcvarsall.bat yourself and use a specific
+version, use the following:
+
+.. code-block:: powershell
+
+    function SetVCVars($vcvarsdir, $platform="amd64")
+    {
+        pushd $vcvarsdir
+        try
+        {
+            cmd /c "vcvarsall.bat $platform & set" |
+            foreach {
+              if ($_ -match "=") {
+                $v = $_.split("="); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
+              }
+            }
+        }
+        finally
+        {
+            popd
+        }
+    }
+
+    # Replace this folder with the one in which the vcvarsall.bat script is
+    # located (the exact location depends on the Visual Studio version).
+    # SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\VC\Auxiliary\Build"
+    SetVCVars "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC"
+
+    $env:DISTUTILS_USE_SDK=1
+    $env:MSSdk=1
+
+    python setup.py bdist_wheel
+
+Make sure to use the Visual Studio toolset that matches the Python version
+that you're targetting: https://wiki.python.org/moin/WindowsCompilers.
+
+By default, we're statically linking the VC runtime. To enable dynamic
+linking, set ``$env:PYMI_VCRUNTIME_DYNAMIC_LINKING="y"``.
+
+Debug builds
+^^^^^^^^^^^^
+
+The easiest way to do a debug build is to set the following in setup.cfg:
+
+.. code-block::
+
+    [build]
+    debug = 1
+
+This will be honored regardless of the build type (e.g. stdist, wheel, etc).
+
+To enable distutils debug logging, you may set the following:
+
+.. code-block:: powershell
+
+    $env:DISTUTILS_DEBUG = 1
+
+Before doing a debug build, you may wish to clean the build dir.
+
+Using the Visual Studio Solution
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Open the provided *PyMI.sln* solution in Visual Studio 2015 [#VS2015]_, choose
+your target Python version / platform and build. Wheel packages are
+automatically generated in the *dist* folder for release builds.
+
+Note: the target Python version must be present. The Python path can be
+customized by setting the corresponding PythonDir* user macro,
+e.g. *PythonDir_34_x64*. The *wheel* and *GitPython* packages are required during the build process:
+
+.. code-block:: powershell
+
+    pip install wheel
+    pip install GitPython
+
+As an alternative, you can use the MSBuild CLI tool:
+
+.. code-block:: powershell
+
+    $env:MSBuildEmitSolution="TRUE"
+    MSBuild.exe .\PyMI.sln /p:Configuration="Release (Python 3.7)"
+
+
+References
+----------
+
+.. [#miapi] MI API https://msdn.microsoft.com/en-us/library/hh404805(v=vs.85).aspx
+.. [#pywmi] Python WMI module https://pypi.python.org/pypi/WMI
+.. [#pymipypi] PyMI on Pypi https://pypi.python.org/pypi/PyMI
+.. [#vs2015] Visual Studio 2015 download https://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx
+
```

### Comparing `PyMI-1.0.6/PyMI.egg-info/SOURCES.txt` & `PyMI-1.0.7/PyMI.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ChangeLog
 LICENSE
 PyMI.sln
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/pymi-cd.yml
 MI/MI++.cpp
 MI/MI++.h
 MI/MI.vcxproj
 MI/MI.vcxproj.filters
 MI/MIExceptions.cpp
 MI/MIExceptions.h
 MI/MIValue.cpp
```

### Comparing `PyMI-1.0.6/PyMI.sln` & `PyMI-1.0.7/PyMI.sln`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/setup.py` & `PyMI-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from distutils import _msvccompiler
 from distutils import ccompiler
 import os
 import setuptools
+import sys
 
 try:
     import multiprocessing  # noqa
 except ImportError:
     pass
 
 
@@ -33,15 +34,16 @@
           self.compile_options_debug.append('/MTd')
 
 
 def new_compiler(plat=None, compiler=None, verbose=0, dry_run=0, force=0):
     return Compiler(None, dry_run, force)
 
 
-ccompiler.new_compiler = new_compiler
+if 'MSC' in sys.version:
+    ccompiler.new_compiler = new_compiler
 
 
 # Setuptools requires relative paths
 mi_dir = 'MI'
 pymi_dir = 'PyMI'
 
 libmipp = (
```

### Comparing `PyMI-1.0.6/wmi/__init__.py` & `PyMI-1.0.7/wmi/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/samples/benchmark.py` & `PyMI-1.0.7/wmi/samples/benchmark.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/samples/benchmark2.py` & `PyMI-1.0.7/wmi/samples/benchmark2.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/samples/benchmark3.py` & `PyMI-1.0.7/wmi/samples/benchmark3.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/samples/custom_operation_options.py` & `PyMI-1.0.7/wmi/samples/custom_operation_options.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/tests/functional/test_base.py` & `PyMI-1.0.7/wmi/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `PyMI-1.0.6/wmi/tests/functional/test_basic_ops.py` & `PyMI-1.0.7/wmi/tests/functional/test_basic_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import os
 import time
 
 import wmi
 from wmi.tests.functional import test_base
 
 
 class BasicOpsTestCase(test_base.BaseFunctionalTestCase):
@@ -43,20 +42,25 @@
 
         with open(temp_file_path, 'r') as f:
             actual_content = f.read().strip('\n ')
 
         self.assertEqual(content, actual_content)
 
     def test_associators(self):
-        logical_disk = self._conn_cimv2.Win32_LogicalDisk()[0]
-        root_dir = logical_disk.associators(
-            wmi_association_class="Win32_LogicalDiskRootDirectory")[0]
-
-        self.assertEqual(logical_disk.Name.lower(),
-                         root_dir.Name.lower().strip('\\'))
+        logical_disks = self._conn_cimv2.Win32_LogicalDisk()
+        found_associators = False
+        for logical_disk in logical_disks:
+            root_dirs = logical_disk.associators(
+                wmi_association_class="Win32_LogicalDiskRootDirectory")
+            if len(root_dirs) == 1:
+                found_associators = True
+                root_dir = root_dirs[0]
+                self.assertEqual(logical_disk.Name.lower(),
+                                 root_dir.Name.lower().strip('\\'))
+        self.assertTrue(found_associators)
 
     def test_new_conn_invalid_creds(self):
         err_code = None
         try:
             wmi.WMI(user='invalidcredstest')
         except wmi.x_wmi as exc:
             err_code = exc.com_error.hresult & 0xFFFF
```

### Comparing `PyMI-1.0.6/wmi/tests/functional/test_timeouts.py` & `PyMI-1.0.7/wmi/tests/functional/test_timeouts.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import os
 import time
+import unittest
 
 import wmi
 from wmi.tests.functional import test_base
 
 
 # The following tests perform various operations,
 # setting timeouts that are expected to be hit.
@@ -27,14 +28,16 @@
         # 'f' is expected to be a method that accepts
         # operation options.
         self.assertRaises(wmi.x_wmi_timed_out,
                           f, *args,
                           operation_options={'operation_timeout': 0.001},
                           **kwargs)
 
+    @unittest.skipIf(os.getenv("GITHUB_ACTIONS") == "true",
+                     "Skipping on GitHub actions")
     def test_query(self):
         self._check_op_timeout(self._conn_cimv2.Win32_Process)
 
     @test_base.BaseFunctionalTestCase.pass_temp_file
     @test_base.BaseFunctionalTestCase.pass_temp_file
     def test_invoke_method(self, temp_src, temp_dest):
         with open(temp_src, 'w') as f:
```

