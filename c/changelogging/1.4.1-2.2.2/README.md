# Comparing `tmp/changelogging-1.4.1.tar.gz` & `tmp/changelogging-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelogging-1.4.1.tar", max compression
+gzip compressed data
```

## Comparing `changelogging-1.4.1.tar` & `changelogging-2.2.2.tar`

### file list

```diff
@@ -1,15 +1,52 @@
--rw-r--r--   0        0        0     1092 2024-02-26 12:12:23.336150 changelogging-1.4.1/LICENSE
--rw-r--r--   0        0        0     3096 2024-02-26 12:12:23.336150 changelogging-1.4.1/README.md
--rw-r--r--   0        0        0      517 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/__init__.py
--rw-r--r--   0        0        0      122 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/__main__.py
--rw-r--r--   0        0        0     9826 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/build.py
--rw-r--r--   0        0        0      810 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/changelogging.toml
--rw-r--r--   0        0        0    13702 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/config.py
--rw-r--r--   0        0        0      645 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/constants.py
--rw-r--r--   0        0        0     5937 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/fragments.py
--rw-r--r--   0        0        0      797 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/git.py
--rw-r--r--   0        0        0     2966 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/main.py
--rw-r--r--   0        0        0        0 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/py.typed
--rw-r--r--   0        0        0      899 2024-02-26 12:12:23.336150 changelogging-1.4.1/changelogging/utils.py
--rw-r--r--   0        0        0     2802 2024-02-26 12:12:23.340149 changelogging-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 changelogging-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 changelogging-2.2.2/Cargo.toml
+-rw-r--r--   0     1001      127      200 2024-05-30 12:18:52.000000 changelogging-2.2.2/.editorconfig
+-rw-r--r--   0     1001      127       75 2024-05-30 12:18:52.000000 changelogging-2.2.2/.gitattributes
+-rw-r--r--   0     1001      127       12 2024-05-30 12:18:52.000000 changelogging-2.2.2/.github/CODEOWNERS
+-rw-r--r--   0     1001      127       53 2024-05-30 12:18:52.000000 changelogging-2.2.2/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      409 2024-05-30 12:18:52.000000 changelogging-2.2.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     9807 2024-05-30 12:18:52.000000 changelogging-2.2.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      453 2024-05-30 12:18:52.000000 changelogging-2.2.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127       20 2024-05-30 12:18:52.000000 changelogging-2.2.2/.gitignore
+-rw-r--r--   0     1001      127      868 2024-05-30 12:18:52.000000 changelogging-2.2.2/CHANGELOG.md
+-rw-r--r--   0     1001      127     5486 2024-05-30 12:18:52.000000 changelogging-2.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127        0 2024-05-30 12:18:52.000000 changelogging-2.2.2/CONTRIBUTING.md
+-rw-r--r--   0     1001      127    25102 2024-05-30 12:18:56.000000 changelogging-2.2.2/Cargo.lock
+-rw-r--r--   0     1001      127     1092 2024-05-30 12:18:52.000000 changelogging-2.2.2/LICENSE
+-rw-r--r--   0     1001      127     3892 2024-05-30 12:18:52.000000 changelogging-2.2.2/README.md
+-rw-r--r--   0     1001      127     5442 2024-05-30 12:18:52.000000 changelogging-2.2.2/SECURITY.md
+-rw-r--r--   0     1001      127     6183 2024-05-30 12:18:52.000000 changelogging-2.2.2/changelogging.schema.json
+-rw-r--r--   0     1001      127     2493 2024-05-30 12:18:52.000000 changelogging-2.2.2/changelogging.svg
+-rw-r--r--   0     1001      127      232 2024-05-30 12:18:52.000000 changelogging-2.2.2/changelogging.toml
+-rw-r--r--   0     1001      127       12 2024-05-30 12:18:52.000000 changelogging-2.2.2/changes/.gitignore
+-rw-r--r--   0     1001      127      410 2024-05-30 12:18:52.000000 changelogging-2.2.2/examples/CHANGELOG.md
+-rw-r--r--   0     1001      127       43 2024-05-30 12:18:52.000000 changelogging-2.2.2/examples/TEMPLATE.md
+-rw-r--r--   0     1001      127     8239 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/app.rs
+-rw-r--r--   0     1001      127    21969 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/builder.rs
+-rw-r--r--   0     1001      127     3070 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/commands/build.rs
+-rw-r--r--   0     1001      127     5003 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/commands/create.rs
+-rw-r--r--   0     1001      127       82 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/commands/mod.rs
+-rw-r--r--   0     1001      127     2142 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/commands/preview.rs
+-rw-r--r--   0     1001      127     9619 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/config.rs
+-rw-r--r--   0     1001      127      918 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/context.rs
+-rw-r--r--   0     1001      127     1277 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/date.rs
+-rw-r--r--   0     1001      127      501 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/defaults.toml
+-rw-r--r--   0     1001      127     5721 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/discover.rs
+-rw-r--r--   0     1001      127     8667 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/fragment.rs
+-rw-r--r--   0     1001      127     1547 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/git.rs
+-rw-r--r--   0     1001      127     2610 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/init.rs
+-rw-r--r--   0     1001      127     5276 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/lib.rs
+-rw-r--r--   0     1001      127      166 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/main.rs
+-rw-r--r--   0     1001      127     2622 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/options.rs
+-rw-r--r--   0     1001      127     4975 2024-05-30 12:18:52.000000 changelogging-2.2.2/src/workspace.rs
+-rw-r--r--   0     1001      127      102 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/TEMPLATE.md
+-rw-r--r--   0     1001      127      232 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changelogging.toml
+-rw-r--r--   0     1001      127       12 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/.gitignore
+-rw-r--r--   0     1001      127       21 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/13.feature.md
+-rw-r--r--   0     1001      127       21 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/22.change.md
+-rw-r--r--   0     1001      127       19 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/34.fix.md
+-rw-r--r--   0     1001      127       24 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/42.deprecation.md
+-rw-r--r--   0     1001      127       79 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/64.security.md
+-rw-r--r--   0     1001      127       21 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/69.removal.md
+-rw-r--r--   0     1001      127       28 2024-05-30 12:18:52.000000 changelogging-2.2.2/tests/changes/96.internal.md
+-rw-r--r--   0     1001      127     1233 2024-05-30 12:18:52.000000 changelogging-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 changelogging-2.2.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `changelogging-1.4.1/LICENSE` & `changelogging-2.2.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-present, Nikita Tikhonov (nekitdev)
+Copyright (c) 2024-present, Nikita Tikhonov (nekitdev)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `changelogging-1.4.1/PKG-INFO` & `changelogging-2.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,149 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: changelogging
-Version: 1.4.1
-Summary: Building changelogs from fragments.
-Home-page: https://github.com/nekitdev/changelogging
-License: MIT
-Keywords: python,changelog,changes
-Author: nekitdev
-Requires-Python: >=3.8
+Version: 2.2.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Dist: attrs (>=23.2.0)
-Requires-Dist: click (>=8.1.7)
-Requires-Dist: entrypoint (>=2.0.2)
-Requires-Dist: funcs (>=0.9.1)
-Requires-Dist: iters (>=0.16.1)
-Requires-Dist: pendulum (>=3.0.0)
-Requires-Dist: toml (>=0.10.2)
-Requires-Dist: typing-aliases (>=1.7.1)
-Requires-Dist: typing-extensions (>=4.10.0)
-Requires-Dist: versions (>=2.1.2)
-Requires-Dist: wraps (>=0.9.1)
-Requires-Dist: yarl (>=1.9.4)
+License-File: LICENSE
+Summary: Building changelogs from fragments.
+Keywords: changelog,changes
+Author: nekitdev <nekit@nekit.dev>
+Author-email: nekitdev <nekit@nekit.dev>
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/nekitdev/changelogging
 Project-URL: Chat, https://nekit.dev/chat
-Project-URL: Documentation, https://nekitdev.github.io/changelogging
+Project-URL: Documentation, https://docs.rs/changelogging
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/changelogging/issues
 Project-URL: Repository, https://github.com/nekitdev/changelogging
-Description-Content-Type: text/markdown
+
+![Image]
 
 # `changelogging`
 
 [![License][License Badge]][License]
 [![Version][Version Badge]][Package]
 [![Downloads][Downloads Badge]][Package]
 [![Discord][Discord Badge]][Discord]
-
-[![Documentation][Documentation Badge]][Documentation]
-[![Check][Check Badge]][Actions]
 [![Test][Test Badge]][Actions]
-[![Coverage][Coverage Badge]][Coverage]
 
 > *Building changelogs from fragments.*
 
 ## Installing
 
-**Python 3.8 or above is required.**
+Installing the crate with `cargo` is quite simple:
 
-### pip
+```console
+$ cargo install changelogging
+```
 
-Installing the library with `pip` is quite simple:
+Alternatively, the crate can be installed from source:
 
 ```console
-$ pip install changelogging
+$ cargo install --git https://github.com/nekitdev/changelogging.git
 ```
 
-Alternatively, the library can be installed from source:
+Or via cloning the repository:
 
 ```console
 $ git clone https://github.com/nekitdev/changelogging.git
 $ cd changelogging
-$ python -m pip install .
+$ cargo install --path .
 ```
 
-### poetry
+The binaries can be downloaded from [releases][Releases].
+
+## Example
+
+Once `changelogging` is installed, we can start building changelogs!
 
-You can add `changelogging` as a dependency with the following command:
+First things first, we need to configure the *context* of the project.
+
+Create `changelogging.toml` and add the *name*, *version* and *URL* of the project:
+
+```toml
+[context]
+name = "changelogging"
+version = "0.2.2"
+url = "https://github.com/nekitdev/changelogging"
+```
+
+Then we need to create the `changes` directory.
 
 ```console
-$ poetry add changelogging
+$ mkdir changes
 ```
 
-Or by directly specifying it in the configuration like so:
+Now we can add *fragments*:
 
-```toml
-[tool.poetry.dependencies]
-changelogging = "^1.4.1"
+```console
+$ changelogging create --content "Added cool features!" 13.feature.md
+$ changelogging create --content "Fixed annoying bugs!" 64.fix.md
 ```
 
-Alternatively, you can add it directly from the source:
+And finally, preview the changelog entry!
 
-```toml
-[tool.poetry.dependencies.changelogging]
-git = "https://github.com/nekitdev/changelogging.git"
+```console
+$ changelogging preview
+## 0.2.2 (YYYY-MM-DD)
+
+### Features
+
+- Added cool features! (#13)
+
+### Fixes
+
+- Fixed annoying bugs! (#64)
+```
+
+Then let us add our `CHANGELOG.md` file with the following content:
+
+```md
+# Changelog
+
+<!-- changelogging: start -->
+```
+
+Note that the `start` is essential if we want to add some content before the changelog entries.
+
+Assuming the preview is what we expected it to be, writing it to the changelog is as simple as:
+
+```console
+$ changelogging build
+```
+
+Finally, let's see the changelog:
+
+```console
+$ cat CHANGELOG.md
+# Changelog
+
+<!-- changelogging: start -->
+
+## 0.2.2 (YYYY-MM-DD)
+
+### Features
+
+- Added cool features! (#13)
+
+### Fixes
+
+- Fixed annoying bugs! (#64)
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
@@ -116,34 +164,32 @@
 If you are interested in contributing to `changelogging`, make sure to take a look at the
 [Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
 
 ## License
 
 `changelogging` is licensed under the MIT License terms. See [License][License] for details.
 
+[Image]: https://github.com/nekitdev/changelogging/blob/main/changelogging.svg?raw=true
+
 [Email]: mailto:support@nekit.dev
 
 [Discord]: https://nekit.dev/chat
 
 [Actions]: https://github.com/nekitdev/changelogging/actions
+[Releases]: https://github.com/nekitdev/changelogging/releases
 
 [Changelog]: https://github.com/nekitdev/changelogging/blob/main/CHANGELOG.md
 [Code of Conduct]: https://github.com/nekitdev/changelogging/blob/main/CODE_OF_CONDUCT.md
 [Contributing Guide]: https://github.com/nekitdev/changelogging/blob/main/CONTRIBUTING.md
 [Security]: https://github.com/nekitdev/changelogging/blob/main/SECURITY.md
 
 [License]: https://github.com/nekitdev/changelogging/blob/main/LICENSE
 
-[Package]: https://pypi.org/project/changelogging
-[Coverage]: https://codecov.io/gh/nekitdev/changelogging
-[Documentation]: https://nekitdev.github.io/changelogging
+[Package]: https://crates.io/crates/changelogging
+[Documentation]: https://docs.rs/changelogging
 
 [Discord Badge]: https://img.shields.io/discord/728012506899021874
-[License Badge]: https://img.shields.io/pypi/l/changelogging
-[Version Badge]: https://img.shields.io/pypi/v/changelogging
-[Downloads Badge]: https://img.shields.io/pypi/dm/changelogging
-
-[Documentation Badge]: https://github.com/nekitdev/changelogging/workflows/docs/badge.svg
-[Check Badge]: https://github.com/nekitdev/changelogging/workflows/check/badge.svg
+[License Badge]: https://img.shields.io/crates/l/changelogging
+[Version Badge]: https://img.shields.io/crates/v/changelogging
+[Downloads Badge]: https://img.shields.io/crates/dr/changelogging
 [Test Badge]: https://github.com/nekitdev/changelogging/workflows/test/badge.svg
-[Coverage Badge]: https://codecov.io/gh/nekitdev/changelogging/branch/main/graph/badge.svg
```

