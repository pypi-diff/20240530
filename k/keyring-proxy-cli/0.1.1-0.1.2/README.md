# Comparing `tmp/keyring_proxy_cli-0.1.1.tar.gz` & `tmp/keyring_proxy_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy_cli-0.1.1.tar", last modified: Thu May 30 11:10:54 2024, max compression
+gzip compressed data, was "keyring_proxy_cli-0.1.2.tar", last modified: Thu May 30 11:19:56 2024, max compression
```

## Comparing `keyring_proxy_cli-0.1.1.tar` & `keyring_proxy_cli-0.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       20 2024-05-30 10:55:43.636880 keyring_proxy_cli-0.1.1/README.md
--rw-r--r--   0        0        0      823 2024-05-30 11:10:54.459151 keyring_proxy_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2024-05-30 10:56:25.116648 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/@plugins_snapshot.json
--rw-r--r--   0        0        0   189316 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.data.json
--rw-r--r--   0        0        0     1671 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.meta.json
--rw-r--r--   0        0        0    57014 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.data.json
--rw-r--r--   0        0        0     1711 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.meta.json
--rw-r--r--   0        0        0    26727 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.data.json
--rw-r--r--   0        0        0     1682 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.meta.json
--rw-r--r--   0        0        0   110678 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1736 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    27616 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/abc.data.json
--rw-r--r--   0        0        0     1654 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/abc.meta.json
--rw-r--r--   0        0        0  1646741 2024-05-30 10:56:00.368015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.data.json
--rw-r--r--   0        0        0     1738 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.meta.json
--rw-r--r--   0        0        0   129530 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.data.json
--rw-r--r--   0        0        0     1722 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.meta.json
--rw-r--r--   0        0        0   717970 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.data.json
--rw-r--r--   0        0        0     1727 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.meta.json
--rw-r--r--   0        0        0     3841 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.data.json
--rw-r--r--   0        0        0     1638 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.meta.json
--rw-r--r--   0        0        0   128242 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.data.json
--rw-r--r--   0        0        0     1690 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.meta.json
--rw-r--r--   0        0        0    82332 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.data.json
--rw-r--r--   0        0        0     1705 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.meta.json
--rw-r--r--   0        0        0     7682 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.data.json
--rw-r--r--   0        0        0     1690 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.meta.json
--rw-r--r--   0        0        0    16410 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.data.json
--rw-r--r--   0        0        0     1654 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.meta.json
--rw-r--r--   0        0        0     7437 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.data.json
--rw-r--r--   0        0        0     1667 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25149 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.data.json
--rw-r--r--   0        0        0     1639 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.meta.json
--rw-r--r--   0        0        0     9370 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.data.json
--rw-r--r--   0        0        0     1652 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.meta.json
--rw-r--r--   0        0        0   101120 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.data.json
--rw-r--r--   0        0        0     1755 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.meta.json
--rw-r--r--   0        0        0    33224 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.data.json
--rw-r--r--   0        0        0     1740 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.meta.json
--rw-r--r--   0        0        0   114573 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/enum.data.json
--rw-r--r--   0        0        0     1681 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/enum.meta.json
--rw-r--r--   0        0        0    30200 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.data.json
--rw-r--r--   0        0        0     1680 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.meta.json
--rw-r--r--   0        0        0     6285 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.data.json
--rw-r--r--   0        0        0     1667 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.meta.json
--rw-r--r--   0        0        0    77616 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.data.json
--rw-r--r--   0        0        0     1784 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.meta.json
--rw-r--r--   0        0        0    67076 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.data.json
--rw-r--r--   0        0        0     1773 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.meta.json
--rw-r--r--   0        0        0   102899 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1811 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12631 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1655 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    90072 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/io.data.json
--rw-r--r--   0        0        0     1724 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/io.meta.json
--rw-r--r--   0        0        0     1547 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.data.json
--rw-r--r--   0        0        0     1571 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.meta.json
--rw-r--r--   0        0        0   398087 2024-05-30 10:56:00.258010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.data.json
--rw-r--r--   0        0        0     1776 2024-05-30 10:56:00.258010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.meta.json
--rw-r--r--   0        0        0     4928 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.data.json
--rw-r--r--   0        0        0     1627 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.meta.json
--rw-r--r--   0        0        0   107450 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.data.json
--rw-r--r--   0        0        0     1733 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.meta.json
--rw-r--r--   0        0        0   124441 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.data.json
--rw-r--r--   0        0        0     1707 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.meta.json
--rw-r--r--   0        0        0   243099 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/re.data.json
--rw-r--r--   0        0        0     1752 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/re.meta.json
--rw-r--r--   0        0        0    14477 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.data.json
--rw-r--r--   0        0        0     1652 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.meta.json
--rw-r--r--   0        0        0    28934 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.data.json
--rw-r--r--   0        0        0     1664 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.meta.json
--rw-r--r--   0        0        0    50986 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.data.json
--rw-r--r--   0        0        0     1707 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.meta.json
--rw-r--r--   0        0        0   221898 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.data.json
--rw-r--r--   0        0        0     1726 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.meta.json
--rw-r--r--   0        0        0   156120 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sys.data.json
--rw-r--r--   0        0        0     1740 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sys.meta.json
--rw-r--r--   0        0        0   302750 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/types.data.json
--rw-r--r--   0        0        0     1718 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/types.meta.json
--rw-r--r--   0        0        0   609850 2024-05-30 10:56:00.218009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing.data.json
--rw-r--r--   0        0        0     1716 2024-05-30 10:56:00.218009 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing.meta.json
--rw-r--r--   0        0        0    97019 2024-05-30 10:56:00.198008 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.data.json
--rw-r--r--   0        0        0     1727 2024-05-30 10:56:00.198008 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.meta.json
--rw-r--r--   0        0        0      190 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1873 2024-05-30 11:10:46.228764 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/__init__.py
--rw-r--r--   0        0        0       73 2024-05-30 10:56:24.676625 keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/__main__.py
--rw-r--r--   0        0        0        0 2024-05-30 10:55:43.636880 keyring_proxy_cli-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 keyring_proxy_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-30 10:55:43.636880 keyring_proxy_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      823 2024-05-30 11:19:56.122408 keyring_proxy_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2024-05-30 10:56:25.116648 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/@plugins_snapshot.json
+-rw-r--r--   0        0        0   189316 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.data.json
+-rw-r--r--   0        0        0     1671 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.meta.json
+-rw-r--r--   0        0        0    57014 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.data.json
+-rw-r--r--   0        0        0     1711 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.meta.json
+-rw-r--r--   0        0        0    26727 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.data.json
+-rw-r--r--   0        0        0     1682 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.meta.json
+-rw-r--r--   0        0        0   110678 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1736 2024-05-30 10:56:00.328013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    27616 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/abc.data.json
+-rw-r--r--   0        0        0     1654 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/abc.meta.json
+-rw-r--r--   0        0        0  1646741 2024-05-30 10:56:00.368015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.data.json
+-rw-r--r--   0        0        0     1738 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.meta.json
+-rw-r--r--   0        0        0   129530 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.data.json
+-rw-r--r--   0        0        0     1722 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.meta.json
+-rw-r--r--   0        0        0   717970 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.data.json
+-rw-r--r--   0        0        0     1727 2024-05-30 10:56:00.318013 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3841 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.data.json
+-rw-r--r--   0        0        0     1638 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.meta.json
+-rw-r--r--   0        0        0   128242 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.data.json
+-rw-r--r--   0        0        0     1690 2024-05-30 10:56:00.298012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.meta.json
+-rw-r--r--   0        0        0    82332 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.data.json
+-rw-r--r--   0        0        0     1705 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.meta.json
+-rw-r--r--   0        0        0     7682 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.data.json
+-rw-r--r--   0        0        0     1690 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.meta.json
+-rw-r--r--   0        0        0    16410 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.data.json
+-rw-r--r--   0        0        0     1654 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.meta.json
+-rw-r--r--   0        0        0     7437 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1667 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25149 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.data.json
+-rw-r--r--   0        0        0     1639 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.meta.json
+-rw-r--r--   0        0        0     9370 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.data.json
+-rw-r--r--   0        0        0     1652 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.meta.json
+-rw-r--r--   0        0        0   101120 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.data.json
+-rw-r--r--   0        0        0     1755 2024-05-30 10:56:00.288012 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.meta.json
+-rw-r--r--   0        0        0    33224 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.data.json
+-rw-r--r--   0        0        0     1740 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.meta.json
+-rw-r--r--   0        0        0   114573 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/enum.data.json
+-rw-r--r--   0        0        0     1681 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/enum.meta.json
+-rw-r--r--   0        0        0    30200 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.data.json
+-rw-r--r--   0        0        0     1680 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.meta.json
+-rw-r--r--   0        0        0     6285 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1667 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    77616 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.data.json
+-rw-r--r--   0        0        0     1784 2024-05-30 10:56:00.278011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.meta.json
+-rw-r--r--   0        0        0    67076 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1773 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.meta.json
+-rw-r--r--   0        0        0   102899 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1811 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12631 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1655 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    90072 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/io.data.json
+-rw-r--r--   0        0        0     1724 2024-05-30 10:56:00.268011 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/io.meta.json
+-rw-r--r--   0        0        0     1547 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.data.json
+-rw-r--r--   0        0        0     1571 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.meta.json
+-rw-r--r--   0        0        0   398087 2024-05-30 10:56:00.258010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.data.json
+-rw-r--r--   0        0        0     1776 2024-05-30 10:56:00.258010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.meta.json
+-rw-r--r--   0        0        0     4928 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.data.json
+-rw-r--r--   0        0        0     1627 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.meta.json
+-rw-r--r--   0        0        0   107450 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.data.json
+-rw-r--r--   0        0        0     1733 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.meta.json
+-rw-r--r--   0        0        0   124441 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.data.json
+-rw-r--r--   0        0        0     1707 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.meta.json
+-rw-r--r--   0        0        0   243099 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/re.data.json
+-rw-r--r--   0        0        0     1752 2024-05-30 10:56:00.248010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/re.meta.json
+-rw-r--r--   0        0        0    14477 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.data.json
+-rw-r--r--   0        0        0     1652 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.meta.json
+-rw-r--r--   0        0        0    28934 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.data.json
+-rw-r--r--   0        0        0     1664 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.meta.json
+-rw-r--r--   0        0        0    50986 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.data.json
+-rw-r--r--   0        0        0     1707 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.meta.json
+-rw-r--r--   0        0        0   221898 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.data.json
+-rw-r--r--   0        0        0     1726 2024-05-30 10:56:00.238010 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.meta.json
+-rw-r--r--   0        0        0   156120 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sys.data.json
+-rw-r--r--   0        0        0     1740 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sys.meta.json
+-rw-r--r--   0        0        0   302750 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/types.data.json
+-rw-r--r--   0        0        0     1718 2024-05-30 10:56:00.228009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/types.meta.json
+-rw-r--r--   0        0        0   609850 2024-05-30 10:56:00.218009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing.data.json
+-rw-r--r--   0        0        0     1716 2024-05-30 10:56:00.218009 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing.meta.json
+-rw-r--r--   0        0        0    97019 2024-05-30 10:56:00.198008 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.data.json
+-rw-r--r--   0        0        0     1727 2024-05-30 10:56:00.198008 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.meta.json
+-rw-r--r--   0        0        0      190 2024-05-30 10:56:00.378015 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1873 2024-05-30 11:10:46.228764 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-30 10:56:24.676625 keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:55:43.636880 keyring_proxy_cli-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 keyring_proxy_cli-0.1.2/PKG-INFO
```

### Comparing `keyring_proxy_cli-0.1.1/pyproject.toml` & `keyring_proxy_cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "keyring-proxy-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Default template for PDM package"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
-    "keyring-proxy>=0.1.7",
+    "keyring-proxy>=0.1.8",
     "typer>=0.12.3",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/abc.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/abc.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/abc.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/abc.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/enum.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/enum.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/enum.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/enum.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/io.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/io.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/io.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/io.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/keyring_proxy_cli/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/re.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/re.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/re.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/re.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sys.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sys.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/sys.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/sys.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/types.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/types.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/types.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/types.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.data.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.meta.json` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/.mypy_cache/3.12/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `keyring_proxy_cli-0.1.1/src/keyring_proxy_cli/__init__.py` & `keyring_proxy_cli-0.1.2/src/keyring_proxy_cli/__init__.py`

 * *Files identical despite different names*

