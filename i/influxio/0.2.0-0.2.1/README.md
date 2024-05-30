# Comparing `tmp/influxio-0.2.0.tar.gz` & `tmp/influxio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxio-0.2.0.tar", last modified: Wed Apr 10 01:31:15 2024, max compression
+gzip compressed data, was "influxio-0.2.1.tar", last modified: Thu May 30 00:58:45 2024, max compression
```

## Comparing `influxio-0.2.0.tar` & `influxio-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.291934 influxio-0.2.0/
--rw-r--r--   0 amo        (501) staff       (20)      731 2024-04-10 01:30:29.000000 influxio-0.2.0/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)     1097 2023-03-11 00:48:15.000000 influxio-0.2.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)       79 2023-03-11 00:48:15.000000 influxio-0.2.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    12388 2024-04-10 01:31:15.291425 influxio-0.2.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     8997 2024-04-10 01:29:43.000000 influxio-0.2.0/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.278186 influxio-0.2.0/doc/
--rw-r--r--   0 amo        (501) staff       (20)     2781 2024-04-10 01:29:43.000000 influxio-0.2.0/doc/backlog.rst
--rw-r--r--   0 amo        (501) staff       (20)     2338 2024-04-07 22:18:58.000000 influxio-0.2.0/doc/development.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.282279 influxio-0.2.0/influxio/
--rw-r--r--   0 amo        (501) staff       (20)      110 2023-03-13 01:28:31.000000 influxio-0.2.0/influxio/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)    15584 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/adapter.py
--rw-r--r--   0 amo        (501) staff       (20)     4514 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     3354 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/core.py
--rw-r--r--   0 amo        (501) staff       (20)     4084 2024-04-07 22:18:58.000000 influxio-0.2.0/influxio/io.py
--rw-r--r--   0 amo        (501) staff       (20)     2325 2024-04-10 00:09:59.000000 influxio-0.2.0/influxio/model.py
--rw-r--r--   0 amo        (501) staff       (20)     2048 2024-02-14 23:51:01.000000 influxio-0.2.0/influxio/testdata.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.289047 influxio-0.2.0/influxio/util/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-10 22:36:39.000000 influxio-0.2.0/influxio/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1548 2023-03-11 00:20:47.000000 influxio-0.2.0/influxio/util/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     2101 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/util/common.py
--rw-r--r--   0 amo        (501) staff       (20)      328 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/compat.py
--rw-r--r--   0 amo        (501) staff       (20)      414 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/db.py
--rw-r--r--   0 amo        (501) staff       (20)     2605 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/report.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.289622 influxio-0.2.0/influxio.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    12388 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      554 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       46 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      419 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       15 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     5168 2024-04-09 23:21:05.000000 influxio-0.2.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-10 01:31:15.292020 influxio-0.2.0/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-30 00:58:45.285168 influxio-0.2.1/
+-rw-r--r--   0 amo        (501) staff       (20)      817 2024-05-30 00:58:11.000000 influxio-0.2.1/CHANGES.rst
+-rw-r--r--   0 amo        (501) staff       (20)     1097 2023-03-11 00:48:15.000000 influxio-0.2.1/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)       79 2023-03-11 00:48:15.000000 influxio-0.2.1/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    14434 2024-05-30 00:58:45.284690 influxio-0.2.1/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)    10180 2024-05-30 00:57:53.000000 influxio-0.2.1/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-30 00:58:45.263990 influxio-0.2.1/doc/
+-rw-r--r--   0 amo        (501) staff       (20)     2842 2024-05-07 22:19:25.000000 influxio-0.2.1/doc/backlog.rst
+-rw-r--r--   0 amo        (501) staff       (20)      817 2024-05-30 00:58:11.000000 influxio-0.2.1/doc/changes.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2369 2024-05-07 22:19:25.000000 influxio-0.2.1/doc/development.rst
+-rw-r--r--   0 amo        (501) staff       (20)    10180 2024-05-30 00:57:53.000000 influxio-0.2.1/doc/readme.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-30 00:58:45.270505 influxio-0.2.1/influxio/
+-rw-r--r--   0 amo        (501) staff       (20)      110 2023-03-13 01:28:31.000000 influxio-0.2.1/influxio/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)    15815 2024-05-30 00:57:53.000000 influxio-0.2.1/influxio/adapter.py
+-rw-r--r--   0 amo        (501) staff       (20)     4514 2024-04-10 01:29:43.000000 influxio-0.2.1/influxio/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     3354 2024-04-10 01:29:43.000000 influxio-0.2.1/influxio/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     4084 2024-04-07 22:18:58.000000 influxio-0.2.1/influxio/io.py
+-rw-r--r--   0 amo        (501) staff       (20)     2325 2024-04-10 00:09:59.000000 influxio-0.2.1/influxio/model.py
+-rw-r--r--   0 amo        (501) staff       (20)     2048 2024-02-14 23:51:01.000000 influxio-0.2.1/influxio/testdata.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-30 00:58:45.281648 influxio-0.2.1/influxio/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-10 22:36:39.000000 influxio-0.2.1/influxio/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1548 2023-03-11 00:20:47.000000 influxio-0.2.1/influxio/util/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     2101 2024-04-10 01:29:43.000000 influxio-0.2.1/influxio/util/common.py
+-rw-r--r--   0 amo        (501) staff       (20)      328 2023-11-12 01:46:47.000000 influxio-0.2.1/influxio/util/compat.py
+-rw-r--r--   0 amo        (501) staff       (20)      414 2023-11-12 01:46:47.000000 influxio-0.2.1/influxio/util/db.py
+-rw-r--r--   0 amo        (501) staff       (20)     2605 2023-11-12 01:46:47.000000 influxio-0.2.1/influxio/util/report.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-30 00:58:45.282163 influxio-0.2.1/influxio.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    14434 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      585 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       46 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      583 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       15 2024-05-30 00:58:45.000000 influxio-0.2.1/influxio.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     6098 2024-05-29 12:28:35.000000 influxio-0.2.1/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-05-30 00:58:45.285273 influxio-0.2.1/setup.cfg
```

### Comparing `influxio-0.2.0/CHANGES.rst` & `influxio-0.2.1/CHANGES.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-##################
-influxio changelog
-##################
+#########
+Changelog
+#########
 
 
 in progress
 ===========
 
+2024-05-30 v0.2.1
+=================
+- Fix CrateDB Cloud connectivity by propagating ``ssl=true`` query argument
+
 2024-04-10 v0.2.0
 =================
 - Export data from InfluxDB API and data directory into line protocol format
 
 2024-03-22 v0.1.2
 =================
 - Add support for Python 3.12
```

### Comparing `influxio-0.2.0/LICENSE` & `influxio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/PKG-INFO` & `influxio-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Import and export data into/from InfluxDB
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: changelog, https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/daq-tools/influxio
 Project-URL: homepage, https://github.com/daq-tools/influxio
 Project-URL: repository, https://github.com/daq-tools/influxio
@@ -32,20 +32,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Database
 Classifier: Topic :: Documentation
 Classifier: Topic :: Education
+Classifier: Topic :: File Formats
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click<9
@@ -60,19 +68,28 @@
 Requires-Dist: pandas<2.3
 Requires-Dist: psycopg2-binary<3
 Requires-Dist: pueblo>=0.0.7
 Requires-Dist: SQLAlchemy-Utils<0.42
 Requires-Dist: yarl<2
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
-Requires-Dist: mypy==1.9.0; extra == "develop"
-Requires-Dist: poethepoet<0.26; extra == "develop"
-Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff==0.3.5; extra == "develop"
-Requires-Dist: validate-pyproject<0.17; extra == "develop"
+Requires-Dist: mypy<1.11; extra == "develop"
+Requires-Dist: poethepoet<0.27; extra == "develop"
+Requires-Dist: pyproject-fmt<2.2; extra == "develop"
+Requires-Dist: ruff<0.5; extra == "develop"
+Requires-Dist: sphinx-autobuild==2021.3.14; extra == "develop"
+Requires-Dist: validate-pyproject<0.19; extra == "develop"
+Provides-Extra: docs
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: myst-parser[linkify]<4,>=0.18; extra == "docs"
+Requires-Dist: sphinx<8; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx-design-elements<1; extra == "docs"
+Requires-Dist: sphinxcontrib-mermaid<1; extra == "docs"
+Requires-Dist: sphinxext-opengraph<1; extra == "docs"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
 Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-cov<6; extra == "test"
 
@@ -113,14 +130,34 @@
 .. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
 .. end-badges
 
 
+.. start-links
+
+» `Documentation <project-documentation_>`_
+| `Changelog <project-changelog_>`_
+| `PyPI <project-pypi_>`_
+| `Issues <project-issues_>`_
+| `Source code <project-source_>`_
+| `License <project-license_>`_
+
+.. end-links
+
+
+.. _project-documentation: https://influxio.readthedocs.io
+.. _project-changelog: https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
+.. _project-pypi: https://pypi.org/project/influxio/
+.. _project-issues: https://github.com/daq-tools/influxio/issues
+.. _project-source: https://github.com/daq-tools/influxio
+.. _project-license: https://github.com/daq-tools/influxio/blob/main/LICENSE
+
+
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
@@ -265,14 +302,27 @@
         "file://export.lp"
 
     # From API to line protocol on stdout.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://-?format=lp"
 
+Export from Cloud to Cloud
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB Cloud to CrateDB Cloud.
+    influxio copy \
+        "https://8e9ec869a91a3517:T268DVLDHD8AJsjzOEluu...Pic4A==@eu-central-1-1.aws.cloud2.influxdata.com/testdrive/demo" \
+        "crate://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200/testdrive/demo?ssl=true"
+
+    crash \
+        --hosts 'https://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200' \
+        --command 'SELECT * FROM testdrive.demo;'
 
 Export from data directory
 --------------------------
 
 .. code-block:: shell
 
     # From InfluxDB data directory to line protocol file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `influxio-0.2.0/README.rst` & `influxio-0.2.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,34 @@
 .. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
 .. end-badges
 
 
+.. start-links
+
+» `Documentation <project-documentation_>`_
+| `Changelog <project-changelog_>`_
+| `PyPI <project-pypi_>`_
+| `Issues <project-issues_>`_
+| `Source code <project-source_>`_
+| `License <project-license_>`_
+
+.. end-links
+
+
+.. _project-documentation: https://influxio.readthedocs.io
+.. _project-changelog: https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
+.. _project-pypi: https://pypi.org/project/influxio/
+.. _project-issues: https://github.com/daq-tools/influxio/issues
+.. _project-source: https://github.com/daq-tools/influxio
+.. _project-license: https://github.com/daq-tools/influxio/blob/main/LICENSE
+
+
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
@@ -187,14 +207,27 @@
         "file://export.lp"
 
     # From API to line protocol on stdout.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://-?format=lp"
 
+Export from Cloud to Cloud
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB Cloud to CrateDB Cloud.
+    influxio copy \
+        "https://8e9ec869a91a3517:T268DVLDHD8AJsjzOEluu...Pic4A==@eu-central-1-1.aws.cloud2.influxdata.com/testdrive/demo" \
+        "crate://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200/testdrive/demo?ssl=true"
+
+    crash \
+        --hosts 'https://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200' \
+        --command 'SELECT * FROM testdrive.demo;'
 
 Export from data directory
 --------------------------
 
 .. code-block:: shell
 
     # From InfluxDB data directory to line protocol file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `influxio-0.2.0/doc/backlog.rst` & `influxio-0.2.1/doc/backlog.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-################
-influxio backlog
-################
+#######
+Backlog
+#######
 
 
 ************
 Iteration +1
 ************
 - [o] README: Demonstrate "library use"
 - [o] README: Caveat about overwrite protection
@@ -23,19 +23,21 @@
 
 
 ************
 Iteration +2
 ************
 - [o] Fix ``cratedb_toolkit.sqlalchemy.patch_inspector()`` re. reflection of ``?schema=`` URL parameter
 - [o] Fix ``crate.client.sqlalchemy.dialect.DateTime`` re. ``TimezoneUnawareException``
-- [o] Support InfluxDB 1.x
+- [o] Support InfluxDB 1.x and 3.x
 - [o] Add Docker Compose file for auxiliary services
 - [o] Refactor general purpose code to ``pueblo`` package
 - [o] Verify import and export of ILP and CSV files works well
 - [o] Tests using ``assert_dataframe_equal``? Maybe in ``cratedb-toolkit``?
+- [o] fluXpipe adapter
+  https://github.com/crate/crate-clients-tools/issues/94
 
 
 ************
 Iteration +3
 ************
 - [o] Unlock more parameters in InfluxDbApiAdapter.write_df
 - [o] Format: Compressed line protocol
```

### Comparing `influxio-0.2.0/doc/development.rst` & `influxio-0.2.1/doc/development.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. _development:
+.. _sandbox:
+
 ###########
 Development
 ###########
 
 
 *******
 Sandbox
```

### Comparing `influxio-0.2.0/influxio/adapter.py` & `influxio-0.2.1/influxio/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,17 +272,22 @@
             url: URL = URL(url)
 
         self.database, self.table = SqlAlchemyAdapter.decode_database_table(url)
 
         # Special handling for SQLite and CrateDB databases.
         self.dburi = str(url.with_query(None))
         if url.scheme == "crate":
+            query_args_passthrough = ["ssl"]
+            query = url.query
             url = url.with_path("")
             if self.database:
-                url = url.with_query({"schema": self.database})
+                url = url.update_query({"schema": self.database})
+                for arg in query_args_passthrough:
+                    if arg in query:
+                        url = url.update_query({arg: query[arg]})
             self.dburi = str(url)
         elif url.scheme == "sqlite":
             self.dburi = self.dburi.replace("sqlite:/", "sqlite:///")
         else:
             url = url.with_path(self.database)
             self.dburi = str(url)
```

### Comparing `influxio-0.2.0/influxio/cli.py` & `influxio-0.2.1/influxio/cli.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/core.py` & `influxio-0.2.1/influxio/core.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/io.py` & `influxio-0.2.1/influxio/io.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/model.py` & `influxio-0.2.1/influxio/model.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/testdata.py` & `influxio-0.2.1/influxio/testdata.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/util/cli.py` & `influxio-0.2.1/influxio/util/cli.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/util/common.py` & `influxio-0.2.1/influxio/util/common.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio/util/report.py` & `influxio-0.2.1/influxio/util/report.py`

 * *Files identical despite different names*

### Comparing `influxio-0.2.0/influxio.egg-info/PKG-INFO` & `influxio-0.2.1/influxio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Import and export data into/from InfluxDB
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: changelog, https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/daq-tools/influxio
 Project-URL: homepage, https://github.com/daq-tools/influxio
 Project-URL: repository, https://github.com/daq-tools/influxio
@@ -32,20 +32,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Database
 Classifier: Topic :: Documentation
 Classifier: Topic :: Education
+Classifier: Topic :: File Formats
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click<9
@@ -60,19 +68,28 @@
 Requires-Dist: pandas<2.3
 Requires-Dist: psycopg2-binary<3
 Requires-Dist: pueblo>=0.0.7
 Requires-Dist: SQLAlchemy-Utils<0.42
 Requires-Dist: yarl<2
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
-Requires-Dist: mypy==1.9.0; extra == "develop"
-Requires-Dist: poethepoet<0.26; extra == "develop"
-Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff==0.3.5; extra == "develop"
-Requires-Dist: validate-pyproject<0.17; extra == "develop"
+Requires-Dist: mypy<1.11; extra == "develop"
+Requires-Dist: poethepoet<0.27; extra == "develop"
+Requires-Dist: pyproject-fmt<2.2; extra == "develop"
+Requires-Dist: ruff<0.5; extra == "develop"
+Requires-Dist: sphinx-autobuild==2021.3.14; extra == "develop"
+Requires-Dist: validate-pyproject<0.19; extra == "develop"
+Provides-Extra: docs
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: myst-parser[linkify]<4,>=0.18; extra == "docs"
+Requires-Dist: sphinx<8; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx-design-elements<1; extra == "docs"
+Requires-Dist: sphinxcontrib-mermaid<1; extra == "docs"
+Requires-Dist: sphinxext-opengraph<1; extra == "docs"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
 Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-cov<6; extra == "test"
 
@@ -113,14 +130,34 @@
 .. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
 .. end-badges
 
 
+.. start-links
+
+» `Documentation <project-documentation_>`_
+| `Changelog <project-changelog_>`_
+| `PyPI <project-pypi_>`_
+| `Issues <project-issues_>`_
+| `Source code <project-source_>`_
+| `License <project-license_>`_
+
+.. end-links
+
+
+.. _project-documentation: https://influxio.readthedocs.io
+.. _project-changelog: https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
+.. _project-pypi: https://pypi.org/project/influxio/
+.. _project-issues: https://github.com/daq-tools/influxio/issues
+.. _project-source: https://github.com/daq-tools/influxio
+.. _project-license: https://github.com/daq-tools/influxio/blob/main/LICENSE
+
+
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
@@ -265,14 +302,27 @@
         "file://export.lp"
 
     # From API to line protocol on stdout.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://-?format=lp"
 
+Export from Cloud to Cloud
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB Cloud to CrateDB Cloud.
+    influxio copy \
+        "https://8e9ec869a91a3517:T268DVLDHD8AJsjzOEluu...Pic4A==@eu-central-1-1.aws.cloud2.influxdata.com/testdrive/demo" \
+        "crate://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200/testdrive/demo?ssl=true"
+
+    crash \
+        --hosts 'https://admin:dZ,Y18*Z...7)6LqB@green-shaak-ti.eks1.eu-west-1.aws.cratedb.net:4200' \
+        --command 'SELECT * FROM testdrive.demo;'
 
 Export from data directory
 --------------------------
 
 .. code-block:: shell
 
     # From InfluxDB data directory to line protocol file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `influxio-0.2.0/influxio.egg-info/SOURCES.txt` & `influxio-0.2.1/influxio.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 doc/backlog.rst
+doc/changes.rst
 doc/development.rst
+doc/readme.rst
 influxio/__init__.py
 influxio/adapter.py
 influxio/cli.py
 influxio/core.py
 influxio/io.py
 influxio/model.py
 influxio/testdata.py
```

### Comparing `influxio-0.2.0/pyproject.toml` & `influxio-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -58,20 +58,28 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Communications",
   "Topic :: Database",
   "Topic :: Documentation",
   "Topic :: Education",
+  "Topic :: File Formats",
   "Topic :: Office/Business",
   "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Human Machine Interfaces",
+  "Topic :: Scientific/Engineering :: Information Analysis",
+  "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing",
   "Topic :: Software Development :: Version Control",
   "Topic :: System :: Archiving",
+  "Topic :: System :: Logging",
+  "Topic :: System :: Monitoring",
+  "Topic :: System :: Networking",
+  "Topic :: System :: Recovery Tools",
   "Topic :: System :: Systems Administration",
   "Topic :: Text Processing",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
@@ -90,19 +98,29 @@
   "pueblo>=0.0.7",
   "SQLAlchemy-Utils<0.42",
   "yarl<2",
 ]
 [project.optional-dependencies]
 develop = [
   "black<25",
-  "mypy==1.9.0",
-  "poethepoet<0.26",
-  "pyproject-fmt<1.8",
-  "ruff==0.3.5",
-  "validate-pyproject<0.17",
+  "mypy<1.11",
+  "poethepoet<0.27",
+  "pyproject-fmt<2.2",
+  "ruff<0.5",
+  "sphinx-autobuild==2021.3.14", # Newer versions stopped "watching" appropriately?
+  "validate-pyproject<0.19",
+]
+docs = [
+  "furo",
+  "myst-parser[linkify]>=0.18,<4",
+  "sphinx<8",
+  "sphinx-copybutton",
+  "sphinx-design-elements<1",
+  "sphinxcontrib-mermaid<1",
+  "sphinxext-opengraph<1",
 ]
 release = [
   "build<2",
   "twine<6",
 ]
 test = [
   "pytest<9",
@@ -192,14 +210,15 @@
   # Unnecessary variable assignment before `return` statement
   "RET504",
   # Unnecessary `elif` after `return` statement
   "RET505",
 ]
 
 [tool.ruff.lint.per-file-ignores]
+"doc/conf.py" = ["A001", "ERA001"]
 "tests/*" = ["S101"]  # Use of `assert` detected
 "influxio/util/report.py" = ["T201"]
 
 [tool.setuptools.packages.find]
 namespaces = false
 
 
@@ -210,14 +229,24 @@
 [tool.poe.tasks]
 
 check = [
   "lint",
   "test",
 ]
 
+docs-autobuild = [
+  { cmd = "sphinx-autobuild --open-browser --watch influxio doc doc/_build" }
+]
+docs-html = [
+  { cmd = "sphinx-build -W --keep-going doc doc/_build" }
+]
+docs-linkcheck = [
+  { cmd = "sphinx-build -W --keep-going -b linkcheck doc doc/_build" }
+]
+
 format = [
   { cmd = "black ." },
   # Configure Ruff not to auto-fix (remove!) unused variables (F841) and `print` statements (T201).
   { cmd = "ruff check --fix --ignore=ERA --ignore=F401 --ignore=F841 --ignore=T20 ." },
   { cmd = "pyproject-fmt --keep-full-version pyproject.toml" },
 ]
```

