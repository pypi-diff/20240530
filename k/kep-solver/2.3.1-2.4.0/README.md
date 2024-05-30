# Comparing `tmp/kep_solver-2.3.1.tar.gz` & `tmp/kep_solver-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kep_solver-2.3.1.tar", last modified: Thu Feb 29 13:02:28 2024, max compression
+gzip compressed data, was "kep_solver-2.4.0.tar", last modified: Thu May 30 14:19:25 2024, max compression
```

## Comparing `kep_solver-2.3.1.tar` & `kep_solver-2.4.0.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.664182 kep_solver-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-29 13:02:08.000000 kep_solver-2.3.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-02-29 13:02:08.000000 kep_solver-2.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-02-29 13:02:08.000000 kep_solver-2.3.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-02-29 13:02:08.000000 kep_solver-2.3.1/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6624 2024-02-29 13:02:08.000000 kep_solver-2.3.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     8779 2024-02-29 13:02:08.000000 kep_solver-2.3.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    34462 2024-02-29 13:02:08.000000 kep_solver-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45792 2024-02-29 13:02:28.663182 kep_solver-2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4482 2024-02-29 13:02:08.000000 kep_solver-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.633181 kep_solver-2.3.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2834 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.634181 kep_solver-2.3.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)      699 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/source/faq.rst
--rw-rw-rw-   0 root         (0) root         (0)    12990 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/source/formats.rst
--rw-rw-rw-   0 root         (0) root         (0)     5405 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/source/terms.rst
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-02-29 13:02:08.000000 kep_solver-2.3.1/docs/source/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.636181 kep_solver-2.3.1/kep_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27717 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/entities.py
--rw-rw-rw-   0 root         (0) root         (0)    16478 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    36751 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/generation.py
--rw-rw-rw-   0 root         (0) root         (0)    27517 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    23859 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8706 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/pool.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-29 13:02:08.000000 kep_solver-2.3.1/kep_solver/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.662181 kep_solver-2.3.1/kep_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45792 2024-02-29 13:02:28.000000 kep_solver-2.3.1/kep_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3229 2024-02-29 13:02:28.000000 kep_solver-2.3.1/kep_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 13:02:28.000000 kep_solver-2.3.1/kep_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2024-02-29 13:02:28.000000 kep_solver-2.3.1/kep_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-29 13:02:28.000000 kep_solver-2.3.1/kep_solver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-02-29 13:02:08.000000 kep_solver-2.3.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.638181 kep_solver-2.3.1/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)     6159 2024-02-29 13:02:08.000000 kep_solver-2.3.1/notebooks/Match Run.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1485 2024-02-29 13:02:08.000000 kep_solver-2.3.1/notebooks/README.md
--rw-rw-rw-   0 root         (0) root         (0)    23889 2024-02-29 13:02:08.000000 kep_solver-2.3.1/notebooks/Statistical Analysis.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.638181 kep_solver-2.3.1/paper/
--rw-rw-rw-   0 root         (0) root         (0)     2848 2024-02-29 13:02:08.000000 kep_solver-2.3.1/paper/paper.bib
--rw-rw-rw-   0 root         (0) root         (0)     6286 2024-02-29 13:02:08.000000 kep_solver-2.3.1/paper/paper.md
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-02-29 13:02:08.000000 kep_solver-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 13:02:28.664182 kep_solver-2.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.640181 kep_solver-2.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9045 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    22957 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    23309 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 13:02:28.661182 kep_solver-2.3.1/tests/test_instances/
--rw-rw-rw-   0 root         (0) root         (0)   514090 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-1.json
--rw-rw-rw-   0 root         (0) root         (0)   590458 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-10.json
--rw-rw-rw-   0 root         (0) root         (0)   610079 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-2.json
--rw-rw-rw-   0 root         (0) root         (0)   590792 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-3.json
--rw-rw-rw-   0 root         (0) root         (0)   550366 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-4.json
--rw-rw-rw-   0 root         (0) root         (0)   575193 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-5.json
--rw-rw-rw-   0 root         (0) root         (0)   660843 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-6.json
--rw-rw-rw-   0 root         (0) root         (0)   665457 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-7.json
--rw-rw-rw-   0 root         (0) root         (0)   684308 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-8.json
--rw-rw-rw-   0 root         (0) root         (0)   686677 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/large-9.json
--rw-rw-rw-   0 root         (0) root         (0)    40468 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-1.json
--rw-rw-rw-   0 root         (0) root         (0)    32770 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-10.json
--rw-rw-rw-   0 root         (0) root         (0)    43595 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-2.json
--rw-rw-rw-   0 root         (0) root         (0)    33837 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-3.json
--rw-rw-rw-   0 root         (0) root         (0)    34664 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-4.json
--rw-rw-rw-   0 root         (0) root         (0)    38406 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-5.json
--rw-rw-rw-   0 root         (0) root         (0)    33991 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-6.json
--rw-rw-rw-   0 root         (0) root         (0)    35438 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-7.json
--rw-rw-rw-   0 root         (0) root         (0)    37158 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-8.json
--rw-rw-rw-   0 root         (0) root         (0)    46046 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/medium-9.json
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1.txt
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1.xml
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test10.json
--rw-rw-rw-   0 root         (0) root         (0)     2598 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test10_output.json
--rw-rw-rw-   0 root         (0) root         (0)     2838 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test10_output.xml
--rw-rw-rw-   0 root         (0) root         (0)      659 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1_output.json
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test1_output.xml
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test2.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test2.txt
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test2.xml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test2.yaml
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3.json
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3.txt
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3.xml
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3b.json
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3b.txt
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3b.xml
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test3b.yaml
--rw-rw-rw-   0 root         (0) root         (0)      827 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test4.json
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test4.txt
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test4.xml
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test4.yaml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5.json
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5.txt
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5.xml
--rw-rw-rw-   0 root         (0) root         (0)      462 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5.yaml
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5b.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test5b.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test6.txt
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test6a.json
--rw-rw-rw-   0 root         (0) root         (0)     1037 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test6a.xml
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test6b.json
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test6b.xml
--rw-rw-rw-   0 root         (0) root         (0)   116023 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test7.json
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test7.txt
--rw-rw-rw-   0 root         (0) root         (0)    48578 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test7.yaml
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8.json
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8.txt
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8b.json
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8b.txt
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8c.json
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test8c.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test9.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test9_output.json
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test9_output.xml
--rw-rw-rw-   0 root         (0) root         (0)      438 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test_simple_chains.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_instances/test_simple_chains.txt
--rw-rw-rw-   0 root         (0) root         (0)    11105 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_output.py
--rw-rw-rw-   0 root         (0) root         (0)     9180 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     4124 2024-02-29 13:02:08.000000 kep_solver-2.3.1/tests/test_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.600795 kep_solver-2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-30 14:19:08.000000 kep_solver-2.4.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-30 14:19:08.000000 kep_solver-2.4.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-30 14:19:08.000000 kep_solver-2.4.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-30 14:19:08.000000 kep_solver-2.4.0/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2024-05-30 14:19:08.000000 kep_solver-2.4.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      933 2024-05-30 14:19:08.000000 kep_solver-2.4.0/CITATION.cff
+-rw-rw-rw-   0 root         (0) root         (0)     8779 2024-05-30 14:19:08.000000 kep_solver-2.4.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    34462 2024-05-30 14:19:08.000000 kep_solver-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45951 2024-05-30 14:19:25.599795 kep_solver-2.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2024-05-30 14:19:08.000000 kep_solver-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.566794 kep_solver-2.4.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.567794 kep_solver-2.4.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/source/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12990 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/source/formats.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/source/terms.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/source/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-30 14:19:08.000000 kep_solver-2.4.0/docs/source/zreferences.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.569795 kep_solver-2.4.0/kep_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27717 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    16478 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    36733 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/generation.py
+-rw-rw-rw-   0 root         (0) root         (0)    28671 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    41015 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     9515 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/pool.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 14:19:08.000000 kep_solver-2.4.0/kep_solver/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.598795 kep_solver-2.4.0/kep_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45951 2024-05-30 14:19:25.000000 kep_solver-2.4.0/kep_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-30 14:19:25.000000 kep_solver-2.4.0/kep_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 14:19:25.000000 kep_solver-2.4.0/kep_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2024-05-30 14:19:25.000000 kep_solver-2.4.0/kep_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-30 14:19:25.000000 kep_solver-2.4.0/kep_solver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-30 14:19:08.000000 kep_solver-2.4.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.571795 kep_solver-2.4.0/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)     6159 2024-05-30 14:19:08.000000 kep_solver-2.4.0/notebooks/Match Run.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-30 14:19:08.000000 kep_solver-2.4.0/notebooks/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    23889 2024-05-30 14:19:08.000000 kep_solver-2.4.0/notebooks/Statistical Analysis.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.572795 kep_solver-2.4.0/paper/
+-rw-rw-rw-   0 root         (0) root         (0)     2848 2024-05-30 14:19:08.000000 kep_solver-2.4.0/paper/paper.bib
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2024-05-30 14:19:08.000000 kep_solver-2.4.0/paper/paper.md
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-30 14:19:08.000000 kep_solver-2.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 14:19:25.600795 kep_solver-2.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.573794 kep_solver-2.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9045 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    22957 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    23309 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:19:25.598795 kep_solver-2.4.0/tests/test_instances/
+-rw-rw-rw-   0 root         (0) root         (0)   514090 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-1.json
+-rw-rw-rw-   0 root         (0) root         (0)   590458 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-10.json
+-rw-rw-rw-   0 root         (0) root         (0)   610079 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-2.json
+-rw-rw-rw-   0 root         (0) root         (0)   590792 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-3.json
+-rw-rw-rw-   0 root         (0) root         (0)   550366 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-4.json
+-rw-rw-rw-   0 root         (0) root         (0)   575193 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-5.json
+-rw-rw-rw-   0 root         (0) root         (0)   660843 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-6.json
+-rw-rw-rw-   0 root         (0) root         (0)   665457 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-7.json
+-rw-rw-rw-   0 root         (0) root         (0)   684308 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-8.json
+-rw-rw-rw-   0 root         (0) root         (0)   686677 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/large-9.json
+-rw-rw-rw-   0 root         (0) root         (0)    40468 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-1.json
+-rw-rw-rw-   0 root         (0) root         (0)    32770 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-10.json
+-rw-rw-rw-   0 root         (0) root         (0)    43595 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-2.json
+-rw-rw-rw-   0 root         (0) root         (0)    33837 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-3.json
+-rw-rw-rw-   0 root         (0) root         (0)    34664 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-4.json
+-rw-rw-rw-   0 root         (0) root         (0)    38406 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-5.json
+-rw-rw-rw-   0 root         (0) root         (0)    33991 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-6.json
+-rw-rw-rw-   0 root         (0) root         (0)    35438 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-7.json
+-rw-rw-rw-   0 root         (0) root         (0)    37158 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-8.json
+-rw-rw-rw-   0 root         (0) root         (0)    46046 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/medium-9.json
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1.xml
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test10.json
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test10_output.json
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test10_output.xml
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test1_output.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test2.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test2.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test2.xml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test2.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3.json
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3.txt
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3.xml
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3b.json
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3b.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3b.xml
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test3b.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test4.json
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test4.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test4.xml
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test4.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5.json
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5.txt
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5.xml
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5b.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test5b.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test6.txt
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test6a.json
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test6a.xml
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test6b.json
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test6b.xml
+-rw-rw-rw-   0 root         (0) root         (0)   116023 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test7.json
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test7.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48578 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test7.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8.json
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8.txt
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8b.json
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8b.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8c.json
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test8c.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test9.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test9_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test9_output.xml
+-rw-rw-rw-   0 root         (0) root         (0)      438 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test_simple_chains.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_instances/test_simple_chains.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11105 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_output.py
+-rw-rw-rw-   0 root         (0) root         (0)    11107 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4124 2024-05-30 14:19:08.000000 kep_solver-2.4.0/tests/test_statistics.py
```

### Comparing `kep_solver-2.3.1/.gitlab-ci.yml` & `kep_solver-2.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/CHANGELOG.md` & `kep_solver-2.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## [Unreleased]
 
+## [2.4.0]
+
+- Add PICEF model
+
 ## [2.3.1]
 
 - Add ability to output CompatibilityGraph in DOT graph format
 - Add an option `build_alt_embed` to models that can be set to 0 (for no
     alternate or embedded cycles), 1 (for all alternate and embedded cycles) and
     2 and 3 (two ways of restricting alternate and embedded cycles to those
     expected by NHSBT).
```

### Comparing `kep_solver-2.3.1/CONTRIBUTING.md` & `kep_solver-2.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/LICENSE` & `kep_solver-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/PKG-INFO` & `kep_solver-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kep_solver
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Author-email: William Pettersson <william@ewpettersson.se>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -811,10 +811,13 @@
 submit code. Details on contributing can be found in
 [CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
-Research Council (EPSRC) grant
+Research Council (EPSRC) grants
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
-(Multilayer Algorithmics to Leverage Graph Structure).
+(Multilayer Algorithmics to Leverage Graph Structure)
+and
+[EP/X013618/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/X013618/1)
+(KidneyAlgo: New Algorithms for UK and International Kidney Exchange).
```

### Comparing `kep_solver-2.3.1/README.md` & `kep_solver-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -113,10 +113,13 @@
 submit code. Details on contributing can be found in
 [CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
-Research Council (EPSRC) grant
+Research Council (EPSRC) grants
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
-(Multilayer Algorithmics to Leverage Graph Structure).
+(Multilayer Algorithmics to Leverage Graph Structure)
+and
+[EP/X013618/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/X013618/1)
+(KidneyAlgo: New Algorithms for UK and International Kidney Exchange).
```

### Comparing `kep_solver-2.3.1/docs/Makefile` & `kep_solver-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/docs/conf.py` & `kep_solver-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/docs/source/faq.rst` & `kep_solver-2.4.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/docs/source/formats.rst` & `kep_solver-2.4.0/docs/source/formats.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/docs/source/terms.rst` & `kep_solver-2.4.0/docs/source/terms.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/kep_solver/entities.py` & `kep_solver-2.4.0/kep_solver/entities.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/kep_solver/fileio.py` & `kep_solver-2.4.0/kep_solver/fileio.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/kep_solver/generation.py` & `kep_solver-2.4.0/kep_solver/generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Generation of KEP instances."""
 
-import json
 import random
-from typing import Callable, Optional, Any, Union
+from typing import Callable, Optional, Union
 
 from kep_solver.entities import Donor, Recipient, BloodGroup, Instance, Transplant
 
 
 BloodGroupGeneratorConfig = dict[str, float]
 
 
@@ -822,15 +821,15 @@
         ]
         for r in recips:
             # This also adds corresponding donors
             i.addRecipient(r)
         if self._ndd_bloodgroup_generator is None:
             if numNonDirectedDonors:
                 raise Exception(
-                    f"Tried to generate non-directed donor without knowing blood group distribution of non-directed donors."
+                    "Tried to generate non-directed donor without knowing blood group distribution of non-directed donors."
                 )
         else:
             for num in range(numNonDirectedDonors):
                 donor = Donor(ndd_id_function(num))
                 donor.NDD = True
                 donor.bloodGroup = self._ndd_bloodgroup_generator.draw()
                 i.addDonor(donor)
```

### Comparing `kep_solver-2.3.1/kep_solver/graph.py` & `kep_solver-2.4.0/kep_solver/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from kep_solver.entities import Donor, Recipient, Status
 
 
 class Vertex:
     """A vertex in a digraph representing a donor (directed or
     non-directed)."""
 
+    _sink: Optional["Vertex"] = None
+
     def __init__(self, index: int, represents: Donor) -> None:
         self._index: int = index
         self._represents: Donor = represents
         self._properties: dict[str, Any] = {}
         self._edges_out: list[Edge] = []
         self._edges_in: list[Edge] = []
         self._adj: Optional[list[Vertex]] = None
@@ -90,14 +92,22 @@
             return f"V({self.donor} ({self.index}))"
         else:
             return f"V({self.donor},{self.donor.recipient} ({self.index}))"
 
     def __repr__(self) -> str:
         return str(self)
 
+    @staticmethod
+    def sink() -> Vertex:
+        if Vertex._sink is None:
+            sink_donor = Donor(id="sink")
+            sink_donor.NDD = True
+            Vertex._sink = Vertex(index=-1, represents=sink_donor)
+        return Vertex._sink
+
 
 class Exchange:
     """An exchange is either a cycle or a chain. This class lets us embed
     information (like embedded exchanges, or alternates) into the exchange.
     """
 
     def __init__(self, _id: str, vertices: list[Vertex]):
@@ -404,14 +414,40 @@
     def edges(self) -> list[Edge]:
         """The edges in the graph.
 
         :return: the edges
         """
         return self._edges
 
+    def number_ndds(self) -> int:
+        """Count the number of non-directed donors in this graph.
+
+        :return: The number of non-directed donors.
+        """
+        return len([v for v in self.vertices if v.isNdd()])
+
+    def exchangeEdges(self, exchange: Exchange) -> list[Edge]:
+        """Return the edges in the given exchange.
+
+        :param exchange: The exchange in question
+        :return: The edges in this exchange.
+        """
+        result: list[Edge] = []
+        for j, vertex in enumerate(exchange[:-1]):
+            for edge in vertex.edgesOut():
+                if edge.end == exchange[j + 1]:
+                    result.append(edge)
+                    break
+        if not exchange.chain:
+            for edge in exchange[-1].edgesOut():
+                if edge.end == exchange[0]:
+                    result.append(edge)
+                    break
+        return result
+
     def addDonor(self, donor: Donor) -> None:
         """Add a vertex representing a donor.
 
         :param donor: a donor to be added to the graph.
         """
         vertex = Vertex(len(self._vertices), donor)
         self._vertices.append(vertex)
@@ -512,15 +548,14 @@
         # Comput., 1975
         # There are some changes, however. Blocklists (B(n) in the
         # paper) aren't used, as since we limit cycle lengths we will
         # return when the stack is too long, but that doesn't mean we
         # must've created all cycles through a given vertex. For the
         # same reason, v is unblocked after each visit, regardless of
         # whether we find any cycles
-        blocked: set[int] = set()
         stack: list[int] = []
         cycles: list[list[int]] = []
 
         def _circuit(v: int, condition: Callable[[int], bool]) -> None:
             stack.append(v)
             for w in self.vertices[v].adjacent():
                 if w.index == stack[0]:
```

### Comparing `kep_solver-2.3.1/kep_solver/model.py` & `kep_solver-2.4.0/kep_solver/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from collections import defaultdict
 from collections.abc import ValuesView
 from enum import Enum
 from time import thread_time
-from typing import Optional
+from typing import Optional, Union
 
 import pulp  # type: ignore
 import warnings  # We use this to ignore one specific warning from pulp
 
 
 from kep_solver.entities import Instance, Donor
 from kep_solver.graph import (
     CompatibilityGraph,
     Vertex,
+    Edge,
     Exchange,
     build_alternates_and_embeds,
 )
 
 
 class Sense(Enum):
     """An enumeration of the sense of an objective."""
@@ -52,22 +54,38 @@
 
 class Objective:
     """A base class for an objective."""
 
     def __init__(self):
         raise Exception("Plain Objective objects cannot be instantiated")
 
+    def edgeValue(
+        self, graph: CompatibilityGraph, edge: Edge, position: Optional[int] = None
+    ) -> float:
+        """What value should the given transplant in the given graph be given,
+        if it is at the given position (i.e., position = 1 means this is the
+        first edge in a chain)?
+
+        :param graph: The graph containing the exchange
+        :param edge: The edge, representing a transplant
+        :param position: The position of this edge in an exchange
+        :return: The value of this edge in this position
+        """
+        raise Exception("Edge value not defined for this objective")
+
     def value(self, graph: CompatibilityGraph, exchange: Exchange) -> float:
         """What value should the given exchange in the given graph
         be given?
 
         :param graph: The graph containing the exchange
         :param exchange: A cycle or chain.
         """
-        raise Exception("Plain Objective objects should not be instantiated or called")
+        return sum(
+            self.edgeValue(graph, edge) for edge in graph.exchangeEdges(exchange)
+        )
 
     def describe(self) -> str:
         """Describes what this objective optimises.
 
         :return: the description
         """
         raise Exception("Plain Objective objects should not be instantiated or called")
@@ -84,14 +102,28 @@
     would go to a deceased-donor waiting list) is counted as a
     transplant.
     """
 
     def __init__(self):
         pass
 
+    def edgeValue(
+        self, graph: CompatibilityGraph, edge: Edge, position: Optional[int] = None
+    ) -> float:
+        """What value should the given transplant in the given graph be given,
+        if it is at the given position (i.e., position = 1 means this is the
+        first edge in a chain)?
+
+        :param graph: The graph containing the exchange
+        :param edge: The edge, representing a transplant
+        :param position: The position of this edge in an exchange
+        :return: The value of this edge in this position
+        """
+        return 1
+
     def value(self, graph: CompatibilityGraph, exchange: Exchange) -> float:
         """How many transplants does the given exchange represent.
 
         :param graph: The graph containing the exchange
         :param exchange: A cycle or chain.
         :return: the number of transplants
         """
@@ -203,15 +235,14 @@
     _age_weight_selector = 20
     _age_weight = 3
     _age_diff_factor = 1e-5
     _max_age_diff = 70
 
     if d2.NDD:
         return 0, 0
-    bonus = 0
     age_diff = abs(d1.age - d2.age)
     tb = _age_diff_factor * ((_max_age_diff - age_diff) ** 2)
     tb = round(tb, 5)
     if age_diff <= _age_weight_selector:
         return _age_weight, tb
     return 0, tb
 
@@ -294,16 +325,47 @@
 class Model(pulp.LpProblem):
     """A base class for all models for KEPs. Any new models should
     inherit from this and implement all associated functions.
     """
 
     supports: list[type[Objective]] = []
 
-    def __init__(self):
+    def __init__(
+        self,
+        instance: Instance,
+        objectives: list[Objective],
+        *,
+        maxCycleLength: int,
+        maxChainLength: int,
+        build_alt_embed: int = 0,
+    ):
+        """Create a Model. Note that this base class has no implementation and
+        should not be directly constructed.
+
+        :param instance: The instance to build the model from
+        :param objectives: The list of objectives for this pool
+        :param maxCycleLength: The maximum length of a cycle
+        :param maxChainLength: The maximum length of a chain
+        :param build_alt_embed: Whether to build alternate and embedded
+            exchanges. build_alt_embed can be set to any of the following:
+
+            0. Don't build alternate and embedded cycles. Faster, if you don't need alternate and embedded cycles
+            1. Build all alternate and embedded cycles.
+            2. Build only those alternate and embedded cycles that NHSBT expects
+            3. Build only those alternate and embedded cycles that NHSBT expects, where embedded exchanges cannot use new donors
+        """
         super().__init__()
+        self._instance: Instance = instance
+        self._graph: CompatibilityGraph = CompatibilityGraph(instance)
+        # List comprehension to make a copy of the list of objectives
+        self._objectives: list[Objective] = [obj for obj in objectives]
+        self._objective_values: list[float] = []
+        self._maxCycleLength = maxCycleLength
+        self._maxChainLength = maxChainLength
+        self._build_alt_embed = build_alt_embed
 
     @property
     def cycles(self) -> ValuesView[Exchange]:
         """Return the list of cycles in this model.
 
         :return: the list of cycles
         """
@@ -372,14 +434,383 @@
         :return: A list of selected transplants, a list of the time taken
             to solve for each objective in the pool, and a list of the number
             of optimal solutions found for each objective
         """
         raise Exception("Plain Model objects should not be instantiated or called")
 
 
+class PICEF(Model):
+    """A model that represents each cycle by a variable, but otherwise
+    represents edges in chains as a variable.
+    """
+
+    supports = [TransplantCount]
+
+    def __init__(
+        self,
+        instance: Instance,
+        objectives: list[Objective],
+        *,
+        maxCycleLength: int,
+        maxChainLength: int,
+        build_alt_embed: int = 0,
+    ):
+        """Construct a PICEF model from an instance.
+
+        :param instance: The instance to build the model from
+        :param objectives: The list of objectives for this pool
+        :param maxCycleLength: The maximum length of a cycle
+        :param maxChainLength: The maximum length of a chain
+        :param build_alt_embed: Determines which alternative and embedded
+            exchanges should be enumerated. For PICEF, this must be set to zero.
+        """
+        if build_alt_embed != 0:
+            raise Exception(f"Unable to use PICEF with {build_alt_embed=}")
+        super().__init__(
+            instance,
+            objectives,
+            maxCycleLength=maxCycleLength,
+            maxChainLength=maxChainLength,
+            build_alt_embed=0,
+        )
+        self._cycles: dict[pulp.LpVariable, Exchange] = {}
+        self._vars_by_vertex: dict[Vertex, list[pulp.LpVariable]] = {}
+        self._vars_by_exchange: dict[Exchange, pulp.LpVariable] = {}
+        self._chain_edge_vars: dict[Edge, list[pulp.LpVariable]] = defaultdict(list)
+        self._chain_vars_out: dict[int, dict[int, list[pulp.LpVariable]]] = defaultdict(
+            lambda: defaultdict(list)
+        )
+        self._chain_vars_in: dict[int, dict[int, list[pulp.LpVariable]]] = defaultdict(
+            lambda: defaultdict(list)
+        )
+
+    @property
+    def cycles(self) -> ValuesView[Exchange]:
+        """Return the list of cycles in this model.
+
+        :return: the list of cycles
+        """
+        return self._cycles.values()
+
+    @property
+    def chains(self) -> ValuesView[Exchange]:
+        """Return the list of chains in this model.
+
+        :return: the list of chains
+        """
+        raise Exception("chains() not implemented for PICEF")
+
+    @property
+    def exchanges(self) -> list[Exchange]:
+        """Return the list of cycles and chains in this model.
+
+        :return: the list of cycles and chains
+        """
+        raise Exception("It's vague to do this now as what is chains()? in PICEF")
+        return list(self.chains) + list(self.cycles)
+
+    @property
+    def graph(self) -> CompatibilityGraph:
+        """The graph used for this model.
+
+        :return: The graph used for this model.
+        """
+        return self._graph
+
+    def exchange_values(self, exchange: Exchange) -> list[float]:
+        """Given an exchange, return the value of the exchange for
+        each objective.
+
+        :param exchange: The exchange whose value is to be returned
+        :return: the list of values of this exchange
+        """
+        return [
+            objective.value(self._graph, exchange) for objective in self._objectives
+        ]
+
+    def _var_from_donor(self, donor: Donor) -> pulp.LpVariable:
+        """Given a donor, find its corresponding variable. This means
+        going via the CompatibilityGraph.
+
+        :param donor: the donor to search for
+        :return: the donor's variable
+        """
+        return self._vars_by_vertex[self._graph.donorVertex(donor)]
+
+    def _var_from_exchange(self, exchange: Exchange) -> pulp.LpVariable:
+        """Given an exchange, get the variable representing it.
+
+        :param exchange: the exchange to search for
+        :return: the exchange's variable
+        """
+        return self._vars_by_exchange[exchange]
+
+    def _build_chain_vars(self) -> None:
+        """Build the variables for chain variables."""
+        if self._maxChainLength == 0:
+            return
+        donor_queue: list[tuple[Donor, int]] = [
+            (d, 1) for d in self._instance.activeDonors() if d.NDD
+        ]
+        done: set[tuple[int, Union[str, int], int]] = set()
+        while donor_queue:
+            donor, length = donor_queue.pop(0)
+            vertex = self._graph.donorVertex(donor)
+            if length < self._maxChainLength:
+                for e in vertex.edgesOut:
+                    tup = (vertex.index, e.end.index, length)
+                    if tup in done:
+                        continue
+                    var = pulp.LpVariable(
+                        f"chain_{vertex.index}_{e.end.index}_{length}", cat="Binary"
+                    )
+                    var.position = length
+                    done.add(tup)
+                    self._chain_vars_out[vertex.index][length].append(var)
+                    self._chain_vars_in[e.end.index][length].append(var)
+                    self._chain_edge_vars[e].append(var)
+                    donor_queue.append((e.end.donor, length + 1))
+            var = pulp.LpVariable(f"chain_{vertex.index}_sink_{length}", cat="Binary")
+            var.position = length
+            stup = (vertex.index, "sink", length)
+            if stup in done:
+                continue
+            done.add(stup)
+            self._chain_vars_out[vertex.index][length].append(var)
+            sink = Edge(donor, vertex, Vertex.sink())
+            self._chain_edge_vars[sink].append(var)
+
+        return
+
+    def _build_chain_constraints(self) -> None:
+        """Build the constraints for chain variables."""
+        for v in self._graph.vertices:
+            if v.index not in self._chain_vars_out:
+                continue
+            if v.isNdd():
+                length = 1
+                # At most one donation from an NDD
+                name = f"vertex_ndd_{str(v)}_{length}_max"
+                self += (
+                    pulp.lpSum(self._chain_vars_out[v.index][length]) <= 1,
+                    name,
+                )
+            else:
+                for length in range(2, self._maxChainLength + 1):
+                    # Don't donate unless you get a donation
+                    name = f"vertex_{str(v)}_{length}_flow"
+                    self += (
+                        pulp.lpSum(self._chain_vars_out[v.index][length])
+                        <= pulp.lpSum(self._chain_vars_in[v.index][length - 1]),
+                        name,
+                    )
+
+    def _build_chains_from_edges(self, selected: list[Edge]) -> list[Exchange]:
+        """Given a set of edges in a graph (specifically, the compatibility
+        graph associated with this model), build the associated set of chains.
+
+        :param: selected The selected edges to be used
+        :return: The list of chains corresponding to these edges
+        """
+
+        def build_chain(verts_so_far):
+            for e in verts_so_far[-1].edgesOut:
+                if e in selected:
+                    verts_so_far.append(e.end)
+                    build_chain(verts_so_far)
+
+        chains: list[Exchange] = []
+        for donor in self._instance.activeDonors():
+            if not donor.NDD:
+                continue
+            chain_verts = [self._graph.donorVertex(donor)]
+            build_chain(chain_verts)
+            chains.append(Exchange(f"{len(chains)}", chain_verts))
+        return chains
+
+    def build_model(self) -> None:
+        """Build the model. That is, create all the variables and
+        constraints."""
+        for vertex in self._graph.vertices:
+            self._vars_by_vertex[vertex] = []
+        for cycle in self._graph.findCycles(self._maxCycleLength):
+            var = pulp.LpVariable(f"cycle_{len(self._cycles)}", cat="Binary")
+            for vertex in cycle.vertices:
+                self._vars_by_vertex[vertex].append(var)
+            self._vars_by_exchange[cycle] = var
+            self._cycles[var] = cycle
+        self._build_chain_vars()
+        self._build_chain_constraints()
+        for recipient in self._instance.activeRecipients():
+            name = f"recipient_{str(recipient)}"
+            self += (
+                pulp.lpSum(self._var_from_donor(donor) for donor in recipient.donors())
+                + pulp.lpSum(
+                    pulp.lpSum(
+                        pulp.lpSum(
+                            self._chain_vars_in[self._graph.donorVertex(donor).index][
+                                length
+                            ]
+                        )
+                        for length in range(1, self._maxChainLength + 1)
+                    )
+                    for donor in recipient.donors()
+                )
+                <= 1,
+                name,
+            )
+
+    def addObjectiveConstraint(self, objective: Objective, value: float, index: int):
+        """Adds a constraint that ensures the previous objective keeps
+        its value.
+
+        :param objective: The previous objective
+        :param value: The value the previous objective attained
+        :param index: Which number objective is this (only used for
+            naming the constraint)
+        """
+        equation = pulp.lpSum(
+            objective.value(self._graph, cycle) * var
+            for var, cycle in self._cycles.items()
+        )
+        equation += pulp.lpSum(
+            objective.edgeValue(self._graph, edge, var.position) * var
+            for edge, edge_vars in self._chain_edge_vars.items()
+            for var in edge_vars
+        )
+        con = pulp.LpConstraint(
+            equation,
+            sense=objective.sense.toConstraint(),
+            rhs=value,
+            name=f"ObjCon_{index}",
+        )
+        self += con
+
+    def countSolutions(self, maxCount: Optional[int] = None) -> int:
+        """Count the number of distinct solutions available for this instance at this objective.
+
+        Note that this can drastically increase the running time (by several
+        orders of magnitude) as for each distinct solution we need to solve a
+        new IP model.
+        """
+        raise Exception("Not yet implemented")
+        solver = pulp.getSolver("PULP_CBC_CMD", msg=False)
+        copy = self.copy()
+        pulp.LpProblem.solve(copy, solver)
+        solns = 1
+        target = pulp.valueOrDefault(copy.objective)
+        while True:
+            selected = [x for x in copy.variables() if x.value() > 0.9]
+            copy += pulp.LpConstraint(
+                pulp.lpSum(selected),
+                sense=pulp.LpConstraintLE,
+                rhs=len(selected) - 1,  # -1 for less-or-equal
+                name=f"Avoid_soln_{solns}",
+            )
+            pulp.LpProblem.solve(copy, solver)
+            objective = pulp.valueOrDefault(copy.objective)
+            if (
+                copy.status != pulp.constants.LpStatusOptimal
+                or abs(target - objective) > 1e-4
+            ):
+                return solns
+            solns += 1
+            if maxCount and solns >= maxCount:
+                return solns
+
+    def solve(
+        self,
+        countSolutions: bool = False,
+        maxCount: Optional[list[int]] = None,
+        solver=None,
+    ) -> tuple[list[Exchange], list[tuple[str, float]], list[int]]:
+        """Solve the model to find an optimal solution.
+
+        :param countSolutions: If true, count the number of distinct solutions
+            found at each level of optimisation. Note that this solves a new
+            optimisation problem for each such solution found, and thus can be very
+            time-consuming.
+
+        :param solver: An instantiated PuLP solver. If empty, a CBC solver is
+            created and used
+
+        :return: A list of selected transplants, a list of the time taken
+            to solve for each objective in the pool, and a list of the number
+            of optimal solutions found for each objective
+        """
+        self.build_model()
+        selected: list[Exchange] = []
+        num_solutions: list[int] = []
+        times: list[tuple[str, float]] = []
+        if solver is None:
+            solver = pulp.getSolver("PULP_CBC_CMD", msg=False)
+        for index, obj in enumerate(self._objectives):
+            obj_equation = pulp.lpSum(
+                obj.value(self._graph, cycle) * var
+                for var, cycle in self._cycles.items()
+            )
+            obj_equation += pulp.lpSum(
+                obj.edgeValue(self._graph, edge, var.position) * var
+                for edge, edge_vars in self._chain_edge_vars.items()
+                for var in edge_vars
+            )
+            # If there is nothing in the objective function, we skip it.
+            # Otherwise, PuLP sometimes has issues.
+            if not obj_equation:
+                self._objective_values.append(0)
+                continue
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", "Overwriting previously set objective."
+                )
+                self += obj_equation
+            self.sense = obj.sense.toObjective()
+            t = thread_time()
+            pulp.LpProblem.solve(self, solver)
+            if self.status != pulp.constants.LpStatusOptimal:
+                raise Exception("Optimising returned non-optimal, no solution found")
+            self._objective_values.append(pulp.valueOrDefault(self.objective))
+            if countSolutions:
+                limit = None
+                if maxCount:
+                    limit = maxCount[index]
+                num_solutions.append(self.countSolutions(limit))
+            times.append((f"Solving {obj.describe()}", thread_time() - t))
+            if index < len(self._objectives) - 1:
+                self.addObjectiveConstraint(obj, self._objective_values[-1], index)
+            else:
+                for var, cycle in self._cycles.items():
+                    if var.value() > 0.9:
+                        selected.append(cycle)
+                selected_edges: list[Edge] = []
+                for edge, varList in self._chain_edge_vars.items():
+                    if any(var.value() > 0.9 for var in varList):
+                        selected_edges.append(edge)
+                selected.extend(self._build_chains_from_edges(selected_edges))
+        return selected, times, num_solutions
+
+    @property
+    def objective_values(self) -> list[float]:
+        """The list of all objective values."""
+        return self._objective_values
+
+    def objective_value(self, objective_index: int) -> float:
+        """Return the value of an objective, if it has been solved.
+        If this model has not been solved, accessing this raises an
+        error.
+
+        :param objective_index: the index of the objective whose value
+            is to be returned
+        :return: the value of the objective as given by objective_index
+        """
+        if not self._objective_values:
+            raise Exception("Tried to get objective value when model is not solved.")
+        return self._objective_values[objective_index]
+
+
 class CycleAndChainModel(Model):
     """A model that represents each cycle or chain with a binary
     variable.  Note that since CompatibilityGraph has one vertex per
     donor, and recipients may have multiple donors, this means that
     constraints may be needed to ensure at most one donor per recipient
     is selected.
 
@@ -400,36 +831,31 @@
 
         :param instance: The instance to build the model from
         :param objectives: The list of objectives for this pool
         :param maxCycleLength: The maximum length of a cycle
         :param maxChainLength: The maximum length of a chain
         :param build_alt_embed: Whether to build alternate and embedded
             exchanges. build_alt_embed can be set to any of the following:
-                0: Don't build alternate and embedded cycles. Faster, if you don't need
-                   alternate and embedded cycles
-                1: Build all alternate and embedded cycles.
-                2: Build only those alternate and embedded cycles that NHSBT expects
-                3: Build only those alternate and embedded cycles that NHSBT
-                   expects, where embedded exchanges cannot use new donors
-        """
-        super().__init__()
-        self._instance: Instance = instance
-        self._graph: CompatibilityGraph = CompatibilityGraph(instance)
-        # List comprehension to make a copy of the list of objectives
-        self._objectives: list[Objective] = [obj for obj in objectives]
-        self._maxCycleLength = maxCycleLength
-        self._maxChainLength = maxChainLength
+
+            0. Don't build alternate and embedded cycles. Faster, if you don't need alternate and embedded cycles
+            1. Build all alternate and embedded cycles.
+            2. Build only those alternate and embedded cycles that NHSBT expects
+            3. Build only those alternate and embedded cycles that NHSBT expects, where embedded exchanges cannot use new donors
+        """
+        super().__init__(
+            instance,
+            objectives,
+            maxCycleLength=maxCycleLength,
+            maxChainLength=maxChainLength,
+            build_alt_embed=build_alt_embed,
+        )
         self._cycles: dict[pulp.LpVariable, Exchange] = {}
         self._chains: dict[pulp.LpVariable, Exchange] = {}
-        self._objective_values: list[float] = []
         self._vars_by_vertex: dict[Vertex, list[pulp.LpVariable]] = {}
         self._vars_by_exchange: dict[Exchange, pulp.LpVariable] = {}
-        # Note that self._build_alt_embed - 1 must map onto the uk_variant
-        # parameter of the build_alternates_and_embeds function
-        self._build_alt_embed = build_alt_embed
 
     @property
     def cycles(self) -> ValuesView[Exchange]:
         """Return the list of cycles in this model.
 
         :return: the list of cycles
         """
```

### Comparing `kep_solver-2.3.1/kep_solver/pool.py` & `kep_solver-2.4.0/kep_solver/pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 algorithms for a particular KEP.
 """
 
 from time import thread_time
 from typing import Optional
 
 from kep_solver.entities import Instance
-from kep_solver.model import Objective, Model, CycleAndChainModel
+from kep_solver.model import Objective, Model, CycleAndChainModel, PICEF
 from kep_solver.graph import Exchange
 
 
 class ModelledExchange:
     """An exchange as modelled, including its value for various
     objectives and any other relevant information.
     """
@@ -128,37 +128,45 @@
     def __init__(
         self,
         objectives: list[Objective],
         maxCycleLength: int,
         maxChainLength: int,
         description: str,
         build_alt_embed: int = 0,
+        full_details: bool = True,
+        model: type[Model] = CycleAndChainModel,
     ):
         """Constructor for Pool. This represents a set of objectives, and
         parameters for running matchings (such as maximum cycle and chain
         lengths).
 
         :param objectives: the list of objectives
         :param maxCycleLength: The longest cycle length allowed.
         :param maxChainLength: The longest chain length allowed. Note that the
             length of a chain includes the non-directed donor.
         :param description: A description of this pool.
         :param build_alt_embed: Whether to build alternate and embedded
             exchanges. build_alt_embed can be set to any of the following:
-                0: Don't build alternate and embedded cycles. Faster, if you don't need
-                alternate and embedded cycles
-                1: Build all alternate and embedded cycles.
-                2: Build only those alternate and embedded cycles that NHSBT expects
+
+            0. Don't build alternate and embedded cycles. Faster, if you don't need alternate and embedded cycles
+            1. Build all alternate and embedded cycles.
+            2. Build only those alternate and embedded cycles that NHSBT expects
+            3. Build only those alternate and embedded cycles that NHSBT expects, where embedded exchanges cannot use new donors
+        :param full_details: If True, try to return details for all possible
+            exchanges (even the ones not selected). Note that this will fail on
+            some models that don't enumerate all possible exchnages.
         """
         # Create a copy of the list of objectives with the magic colon
         self._objectives: list[Objective] = objectives[:]
         self._maxCycleLength: int = maxCycleLength
         self._maxChainLength: int = maxChainLength
+        self._full_details: bool = full_details
         self._description: str = description
         self._build_alt_embed = build_alt_embed
+        self._modelClass = model
 
     @property
     def description(self) -> str:
         """A description of this pool."""
         return self._description
 
     @description.setter
@@ -207,15 +215,15 @@
             occured, as well as the model that was solved.
         """
         if maxCycleLength is None:
             maxCycleLength = self._maxCycleLength
         if maxChainLength is None:
             maxChainLength = self._maxChainLength
         t = thread_time()
-        model = CycleAndChainModel(
+        model = self._modelClass(
             instance,
             self._objectives,
             maxChainLength=maxChainLength,
             maxCycleLength=maxCycleLength,
             build_alt_embed=self._build_alt_embed,
         )
         times = [("Model building", thread_time() - t)]
@@ -224,15 +232,23 @@
             countSolutions, maxCount, solver
         )
         times.extend(model_times)
         times.append(("Total model solving", thread_time() - t))
         if solution is None:
             return None
         values = model.objective_values
-        exchange_values: dict[Exchange, list[float]] = {
-            exchange: model.exchange_values(exchange) for exchange in model.exchanges
-        }
-        solutions = [ModelledExchange(ex, exchange_values[ex]) for ex in solution]
-        possible = [
-            ModelledExchange(ex, exchange_values[ex]) for ex in exchange_values.keys()
-        ]
-        return Solution(solutions, values, possible, times, numSolutions), model
+        if self._full_details:
+            exchange_values: dict[Exchange, list[float]] = {
+                exchange: model.exchange_values(exchange)
+                for exchange in model.exchanges
+            }
+            solutions = [ModelledExchange(ex, exchange_values[ex]) for ex in solution]
+            possible = [
+                ModelledExchange(ex, exchange_values[ex])
+                for ex in exchange_values.keys()
+            ]
+            return Solution(solutions, values, possible, times, numSolutions), model
+        else:
+            solutions = [
+                ModelledExchange(ex, model.exchange_values(ex)) for ex in solution
+            ]
+            return Solution(solutions, values, [], times, numSolutions), model
```

### Comparing `kep_solver-2.3.1/kep_solver.egg-info/PKG-INFO` & `kep_solver-2.4.0/kep_solver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kep_solver
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Author-email: William Pettersson <william@ewpettersson.se>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -811,10 +811,13 @@
 submit code. Details on contributing can be found in
 [CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
-Research Council (EPSRC) grant
+Research Council (EPSRC) grants
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
-(Multilayer Algorithmics to Leverage Graph Structure).
+(Multilayer Algorithmics to Leverage Graph Structure)
+and
+[EP/X013618/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/X013618/1)
+(KidneyAlgo: New Algorithms for UK and International Kidney Exchange).
```

### Comparing `kep_solver-2.3.1/kep_solver.egg-info/SOURCES.txt` & `kep_solver-2.4.0/kep_solver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 .coveragerc
 .gitignore
 .gitlab-ci.yml
 .readthedocs.yaml
 CHANGELOG.md
+CITATION.cff
 CONTRIBUTING.md
 LICENSE
 README.md
 mypy.ini
 pyproject.toml
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/source/faq.rst
 docs/source/formats.rst
 docs/source/terms.rst
 docs/source/usage.rst
+docs/source/zreferences.rst
 kep_solver/__init__.py
 kep_solver/entities.py
 kep_solver/fileio.py
 kep_solver/generation.py
 kep_solver/graph.py
 kep_solver/model.py
 kep_solver/pool.py
```

### Comparing `kep_solver-2.3.1/notebooks/Match Run.ipynb` & `kep_solver-2.4.0/notebooks/Match Run.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/notebooks/README.md` & `kep_solver-2.4.0/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/notebooks/Statistical Analysis.ipynb` & `kep_solver-2.4.0/notebooks/Statistical Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/paper/paper.bib` & `kep_solver-2.4.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/paper/paper.md` & `kep_solver-2.4.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/pyproject.toml` & `kep_solver-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_fileio.py` & `kep_solver-2.4.0/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_generator.py` & `kep_solver-2.4.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_graph.py` & `kep_solver-2.4.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-1.json` & `kep_solver-2.4.0/tests/test_instances/large-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-10.json` & `kep_solver-2.4.0/tests/test_instances/large-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-2.json` & `kep_solver-2.4.0/tests/test_instances/large-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-3.json` & `kep_solver-2.4.0/tests/test_instances/large-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-4.json` & `kep_solver-2.4.0/tests/test_instances/large-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-5.json` & `kep_solver-2.4.0/tests/test_instances/large-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-6.json` & `kep_solver-2.4.0/tests/test_instances/large-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-7.json` & `kep_solver-2.4.0/tests/test_instances/large-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-8.json` & `kep_solver-2.4.0/tests/test_instances/large-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/large-9.json` & `kep_solver-2.4.0/tests/test_instances/large-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-1.json` & `kep_solver-2.4.0/tests/test_instances/medium-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-10.json` & `kep_solver-2.4.0/tests/test_instances/medium-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-2.json` & `kep_solver-2.4.0/tests/test_instances/medium-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-3.json` & `kep_solver-2.4.0/tests/test_instances/medium-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-4.json` & `kep_solver-2.4.0/tests/test_instances/medium-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-5.json` & `kep_solver-2.4.0/tests/test_instances/medium-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-6.json` & `kep_solver-2.4.0/tests/test_instances/medium-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-7.json` & `kep_solver-2.4.0/tests/test_instances/medium-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-8.json` & `kep_solver-2.4.0/tests/test_instances/medium-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/medium-9.json` & `kep_solver-2.4.0/tests/test_instances/medium-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test1.json` & `kep_solver-2.4.0/tests/test_instances/test1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test1.xml` & `kep_solver-2.4.0/tests/test_instances/test1.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test1.yaml` & `kep_solver-2.4.0/tests/test_instances/test1.yaml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test10.json` & `kep_solver-2.4.0/tests/test_instances/test10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test10_output.json` & `kep_solver-2.4.0/tests/test_instances/test10_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test10_output.xml` & `kep_solver-2.4.0/tests/test_instances/test10_output.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test1_output.json` & `kep_solver-2.4.0/tests/test_instances/test1_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test1_output.xml` & `kep_solver-2.4.0/tests/test_instances/test1_output.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test2.json` & `kep_solver-2.4.0/tests/test_instances/test2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test2.xml` & `kep_solver-2.4.0/tests/test_instances/test2.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test2.yaml` & `kep_solver-2.4.0/tests/test_instances/test2.yaml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test3.json` & `kep_solver-2.4.0/tests/test_instances/test3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test3.xml` & `kep_solver-2.4.0/tests/test_instances/test3.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test3b.json` & `kep_solver-2.4.0/tests/test_instances/test3b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test3b.xml` & `kep_solver-2.4.0/tests/test_instances/test3b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test3b.yaml` & `kep_solver-2.4.0/tests/test_instances/test3b.yaml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test4.json` & `kep_solver-2.4.0/tests/test_instances/test4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test4.xml` & `kep_solver-2.4.0/tests/test_instances/test4.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test4.yaml` & `kep_solver-2.4.0/tests/test_instances/test4.yaml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test5.json` & `kep_solver-2.4.0/tests/test_instances/test5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test5.xml` & `kep_solver-2.4.0/tests/test_instances/test5.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test6a.json` & `kep_solver-2.4.0/tests/test_instances/test6a.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test6a.xml` & `kep_solver-2.4.0/tests/test_instances/test6a.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test6b.json` & `kep_solver-2.4.0/tests/test_instances/test6b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test6b.xml` & `kep_solver-2.4.0/tests/test_instances/test6b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test7.json` & `kep_solver-2.4.0/tests/test_instances/test7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test7.yaml` & `kep_solver-2.4.0/tests/test_instances/test7.yaml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test8.json` & `kep_solver-2.4.0/tests/test_instances/test8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test8b.json` & `kep_solver-2.4.0/tests/test_instances/test8b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test8c.json` & `kep_solver-2.4.0/tests/test_instances/test8c.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test9_output.json` & `kep_solver-2.4.0/tests/test_instances/test9_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_instances/test9_output.xml` & `kep_solver-2.4.0/tests/test_instances/test9_output.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_model.py` & `kep_solver-2.4.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_output.py` & `kep_solver-2.4.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.3.1/tests/test_pool.py` & `kep_solver-2.4.0/tests/test_pool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,260 +1,317 @@
 import pytest
 
 import kep_solver.model as model
 import kep_solver.pool as pool
 import kep_solver.fileio as fileio
 
 
-@pytest.fixture(scope="module")
-def transplant_pool():
+@pytest.fixture(
+    scope="module",
+    params=[
+        ("CycleAndChainModel", model.CycleAndChainModel),
+        ("PICEF", model.PICEF),
+    ],
+)
+def transplant_pool_details(request):
     obj = model.TransplantCount()
-    return pool.Pool([obj], description="Test Pool", maxCycleLength=3, maxChainLength=3)
+    yield (
+        request.param[0],
+        pool.Pool(
+            [obj],
+            description="Test Pool",
+            maxCycleLength=3,
+            maxChainLength=3,
+            model=request.param[1],
+            full_details=request.param[0] == "CycleAndChainModel",
+        ),
+    )
 
 
-def test_transplant_count_test1(transplant_pool) -> None:
+def test_transplant_count_test1(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test1.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 3
 
 
-def test_transplant_count_possible(transplant_pool) -> None:
+def test_transplant_count_possible(transplant_pool_details) -> None:
     for testfile in [
         "tests/test_instances/test1.json",
         "tests/test_instances/test2.json",
         "tests/test_instances/test3.json",
         "tests/test_instances/test3b.json",
         "tests/test_instances/test4.json",
         "tests/test_instances/test5.json",
     ]:
         instance = fileio.read_json(testfile)
-        solution, _ = transplant_pool.solve_single(instance)
+        solution, _ = transplant_pool_details[1].solve_single(instance)
         for exchange in solution.possible:
             assert len(exchange.exchange) == exchange.values[0]
 
 
-def test_transplant_count_test2(transplant_pool) -> None:
+def test_transplant_count_test2(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test2.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 6
 
 
-def test_transplant_count_test3(transplant_pool) -> None:
+def test_transplant_count_test3(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test3.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 3
 
 
-def test_transplant_count_test3b(transplant_pool) -> None:
+def test_transplant_count_test3b(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test3b.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 4
 
 
-def test_transplant_count_test4(transplant_pool) -> None:
+def test_transplant_count_test4(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test4.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 3
 
 
-def test_transplant_count_test5(transplant_pool) -> None:
+def test_transplant_count_test5(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test5.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 4
 
 
-def test_transplant_count_medium1(transplant_pool) -> None:
+def test_transplant_count_medium1(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-1.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 23
 
 
-def test_transplant_count_medium2(transplant_pool) -> None:
+def test_transplant_count_medium2(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-2.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 22
 
 
-def test_transplant_count_medium3(transplant_pool) -> None:
+def test_transplant_count_medium3(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-3.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 22
 
 
-def test_transplant_count_medium4(transplant_pool) -> None:
+def test_transplant_count_medium4(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-4.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 19
 
 
-def test_transplant_count_medium5(transplant_pool) -> None:
+def test_transplant_count_medium5(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-5.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 23
 
 
-def test_transplant_count_medium6(transplant_pool) -> None:
+def test_transplant_count_medium6(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-6.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 23
 
 
-def test_transplant_count_medium7(transplant_pool) -> None:
+def test_transplant_count_medium7(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-7.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 23
 
 
-def test_transplant_count_medium8(transplant_pool) -> None:
+def test_transplant_count_medium8(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-8.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 18
 
 
-def test_transplant_count_medium9(transplant_pool) -> None:
+def test_transplant_count_medium9(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-9.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 30
 
 
-def test_transplant_count_medium10(transplant_pool) -> None:
+def test_transplant_count_medium10(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/medium-10.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 21
 
 
-def test_transplant_count_large1(transplant_pool) -> None:
+def test_transplant_count_large1(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-1.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 146
 
 
-def test_transplant_count_large2(transplant_pool) -> None:
+def test_transplant_count_large2(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-2.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 168
 
 
-def test_transplant_count_large3(transplant_pool) -> None:
+def test_transplant_count_large3(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-3.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 161
 
 
-def test_transplant_count_large4(transplant_pool) -> None:
+def test_transplant_count_large4(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-4.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 149
 
 
-def test_transplant_count_large5(transplant_pool) -> None:
+def test_transplant_count_large5(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-5.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 162
 
 
-def test_transplant_count_large6(transplant_pool) -> None:
+def test_transplant_count_large6(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-6.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 152
 
 
-def test_transplant_count_large7(transplant_pool) -> None:
+def test_transplant_count_large7(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-7.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 154
 
 
-def test_transplant_count_large8(transplant_pool) -> None:
+def test_transplant_count_large8(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-8.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 176
 
 
-def test_transplant_count_large9(transplant_pool) -> None:
+def test_transplant_count_large9(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-9.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 174
 
 
-def test_transplant_count_large10(transplant_pool) -> None:
+def test_transplant_count_large10(transplant_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/large-10.json")
-    solution, _ = transplant_pool.solve_single(instance)
+    solution, _ = transplant_pool_details[1].solve_single(instance)
     assert solution.values[0] == 158
 
 
-@pytest.fixture(scope="module")
-def twoway_pool():
+@pytest.fixture(
+    scope="module",
+    params=[
+        ("CycleAndChainModel", model.CycleAndChainModel),
+        # ("PICEF", model.PICEF),  Cannot optimise this objective
+    ],
+)
+def twoway_pool_details(request):
     obj = model.EffectiveTwoWay()
-    return pool.Pool([obj], description="Test Pool", maxCycleLength=3, maxChainLength=3)
+    yield (
+        request.param[0],
+        pool.Pool(
+            [obj],
+            description="Test Pool",
+            maxCycleLength=3,
+            maxChainLength=3,
+            model=request.param[1],
+        ),
+    )
 
 
-def test_effective_twoway_count_test1(twoway_pool) -> None:
+def test_effective_twoway_count_test1(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test1.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 1
 
 
-def test_effective_twoway_count_test2(twoway_pool) -> None:
+def test_effective_twoway_count_test2(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test2.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 3
 
 
-def test_effective_twoway_count_test3(twoway_pool) -> None:
+def test_effective_twoway_count_test3(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test3.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 1
 
 
-def test_effective_twoway_count_test3b(twoway_pool) -> None:
+def test_effective_twoway_count_test3b(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test3b.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 2
 
 
-def test_effective_twoway_count_test4(twoway_pool) -> None:
+def test_effective_twoway_count_test4(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test4.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 1
 
 
-def test_effective_twoway_count_test5(twoway_pool) -> None:
+def test_effective_twoway_count_test5(twoway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test5.json")
-    solution, _ = twoway_pool.solve_single(instance)
+    solution, _ = twoway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 2
 
 
-@pytest.fixture(scope="module")
-def backarc_pool():
+@pytest.fixture(
+    scope="module",
+    params=[
+        ("CycleAndChainModel", model.CycleAndChainModel),
+        # ("PICEF", model.PICEF),  # Cannot optimise this objective
+    ],
+)
+def backarc_pool_details(request):
     obj = model.BackArcs()
-    return pool.Pool(
-        [obj],
-        description="Test Pool",
-        maxCycleLength=3,
-        maxChainLength=3,
-        build_alt_embed=1,
+    yield (
+        request.param[0],
+        pool.Pool(
+            [obj],
+            description="Test Pool",
+            maxCycleLength=3,
+            maxChainLength=3,
+            build_alt_embed=1,
+            model=request.param[1],
+        ),
     )
 
 
-def test_backarcs_test3(backarc_pool) -> None:
+def test_backarcs_test3(backarc_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test3b.json")
-    solution, _ = backarc_pool.solve_single(instance)
+    solution, _ = backarc_pool_details[1].solve_single(instance)
     assert solution.values[0] == 3
 
 
-def test_backarcs_test5(backarc_pool) -> None:
+def test_backarcs_test5(backarc_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test5.json")
-    solution, _ = backarc_pool.solve_single(instance)
+    solution, _ = backarc_pool_details[1].solve_single(instance)
     assert solution.values[0] == 2
 
 
-@pytest.fixture(scope="module")
-def threeway_pool():
+@pytest.fixture(
+    scope="module",
+    params=[
+        ("CycleAndChainModel", model.CycleAndChainModel),
+        # ("PICEF", model.PICEF),  Cannot optimise this objective
+    ],
+)
+def threeway_pool_details(request):
     obj = model.ThreeWay()
-    return pool.Pool([obj], description="Test Pool", maxCycleLength=3, maxChainLength=3)
+    yield (
+        request.param[0],
+        pool.Pool(
+            [obj],
+            description="Test Pool",
+            maxCycleLength=3,
+            maxChainLength=3,
+            build_alt_embed=1,
+            model=request.param[1],
+        ),
+    )
 
 
-def test_threeway_count_test1(threeway_pool) -> None:
+def test_threeway_count_test1(threeway_pool_details) -> None:
     instance = fileio.read_json("tests/test_instances/test1.json")
-    solution, _ = threeway_pool.solve_single(instance)
+    solution, _ = threeway_pool_details[1].solve_single(instance)
     assert solution.values[0] == 0
```

### Comparing `kep_solver-2.3.1/tests/test_statistics.py` & `kep_solver-2.4.0/tests/test_statistics.py`

 * *Files identical despite different names*

