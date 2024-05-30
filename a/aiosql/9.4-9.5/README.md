# Comparing `tmp/aiosql-9.4.tar.gz` & `tmp/aiosql-9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosql-9.4.tar", last modified: Sun Jan 28 12:08:18 2024, max compression
+gzip compressed data, was "aiosql-9.5.tar", last modified: Sun Feb 18 08:24:04 2024, max compression
```

## Comparing `aiosql-9.4.tar` & `aiosql-9.5.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.334126 aiosql-9.4/
--rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.4/.dockerignore
--rw-------   0 fabien    (1001) fabien    (1001)      417 2023-05-14 12:34:57.000000 aiosql-9.4/.editorconfig
--rw-------   0 fabien    (1001) fabien    (1001)      176 2023-05-14 12:34:57.000000 aiosql-9.4/.flake8
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.322126 aiosql-9.4/.github/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/.github/scripts/
--rwx------   0 fabien    (1001) fabien    (1001)      577 2023-07-12 06:05:15.000000 aiosql-9.4/.github/scripts/docs.sh
--rwx------   0 fabien    (1001) fabien    (1001)       87 2023-05-14 12:34:57.000000 aiosql-9.4/.github/scripts/package-build.sh
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/.github/workflows/
--rw-------   0 fabien    (1001) fabien    (1001)     1593 2024-01-28 12:07:41.000000 aiosql-9.4/.github/workflows/aiosql-package.yml
--rw-------   0 fabien    (1001) fabien    (1001)      742 2023-05-14 12:34:57.000000 aiosql-9.4/.github/workflows/deploy-pages.yml
--rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.4/.gitignore
--rw-------   0 fabien    (1001) fabien    (1001)     1552 2023-05-14 12:34:57.000000 aiosql-9.4/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       25 2023-05-29 10:11:04.000000 aiosql-9.4/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)    10215 2024-01-28 12:07:41.000000 aiosql-9.4/Makefile
--rw-r--r--   0 fabien    (1001) fabien    (1001)    10517 2024-01-28 12:08:18.334126 aiosql-9.4/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 06:05:15.000000 aiosql-9.4/README.rst
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/aiosql/
--rw-------   0 fabien    (1001) fabien    (1001)      283 2023-05-27 17:26:40.000000 aiosql-9.4/aiosql/__init__.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/aiosql/adapters/
--rw-------   0 fabien    (1001) fabien    (1001)      370 2023-05-14 12:34:57.000000 aiosql-9.4/aiosql/adapters/__init__.py
--rw-------   0 fabien    (1001) fabien    (1001)     2449 2024-01-28 10:31:13.000000 aiosql-9.4/aiosql/adapters/aiosqlite.py
--rw-------   0 fabien    (1001) fabien    (1001)     5181 2024-01-28 10:31:13.000000 aiosql-9.4/aiosql/adapters/asyncpg.py
--rw-------   0 fabien    (1001) fabien    (1001)     3247 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/adapters/duckdb.py
--rw-------   0 fabien    (1001) fabien    (1001)     4305 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/adapters/generic.py
--rw-------   0 fabien    (1001) fabien    (1001)     1117 2024-01-28 10:31:13.000000 aiosql-9.4/aiosql/adapters/mysql.py
--rw-------   0 fabien    (1001) fabien    (1001)      182 2023-05-14 12:34:57.000000 aiosql-9.4/aiosql/adapters/pg8000.py
--rw-------   0 fabien    (1001) fabien    (1001)      640 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/adapters/pyformat.py
--rw-------   0 fabien    (1001) fabien    (1001)      502 2023-05-14 12:34:57.000000 aiosql-9.4/aiosql/adapters/sqlite3.py
--rw-------   0 fabien    (1001) fabien    (1001)     6751 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/aiosql.py
--rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.4/aiosql/py.typed
--rw-------   0 fabien    (1001) fabien    (1001)     8604 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/queries.py
--rw-------   0 fabien    (1001) fabien    (1001)     6992 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/query_loader.py
--rw-------   0 fabien    (1001) fabien    (1001)     4603 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/types.py
--rw-------   0 fabien    (1001) fabien    (1001)      723 2024-01-28 12:07:41.000000 aiosql-9.4/aiosql/utils.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/aiosql.egg-info/
--rw-r--r--   0 fabien    (1001) fabien    (1001)    10517 2024-01-28 12:08:18.000000 aiosql-9.4/aiosql.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     2490 2024-01-28 12:08:18.000000 aiosql-9.4/aiosql.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2024-01-28 12:08:18.000000 aiosql-9.4/aiosql.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)      435 2024-01-28 12:08:18.000000 aiosql-9.4/aiosql.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)        7 2024-01-28 12:08:18.000000 aiosql-9.4/aiosql.egg-info/top_level.txt
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/docker/
--rw-------   0 fabien    (1001) fabien    (1001)       17 2023-05-14 12:34:57.000000 aiosql-9.4/docker/.gitignore
--rwx------   0 fabien    (1001) fabien    (1001)     1458 2023-05-14 12:34:57.000000 aiosql-9.4/docker/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     1052 2023-07-12 06:05:15.000000 aiosql-9.4/docker/README.md
--rw-------   0 fabien    (1001) fabien    (1001)     1346 2023-05-27 17:26:40.000000 aiosql-9.4/docker/docker-compose.yml
--rw-------   0 fabien    (1001) fabien    (1001)      791 2023-07-06 06:26:19.000000 aiosql-9.4/docker/dockerfile.python-mariadb
--rw-------   0 fabien    (1001) fabien    (1001)      505 2023-07-06 06:26:19.000000 aiosql-9.4/docker/dockerfile.python-mysql
--rw-------   0 fabien    (1001) fabien    (1001)      492 2023-07-06 06:26:19.000000 aiosql-9.4/docker/dockerfile.python-postgres
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.322126 aiosql-9.4/docs/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/docs/source/
--rw-------   0 fabien    (1001) fabien    (1001)     7898 2023-05-28 06:48:04.000000 aiosql-9.4/docs/source/advanced-topics.rst
--rw-------   0 fabien    (1001) fabien    (1001)     2515 2023-12-06 07:39:58.000000 aiosql-9.4/docs/source/conf.py
--rw-------   0 fabien    (1001) fabien    (1001)     2447 2023-05-28 06:48:04.000000 aiosql-9.4/docs/source/contributing.rst
--rw-------   0 fabien    (1001) fabien    (1001)     4738 2023-05-28 06:48:04.000000 aiosql-9.4/docs/source/database-driver-adapters.rst
--rw-------   0 fabien    (1001) fabien    (1001)     7747 2023-08-11 23:46:16.000000 aiosql-9.4/docs/source/defining-sql-queries.rst
--rw-------   0 fabien    (1001) fabien    (1001)     9793 2023-05-29 10:11:04.000000 aiosql-9.4/docs/source/getting-started.rst
--rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 06:05:15.000000 aiosql-9.4/docs/source/index.rst
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.326126 aiosql-9.4/docs/source/pydoc/
--rw-------   0 fabien    (1001) fabien    (1001)     1452 2023-05-28 06:58:31.000000 aiosql-9.4/docs/source/pydoc/aiosql.adapters.rst
--rw-------   0 fabien    (1001) fabien    (1001)      896 2023-05-28 06:58:31.000000 aiosql-9.4/docs/source/pydoc/aiosql.rst
--rw-------   0 fabien    (1001) fabien    (1001)       55 2023-05-28 06:58:31.000000 aiosql-9.4/docs/source/pydoc/modules.rst
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/example/
--rw-------   0 fabien    (1001) fabien    (1001)     2640 2023-05-14 12:34:57.000000 aiosql-9.4/example/example.py
--rw-------   0 fabien    (1001) fabien    (1001)      299 2023-05-14 12:34:57.000000 aiosql-9.4/example/greetings.py
--rwx------   0 fabien    (1001) fabien    (1001)      303 2023-05-14 12:34:57.000000 aiosql-9.4/example/greetings.sh
--rw-------   0 fabien    (1001) fabien    (1001)      289 2023-05-14 12:34:57.000000 aiosql-9.4/example/greetings.sql
--rw-------   0 fabien    (1001) fabien    (1001)      485 2023-05-14 12:34:57.000000 aiosql-9.4/example/greetings_async.py
--rw-------   0 fabien    (1001) fabien    (1001)      509 2023-05-14 12:34:57.000000 aiosql-9.4/example/greetings_create.sql
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/example/sql/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/example/sql/blogs/
--rw-------   0 fabien    (1001) fabien    (1001)      671 2023-05-14 12:34:57.000000 aiosql-9.4/example/sql/blogs/blogs.sql
--rw-------   0 fabien    (1001) fabien    (1001)      422 2023-05-14 12:34:57.000000 aiosql-9.4/example/sql/create_schema.sql
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/example/sql/users/
--rw-------   0 fabien    (1001) fabien    (1001)      189 2023-05-14 12:34:57.000000 aiosql-9.4/example/sql/users/users.sql
--rw-------   0 fabien    (1001) fabien    (1001)     1774 2024-01-28 12:07:41.000000 aiosql-9.4/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)       38 2024-01-28 12:08:18.334126 aiosql-9.4/setup.cfg
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.322126 aiosql-9.4/tests/blogdb/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/blogdb/data/
--rw-------   0 fabien    (1001) fabien    (1001)      199 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/data/blogs_data.csv
--rw-------   0 fabien    (1001) fabien    (1001)       53 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/data/users_data.csv
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.322126 aiosql-9.4/tests/blogdb/sql/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/blogdb/sql/blogs/
--rw-------   0 fabien    (1001) fabien    (1001)       29 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs.oops
--rw-------   0 fabien    (1001) fabien    (1001)      935 2023-05-27 17:26:40.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs.sql
--rw-------   0 fabien    (1001) fabien    (1001)      700 2023-05-27 17:26:40.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs_duckdb.sql
--rw-------   0 fabien    (1001) fabien    (1001)      486 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs_mysql.sql
--rw-------   0 fabien    (1001) fabien    (1001)      975 2023-05-27 17:26:40.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs_pg.sql
--rw-------   0 fabien    (1001) fabien    (1001)      588 2023-05-27 17:26:40.000000 aiosql-9.4/tests/blogdb/sql/blogs/blogs_sqlite.sql
--rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/blogs/empty.sql
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/blogdb/sql/comments/
--rw-------   0 fabien    (1001) fabien    (1001)      271 2023-05-27 17:26:40.000000 aiosql-9.4/tests/blogdb/sql/comments/comments_duckdb.sql
--rw-------   0 fabien    (1001) fabien    (1001)      218 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/comments/comments_pg.sql
--rw-------   0 fabien    (1001) fabien    (1001)      241 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/comments/comments_sqlite.sql
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/blogdb/sql/misc/
--rw-------   0 fabien    (1001) fabien    (1001)      777 2024-01-28 10:31:13.000000 aiosql-9.4/tests/blogdb/sql/misc/misc.sql
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-01-28 12:08:18.330126 aiosql-9.4/tests/blogdb/sql/users/
--rw-------   0 fabien    (1001) fabien    (1001)     1122 2023-05-14 12:34:57.000000 aiosql-9.4/tests/blogdb/sql/users/users.sql
--rw-------   0 fabien    (1001) fabien    (1001)     1436 2023-05-29 10:11:04.000000 aiosql-9.4/tests/conf_duckdb.py
--rw-------   0 fabien    (1001) fabien    (1001)     3288 2023-05-14 12:34:57.000000 aiosql-9.4/tests/conf_mysql.py
--rw-------   0 fabien    (1001) fabien    (1001)     3656 2023-05-29 10:11:04.000000 aiosql-9.4/tests/conf_pgsql.py
--rw-------   0 fabien    (1001) fabien    (1001)     2200 2024-01-28 12:07:41.000000 aiosql-9.4/tests/conf_schema.py
--rw-------   0 fabien    (1001) fabien    (1001)      494 2023-05-29 10:11:04.000000 aiosql-9.4/tests/conf_sqlite.py
--rw-------   0 fabien    (1001) fabien    (1001)      830 2023-05-27 17:26:40.000000 aiosql-9.4/tests/conftest.py
--rw-------   0 fabien    (1001) fabien    (1001)      256 2023-05-27 17:26:40.000000 aiosql-9.4/tests/pytest.ini
--rw-------   0 fabien    (1001) fabien    (1001)    14926 2024-01-28 12:07:41.000000 aiosql-9.4/tests/run_tests.py
--rw-------   0 fabien    (1001) fabien    (1001)     3305 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_aiosqlite.py
--rw-------   0 fabien    (1001) fabien    (1001)     2757 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_apsw.py
--rw-------   0 fabien    (1001) fabien    (1001)     5363 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_asyncpg.py
--rw-------   0 fabien    (1001) fabien    (1001)     2311 2023-12-06 07:39:58.000000 aiosql-9.4/tests/test_duckdb.py
--rw-------   0 fabien    (1001) fabien    (1001)     6944 2024-01-28 12:07:41.000000 aiosql-9.4/tests/test_loading.py
--rw-------   0 fabien    (1001) fabien    (1001)     2346 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_mariadb.py
--rw-------   0 fabien    (1001) fabien    (1001)     2386 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_myco.py
--rw-------   0 fabien    (1001) fabien    (1001)     2637 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_mysqldb.py
--rw-------   0 fabien    (1001) fabien    (1001)     3439 2023-05-14 12:34:57.000000 aiosql-9.4/tests/test_patterns.py
--rw-------   0 fabien    (1001) fabien    (1001)     2467 2024-01-28 10:31:13.000000 aiosql-9.4/tests/test_pg8000.py
--rw-------   0 fabien    (1001) fabien    (1001)     2129 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_psycopg2.py
--rw-------   0 fabien    (1001) fabien    (1001)     2193 2024-01-28 10:31:13.000000 aiosql-9.4/tests/test_psycopg3.py
--rw-------   0 fabien    (1001) fabien    (1001)     2424 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_pygresql.py
--rw-------   0 fabien    (1001) fabien    (1001)     2323 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_pymysql.py
--rw-------   0 fabien    (1001) fabien    (1001)     1933 2023-05-29 10:11:04.000000 aiosql-9.4/tests/test_sqlite3.py
--rw-------   0 fabien    (1001) fabien    (1001)      948 2024-01-28 11:43:13.000000 aiosql-9.4/tests/utils.py
--rwx------   0 fabien    (1001) fabien    (1001)      149 2023-05-14 12:34:57.000000 aiosql-9.4/tests/wait.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.719263 aiosql-9.5/
+-rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.5/.dockerignore
+-rw-------   0 fabien    (1001) fabien    (1001)      417 2023-05-14 12:34:57.000000 aiosql-9.5/.editorconfig
+-rw-------   0 fabien    (1001) fabien    (1001)      176 2023-05-14 12:34:57.000000 aiosql-9.5/.flake8
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/.github/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/.github/scripts/
+-rwx------   0 fabien    (1001) fabien    (1001)      577 2023-07-12 06:05:15.000000 aiosql-9.5/.github/scripts/docs.sh
+-rwx------   0 fabien    (1001) fabien    (1001)       87 2023-05-14 12:34:57.000000 aiosql-9.5/.github/scripts/package-build.sh
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/.github/workflows/
+-rw-------   0 fabien    (1001) fabien    (1001)     1524 2024-02-18 08:22:03.000000 aiosql-9.5/.github/workflows/aiosql-package.yml
+-rw-------   0 fabien    (1001) fabien    (1001)      742 2023-05-14 12:34:57.000000 aiosql-9.5/.github/workflows/deploy-pages.yml
+-rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.5/.gitignore
+-rw-------   0 fabien    (1001) fabien    (1001)     1552 2023-05-14 12:34:57.000000 aiosql-9.5/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       25 2023-05-29 10:11:04.000000 aiosql-9.5/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)    10215 2024-01-28 12:07:41.000000 aiosql-9.5/Makefile
+-rw-r--r--   0 fabien    (1001) fabien    (1001)    10489 2024-02-18 08:24:04.719263 aiosql-9.5/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 06:05:15.000000 aiosql-9.5/README.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/aiosql/
+-rw-------   0 fabien    (1001) fabien    (1001)      283 2023-05-27 17:26:40.000000 aiosql-9.5/aiosql/__init__.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.703264 aiosql-9.5/aiosql/adapters/
+-rw-------   0 fabien    (1001) fabien    (1001)      370 2023-05-14 12:34:57.000000 aiosql-9.5/aiosql/adapters/__init__.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2449 2024-01-28 10:31:13.000000 aiosql-9.5/aiosql/adapters/aiosqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)     5181 2024-01-28 10:31:13.000000 aiosql-9.5/aiosql/adapters/asyncpg.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3247 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/adapters/duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     4305 2024-02-03 18:46:34.000000 aiosql-9.5/aiosql/adapters/generic.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1117 2024-01-28 10:31:13.000000 aiosql-9.5/aiosql/adapters/mysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)      182 2023-05-14 12:34:57.000000 aiosql-9.5/aiosql/adapters/pg8000.py
+-rw-------   0 fabien    (1001) fabien    (1001)      640 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/adapters/pyformat.py
+-rw-------   0 fabien    (1001) fabien    (1001)      502 2023-05-14 12:34:57.000000 aiosql-9.5/aiosql/adapters/sqlite3.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6751 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/aiosql.py
+-rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.5/aiosql/py.typed
+-rw-------   0 fabien    (1001) fabien    (1001)     8604 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/queries.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6992 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/query_loader.py
+-rw-------   0 fabien    (1001) fabien    (1001)     4603 2024-01-28 12:07:41.000000 aiosql-9.5/aiosql/types.py
+-rw-------   0 fabien    (1001) fabien    (1001)      723 2024-02-03 18:46:45.000000 aiosql-9.5/aiosql/utils.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.715263 aiosql-9.5/aiosql.egg-info/
+-rw-r--r--   0 fabien    (1001) fabien    (1001)    10489 2024-02-18 08:24:04.000000 aiosql-9.5/aiosql.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     2490 2024-02-18 08:24:04.000000 aiosql-9.5/aiosql.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2024-02-18 08:24:04.000000 aiosql-9.5/aiosql.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      397 2024-02-18 08:24:04.000000 aiosql-9.5/aiosql.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        7 2024-02-18 08:24:04.000000 aiosql-9.5/aiosql.egg-info/top_level.txt
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.703264 aiosql-9.5/docker/
+-rw-------   0 fabien    (1001) fabien    (1001)       17 2023-05-14 12:34:57.000000 aiosql-9.5/docker/.gitignore
+-rwx------   0 fabien    (1001) fabien    (1001)     1458 2023-05-14 12:34:57.000000 aiosql-9.5/docker/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     1052 2023-07-12 06:05:15.000000 aiosql-9.5/docker/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1346 2023-05-27 17:26:40.000000 aiosql-9.5/docker/docker-compose.yml
+-rw-------   0 fabien    (1001) fabien    (1001)      791 2023-07-06 06:26:19.000000 aiosql-9.5/docker/dockerfile.python-mariadb
+-rw-------   0 fabien    (1001) fabien    (1001)      505 2023-07-06 06:26:19.000000 aiosql-9.5/docker/dockerfile.python-mysql
+-rw-------   0 fabien    (1001) fabien    (1001)      492 2023-07-06 06:26:19.000000 aiosql-9.5/docker/dockerfile.python-postgres
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/docs/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.703264 aiosql-9.5/docs/source/
+-rw-------   0 fabien    (1001) fabien    (1001)     7898 2023-05-28 06:48:04.000000 aiosql-9.5/docs/source/advanced-topics.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     2515 2023-12-06 07:39:58.000000 aiosql-9.5/docs/source/conf.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2447 2023-05-28 06:48:04.000000 aiosql-9.5/docs/source/contributing.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     4738 2023-05-28 06:48:04.000000 aiosql-9.5/docs/source/database-driver-adapters.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     7747 2023-08-11 23:46:16.000000 aiosql-9.5/docs/source/defining-sql-queries.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     9793 2023-05-29 10:11:04.000000 aiosql-9.5/docs/source/getting-started.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 06:05:15.000000 aiosql-9.5/docs/source/index.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.703264 aiosql-9.5/docs/source/pydoc/
+-rw-------   0 fabien    (1001) fabien    (1001)     1452 2023-05-28 06:58:31.000000 aiosql-9.5/docs/source/pydoc/aiosql.adapters.rst
+-rw-------   0 fabien    (1001) fabien    (1001)      896 2023-05-28 06:58:31.000000 aiosql-9.5/docs/source/pydoc/aiosql.rst
+-rw-------   0 fabien    (1001) fabien    (1001)       55 2023-05-28 06:58:31.000000 aiosql-9.5/docs/source/pydoc/modules.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.707264 aiosql-9.5/example/
+-rw-------   0 fabien    (1001) fabien    (1001)     2640 2023-05-14 12:34:57.000000 aiosql-9.5/example/example.py
+-rw-------   0 fabien    (1001) fabien    (1001)      299 2023-05-14 12:34:57.000000 aiosql-9.5/example/greetings.py
+-rwx------   0 fabien    (1001) fabien    (1001)      303 2023-05-14 12:34:57.000000 aiosql-9.5/example/greetings.sh
+-rw-------   0 fabien    (1001) fabien    (1001)      289 2023-05-14 12:34:57.000000 aiosql-9.5/example/greetings.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      485 2023-05-14 12:34:57.000000 aiosql-9.5/example/greetings_async.py
+-rw-------   0 fabien    (1001) fabien    (1001)      509 2023-05-14 12:34:57.000000 aiosql-9.5/example/greetings_create.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.707264 aiosql-9.5/example/sql/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.707264 aiosql-9.5/example/sql/blogs/
+-rw-------   0 fabien    (1001) fabien    (1001)      671 2023-05-14 12:34:57.000000 aiosql-9.5/example/sql/blogs/blogs.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      422 2023-05-14 12:34:57.000000 aiosql-9.5/example/sql/create_schema.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.707264 aiosql-9.5/example/sql/users/
+-rw-------   0 fabien    (1001) fabien    (1001)      189 2023-05-14 12:34:57.000000 aiosql-9.5/example/sql/users/users.sql
+-rw-------   0 fabien    (1001) fabien    (1001)     1632 2024-02-18 08:22:03.000000 aiosql-9.5/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2024-02-18 08:24:04.719263 aiosql-9.5/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.711264 aiosql-9.5/tests/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/tests/blogdb/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.711264 aiosql-9.5/tests/blogdb/data/
+-rw-------   0 fabien    (1001) fabien    (1001)      199 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/data/blogs_data.csv
+-rw-------   0 fabien    (1001) fabien    (1001)       53 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/data/users_data.csv
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.699264 aiosql-9.5/tests/blogdb/sql/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.715263 aiosql-9.5/tests/blogdb/sql/blogs/
+-rw-------   0 fabien    (1001) fabien    (1001)       29 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs.oops
+-rw-------   0 fabien    (1001) fabien    (1001)      935 2023-05-27 17:26:40.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      700 2023-05-27 17:26:40.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs_duckdb.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      486 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs_mysql.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      975 2023-05-27 17:26:40.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs_pg.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      588 2023-05-27 17:26:40.000000 aiosql-9.5/tests/blogdb/sql/blogs/blogs_sqlite.sql
+-rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/blogs/empty.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.715263 aiosql-9.5/tests/blogdb/sql/comments/
+-rw-------   0 fabien    (1001) fabien    (1001)      271 2023-05-27 17:26:40.000000 aiosql-9.5/tests/blogdb/sql/comments/comments_duckdb.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      218 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/comments/comments_pg.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      241 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/comments/comments_sqlite.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.715263 aiosql-9.5/tests/blogdb/sql/misc/
+-rw-------   0 fabien    (1001) fabien    (1001)      777 2024-01-28 10:31:13.000000 aiosql-9.5/tests/blogdb/sql/misc/misc.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-02-18 08:24:04.715263 aiosql-9.5/tests/blogdb/sql/users/
+-rw-------   0 fabien    (1001) fabien    (1001)     1122 2023-05-14 12:34:57.000000 aiosql-9.5/tests/blogdb/sql/users/users.sql
+-rw-------   0 fabien    (1001) fabien    (1001)     1436 2023-05-29 10:11:04.000000 aiosql-9.5/tests/conf_duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3288 2023-05-14 12:34:57.000000 aiosql-9.5/tests/conf_mysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3656 2023-05-29 10:11:04.000000 aiosql-9.5/tests/conf_pgsql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2200 2024-01-28 12:07:41.000000 aiosql-9.5/tests/conf_schema.py
+-rw-------   0 fabien    (1001) fabien    (1001)      494 2023-05-29 10:11:04.000000 aiosql-9.5/tests/conf_sqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)      830 2023-05-27 17:26:40.000000 aiosql-9.5/tests/conftest.py
+-rw-------   0 fabien    (1001) fabien    (1001)      256 2023-05-27 17:26:40.000000 aiosql-9.5/tests/pytest.ini
+-rw-------   0 fabien    (1001) fabien    (1001)    14926 2024-01-28 12:07:41.000000 aiosql-9.5/tests/run_tests.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3305 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_aiosqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2757 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_apsw.py
+-rw-------   0 fabien    (1001) fabien    (1001)     5363 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_asyncpg.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2311 2023-12-06 07:39:58.000000 aiosql-9.5/tests/test_duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6944 2024-01-28 12:07:41.000000 aiosql-9.5/tests/test_loading.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2346 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_mariadb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2386 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_myco.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2637 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_mysqldb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3439 2023-05-14 12:34:57.000000 aiosql-9.5/tests/test_patterns.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2467 2024-01-28 10:31:13.000000 aiosql-9.5/tests/test_pg8000.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2129 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_psycopg2.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2193 2024-01-28 10:31:13.000000 aiosql-9.5/tests/test_psycopg3.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2424 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_pygresql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2323 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_pymysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1933 2023-05-29 10:11:04.000000 aiosql-9.5/tests/test_sqlite3.py
+-rw-------   0 fabien    (1001) fabien    (1001)      948 2024-01-28 11:43:13.000000 aiosql-9.5/tests/utils.py
+-rwx------   0 fabien    (1001) fabien    (1001)      149 2023-05-14 12:34:57.000000 aiosql-9.5/tests/wait.py
```

### Comparing `aiosql-9.4/.dockerignore` & `aiosql-9.5/.dockerignore`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/.github/scripts/docs.sh` & `aiosql-9.5/.github/scripts/docs.sh`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/.github/workflows/aiosql-package.yml` & `aiosql-9.5/.github/workflows/aiosql-package.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        # NOTE duckdb does not install with python 3.12 (2023-12-06)
         # https://github.com/actions/python-versions (versions-manifest.json)
         # https://downloads.python.org/pypy/versions.json
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
```

### Comparing `aiosql-9.4/.github/workflows/deploy-pages.yml` & `aiosql-9.5/.github/workflows/deploy-pages.yml`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/.gitignore` & `aiosql-9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/LICENSE` & `aiosql-9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/Makefile` & `aiosql-9.5/Makefile`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/PKG-INFO` & `aiosql-9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosql
-Version: 9.4
+Version: 9.5
 Summary: Simple SQL in Python
 Author-email: "William Vaughn et al." <vaughnwilld@gmail.com>
 License: BSD 2-Clause License
 Project-URL: repository, https://github.com/nackjicholson/aiosql
 Project-URL: documentation, https://nackjicholson.github.io/aiosql/
 Project-URL: issues, https://github.com/nackjicholson/aiosql/issues
 Project-URL: package, https://pypi.org/project/aiosql/
@@ -22,15 +22,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: dev-duckdb
-Requires-Dist: duckdb; python_version < "3.12" and extra == "dev-duckdb"
+Requires-Dist: duckdb; extra == "dev-duckdb"
 Provides-Extra: dev-sqlite
 Requires-Dist: aiosqlite; extra == "dev-sqlite"
 Requires-Dist: apsw; extra == "dev-sqlite"
 Provides-Extra: dev-postgres
 Requires-Dist: pytest-postgresql; extra == "dev-postgres"
 Requires-Dist: asyncpg; extra == "dev-postgres"
 Requires-Dist: psycopg>=3; extra == "dev-postgres"
```

### Comparing `aiosql-9.4/README.rst` & `aiosql-9.5/README.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/aiosqlite.py` & `aiosql-9.5/aiosql/adapters/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/asyncpg.py` & `aiosql-9.5/aiosql/adapters/asyncpg.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/duckdb.py` & `aiosql-9.5/aiosql/adapters/duckdb.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/generic.py` & `aiosql-9.5/aiosql/adapters/generic.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/mysql.py` & `aiosql-9.5/aiosql/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/adapters/pyformat.py` & `aiosql-9.5/aiosql/adapters/pyformat.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/aiosql.py` & `aiosql-9.5/aiosql/aiosql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/queries.py` & `aiosql-9.5/aiosql/queries.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/query_loader.py` & `aiosql-9.5/aiosql/query_loader.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/types.py` & `aiosql-9.5/aiosql/types.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql/utils.py` & `aiosql-9.5/aiosql/utils.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/aiosql.egg-info/PKG-INFO` & `aiosql-9.5/aiosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosql
-Version: 9.4
+Version: 9.5
 Summary: Simple SQL in Python
 Author-email: "William Vaughn et al." <vaughnwilld@gmail.com>
 License: BSD 2-Clause License
 Project-URL: repository, https://github.com/nackjicholson/aiosql
 Project-URL: documentation, https://nackjicholson.github.io/aiosql/
 Project-URL: issues, https://github.com/nackjicholson/aiosql/issues
 Project-URL: package, https://pypi.org/project/aiosql/
@@ -22,15 +22,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: dev-duckdb
-Requires-Dist: duckdb; python_version < "3.12" and extra == "dev-duckdb"
+Requires-Dist: duckdb; extra == "dev-duckdb"
 Provides-Extra: dev-sqlite
 Requires-Dist: aiosqlite; extra == "dev-sqlite"
 Requires-Dist: apsw; extra == "dev-sqlite"
 Provides-Extra: dev-postgres
 Requires-Dist: pytest-postgresql; extra == "dev-postgres"
 Requires-Dist: asyncpg; extra == "dev-postgres"
 Requires-Dist: psycopg>=3; extra == "dev-postgres"
```

### Comparing `aiosql-9.4/aiosql.egg-info/SOURCES.txt` & `aiosql-9.5/aiosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docker/Makefile` & `aiosql-9.5/docker/Makefile`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docker/README.md` & `aiosql-9.5/docker/README.md`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docker/docker-compose.yml` & `aiosql-9.5/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docker/dockerfile.python-mariadb` & `aiosql-9.5/docker/dockerfile.python-mariadb`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/advanced-topics.rst` & `aiosql-9.5/docs/source/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/conf.py` & `aiosql-9.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/contributing.rst` & `aiosql-9.5/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/database-driver-adapters.rst` & `aiosql-9.5/docs/source/database-driver-adapters.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/defining-sql-queries.rst` & `aiosql-9.5/docs/source/defining-sql-queries.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/getting-started.rst` & `aiosql-9.5/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/index.rst` & `aiosql-9.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/pydoc/aiosql.adapters.rst` & `aiosql-9.5/docs/source/pydoc/aiosql.adapters.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/docs/source/pydoc/aiosql.rst` & `aiosql-9.5/docs/source/pydoc/aiosql.rst`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/example/example.py` & `aiosql-9.5/example/example.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/example/sql/blogs/blogs.sql` & `aiosql-9.5/example/sql/blogs/blogs.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/pyproject.toml` & `aiosql-9.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiosql"
-version = "9.4"
+version = "9.5"
 authors = [ { name = "William Vaughn et al.", email = "vaughnwilld@gmail.com" } ]
 description = "Simple SQL in Python"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { text = "BSD 2-Clause License" }
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -19,18 +19,15 @@
 [project.optional-dependencies]
 dev = [
     "pytest<8", "pytest-asyncio",
     "rstcheck", "black", "coverage", "flake8",
     "mypy", "pyright", "types-setuptools", "build"
 ]
 dev-duckdb = [
-    # FIXME duckdb does not compile on 3.12.0 on 2023-12-06
-    # NOTE leaving it out breaks coverage
-    "duckdb; python_version < '3.12'"
-    # "duckdb"
+    "duckdb"
 ]
 dev-sqlite = [
     "aiosqlite", "apsw"
 ]
 dev-postgres = [
     "pytest-postgresql",
     "asyncpg",
```

### Comparing `aiosql-9.4/tests/blogdb/sql/blogs/blogs.sql` & `aiosql-9.5/tests/blogdb/sql/blogs/blogs.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/blogdb/sql/blogs/blogs_duckdb.sql` & `aiosql-9.5/tests/blogdb/sql/blogs/blogs_duckdb.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/blogdb/sql/blogs/blogs_pg.sql` & `aiosql-9.5/tests/blogdb/sql/blogs/blogs_pg.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/blogdb/sql/blogs/blogs_sqlite.sql` & `aiosql-9.5/tests/blogdb/sql/blogs/blogs_sqlite.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/blogdb/sql/misc/misc.sql` & `aiosql-9.5/tests/blogdb/sql/misc/misc.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/blogdb/sql/users/users.sql` & `aiosql-9.5/tests/blogdb/sql/users/users.sql`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/conf_duckdb.py` & `aiosql-9.5/tests/conf_duckdb.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/conf_mysql.py` & `aiosql-9.5/tests/conf_mysql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/conf_pgsql.py` & `aiosql-9.5/tests/conf_pgsql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/conf_schema.py` & `aiosql-9.5/tests/conf_schema.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/conftest.py` & `aiosql-9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/run_tests.py` & `aiosql-9.5/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_aiosqlite.py` & `aiosql-9.5/tests/test_aiosqlite.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_apsw.py` & `aiosql-9.5/tests/test_apsw.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_asyncpg.py` & `aiosql-9.5/tests/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_duckdb.py` & `aiosql-9.5/tests/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_loading.py` & `aiosql-9.5/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_mariadb.py` & `aiosql-9.5/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_myco.py` & `aiosql-9.5/tests/test_myco.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_mysqldb.py` & `aiosql-9.5/tests/test_mysqldb.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_patterns.py` & `aiosql-9.5/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_pg8000.py` & `aiosql-9.5/tests/test_pg8000.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_psycopg2.py` & `aiosql-9.5/tests/test_psycopg2.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_psycopg3.py` & `aiosql-9.5/tests/test_psycopg3.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_pygresql.py` & `aiosql-9.5/tests/test_pygresql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_pymysql.py` & `aiosql-9.5/tests/test_pymysql.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/test_sqlite3.py` & `aiosql-9.5/tests/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `aiosql-9.4/tests/utils.py` & `aiosql-9.5/tests/utils.py`

 * *Files identical despite different names*

