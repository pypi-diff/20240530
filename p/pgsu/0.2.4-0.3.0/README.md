# Comparing `tmp/pgsu-0.2.4.tar.gz` & `tmp/pgsu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgsu-0.2.4.tar", last modified: Tue Jul 11 04:17:02 2023, max compression
+gzip compressed data, was "pgsu-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pgsu-0.2.4.tar` & `pgsu-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 04:16:52.000000 pgsu-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 04:16:52.000000 pgsu-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-11 04:17:02.484777 pgsu-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-11 04:16:52.000000 pgsu-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/pgsu/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-07-11 04:16:52.000000 pgsu-0.2.4/pgsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 04:16:52.000000 pgsu-0.2.4/pgsu/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/pgsu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 04:17:02.000000 pgsu-0.2.4/pgsu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 04:16:52.000000 pgsu-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-11 04:17:02.484777 pgsu-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 04:16:52.000000 pgsu-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:17:02.484777 pgsu-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_pgtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-11 04:16:52.000000 pgsu-0.2.4/tests/test_sql.py
+-rw-r--r--   0        0        0     1072 2024-05-30 18:50:33.927497 pgsu-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3195 2024-05-30 18:50:33.927497 pgsu-0.3.0/README.md
+-rw-r--r--   0        0        0    14836 2024-05-30 18:50:33.927497 pgsu-0.3.0/pgsu/__init__.py
+-rw-r--r--   0        0        0      469 2024-05-30 18:50:33.927497 pgsu-0.3.0/pgsu/cli.py
+-rw-r--r--   0        0        0     1638 2024-05-30 18:50:33.927497 pgsu-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      387 2024-05-30 18:50:33.931497 pgsu-0.3.0/tox.ini
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 pgsu-0.3.0/PKG-INFO
```

### Comparing `pgsu-0.2.4/LICENSE` & `pgsu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgsu-0.2.4/PKG-INFO` & `pgsu-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 Metadata-Version: 2.1
 Name: pgsu
-Version: 0.2.4
-Summary: Connect to an existing PostgreSQL cluster as a postgres superuser and execute SQL commands.
-Home-page: https://github.com/aiidateam/pgsu
-Author: AiiDA Team
-Author-email: aiidateam@gmail.com
-License: MIT
+Version: 0.3.0
+Summary: Connect to an existing PostgreSQL cluster as the `postgres` superuser and execute SQL commands.
+Author-email: AiiDA Team <aiidateam@gmail.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: pre_commit
-Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: psycopg[binary]>=3.0
+Requires-Dist: pre-commit~=2.2 ; extra == "dev"
+Requires-Dist: pylint~=2.5.0 ; extra == "dev"
+Requires-Dist: pgtest>=1.3.1 ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Project-URL: homepage, https://github.com/aiidateam/pgsu
+Project-URL: source, https://github.com/aiidateam/pgsu
+Project-URL: tracker, https://github.com/aiidateam/pgsu/issues
+Provides-Extra: dev
 
 [![Build Status](https://github.com/aiidateam/pgsu/workflows/ci/badge.svg)](https://github.com/aiidateam/pgsu/actions)
 [![Coverage Status](https://codecov.io/gh/aiidateam/pgsu/branch/master/graph/badge.svg)](https://codecov.io/gh/aiidateam/pgsu)
 [![PyPI version](https://badge.fury.io/py/pgsu.svg)](https://badge.fury.io/py/pgsu)
 [![GitHub license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/aiidateam/pgsu/blob/master/LICENSE)
 # pgsu
 
 Connect to an existing PostgreSQL cluster as a PostgreSQL [SUPERUSER](https://www.postgresql.org/docs/current/sql-createrole.html) and execute SQL commands.
 
-[`psycopg2`](https://pypi.org/project/psycopg2/) has a great API for interacting with PostgreSQL, once you provide it with the connection parameters for a given database.
+[`psycopg`](https://pypi.org/project/psycopg/) has a great API for interacting with PostgreSQL, once you provide it with the connection parameters for a given database.
 However, what if your desired database and database user do not yet exist?
 In order to create them, you will need to connect to PostgreSQL as a SUPERUSER.
 
 ## Features
 
  * autodetects postgres setup, tested on
+   * [Ubuntu 22.04](https://github.com/actions/virtual-environments/blob/main/images/linux/Ubuntu2204-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 20.04](https://github.com/actions/virtual-environments/blob/main/images/linux/Ubuntu2004-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 16.04](https://github.com/actions/virtual-environments/blob/master/images/linux/Ubuntu1604-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 18.04](https://github.com/actions/virtual-environments/blob/master/images/linux/Ubuntu1804-README.md) & PostgreSQL docker container
    * [MacOS 12](https://github.com/actions/virtual-environments/blob/master/images/macos/macos-12-Readme.md) and PostgreSQL installed via `conda`
    * [Windows Server 2019](https://github.com/actions/virtual-environments/blob/master/images/win/Windows2019-Readme.md) and PostgreSQL installed via `conda`
- * uses [psycopg2](http://initd.org/psycopg/docs/index.html) to connect if possible
+ * uses [psycopg](http://initd.org/psycopg/docs/index.html) to connect if possible
  * can use `sudo` to become the `postgres` UNIX user if necessary/possible (default Ubuntu PostgreSQL setups)
 
 ## Usage
 
 ### Python API
 ```python
 from pgsu import PGSU
@@ -63,15 +70,15 @@
 ```python
 from pgsu import PGSU
 pgsu = PGSU(dsn={
     'host': None,
     'port': 5432,
     'user': 'postgres',
     'password': None,
-    'database': 'template1',  # Note: you cannot drop databases you are connected to
+    'dbname': 'template1',  # Note: you cannot drop databases you are connected to
 })
 ```
 
 ### Command line tool
 
 The package also comes with a very basic `pgsu` command line tool that allows users to execute PostgreSQL commands as the superuser:
 ```
@@ -82,10 +89,11 @@
  ('postgres',)]
 ```
 
 ## Tests
 
 Run the tests as follows:
 ```bash
-pip install -e .[testing]
+pip install -e .[dev]
 pytest
 ```
+
```

### Comparing `pgsu-0.2.4/README.md` & `pgsu-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 [![Coverage Status](https://codecov.io/gh/aiidateam/pgsu/branch/master/graph/badge.svg)](https://codecov.io/gh/aiidateam/pgsu)
 [![PyPI version](https://badge.fury.io/py/pgsu.svg)](https://badge.fury.io/py/pgsu)
 [![GitHub license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/aiidateam/pgsu/blob/master/LICENSE)
 # pgsu
 
 Connect to an existing PostgreSQL cluster as a PostgreSQL [SUPERUSER](https://www.postgresql.org/docs/current/sql-createrole.html) and execute SQL commands.
 
-[`psycopg2`](https://pypi.org/project/psycopg2/) has a great API for interacting with PostgreSQL, once you provide it with the connection parameters for a given database.
+[`psycopg`](https://pypi.org/project/psycopg/) has a great API for interacting with PostgreSQL, once you provide it with the connection parameters for a given database.
 However, what if your desired database and database user do not yet exist?
 In order to create them, you will need to connect to PostgreSQL as a SUPERUSER.
 
 ## Features
 
  * autodetects postgres setup, tested on
+   * [Ubuntu 22.04](https://github.com/actions/virtual-environments/blob/main/images/linux/Ubuntu2204-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 20.04](https://github.com/actions/virtual-environments/blob/main/images/linux/Ubuntu2004-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 16.04](https://github.com/actions/virtual-environments/blob/master/images/linux/Ubuntu1604-README.md) & PostgreSQL installed via `apt`
    * [Ubuntu 18.04](https://github.com/actions/virtual-environments/blob/master/images/linux/Ubuntu1804-README.md) & PostgreSQL docker container
    * [MacOS 12](https://github.com/actions/virtual-environments/blob/master/images/macos/macos-12-Readme.md) and PostgreSQL installed via `conda`
    * [Windows Server 2019](https://github.com/actions/virtual-environments/blob/master/images/win/Windows2019-Readme.md) and PostgreSQL installed via `conda`
- * uses [psycopg2](http://initd.org/psycopg/docs/index.html) to connect if possible
+ * uses [psycopg](http://initd.org/psycopg/docs/index.html) to connect if possible
  * can use `sudo` to become the `postgres` UNIX user if necessary/possible (default Ubuntu PostgreSQL setups)
 
 ## Usage
 
 ### Python API
 ```python
 from pgsu import PGSU
@@ -37,15 +38,15 @@
 ```python
 from pgsu import PGSU
 pgsu = PGSU(dsn={
     'host': None,
     'port': 5432,
     'user': 'postgres',
     'password': None,
-    'database': 'template1',  # Note: you cannot drop databases you are connected to
+    'dbname': 'template1',  # Note: you cannot drop databases you are connected to
 })
 ```
 
 ### Command line tool
 
 The package also comes with a very basic `pgsu` command line tool that allows users to execute PostgreSQL commands as the superuser:
 ```
@@ -56,10 +57,10 @@
  ('postgres',)]
 ```
 
 ## Tests
 
 Run the tests as follows:
 ```bash
-pip install -e .[testing]
+pip install -e .[dev]
 pytest
 ```
```

### Comparing `pgsu-0.2.4/pgsu/__init__.py` & `pgsu-0.3.0/pgsu/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
-"""Connect to an existing PostgreSQL cluster as the `postgres` superuser and execute SQL commands.
-
-"""
+"""Connect to an existing PostgreSQL cluster as the `postgres` superuser and execute SQL commands."""
+__version__ = '0.3.0'
 
 import logging
 import traceback
 import os
 from enum import IntEnum
 import subprocess
+import warnings
 
 # By default, try "sudo" only when 'postgres' user exists
 DEFAULT_POSTGRES_UNIX_USER = 'postgres'
 try:
     import pwd
     pwd.getpwnam(DEFAULT_POSTGRES_UNIX_USER)
     DEFAULT_TRY_SUDO = True
@@ -25,15 +25,15 @@
 
 DEFAULT_DSN = {
     'host':
     None,  # 'localhost' causes psql to connect via method 'host' instead of 'local'
     'port': 5432,
     'user': DEFAULT_POSTGRES_SUPERUSER,
     'password': None,
-    'database': 'template1',
+    'dbname': 'template1',
 }
 
 LOGGER = logging.getLogger('pgsu')
 LOGGER.setLevel(logging.DEBUG)
 
 
 class PostgresConnectionMode(IntEnum):
@@ -44,15 +44,15 @@
     PSQL = 2
 
 
 class PGSU:
     """
     Connect to an existing PostgreSQL cluster as the `postgres` superuser and execute SQL commands.
 
-    Tries to use psycopg2 with a fallback to psql subcommands (using ``sudo su`` to run as postgres user).
+    Tries to use psycopg with a fallback to psql subcommands (using ``sudo su`` to run as postgres user).
 
     Simple Example::
 
         pgsu = PGSU()
         pgsu.execute("CREATE USER testuser PASSWORD 'testpw'")
 
     Complex Example::
@@ -72,21 +72,21 @@
                  determine_setup=True,
                  try_sudo=DEFAULT_TRY_SUDO,
                  postgres_unix_user=DEFAULT_POSTGRES_UNIX_USER):
         """Store postgres connection info.
 
         :param interactive: use True for verdi commands
         :param quiet: use False to show warnings/exceptions
-        :param dsn: psycopg dictionary containing keys like 'host', 'user', 'port', 'database'.
+        :param dsn: psycopg dictionary containing keys like 'host', 'user', 'port', 'dbname'.
             It is sufficient to provide only those values that deviate from the defaults.
         :param determine_setup: Whether to determine setup upon instantiation.
             You may set this to False and use the 'determine_setup()' method instead.
-        :param try_sudo: If connection via psycopg2 fails, whether to try and use `sudo` to  become
+        :param try_sudo: If connection via psycopg fails, whether to try and use `sudo` to  become
             the `postgres_unix_user` and run commands using passwordless `psql`.
-        :param postgres_unix_user: UNIX user to try to "become", if connection via psycopg2 fails
+        :param postgres_unix_user: UNIX user to try to "become", if connection via psycopg fails
         """
         self.interactive = interactive
         if not quiet:
             handler = logging.StreamHandler()
             handler.setLevel(logging.INFO)
             LOGGER.addHandler(handler)
         self.connection_mode = PostgresConnectionMode.DISCONNECTED
@@ -94,14 +94,20 @@
         self.setup_fail_counter = 0
         self.setup_max_tries = 1
 
         self.dsn = DEFAULT_DSN.copy()
         if dsn is not None:
             self.dsn.update(dsn)
 
+        if 'database' in self.dsn:
+            warnings.warn(
+                'The dsn contained the key `database` which was renamed to `dbname` in psycopg v3. '
+                'Renamed the database key to dbname', UserWarning)
+            self.dsn['dbname'] = self.dsn.pop('database')
+
         self.try_sudo = try_sudo
         self.postgres_unix_user = postgres_unix_user
 
         if determine_setup:
             self.determine_setup()
 
     def execute(self, command, **kwargs):
@@ -122,27 +128,27 @@
         raise ConnectionError(
             'Could not connect to PostgreSQL server using dsn={dsn}.\n' \
                 + 'Consider providing connection parameters via PGSU(dsn={...}).')
 
     def determine_setup(self):
         """Determine how to connect as the postgres superuser.
 
-        Depending on how postgres is set up, psycopg2 can be used to create dbs and db users,
+        Depending on how postgres is set up, psycopg can be used to create dbs and db users,
         otherwise a subprocess has to be used that executes psql as an os user with appropriate permissions.
 
         Note: We aim to connect as a superuser (typically 'postgres') with privileges to manipulate (create/drop)
           databases and database users.
 
         :returns success: True, if connection could be established.
         :rtype success: bool
         """
         dsn = self.dsn.copy()
 
-        # Try to connect as a postgres superuser via psycopg2 (equivalent to using psql).
-        LOGGER.debug('Trying to connect via "psycopg2"...')
+        # Try to connect as a postgres superuser via psycopg (equivalent to using psql).
+        LOGGER.debug('Trying to connect via "psycopg"...')
         for pg_user in unique_list([self.dsn.get('user'), None]):
             dsn['user'] = pg_user
             # First try the host specified (works if 'host' has setting 'trust' in pg_hba.conf).
             # Then try local connection (works if 'local' has setting 'trust' in pg_hba.conf).
             # Then try 'host' localhost via TCP/IP.
             for pg_host in unique_list([self.dsn.get('host'), None, 'localhost']):   # yapf: disable
                 dsn['host'] = pg_host
@@ -201,64 +207,64 @@
 
     :return: dictionary with the keys: host, port, database, user, password
     """
     import click  # pylint: disable=import-outside-toplevel
     click.echo('Please provide PostgreSQL connection info:')
 
     # Note: Using '' as the prompt default is necessary to allow users to leave the field empty.
-    #       Using `None` in the dictionary is necessary in order for psycopg2 to interpret the value as not provided.
+    #       Using `None` in the dictionary is necessary in order for  to interpret the value as not provided.
     dsn_new = {}
     dsn_new['host'] = click.prompt(
         'postgres host', default=dsn.get('host') or '', type=str) or None
     dsn_new['port'] = click.prompt(
         'postgres port', default=dsn.get('port'), type=int) or None
     dsn_new['user'] = click.prompt(
         'postgres super user', default=dsn.get('user'), type=str) or None
-    dsn_new['database'] = click.prompt(
-        'database', default=dsn.get('database'), type=str) or None
+    dsn_new['dbname'] = click.prompt(
+        'dbname', default=dsn.get('dbname'), type=str) or None
     dsn_new['password'] = click.prompt(
         'postgres password of {dsn_new["user"]}',
         #hide_input=True,   # this breaks the input mocking in the tests. could make this configurable instead
         type=str,
         default=dsn.get('password') or '') or None
 
     return dsn_new
 
 
 def _try_connect_psycopg(**kwargs):
     """
-    try to start a psycopg2 connection.
+    try to start a psycopg connection.
 
     :return: True if successful, False otherwise
     """
-    from psycopg2 import connect  # pylint: disable=import-outside-toplevel
+    from psycopg import connect  # pylint: disable=import-outside-toplevel
     success = False
     try:
         conn = connect(**kwargs)
         success = True
         conn.close()
     except Exception:  # pylint: disable=broad-except
         LOGGER.debug('Unable to connect via psycopg')
         LOGGER.debug(traceback.format_exc())
     return success
 
 
 def _execute_psyco(command, dsn):
     """
-    executes a postgres commandline through psycopg2
+    executes a postgres commandline through psycopg
 
     :param command: A psql command line as a str
-    :param dsn: will be forwarded to psycopg2.connect
+    :param dsn: will be forwarded to psycopg.connect
     """
-    import psycopg2  # pylint: disable=import-outside-toplevel
+    import psycopg  # pylint: disable=import-outside-toplevel
 
     conn = None
     output = None
     try:
-        conn = psycopg2.connect(**dsn)
+        conn = psycopg.connect(**dsn)
         conn.autocommit = True
         with conn.cursor() as cursor:
             cursor.execute(command)
             if cursor.description is not None:
                 output = cursor.fetchall()
     finally:
         if conn:
@@ -304,22 +310,28 @@
 
     Tries to "become" the user specified in ``dsn`` (i.e. interpreted as UNIX system user)
     and run psql in a subprocess.
 
     Logs any output on 'stderr' to the pgsu logger at 'warning' level.
 
     :param command: A psql command line as a str
-    :param dsn: connection details to forward to psql, signature as in psycopg2.connect
+    :param dsn: connection details to forward to psql, signature as in psycopg.connect
     :param interactive: If False, `sudo` won't ask for a password and fail if one is required.
     """
     psql_option_str = ''
 
-    database = dsn.get('database')
-    if database:
-        psql_option_str += f'-d {database}'
+    if 'database' in dsn:
+        warnings.warn(
+            'The dsn contained the key `database` which was renamed to `dbname` in psycopg v3. '
+            'Renamed the database key to dbname', UserWarning)
+        dsn['dbname'] = dsn.pop('database')
+
+    dbname = dsn.get('dbname')
+    if dbname:
+        psql_option_str += f'-d {dbname}'
 
     # to do: Forward password to psql; ignore host only when the password is None.  # pylint: disable=fixme
     # Note: There is currently no known postgresql setup that needs this, though
     # password = dsn.get('password')
 
     host = dsn.pop('host', 'localhost')
     if host and host != 'localhost':
```

