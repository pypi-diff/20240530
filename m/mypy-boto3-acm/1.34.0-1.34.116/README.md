# Comparing `tmp/mypy-boto3-acm-1.34.0.tar.gz` & `tmp/mypy_boto3_acm-1.34.116.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.34.0.tar", last modified: Wed Dec 13 21:21:50 2023, max compression
+gzip compressed data, was "mypy_boto3_acm-1.34.116.tar", last modified: Thu May 30 20:33:06 2024, max compression
```

## Comparing `mypy-boto3-acm-1.34.0.tar` & `mypy_boto3_acm-1.34.116.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:21:50.051111 mypy-boto3-acm-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2023-12-13 21:21:50.051111 mypy-boto3-acm-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:21:50.051111 mypy-boto3-acm-1.34.0/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13670 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:21:50.051111 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:21:50.000000 mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:21:50.051111 mypy-boto3-acm-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:05:13.000000 mypy-boto3-acm-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.160221 mypy_boto3_acm-1.34.116/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-30 20:33:06.160221 mypy_boto3_acm-1.34.116/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.160221 mypy_boto3_acm-1.34.116/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13613 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-30 20:32:05.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:33:06.160221 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 20:33:06.000000 mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 20:33:06.160221 mypy_boto3_acm-1.34.116/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 20:32:04.000000 mypy_boto3_acm-1.34.116/setup.py
```

### Comparing `mypy-boto3-acm-1.34.0/LICENSE` & `mypy_boto3_acm-1.34.116/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-acm-1.34.0/PKG-INFO` & `mypy_boto3_acm-1.34.116/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.34.0
-Summary: Type annotations for boto3.ACM 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.116
+Summary: Type annotations for boto3.ACM 1.34.116 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.34.0/README.md` & `mypy_boto3_acm-1.34.116/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/__init__.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 
 from .client import ACMClient
 from .paginator import ListCertificatesPaginator
 from .waiter import CertificateValidatedWaiter
 
 Client = ACMClient
 
-
 __all__ = ("ACMClient", "CertificateValidatedWaiter", "Client", "ListCertificatesPaginator")
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/__init__.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/__main__.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACM 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ACM 1.34.116\n"
+        "Version:         1.34.116\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.116")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/client.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 from .waiter import CertificateValidatedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ACMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -183,15 +182,15 @@
     def import_certificate(
         self,
         *,
         Certificate: BlobTypeDef,
         PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
         CertificateChain: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with
         ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
@@ -202,15 +201,15 @@
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         NextToken: str = ...,
         MaxItems: int = ...,
         SortBy: Literal["CREATED_AT"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCertificatesResponseTypeDef:
         """
         Retrieves a list of certificate ARNs and domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#list_certificates)
         """
@@ -260,15 +259,15 @@
         ValidationMethod: ValidationMethodType = ...,
         SubjectAlternativeNames: Sequence[str] = ...,
         IdempotencyToken: str = ...,
         DomainValidationOptions: Sequence[DomainValidationOptionTypeDef] = ...,
         Options: CertificateOptionsTypeDef = ...,
         CertificateAuthorityArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KeyAlgorithm: KeyAlgorithmType = ...
+        KeyAlgorithm: KeyAlgorithmType = ...,
     ) -> RequestCertificateResponseTypeDef:
         """
         Requests an ACM certificate for use with other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#request_certificate)
         """
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/client.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     def import_certificate(
         self,
         *,
         Certificate: BlobTypeDef,
         PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
         CertificateChain: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with
         ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
@@ -198,15 +198,15 @@
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         NextToken: str = ...,
         MaxItems: int = ...,
         SortBy: Literal["CREATED_AT"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCertificatesResponseTypeDef:
         """
         Retrieves a list of certificate ARNs and domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#list_certificates)
         """
@@ -256,15 +256,15 @@
         ValidationMethod: ValidationMethodType = ...,
         SubjectAlternativeNames: Sequence[str] = ...,
         IdempotencyToken: str = ...,
         DomainValidationOptions: Sequence[DomainValidationOptionTypeDef] = ...,
         Options: CertificateOptionsTypeDef = ...,
         CertificateAuthorityArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KeyAlgorithm: KeyAlgorithmType = ...
+        KeyAlgorithm: KeyAlgorithmType = ...,
     ) -> RequestCertificateResponseTypeDef:
         """
         Requests an ACM certificate for use with other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#request_certificate)
         """
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/literals.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CertificateStatusType",
     "CertificateTransparencyLoggingPreferenceType",
     "CertificateTypeType",
     "CertificateValidatedWaiterName",
     "DomainStatusType",
     "ExtendedKeyUsageNameType",
@@ -42,15 +41,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CertificateStatusType = Literal[
     "EXPIRED",
     "FAILED",
     "INACTIVE",
     "ISSUED",
     "PENDING_VALIDATION",
     "REVOKED",
@@ -151,14 +149,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -169,14 +168,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -194,14 +194,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -214,24 +215,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -292,15 +295,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -342,14 +344,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -372,17 +375,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -427,14 +432,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -472,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -528,14 +536,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/literals.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -167,14 +168,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -192,14 +194,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -212,24 +215,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -290,15 +295,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -340,14 +344,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -370,17 +375,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -425,14 +432,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -470,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -526,14 +536,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/paginator.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,16 @@
 from .type_defs import FiltersTypeDef, ListCertificatesResponseTypeDef, PaginatorConfigTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ListCertificatesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -56,13 +54,13 @@
     def paginate(
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         SortBy: Literal["CREATED_AT"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/paginators/#listcertificatespaginator)
         """
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/paginator.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,13 +52,13 @@
     def paginate(
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         SortBy: Literal["CREATED_AT"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/paginators/#listcertificatespaginator)
         """
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/type_defs.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
@@ -163,18 +162,18 @@
         "CertificateArn": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DomainValidationOptionTypeDef = TypedDict(
     "DomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ValidationDomain": str,
@@ -310,17 +309,17 @@
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
-        "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForCertificateResponseTypeDef = TypedDict(
     "ListTagsForCertificateResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/type_defs.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,18 @@
         "CertificateArn": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DomainValidationOptionTypeDef = TypedDict(
     "DomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ValidationDomain": str,
@@ -309,17 +309,17 @@
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
-        "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForCertificateResponseTypeDef = TypedDict(
     "ListTagsForCertificateResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/waiter.py` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm/waiter.pyi` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.34.0
-Summary: Type annotations for boto3.ACM 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.116
+Summary: Type annotations for boto3.ACM 1.34.116 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.34.116](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.34.0/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy_boto3_acm-1.34.116/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.34.0/setup.py` & `mypy_boto3_acm-1.34.116/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.34.0",
+    version="1.34.116",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ACM 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.ACM 1.34.116 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 acm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_acm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

