# Comparing `tmp/hydra_genetics-2.0.1.tar.gz` & `tmp/hydra_genetics-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_genetics-2.0.1.tar", last modified: Thu Apr 25 12:35:29 2024, max compression
+gzip compressed data, was "hydra_genetics-3.0.0.tar", last modified: Thu May 30 08:06:27 2024, max compression
```

## Comparing `hydra_genetics-2.0.1.tar` & `hydra_genetics-3.0.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.481269 hydra_genetics-2.0.1/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 12:35:29.481269 hydra_genetics-2.0.1/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51186 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/commands/prep_pipeline_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/commands/references.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/test-build-mkdocs
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.461269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.469269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/config/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/output_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (127)    61275 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/images/hydragenetics.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/rules/common.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.473269 hydra_genetics-2.0.1/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/rule-template/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/rule-template/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/rule-template/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/rule-template/skeleton_rule.smk
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/rule-template/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/software_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 12:35:29.000000 hydra_genetics-2.0.1/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 12:35:29.481269 hydra_genetics-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (127)    87635 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:29.477269 hydra_genetics-2.0.1/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    28006 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    80044 2024-04-25 12:35:26.000000 hydra_genetics-2.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.248502 hydra_genetics-3.0.0/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51186 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/commands/references.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/test-build-mkdocs
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.244502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.252502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/output_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    61275 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.256502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22146 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/software_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 08:06:27.000000 hydra_genetics-3.0.0/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.260502 hydra_genetics-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114087 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:27.264502 hydra_genetics-3.0.0/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28006 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80044 2024-05-30 08:06:24.000000 hydra_genetics-3.0.0/versioneer.py
```

### Comparing `hydra_genetics-2.0.1/LICENSE.md` & `hydra_genetics-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/PKG-INFO` & `hydra_genetics-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 2.0.1
+Version: 3.0.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hydra-genetics Version: 2.0.1 Summary: Helper tools
+Metadata-Version: 2.1 Name: hydra-genetics Version: 3.0.0 Summary: Helper tools
 for use with hydra-genetics pipelines. Home-page: https://github.com/hydra-
 genetics/tools Author: Patrik Smeds Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3 Keywords: hydra-
 genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next
 generation sequencing Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: pandas>=1.3.1 Requires-Dist: click<9,>=8 Requires-
 Dist: jinja2==3.0.1 Requires-Dist: rich==10.9.0 Requires-Dist: snakemake
```

### Comparing `hydra_genetics-2.0.1/README.md` & `hydra_genetics-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/__init__.py` & `hydra_genetics-3.0.0/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/__main__.py` & `hydra_genetics-3.0.0/hydra_genetics/__main__.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/commands/create.py` & `hydra_genetics-3.0.0/hydra_genetics/commands/create.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/commands/prep_pipeline_env.py` & `hydra_genetics-3.0.0/hydra_genetics/commands/prep_pipeline_env.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/commands/references.py` & `hydra_genetics-3.0.0/hydra_genetics/commands/references.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/.github/workflows/test-build-mkdocs` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/.github/workflows/test-build-mkdocs`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/LICENSE.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/README.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/README.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/extra.css` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/extra.css`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/docs/index.md` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/images/hydragenetics.png` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/images/hydragenetics.png`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/mkdocs.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/rules/common.smk` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/rules/common.smk`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/rule-template/config.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/rule-template/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/rule-template/resources.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/rule-template/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/rule-template/rules.schema.yaml` & `hydra_genetics-3.0.0/hydra_genetics/rule-template/rules.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra_genetics-3.0.0/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/chr.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/hotspot.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/hotspot_report.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/hotspot_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,17 +263,15 @@
                     for index, variant in enumerate(hotspot.VARIANTS):
                         # even though no variants were found print hotspot and region all entries
                         if not variant['variants'] and not variant['extended']:
                             depth = get_depth(depth_data,
                                               chr_translater.get_chr_value(hotspot.CHROMOSOME),
                                               hotspot.EXTENDED_START + index-1,
                                               hotspot.EXTENDED_START + index)
-                            if hotspot.REPORT == ReportClass.region_all and depth > 299:  # ToDo remove harcoded value
-                                continue
-                            elif hotspot.ALWAYS_PRINT:
+                            if hotspot.ALWAYS_PRINT:
                                 data = {'sample': sample,
                                         'chr': hotspot.CHROMOSOME,
                                         'start': hotspot.EXTENDED_START + index,
                                         'stop': hotspot.EXTENDED_START + index,
                                         'ref': '-',
                                         'alt': '-',
                                         'report':  utils.format_report_type(hotspot),
```

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/multibp.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/reference.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/reference.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/io/utils.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/misc.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/models/hotspot.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/samples.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/software_versions.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/software_versions.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,60 +9,59 @@
 from datetime import datetime
 from snakemake.common import is_local_file
 
 
 def _create_container_name_version_string(image_information):
     if image_information.endswith(".sif"):
         container_name_and_version = re.search(r"__([A-Za-z0-9-]+)_([A-Za-z0-9.-]+)\.sif$", image_information)
-        print(container_name_and_version)
         if container_name_and_version:
             return "_".join(container_name_and_version.groups())
         else:
             container_name = re.search(r"([A-Za-z0-9-]+)\.sif$", image_information)
             if container_name:
-                return "_".join([container_name.groups()[0], 'NoVersion'])
+                return "_".join([container_name.groups()[0], "NoVersion"])
             else:
                 raise Exception(f"Unable to extract container name from {image_information}")
     else:
         container_name_and_version = re.search("/([A-Za-z0-9-_.]+):[ ]*([A-Za-z0-9-_.]+)$", image_information)
         if container_name_and_version:
             return "_".join(container_name_and_version.groups())
         else:
             container_name = re.search("/([A-Za-z0-9-]+)$", image_information)
             if container_name:
-                return "_".join([container_name.groups()[0], 'NoVersion'])
+                return "_".join([container_name.groups()[0], "NoVersion"])
             else:
                 raise Exception(f"Unable to extract container name from {image_information}")
 
 
 def add_version_files_to_multiqc(config, file_list):
-    for report in config['multiqc']['reports']:
-        config['multiqc']['reports'][report]['qc_files'] += file_list
+    for report in config["multiqc"]["reports"]:
+        config["multiqc"]["reports"][report]["qc_files"] += file_list
 
 
 def _touch(fname):
     if os.path.exists(fname):
         os.utime(fname, None)
     else:
-        open(fname, 'a').close()
+        open(fname, "a").close()
 
 
 def get_container_prefix(workflow):
-    '''
+    """
     Function used to fetch singularity cache location
-    '''
+    """
 
-    if hasattr(workflow, 'use_singularity'):
+    if hasattr(workflow, "use_singularity"):
         # Fetch singularity prefix for snakemake version with version less
         # then 8
-        if hasattr(workflow, 'singularity_prefix'):
+        if hasattr(workflow, "singularity_prefix"):
             return workflow.singularity_prefix
         else:
             return ".snakemake/singularity"
-    elif hasattr(workflow, 'deployment_settings'):
+    elif hasattr(workflow, "deployment_settings"):
         # Fetch singularity prefix for snakemake version with equal to 8.0 or newer
         if workflow.deployment_settings.apptainer_prefix is None:
             return ".snakemake/singularity"
         else:
             return workflow.deployment_settings.apptainer_prefix
     return None
 
@@ -76,22 +75,24 @@
     workflow: object
         workflow object from snakemake that contain a basedir attribute
 
     Return
     ------
     dict with pipeline version and commit, ex {'pipeline_version': 'v1', 'pipeline_commit': 'achgk2...kacaa'}
     """
+
     def _find_root_repo(path):
         if path is None:
             return None
         elif os.path.isdir(str(os.path.join(str(path), ".git"))):
             return path
         else:
             return _find_root_repo(os.path.dirname(path))
-    repo_path = _find_root_repo(getattr(workflow, 'basedir'))
+
+    repo_path = _find_root_repo(getattr(workflow, "basedir"))
 
     # Initialize a Git repo object
     repo = git.Repo(repo_path)
 
     # Get the currently checked out commit
     head_commit = repo.head.commit
 
@@ -104,19 +105,19 @@
     if pipeline_version is None:
         try:
             pipeline_version = repo.active_branch
         except TypeError as e:
             logger = logging.getLogger(__name__)
             logger.warning("Unable to get version (from tags) or an active_branch")
 
-    return {'pipeline_version': str(pipeline_version), 'pipeline_commit': str(head_commit)}
+    return {"pipeline_version": str(pipeline_version), "pipeline_commit": str(head_commit)}
 
 
 def get_software_version_from_labels(image_path):
-    '''
+    """
     Function used to create a list of software version used in a singularity image,
     usually created from a docker image. The software name and version will be extracted
     from labels that have been set in the container.  The expected format is
     ([A-Za-z0-9-_.]+): ([0-9.]+)$, where the first section is the software name
     and second part is the version. In the dockerfile the labels could look like this
     LABEL gatk4=4.11.0
 
@@ -125,20 +126,21 @@
     image_path: str
        path to the image that will be inspected
 
     Returns:
     --------
     list of tuples where each tuple consist of software name and software version.
 
-    '''
+    """
     cmd = ["singularity", "inspect", image_path]
     software_version_list = []
     for row in subprocess.check_output(cmd).decode().split("\n"):
-        if not row.startswith("org.label-schema") and not row.startswith("maintainer"):
-            software_version = re.match("^([A-Za-z0-9-_.]+): ([0-9.]+)$", row)
+
+        if not row.startswith("org.") and not row.startswith("maintainer") and not row.startswith("license"):
+            software_version = re.match("^([A-Za-z0-9-_.]+): ([a-z0-9.]+)$", row)
             if software_version:
                 software_version_list.append(software_version.groups())
     return software_version_list
 
 
 def get_deffile(image_path):
     """
@@ -158,15 +160,15 @@
     for row in subprocess.check_output(cmd).decode().split("\n"):
         if row.startswith("org.label-schema.usage.singularity.deffile.from"):
             return row.split(": ")[1]
     return None
 
 
 def get_image_path(container, singularity_prefix_path):
-    '''
+    """
     Function used to return a path to singularity a image. If it's a local file, .i.e
     a path to a file on the file system the path will be returned without modifications. If it's
     a singularity image that has been downloaded by snakemake the function will create
     the snakemake generated image name and path, which is the singularity prefix as storage
     location followed by a hashname (generated from the provided docker image name and location).
 
     Parameters
@@ -175,43 +177,44 @@
         either a path to a local file or image name and type, ex docker://hydragenetics/bcbio-vc:0.2.6
     :singularity_prefix_path: str
         storage path of singularity/apptainer images
 
     Returns
     -------
     str: path to locally store image
-    '''
+    """
     if is_local_file(container):
         return container
 
     md5hash = hashlib.md5()
     md5hash.update(container.encode())
     return os.path.join(singularity_prefix_path, f"{md5hash.hexdigest()}.simg")
 
 
 def use_container(workflow):
-    '''
+    """
     Function used to check if containers are used,
-    '''
-    if hasattr(workflow, 'use_singularity'):
+    """
+    if hasattr(workflow, "use_singularity"):
         # For snakemake with version less then 8
         return True
-    elif hasattr(workflow, 'deployment_settings') and workflow.deployment_settings.deployment_method:
+    elif hasattr(workflow, "deployment_settings") and workflow.deployment_settings.deployment_method:
         # For snakemake with version 8 or newer
         from snakemake.settings import DeploymentMethod
+
         if DeploymentMethod.APPTAINER in workflow.deployment_settings.deployment_method:
             return True
         else:
             return False
     else:
         return False
 
 
 def add_software_version_to_config(config, workflow, fail_missing_versions=True):
-    '''
+    """
     Function that will look through the config dict to locate
     container definitions. When container information is found the
     softwares version will be extracted and added to the config.
 
     Parameters:
     config: dict
         snakemake dict object
@@ -219,182 +222,149 @@
         snakemake workflow object
     fail_missing_versions: boolean
         if set to true an error will be raised if a container is specified
         and versions can't be extracted.
 
     Returns:
     a config where software_verions have been added
-    '''
+    """
     container_cache = get_container_prefix(workflow)
 
     def _add_software_version(config, version_dict):
         logger = logging.getLogger(__name__)
         version_found = []
-        software_version_key = 'software_versions'
+        software_version_key = "software_versions"
         for key, value in config.items():
             if isinstance(value, dict):
                 config[key], version_dict = _add_software_version(value, version_dict)
             elif key in ["container", "default_container"]:
                 if key == "default_container":
                     software_version_key = f"default_container_software_versions"
                 image_path = get_image_path(value, container_cache)
                 if os.path.isfile(image_path):
                     version_found += get_software_version_from_labels(image_path)
-                    if not is_local_file(value):
-                        name_and_version = _create_container_name_version_string(value)
-                    else:
-                        name_and_version = _create_container_name_version_string(get_software_version_from_labels(value))
+                    name_and_version = _create_container_name_version_string(value)
 
                     if not version_found:
                         if fail_missing_versions:
                             raise Exception(f"could not extract software versions from {image_path}, {value}")
                         else:
                             logger.warning(f"could not extract software versions from {image_path}, {value}")
                             name = name_and_version.split("_")[0]
                             version = "_".join(name_and_version.split("_")[1:])
-                            version_found = [[name, version],
-                                             ('NOTE', 'version extract from image name and not labels')]
+                            version_found = [[name, version], ("NOTE", "version extract from image name and not labels")]
                 else:
                     if fail_missing_versions:
                         raise Exception(f"could not locate local file {image_path} for {value}")
                     else:
                         logger.warning(f"could not locate local file {image_path} for {value}")
         if version_found:
             config[software_version_key] = {s: v for s, v in version_found}
-            if 'version' in config[software_version_key]:
-                del config[software_version_key]['version']
+            if "version" in config[software_version_key]:
+                del config[software_version_key]["version"]
             version_dict[name_and_version] = config[software_version_key]
         return config, version_dict
-    return _add_software_version(config, {})
-
-
-def touch_software_version_files(config, directory="versions/software", file_name_ending="mqc_versions.yaml", date_string=None):
 
-    def _create_name_list(_config, name_list=None):
-        for key, value in _config.items():
-            if isinstance(value, dict):
-                name_list = _create_name_list(value, name_list)
-            elif key in ["container", "default_container"]:
-                name_list.append(_create_container_name_version_string(value))
-        return name_list
-
-    if date_string is None:
-        date_string = datetime.now().strftime('%Y%m%d')
-        if directory is not None and len(directory) > 0:
-            date_string = f"_{date_string}"
-            directory = f"{directory}{date_string}"
-        if len(directory) > 0 and not os.path.isdir(directory):
-            os.makedirs(directory)
-            output_file_list = []
-        for name in _create_name_list(config, []):
-            output_file = os.path.join(directory, f"{name}_{file_name_ending}")
-            output_file_list.append(output_file)
-    _touch(output_file)
-    return output_file_list
+    return _add_software_version(config, {})
 
 
-def export_software_version_as_files(software_dict, directory="versions/software", file_name_ending="mqc_versions.yaml", date_string=None):
+def export_software_version_as_file(
+    software_dict, directory="versions/software", file_name="softwares_mqc_versions.yaml", date_string=None
+):
     """
-    Print software version to files. Requires a dict with key software_info which
+    Print software version to file (should be same as filename in touch_software_version_file). Requires a dict with key software_info which
     should contain a dict with software names and versions.
 
     Parameters:
     -----------
     software_dict: dict
        dict with key software_info, ex {software_info: {'common_1.3': {'samtools': '1.3', 'picard': '1.6'}}}
     directory: str
        path where files will be written
-    file_name_ending: str
-       a string that will be combined with the software name version key
+    file_name: str
+       file name to use for software logging
     date_string: str
        a string that will be added to the folder name to make it unique
     """
     if date_string is None:
-        date_string = datetime.now().strftime('%Y%m%d')
+        date_string = datetime.now().strftime("%Y%m%d")
     if directory is not None and len(directory) > 0:
         date_string = f"_{date_string}"
     directory = f"{directory}{date_string}"
     if len(directory) > 0 and not os.path.isdir(directory):
         os.makedirs(directory)
-    output_file_list = []
-    for name in software_dict:
-        output_file = os.path.join(directory, f"{name}_{file_name_ending}")
-        output_file_list.append(output_file)
-        with open(output_file, 'w') as writer:
-            notification = software_dict[name].pop('NOTE', None)
-            writer.write(yaml.dump(software_dict[name]))
+    output_file = os.path.join(directory, f"{file_name}")
+    with open(output_file, "w") as writer:
+        writer.write(yaml.dump(software_dict))
+        for name in software_dict:
+            notification = software_dict[name].pop("NOTE", None)
             if notification is not None:
                 writer.write(f"# {notification}")
-    return output_file_list
+    return output_file
 
 
-def touch_software_version_files(config, directory="versions/software", file_name_ending="mqc_versions.yaml", date_string=None):
+def touch_software_version_file(config, directory="versions/software", file_name="softwares_mqc_versions.yaml", date_string=None):
     """
     To be able to pass a proper file list to multiqc the version files need to exist before the dag graph
     is built. And before the dag graph is built we can not guarantee that all images exist on the file system,
-    and therefor we can not use export_software_version_as_files to directly create the actual version files.
-    This function will create all files (empty) that export_software_version_as_files will create.
-    NOTE: you need to have the same parameter as with export_software_version_as_files
+    and therefor we can not use export_software_version_as_file to directly create the actual version files.
+    This function will create all files (empty) that export_software_version_as_file will create.
+    NOTE: you need to have the same parameter as with export_software_version_as_file
 
     Parameters:
     -----------
-    software_dict: dict
-       dict with key software_info, ex {software_info: {'common_1.3': {'samtools': '1.3', 'picard': '1.6'}}}
+    config: dict
+       dict with config file # not used?
     directory: str
        path where files will be written
-    file_name_ending: str
-       a string that will be combined with the software name version key
+    file_name: str
+       file name to use for software version logging
     date_string: str
        a string that will be added to the folder name to make it unique
     """
 
-    def _create_name_list(_config, name_list=None):
-        for key, value in _config.items():
-            if isinstance(value, dict):
-                name_list = _create_name_list(value, name_list)
-            elif key in ["container", "default_container"]:
-                name_list.append(_create_container_name_version_string(value))
-        return name_list
-
     if date_string is None:
-        date_string = datetime.now().strftime('%Y%m%d')
+        date_string = datetime.now().strftime("%Y%m%d")
     if directory is not None and len(directory) > 0:
         date_string = f"_{date_string}"
         directory = f"{directory}{date_string}"
     if len(directory) > 0 and not os.path.isdir(directory):
         os.makedirs(directory)
-    output_file_list = []
-    for name in _create_name_list(config, []):
-        output_file = os.path.join(directory, f"{name}_{file_name_ending}")
-        output_file_list.append(output_file)
-        _touch(output_file)
-    return output_file_list
+    output_file = os.path.join(directory, f"{file_name}")
+    _touch(output_file)
+
+    if not file_name.endswith("mqc_versions.yaml"):
+        logger = logging.getLogger(__name__)
+        logger.warning(f"{file_name} is not going to be recognized by MultiQC. Should end with mqc_versions.yaml")
+    return output_file
 
 
-def get_pipeline_version(workflow, pipeline_name='pipeline'):
+def get_pipeline_version(workflow, pipeline_name="pipeline"):
     """
     Will return the pipelines tag name and commit hex.
 
     Parameters:
     -----------
     workflow: object
         workflow object from snakemake that contain a basedir attribute
 
     Return
     ------
     dict with pipeline version and commit, ex {'pipeline_name': {'version': 'v1', 'pipeline_commit': 'achgk2...kacaa'}}
     """
+
     def _find_root_repo(path):
         if path is None:
             return None
         elif os.path.isdir(str(os.path.join(str(path), ".git"))):
             return path
         else:
             return _find_root_repo(os.path.dirname(path))
-    repo_path = _find_root_repo(getattr(workflow, 'basedir'))
+
+    repo_path = _find_root_repo(getattr(workflow, "basedir"))
 
     # Initialize a Git repo object
     repo = git.Repo(repo_path)
 
     # Get the currently checked out commit
     head_commit = repo.head.commit
 
@@ -407,21 +377,20 @@
     if pipeline_version is None:
         try:
             pipeline_version = repo.active_branch
         except TypeError as e:
             logger = logging.getLogger(__name__)
             logger.warning("Unable to get version (from tags) or an active_branch")
 
-    return {pipeline_name: {'version': str(pipeline_version), 'commit_id': str(head_commit)}}
+    return {pipeline_name: {"version": str(pipeline_version), "commit_id": str(head_commit)}}
 
 
-def export_pipeline_version_as_file(pipeline_version_dict,
-                                    directory="versions/software",
-                                    file_name_ending="mqc_versions.yaml",
-                                    date_string=None):
+def export_pipeline_version_as_file(
+    pipeline_version_dict, directory="versions/software", file_name_ending="mqc_versions.yaml", date_string=None
+):
     """
     Print pipeline version to a file. Requires a dict with key pipeline_info which
     should contain a dict with software names and versions.
 
     Parameters:
     -----------
     pipeline_version_dict: dict
@@ -430,61 +399,62 @@
        path where files will be written
     file_name_ending: str
        a string that will be combined with the software name version key
     date_string: str
        a string that will be added to the folder name to make it unique
     """
     if date_string is None:
-        date_string = datetime.now().strftime('%Y%m%d')
+        date_string = datetime.now().strftime("%Y%m%d")
     if directory is not None and len(directory) > 0:
         date_string = f"_{date_string}"
     directory = f"{directory}{date_string}"
     if len(directory) > 0 and not os.path.isdir(directory):
         os.makedirs(directory)
     output_file_list = []
     for pipeline_name in pipeline_version_dict:
-        output_file = os.path.join(directory,
-                                   f"{pipeline_name}__{pipeline_version_dict[pipeline_name]['version']}_{file_name_ending}")
+        output_file = os.path.join(
+            directory, f"{pipeline_name}__{pipeline_version_dict[pipeline_name]['version']}_{file_name_ending}"
+        )
         output_file_list.append(output_file)
-        with open(output_file, 'w') as writer:
-            writer.write(yaml.dump({pipeline_name: pipeline_version_dict[pipeline_name]['version']}))
+        with open(output_file, "w") as writer:
+            writer.write(yaml.dump({pipeline_name: pipeline_version_dict[pipeline_name]["version"]}))
     return output_file_list
 
 
-def touch_pipeline_verion_file_name(pipeline_version_dict,
-                                    directory="versions/software",
-                                    file_name_ending="mqc_versions.yaml",
-                                    date_string=None):
+def touch_pipeline_version_file_name(
+    pipeline_version_dict, directory="versions/software", file_name_ending="mqc_versions.yaml", date_string=None
+):
     """
     Function used to create empty version file for pipeline version. This
     function is a bit redundant and export_pipeline_version_as_file could be used,
     since this function isn't dependent on singularity images which
-    export_software_version_as_files is. But the function exist to have a similar workflow
+    export_software_version_as_file is. But the function exist to have a similar workflow
     for both pipeline and software. NOTE: you need to have same parameters into
-    touch_pipeline_verion_file_name as to export_pipeline_version_as_file.
+    touch_pipeline_version_file_name as to export_pipeline_version_as_file.
 
     Parameters:
     -----------
     pipeline_version_dict: dict
        dict with key pipeline_version_dict, ex {pipeline_name: {'version': '1.3', 'commit_id': 'ac8ac8t73'}}
     directory: str
        path where files will be written
     file_name_ending: str
        a string that will be combined with the software name version key
     date_string: str
        a string that will be added to the folder name to make it unique
     """
     if date_string is None:
-        date_string = datetime.now().strftime('%Y%m%d')
+        date_string = datetime.now().strftime("%Y%m%d")
     if directory is not None and len(directory) > 0:
         date_string = f"_{date_string}"
     directory = f"{directory}{date_string}"
     if len(directory) > 0 and not os.path.isdir(directory):
         os.makedirs(directory)
 
     output_file_list = []
     for pipeline_name in pipeline_version_dict:
-        output_file = os.path.join(directory,
-                                   f"{pipeline_name}__{pipeline_version_dict[pipeline_name]['version']}_{file_name_ending}")
+        output_file = os.path.join(
+            directory, f"{pipeline_name}__{pipeline_version_dict[pipeline_name]['version']}_{file_name_ending}"
+        )
         output_file_list.append(output_file)
         _touch(output_file)
     return output_file_list
```

### Comparing `hydra_genetics-2.0.1/hydra_genetics/utils/units.py` & `hydra_genetics-3.0.0/hydra_genetics/utils/units.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/hydra_genetics.egg-info/PKG-INFO` & `hydra_genetics-3.0.0/hydra_genetics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 2.0.1
+Version: 3.0.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hydra-genetics Version: 2.0.1 Summary: Helper tools
+Metadata-Version: 2.1 Name: hydra-genetics Version: 3.0.0 Summary: Helper tools
 for use with hydra-genetics pipelines. Home-page: https://github.com/hydra-
 genetics/tools Author: Patrik Smeds Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3 Keywords: hydra-
 genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next
 generation sequencing Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: pandas>=1.3.1 Requires-Dist: click<9,>=8 Requires-
 Dist: jinja2==3.0.1 Requires-Dist: rich==10.9.0 Requires-Dist: snakemake
```

### Comparing `hydra_genetics-2.0.1/hydra_genetics.egg-info/SOURCES.txt` & `hydra_genetics-3.0.0/hydra_genetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/setup.py` & `hydra_genetics-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/io/test_hotspot.py` & `hydra_genetics-3.0.0/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/io/test_mutations_report.py` & `hydra_genetics-3.0.0/tests/utils/io/test_mutations_report.py`

 * *Files 24% similar despite different names*

```diff
@@ -3630,15 +3630,15 @@
 0000e2d0: 7265 665f 6465 7074 6822 2c20 2261 6c74  ref_depth", "alt
 0000e2e0: 5f64 6570 7468 225d 2929 2020 2320 6e6f  _depth"]))  # no
 0000e2f0: 7161 0a20 2020 2020 2020 2020 2020 2072  qa.            r
 0000e300: 6573 756c 7420 3d20 7265 706f 7274 5f72  esult = report_r
 0000e310: 6573 756c 742e 7265 6164 6c69 6e65 7328  esult.readlines(
 0000e320: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
 0000e330: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-0000e340: 656e 2872 6573 756c 7429 2c20 3133 290a  en(result), 13).
+0000e340: 656e 2872 6573 756c 7429 2c20 3335 290a  en(result), 35).
 0000e350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 0000e360: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
 0000e370: 756c 745b 305d 2e72 7374 7269 7028 292c  ult[0].rstrip(),
 0000e380: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
 0000e390: 3030 322e 3131 0932 3934 3435 3237 3109  002.11.29445271.
 0000e3a0: 3239 3434 3532 3731 0947 0941 0931 2d68  29445271.G.A.1-h
 0000e3b0: 6f74 7370 6f74 0936 3230 0933 3539 0934  otspot.620.359.4
@@ -3671,1808 +3671,3461 @@
 0000e560: 372e 3133 0931 3136 3431 3230 3433 0931  7.13.116412043.1
 0000e570: 3136 3431 3230 3433 092d 092d 0931 2d68  16412043.-.-.1-h
 0000e580: 6f74 7370 6f74 0930 092d 092d 2229 0a20  otspot.0.-.-"). 
 0000e590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
 0000e5a0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
 0000e5b0: 6c74 5b35 5d2e 7273 7472 6970 2829 2c20  lt[5].rstrip(), 
 0000e5c0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-0000e5d0: 3032 2e31 3109 3239 3434 3532 3732 0932  02.11.29445272.2
-0000e5e0: 3934 3435 3237 3209 2d09 2d09 332d 6368  9445272.-.-.3-ch
-0000e5f0: 6563 6b09 3232 3109 2d09 2d22 290a 2020  eck.221.-.-").  
+0000e5d0: 3032 2e31 3109 3239 3434 3532 3731 0932  02.11.29445271.2
+0000e5e0: 3934 3435 3237 3109 2d09 2d09 332d 6368  9445271.-.-.3-ch
+0000e5f0: 6563 6b09 3632 3009 2d09 2d22 290a 2020  eck.620.-.-").  
 0000e600: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
 0000e610: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
 0000e620: 745b 365d 2e72 7374 7269 7028 292c 2022  t[6].rstrip(), "
 0000e630: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
-0000e640: 322e 3131 0932 3934 3435 3237 3709 3239  2.11.29445277.29
-0000e650: 3434 3532 3737 092d 092d 0933 2d63 6865  445277.-.-.3-che
-0000e660: 636b 0931 3832 092d 092d 2229 0a20 2020  ck.182.-.-").   
+0000e640: 322e 3131 0932 3934 3435 3237 3209 3239  2.11.29445272.29
+0000e650: 3434 3532 3732 092d 092d 0933 2d63 6865  445272.-.-.3-che
+0000e660: 636b 0932 3231 092d 092d 2229 0a20 2020  ck.221.-.-").   
 0000e670: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
 0000e680: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
 0000e690: 5b37 5d2e 7273 7472 6970 2829 2c20 2273  [7].rstrip(), "s
-0000e6a0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
-0000e6b0: 2e31 3109 3134 3537 3338 3736 3809 3134  .11.145738768.14
-0000e6c0: 3537 3338 3736 3809 4709 4309 332d 6368  5738768.G.C.3-ch
-0000e6d0: 6563 6b09 3135 3437 0935 0932 3722 290a  eck.1547.5.27").
-0000e6e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e6f0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-0000e700: 756c 745b 385d 2e72 7374 7269 7028 292c  ult[8].rstrip(),
-0000e710: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
-0000e720: 3030 382e 3131 0931 3435 3733 3837 3736  008.11.145738776
-0000e730: 0931 3435 3733 3837 3736 092d 092d 0933  .145738776.-.-.3
-0000e740: 2d63 6865 636b 0930 092d 092d 2229 0a20  -check.0.-.-"). 
-0000e750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e760: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-0000e770: 6c74 5b39 5d2e 7273 7472 6970 2829 2c20  lt[9].rstrip(), 
-0000e780: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-0000e790: 3038 2e31 3109 3134 3537 3432 3531 3409  08.11.145742514.
-0000e7a0: 3134 3537 3432 3531 3409 4109 4709 332d  145742514.A.G.3-
-0000e7b0: 6368 6563 6b09 3009 3009 3833 3922 290a  check.0.0.839").
-0000e7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e7d0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-0000e7e0: 756c 745b 3130 5d2e 7273 7472 6970 2829  ult[10].rstrip()
-0000e7f0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-0000e800: 3030 3136 2e31 3109 3831 3935 3437 3839  0016.11.81954789
-0000e810: 0938 3139 3534 3738 3909 4309 4754 0932  .81954789.C.GT.2
-0000e820: 2d69 6e64 656c 0931 3134 3409 3131 3732  -indel.1144.1172
-0000e830: 0932 3922 290a 2020 2020 2020 2020 2020  .29").          
-0000e840: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000e850: 616c 2872 6573 756c 745b 3131 5d2e 7273  al(result[11].rs
-0000e860: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-0000e870: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
-0000e880: 3434 3532 3832 0932 3934 3435 3238 3209  445282.29445282.
-0000e890: 4709 4109 342d 6f74 6865 7209 3532 3009  G.A.4-other.520.
-0000e8a0: 3238 3409 3322 290a 2020 2020 2020 2020  284.3").        
-0000e8b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000e8c0: 7175 616c 2872 6573 756c 745b 3132 5d2e  qual(result[12].
-0000e8d0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
-0000e8e0: 6531 094e 435f 3030 3030 3136 2e31 3109  e1.NC_000016.11.
-0000e8f0: 3831 3935 3437 3839 0938 3139 3534 3738  81954789.8195478
-0000e900: 3909 4309 4709 342d 6f74 6865 7209 3131  9.C.G.4-other.11
-0000e910: 3434 0934 3432 0933 3439 2229 0a0a 2020  44.442.349")..  
-0000e920: 2020 2020 2020 7265 706f 7274 203d 206f        report = o
-0000e930: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-0000e940: 2e74 656d 7064 6972 2c20 2266 696c 7465  .tempdir, "filte
-0000e950: 7265 642e 7265 706f 7274 2229 0a20 2020  red.report").   
-0000e960: 2020 2020 2067 656e 6572 6174 655f 686f       generate_ho
-0000e970: 7473 706f 745f 7265 706f 7274 2822 7361  tspot_report("sa
-0000e980: 6d70 6c65 3122 2c0a 2020 2020 2020 2020  mple1",.        
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 2020 2020 2020 7265 706f 7274 2c0a          report,.
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 6c65 7665 6c73 2c0a 2020 2020 2020 2020  levels,.        
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2020 2020 2020 7365 6c66 2e68 6f74          self.hot
-0000ea00: 7370 6f74 2c0a 2020 2020 2020 2020 2020  spot,.          
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 2020 2020 2020 7365 6c66 2e76 6366 5f76        self.vcf_v
-0000ea30: 6570 202b 2022 2e67 7a22 2c0a 2020 2020  ep + ".gz",.    
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ea60: 2e67 7663 6620 2b20 222e 677a 222c 0a20  .gvcf + ".gz",. 
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ea90: 656c 662e 7265 6665 7265 6e63 652c 0a20  elf.reference,. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000eac0: 656c 662e 7663 665f 7665 705f 776f 5f70  elf.vcf_vep_wo_p
-0000ead0: 6963 6b20 2b20 222e 677a 222c 0a20 2020  ick + ".gz",.   
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-0000eb00: 7374 732f 7574 696c 732f 6669 6c65 732f  sts/utils/files/
-0000eb10: 7265 706f 7274 5f63 6f6c 756d 6e73 5f76  report_columns_v
-0000eb20: 6570 2e79 616d 6c22 290a 2020 2020 2020  ep.yaml").      
-0000eb30: 2020 7769 7468 206f 7065 6e28 7265 706f    with open(repo
-0000eb40: 7274 2c20 2772 2729 2061 7320 7265 706f  rt, 'r') as repo
-0000eb50: 7274 5f72 6573 756c 743a 0a20 2020 2020  rt_result:.     
-0000eb60: 2020 2020 2020 2068 6561 6420 3d20 7265         head = re
-0000eb70: 706f 7274 5f72 6573 756c 742e 7265 6164  port_result.read
-0000eb80: 6c69 6e65 2829 0a20 2020 2020 2020 2020  line().         
-0000eb90: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000eba0: 7561 6c28 6865 6164 2e72 7374 7269 7028  ual(head.rstrip(
-0000ebb0: 292c 2022 5c74 222e 6a6f 696e 285b 2273  ), "\t".join(["s
-0000ebc0: 616d 706c 6522 2c20 2263 6872 222c 2022  ample", "chr", "
-0000ebd0: 7374 6172 7422 2c20 2273 746f 7022 2c20  start", "stop", 
-0000ebe0: 2272 6566 222c 2022 616c 7422 2c20 2272  "ref", "alt", "r
-0000ebf0: 6570 6f72 7422 2c20 2767 7663 665f 6465  eport", 'gvcf_de
-0000ec00: 7074 6827 2c20 2272 6566 5f64 6570 7468  pth', "ref_depth
-0000ec10: 222c 2022 616c 745f 6465 7074 6822 2c20  ", "alt_depth", 
-0000ec20: 2741 6e61 6c79 7a61 626c 6527 2c20 274d  'Analyzable', 'M
-0000ec30: 696e 5f72 6561 645f 6465 7074 6833 3030  in_read_depth300
-0000ec40: 272c 2027 4765 6e65 272c 2027 5661 7269  ', 'Gene', 'Vari
-0000ec50: 616e 745f 7479 7065 272c 2027 436f 6e73  ant_type', 'Cons
-0000ec60: 6571 7565 6e63 6527 2c20 2743 616c 6c65  equence', 'Calle
-0000ec70: 7273 272c 2027 436f 6d6d 656e 7427 5d29  rs', 'Comment'])
-0000ec80: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
-0000ec90: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
-0000eca0: 6570 6f72 745f 7265 7375 6c74 2e72 6561  eport_result.rea
-0000ecb0: 646c 696e 6573 2829 0a20 2020 2020 2020  dlines().       
-0000ecc0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ecd0: 4571 7561 6c28 6c65 6e28 7265 7375 6c74  Equal(len(result
-0000ece0: 292c 2031 3329 0a20 2020 2020 2020 2020  ), 13).         
-0000ecf0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000ed00: 7561 6c28 7265 7375 6c74 5b30 5d2e 7273  ual(result[0].rs
-0000ed10: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-0000ed20: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
-0000ed30: 3434 3532 3731 0932 3934 3435 3237 3109  445271.29445271.
-0000ed40: 4709 4109 312d 686f 7473 706f 7409 3632  G.A.1-hotspot.62
-0000ed50: 3009 3335 3909 3409 7965 7309 6f6b 0941  0.359.4.yes.ok.A
-0000ed60: 4c4b 0970 726f 7465 696e 5f63 6f64 696e  LK.protein_codin
-0000ed70: 6709 7379 6e6f 6e79 6d6f 7573 5f76 6172  g.synonymous_var
-0000ed80: 6961 6e74 0976 6172 6469 6374 0972 6573  iant.vardict.res
-0000ed90: 6973 7461 6e63 655f 6d75 7461 7469 6f6e  istance_mutation
-0000eda0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-0000edb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000edc0: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
-0000edd0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-0000ede0: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
-0000edf0: 3309 3134 3034 3938 3335 3909 3134 3034  3.140498359.1404
-0000ee00: 3938 3336 3209 4354 5454 0943 0932 2d69  98362.CTTT.C.2-i
-0000ee10: 6e64 656c 0931 3030 2e35 0932 3709 3409  ndel.100.5.27.4.
-0000ee20: 7965 7309 6c6f 7709 4252 4146 0970 726f  yes.low.BRAF.pro
-0000ee30: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
-0000ee40: 6f6e 5f76 6172 6961 6e74 096d 7574 6563  on_variant.mutec
-0000ee50: 7432 092d 2229 2020 2320 6e6f 7161 0a20  t2.-")  # noqa. 
-0000ee60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ee70: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-0000ee80: 6c74 5b32 5d2e 7273 7472 6970 2829 2c20  lt[2].rstrip(), 
-0000ee90: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-0000eea0: 3037 2e31 3309 3134 3034 3938 3336 3109  07.13.140498361.
-0000eeb0: 3134 3034 3938 3336 3109 2d09 2d09 312d  140498361.-.-.1-
-0000eec0: 686f 7473 706f 7409 3131 3009 2d09 2d09  hotspot.110.-.-.
-0000eed0: 7965 7309 6c6f 7709 2d09 2d09 2d09 2d09  yes.low.-.-.-.-.
-0000eee0: 2d22 2920 2020 2320 6e6f 7161 0a20 2020  -")   # noqa.   
-0000eef0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000ef00: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-0000ef10: 5b33 5d2e 7273 7472 6970 2829 2c20 2273  [3].rstrip(), "s
-0000ef20: 616d 706c 6531 094e 435f 3030 3030 3037  ample1.NC_000007
-0000ef30: 2e31 3309 3134 3034 3533 3133 3609 3134  .13.140453136.14
-0000ef40: 3034 3533 3133 3609 2d09 2d09 312d 686f  0453136.-.-.1-ho
-0000ef50: 7473 706f 7409 3009 2d09 2d09 6e6f 7420  tspot.0.-.-.not 
-0000ef60: 616e 616c 797a 6162 6c65 096c 6f77 092d  analyzable.low.-
-0000ef70: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
-0000ef80: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-0000ef90: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000efa0: 7265 7375 6c74 5b34 5d2e 7273 7472 6970  result[4].rstrip
-0000efb0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-0000efc0: 3030 3030 3037 2e31 3309 3131 3634 3132  000007.13.116412
-0000efd0: 3034 3309 3131 3634 3132 3034 3309 2d09  043.116412043.-.
-0000efe0: 2d09 312d 686f 7473 706f 7409 3009 2d09  -.1-hotspot.0.-.
-0000eff0: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
-0000f000: 096c 6f77 092d 092d 092d 092d 092d 2229  .low.-.-.-.-.-")
-0000f010: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-0000f020: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000f030: 4571 7561 6c28 7265 7375 6c74 5b35 5d2e  Equal(result[5].
-0000f040: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
-0000f050: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
-0000f060: 3239 3434 3532 3732 0932 3934 3435 3237  29445272.2944527
-0000f070: 3209 2d09 2d09 332d 6368 6563 6b09 3232  2.-.-.3-check.22
-0000f080: 3109 2d09 2d09 7965 7309 6c6f 7709 2d09  1.-.-.yes.low.-.
-0000f090: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
-0000f0a0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+0000e6a0: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
+0000e6b0: 2e31 3109 3239 3434 3532 3733 0932 3934  .11.29445273.294
+0000e6c0: 3435 3237 3309 2d09 2d09 332d 6368 6563  45273.-.-.3-chec
+0000e6d0: 6b09 3632 3809 2d09 2d22 290a 2020 2020  k.628.-.-").    
+0000e6e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000e6f0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0000e700: 385d 2e72 7374 7269 7028 292c 2022 7361  8].rstrip(), "sa
+0000e710: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+0000e720: 3131 0932 3934 3435 3237 3409 3239 3434  11.29445274.2944
+0000e730: 3532 3734 092d 092d 0933 2d63 6865 636b  5274.-.-.3-check
+0000e740: 0936 3138 092d 092d 2229 0a20 2020 2020  .618.-.-").     
+0000e750: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000e760: 7274 4571 7561 6c28 7265 7375 6c74 5b39  rtEqual(result[9
+0000e770: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e780: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e790: 3109 3239 3434 3532 3735 0932 3934 3435  1.29445275.29445
+0000e7a0: 3237 3509 2d09 2d09 332d 6368 6563 6b09  275.-.-.3-check.
+0000e7b0: 3630 3809 2d09 2d22 290a 2020 2020 2020  608.-.-").      
+0000e7c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e7d0: 7445 7175 616c 2872 6573 756c 745b 3130  tEqual(result[10
+0000e7e0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e7f0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e800: 3109 3239 3434 3532 3736 0932 3934 3435  1.29445276.29445
+0000e810: 3237 3609 2d09 2d09 332d 6368 6563 6b09  276.-.-.3-check.
+0000e820: 3632 3109 2d09 2d22 290a 2020 2020 2020  621.-.-").      
+0000e830: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e840: 7445 7175 616c 2872 6573 756c 745b 3131  tEqual(result[11
+0000e850: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e860: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e870: 3109 3239 3434 3532 3737 0932 3934 3435  1.29445277.29445
+0000e880: 3237 3709 2d09 2d09 332d 6368 6563 6b09  277.-.-.3-check.
+0000e890: 3138 3209 2d09 2d22 290a 2020 2020 2020  182.-.-").      
+0000e8a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e8b0: 7445 7175 616c 2872 6573 756c 745b 3132  tEqual(result[12
+0000e8c0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e8d0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e8e0: 3109 3239 3434 3532 3738 0932 3934 3435  1.29445278.29445
+0000e8f0: 3237 3809 2d09 2d09 332d 6368 6563 6b09  278.-.-.3-check.
+0000e900: 3535 3009 2d09 2d22 290a 2020 2020 2020  550.-.-").      
+0000e910: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e920: 7445 7175 616c 2872 6573 756c 745b 3133  tEqual(result[13
+0000e930: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e940: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e950: 3109 3239 3434 3532 3739 0932 3934 3435  1.29445279.29445
+0000e960: 3237 3909 2d09 2d09 332d 6368 6563 6b09  279.-.-.3-check.
+0000e970: 3539 3409 2d09 2d22 290a 2020 2020 2020  594.-.-").      
+0000e980: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e990: 7445 7175 616c 2872 6573 756c 745b 3134  tEqual(result[14
+0000e9a0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000e9b0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000e9c0: 3109 3239 3434 3532 3830 0932 3934 3435  1.29445280.29445
+0000e9d0: 3238 3009 2d09 2d09 332d 6368 6563 6b09  280.-.-.3-check.
+0000e9e0: 3533 3909 2d09 2d22 290a 2020 2020 2020  539.-.-").      
+0000e9f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ea00: 7445 7175 616c 2872 6573 756c 745b 3135  tEqual(result[15
+0000ea10: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000ea20: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0000ea30: 3109 3239 3434 3532 3831 0932 3934 3435  1.29445281.29445
+0000ea40: 3238 3109 2d09 2d09 332d 6368 6563 6b09  281.-.-.3-check.
+0000ea50: 3532 3609 2d09 2d22 290a 2020 2020 2020  526.-.-").      
+0000ea60: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ea70: 7445 7175 616c 2872 6573 756c 745b 3136  tEqual(result[16
+0000ea80: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000ea90: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+0000eaa0: 3109 3134 3537 3338 3736 3509 3134 3537  1.145738765.1457
+0000eab0: 3338 3736 3509 2d09 2d09 332d 6368 6563  38765.-.-.3-chec
+0000eac0: 6b09 3136 3136 092d 092d 2229 0a20 2020  k.1616.-.-").   
+0000ead0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000eae0: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+0000eaf0: 5b31 375d 2e72 7374 7269 7028 292c 2022  [17].rstrip(), "
+0000eb00: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0000eb10: 382e 3131 0931 3435 3733 3837 3636 0931  8.11.145738766.1
+0000eb20: 3435 3733 3837 3636 092d 092d 0933 2d63  45738766.-.-.3-c
+0000eb30: 6865 636b 0931 3631 3909 2d09 2d22 290a  heck.1619.-.-").
+0000eb40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eb50: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000eb60: 756c 745b 3138 5d2e 7273 7472 6970 2829  ult[18].rstrip()
+0000eb70: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0000eb80: 3030 3038 2e31 3109 3134 3537 3338 3736  0008.11.14573876
+0000eb90: 3709 3134 3537 3338 3736 3709 2d09 2d09  7.145738767.-.-.
+0000eba0: 332d 6368 6563 6b09 3135 3935 092d 092d  3-check.1595.-.-
+0000ebb0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0000ebc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000ebd0: 7265 7375 6c74 5b31 395d 2e72 7374 7269  result[19].rstri
+0000ebe0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0000ebf0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+0000ec00: 3837 3638 0931 3435 3733 3837 3638 0947  8768.145738768.G
+0000ec10: 0943 0933 2d63 6865 636b 0931 3534 3709  .C.3-check.1547.
+0000ec20: 3509 3237 2229 0a20 2020 2020 2020 2020  5.27").         
+0000ec30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000ec40: 7561 6c28 7265 7375 6c74 5b32 305d 2e72  ual(result[20].r
+0000ec50: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0000ec60: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
+0000ec70: 3435 3733 3837 3639 0931 3435 3733 3837  45738769.1457387
+0000ec80: 3639 092d 092d 0933 2d63 6865 636b 0931  69.-.-.3-check.1
+0000ec90: 3634 3409 2d09 2d22 290a 2020 2020 2020  644.-.-").      
+0000eca0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ecb0: 7445 7175 616c 2872 6573 756c 745b 3231  tEqual(result[21
+0000ecc0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0000ecd0: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+0000ece0: 3109 3134 3537 3338 3737 3009 3134 3537  1.145738770.1457
+0000ecf0: 3338 3737 3009 2d09 2d09 332d 6368 6563  38770.-.-.3-chec
+0000ed00: 6b09 3136 3637 092d 092d 2229 0a20 2020  k.1667.-.-").   
+0000ed10: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000ed20: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+0000ed30: 5b32 325d 2e72 7374 7269 7028 292c 2022  [22].rstrip(), "
+0000ed40: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0000ed50: 382e 3131 0931 3435 3733 3837 3731 0931  8.11.145738771.1
+0000ed60: 3435 3733 3837 3731 092d 092d 0933 2d63  45738771.-.-.3-c
+0000ed70: 6865 636b 0931 3638 3509 2d09 2d22 290a  heck.1685.-.-").
+0000ed80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ed90: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000eda0: 756c 745b 3233 5d2e 7273 7472 6970 2829  ult[23].rstrip()
+0000edb0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0000edc0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+0000edd0: 3209 3134 3537 3338 3737 3209 2d09 2d09  2.145738772.-.-.
+0000ede0: 332d 6368 6563 6b09 3136 3839 092d 092d  3-check.1689.-.-
+0000edf0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0000ee00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000ee10: 7265 7375 6c74 5b32 345d 2e72 7374 7269  result[24].rstri
+0000ee20: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0000ee30: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+0000ee40: 3837 3733 0931 3435 3733 3837 3733 092d  8773.145738773.-
+0000ee50: 092d 0933 2d63 6865 636b 0931 3934 3009  .-.3-check.1940.
+0000ee60: 2d09 2d22 290a 2020 2020 2020 2020 2020  -.-").          
+0000ee70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000ee80: 616c 2872 6573 756c 745b 3235 5d2e 7273  al(result[25].rs
+0000ee90: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+0000eea0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+0000eeb0: 3537 3338 3737 3409 3134 3537 3338 3737  5738774.14573877
+0000eec0: 3409 2d09 2d09 332d 6368 6563 6b09 3139  4.-.-.3-check.19
+0000eed0: 3430 092d 092d 2229 0a20 2020 2020 2020  40.-.-").       
+0000eee0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000eef0: 4571 7561 6c28 7265 7375 6c74 5b32 365d  Equal(result[26]
+0000ef00: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+0000ef10: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+0000ef20: 0931 3435 3733 3837 3735 0931 3435 3733  .145738775.14573
+0000ef30: 3837 3735 092d 092d 0933 2d63 6865 636b  8775.-.-.3-check
+0000ef40: 0931 3936 3309 2d09 2d22 290a 2020 2020  .1963.-.-").    
+0000ef50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000ef60: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0000ef70: 3237 5d2e 7273 7472 6970 2829 2c20 2273  27].rstrip(), "s
+0000ef80: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+0000ef90: 2e31 3109 3134 3537 3338 3737 3609 3134  .11.145738776.14
+0000efa0: 3537 3338 3737 3609 2d09 2d09 332d 6368  5738776.-.-.3-ch
+0000efb0: 6563 6b09 3009 2d09 2d22 290a 2020 2020  eck.0.-.-").    
+0000efc0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000efd0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0000efe0: 3238 5d2e 7273 7472 6970 2829 2c20 2273  28].rstrip(), "s
+0000eff0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+0000f000: 2e31 3109 3134 3537 3338 3737 3709 3134  .11.145738777.14
+0000f010: 3537 3338 3737 3709 2d09 2d09 332d 6368  5738777.-.-.3-ch
+0000f020: 6563 6b09 3139 3634 092d 092d 2229 0a20  eck.1964.-.-"). 
+0000f030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f040: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0000f050: 6c74 5b32 395d 2e72 7374 7269 7028 292c  lt[29].rstrip(),
+0000f060: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0000f070: 3030 382e 3131 0931 3435 3733 3837 3738  008.11.145738778
+0000f080: 0931 3435 3733 3837 3738 092d 092d 0933  .145738778.-.-.3
+0000f090: 2d63 6865 636b 0931 3936 3309 2d09 2d22  -check.1963.-.-"
+0000f0a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
 0000f0b0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-0000f0c0: 6573 756c 745b 365d 2e72 7374 7269 7028  esult[6].rstrip(
-0000f0d0: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-0000f0e0: 3030 3030 322e 3131 0932 3934 3435 3237  00002.11.2944527
-0000f0f0: 3709 3239 3434 3532 3737 092d 092d 0933  7.29445277.-.-.3
-0000f100: 2d63 6865 636b 0931 3832 092d 092d 0979  -check.182.-.-.y
-0000f110: 6573 096c 6f77 092d 092d 092d 092d 092d  es.low.-.-.-.-.-
-0000f120: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-0000f130: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000f140: 7274 4571 7561 6c28 7265 7375 6c74 5b37  rtEqual(result[7
-0000f150: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-0000f160: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
-0000f170: 3109 3134 3537 3338 3736 3809 3134 3537  1.145738768.1457
-0000f180: 3338 3736 3809 4709 4309 332d 6368 6563  38768.G.C.3-chec
-0000f190: 6b09 3135 3437 0935 0932 3709 7965 7309  k.1547.5.27.yes.
-0000f1a0: 6f6b 094c 5252 4331 3409 7072 6f74 6569  ok.LRRC14.protei
-0000f1b0: 6e5f 636f 6469 6e67 0975 7073 7472 6561  n_coding.upstrea
-0000f1c0: 6d5f 6765 6e65 5f76 6172 6961 6e74 0976  m_gene_variant.v
-0000f1d0: 6172 6469 6374 092d 2229 2020 2320 6e6f  ardict.-")  # no
-0000f1e0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-0000f1f0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000f200: 7265 7375 6c74 5b38 5d2e 7273 7472 6970  result[8].rstrip
-0000f210: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-0000f220: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
-0000f230: 3737 3609 3134 3537 3338 3737 3609 2d09  776.145738776.-.
-0000f240: 2d09 332d 6368 6563 6b09 3009 2d09 2d09  -.3-check.0.-.-.
-0000f250: 6e6f 7420 616e 616c 797a 6162 6c65 096c  not analyzable.l
-0000f260: 6f77 092d 092d 092d 092d 092d 2229 2020  ow.-.-.-.-.-")  
-0000f270: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-0000f280: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000f290: 7561 6c28 7265 7375 6c74 5b39 5d2e 7273  ual(result[9].rs
-0000f2a0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-0000f2b0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
-0000f2c0: 3537 3432 3531 3409 3134 3537 3432 3531  5742514.14574251
-0000f2d0: 3409 4109 4709 332d 6368 6563 6b09 3009  4.A.G.3-check.0.
-0000f2e0: 3009 3833 3909 6e6f 7420 616e 616c 797a  0.839.not analyz
-0000f2f0: 6162 6c65 096c 6f77 0952 4543 514c 3409  able.low.RECQL4.
-0000f300: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-0000f310: 796e 6f6e 796d 6f75 735f 7661 7269 616e  ynonymous_varian
-0000f320: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
-0000f330: 3209 2d22 2920 2023 206e 6f71 610a 2020  2.-")  # noqa.  
-0000f340: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000f350: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-0000f360: 745b 3130 5d2e 7273 7472 6970 2829 2c20  t[10].rstrip(), 
-0000f370: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-0000f380: 3136 2e31 3109 3831 3935 3437 3839 0938  16.11.81954789.8
-0000f390: 3139 3534 3738 3909 4309 4754 0932 2d69  1954789.C.GT.2-i
-0000f3a0: 6e64 656c 0931 3134 3409 3131 3732 0932  ndel.1144.1172.2
-0000f3b0: 3909 7965 7309 6f6b 0950 4c43 4732 0970  9.yes.ok.PLCG2.p
-0000f3c0: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-0000f3d0: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-0000f3e0: 6469 6374 092d 2229 2020 2320 6e6f 7161  dict.-")  # noqa
-0000f3f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f400: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-0000f410: 7375 6c74 5b31 315d 2e72 7374 7269 7028  sult[11].rstrip(
-0000f420: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-0000f430: 3030 3030 322e 3131 0932 3934 3435 3238  00002.11.2944528
-0000f440: 3209 3239 3434 3532 3832 0947 0941 0934  2.29445282.G.A.4
-0000f450: 2d6f 7468 6572 0935 3230 0932 3834 0933  -other.520.284.3
-0000f460: 0979 6573 096f 6b09 414c 4b09 7072 6f74  .yes.ok.ALK.prot
-0000f470: 6569 6e5f 636f 6469 6e67 0973 706c 6963  ein_coding.splic
-0000f480: 655f 7265 6769 6f6e 5f76 6172 6961 6e74  e_region_variant
-0000f490: 2669 6e74 726f 6e5f 7661 7269 616e 7409  &intron_variant.
-0000f4a0: 7661 7264 6963 7409 2d22 2920 2023 206e  vardict.-")  # n
-0000f4b0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-0000f4c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000f4d0: 2872 6573 756c 745b 3132 5d2e 7273 7472  (result[12].rstr
-0000f4e0: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
-0000f4f0: 435f 3030 3030 3136 2e31 3109 3831 3935  C_000016.11.8195
-0000f500: 3437 3839 0938 3139 3534 3738 3909 4309  4789.81954789.C.
-0000f510: 4709 342d 6f74 6865 7209 3131 3434 0934  G.4-other.1144.4
-0000f520: 3432 0933 3439 0979 6573 096f 6b09 5345  42.349.yes.ok.SE
-0000f530: 5054 0970 726f 7465 696e 5f63 6f64 696e  PT.protein_codin
-0000f540: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
-0000f550: 0976 6172 6469 6374 2c6d 7574 6563 7432  .vardict,mutect2
-0000f560: 092d 2229 2020 2320 6e6f 7161 0a0a 2020  .-")  # noqa..  
-0000f570: 2020 6465 6620 7465 7374 5f66 696c 7465    def test_filte
-0000f580: 7265 645f 6d75 7461 7469 6f6e 5f63 6861  red_mutation_cha
-0000f590: 6e67 655f 6f75 7470 7574 5f6f 7264 6572  nge_output_order
-0000f5a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f5b0: 6672 6f6d 2068 7964 7261 5f67 656e 6574  from hydra_genet
-0000f5c0: 6963 732e 7574 696c 732e 696f 2e68 6f74  ics.utils.io.hot
-0000f5d0: 7370 6f74 5f72 6570 6f72 7420 696d 706f  spot_report impo
-0000f5e0: 7274 2067 656e 6572 6174 655f 686f 7473  rt generate_hots
-0000f5f0: 706f 745f 7265 706f 7274 0a20 2020 2020  pot_report.     
-0000f600: 2020 206c 6576 656c 7320 3d20 5b28 3330     levels = [(30
-0000f610: 302c 2022 6f6b 222c 2022 7965 7322 292c  0, "ok", "yes"),
-0000f620: 2028 3330 2c20 226c 6f77 222c 2022 7965   (30, "low", "ye
-0000f630: 7322 292c 2028 302c 2022 6c6f 7722 2c20  s"), (0, "low", 
-0000f640: 226e 6f74 2061 6e61 6c79 7a61 626c 6522  "not analyzable"
-0000f650: 295d 0a20 2020 2020 2020 2073 656c 662e  )].        self.
-0000f660: 6d61 7844 6966 6620 3d20 3130 3030 300a  maxDiff = 10000.
-0000f670: 0a20 2020 2020 2020 2072 6570 6f72 7420  .        report 
-0000f680: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-0000f690: 656c 662e 7465 6d70 6469 722c 2022 6669  elf.tempdir, "fi
-0000f6a0: 6c74 6572 6564 2e72 6570 6f72 7422 290a  ltered.report").
-0000f6b0: 2020 2020 2020 2020 6765 6e65 7261 7465          generate
-0000f6c0: 5f68 6f74 7370 6f74 5f72 6570 6f72 7428  _hotspot_report(
-0000f6d0: 2273 616d 706c 6531 222c 0a20 2020 2020  "sample1",.     
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-0000f700: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f720: 2020 206c 6576 656c 732c 0a20 2020 2020     levels,.     
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f750: 686f 7473 706f 742c 0a20 2020 2020 2020  hotspot,.       
-0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 2020 2020 2020 2020 2073 656c 662e 7663           self.vc
-0000f780: 665f 7665 7020 2b20 222e 677a 222c 0a20  f_vep + ".gz",. 
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f7b0: 656c 662e 6776 6366 202b 2022 2e67 7a22  elf.gvcf + ".gz"
-0000f7c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7e0: 2020 7365 6c66 2e72 6566 6572 656e 6365    self.reference
-0000f7f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2020 7365 6c66 2e76 6366 5f76 6570 5f77    self.vcf_vep_w
-0000f820: 6f5f 7069 636b 202b 2022 2e67 7a22 2c0a  o_pick + ".gz",.
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 2274 6573 7473 2f75 7469 6c73 2f66 696c  "tests/utils/fil
-0000f860: 6573 2f72 6570 6f72 745f 636f 6c75 6d6e  es/report_column
-0000f870: 735f 7665 705f 6f72 6465 725f 6f75 7470  s_vep_order_outp
-0000f880: 7574 2e79 616d 6c22 290a 2020 2020 2020  ut.yaml").      
-0000f890: 2020 7769 7468 206f 7065 6e28 7265 706f    with open(repo
-0000f8a0: 7274 2c20 2772 2729 2061 7320 7265 706f  rt, 'r') as repo
-0000f8b0: 7274 5f72 6573 756c 743a 0a20 2020 2020  rt_result:.     
-0000f8c0: 2020 2020 2020 2068 6561 6420 3d20 7265         head = re
-0000f8d0: 706f 7274 5f72 6573 756c 742e 7265 6164  port_result.read
-0000f8e0: 6c69 6e65 2829 0a20 2020 2020 2020 2020  line().         
-0000f8f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000f900: 7561 6c28 6865 6164 2e72 7374 7269 7028  ual(head.rstrip(
-0000f910: 292c 2022 5c74 222e 6a6f 696e 285b 2273  ), "\t".join(["s
-0000f920: 746f 7022 2c20 2273 7461 7274 222c 2022  top", "start", "
-0000f930: 6368 7222 2c20 2747 656e 6527 2c20 2273  chr", 'Gene', "s
-0000f940: 616d 706c 6522 2c20 2772 6566 272c 2027  ample", 'ref', '
-0000f950: 616c 7427 2c20 2272 6570 6f72 7422 2c20  alt', "report", 
-0000f960: 2767 7663 665f 6465 7074 6827 2c20 2772  'gvcf_depth', 'r
-0000f970: 6566 5f64 6570 7468 272c 2027 616c 745f  ef_depth', 'alt_
-0000f980: 6465 7074 6827 2c20 2741 6e61 6c79 7a61  depth', 'Analyza
-0000f990: 626c 6527 2c20 274d 696e 5f72 6561 645f  ble', 'Min_read_
-0000f9a0: 6465 7074 6833 3030 272c 2027 5661 7269  depth300', 'Vari
-0000f9b0: 616e 745f 7479 7065 272c 2027 436f 6e73  ant_type', 'Cons
-0000f9c0: 6571 7565 6e63 6527 2c20 2743 616c 6c65  equence', 'Calle
-0000f9d0: 7273 272c 2027 436f 6d6d 656e 7427 5d29  rs', 'Comment'])
-0000f9e0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
-0000f9f0: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
-0000fa00: 6570 6f72 745f 7265 7375 6c74 2e72 6561  eport_result.rea
-0000fa10: 646c 696e 6573 2829 0a20 2020 2020 2020  dlines().       
-0000fa20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000fa30: 4571 7561 6c28 6c65 6e28 7265 7375 6c74  Equal(len(result
-0000fa40: 292c 2031 3329 0a20 2020 2020 2020 2020  ), 13).         
-0000fa50: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000fa60: 7561 6c28 7265 7375 6c74 5b30 5d2e 7273  ual(result[0].rs
-0000fa70: 7472 6970 2829 2c20 2232 3934 3435 3237  trip(), "2944527
-0000fa80: 3109 3239 3434 3532 3731 094e 435f 3030  1.29445271.NC_00
-0000fa90: 3030 3032 2e31 3109 414c 4b09 7361 6d70  0002.11.ALK.samp
-0000faa0: 6c65 3109 4709 4109 312d 686f 7473 706f  le1.G.A.1-hotspo
-0000fab0: 7409 3632 3009 3335 3909 3409 7965 7309  t.620.359.4.yes.
-0000fac0: 6f6b 0970 726f 7465 696e 5f63 6f64 696e  ok.protein_codin
-0000fad0: 6709 7379 6e6f 6e79 6d6f 7573 5f76 6172  g.synonymous_var
-0000fae0: 6961 6e74 0976 6172 6469 6374 0972 6573  iant.vardict.res
-0000faf0: 6973 7461 6e63 655f 6d75 7461 7469 6f6e  istance_mutation
-0000fb00: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-0000fb10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fb20: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
-0000fb30: 5d2e 7273 7472 6970 2829 2c20 2231 3430  ].rstrip(), "140
-0000fb40: 3439 3833 3632 0931 3430 3439 3833 3539  498362.140498359
-0000fb50: 094e 435f 3030 3030 3037 2e31 3309 4252  .NC_000007.13.BR
-0000fb60: 4146 0973 616d 706c 6531 0943 5454 5409  AF.sample1.CTTT.
-0000fb70: 4309 322d 696e 6465 6c09 3130 302e 3509  C.2-indel.100.5.
-0000fb80: 3237 0934 0979 6573 096c 6f77 0970 726f  27.4.yes.low.pro
-0000fb90: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
-0000fba0: 6f6e 5f76 6172 6961 6e74 096d 7574 6563  on_variant.mutec
-0000fbb0: 7432 092d 2229 2020 2320 6e6f 7161 0a20  t2.-")  # noqa. 
-0000fbc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fbd0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-0000fbe0: 6c74 5b32 5d2e 7273 7472 6970 2829 2c20  lt[2].rstrip(), 
-0000fbf0: 2231 3430 3439 3833 3631 0931 3430 3439  "140498361.14049
-0000fc00: 3833 3631 094e 435f 3030 3030 3037 2e31  8361.NC_000007.1
-0000fc10: 3309 2d09 7361 6d70 6c65 3109 2d09 2d09  3.-.sample1.-.-.
-0000fc20: 312d 686f 7473 706f 7409 3131 3009 2d09  1-hotspot.110.-.
-0000fc30: 2d09 7965 7309 6c6f 7709 2d09 2d09 2d09  -.yes.low.-.-.-.
-0000fc40: 2d22 2920 2020 2320 6e6f 7161 0a20 2020  -")   # noqa.   
-0000fc50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000fc60: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-0000fc70: 5b33 5d2e 7273 7472 6970 2829 2c20 2231  [3].rstrip(), "1
-0000fc80: 3430 3435 3331 3336 0931 3430 3435 3331  40453136.1404531
-0000fc90: 3336 094e 435f 3030 3030 3037 2e31 3309  36.NC_000007.13.
-0000fca0: 2d09 7361 6d70 6c65 3109 2d09 2d09 312d  -.sample1.-.-.1-
-0000fcb0: 686f 7473 706f 7409 3009 2d09 2d09 6e6f  hotspot.0.-.-.no
-0000fcc0: 7420 616e 616c 797a 6162 6c65 096c 6f77  t analyzable.low
-0000fcd0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
-0000fce0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-0000fcf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000fd00: 7265 7375 6c74 5b34 5d2e 7273 7472 6970  result[4].rstrip
-0000fd10: 2829 2c20 2231 3136 3431 3230 3433 0931  (), "116412043.1
-0000fd20: 3136 3431 3230 3433 094e 435f 3030 3030  16412043.NC_0000
-0000fd30: 3037 2e31 3309 2d09 7361 6d70 6c65 3109  07.13.-.sample1.
-0000fd40: 2d09 2d09 312d 686f 7473 706f 7409 3009  -.-.1-hotspot.0.
-0000fd50: 2d09 2d09 6e6f 7420 616e 616c 797a 6162  -.-.not analyzab
-0000fd60: 6c65 096c 6f77 092d 092d 092d 092d 2229  le.low.-.-.-.-")
-0000fd70: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-0000fd80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000fd90: 4571 7561 6c28 7265 7375 6c74 5b35 5d2e  Equal(result[5].
-0000fda0: 7273 7472 6970 2829 2c20 2232 3934 3435  rstrip(), "29445
-0000fdb0: 3237 3209 3239 3434 3532 3732 094e 435f  272.29445272.NC_
-0000fdc0: 3030 3030 3032 2e31 3109 2d09 7361 6d70  000002.11.-.samp
-0000fdd0: 6c65 3109 2d09 2d09 332d 6368 6563 6b09  le1.-.-.3-check.
-0000fde0: 3232 3109 2d09 2d09 7965 7309 6c6f 7709  221.-.-.yes.low.
-0000fdf0: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
-0000fe00: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-0000fe10: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-0000fe20: 6573 756c 745b 365d 2e72 7374 7269 7028  esult[6].rstrip(
-0000fe30: 292c 2022 3239 3434 3532 3737 0932 3934  ), "29445277.294
-0000fe40: 3435 3237 3709 4e43 5f30 3030 3030 322e  45277.NC_000002.
-0000fe50: 3131 092d 0973 616d 706c 6531 092d 092d  11.-.sample1.-.-
-0000fe60: 0933 2d63 6865 636b 0931 3832 092d 092d  .3-check.182.-.-
-0000fe70: 0979 6573 096c 6f77 092d 092d 092d 092d  .yes.low.-.-.-.-
-0000fe80: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-0000fe90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fea0: 7274 4571 7561 6c28 7265 7375 6c74 5b37  rtEqual(result[7
-0000feb0: 5d2e 7273 7472 6970 2829 2c20 2231 3435  ].rstrip(), "145
-0000fec0: 3733 3837 3638 0931 3435 3733 3837 3638  738768.145738768
-0000fed0: 094e 435f 3030 3030 3038 2e31 3109 4c52  .NC_000008.11.LR
-0000fee0: 5243 3134 0973 616d 706c 6531 0947 0943  RC14.sample1.G.C
-0000fef0: 0933 2d63 6865 636b 0931 3534 3709 3509  .3-check.1547.5.
-0000ff00: 3237 0979 6573 096f 6b09 7072 6f74 6569  27.yes.ok.protei
-0000ff10: 6e5f 636f 6469 6e67 0975 7073 7472 6561  n_coding.upstrea
-0000ff20: 6d5f 6765 6e65 5f76 6172 6961 6e74 0976  m_gene_variant.v
-0000ff30: 6172 6469 6374 092d 2229 2020 2320 6e6f  ardict.-")  # no
-0000ff40: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-0000ff50: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000ff60: 7265 7375 6c74 5b38 5d2e 7273 7472 6970  result[8].rstrip
-0000ff70: 2829 2c20 2231 3435 3733 3837 3736 0931  (), "145738776.1
-0000ff80: 3435 3733 3837 3736 094e 435f 3030 3030  45738776.NC_0000
-0000ff90: 3038 2e31 3109 2d09 7361 6d70 6c65 3109  08.11.-.sample1.
-0000ffa0: 2d09 2d09 332d 6368 6563 6b09 3009 2d09  -.-.3-check.0.-.
-0000ffb0: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
-0000ffc0: 096c 6f77 092d 092d 092d 092d 2229 2020  .low.-.-.-.-")  
-0000ffd0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-0000ffe0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000fff0: 7561 6c28 7265 7375 6c74 5b39 5d2e 7273  ual(result[9].rs
-00010000: 7472 6970 2829 2c20 2231 3435 3734 3235  trip(), "1457425
-00010010: 3134 0931 3435 3734 3235 3134 094e 435f  14.145742514.NC_
-00010020: 3030 3030 3038 2e31 3109 5245 4351 4c34  000008.11.RECQL4
-00010030: 0973 616d 706c 6531 0941 0947 0933 2d63  .sample1.A.G.3-c
-00010040: 6865 636b 0930 0930 0938 3339 096e 6f74  heck.0.0.839.not
-00010050: 2061 6e61 6c79 7a61 626c 6509 6c6f 7709   analyzable.low.
-00010060: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-00010070: 796e 6f6e 796d 6f75 735f 7661 7269 616e  ynonymous_varian
-00010080: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
-00010090: 3209 2d22 2920 2023 206e 6f71 610a 2020  2.-")  # noqa.  
-000100a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000100b0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-000100c0: 745b 3130 5d2e 7273 7472 6970 2829 2c20  t[10].rstrip(), 
-000100d0: 2238 3139 3534 3738 3909 3831 3935 3437  "81954789.819547
-000100e0: 3839 094e 435f 3030 3030 3136 2e31 3109  89.NC_000016.11.
-000100f0: 504c 4347 3209 7361 6d70 6c65 3109 4309  PLCG2.sample1.C.
-00010100: 4754 0932 2d69 6e64 656c 0931 3134 3409  GT.2-indel.1144.
-00010110: 3131 3732 0932 3909 7965 7309 6f6b 0970  1172.29.yes.ok.p
-00010120: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-00010130: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-00010140: 6469 6374 092d 2229 2020 2320 6e6f 7161  dict.-")  # noqa
-00010150: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010160: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00010170: 7375 6c74 5b31 315d 2e72 7374 7269 7028  sult[11].rstrip(
-00010180: 292c 2022 3239 3434 3532 3832 0932 3934  ), "29445282.294
-00010190: 3435 3238 3209 4e43 5f30 3030 3030 322e  45282.NC_000002.
-000101a0: 3131 0941 4c4b 0973 616d 706c 6531 0947  11.ALK.sample1.G
-000101b0: 0941 0934 2d6f 7468 6572 0935 3230 0932  .A.4-other.520.2
-000101c0: 3834 0933 0979 6573 096f 6b09 7072 6f74  84.3.yes.ok.prot
-000101d0: 6569 6e5f 636f 6469 6e67 0973 706c 6963  ein_coding.splic
-000101e0: 655f 7265 6769 6f6e 5f76 6172 6961 6e74  e_region_variant
-000101f0: 2669 6e74 726f 6e5f 7661 7269 616e 7409  &intron_variant.
-00010200: 7661 7264 6963 7409 2d22 2920 2023 206e  vardict.-")  # n
-00010210: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00010220: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00010230: 2872 6573 756c 745b 3132 5d2e 7273 7472  (result[12].rstr
-00010240: 6970 2829 2c20 2238 3139 3534 3738 3909  ip(), "81954789.
-00010250: 3831 3935 3437 3839 094e 435f 3030 3030  81954789.NC_0000
-00010260: 3136 2e31 3109 5345 5054 0973 616d 706c  16.11.SEPT.sampl
-00010270: 6531 0943 0947 0934 2d6f 7468 6572 0931  e1.C.G.4-other.1
-00010280: 3134 3409 3434 3209 3334 3909 7965 7309  144.442.349.yes.
-00010290: 6f6b 0970 726f 7465 696e 5f63 6f64 696e  ok.protein_codin
-000102a0: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
-000102b0: 0976 6172 6469 6374 2c6d 7574 6563 7432  .vardict,mutect2
-000102c0: 092d 2229 2020 2320 6e6f 7161 0a0a 2020  .-")  # noqa..  
-000102d0: 2020 6465 6620 7465 7374 5f66 696c 7465    def test_filte
-000102e0: 7265 645f 6d75 7461 7469 6f6e 5f68 6964  red_mutation_hid
-000102f0: 655f 636f 6c75 6d6e 2873 656c 6629 3a0a  e_column(self):.
-00010300: 2020 2020 2020 2020 6672 6f6d 2068 7964          from hyd
-00010310: 7261 5f67 656e 6574 6963 732e 7574 696c  ra_genetics.util
-00010320: 732e 696f 2e68 6f74 7370 6f74 5f72 6570  s.io.hotspot_rep
-00010330: 6f72 7420 696d 706f 7274 2067 656e 6572  ort import gener
-00010340: 6174 655f 686f 7473 706f 745f 7265 706f  ate_hotspot_repo
-00010350: 7274 0a20 2020 2020 2020 206c 6576 656c  rt.        level
-00010360: 7320 3d20 5b28 3330 302c 2022 6f6b 222c  s = [(300, "ok",
-00010370: 2022 7965 7322 292c 2028 3330 2c20 226c   "yes"), (30, "l
-00010380: 6f77 222c 2022 7965 7322 292c 2028 302c  ow", "yes"), (0,
-00010390: 2022 6c6f 7722 2c20 226e 6f74 2061 6e61   "low", "not ana
-000103a0: 6c79 7a61 626c 6522 295d 0a20 2020 2020  lyzable")].     
-000103b0: 2020 2073 656c 662e 6d61 7844 6966 6620     self.maxDiff 
-000103c0: 3d20 3130 3030 300a 0a20 2020 2020 2020  = 10000..       
-000103d0: 2072 6570 6f72 7420 3d20 6f73 2e70 6174   report = os.pat
-000103e0: 682e 6a6f 696e 2873 656c 662e 7465 6d70  h.join(self.temp
-000103f0: 6469 722c 2022 6669 6c74 6572 6564 2e72  dir, "filtered.r
-00010400: 6570 6f72 7422 290a 2020 2020 2020 2020  eport").        
-00010410: 6765 6e65 7261 7465 5f68 6f74 7370 6f74  generate_hotspot
-00010420: 5f72 6570 6f72 7428 2273 616d 706c 6531  _report("sample1
-00010430: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2072 6570 6f72 742c 0a20 2020 2020     report,.     
-00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010470: 2020 2020 2020 2020 2020 206c 6576 656c             level
-00010480: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2073 656c 662e 686f 7473 706f 742c     self.hotspot,
-000104b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2073 656c 662e 7663 665f 7665 7020 2b20   self.vcf_vep + 
-000104e0: 222e 677a 222c 0a20 2020 2020 2020 2020  ".gz",.         
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2020 2020 2073 656c 662e 6776 6366         self.gvcf
-00010510: 202b 2022 2e67 7a22 2c0a 2020 2020 2020   + ".gz",.      
-00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010540: 6566 6572 656e 6365 2c0a 2020 2020 2020  eference,.      
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00010570: 6366 5f76 6570 5f77 6f5f 7069 636b 202b  cf_vep_wo_pick +
-00010580: 2022 2e67 7a22 2c0a 2020 2020 2020 2020   ".gz",.        
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 2274 6573 7473 2f75          "tests/u
-000105b0: 7469 6c73 2f66 696c 6573 2f72 6570 6f72  tils/files/repor
-000105c0: 745f 636f 6c75 6d6e 735f 7665 705f 6869  t_columns_vep_hi
-000105d0: 6465 5f63 6f6c 756d 6e2e 7961 6d6c 2229  de_column.yaml")
-000105e0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-000105f0: 656e 2872 6570 6f72 742c 2027 7227 2920  en(report, 'r') 
-00010600: 6173 2072 6570 6f72 745f 7265 7375 6c74  as report_result
-00010610: 3a0a 2020 2020 2020 2020 2020 2020 6865  :.            he
-00010620: 6164 203d 2072 6570 6f72 745f 7265 7375  ad = report_resu
-00010630: 6c74 2e72 6561 646c 696e 6528 290a 2020  lt.readline().  
-00010640: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00010650: 7373 6572 7445 7175 616c 2868 6561 642e  ssertEqual(head.
-00010660: 7273 7472 6970 2829 2c20 225c 7422 2e6a  rstrip(), "\t".j
-00010670: 6f69 6e28 5b27 4765 6e65 272c 2022 7361  oin(['Gene', "sa
-00010680: 6d70 6c65 222c 2022 7374 6172 7422 2c20  mple", "start", 
-00010690: 2272 6566 222c 2022 616c 7422 2c20 2272  "ref", "alt", "r
-000106a0: 6570 6f72 7422 2c20 2767 7663 665f 6465  eport", 'gvcf_de
-000106b0: 7074 6827 2c20 2272 6566 5f64 6570 7468  pth', "ref_depth
-000106c0: 222c 2022 616c 745f 6465 7074 6822 2c20  ", "alt_depth", 
-000106d0: 2741 6e61 6c79 7a61 626c 6527 2c20 2756  'Analyzable', 'V
-000106e0: 6172 6961 6e74 5f74 7970 6527 2c20 2743  ariant_type', 'C
-000106f0: 6f6e 7365 7175 656e 6365 272c 2027 4361  onsequence', 'Ca
-00010700: 6c6c 6572 7327 2c20 2743 6f6d 6d65 6e74  llers', 'Comment
-00010710: 275d 2929 2020 2320 6e6f 7161 0a20 2020  ']))  # noqa.   
-00010720: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00010730: 3d20 7265 706f 7274 5f72 6573 756c 742e  = report_result.
-00010740: 7265 6164 6c69 6e65 7328 290a 2020 2020  readlines().    
-00010750: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010760: 6572 7445 7175 616c 286c 656e 2872 6573  ertEqual(len(res
-00010770: 756c 7429 2c20 3133 290a 2020 2020 2020  ult), 13).      
-00010780: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010790: 7445 7175 616c 2872 6573 756c 745b 305d  tEqual(result[0]
-000107a0: 2e72 7374 7269 7028 292c 2022 414c 4b09  .rstrip(), "ALK.
-000107b0: 7361 6d70 6c65 3109 3239 3434 3532 3731  sample1.29445271
-000107c0: 0947 0941 0931 2d68 6f74 7370 6f74 0936  .G.A.1-hotspot.6
-000107d0: 3230 0933 3539 0934 0979 6573 0970 726f  20.359.4.yes.pro
-000107e0: 7465 696e 5f63 6f64 696e 6709 7379 6e6f  tein_coding.syno
-000107f0: 6e79 6d6f 7573 5f76 6172 6961 6e74 0976  nymous_variant.v
-00010800: 6172 6469 6374 0972 6573 6973 7461 6e63  ardict.resistanc
-00010810: 655f 6d75 7461 7469 6f6e 2229 2020 2320  e_mutation")  # 
-00010820: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00010830: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00010840: 6c28 7265 7375 6c74 5b31 5d2e 7273 7472  l(result[1].rstr
-00010850: 6970 2829 2c20 2242 5241 4609 7361 6d70  ip(), "BRAF.samp
-00010860: 6c65 3109 3134 3034 3938 3335 3909 4354  le1.140498359.CT
-00010870: 5454 0943 0932 2d69 6e64 656c 0931 3030  TT.C.2-indel.100
-00010880: 2e35 0932 3709 3409 7965 7309 7072 6f74  .5.27.4.yes.prot
-00010890: 6569 6e5f 636f 6469 6e67 0969 6e74 726f  ein_coding.intro
-000108a0: 6e5f 7661 7269 616e 7409 6d75 7465 6374  n_variant.mutect
-000108b0: 3209 2d22 2920 2023 206e 6f71 610a 2020  2.-")  # noqa.  
-000108c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000108d0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-000108e0: 745b 325d 2e72 7374 7269 7028 292c 2022  t[2].rstrip(), "
-000108f0: 2d09 7361 6d70 6c65 3109 3134 3034 3938  -.sample1.140498
-00010900: 3336 3109 2d09 2d09 312d 686f 7473 706f  361.-.-.1-hotspo
-00010910: 7409 3131 3009 2d09 2d09 7965 7309 2d09  t.110.-.-.yes.-.
-00010920: 2d09 2d09 2d22 2920 2020 2320 6e6f 7161  -.-.-")   # noqa
-00010930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010940: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00010950: 7375 6c74 5b33 5d2e 7273 7472 6970 2829  sult[3].rstrip()
-00010960: 2c20 222d 0973 616d 706c 6531 0931 3430  , "-.sample1.140
-00010970: 3435 3331 3336 092d 092d 0931 2d68 6f74  453136.-.-.1-hot
-00010980: 7370 6f74 0930 092d 092d 096e 6f74 2061  spot.0.-.-.not a
-00010990: 6e61 6c79 7a61 626c 6509 2d09 2d09 2d09  nalyzable.-.-.-.
-000109a0: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
-000109b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000109c0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-000109d0: 345d 2e72 7374 7269 7028 292c 2022 2d09  4].rstrip(), "-.
-000109e0: 7361 6d70 6c65 3109 3131 3634 3132 3034  sample1.11641204
-000109f0: 3309 2d09 2d09 312d 686f 7473 706f 7409  3.-.-.1-hotspot.
-00010a00: 3009 2d09 2d09 6e6f 7420 616e 616c 797a  0.-.-.not analyz
-00010a10: 6162 6c65 092d 092d 092d 092d 2229 2020  able.-.-.-.-")  
-00010a20: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00010a30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00010a40: 7561 6c28 7265 7375 6c74 5b35 5d2e 7273  ual(result[5].rs
-00010a50: 7472 6970 2829 2c20 222d 0973 616d 706c  trip(), "-.sampl
-00010a60: 6531 0932 3934 3435 3237 3209 2d09 2d09  e1.29445272.-.-.
-00010a70: 332d 6368 6563 6b09 3232 3109 2d09 2d09  3-check.221.-.-.
-00010a80: 7965 7309 2d09 2d09 2d09 2d22 2920 2023  yes.-.-.-.-")  #
-00010a90: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
-00010aa0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00010ab0: 616c 2872 6573 756c 745b 365d 2e72 7374  al(result[6].rst
-00010ac0: 7269 7028 292c 2022 2d09 7361 6d70 6c65  rip(), "-.sample
-00010ad0: 3109 3239 3434 3532 3737 092d 092d 0933  1.29445277.-.-.3
-00010ae0: 2d63 6865 636b 0931 3832 092d 092d 0979  -check.182.-.-.y
-00010af0: 6573 092d 092d 092d 092d 2229 2020 2320  es.-.-.-.-")  # 
-00010b00: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00010b10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00010b20: 6c28 7265 7375 6c74 5b37 5d2e 7273 7472  l(result[7].rstr
-00010b30: 6970 2829 2c20 224c 5252 4331 3409 7361  ip(), "LRRC14.sa
-00010b40: 6d70 6c65 3109 3134 3537 3338 3736 3809  mple1.145738768.
-00010b50: 4709 4309 332d 6368 6563 6b09 3135 3437  G.C.3-check.1547
-00010b60: 0935 0932 3709 7965 7309 7072 6f74 6569  .5.27.yes.protei
-00010b70: 6e5f 636f 6469 6e67 0975 7073 7472 6561  n_coding.upstrea
-00010b80: 6d5f 6765 6e65 5f76 6172 6961 6e74 0976  m_gene_variant.v
-00010b90: 6172 6469 6374 092d 2229 2020 2320 6e6f  ardict.-")  # no
-00010ba0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-00010bb0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00010bc0: 7265 7375 6c74 5b38 5d2e 7273 7472 6970  result[8].rstrip
-00010bd0: 2829 2c20 222d 0973 616d 706c 6531 0931  (), "-.sample1.1
-00010be0: 3435 3733 3837 3736 092d 092d 0933 2d63  45738776.-.-.3-c
-00010bf0: 6865 636b 0930 092d 092d 096e 6f74 2061  heck.0.-.-.not a
-00010c00: 6e61 6c79 7a61 626c 6509 2d09 2d09 2d09  nalyzable.-.-.-.
-00010c10: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
-00010c20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010c30: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-00010c40: 395d 2e72 7374 7269 7028 292c 2022 5245  9].rstrip(), "RE
-00010c50: 4351 4c34 0973 616d 706c 6531 0931 3435  CQL4.sample1.145
-00010c60: 3734 3235 3134 0941 0947 0933 2d63 6865  742514.A.G.3-che
-00010c70: 636b 0930 0930 0938 3339 096e 6f74 2061  ck.0.0.839.not a
-00010c80: 6e61 6c79 7a61 626c 6509 7072 6f74 6569  nalyzable.protei
-00010c90: 6e5f 636f 6469 6e67 0973 796e 6f6e 796d  n_coding.synonym
-00010ca0: 6f75 735f 7661 7269 616e 7409 7661 7264  ous_variant.vard
-00010cb0: 6963 742c 6d75 7465 6374 3209 2d22 2920  ict,mutect2.-") 
-00010cc0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00010cd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00010ce0: 7175 616c 2872 6573 756c 745b 3130 5d2e  qual(result[10].
-00010cf0: 7273 7472 6970 2829 2c20 2250 4c43 4732  rstrip(), "PLCG2
-00010d00: 0973 616d 706c 6531 0938 3139 3534 3738  .sample1.8195478
-00010d10: 3909 4309 4754 0932 2d69 6e64 656c 0931  9.C.GT.2-indel.1
-00010d20: 3134 3409 3131 3732 0932 3909 7965 7309  144.1172.29.yes.
-00010d30: 7072 6f74 6569 6e5f 636f 6469 6e67 0969  protein_coding.i
-00010d40: 6e74 726f 6e5f 7661 7269 616e 7409 7661  ntron_variant.va
-00010d50: 7264 6963 7409 2d22 2920 2023 206e 6f71  rdict.-")  # noq
-00010d60: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00010d70: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00010d80: 6573 756c 745b 3131 5d2e 7273 7472 6970  esult[11].rstrip
-00010d90: 2829 2c20 2241 4c4b 0973 616d 706c 6531  (), "ALK.sample1
-00010da0: 0932 3934 3435 3238 3209 4709 4109 342d  .29445282.G.A.4-
-00010db0: 6f74 6865 7209 3532 3009 3238 3409 3309  other.520.284.3.
-00010dc0: 7965 7309 7072 6f74 6569 6e5f 636f 6469  yes.protein_codi
-00010dd0: 6e67 0973 706c 6963 655f 7265 6769 6f6e  ng.splice_region
-00010de0: 5f76 6172 6961 6e74 2669 6e74 726f 6e5f  _variant&intron_
-00010df0: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
-00010e00: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
-00010e10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010e20: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-00010e30: 3132 5d2e 7273 7472 6970 2829 2c20 2253  12].rstrip(), "S
-00010e40: 4550 5409 7361 6d70 6c65 3109 3831 3935  EPT.sample1.8195
-00010e50: 3437 3839 0943 0947 0934 2d6f 7468 6572  4789.C.G.4-other
-00010e60: 0931 3134 3409 3434 3209 3334 3909 7965  .1144.442.349.ye
-00010e70: 7309 7072 6f74 6569 6e5f 636f 6469 6e67  s.protein_coding
-00010e80: 0969 6e74 726f 6e5f 7661 7269 616e 7409  .intron_variant.
-00010e90: 7661 7264 6963 742c 6d75 7465 6374 3209  vardict,mutect2.
-00010ea0: 2d22 2920 2023 206e 6f71 610a 0a20 2020  -")  # noqa..   
-00010eb0: 2064 6566 2074 6573 745f 6669 6c74 6572   def test_filter
-00010ec0: 6564 5f76 6570 5f72 6567 6578 5f65 7874  ed_vep_regex_ext
-00010ed0: 7261 6374 2873 656c 6629 3a0a 2020 2020  ract(self):.    
-00010ee0: 2020 2020 6672 6f6d 2068 7964 7261 5f67      from hydra_g
-00010ef0: 656e 6574 6963 732e 7574 696c 732e 696f  enetics.utils.io
-00010f00: 2e68 6f74 7370 6f74 5f72 6570 6f72 7420  .hotspot_report 
-00010f10: 696d 706f 7274 2067 656e 6572 6174 655f  import generate_
-00010f20: 686f 7473 706f 745f 7265 706f 7274 0a20  hotspot_report. 
-00010f30: 2020 2020 2020 206c 6576 656c 7320 3d20         levels = 
-00010f40: 5b28 3330 302c 2022 6f6b 222c 2022 7965  [(300, "ok", "ye
-00010f50: 7322 292c 2028 3330 2c20 226c 6f77 222c  s"), (30, "low",
-00010f60: 2022 7965 7322 292c 2028 302c 2022 6c6f   "yes"), (0, "lo
-00010f70: 7722 2c20 226e 6f74 2061 6e61 6c79 7a61  w", "not analyza
-00010f80: 626c 6522 295d 0a20 2020 2020 2020 2073  ble")].        s
-00010f90: 656c 662e 6d61 7844 6966 6620 3d20 3130  elf.maxDiff = 10
-00010fa0: 3030 300a 0a20 2020 2020 2020 2072 6570  000..        rep
-00010fb0: 6f72 7420 3d20 6f73 2e70 6174 682e 6a6f  ort = os.path.jo
-00010fc0: 696e 2873 656c 662e 7465 6d70 6469 722c  in(self.tempdir,
-00010fd0: 2022 6669 6c74 6572 6564 2e72 6570 6f72   "filtered.repor
-00010fe0: 7422 290a 2020 2020 2020 2020 6765 6e65  t").        gene
-00010ff0: 7261 7465 5f68 6f74 7370 6f74 5f72 6570  rate_hotspot_rep
-00011000: 6f72 7428 2273 616d 706c 6531 222c 0a20  ort("sample1",. 
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011030: 6570 6f72 742c 0a20 2020 2020 2020 2020  eport,.         
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 206c 6576 656c 732c 0a20         levels,. 
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011080: 656c 662e 686f 7473 706f 742c 0a20 2020  elf.hotspot,.   
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000110b0: 662e 7663 665f 7665 7020 2b20 222e 677a  f.vcf_vep + ".gz
-000110c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2073 656c 662e 6776 6366 202b 2022     self.gvcf + "
-000110f0: 2e67 7a22 2c0a 2020 2020 2020 2020 2020  .gz",.          
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 7365 6c66 2e72 6566 6572        self.refer
-00011120: 656e 6365 2c0a 2020 2020 2020 2020 2020  ence,.          
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 2020 2020 7365 6c66 2e76 6366 5f76        self.vcf_v
-00011150: 6570 5f77 6f5f 7069 636b 202b 2022 2e67  ep_wo_pick + ".g
-00011160: 7a22 2c0a 2020 2020 2020 2020 2020 2020  z",.            
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2274 6573 7473 2f75 7469 6c73      "tests/utils
-00011190: 2f66 696c 6573 2f72 6570 6f72 745f 636f  /files/report_co
-000111a0: 6c75 6d6e 735f 7665 705f 7265 6765 785f  lumns_vep_regex_
-000111b0: 6578 7472 6163 742e 7961 6d6c 2229 0a20  extract.yaml"). 
-000111c0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-000111d0: 2872 6570 6f72 742c 2027 7227 2920 6173  (report, 'r') as
-000111e0: 2072 6570 6f72 745f 7265 7375 6c74 3a0a   report_result:.
-000111f0: 2020 2020 2020 2020 2020 2020 6865 6164              head
-00011200: 203d 2072 6570 6f72 745f 7265 7375 6c74   = report_result
-00011210: 2e72 6561 646c 696e 6528 290a 2020 2020  .readline().    
-00011220: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00011230: 6572 7445 7175 616c 2868 6561 642e 7273  ertEqual(head.rs
-00011240: 7472 6970 2829 2c20 225c 7422 2e6a 6f69  trip(), "\t".joi
-00011250: 6e28 5b22 7361 6d70 6c65 222c 2022 6368  n(["sample", "ch
-00011260: 7222 2c20 2273 7461 7274 222c 2022 7374  r", "start", "st
-00011270: 6f70 222c 2022 7265 6622 2c20 2261 6c74  op", "ref", "alt
-00011280: 222c 2022 7265 706f 7274 222c 2027 6776  ", "report", 'gv
-00011290: 6366 5f64 6570 7468 272c 2027 7265 665f  cf_depth', 'ref_
-000112a0: 6465 7074 6827 2c20 2761 6c74 5f64 6570  depth', 'alt_dep
-000112b0: 7468 272c 2027 7273 275d 2929 2020 2320  th', 'rs']))  # 
-000112c0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-000112d0: 2072 6573 756c 7420 3d20 7265 706f 7274   result = report
-000112e0: 5f72 6573 756c 742e 7265 6164 6c69 6e65  _result.readline
-000112f0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00011300: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00011310: 286c 656e 2872 6573 756c 7429 2c20 3133  (len(result), 13
-00011320: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00011330: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00011340: 6573 756c 745b 305d 2e72 7374 7269 7028  esult[0].rstrip(
-00011350: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-00011360: 3030 3030 322e 3131 0932 3934 3435 3237  00002.11.2944527
-00011370: 3109 3239 3434 3532 3731 0947 0941 0931  1.29445271.G.A.1
-00011380: 2d68 6f74 7370 6f74 0936 3230 0933 3539  -hotspot.620.359
-00011390: 0934 092d 2229 2020 2320 6e6f 7161 0a20  .4.-")  # noqa. 
-000113a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000113b0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-000113c0: 6c74 5b31 5d2e 7273 7472 6970 2829 2c20  lt[1].rstrip(), 
-000113d0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-000113e0: 3037 2e31 3309 3134 3034 3938 3335 3909  07.13.140498359.
-000113f0: 3134 3034 3938 3336 3209 4354 5454 0943  140498362.CTTT.C
-00011400: 0932 2d69 6e64 656c 0931 3030 2e35 0932  .2-indel.100.5.2
-00011410: 3709 3409 7273 3132 3734 3436 3031 3737  7.4.rs1274460177
-00011420: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-00011430: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011440: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
-00011450: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-00011460: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
-00011470: 3309 3134 3034 3938 3336 3109 3134 3034  3.140498361.1404
-00011480: 3938 3336 3109 2d09 2d09 312d 686f 7473  98361.-.-.1-hots
-00011490: 706f 7409 3131 3009 2d09 2d09 2d22 2920  pot.110.-.-.-") 
-000114a0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-000114b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000114c0: 4571 7561 6c28 7265 7375 6c74 5b33 5d2e  Equal(result[3].
-000114d0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
-000114e0: 6531 094e 435f 3030 3030 3037 2e31 3309  e1.NC_000007.13.
-000114f0: 3134 3034 3533 3133 3609 3134 3034 3533  140453136.140453
-00011500: 3133 3609 2d09 2d09 312d 686f 7473 706f  136.-.-.1-hotspo
-00011510: 7409 3009 2d09 2d09 2d22 2920 2023 206e  t.0.-.-.-")  # n
-00011520: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00011530: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00011540: 2872 6573 756c 745b 345d 2e72 7374 7269  (result[4].rstri
-00011550: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
-00011560: 5f30 3030 3030 372e 3133 0931 3136 3431  _000007.13.11641
-00011570: 3230 3433 0931 3136 3431 3230 3433 092d  2043.116412043.-
-00011580: 092d 0931 2d68 6f74 7370 6f74 0930 092d  .-.1-hotspot.0.-
-00011590: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
-000115a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000115b0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-000115c0: 6c74 5b35 5d2e 7273 7472 6970 2829 2c20  lt[5].rstrip(), 
-000115d0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-000115e0: 3032 2e31 3109 3239 3434 3532 3732 0932  02.11.29445272.2
-000115f0: 3934 3435 3237 3209 2d09 2d09 332d 6368  9445272.-.-.3-ch
-00011600: 6563 6b09 3232 3109 2d09 2d09 2d22 2920  eck.221.-.-.-") 
-00011610: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00011620: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00011630: 7175 616c 2872 6573 756c 745b 365d 2e72  qual(result[6].r
-00011640: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
-00011650: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
-00011660: 3934 3435 3237 3709 3239 3434 3532 3737  9445277.29445277
-00011670: 092d 092d 0933 2d63 6865 636b 0931 3832  .-.-.3-check.182
-00011680: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
-00011690: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000116a0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-000116b0: 7375 6c74 5b37 5d2e 7273 7472 6970 2829  sult[7].rstrip()
-000116c0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-000116d0: 3030 3038 2e31 3109 3134 3537 3338 3736  0008.11.14573876
-000116e0: 3809 3134 3537 3338 3736 3809 4709 4309  8.145738768.G.C.
-000116f0: 332d 6368 6563 6b09 3135 3437 0935 0932  3-check.1547.5.2
-00011700: 3709 7273 3131 3334 3838 3032 3222 2920  7.rs113488022") 
-00011710: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00011720: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00011730: 7175 616c 2872 6573 756c 745b 385d 2e72  qual(result[8].r
-00011740: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
-00011750: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
-00011760: 3435 3733 3837 3736 0931 3435 3733 3837  45738776.1457387
-00011770: 3736 092d 092d 0933 2d63 6865 636b 0930  76.-.-.3-check.0
-00011780: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
-00011790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000117a0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-000117b0: 7375 6c74 5b39 5d2e 7273 7472 6970 2829  sult[9].rstrip()
-000117c0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-000117d0: 3030 3038 2e31 3109 3134 3537 3432 3531  0008.11.14574251
-000117e0: 3409 3134 3537 3432 3531 3409 4109 4709  4.145742514.A.G.
-000117f0: 332d 6368 6563 6b09 3009 3009 3833 3909  3-check.0.0.839.
-00011800: 7273 3237 3231 3139 3022 2920 2023 206e  rs2721190")  # n
-00011810: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00011820: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00011830: 2872 6573 756c 745b 3130 5d2e 7273 7472  (result[10].rstr
-00011840: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
-00011850: 435f 3030 3030 3136 2e31 3109 3831 3935  C_000016.11.8195
-00011860: 3437 3839 0938 3139 3534 3738 3909 4309  4789.81954789.C.
-00011870: 4754 0932 2d69 6e64 656c 0931 3134 3409  GT.2-indel.1144.
-00011880: 3131 3732 0932 3909 2d22 2920 2023 206e  1172.29.-")  # n
-00011890: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-000118a0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000118b0: 2872 6573 756c 745b 3131 5d2e 7273 7472  (result[11].rstr
-000118c0: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
-000118d0: 435f 3030 3030 3032 2e31 3109 3239 3434  C_000002.11.2944
-000118e0: 3532 3832 0932 3934 3435 3238 3209 4709  5282.29445282.G.
-000118f0: 4109 342d 6f74 6865 7209 3532 3009 3238  A.4-other.520.28
-00011900: 3409 3309 7273 3133 3035 3138 3331 3530  4.3.rs1305183150
-00011910: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-00011920: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011930: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
-00011940: 325d 2e72 7374 7269 7028 292c 2022 7361  2].rstrip(), "sa
-00011950: 6d70 6c65 3109 4e43 5f30 3030 3031 362e  mple1.NC_000016.
-00011960: 3131 0938 3139 3534 3738 3909 3831 3935  11.81954789.8195
-00011970: 3437 3839 0943 0947 0934 2d6f 7468 6572  4789.C.G.4-other
-00011980: 0931 3134 3409 3434 3209 3334 3909 7273  .1144.442.349.rs
-00011990: 3132 3434 3631 3237 2229 2020 2320 6e6f  12446127")  # no
-000119a0: 7161 0a0a 2020 2020 6465 6620 7465 7374  qa..    def test
-000119b0: 5f66 696c 7465 7265 645f 6d75 7461 7469  _filtered_mutati
-000119c0: 6f6e 5f63 6f6d 6269 6e65 5f63 6f6c 756d  on_combine_colum
-000119d0: 6e73 2873 656c 6629 3a0a 2020 2020 2020  ns(self):.      
-000119e0: 2020 6672 6f6d 2068 7964 7261 5f67 656e    from hydra_gen
-000119f0: 6574 6963 732e 7574 696c 732e 696f 2e68  etics.utils.io.h
-00011a00: 6f74 7370 6f74 5f72 6570 6f72 7420 696d  otspot_report im
-00011a10: 706f 7274 2067 656e 6572 6174 655f 686f  port generate_ho
-00011a20: 7473 706f 745f 7265 706f 7274 0a20 2020  tspot_report.   
-00011a30: 2020 2020 206c 6576 656c 7320 3d20 5b28       levels = [(
-00011a40: 3330 302c 2022 6f6b 222c 2022 7965 7322  300, "ok", "yes"
-00011a50: 292c 2028 3330 2c20 226c 6f77 222c 2022  ), (30, "low", "
-00011a60: 7965 7322 292c 2028 302c 2022 6c6f 7722  yes"), (0, "low"
-00011a70: 2c20 226e 6f74 2061 6e61 6c79 7a61 626c  , "not analyzabl
-00011a80: 6522 295d 0a0a 2020 2020 2020 2020 7365  e")]..        se
-00011a90: 6c66 2e6d 6178 4469 6666 203d 2031 3030  lf.maxDiff = 100
-00011aa0: 3030 0a0a 2020 2020 2020 2020 7265 706f  00..        repo
-00011ab0: 7274 203d 206f 732e 7061 7468 2e6a 6f69  rt = os.path.joi
-00011ac0: 6e28 7365 6c66 2e74 656d 7064 6972 2c20  n(self.tempdir, 
-00011ad0: 2266 696c 7465 7265 642e 7265 706f 7274  "filtered.report
-00011ae0: 2229 0a20 2020 2020 2020 2067 656e 6572  ").        gener
-00011af0: 6174 655f 686f 7473 706f 745f 7265 706f  ate_hotspot_repo
-00011b00: 7274 2822 7361 6d70 6c65 3122 2c0a 2020  rt("sample1",.  
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00011b30: 706f 7274 2c0a 2020 2020 2020 2020 2020  port,.          
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 2020 2020 6c65 7665 6c73 2c0a 2020        levels,.  
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011b80: 6c66 2e68 6f74 7370 6f74 2c0a 2020 2020  lf.hotspot,.    
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011bb0: 2e76 6366 5f76 6570 202b 2022 2e67 7a22  .vcf_vep + ".gz"
-00011bc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2020 7365 6c66 2e67 7663 6620 2b20 222e    self.gvcf + ".
-00011bf0: 677a 222c 0a20 2020 2020 2020 2020 2020  gz",.           
-00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c10: 2020 2020 2073 656c 662e 7265 6665 7265       self.refere
-00011c20: 6e63 652c 0a20 2020 2020 2020 2020 2020  nce,.           
-00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c40: 2020 2020 2073 656c 662e 7663 665f 7665       self.vcf_ve
-00011c50: 705f 776f 5f70 6963 6b20 2b20 222e 677a  p_wo_pick + ".gz
-00011c60: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00011c70: 6d61 7844 6966 6620 3d20 3130 3030 300a  maxDiff = 10000.
-00011c80: 0a20 2020 2020 2020 2023 2056 6172 6961  .        # Varia
-00011c90: 6e74 730a 2020 2020 2020 2020 2320 6368  nts.        # ch
-00011ca0: 7232 0932 3934 3435 3237 3109 2e09 4709  r2.29445271...G.
-00011cb0: 4120 2028 3129 0a20 2020 2020 2020 2023  A  (1).        #
-00011cc0: 2063 6872 3209 3239 3434 3532 3832 092e   chr2.29445282..
-00011cd0: 0947 0941 2020 286f 7468 6572 290a 2020  .G.A  (other).  
-00011ce0: 2020 2020 2020 2320 6368 7237 0931 3430        # chr7.140
-00011cf0: 3439 3833 3539 092e 0943 5454 5409 4320  498359...CTTT.C 
-00011d00: 2833 290a 2020 2020 2020 2020 2320 6368  (3).        # ch
-00011d10: 7238 0931 3435 3733 3837 3638 092e 0947  r8.145738768...G
-00011d20: 0943 2028 3629 0a20 2020 2020 2020 2023  .C (6).        #
-00011d30: 2063 6872 3809 3134 3537 3432 3531 3409   chr8.145742514.
-00011d40: 2e09 4109 470a 2020 2020 2020 2020 2320  ..A.G.        # 
-00011d50: 6368 7231 3620 3831 3935 3437 3839 092e  chr16 81954789..
-00011d60: 0943 0947 540a 2020 2020 2020 2020 2320  .C.GT.        # 
-00011d70: 6368 7231 3609 3831 3935 3437 3839 092e  chr16.81954789..
-00011d80: 0943 0947 0a20 2020 2020 2020 2023 0a20  .C.G.        #. 
-00011d90: 2020 2020 2020 2023 2048 6f74 7370 6f74         # Hotspot
-00011da0: 0a20 2020 2020 2020 2023 2031 202d 204e  .        # 1 - N
-00011db0: 435f 3030 3030 3032 2e31 3120 2032 3934  C_000002.11  294
-00011dc0: 3435 3237 3120 2020 2032 3934 3435 3237  45271    2944527
-00011dd0: 3120 2020 2068 6f74 7370 6f74 0a20 2020  1    hotspot.   
-00011de0: 2020 2020 2023 2032 202d 204e 435f 3030       # 2 - NC_00
-00011df0: 3030 3032 2e31 3120 2032 3934 3435 3237  0002.11  2944527
-00011e00: 3120 2020 2032 3934 3435 3238 3120 2020  1    29445281   
-00011e10: 2072 6567 696f 6e5f 616c 6c0a 2020 2020   region_all.    
-00011e20: 2020 2020 2320 3320 2d20 4e43 5f30 3030      # 3 - NC_000
-00011e30: 3030 372e 3133 2020 3134 3034 3938 3336  007.13  14049836
-00011e40: 3120 2020 3134 3034 3938 3336 3120 2020  1   140498361   
-00011e50: 686f 7473 706f 7420 2023 2053 686f 756c  hotspot  # Shoul
-00011e60: 6420 7468 6973 206f 6e65 2062 6520 7072  d this one be pr
-00011e70: 696e 7465 6420 6576 656e 7468 6f75 6768  inted eventhough
-00011e80: 2061 2069 6e64 656c 206f 7665 726c 6170   a indel overlap
-00011e90: 7320 6974 3f0a 2020 2020 2020 2020 2320  s it?.        # 
-00011ea0: 3420 2d20 4e43 5f30 3030 3030 372e 3133  4 - NC_000007.13
-00011eb0: 2020 3134 3034 3533 3133 3620 2020 3134    140453136   14
-00011ec0: 3034 3533 3133 3620 2020 686f 7473 706f  0453136   hotspo
-00011ed0: 740a 2020 2020 2020 2020 2320 3520 2d20  t.        # 5 - 
-00011ee0: 4e43 5f30 3030 3030 372e 3133 2020 3131  NC_000007.13  11
-00011ef0: 3634 3132 3034 3320 2020 3131 3634 3132  6412043   116412
-00011f00: 3034 3320 2020 686f 7473 706f 740a 2020  043   hotspot.  
-00011f10: 2020 2020 2020 2320 3620 2d20 4e43 5f30        # 6 - NC_0
-00011f20: 3030 3030 382e 3131 2020 3134 3537 3338  00008.11  145738
-00011f30: 3736 3520 2020 2031 3435 3733 3837 3739  765    145738779
-00011f40: 2020 2020 7265 6769 6f6e 5f61 6c6c 0a20      region_all. 
-00011f50: 2020 2020 2020 2023 2037 202d 204e 435f         # 7 - NC_
-00011f60: 3030 3030 3038 2e31 3120 2031 3435 3734  000008.11  14574
-00011f70: 3235 3130 2020 2020 3134 3537 3432 3532  2510    14574252
-00011f80: 3420 2020 2072 6567 696f 6e0a 2020 2020  4    region.    
-00011f90: 2020 2020 2320 3820 2d20 4e43 5f30 3030      # 8 - NC_000
-00011fa0: 3031 362e 3131 2020 3831 3935 3437 3835  016.11  81954785
-00011fb0: 2020 2020 3831 3935 3437 3935 2020 2020      81954795    
-00011fc0: 696e 6465 6c0a 2020 2020 2020 2020 230a  indel.        #.
-00011fd0: 2020 2020 2020 2020 7265 706f 7274 203d          report =
-00011fe0: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00011ff0: 6c66 2e74 656d 7064 6972 2c20 2266 696c  lf.tempdir, "fil
-00012000: 7465 7265 642e 7265 706f 7274 2229 0a20  tered.report"). 
-00012010: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
-00012020: 686f 7473 706f 745f 7265 706f 7274 2822  hotspot_report("
-00012030: 7361 6d70 6c65 3122 2c0a 2020 2020 2020  sample1",.      
-00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012050: 2020 2020 2020 2020 2020 7265 706f 7274            report
-00012060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2020 6c65 7665 6c73 2c0a 2020 2020 2020    levels,.      
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-000120b0: 6f74 7370 6f74 2c0a 2020 2020 2020 2020  otspot,.        
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 2020 2020 2020 2020 7365 6c66 2e76 6366          self.vcf
-000120e0: 5f76 6570 202b 2022 2e67 7a22 2c0a 2020  _vep + ".gz",.  
-000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012110: 6c66 2e67 7663 6620 2b20 222e 677a 222c  lf.gvcf + ".gz",
-00012120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2073 656c 662e 7265 6665 7265 6e63 652c   self.reference,
-00012150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2073 656c 662e 7663 665f 7665 705f 776f   self.vcf_vep_wo
-00012180: 5f70 6963 6b20 2b20 222e 677a 222c 0a20  _pick + ".gz",. 
-00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000121b0: 7465 7374 732f 7574 696c 732f 6669 6c65  tests/utils/file
-000121c0: 732f 7265 706f 7274 5f63 6f6c 756d 6e73  s/report_columns
-000121d0: 5f63 6f6d 6269 6e65 5f63 6f6c 756d 6e73  _combine_columns
-000121e0: 2e79 616d 6c22 290a 2020 2020 2020 2020  .yaml").        
-000121f0: 7769 7468 206f 7065 6e28 7265 706f 7274  with open(report
-00012200: 2c20 2772 2729 2061 7320 7265 706f 7274  , 'r') as report
-00012210: 5f72 6573 756c 743a 0a20 2020 2020 2020  _result:.       
-00012220: 2020 2020 2068 6561 6420 3d20 7265 706f       head = repo
-00012230: 7274 5f72 6573 756c 742e 7265 6164 6c69  rt_result.readli
-00012240: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
-00012250: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00012260: 6c28 6865 6164 2e72 7374 7269 7028 292c  l(head.rstrip(),
-00012270: 2022 5c74 222e 6a6f 696e 285b 2273 616d   "\t".join(["sam
-00012280: 706c 6522 2c20 2263 6872 222c 2022 7374  ple", "chr", "st
-00012290: 6172 7422 2c20 2273 746f 7022 2c20 2272  art", "stop", "r
-000122a0: 6566 222c 2022 616c 7422 2c20 2272 6570  ef", "alt", "rep
-000122b0: 6f72 7422 2c20 2767 7663 665f 6465 7074  ort", 'gvcf_dept
-000122c0: 6827 2c20 2272 6566 5f64 6570 7468 222c  h', "ref_depth",
-000122d0: 2022 616c 745f 6465 7074 6822 2c20 2741   "alt_depth", 'A
-000122e0: 6e61 6c79 7a61 626c 6527 2c20 274d 696e  nalyzable', 'Min
-000122f0: 5f72 6561 645f 6465 7074 6833 3030 272c  _read_depth300',
-00012300: 2027 4765 6e65 5f76 6570 3b68 6f74 7370   'Gene_vep;hotsp
-00012310: 6f74 272c 2027 5661 7269 616e 745f 7479  ot', 'Variant_ty
-00012320: 7065 272c 2027 436f 6e73 6571 7565 6e63  pe', 'Consequenc
-00012330: 6527 2c20 2743 616c 6c65 7273 272c 2027  e', 'Callers', '
-00012340: 436f 6d6d 656e 7427 5d29 2920 2023 206e  Comment']))  # n
-00012350: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00012360: 7265 7375 6c74 203d 2072 6570 6f72 745f  result = report_
-00012370: 7265 7375 6c74 2e72 6561 646c 696e 6573  result.readlines
-00012380: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00012390: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000123a0: 6c65 6e28 7265 7375 6c74 292c 2031 3329  len(result), 13)
-000123b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000123c0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-000123d0: 7375 6c74 5b30 5d2e 7273 7472 6970 2829  sult[0].rstrip()
-000123e0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-000123f0: 3030 3032 2e31 3109 3239 3434 3532 3731  0002.11.29445271
-00012400: 0932 3934 3435 3237 3109 4709 4109 312d  .29445271.G.A.1-
-00012410: 686f 7473 706f 7409 3632 3009 3335 392e  hotspot.620.359.
-00012420: 3030 0934 0979 6573 096f 6b09 414c 4b3b  00.4.yes.ok.ALK;
-00012430: 414c 4b09 7072 6f74 6569 6e5f 636f 6469  ALK.protein_codi
-00012440: 6e67 0973 796e 6f6e 796d 6f75 735f 7661  ng.synonymous_va
-00012450: 7269 616e 7409 7661 7264 6963 7409 7265  riant.vardict.re
-00012460: 7369 7374 616e 6365 5f6d 7574 6174 696f  sistance_mutatio
-00012470: 6e22 2920 2023 206e 6f71 610a 2020 2020  n")  # noqa.    
-00012480: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00012490: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-000124a0: 315d 2e72 7374 7269 7028 292c 2022 7361  1].rstrip(), "sa
-000124b0: 6d70 6c65 3109 4e43 5f30 3030 3030 372e  mple1.NC_000007.
-000124c0: 3133 0931 3430 3439 3833 3539 0931 3430  13.140498359.140
-000124d0: 3439 3833 3632 0943 5454 5409 4309 322d  498362.CTTT.C.2-
-000124e0: 696e 6465 6c09 3130 302e 3509 3237 2e30  indel.100.5.27.0
-000124f0: 3009 3409 7965 7309 6c6f 7709 4252 4146  0.4.yes.low.BRAF
-00012500: 3b45 4746 5209 7072 6f74 6569 6e5f 636f  ;EGFR.protein_co
-00012510: 6469 6e67 0969 6e74 726f 6e5f 7661 7269  ding.intron_vari
-00012520: 616e 7409 6d75 7465 6374 3209 2d22 2920  ant.mutect2.-") 
-00012530: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00012540: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00012550: 7175 616c 2872 6573 756c 745b 325d 2e72  qual(result[2].r
-00012560: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
-00012570: 3109 4e43 5f30 3030 3030 372e 3133 0931  1.NC_000007.13.1
-00012580: 3430 3439 3833 3631 0931 3430 3439 3833  40498361.1404983
-00012590: 3631 092d 092d 0931 2d68 6f74 7370 6f74  61.-.-.1-hotspot
-000125a0: 0931 3130 092d 092d 0979 6573 096c 6f77  .110.-.-.yes.low
-000125b0: 092d 3b45 4746 5209 2d09 2d09 2d09 2d22  .-;EGFR.-.-.-.-"
-000125c0: 2920 2020 2320 6e6f 7161 0a20 2020 2020  )   # noqa.     
-000125d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000125e0: 7274 4571 7561 6c28 7265 7375 6c74 5b33  rtEqual(result[3
-000125f0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-00012600: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
-00012610: 3309 3134 3034 3533 3133 3609 3134 3034  3.140453136.1404
-00012620: 3533 3133 3609 2d09 2d09 312d 686f 7473  53136.-.-.1-hots
-00012630: 706f 7409 3009 2d09 2d09 6e6f 7420 616e  pot.0.-.-.not an
-00012640: 616c 797a 6162 6c65 096c 6f77 092d 3b42  alyzable.low.-;B
-00012650: 5241 4609 2d09 2d09 2d09 2d22 2920 2023  RAF.-.-.-.-")  #
-00012660: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
-00012670: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00012680: 616c 2872 6573 756c 745b 345d 2e72 7374  al(result[4].rst
-00012690: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
-000126a0: 4e43 5f30 3030 3030 372e 3133 0931 3136  NC_000007.13.116
-000126b0: 3431 3230 3433 0931 3136 3431 3230 3433  412043.116412043
-000126c0: 092d 092d 0931 2d68 6f74 7370 6f74 0930  .-.-.1-hotspot.0
-000126d0: 092d 092d 096e 6f74 2061 6e61 6c79 7a61  .-.-.not analyza
-000126e0: 626c 6509 6c6f 7709 2d3b 4d45 5409 2d09  ble.low.-;MET.-.
-000126f0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
-00012700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012710: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-00012720: 756c 745b 355d 2e72 7374 7269 7028 292c  ult[5].rstrip(),
-00012730: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
-00012740: 3030 322e 3131 0932 3934 3435 3237 3209  002.11.29445272.
-00012750: 3239 3434 3532 3732 092d 092d 0933 2d63  29445272.-.-.3-c
-00012760: 6865 636b 0932 3231 092d 092d 0979 6573  heck.221.-.-.yes
-00012770: 096c 6f77 092d 3b41 4c4b 092d 092d 092d  .low.-;ALK.-.-.-
-00012780: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
-00012790: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000127a0: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-000127b0: 5b36 5d2e 7273 7472 6970 2829 2c20 2273  [6].rstrip(), "s
-000127c0: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
-000127d0: 2e31 3109 3239 3434 3532 3737 0932 3934  .11.29445277.294
-000127e0: 3435 3237 3709 2d09 2d09 332d 6368 6563  45277.-.-.3-chec
-000127f0: 6b09 3138 3209 2d09 2d09 7965 7309 6c6f  k.182.-.-.yes.lo
-00012800: 7709 2d3b 414c 4b09 2d09 2d09 2d09 2d22  w.-;ALK.-.-.-.-"
-00012810: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
-00012820: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00012830: 7445 7175 616c 2872 6573 756c 745b 375d  tEqual(result[7]
-00012840: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
-00012850: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
-00012860: 0931 3435 3733 3837 3638 0931 3435 3733  .145738768.14573
-00012870: 3837 3638 0947 0943 0933 2d63 6865 636b  8768.G.C.3-check
-00012880: 0931 3534 3709 352e 3030 0932 3709 7965  .1547.5.00.27.ye
-00012890: 7309 6f6b 094c 5252 4331 343b 2d09 7072  s.ok.LRRC14;-.pr
-000128a0: 6f74 6569 6e5f 636f 6469 6e67 0975 7073  otein_coding.ups
-000128b0: 7472 6561 6d5f 6765 6e65 5f76 6172 6961  tream_gene_varia
-000128c0: 6e74 0976 6172 6469 6374 092d 2229 2020  nt.vardict.-")  
-000128d0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-000128e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000128f0: 7561 6c28 7265 7375 6c74 5b38 5d2e 7273  ual(result[8].rs
-00012900: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-00012910: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
-00012920: 3537 3338 3737 3609 3134 3537 3338 3737  5738776.14573877
-00012930: 3609 2d09 2d09 332d 6368 6563 6b09 3009  6.-.-.3-check.0.
-00012940: 2d09 2d09 6e6f 7420 616e 616c 797a 6162  -.-.not analyzab
-00012950: 6c65 096c 6f77 092d 3b2d 092d 092d 092d  le.low.-;-.-.-.-
-00012960: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
-00012970: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00012980: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-00012990: 5b39 5d2e 7273 7472 6970 2829 2c20 2273  [9].rstrip(), "s
-000129a0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
-000129b0: 2e31 3109 3134 3537 3432 3531 3409 3134  .11.145742514.14
-000129c0: 3537 3432 3531 3409 4109 4709 332d 6368  5742514.A.G.3-ch
-000129d0: 6563 6b09 3009 302e 3030 0938 3339 096e  eck.0.0.00.839.n
-000129e0: 6f74 2061 6e61 6c79 7a61 626c 6509 6c6f  ot analyzable.lo
-000129f0: 7709 5245 4351 4c34 3b2d 0970 726f 7465  w.RECQL4;-.prote
-00012a00: 696e 5f63 6f64 696e 6709 7379 6e6f 6e79  in_coding.synony
-00012a10: 6d6f 7573 5f76 6172 6961 6e74 0976 6172  mous_variant.var
-00012a20: 6469 6374 2c6d 7574 6563 7432 092d 2229  dict,mutect2.-")
-00012a30: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-00012a40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00012a50: 4571 7561 6c28 7265 7375 6c74 5b31 305d  Equal(result[10]
-00012a60: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
-00012a70: 6c65 3109 4e43 5f30 3030 3031 362e 3131  le1.NC_000016.11
-00012a80: 0938 3139 3534 3738 3909 3831 3935 3437  .81954789.819547
-00012a90: 3839 0943 0947 5409 322d 696e 6465 6c09  89.C.GT.2-indel.
-00012aa0: 3131 3434 0931 3137 322e 3030 0932 3909  1144.1172.00.29.
-00012ab0: 7965 7309 6f6b 0950 4c43 4732 3b2d 0970  yes.ok.PLCG2;-.p
-00012ac0: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-00012ad0: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-00012ae0: 6469 6374 092d 2229 2020 2320 6e6f 7161  dict.-")  # noqa
-00012af0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012b00: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00012b10: 7375 6c74 5b31 315d 2e72 7374 7269 7028  sult[11].rstrip(
-00012b20: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-00012b30: 3030 3030 322e 3131 0932 3934 3435 3238  00002.11.2944528
-00012b40: 3209 3239 3434 3532 3832 0947 0941 0934  2.29445282.G.A.4
-00012b50: 2d6f 7468 6572 0935 3230 0932 3834 2e30  -other.520.284.0
-00012b60: 3009 3309 7965 7309 6f6b 0941 4c4b 3b2d  0.3.yes.ok.ALK;-
-00012b70: 0970 726f 7465 696e 5f63 6f64 696e 6709  .protein_coding.
-00012b80: 7370 6c69 6365 5f72 6567 696f 6e5f 7661  splice_region_va
-00012b90: 7269 616e 7426 696e 7472 6f6e 5f76 6172  riant&intron_var
-00012ba0: 6961 6e74 0976 6172 6469 6374 092d 2229  iant.vardict.-")
-00012bb0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-00012bc0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00012bd0: 4571 7561 6c28 7265 7375 6c74 5b31 325d  Equal(result[12]
-00012be0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
-00012bf0: 6c65 3109 4e43 5f30 3030 3031 362e 3131  le1.NC_000016.11
-00012c00: 0938 3139 3534 3738 3909 3831 3935 3437  .81954789.819547
-00012c10: 3839 0943 0947 0934 2d6f 7468 6572 0931  89.C.G.4-other.1
-00012c20: 3134 3409 3434 322e 3030 0933 3439 0979  144.442.00.349.y
-00012c30: 6573 096f 6b09 c2b4 5345 5054 3b2d 0970  es.ok...SEPT;-.p
-00012c40: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-00012c50: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-00012c60: 6469 6374 2c6d 7574 6563 7432 092d 2229  dict,mutect2.-")
-00012c70: 2020 2320 6e6f 7161 0a0a 2020 2020 2020    # noqa..      
-00012c80: 2020 7265 706f 7274 203d 206f 732e 7061    report = os.pa
-00012c90: 7468 2e6a 6f69 6e28 7365 6c66 2e74 656d  th.join(self.tem
-00012ca0: 7064 6972 2c20 2266 696c 7465 7265 642e  pdir, "filtered.
-00012cb0: 7265 706f 7274 2229 0a20 2020 2020 2020  report").       
-00012cc0: 2067 656e 6572 6174 655f 686f 7473 706f   generate_hotspo
-00012cd0: 745f 7265 706f 7274 2822 7361 6d70 6c65  t_report("sample
-00012ce0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2020 7265 706f 7274 2c0a 2020 2020      report,.    
-00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d20: 2020 2020 2020 2020 2020 2020 6c65 7665              leve
-00012d30: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00012d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d50: 2020 2020 7365 6c66 2e68 6f74 7370 6f74      self.hotspot
-00012d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 7365 6c66 2e76 6366 5f76 6570 202b    self.vcf_vep +
-00012d90: 2022 2e67 7a22 2c0a 2020 2020 2020 2020   ".gz",.        
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 2020 2020 7365 6c66 2e67 7663          self.gvc
-00012dc0: 6620 2b20 222e 677a 222c 0a20 2020 2020  f + ".gz",.     
-00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012df0: 7265 6665 7265 6e63 652c 0a20 2020 2020  reference,.     
-00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012e20: 7663 665f 7665 705f 776f 5f70 6963 6b20  vcf_vep_wo_pick 
-00012e30: 2b20 222e 677a 222c 0a20 2020 2020 2020  + ".gz",.       
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2020 2022 7465 7374 732f           "tests/
-00012e60: 7574 696c 732f 6669 6c65 732f 7265 706f  utils/files/repo
-00012e70: 7274 5f63 6f6c 756d 6e73 5f63 6f6d 6269  rt_columns_combi
-00012e80: 6e65 5f63 6f6c 756d 6e73 5f6d 756c 7469  ne_columns_multi
-00012e90: 5f6c 6576 656c 2e79 616d 6c22 290a 2020  _level.yaml").  
-00012ea0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00012eb0: 7265 706f 7274 2c20 2772 2729 2061 7320  report, 'r') as 
-00012ec0: 7265 706f 7274 5f72 6573 756c 743a 0a20  report_result:. 
-00012ed0: 2020 2020 2020 2020 2020 2068 6561 6420             head 
-00012ee0: 3d20 7265 706f 7274 5f72 6573 756c 742e  = report_result.
-00012ef0: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
-00012f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00012f10: 7274 4571 7561 6c28 6865 6164 2e72 7374  rtEqual(head.rst
-00012f20: 7269 7028 292c 2022 5c74 222e 6a6f 696e  rip(), "\t".join
-00012f30: 285b 2273 616d 706c 6522 2c20 2263 6872  (["sample", "chr
-00012f40: 222c 2022 7374 6172 7422 2c20 2273 746f  ", "start", "sto
-00012f50: 7022 2c20 2272 6566 222c 2022 616c 7422  p", "ref", "alt"
-00012f60: 2c20 2272 6570 6f72 7422 2c20 2767 7663  , "report", 'gvc
-00012f70: 665f 6465 7074 6827 2c20 2272 6566 5f64  f_depth', "ref_d
-00012f80: 6570 7468 222c 2022 616c 745f 6465 7074  epth", "alt_dept
-00012f90: 6822 2c20 2741 6e61 6c79 7a61 626c 6527  h", 'Analyzable'
-00012fa0: 2c20 274d 696e 5f72 6561 645f 6465 7074  , 'Min_read_dept
-00012fb0: 6833 3030 272c 2027 4765 6e65 5f76 6570  h300', 'Gene_vep
-00012fc0: 3b68 6f74 7370 6f74 5f61 613a 6364 7327  ;hotspot_aa:cds'
-00012fd0: 2c20 2756 6172 6961 6e74 5f74 7970 6527  , 'Variant_type'
-00012fe0: 2c20 2743 6f6e 7365 7175 656e 6365 272c  , 'Consequence',
-00012ff0: 2027 4361 6c6c 6572 7327 2c20 2743 6f6d   'Callers', 'Com
-00013000: 6d65 6e74 275d 2929 2020 2320 6e6f 7161  ment']))  # noqa
-00013010: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00013020: 756c 7420 3d20 7265 706f 7274 5f72 6573  ult = report_res
-00013030: 756c 742e 7265 6164 6c69 6e65 7328 290a  ult.readlines().
-00013040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013050: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00013060: 2872 6573 756c 7429 2c20 3133 290a 2020  (result), 13).  
-00013070: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00013080: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-00013090: 745b 305d 2e72 7374 7269 7028 292c 2022  t[0].rstrip(), "
-000130a0: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
-000130b0: 322e 3131 0932 3934 3435 3237 3109 3239  2.11.29445271.29
-000130c0: 3434 3532 3731 0947 0941 0931 2d68 6f74  445271.G.A.1-hot
-000130d0: 7370 6f74 0936 3230 0933 3539 0934 0979  spot.620.359.4.y
-000130e0: 6573 096f 6b09 414c 4b3b 702e 4331 3135  es.ok.ALK;p.C115
-000130f0: 363a 632e 4733 3436 3709 7072 6f74 6569  6:c.G3467.protei
-00013100: 6e5f 636f 6469 6e67 0973 796e 6f6e 796d  n_coding.synonym
-00013110: 6f75 735f 7661 7269 616e 7409 7661 7264  ous_variant.vard
-00013120: 6963 7409 7265 7369 7374 616e 6365 5f6d  ict.resistance_m
-00013130: 7574 6174 696f 6e22 2920 2023 206e 6f71  utation")  # noq
-00013140: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00013150: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00013160: 6573 756c 745b 315d 2e72 7374 7269 7028  esult[1].rstrip(
-00013170: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-00013180: 3030 3030 372e 3133 0931 3430 3439 3833  00007.13.1404983
-00013190: 3539 0931 3430 3439 3833 3632 0943 5454  59.140498362.CTT
-000131a0: 5409 4309 322d 696e 6465 6c09 3130 302e  T.C.2-indel.100.
-000131b0: 3509 3237 0934 0979 6573 096c 6f77 0942  5.27.4.yes.low.B
-000131c0: 5241 463b 702e 4537 3436 3a63 2e47 3232  RAF;p.E746:c.G22
-000131d0: 3336 0970 726f 7465 696e 5f63 6f64 696e  36.protein_codin
-000131e0: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
-000131f0: 096d 7574 6563 7432 092d 2229 2020 2320  .mutect2.-")  # 
-00013200: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00013210: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00013220: 6c28 7265 7375 6c74 5b32 5d2e 7273 7472  l(result[2].rstr
-00013230: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
-00013240: 435f 3030 3030 3037 2e31 3309 3134 3034  C_000007.13.1404
-00013250: 3938 3336 3109 3134 3034 3938 3336 3109  98361.140498361.
-00013260: 2d09 2d09 312d 686f 7473 706f 7409 3131  -.-.1-hotspot.11
-00013270: 3009 2d09 2d09 7965 7309 6c6f 7709 2d3b  0.-.-.yes.low.-;
-00013280: 702e 4537 3436 3a63 2e47 3232 3336 092d  p.E746:c.G2236.-
-00013290: 092d 092d 092d 2229 2020 2023 206e 6f71  .-.-.-")   # noq
-000132a0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-000132b0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-000132c0: 6573 756c 745b 335d 2e72 7374 7269 7028  esult[3].rstrip(
-000132d0: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-000132e0: 3030 3030 372e 3133 0931 3430 3435 3331  00007.13.1404531
-000132f0: 3336 0931 3430 3435 3331 3336 092d 092d  36.140453136.-.-
-00013300: 0931 2d68 6f74 7370 6f74 0930 092d 092d  .1-hotspot.0.-.-
-00013310: 096e 6f74 2061 6e61 6c79 7a61 626c 6509  .not analyzable.
-00013320: 6c6f 7709 2d3b 702e 5636 3030 3a63 2e54  low.-;p.V600:c.T
-00013330: 3137 3939 092d 092d 092d 092d 2229 2020  1799.-.-.-.-")  
-00013340: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00013350: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00013360: 7561 6c28 7265 7375 6c74 5b34 5d2e 7273  ual(result[4].rs
-00013370: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-00013380: 094e 435f 3030 3030 3037 2e31 3309 3131  .NC_000007.13.11
-00013390: 3634 3132 3034 3309 3131 3634 3132 3034  6412043.11641204
-000133a0: 3309 2d09 2d09 312d 686f 7473 706f 7409  3.-.-.1-hotspot.
-000133b0: 3009 2d09 2d09 6e6f 7420 616e 616c 797a  0.-.-.not analyz
-000133c0: 6162 6c65 096c 6f77 092d 3b70 2e44 3130  able.low.-;p.D10
-000133d0: 3238 3a63 2e47 3330 3832 092d 092d 092d  28:c.G3082.-.-.-
-000133e0: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
-000133f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00013400: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
-00013410: 5b35 5d2e 7273 7472 6970 2829 2c20 2273  [5].rstrip(), "s
-00013420: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
-00013430: 2e31 3109 3239 3434 3532 3732 0932 3934  .11.29445272.294
-00013440: 3435 3237 3209 2d09 2d09 332d 6368 6563  45272.-.-.3-chec
-00013450: 6b09 3232 3109 2d09 2d09 7965 7309 6c6f  k.221.-.-.yes.lo
-00013460: 7709 2d3b 702e 4331 3135 363a 632e 4733  w.-;p.C1156:c.G3
-00013470: 3436 3709 2d09 2d09 2d09 2d22 2920 2023  467.-.-.-.-")  #
-00013480: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
-00013490: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000134a0: 616c 2872 6573 756c 745b 365d 2e72 7374  al(result[6].rst
-000134b0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
-000134c0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
-000134d0: 3435 3237 3709 3239 3434 3532 3737 092d  45277.29445277.-
-000134e0: 092d 0933 2d63 6865 636b 0931 3832 092d  .-.3-check.182.-
-000134f0: 092d 0979 6573 096c 6f77 092d 3b70 2e43  .-.yes.low.-;p.C
-00013500: 3131 3536 3a63 2e47 3334 3637 092d 092d  1156:c.G3467.-.-
-00013510: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
-00013520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013530: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-00013540: 6c74 5b37 5d2e 7273 7472 6970 2829 2c20  lt[7].rstrip(), 
-00013550: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-00013560: 3038 2e31 3109 3134 3537 3338 3736 3809  08.11.145738768.
-00013570: 3134 3537 3338 3736 3809 4709 4309 332d  145738768.G.C.3-
-00013580: 6368 6563 6b09 3135 3437 0935 0932 3709  check.1547.5.27.
-00013590: 7965 7309 6f6b 094c 5252 4331 343b 2d3a  yes.ok.LRRC14;-:
-000135a0: 2d09 7072 6f74 6569 6e5f 636f 6469 6e67  -.protein_coding
-000135b0: 0975 7073 7472 6561 6d5f 6765 6e65 5f76  .upstream_gene_v
-000135c0: 6172 6961 6e74 0976 6172 6469 6374 092d  ariant.vardict.-
-000135d0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-000135e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000135f0: 7274 4571 7561 6c28 7265 7375 6c74 5b38  rtEqual(result[8
-00013600: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-00013610: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
-00013620: 3109 3134 3537 3338 3737 3609 3134 3537  1.145738776.1457
-00013630: 3338 3737 3609 2d09 2d09 332d 6368 6563  38776.-.-.3-chec
-00013640: 6b09 3009 2d09 2d09 6e6f 7420 616e 616c  k.0.-.-.not anal
-00013650: 797a 6162 6c65 096c 6f77 092d 3b2d 3a2d  yzable.low.-;-:-
-00013660: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
-00013670: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-00013680: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00013690: 7265 7375 6c74 5b39 5d2e 7273 7472 6970  result[9].rstrip
-000136a0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-000136b0: 3030 3030 3038 2e31 3109 3134 3537 3432  000008.11.145742
-000136c0: 3531 3409 3134 3537 3432 3531 3409 4109  514.145742514.A.
-000136d0: 4709 332d 6368 6563 6b09 3009 3009 3833  G.3-check.0.0.83
-000136e0: 3909 6e6f 7420 616e 616c 797a 6162 6c65  9.not analyzable
-000136f0: 096c 6f77 0952 4543 514c 343b 2d3a 2d09  .low.RECQL4;-:-.
-00013700: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-00013710: 796e 6f6e 796d 6f75 735f 7661 7269 616e  ynonymous_varian
-00013720: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
-00013730: 3209 2d22 2920 2023 206e 6f71 610a 2020  2.-")  # noqa.  
-00013740: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00013750: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-00013760: 745b 3130 5d2e 7273 7472 6970 2829 2c20  t[10].rstrip(), 
-00013770: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-00013780: 3136 2e31 3109 3831 3935 3437 3839 0938  16.11.81954789.8
-00013790: 3139 3534 3738 3909 4309 4754 0932 2d69  1954789.C.GT.2-i
-000137a0: 6e64 656c 0931 3134 3409 3131 3732 0932  ndel.1144.1172.2
-000137b0: 3909 7965 7309 6f6b 0950 4c43 4732 3b2d  9.yes.ok.PLCG2;-
-000137c0: 3a2d 0970 726f 7465 696e 5f63 6f64 696e  :-.protein_codin
-000137d0: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
-000137e0: 0976 6172 6469 6374 092d 2229 2020 2320  .vardict.-")  # 
-000137f0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00013800: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00013810: 6c28 7265 7375 6c74 5b31 315d 2e72 7374  l(result[11].rst
-00013820: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
-00013830: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
-00013840: 3435 3238 3209 3239 3434 3532 3832 0947  45282.29445282.G
-00013850: 0941 0934 2d6f 7468 6572 0935 3230 0932  .A.4-other.520.2
-00013860: 3834 0933 0979 6573 096f 6b09 414c 4b3b  84.3.yes.ok.ALK;
-00013870: 2d3a 2d09 7072 6f74 6569 6e5f 636f 6469  -:-.protein_codi
-00013880: 6e67 0973 706c 6963 655f 7265 6769 6f6e  ng.splice_region
-00013890: 5f76 6172 6961 6e74 2669 6e74 726f 6e5f  _variant&intron_
-000138a0: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
-000138b0: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
-000138c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000138d0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-000138e0: 3132 5d2e 7273 7472 6970 2829 2c20 2273  12].rstrip(), "s
-000138f0: 616d 706c 6531 094e 435f 3030 3030 3136  ample1.NC_000016
-00013900: 2e31 3109 3831 3935 3437 3839 0938 3139  .11.81954789.819
-00013910: 3534 3738 3909 4309 4709 342d 6f74 6865  54789.C.G.4-othe
-00013920: 7209 3131 3434 0934 3432 0933 3439 0979  r.1144.442.349.y
-00013930: 6573 096f 6b09 5345 5054 3b2d 3a2d 0970  es.ok.SEPT;-:-.p
-00013940: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-00013950: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-00013960: 6469 6374 2c6d 7574 6563 7432 092d 2229  dict,mutect2.-")
-00013970: 2020 2320 6e6f 7161 0a0a 2020 2020 6465    # noqa..    de
-00013980: 6620 7465 7374 5f66 696c 7465 7265 645f  f test_filtered_
-00013990: 6d75 7461 7469 6f6e 5f73 656c 6563 745f  mutation_select_
-000139a0: 6f6e 655f 636f 6c75 6d6e 7328 7365 6c66  one_columns(self
-000139b0: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
-000139c0: 6879 6472 615f 6765 6e65 7469 6373 2e75  hydra_genetics.u
-000139d0: 7469 6c73 2e69 6f2e 686f 7473 706f 745f  tils.io.hotspot_
-000139e0: 7265 706f 7274 2069 6d70 6f72 7420 6765  report import ge
-000139f0: 6e65 7261 7465 5f68 6f74 7370 6f74 5f72  nerate_hotspot_r
-00013a00: 6570 6f72 740a 2020 2020 2020 2020 6c65  eport.        le
-00013a10: 7665 6c73 203d 205b 2833 3030 2c20 226f  vels = [(300, "o
-00013a20: 6b22 2c20 2279 6573 2229 2c20 2833 302c  k", "yes"), (30,
-00013a30: 2022 6c6f 7722 2c20 2279 6573 2229 2c20   "low", "yes"), 
-00013a40: 2830 2c20 226c 6f77 222c 2022 6e6f 7420  (0, "low", "not 
-00013a50: 616e 616c 797a 6162 6c65 2229 5d0a 0a20  analyzable")].. 
-00013a60: 2020 2020 2020 2073 656c 662e 6d61 7844         self.maxD
-00013a70: 6966 6620 3d20 3130 3030 300a 0a20 2020  iff = 10000..   
-00013a80: 2020 2020 2072 6570 6f72 7420 3d20 6f73       report = os
-00013a90: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00013aa0: 7465 6d70 6469 722c 2022 6669 6c74 6572  tempdir, "filter
-00013ab0: 6564 2e72 6570 6f72 7422 290a 2020 2020  ed.report").    
-00013ac0: 2020 2020 6765 6e65 7261 7465 5f68 6f74      generate_hot
-00013ad0: 7370 6f74 5f72 6570 6f72 7428 2273 616d  spot_report("sam
-00013ae0: 706c 6531 222c 0a20 2020 2020 2020 2020  ple1",.         
-00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b00: 2020 2020 2020 2072 6570 6f72 742c 0a20         report,. 
-00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b20: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00013b30: 6576 656c 732c 0a20 2020 2020 2020 2020  evels,.         
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b50: 2020 2020 2020 2073 656c 662e 686f 7473         self.hots
-00013b60: 706f 742c 0a20 2020 2020 2020 2020 2020  pot,.           
+0000f0c0: 6573 756c 745b 3330 5d2e 7273 7472 6970  esult[30].rstrip
+0000f0d0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+0000f0e0: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
+0000f0f0: 3737 3909 3134 3537 3338 3737 3909 2d09  779.145738779.-.
+0000f100: 2d09 332d 6368 6563 6b09 3139 3538 092d  -.3-check.1958.-
+0000f110: 092d 2229 0a20 2020 2020 2020 2020 2020  .-").           
+0000f120: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000f130: 6c28 7265 7375 6c74 5b33 315d 2e72 7374  l(result[31].rst
+0000f140: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0000f150: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+0000f160: 3734 3235 3134 0931 3435 3734 3235 3134  742514.145742514
+0000f170: 0941 0947 0933 2d63 6865 636b 0930 0930  .A.G.3-check.0.0
+0000f180: 0938 3339 2229 0a20 2020 2020 2020 2020  .839").         
+0000f190: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000f1a0: 7561 6c28 7265 7375 6c74 5b33 325d 2e72  ual(result[32].r
+0000f1b0: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0000f1c0: 3109 4e43 5f30 3030 3031 362e 3131 0938  1.NC_000016.11.8
+0000f1d0: 3139 3534 3738 3909 3831 3935 3437 3839  1954789.81954789
+0000f1e0: 0943 0947 5409 322d 696e 6465 6c09 3131  .C.GT.2-indel.11
+0000f1f0: 3434 0931 3137 3209 3239 2229 0a20 2020  44.1172.29").   
+0000f200: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000f210: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+0000f220: 5b33 335d 2e72 7374 7269 7028 292c 2022  [33].rstrip(), "
+0000f230: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0000f240: 322e 3131 0932 3934 3435 3238 3209 3239  2.11.29445282.29
+0000f250: 3434 3532 3832 0947 0941 0934 2d6f 7468  445282.G.A.4-oth
+0000f260: 6572 0935 3230 0932 3834 0933 2229 0a20  er.520.284.3"). 
+0000f270: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f280: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0000f290: 6c74 5b33 345d 2e72 7374 7269 7028 292c  lt[34].rstrip(),
+0000f2a0: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0000f2b0: 3031 362e 3131 0938 3139 3534 3738 3909  016.11.81954789.
+0000f2c0: 3831 3935 3437 3839 0943 0947 0934 2d6f  81954789.C.G.4-o
+0000f2d0: 7468 6572 0931 3134 3409 3434 3209 3334  ther.1144.442.34
+0000f2e0: 3922 290a 0a20 2020 2020 2020 2072 6570  9")..        rep
+0000f2f0: 6f72 7420 3d20 6f73 2e70 6174 682e 6a6f  ort = os.path.jo
+0000f300: 696e 2873 656c 662e 7465 6d70 6469 722c  in(self.tempdir,
+0000f310: 2022 6669 6c74 6572 6564 2e72 6570 6f72   "filtered.repor
+0000f320: 7422 290a 2020 2020 2020 2020 6765 6e65  t").        gene
+0000f330: 7261 7465 5f68 6f74 7370 6f74 5f72 6570  rate_hotspot_rep
+0000f340: 6f72 7428 2273 616d 706c 6531 222c 0a20  ort("sample1",. 
+0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f360: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f370: 6570 6f72 742c 0a20 2020 2020 2020 2020  eport,.         
+0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f390: 2020 2020 2020 206c 6576 656c 732c 0a20         levels,. 
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f3c0: 656c 662e 686f 7473 706f 742c 0a20 2020  elf.hotspot,.   
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f3f0: 662e 7663 665f 7665 7020 2b20 222e 677a  f.vcf_vep + ".gz
+0000f400: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f420: 2020 2073 656c 662e 6776 6366 202b 2022     self.gvcf + "
+0000f430: 2e67 7a22 2c0a 2020 2020 2020 2020 2020  .gz",.          
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 2020 2020 2020 7365 6c66 2e72 6566 6572        self.refer
+0000f460: 656e 6365 2c0a 2020 2020 2020 2020 2020  ence,.          
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 2020 2020 2020 7365 6c66 2e76 6366 5f76        self.vcf_v
+0000f490: 6570 5f77 6f5f 7069 636b 202b 2022 2e67  ep_wo_pick + ".g
+0000f4a0: 7a22 2c0a 2020 2020 2020 2020 2020 2020  z",.            
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4c0: 2020 2020 2274 6573 7473 2f75 7469 6c73      "tests/utils
+0000f4d0: 2f66 696c 6573 2f72 6570 6f72 745f 636f  /files/report_co
+0000f4e0: 6c75 6d6e 735f 7665 702e 7961 6d6c 2229  lumns_vep.yaml")
+0000f4f0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+0000f500: 656e 2872 6570 6f72 742c 2027 7227 2920  en(report, 'r') 
+0000f510: 6173 2072 6570 6f72 745f 7265 7375 6c74  as report_result
+0000f520: 3a0a 2020 2020 2020 2020 2020 2020 6865  :.            he
+0000f530: 6164 203d 2072 6570 6f72 745f 7265 7375  ad = report_resu
+0000f540: 6c74 2e72 6561 646c 696e 6528 290a 2020  lt.readline().  
+0000f550: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000f560: 7373 6572 7445 7175 616c 2868 6561 642e  ssertEqual(head.
+0000f570: 7273 7472 6970 2829 2c20 225c 7422 2e6a  rstrip(), "\t".j
+0000f580: 6f69 6e28 5b22 7361 6d70 6c65 222c 2022  oin(["sample", "
+0000f590: 6368 7222 2c20 2273 7461 7274 222c 2022  chr", "start", "
+0000f5a0: 7374 6f70 222c 2022 7265 6622 2c20 2261  stop", "ref", "a
+0000f5b0: 6c74 222c 2022 7265 706f 7274 222c 2027  lt", "report", '
+0000f5c0: 6776 6366 5f64 6570 7468 272c 2022 7265  gvcf_depth', "re
+0000f5d0: 665f 6465 7074 6822 2c20 2261 6c74 5f64  f_depth", "alt_d
+0000f5e0: 6570 7468 222c 2027 416e 616c 797a 6162  epth", 'Analyzab
+0000f5f0: 6c65 272c 2027 4d69 6e5f 7265 6164 5f64  le', 'Min_read_d
+0000f600: 6570 7468 3330 3027 2c20 2747 656e 6527  epth300', 'Gene'
+0000f610: 2c20 2756 6172 6961 6e74 5f74 7970 6527  , 'Variant_type'
+0000f620: 2c20 2743 6f6e 7365 7175 656e 6365 272c  , 'Consequence',
+0000f630: 2027 4361 6c6c 6572 7327 2c20 2743 6f6d   'Callers', 'Com
+0000f640: 6d65 6e74 275d 2929 2020 2320 6e6f 7161  ment']))  # noqa
+0000f650: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000f660: 756c 7420 3d20 7265 706f 7274 5f72 6573  ult = report_res
+0000f670: 756c 742e 7265 6164 6c69 6e65 7328 290a  ult.readlines().
+0000f680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f690: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+0000f6a0: 2872 6573 756c 7429 2c20 3335 290a 2020  (result), 35).  
+0000f6b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000f6c0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+0000f6d0: 745b 305d 2e72 7374 7269 7028 292c 2022  t[0].rstrip(), "
+0000f6e0: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0000f6f0: 322e 3131 0932 3934 3435 3237 3109 3239  2.11.29445271.29
+0000f700: 3434 3532 3731 0947 0941 0931 2d68 6f74  445271.G.A.1-hot
+0000f710: 7370 6f74 0936 3230 0933 3539 0934 0979  spot.620.359.4.y
+0000f720: 6573 096f 6b09 414c 4b09 7072 6f74 6569  es.ok.ALK.protei
+0000f730: 6e5f 636f 6469 6e67 0973 796e 6f6e 796d  n_coding.synonym
+0000f740: 6f75 735f 7661 7269 616e 7409 7661 7264  ous_variant.vard
+0000f750: 6963 7409 7265 7369 7374 616e 6365 5f6d  ict.resistance_m
+0000f760: 7574 6174 696f 6e22 2920 2023 206e 6f71  utation")  # noq
+0000f770: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+0000f780: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+0000f790: 6573 756c 745b 315d 2e72 7374 7269 7028  esult[1].rstrip(
+0000f7a0: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+0000f7b0: 3030 3030 372e 3133 0931 3430 3439 3833  00007.13.1404983
+0000f7c0: 3539 0931 3430 3439 3833 3632 0943 5454  59.140498362.CTT
+0000f7d0: 5409 4309 322d 696e 6465 6c09 3130 302e  T.C.2-indel.100.
+0000f7e0: 3509 3237 0934 0979 6573 096c 6f77 0942  5.27.4.yes.low.B
+0000f7f0: 5241 4609 7072 6f74 6569 6e5f 636f 6469  RAF.protein_codi
+0000f800: 6e67 0969 6e74 726f 6e5f 7661 7269 616e  ng.intron_varian
+0000f810: 7409 6d75 7465 6374 3209 2d22 2920 2023  t.mutect2.-")  #
+0000f820: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+0000f830: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000f840: 616c 2872 6573 756c 745b 325d 2e72 7374  al(result[2].rst
+0000f850: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0000f860: 4e43 5f30 3030 3030 372e 3133 0931 3430  NC_000007.13.140
+0000f870: 3439 3833 3631 0931 3430 3439 3833 3631  498361.140498361
+0000f880: 092d 092d 0931 2d68 6f74 7370 6f74 0931  .-.-.1-hotspot.1
+0000f890: 3130 092d 092d 0979 6573 096c 6f77 092d  10.-.-.yes.low.-
+0000f8a0: 092d 092d 092d 092d 2229 2020 2023 206e  .-.-.-.-")   # n
+0000f8b0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+0000f8c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000f8d0: 2872 6573 756c 745b 335d 2e72 7374 7269  (result[3].rstri
+0000f8e0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0000f8f0: 5f30 3030 3030 372e 3133 0931 3430 3435  _000007.13.14045
+0000f900: 3331 3336 0931 3430 3435 3331 3336 092d  3136.140453136.-
+0000f910: 092d 0931 2d68 6f74 7370 6f74 0930 092d  .-.1-hotspot.0.-
+0000f920: 092d 096e 6f74 2061 6e61 6c79 7a61 626c  .-.not analyzabl
+0000f930: 6509 6c6f 7709 2d09 2d09 2d09 2d09 2d22  e.low.-.-.-.-.-"
+0000f940: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+0000f950: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000f960: 7445 7175 616c 2872 6573 756c 745b 345d  tEqual(result[4]
+0000f970: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+0000f980: 6c65 3109 4e43 5f30 3030 3030 372e 3133  le1.NC_000007.13
+0000f990: 0931 3136 3431 3230 3433 0931 3136 3431  .116412043.11641
+0000f9a0: 3230 3433 092d 092d 0931 2d68 6f74 7370  2043.-.-.1-hotsp
+0000f9b0: 6f74 0930 092d 092d 096e 6f74 2061 6e61  ot.0.-.-.not ana
+0000f9c0: 6c79 7a61 626c 6509 6c6f 7709 2d09 2d09  lyzable.low.-.-.
+0000f9d0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+0000f9e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f9f0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000fa00: 756c 745b 355d 2e72 7374 7269 7028 292c  ult[5].rstrip(),
+0000fa10: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0000fa20: 3030 322e 3131 0932 3934 3435 3237 3109  002.11.29445271.
+0000fa30: 3239 3434 3532 3731 092d 092d 0933 2d63  29445271.-.-.3-c
+0000fa40: 6865 636b 0936 3230 092d 092d 0979 6573  heck.620.-.-.yes
+0000fa50: 096f 6b09 2d09 2d09 2d09 2d09 2d22 2920  .ok.-.-.-.-.-") 
+0000fa60: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+0000fa70: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000fa80: 7175 616c 2872 6573 756c 745b 365d 2e72  qual(result[6].r
+0000fa90: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0000faa0: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
+0000fab0: 3934 3435 3237 3209 3239 3434 3532 3732  9445272.29445272
+0000fac0: 092d 092d 0933 2d63 6865 636b 0932 3231  .-.-.3-check.221
+0000fad0: 092d 092d 0979 6573 096c 6f77 092d 092d  .-.-.yes.low.-.-
+0000fae0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+0000faf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fb00: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+0000fb10: 7375 6c74 5b37 5d2e 7273 7472 6970 2829  sult[7].rstrip()
+0000fb20: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0000fb30: 3030 3032 2e31 3109 3239 3434 3532 3733  0002.11.29445273
+0000fb40: 0932 3934 3435 3237 3309 2d09 2d09 332d  .29445273.-.-.3-
+0000fb50: 6368 6563 6b09 3632 3809 2d09 2d09 7965  check.628.-.-.ye
+0000fb60: 7309 6f6b 092d 092d 092d 092d 092d 2229  s.ok.-.-.-.-.-")
+0000fb70: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+0000fb80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000fb90: 4571 7561 6c28 7265 7375 6c74 5b38 5d2e  Equal(result[8].
+0000fba0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+0000fbb0: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
+0000fbc0: 3239 3434 3532 3734 0932 3934 3435 3237  29445274.2944527
+0000fbd0: 3409 2d09 2d09 332d 6368 6563 6b09 3631  4.-.-.3-check.61
+0000fbe0: 3809 2d09 2d09 7965 7309 6f6b 092d 092d  8.-.-.yes.ok.-.-
+0000fbf0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+0000fc00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fc10: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+0000fc20: 7375 6c74 5b39 5d2e 7273 7472 6970 2829  sult[9].rstrip()
+0000fc30: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0000fc40: 3030 3032 2e31 3109 3239 3434 3532 3735  0002.11.29445275
+0000fc50: 0932 3934 3435 3237 3509 2d09 2d09 332d  .29445275.-.-.3-
+0000fc60: 6368 6563 6b09 3630 3809 2d09 2d09 7965  check.608.-.-.ye
+0000fc70: 7309 6f6b 092d 092d 092d 092d 092d 2229  s.ok.-.-.-.-.-")
+0000fc80: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+0000fc90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000fca0: 4571 7561 6c28 7265 7375 6c74 5b31 305d  Equal(result[10]
+0000fcb0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+0000fcc0: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
+0000fcd0: 0932 3934 3435 3237 3609 3239 3434 3532  .29445276.294452
+0000fce0: 3736 092d 092d 0933 2d63 6865 636b 0936  76.-.-.3-check.6
+0000fcf0: 3231 092d 092d 0979 6573 096f 6b09 2d09  21.-.-.yes.ok.-.
+0000fd00: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+0000fd10: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+0000fd20: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+0000fd30: 6573 756c 745b 3131 5d2e 7273 7472 6970  esult[11].rstrip
+0000fd40: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+0000fd50: 3030 3030 3032 2e31 3109 3239 3434 3532  000002.11.294452
+0000fd60: 3737 0932 3934 3435 3237 3709 2d09 2d09  77.29445277.-.-.
+0000fd70: 332d 6368 6563 6b09 3138 3209 2d09 2d09  3-check.182.-.-.
+0000fd80: 7965 7309 6c6f 7709 2d09 2d09 2d09 2d09  yes.low.-.-.-.-.
+0000fd90: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+0000fda0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000fdb0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0000fdc0: 3132 5d2e 7273 7472 6970 2829 2c20 2273  12].rstrip(), "s
+0000fdd0: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
+0000fde0: 2e31 3109 3239 3434 3532 3738 0932 3934  .11.29445278.294
+0000fdf0: 3435 3237 3809 2d09 2d09 332d 6368 6563  45278.-.-.3-chec
+0000fe00: 6b09 3535 3009 2d09 2d09 7965 7309 6f6b  k.550.-.-.yes.ok
+0000fe10: 092d 092d 092d 092d 092d 2229 2020 2320  .-.-.-.-.-")  # 
+0000fe20: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+0000fe30: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000fe40: 6c28 7265 7375 6c74 5b31 335d 2e72 7374  l(result[13].rst
+0000fe50: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0000fe60: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+0000fe70: 3435 3237 3909 3239 3434 3532 3739 092d  45279.29445279.-
+0000fe80: 092d 0933 2d63 6865 636b 0935 3934 092d  .-.3-check.594.-
+0000fe90: 092d 0979 6573 096f 6b09 2d09 2d09 2d09  .-.yes.ok.-.-.-.
+0000fea0: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+0000feb0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fec0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+0000fed0: 745b 3134 5d2e 7273 7472 6970 2829 2c20  t[14].rstrip(), 
+0000fee0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+0000fef0: 3032 2e31 3109 3239 3434 3532 3830 0932  02.11.29445280.2
+0000ff00: 3934 3435 3238 3009 2d09 2d09 332d 6368  9445280.-.-.3-ch
+0000ff10: 6563 6b09 3533 3909 2d09 2d09 7965 7309  eck.539.-.-.yes.
+0000ff20: 6f6b 092d 092d 092d 092d 092d 2229 2020  ok.-.-.-.-.-")  
+0000ff30: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+0000ff40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000ff50: 7561 6c28 7265 7375 6c74 5b31 355d 2e72  ual(result[15].r
+0000ff60: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0000ff70: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
+0000ff80: 3934 3435 3238 3109 3239 3434 3532 3831  9445281.29445281
+0000ff90: 092d 092d 0933 2d63 6865 636b 0935 3236  .-.-.3-check.526
+0000ffa0: 092d 092d 0979 6573 096f 6b09 2d09 2d09  .-.-.yes.ok.-.-.
+0000ffb0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+0000ffc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ffd0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0000ffe0: 756c 745b 3136 5d2e 7273 7472 6970 2829  ult[16].rstrip()
+0000fff0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00010000: 3030 3038 2e31 3109 3134 3537 3338 3736  0008.11.14573876
+00010010: 3509 3134 3537 3338 3736 3509 2d09 2d09  5.145738765.-.-.
+00010020: 332d 6368 6563 6b09 3136 3136 092d 092d  3-check.1616.-.-
+00010030: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00010040: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+00010050: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00010060: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00010070: 3137 5d2e 7273 7472 6970 2829 2c20 2273  17].rstrip(), "s
+00010080: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+00010090: 2e31 3109 3134 3537 3338 3736 3609 3134  .11.145738766.14
+000100a0: 3537 3338 3736 3609 2d09 2d09 332d 6368  5738766.-.-.3-ch
+000100b0: 6563 6b09 3136 3139 092d 092d 0979 6573  eck.1619.-.-.yes
+000100c0: 096f 6b09 2d09 2d09 2d09 2d09 2d22 2920  .ok.-.-.-.-.-") 
+000100d0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+000100e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000100f0: 7175 616c 2872 6573 756c 745b 3138 5d2e  qual(result[18].
+00010100: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00010110: 6531 094e 435f 3030 3030 3038 2e31 3109  e1.NC_000008.11.
+00010120: 3134 3537 3338 3736 3709 3134 3537 3338  145738767.145738
+00010130: 3736 3709 2d09 2d09 332d 6368 6563 6b09  767.-.-.3-check.
+00010140: 3135 3935 092d 092d 0979 6573 096f 6b09  1595.-.-.yes.ok.
+00010150: 2d09 2d09 2d09 2d09 2d22 2920 2023 206e  -.-.-.-.-")  # n
+00010160: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00010170: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00010180: 2872 6573 756c 745b 3139 5d2e 7273 7472  (result[19].rstr
+00010190: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+000101a0: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
+000101b0: 3338 3736 3809 3134 3537 3338 3736 3809  38768.145738768.
+000101c0: 4709 4309 332d 6368 6563 6b09 3135 3437  G.C.3-check.1547
+000101d0: 0935 0932 3709 7965 7309 6f6b 094c 5252  .5.27.yes.ok.LRR
+000101e0: 4331 3409 7072 6f74 6569 6e5f 636f 6469  C14.protein_codi
+000101f0: 6e67 0975 7073 7472 6561 6d5f 6765 6e65  ng.upstream_gene
+00010200: 5f76 6172 6961 6e74 0976 6172 6469 6374  _variant.vardict
+00010210: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00010220: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00010230: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00010240: 5b32 305d 2e72 7374 7269 7028 292c 2022  [20].rstrip(), "
+00010250: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00010260: 382e 3131 0931 3435 3733 3837 3639 0931  8.11.145738769.1
+00010270: 3435 3733 3837 3639 092d 092d 0933 2d63  45738769.-.-.3-c
+00010280: 6865 636b 0931 3634 3409 2d09 2d09 7965  heck.1644.-.-.ye
+00010290: 7309 6f6b 092d 092d 092d 092d 092d 2229  s.ok.-.-.-.-.-")
+000102a0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000102b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000102c0: 4571 7561 6c28 7265 7375 6c74 5b32 315d  Equal(result[21]
+000102d0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+000102e0: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+000102f0: 0931 3435 3733 3837 3730 0931 3435 3733  .145738770.14573
+00010300: 3837 3730 092d 092d 0933 2d63 6865 636b  8770.-.-.3-check
+00010310: 0931 3636 3709 2d09 2d09 7965 7309 6f6b  .1667.-.-.yes.ok
+00010320: 092d 092d 092d 092d 092d 2229 2020 2320  .-.-.-.-.-")  # 
+00010330: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00010340: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00010350: 6c28 7265 7375 6c74 5b32 325d 2e72 7374  l(result[22].rst
+00010360: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00010370: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+00010380: 3733 3837 3731 0931 3435 3733 3837 3731  738771.145738771
+00010390: 092d 092d 0933 2d63 6865 636b 0931 3638  .-.-.3-check.168
+000103a0: 3509 2d09 2d09 7965 7309 6f6b 092d 092d  5.-.-.yes.ok.-.-
+000103b0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+000103c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000103d0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+000103e0: 7375 6c74 5b32 335d 2e72 7374 7269 7028  sult[23].rstrip(
+000103f0: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+00010400: 3030 3030 382e 3131 0931 3435 3733 3837  00008.11.1457387
+00010410: 3732 0931 3435 3733 3837 3732 092d 092d  72.145738772.-.-
+00010420: 0933 2d63 6865 636b 0931 3638 3909 2d09  .3-check.1689.-.
+00010430: 2d09 7965 7309 6f6b 092d 092d 092d 092d  -.yes.ok.-.-.-.-
+00010440: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00010450: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00010460: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00010470: 5b32 345d 2e72 7374 7269 7028 292c 2022  [24].rstrip(), "
+00010480: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00010490: 382e 3131 0931 3435 3733 3837 3733 0931  8.11.145738773.1
+000104a0: 3435 3733 3837 3733 092d 092d 0933 2d63  45738773.-.-.3-c
+000104b0: 6865 636b 0931 3934 3009 2d09 2d09 7965  heck.1940.-.-.ye
+000104c0: 7309 6f6b 092d 092d 092d 092d 092d 2229  s.ok.-.-.-.-.-")
+000104d0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000104e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000104f0: 4571 7561 6c28 7265 7375 6c74 5b32 355d  Equal(result[25]
+00010500: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00010510: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00010520: 0931 3435 3733 3837 3734 0931 3435 3733  .145738774.14573
+00010530: 3837 3734 092d 092d 0933 2d63 6865 636b  8774.-.-.3-check
+00010540: 0931 3934 3009 2d09 2d09 7965 7309 6f6b  .1940.-.-.yes.ok
+00010550: 092d 092d 092d 092d 092d 2229 2020 2320  .-.-.-.-.-")  # 
+00010560: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00010570: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00010580: 6c28 7265 7375 6c74 5b32 365d 2e72 7374  l(result[26].rst
+00010590: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+000105a0: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+000105b0: 3733 3837 3735 0931 3435 3733 3837 3735  738775.145738775
+000105c0: 092d 092d 0933 2d63 6865 636b 0931 3936  .-.-.3-check.196
+000105d0: 3309 2d09 2d09 7965 7309 6f6b 092d 092d  3.-.-.yes.ok.-.-
+000105e0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+000105f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010600: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00010610: 7375 6c74 5b32 375d 2e72 7374 7269 7028  sult[27].rstrip(
+00010620: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+00010630: 3030 3030 382e 3131 0931 3435 3733 3837  00008.11.1457387
+00010640: 3736 0931 3435 3733 3837 3736 092d 092d  76.145738776.-.-
+00010650: 0933 2d63 6865 636b 0930 092d 092d 096e  .3-check.0.-.-.n
+00010660: 6f74 2061 6e61 6c79 7a61 626c 6509 6c6f  ot analyzable.lo
+00010670: 7709 2d09 2d09 2d09 2d09 2d22 2920 2023  w.-.-.-.-.-")  #
+00010680: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00010690: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000106a0: 616c 2872 6573 756c 745b 3238 5d2e 7273  al(result[28].rs
+000106b0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+000106c0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+000106d0: 3537 3338 3737 3709 3134 3537 3338 3737  5738777.14573877
+000106e0: 3709 2d09 2d09 332d 6368 6563 6b09 3139  7.-.-.3-check.19
+000106f0: 3634 092d 092d 0979 6573 096f 6b09 2d09  64.-.-.yes.ok.-.
+00010700: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00010710: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00010720: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00010730: 6573 756c 745b 3239 5d2e 7273 7472 6970  esult[29].rstrip
+00010740: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00010750: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
+00010760: 3737 3809 3134 3537 3338 3737 3809 2d09  778.145738778.-.
+00010770: 2d09 332d 6368 6563 6b09 3139 3633 092d  -.3-check.1963.-
+00010780: 092d 0979 6573 096f 6b09 2d09 2d09 2d09  .-.yes.ok.-.-.-.
+00010790: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+000107a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000107b0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+000107c0: 745b 3330 5d2e 7273 7472 6970 2829 2c20  t[30].rstrip(), 
+000107d0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+000107e0: 3038 2e31 3109 3134 3537 3338 3737 3909  08.11.145738779.
+000107f0: 3134 3537 3338 3737 3909 2d09 2d09 332d  145738779.-.-.3-
+00010800: 6368 6563 6b09 3139 3538 092d 092d 0979  check.1958.-.-.y
+00010810: 6573 096f 6b09 2d09 2d09 2d09 2d09 2d22  es.ok.-.-.-.-.-"
+00010820: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00010830: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00010840: 7445 7175 616c 2872 6573 756c 745b 3331  tEqual(result[31
+00010850: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00010860: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+00010870: 3109 3134 3537 3432 3531 3409 3134 3537  1.145742514.1457
+00010880: 3432 3531 3409 4109 4709 332d 6368 6563  42514.A.G.3-chec
+00010890: 6b09 3009 3009 3833 3909 6e6f 7420 616e  k.0.0.839.not an
+000108a0: 616c 797a 6162 6c65 096c 6f77 0952 4543  alyzable.low.REC
+000108b0: 514c 3409 7072 6f74 6569 6e5f 636f 6469  QL4.protein_codi
+000108c0: 6e67 0973 796e 6f6e 796d 6f75 735f 7661  ng.synonymous_va
+000108d0: 7269 616e 7409 7661 7264 6963 742c 6d75  riant.vardict,mu
+000108e0: 7465 6374 3209 2d22 2920 2023 206e 6f71  tect2.-")  # noq
+000108f0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00010900: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00010910: 6573 756c 745b 3332 5d2e 7273 7472 6970  esult[32].rstrip
+00010920: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00010930: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
+00010940: 3839 0938 3139 3534 3738 3909 4309 4754  89.81954789.C.GT
+00010950: 0932 2d69 6e64 656c 0931 3134 3409 3131  .2-indel.1144.11
+00010960: 3732 0932 3909 7965 7309 6f6b 0950 4c43  72.29.yes.ok.PLC
+00010970: 4732 0970 726f 7465 696e 5f63 6f64 696e  G2.protein_codin
+00010980: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
+00010990: 0976 6172 6469 6374 092d 2229 2020 2320  .vardict.-")  # 
+000109a0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+000109b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000109c0: 6c28 7265 7375 6c74 5b33 335d 2e72 7374  l(result[33].rst
+000109d0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+000109e0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+000109f0: 3435 3238 3209 3239 3434 3532 3832 0947  45282.29445282.G
+00010a00: 0941 0934 2d6f 7468 6572 0935 3230 0932  .A.4-other.520.2
+00010a10: 3834 0933 0979 6573 096f 6b09 414c 4b09  84.3.yes.ok.ALK.
+00010a20: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
+00010a30: 706c 6963 655f 7265 6769 6f6e 5f76 6172  plice_region_var
+00010a40: 6961 6e74 2669 6e74 726f 6e5f 7661 7269  iant&intron_vari
+00010a50: 616e 7409 7661 7264 6963 7409 2d22 2920  ant.vardict.-") 
+00010a60: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00010a70: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00010a80: 7175 616c 2872 6573 756c 745b 3334 5d2e  qual(result[34].
+00010a90: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00010aa0: 6531 094e 435f 3030 3030 3136 2e31 3109  e1.NC_000016.11.
+00010ab0: 3831 3935 3437 3839 0938 3139 3534 3738  81954789.8195478
+00010ac0: 3909 4309 4709 342d 6f74 6865 7209 3131  9.C.G.4-other.11
+00010ad0: 3434 0934 3432 0933 3439 0979 6573 096f  44.442.349.yes.o
+00010ae0: 6b09 5345 5054 0970 726f 7465 696e 5f63  k.SEPT.protein_c
+00010af0: 6f64 696e 6709 696e 7472 6f6e 5f76 6172  oding.intron_var
+00010b00: 6961 6e74 0976 6172 6469 6374 2c6d 7574  iant.vardict,mut
+00010b10: 6563 7432 092d 2229 2020 2320 6e6f 7161  ect2.-")  # noqa
+00010b20: 0a0a 2020 2020 6465 6620 7465 7374 5f66  ..    def test_f
+00010b30: 696c 7465 7265 645f 6d75 7461 7469 6f6e  iltered_mutation
+00010b40: 5f63 6861 6e67 655f 6f75 7470 7574 5f6f  _change_output_o
+00010b50: 7264 6572 2873 656c 6629 3a0a 2020 2020  rder(self):.    
+00010b60: 2020 2020 6672 6f6d 2068 7964 7261 5f67      from hydra_g
+00010b70: 656e 6574 6963 732e 7574 696c 732e 696f  enetics.utils.io
+00010b80: 2e68 6f74 7370 6f74 5f72 6570 6f72 7420  .hotspot_report 
+00010b90: 696d 706f 7274 2067 656e 6572 6174 655f  import generate_
+00010ba0: 686f 7473 706f 745f 7265 706f 7274 0a20  hotspot_report. 
+00010bb0: 2020 2020 2020 206c 6576 656c 7320 3d20         levels = 
+00010bc0: 5b28 3330 302c 2022 6f6b 222c 2022 7965  [(300, "ok", "ye
+00010bd0: 7322 292c 2028 3330 2c20 226c 6f77 222c  s"), (30, "low",
+00010be0: 2022 7965 7322 292c 2028 302c 2022 6c6f   "yes"), (0, "lo
+00010bf0: 7722 2c20 226e 6f74 2061 6e61 6c79 7a61  w", "not analyza
+00010c00: 626c 6522 295d 0a20 2020 2020 2020 2073  ble")].        s
+00010c10: 656c 662e 6d61 7844 6966 6620 3d20 3130  elf.maxDiff = 10
+00010c20: 3030 300a 0a20 2020 2020 2020 2072 6570  000..        rep
+00010c30: 6f72 7420 3d20 6f73 2e70 6174 682e 6a6f  ort = os.path.jo
+00010c40: 696e 2873 656c 662e 7465 6d70 6469 722c  in(self.tempdir,
+00010c50: 2022 6669 6c74 6572 6564 2e72 6570 6f72   "filtered.repor
+00010c60: 7422 290a 2020 2020 2020 2020 6765 6e65  t").        gene
+00010c70: 7261 7465 5f68 6f74 7370 6f74 5f72 6570  rate_hotspot_rep
+00010c80: 6f72 7428 2273 616d 706c 6531 222c 0a20  ort("sample1",. 
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010cb0: 6570 6f72 742c 0a20 2020 2020 2020 2020  eport,.         
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 2020 2020 2020 206c 6576 656c 732c 0a20         levels,. 
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010d00: 656c 662e 686f 7473 706f 742c 0a20 2020  elf.hotspot,.   
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010d30: 662e 7663 665f 7665 7020 2b20 222e 677a  f.vcf_vep + ".gz
+00010d40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 2020 2073 656c 662e 6776 6366 202b 2022     self.gvcf + "
+00010d70: 2e67 7a22 2c0a 2020 2020 2020 2020 2020  .gz",.          
+00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d90: 2020 2020 2020 7365 6c66 2e72 6566 6572        self.refer
+00010da0: 656e 6365 2c0a 2020 2020 2020 2020 2020  ence,.          
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010dc0: 2020 2020 2020 7365 6c66 2e76 6366 5f76        self.vcf_v
+00010dd0: 6570 5f77 6f5f 7069 636b 202b 2022 2e67  ep_wo_pick + ".g
+00010de0: 7a22 2c0a 2020 2020 2020 2020 2020 2020  z",.            
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2274 6573 7473 2f75 7469 6c73      "tests/utils
+00010e10: 2f66 696c 6573 2f72 6570 6f72 745f 636f  /files/report_co
+00010e20: 6c75 6d6e 735f 7665 705f 6f72 6465 725f  lumns_vep_order_
+00010e30: 6f75 7470 7574 2e79 616d 6c22 290a 2020  output.yaml").  
+00010e40: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00010e50: 7265 706f 7274 2c20 2772 2729 2061 7320  report, 'r') as 
+00010e60: 7265 706f 7274 5f72 6573 756c 743a 0a20  report_result:. 
+00010e70: 2020 2020 2020 2020 2020 2068 6561 6420             head 
+00010e80: 3d20 7265 706f 7274 5f72 6573 756c 742e  = report_result.
+00010e90: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
+00010ea0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010eb0: 7274 4571 7561 6c28 6865 6164 2e72 7374  rtEqual(head.rst
+00010ec0: 7269 7028 292c 2022 5c74 222e 6a6f 696e  rip(), "\t".join
+00010ed0: 285b 2273 746f 7022 2c20 2273 7461 7274  (["stop", "start
+00010ee0: 222c 2022 6368 7222 2c20 2747 656e 6527  ", "chr", 'Gene'
+00010ef0: 2c20 2273 616d 706c 6522 2c20 2772 6566  , "sample", 'ref
+00010f00: 272c 2027 616c 7427 2c20 2272 6570 6f72  ', 'alt', "repor
+00010f10: 7422 2c20 2767 7663 665f 6465 7074 6827  t", 'gvcf_depth'
+00010f20: 2c20 2772 6566 5f64 6570 7468 272c 2027  , 'ref_depth', '
+00010f30: 616c 745f 6465 7074 6827 2c20 2741 6e61  alt_depth', 'Ana
+00010f40: 6c79 7a61 626c 6527 2c20 274d 696e 5f72  lyzable', 'Min_r
+00010f50: 6561 645f 6465 7074 6833 3030 272c 2027  ead_depth300', '
+00010f60: 5661 7269 616e 745f 7479 7065 272c 2027  Variant_type', '
+00010f70: 436f 6e73 6571 7565 6e63 6527 2c20 2743  Consequence', 'C
+00010f80: 616c 6c65 7273 272c 2027 436f 6d6d 656e  allers', 'Commen
+00010f90: 7427 5d29 2920 2023 206e 6f71 610a 2020  t']))  # noqa.  
+00010fa0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00010fb0: 203d 2072 6570 6f72 745f 7265 7375 6c74   = report_result
+00010fc0: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+00010fd0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00010fe0: 7365 7274 4571 7561 6c28 6c65 6e28 7265  sertEqual(len(re
+00010ff0: 7375 6c74 292c 2033 3529 0a20 2020 2020  sult), 35).     
+00011000: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011010: 7274 4571 7561 6c28 7265 7375 6c74 5b30  rtEqual(result[0
+00011020: 5d2e 7273 7472 6970 2829 2c20 2232 3934  ].rstrip(), "294
+00011030: 3435 3237 3109 3239 3434 3532 3731 094e  45271.29445271.N
+00011040: 435f 3030 3030 3032 2e31 3109 414c 4b09  C_000002.11.ALK.
+00011050: 7361 6d70 6c65 3109 4709 4109 312d 686f  sample1.G.A.1-ho
+00011060: 7473 706f 7409 3632 3009 3335 3909 3409  tspot.620.359.4.
+00011070: 7965 7309 6f6b 0970 726f 7465 696e 5f63  yes.ok.protein_c
+00011080: 6f64 696e 6709 7379 6e6f 6e79 6d6f 7573  oding.synonymous
+00011090: 5f76 6172 6961 6e74 0976 6172 6469 6374  _variant.vardict
+000110a0: 0972 6573 6973 7461 6e63 655f 6d75 7461  .resistance_muta
+000110b0: 7469 6f6e 2229 2020 2320 6e6f 7161 0a20  tion")  # noqa. 
+000110c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000110d0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+000110e0: 6c74 5b31 5d2e 7273 7472 6970 2829 2c20  lt[1].rstrip(), 
+000110f0: 2231 3430 3439 3833 3632 0931 3430 3439  "140498362.14049
+00011100: 3833 3539 094e 435f 3030 3030 3037 2e31  8359.NC_000007.1
+00011110: 3309 4252 4146 0973 616d 706c 6531 0943  3.BRAF.sample1.C
+00011120: 5454 5409 4309 322d 696e 6465 6c09 3130  TTT.C.2-indel.10
+00011130: 302e 3509 3237 0934 0979 6573 096c 6f77  0.5.27.4.yes.low
+00011140: 0970 726f 7465 696e 5f63 6f64 696e 6709  .protein_coding.
+00011150: 696e 7472 6f6e 5f76 6172 6961 6e74 096d  intron_variant.m
+00011160: 7574 6563 7432 092d 2229 2020 2320 6e6f  utect2.-")  # no
+00011170: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00011180: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00011190: 7265 7375 6c74 5b32 5d2e 7273 7472 6970  result[2].rstrip
+000111a0: 2829 2c20 2231 3430 3439 3833 3631 0931  (), "140498361.1
+000111b0: 3430 3439 3833 3631 094e 435f 3030 3030  40498361.NC_0000
+000111c0: 3037 2e31 3309 2d09 7361 6d70 6c65 3109  07.13.-.sample1.
+000111d0: 2d09 2d09 312d 686f 7473 706f 7409 3131  -.-.1-hotspot.11
+000111e0: 3009 2d09 2d09 7965 7309 6c6f 7709 2d09  0.-.-.yes.low.-.
+000111f0: 2d09 2d09 2d22 2920 2020 2320 6e6f 7161  -.-.-")   # noqa
+00011200: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011210: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00011220: 7375 6c74 5b33 5d2e 7273 7472 6970 2829  sult[3].rstrip()
+00011230: 2c20 2231 3430 3435 3331 3336 0931 3430  , "140453136.140
+00011240: 3435 3331 3336 094e 435f 3030 3030 3037  453136.NC_000007
+00011250: 2e31 3309 2d09 7361 6d70 6c65 3109 2d09  .13.-.sample1.-.
+00011260: 2d09 312d 686f 7473 706f 7409 3009 2d09  -.1-hotspot.0.-.
+00011270: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
+00011280: 096c 6f77 092d 092d 092d 092d 2229 2020  .low.-.-.-.-")  
+00011290: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+000112a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000112b0: 7561 6c28 7265 7375 6c74 5b34 5d2e 7273  ual(result[4].rs
+000112c0: 7472 6970 2829 2c20 2231 3136 3431 3230  trip(), "1164120
+000112d0: 3433 0931 3136 3431 3230 3433 094e 435f  43.116412043.NC_
+000112e0: 3030 3030 3037 2e31 3309 2d09 7361 6d70  000007.13.-.samp
+000112f0: 6c65 3109 2d09 2d09 312d 686f 7473 706f  le1.-.-.1-hotspo
+00011300: 7409 3009 2d09 2d09 6e6f 7420 616e 616c  t.0.-.-.not anal
+00011310: 797a 6162 6c65 096c 6f77 092d 092d 092d  yzable.low.-.-.-
+00011320: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00011330: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011340: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00011350: 5b35 5d2e 7273 7472 6970 2829 2c20 2232  [5].rstrip(), "2
+00011360: 3934 3435 3237 3109 3239 3434 3532 3731  9445271.29445271
+00011370: 094e 435f 3030 3030 3032 2e31 3109 2d09  .NC_000002.11.-.
+00011380: 7361 6d70 6c65 3109 2d09 2d09 332d 6368  sample1.-.-.3-ch
+00011390: 6563 6b09 3632 3009 2d09 2d09 7965 7309  eck.620.-.-.yes.
+000113a0: 6f6b 092d 092d 092d 092d 2229 2020 2320  ok.-.-.-.-")  # 
+000113b0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+000113c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000113d0: 6c28 7265 7375 6c74 5b36 5d2e 7273 7472  l(result[6].rstr
+000113e0: 6970 2829 2c20 2232 3934 3435 3237 3209  ip(), "29445272.
+000113f0: 3239 3434 3532 3732 094e 435f 3030 3030  29445272.NC_0000
+00011400: 3032 2e31 3109 2d09 7361 6d70 6c65 3109  02.11.-.sample1.
+00011410: 2d09 2d09 332d 6368 6563 6b09 3232 3109  -.-.3-check.221.
+00011420: 2d09 2d09 7965 7309 6c6f 7709 2d09 2d09  -.-.yes.low.-.-.
+00011430: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00011440: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011450: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00011460: 745b 375d 2e72 7374 7269 7028 292c 2022  t[7].rstrip(), "
+00011470: 3239 3434 3532 3733 0932 3934 3435 3237  29445273.2944527
+00011480: 3309 4e43 5f30 3030 3030 322e 3131 092d  3.NC_000002.11.-
+00011490: 0973 616d 706c 6531 092d 092d 0933 2d63  .sample1.-.-.3-c
+000114a0: 6865 636b 0936 3238 092d 092d 0979 6573  heck.628.-.-.yes
+000114b0: 096f 6b09 2d09 2d09 2d09 2d22 2920 2023  .ok.-.-.-.-")  #
+000114c0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+000114d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000114e0: 616c 2872 6573 756c 745b 385d 2e72 7374  al(result[8].rst
+000114f0: 7269 7028 292c 2022 3239 3434 3532 3734  rip(), "29445274
+00011500: 0932 3934 3435 3237 3409 4e43 5f30 3030  .29445274.NC_000
+00011510: 3030 322e 3131 092d 0973 616d 706c 6531  002.11.-.sample1
+00011520: 092d 092d 0933 2d63 6865 636b 0936 3138  .-.-.3-check.618
+00011530: 092d 092d 0979 6573 096f 6b09 2d09 2d09  .-.-.yes.ok.-.-.
+00011540: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00011550: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011560: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00011570: 745b 395d 2e72 7374 7269 7028 292c 2022  t[9].rstrip(), "
+00011580: 3239 3434 3532 3735 0932 3934 3435 3237  29445275.2944527
+00011590: 3509 4e43 5f30 3030 3030 322e 3131 092d  5.NC_000002.11.-
+000115a0: 0973 616d 706c 6531 092d 092d 0933 2d63  .sample1.-.-.3-c
+000115b0: 6865 636b 0936 3038 092d 092d 0979 6573  heck.608.-.-.yes
+000115c0: 096f 6b09 2d09 2d09 2d09 2d22 2920 2023  .ok.-.-.-.-")  #
+000115d0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+000115e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000115f0: 616c 2872 6573 756c 745b 3130 5d2e 7273  al(result[10].rs
+00011600: 7472 6970 2829 2c20 2232 3934 3435 3237  trip(), "2944527
+00011610: 3609 3239 3434 3532 3736 094e 435f 3030  6.29445276.NC_00
+00011620: 3030 3032 2e31 3109 2d09 7361 6d70 6c65  0002.11.-.sample
+00011630: 3109 2d09 2d09 332d 6368 6563 6b09 3632  1.-.-.3-check.62
+00011640: 3109 2d09 2d09 7965 7309 6f6b 092d 092d  1.-.-.yes.ok.-.-
+00011650: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00011660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011670: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00011680: 6c74 5b31 315d 2e72 7374 7269 7028 292c  lt[11].rstrip(),
+00011690: 2022 3239 3434 3532 3737 0932 3934 3435   "29445277.29445
+000116a0: 3237 3709 4e43 5f30 3030 3030 322e 3131  277.NC_000002.11
+000116b0: 092d 0973 616d 706c 6531 092d 092d 0933  .-.sample1.-.-.3
+000116c0: 2d63 6865 636b 0931 3832 092d 092d 0979  -check.182.-.-.y
+000116d0: 6573 096c 6f77 092d 092d 092d 092d 2229  es.low.-.-.-.-")
+000116e0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000116f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00011700: 4571 7561 6c28 7265 7375 6c74 5b31 325d  Equal(result[12]
+00011710: 2e72 7374 7269 7028 292c 2022 3239 3434  .rstrip(), "2944
+00011720: 3532 3738 0932 3934 3435 3237 3809 4e43  5278.29445278.NC
+00011730: 5f30 3030 3030 322e 3131 092d 0973 616d  _000002.11.-.sam
+00011740: 706c 6531 092d 092d 0933 2d63 6865 636b  ple1.-.-.3-check
+00011750: 0935 3530 092d 092d 0979 6573 096f 6b09  .550.-.-.yes.ok.
+00011760: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00011770: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00011780: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00011790: 6573 756c 745b 3133 5d2e 7273 7472 6970  esult[13].rstrip
+000117a0: 2829 2c20 2232 3934 3435 3237 3909 3239  (), "29445279.29
+000117b0: 3434 3532 3739 094e 435f 3030 3030 3032  445279.NC_000002
+000117c0: 2e31 3109 2d09 7361 6d70 6c65 3109 2d09  .11.-.sample1.-.
+000117d0: 2d09 332d 6368 6563 6b09 3539 3409 2d09  -.3-check.594.-.
+000117e0: 2d09 7965 7309 6f6b 092d 092d 092d 092d  -.yes.ok.-.-.-.-
+000117f0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00011800: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011810: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
+00011820: 345d 2e72 7374 7269 7028 292c 2022 3239  4].rstrip(), "29
+00011830: 3434 3532 3830 0932 3934 3435 3238 3009  445280.29445280.
+00011840: 4e43 5f30 3030 3030 322e 3131 092d 0973  NC_000002.11.-.s
+00011850: 616d 706c 6531 092d 092d 0933 2d63 6865  ample1.-.-.3-che
+00011860: 636b 0935 3339 092d 092d 0979 6573 096f  ck.539.-.-.yes.o
+00011870: 6b09 2d09 2d09 2d09 2d22 2920 2023 206e  k.-.-.-.-")  # n
+00011880: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00011890: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000118a0: 2872 6573 756c 745b 3135 5d2e 7273 7472  (result[15].rstr
+000118b0: 6970 2829 2c20 2232 3934 3435 3238 3109  ip(), "29445281.
+000118c0: 3239 3434 3532 3831 094e 435f 3030 3030  29445281.NC_0000
+000118d0: 3032 2e31 3109 2d09 7361 6d70 6c65 3109  02.11.-.sample1.
+000118e0: 2d09 2d09 332d 6368 6563 6b09 3532 3609  -.-.3-check.526.
+000118f0: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+00011900: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00011910: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011920: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00011930: 5b31 365d 2e72 7374 7269 7028 292c 2022  [16].rstrip(), "
+00011940: 3134 3537 3338 3736 3509 3134 3537 3338  145738765.145738
+00011950: 3736 3509 4e43 5f30 3030 3030 382e 3131  765.NC_000008.11
+00011960: 092d 0973 616d 706c 6531 092d 092d 0933  .-.sample1.-.-.3
+00011970: 2d63 6865 636b 0931 3631 3609 2d09 2d09  -check.1616.-.-.
+00011980: 7965 7309 6f6b 092d 092d 092d 092d 2229  yes.ok.-.-.-.-")
+00011990: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000119a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000119b0: 4571 7561 6c28 7265 7375 6c74 5b31 375d  Equal(result[17]
+000119c0: 2e72 7374 7269 7028 292c 2022 3134 3537  .rstrip(), "1457
+000119d0: 3338 3736 3609 3134 3537 3338 3736 3609  38766.145738766.
+000119e0: 4e43 5f30 3030 3030 382e 3131 092d 0973  NC_000008.11.-.s
+000119f0: 616d 706c 6531 092d 092d 0933 2d63 6865  ample1.-.-.3-che
+00011a00: 636b 0931 3631 3909 2d09 2d09 7965 7309  ck.1619.-.-.yes.
+00011a10: 6f6b 092d 092d 092d 092d 2229 2020 2320  ok.-.-.-.-")  # 
+00011a20: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00011a30: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00011a40: 6c28 7265 7375 6c74 5b31 385d 2e72 7374  l(result[18].rst
+00011a50: 7269 7028 292c 2022 3134 3537 3338 3736  rip(), "14573876
+00011a60: 3709 3134 3537 3338 3736 3709 4e43 5f30  7.145738767.NC_0
+00011a70: 3030 3030 382e 3131 092d 0973 616d 706c  00008.11.-.sampl
+00011a80: 6531 092d 092d 0933 2d63 6865 636b 0931  e1.-.-.3-check.1
+00011a90: 3539 3509 2d09 2d09 7965 7309 6f6b 092d  595.-.-.yes.ok.-
+00011aa0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+00011ab0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011ac0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00011ad0: 7375 6c74 5b31 395d 2e72 7374 7269 7028  sult[19].rstrip(
+00011ae0: 292c 2022 3134 3537 3338 3736 3809 3134  ), "145738768.14
+00011af0: 3537 3338 3736 3809 4e43 5f30 3030 3030  5738768.NC_00000
+00011b00: 382e 3131 094c 5252 4331 3409 7361 6d70  8.11.LRRC14.samp
+00011b10: 6c65 3109 4709 4309 332d 6368 6563 6b09  le1.G.C.3-check.
+00011b20: 3135 3437 0935 0932 3709 7965 7309 6f6b  1547.5.27.yes.ok
+00011b30: 0970 726f 7465 696e 5f63 6f64 696e 6709  .protein_coding.
+00011b40: 7570 7374 7265 616d 5f67 656e 655f 7661  upstream_gene_va
+00011b50: 7269 616e 7409 7661 7264 6963 7409 2d22  riant.vardict.-"
+00011b60: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00011b70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00011b80: 7445 7175 616c 2872 6573 756c 745b 3230  tEqual(result[20
+00011b90: 5d2e 7273 7472 6970 2829 2c20 2231 3435  ].rstrip(), "145
+00011ba0: 3733 3837 3639 0931 3435 3733 3837 3639  738769.145738769
+00011bb0: 094e 435f 3030 3030 3038 2e31 3109 2d09  .NC_000008.11.-.
+00011bc0: 7361 6d70 6c65 3109 2d09 2d09 332d 6368  sample1.-.-.3-ch
+00011bd0: 6563 6b09 3136 3434 092d 092d 0979 6573  eck.1644.-.-.yes
+00011be0: 096f 6b09 2d09 2d09 2d09 2d22 2920 2023  .ok.-.-.-.-")  #
+00011bf0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00011c00: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00011c10: 616c 2872 6573 756c 745b 3231 5d2e 7273  al(result[21].rs
+00011c20: 7472 6970 2829 2c20 2231 3435 3733 3837  trip(), "1457387
+00011c30: 3730 0931 3435 3733 3837 3730 094e 435f  70.145738770.NC_
+00011c40: 3030 3030 3038 2e31 3109 2d09 7361 6d70  000008.11.-.samp
+00011c50: 6c65 3109 2d09 2d09 332d 6368 6563 6b09  le1.-.-.3-check.
+00011c60: 3136 3637 092d 092d 0979 6573 096f 6b09  1667.-.-.yes.ok.
+00011c70: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00011c80: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00011c90: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00011ca0: 6573 756c 745b 3232 5d2e 7273 7472 6970  esult[22].rstrip
+00011cb0: 2829 2c20 2231 3435 3733 3837 3731 0931  (), "145738771.1
+00011cc0: 3435 3733 3837 3731 094e 435f 3030 3030  45738771.NC_0000
+00011cd0: 3038 2e31 3109 2d09 7361 6d70 6c65 3109  08.11.-.sample1.
+00011ce0: 2d09 2d09 332d 6368 6563 6b09 3136 3835  -.-.3-check.1685
+00011cf0: 092d 092d 0979 6573 096f 6b09 2d09 2d09  .-.-.yes.ok.-.-.
+00011d00: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00011d10: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011d20: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00011d30: 745b 3233 5d2e 7273 7472 6970 2829 2c20  t[23].rstrip(), 
+00011d40: 2231 3435 3733 3837 3732 0931 3435 3733  "145738772.14573
+00011d50: 3837 3732 094e 435f 3030 3030 3038 2e31  8772.NC_000008.1
+00011d60: 3109 2d09 7361 6d70 6c65 3109 2d09 2d09  1.-.sample1.-.-.
+00011d70: 332d 6368 6563 6b09 3136 3839 092d 092d  3-check.1689.-.-
+00011d80: 0979 6573 096f 6b09 2d09 2d09 2d09 2d22  .yes.ok.-.-.-.-"
+00011d90: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00011da0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00011db0: 7445 7175 616c 2872 6573 756c 745b 3234  tEqual(result[24
+00011dc0: 5d2e 7273 7472 6970 2829 2c20 2231 3435  ].rstrip(), "145
+00011dd0: 3733 3837 3733 0931 3435 3733 3837 3733  738773.145738773
+00011de0: 094e 435f 3030 3030 3038 2e31 3109 2d09  .NC_000008.11.-.
+00011df0: 7361 6d70 6c65 3109 2d09 2d09 332d 6368  sample1.-.-.3-ch
+00011e00: 6563 6b09 3139 3430 092d 092d 0979 6573  eck.1940.-.-.yes
+00011e10: 096f 6b09 2d09 2d09 2d09 2d22 2920 2023  .ok.-.-.-.-")  #
+00011e20: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00011e30: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00011e40: 616c 2872 6573 756c 745b 3235 5d2e 7273  al(result[25].rs
+00011e50: 7472 6970 2829 2c20 2231 3435 3733 3837  trip(), "1457387
+00011e60: 3734 0931 3435 3733 3837 3734 094e 435f  74.145738774.NC_
+00011e70: 3030 3030 3038 2e31 3109 2d09 7361 6d70  000008.11.-.samp
+00011e80: 6c65 3109 2d09 2d09 332d 6368 6563 6b09  le1.-.-.3-check.
+00011e90: 3139 3430 092d 092d 0979 6573 096f 6b09  1940.-.-.yes.ok.
+00011ea0: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00011eb0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00011ec0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00011ed0: 6573 756c 745b 3236 5d2e 7273 7472 6970  esult[26].rstrip
+00011ee0: 2829 2c20 2231 3435 3733 3837 3735 0931  (), "145738775.1
+00011ef0: 3435 3733 3837 3735 094e 435f 3030 3030  45738775.NC_0000
+00011f00: 3038 2e31 3109 2d09 7361 6d70 6c65 3109  08.11.-.sample1.
+00011f10: 2d09 2d09 332d 6368 6563 6b09 3139 3633  -.-.3-check.1963
+00011f20: 092d 092d 0979 6573 096f 6b09 2d09 2d09  .-.-.yes.ok.-.-.
+00011f30: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00011f40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011f50: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00011f60: 745b 3237 5d2e 7273 7472 6970 2829 2c20  t[27].rstrip(), 
+00011f70: 2231 3435 3733 3837 3736 0931 3435 3733  "145738776.14573
+00011f80: 3837 3736 094e 435f 3030 3030 3038 2e31  8776.NC_000008.1
+00011f90: 3109 2d09 7361 6d70 6c65 3109 2d09 2d09  1.-.sample1.-.-.
+00011fa0: 332d 6368 6563 6b09 3009 2d09 2d09 6e6f  3-check.0.-.-.no
+00011fb0: 7420 616e 616c 797a 6162 6c65 096c 6f77  t analyzable.low
+00011fc0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00011fd0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00011fe0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00011ff0: 7265 7375 6c74 5b32 385d 2e72 7374 7269  result[28].rstri
+00012000: 7028 292c 2022 3134 3537 3338 3737 3709  p(), "145738777.
+00012010: 3134 3537 3338 3737 3709 4e43 5f30 3030  145738777.NC_000
+00012020: 3030 382e 3131 092d 0973 616d 706c 6531  008.11.-.sample1
+00012030: 092d 092d 0933 2d63 6865 636b 0931 3936  .-.-.3-check.196
+00012040: 3409 2d09 2d09 7965 7309 6f6b 092d 092d  4.-.-.yes.ok.-.-
+00012050: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00012060: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012070: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00012080: 6c74 5b32 395d 2e72 7374 7269 7028 292c  lt[29].rstrip(),
+00012090: 2022 3134 3537 3338 3737 3809 3134 3537   "145738778.1457
+000120a0: 3338 3737 3809 4e43 5f30 3030 3030 382e  38778.NC_000008.
+000120b0: 3131 092d 0973 616d 706c 6531 092d 092d  11.-.sample1.-.-
+000120c0: 0933 2d63 6865 636b 0931 3936 3309 2d09  .3-check.1963.-.
+000120d0: 2d09 7965 7309 6f6b 092d 092d 092d 092d  -.yes.ok.-.-.-.-
+000120e0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+000120f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00012100: 7274 4571 7561 6c28 7265 7375 6c74 5b33  rtEqual(result[3
+00012110: 305d 2e72 7374 7269 7028 292c 2022 3134  0].rstrip(), "14
+00012120: 3537 3338 3737 3909 3134 3537 3338 3737  5738779.14573877
+00012130: 3909 4e43 5f30 3030 3030 382e 3131 092d  9.NC_000008.11.-
+00012140: 0973 616d 706c 6531 092d 092d 0933 2d63  .sample1.-.-.3-c
+00012150: 6865 636b 0931 3935 3809 2d09 2d09 7965  heck.1958.-.-.ye
+00012160: 7309 6f6b 092d 092d 092d 092d 2229 2020  s.ok.-.-.-.-")  
+00012170: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00012180: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00012190: 7561 6c28 7265 7375 6c74 5b33 315d 2e72  ual(result[31].r
+000121a0: 7374 7269 7028 292c 2022 3134 3537 3432  strip(), "145742
+000121b0: 3531 3409 3134 3537 3432 3531 3409 4e43  514.145742514.NC
+000121c0: 5f30 3030 3030 382e 3131 0952 4543 514c  _000008.11.RECQL
+000121d0: 3409 7361 6d70 6c65 3109 4109 4709 332d  4.sample1.A.G.3-
+000121e0: 6368 6563 6b09 3009 3009 3833 3909 6e6f  check.0.0.839.no
+000121f0: 7420 616e 616c 797a 6162 6c65 096c 6f77  t analyzable.low
+00012200: 0970 726f 7465 696e 5f63 6f64 696e 6709  .protein_coding.
+00012210: 7379 6e6f 6e79 6d6f 7573 5f76 6172 6961  synonymous_varia
+00012220: 6e74 0976 6172 6469 6374 2c6d 7574 6563  nt.vardict,mutec
+00012230: 7432 092d 2229 2020 2320 6e6f 7161 0a20  t2.-")  # noqa. 
+00012240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012250: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00012260: 6c74 5b33 325d 2e72 7374 7269 7028 292c  lt[32].rstrip(),
+00012270: 2022 3831 3935 3437 3839 0938 3139 3534   "81954789.81954
+00012280: 3738 3909 4e43 5f30 3030 3031 362e 3131  789.NC_000016.11
+00012290: 0950 4c43 4732 0973 616d 706c 6531 0943  .PLCG2.sample1.C
+000122a0: 0947 5409 322d 696e 6465 6c09 3131 3434  .GT.2-indel.1144
+000122b0: 0931 3137 3209 3239 0979 6573 096f 6b09  .1172.29.yes.ok.
+000122c0: 7072 6f74 6569 6e5f 636f 6469 6e67 0969  protein_coding.i
+000122d0: 6e74 726f 6e5f 7661 7269 616e 7409 7661  ntron_variant.va
+000122e0: 7264 6963 7409 2d22 2920 2023 206e 6f71  rdict.-")  # noq
+000122f0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00012300: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00012310: 6573 756c 745b 3333 5d2e 7273 7472 6970  esult[33].rstrip
+00012320: 2829 2c20 2232 3934 3435 3238 3209 3239  (), "29445282.29
+00012330: 3434 3532 3832 094e 435f 3030 3030 3032  445282.NC_000002
+00012340: 2e31 3109 414c 4b09 7361 6d70 6c65 3109  .11.ALK.sample1.
+00012350: 4709 4109 342d 6f74 6865 7209 3532 3009  G.A.4-other.520.
+00012360: 3238 3409 3309 7965 7309 6f6b 0970 726f  284.3.yes.ok.pro
+00012370: 7465 696e 5f63 6f64 696e 6709 7370 6c69  tein_coding.spli
+00012380: 6365 5f72 6567 696f 6e5f 7661 7269 616e  ce_region_varian
+00012390: 7426 696e 7472 6f6e 5f76 6172 6961 6e74  t&intron_variant
+000123a0: 0976 6172 6469 6374 092d 2229 2020 2320  .vardict.-")  # 
+000123b0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+000123c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000123d0: 6c28 7265 7375 6c74 5b33 345d 2e72 7374  l(result[34].rst
+000123e0: 7269 7028 292c 2022 3831 3935 3437 3839  rip(), "81954789
+000123f0: 0938 3139 3534 3738 3909 4e43 5f30 3030  .81954789.NC_000
+00012400: 3031 362e 3131 0953 4550 5409 7361 6d70  016.11.SEPT.samp
+00012410: 6c65 3109 4309 4709 342d 6f74 6865 7209  le1.C.G.4-other.
+00012420: 3131 3434 0934 3432 0933 3439 0979 6573  1144.442.349.yes
+00012430: 096f 6b09 7072 6f74 6569 6e5f 636f 6469  .ok.protein_codi
+00012440: 6e67 0969 6e74 726f 6e5f 7661 7269 616e  ng.intron_varian
+00012450: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
+00012460: 3209 2d22 2920 2023 206e 6f71 610a 0a20  2.-")  # noqa.. 
+00012470: 2020 2064 6566 2074 6573 745f 6669 6c74     def test_filt
+00012480: 6572 6564 5f6d 7574 6174 696f 6e5f 6869  ered_mutation_hi
+00012490: 6465 5f63 6f6c 756d 6e28 7365 6c66 293a  de_column(self):
+000124a0: 0a20 2020 2020 2020 2066 726f 6d20 6879  .        from hy
+000124b0: 6472 615f 6765 6e65 7469 6373 2e75 7469  dra_genetics.uti
+000124c0: 6c73 2e69 6f2e 686f 7473 706f 745f 7265  ls.io.hotspot_re
+000124d0: 706f 7274 2069 6d70 6f72 7420 6765 6e65  port import gene
+000124e0: 7261 7465 5f68 6f74 7370 6f74 5f72 6570  rate_hotspot_rep
+000124f0: 6f72 740a 2020 2020 2020 2020 6c65 7665  ort.        leve
+00012500: 6c73 203d 205b 2833 3030 2c20 226f 6b22  ls = [(300, "ok"
+00012510: 2c20 2279 6573 2229 2c20 2833 302c 2022  , "yes"), (30, "
+00012520: 6c6f 7722 2c20 2279 6573 2229 2c20 2830  low", "yes"), (0
+00012530: 2c20 226c 6f77 222c 2022 6e6f 7420 616e  , "low", "not an
+00012540: 616c 797a 6162 6c65 2229 5d0a 2020 2020  alyzable")].    
+00012550: 2020 2020 7365 6c66 2e6d 6178 4469 6666      self.maxDiff
+00012560: 203d 2031 3030 3030 0a0a 2020 2020 2020   = 10000..      
+00012570: 2020 7265 706f 7274 203d 206f 732e 7061    report = os.pa
+00012580: 7468 2e6a 6f69 6e28 7365 6c66 2e74 656d  th.join(self.tem
+00012590: 7064 6972 2c20 2266 696c 7465 7265 642e  pdir, "filtered.
+000125a0: 7265 706f 7274 2229 0a20 2020 2020 2020  report").       
+000125b0: 2067 656e 6572 6174 655f 686f 7473 706f   generate_hotspo
+000125c0: 745f 7265 706f 7274 2822 7361 6d70 6c65  t_report("sample
+000125d0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 2020 2020 7265 706f 7274 2c0a 2020 2020      report,.    
+00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012610: 2020 2020 2020 2020 2020 2020 6c65 7665              leve
+00012620: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 2020 2020 7365 6c66 2e68 6f74 7370 6f74      self.hotspot
+00012650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012670: 2020 7365 6c66 2e76 6366 5f76 6570 202b    self.vcf_vep +
+00012680: 2022 2e67 7a22 2c0a 2020 2020 2020 2020   ".gz",.        
+00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 2020 2020 2020 2020 7365 6c66 2e67 7663          self.gvc
+000126b0: 6620 2b20 222e 677a 222c 0a20 2020 2020  f + ".gz",.     
+000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000126e0: 7265 6665 7265 6e63 652c 0a20 2020 2020  reference,.     
+000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012710: 7663 665f 7665 705f 776f 5f70 6963 6b20  vcf_vep_wo_pick 
+00012720: 2b20 222e 677a 222c 0a20 2020 2020 2020  + ".gz",.       
+00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012740: 2020 2020 2020 2020 2022 7465 7374 732f           "tests/
+00012750: 7574 696c 732f 6669 6c65 732f 7265 706f  utils/files/repo
+00012760: 7274 5f63 6f6c 756d 6e73 5f76 6570 5f68  rt_columns_vep_h
+00012770: 6964 655f 636f 6c75 6d6e 2e79 616d 6c22  ide_column.yaml"
+00012780: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
+00012790: 7065 6e28 7265 706f 7274 2c20 2772 2729  pen(report, 'r')
+000127a0: 2061 7320 7265 706f 7274 5f72 6573 756c   as report_resul
+000127b0: 743a 0a20 2020 2020 2020 2020 2020 2068  t:.            h
+000127c0: 6561 6420 3d20 7265 706f 7274 5f72 6573  ead = report_res
+000127d0: 756c 742e 7265 6164 6c69 6e65 2829 0a20  ult.readline(). 
+000127e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000127f0: 6173 7365 7274 4571 7561 6c28 6865 6164  assertEqual(head
+00012800: 2e72 7374 7269 7028 292c 2022 5c74 222e  .rstrip(), "\t".
+00012810: 6a6f 696e 285b 2747 656e 6527 2c20 2273  join(['Gene', "s
+00012820: 616d 706c 6522 2c20 2273 7461 7274 222c  ample", "start",
+00012830: 2022 7265 6622 2c20 2261 6c74 222c 2022   "ref", "alt", "
+00012840: 7265 706f 7274 222c 2027 6776 6366 5f64  report", 'gvcf_d
+00012850: 6570 7468 272c 2022 7265 665f 6465 7074  epth', "ref_dept
+00012860: 6822 2c20 2261 6c74 5f64 6570 7468 222c  h", "alt_depth",
+00012870: 2027 416e 616c 797a 6162 6c65 272c 2027   'Analyzable', '
+00012880: 5661 7269 616e 745f 7479 7065 272c 2027  Variant_type', '
+00012890: 436f 6e73 6571 7565 6e63 6527 2c20 2743  Consequence', 'C
+000128a0: 616c 6c65 7273 272c 2027 436f 6d6d 656e  allers', 'Commen
+000128b0: 7427 5d29 2920 2023 206e 6f71 610a 2020  t']))  # noqa.  
+000128c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000128d0: 203d 2072 6570 6f72 745f 7265 7375 6c74   = report_result
+000128e0: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+000128f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012900: 7365 7274 4571 7561 6c28 6c65 6e28 7265  sertEqual(len(re
+00012910: 7375 6c74 292c 2033 3529 0a20 2020 2020  sult), 35).     
+00012920: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00012930: 7274 4571 7561 6c28 7265 7375 6c74 5b30  rtEqual(result[0
+00012940: 5d2e 7273 7472 6970 2829 2c20 2241 4c4b  ].rstrip(), "ALK
+00012950: 0973 616d 706c 6531 0932 3934 3435 3237  .sample1.2944527
+00012960: 3109 4709 4109 312d 686f 7473 706f 7409  1.G.A.1-hotspot.
+00012970: 3632 3009 3335 3909 3409 7965 7309 7072  620.359.4.yes.pr
+00012980: 6f74 6569 6e5f 636f 6469 6e67 0973 796e  otein_coding.syn
+00012990: 6f6e 796d 6f75 735f 7661 7269 616e 7409  onymous_variant.
+000129a0: 7661 7264 6963 7409 7265 7369 7374 616e  vardict.resistan
+000129b0: 6365 5f6d 7574 6174 696f 6e22 2920 2023  ce_mutation")  #
+000129c0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+000129d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000129e0: 616c 2872 6573 756c 745b 315d 2e72 7374  al(result[1].rst
+000129f0: 7269 7028 292c 2022 4252 4146 0973 616d  rip(), "BRAF.sam
+00012a00: 706c 6531 0931 3430 3439 3833 3539 0943  ple1.140498359.C
+00012a10: 5454 5409 4309 322d 696e 6465 6c09 3130  TTT.C.2-indel.10
+00012a20: 302e 3509 3237 0934 0979 6573 0970 726f  0.5.27.4.yes.pro
+00012a30: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
+00012a40: 6f6e 5f76 6172 6961 6e74 096d 7574 6563  on_variant.mutec
+00012a50: 7432 092d 2229 2020 2320 6e6f 7161 0a20  t2.-")  # noqa. 
+00012a60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012a70: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00012a80: 6c74 5b32 5d2e 7273 7472 6970 2829 2c20  lt[2].rstrip(), 
+00012a90: 222d 0973 616d 706c 6531 0931 3430 3439  "-.sample1.14049
+00012aa0: 3833 3631 092d 092d 0931 2d68 6f74 7370  8361.-.-.1-hotsp
+00012ab0: 6f74 0931 3130 092d 092d 0979 6573 092d  ot.110.-.-.yes.-
+00012ac0: 092d 092d 092d 2229 2020 2023 206e 6f71  .-.-.-")   # noq
+00012ad0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00012ae0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00012af0: 6573 756c 745b 335d 2e72 7374 7269 7028  esult[3].rstrip(
+00012b00: 292c 2022 2d09 7361 6d70 6c65 3109 3134  ), "-.sample1.14
+00012b10: 3034 3533 3133 3609 2d09 2d09 312d 686f  0453136.-.-.1-ho
+00012b20: 7473 706f 7409 3009 2d09 2d09 6e6f 7420  tspot.0.-.-.not 
+00012b30: 616e 616c 797a 6162 6c65 092d 092d 092d  analyzable.-.-.-
+00012b40: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00012b50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012b60: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00012b70: 5b34 5d2e 7273 7472 6970 2829 2c20 222d  [4].rstrip(), "-
+00012b80: 0973 616d 706c 6531 0931 3136 3431 3230  .sample1.1164120
+00012b90: 3433 092d 092d 0931 2d68 6f74 7370 6f74  43.-.-.1-hotspot
+00012ba0: 0930 092d 092d 096e 6f74 2061 6e61 6c79  .0.-.-.not analy
+00012bb0: 7a61 626c 6509 2d09 2d09 2d09 2d22 2920  zable.-.-.-.-") 
+00012bc0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00012bd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00012be0: 7175 616c 2872 6573 756c 745b 355d 2e72  qual(result[5].r
+00012bf0: 7374 7269 7028 292c 2022 2d09 7361 6d70  strip(), "-.samp
+00012c00: 6c65 3109 3239 3434 3532 3731 092d 092d  le1.29445271.-.-
+00012c10: 0933 2d63 6865 636b 0936 3230 092d 092d  .3-check.620.-.-
+00012c20: 0979 6573 092d 092d 092d 092d 2229 2020  .yes.-.-.-.-")  
+00012c30: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00012c40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00012c50: 7561 6c28 7265 7375 6c74 5b36 5d2e 7273  ual(result[6].rs
+00012c60: 7472 6970 2829 2c20 222d 0973 616d 706c  trip(), "-.sampl
+00012c70: 6531 0932 3934 3435 3237 3209 2d09 2d09  e1.29445272.-.-.
+00012c80: 332d 6368 6563 6b09 3232 3109 2d09 2d09  3-check.221.-.-.
+00012c90: 7965 7309 2d09 2d09 2d09 2d22 2920 2023  yes.-.-.-.-")  #
+00012ca0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00012cb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00012cc0: 616c 2872 6573 756c 745b 375d 2e72 7374  al(result[7].rst
+00012cd0: 7269 7028 292c 2022 2d09 7361 6d70 6c65  rip(), "-.sample
+00012ce0: 3109 3239 3434 3532 3733 092d 092d 0933  1.29445273.-.-.3
+00012cf0: 2d63 6865 636b 0936 3238 092d 092d 0979  -check.628.-.-.y
+00012d00: 6573 092d 092d 092d 092d 2229 2020 2320  es.-.-.-.-")  # 
+00012d10: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00012d20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00012d30: 6c28 7265 7375 6c74 5b38 5d2e 7273 7472  l(result[8].rstr
+00012d40: 6970 2829 2c20 222d 0973 616d 706c 6531  ip(), "-.sample1
+00012d50: 0932 3934 3435 3237 3409 2d09 2d09 332d  .29445274.-.-.3-
+00012d60: 6368 6563 6b09 3631 3809 2d09 2d09 7965  check.618.-.-.ye
+00012d70: 7309 2d09 2d09 2d09 2d22 2920 2023 206e  s.-.-.-.-")  # n
+00012d80: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00012d90: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00012da0: 2872 6573 756c 745b 395d 2e72 7374 7269  (result[9].rstri
+00012db0: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012dc0: 3239 3434 3532 3735 092d 092d 0933 2d63  29445275.-.-.3-c
+00012dd0: 6865 636b 0936 3038 092d 092d 0979 6573  heck.608.-.-.yes
+00012de0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00012df0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00012e00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00012e10: 7265 7375 6c74 5b31 305d 2e72 7374 7269  result[10].rstri
+00012e20: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012e30: 3239 3434 3532 3736 092d 092d 0933 2d63  29445276.-.-.3-c
+00012e40: 6865 636b 0936 3231 092d 092d 0979 6573  heck.621.-.-.yes
+00012e50: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00012e60: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00012e70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00012e80: 7265 7375 6c74 5b31 315d 2e72 7374 7269  result[11].rstri
+00012e90: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012ea0: 3239 3434 3532 3737 092d 092d 0933 2d63  29445277.-.-.3-c
+00012eb0: 6865 636b 0931 3832 092d 092d 0979 6573  heck.182.-.-.yes
+00012ec0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00012ed0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00012ee0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00012ef0: 7265 7375 6c74 5b31 325d 2e72 7374 7269  result[12].rstri
+00012f00: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012f10: 3239 3434 3532 3738 092d 092d 0933 2d63  29445278.-.-.3-c
+00012f20: 6865 636b 0935 3530 092d 092d 0979 6573  heck.550.-.-.yes
+00012f30: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00012f40: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00012f50: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00012f60: 7265 7375 6c74 5b31 335d 2e72 7374 7269  result[13].rstri
+00012f70: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012f80: 3239 3434 3532 3739 092d 092d 0933 2d63  29445279.-.-.3-c
+00012f90: 6865 636b 0935 3934 092d 092d 0979 6573  heck.594.-.-.yes
+00012fa0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00012fb0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00012fc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00012fd0: 7265 7375 6c74 5b31 345d 2e72 7374 7269  result[14].rstri
+00012fe0: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00012ff0: 3239 3434 3532 3830 092d 092d 0933 2d63  29445280.-.-.3-c
+00013000: 6865 636b 0935 3339 092d 092d 0979 6573  heck.539.-.-.yes
+00013010: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00013020: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00013030: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00013040: 7265 7375 6c74 5b31 355d 2e72 7374 7269  result[15].rstri
+00013050: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+00013060: 3239 3434 3532 3831 092d 092d 0933 2d63  29445281.-.-.3-c
+00013070: 6865 636b 0935 3236 092d 092d 0979 6573  heck.526.-.-.yes
+00013080: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00013090: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000130a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000130b0: 7265 7375 6c74 5b31 365d 2e72 7374 7269  result[16].rstri
+000130c0: 7028 292c 2022 2d09 7361 6d70 6c65 3109  p(), "-.sample1.
+000130d0: 3134 3537 3338 3736 3509 2d09 2d09 332d  145738765.-.-.3-
+000130e0: 6368 6563 6b09 3136 3136 092d 092d 0979  check.1616.-.-.y
+000130f0: 6573 092d 092d 092d 092d 2229 2020 2320  es.-.-.-.-")  # 
+00013100: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00013110: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00013120: 6c28 7265 7375 6c74 5b31 375d 2e72 7374  l(result[17].rst
+00013130: 7269 7028 292c 2022 2d09 7361 6d70 6c65  rip(), "-.sample
+00013140: 3109 3134 3537 3338 3736 3609 2d09 2d09  1.145738766.-.-.
+00013150: 332d 6368 6563 6b09 3136 3139 092d 092d  3-check.1619.-.-
+00013160: 0979 6573 092d 092d 092d 092d 2229 2020  .yes.-.-.-.-")  
+00013170: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00013180: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00013190: 7561 6c28 7265 7375 6c74 5b31 385d 2e72  ual(result[18].r
+000131a0: 7374 7269 7028 292c 2022 2d09 7361 6d70  strip(), "-.samp
+000131b0: 6c65 3109 3134 3537 3338 3736 3709 2d09  le1.145738767.-.
+000131c0: 2d09 332d 6368 6563 6b09 3135 3935 092d  -.3-check.1595.-
+000131d0: 092d 0979 6573 092d 092d 092d 092d 2229  .-.yes.-.-.-.-")
+000131e0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000131f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00013200: 4571 7561 6c28 7265 7375 6c74 5b31 395d  Equal(result[19]
+00013210: 2e72 7374 7269 7028 292c 2022 4c52 5243  .rstrip(), "LRRC
+00013220: 3134 0973 616d 706c 6531 0931 3435 3733  14.sample1.14573
+00013230: 3837 3638 0947 0943 0933 2d63 6865 636b  8768.G.C.3-check
+00013240: 0931 3534 3709 3509 3237 0979 6573 0970  .1547.5.27.yes.p
+00013250: 726f 7465 696e 5f63 6f64 696e 6709 7570  rotein_coding.up
+00013260: 7374 7265 616d 5f67 656e 655f 7661 7269  stream_gene_vari
+00013270: 616e 7409 7661 7264 6963 7409 2d22 2920  ant.vardict.-") 
+00013280: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00013290: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000132a0: 7175 616c 2872 6573 756c 745b 3230 5d2e  qual(result[20].
+000132b0: 7273 7472 6970 2829 2c20 222d 0973 616d  rstrip(), "-.sam
+000132c0: 706c 6531 0931 3435 3733 3837 3639 092d  ple1.145738769.-
+000132d0: 092d 0933 2d63 6865 636b 0931 3634 3409  .-.3-check.1644.
+000132e0: 2d09 2d09 7965 7309 2d09 2d09 2d09 2d22  -.-.yes.-.-.-.-"
+000132f0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00013300: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00013310: 7445 7175 616c 2872 6573 756c 745b 3231  tEqual(result[21
+00013320: 5d2e 7273 7472 6970 2829 2c20 222d 0973  ].rstrip(), "-.s
+00013330: 616d 706c 6531 0931 3435 3733 3837 3730  ample1.145738770
+00013340: 092d 092d 0933 2d63 6865 636b 0931 3636  .-.-.3-check.166
+00013350: 3709 2d09 2d09 7965 7309 2d09 2d09 2d09  7.-.-.yes.-.-.-.
+00013360: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+00013370: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00013380: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00013390: 3232 5d2e 7273 7472 6970 2829 2c20 222d  22].rstrip(), "-
+000133a0: 0973 616d 706c 6531 0931 3435 3733 3837  .sample1.1457387
+000133b0: 3731 092d 092d 0933 2d63 6865 636b 0931  71.-.-.3-check.1
+000133c0: 3638 3509 2d09 2d09 7965 7309 2d09 2d09  685.-.-.yes.-.-.
+000133d0: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+000133e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000133f0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00013400: 745b 3233 5d2e 7273 7472 6970 2829 2c20  t[23].rstrip(), 
+00013410: 222d 0973 616d 706c 6531 0931 3435 3733  "-.sample1.14573
+00013420: 3837 3732 092d 092d 0933 2d63 6865 636b  8772.-.-.3-check
+00013430: 0931 3638 3909 2d09 2d09 7965 7309 2d09  .1689.-.-.yes.-.
+00013440: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00013450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013460: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00013470: 756c 745b 3234 5d2e 7273 7472 6970 2829  ult[24].rstrip()
+00013480: 2c20 222d 0973 616d 706c 6531 0931 3435  , "-.sample1.145
+00013490: 3733 3837 3733 092d 092d 0933 2d63 6865  738773.-.-.3-che
+000134a0: 636b 0931 3934 3009 2d09 2d09 7965 7309  ck.1940.-.-.yes.
+000134b0: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+000134c0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000134d0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000134e0: 6573 756c 745b 3235 5d2e 7273 7472 6970  esult[25].rstrip
+000134f0: 2829 2c20 222d 0973 616d 706c 6531 0931  (), "-.sample1.1
+00013500: 3435 3733 3837 3734 092d 092d 0933 2d63  45738774.-.-.3-c
+00013510: 6865 636b 0931 3934 3009 2d09 2d09 7965  heck.1940.-.-.ye
+00013520: 7309 2d09 2d09 2d09 2d22 2920 2023 206e  s.-.-.-.-")  # n
+00013530: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00013540: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013550: 2872 6573 756c 745b 3236 5d2e 7273 7472  (result[26].rstr
+00013560: 6970 2829 2c20 222d 0973 616d 706c 6531  ip(), "-.sample1
+00013570: 0931 3435 3733 3837 3735 092d 092d 0933  .145738775.-.-.3
+00013580: 2d63 6865 636b 0931 3936 3309 2d09 2d09  -check.1963.-.-.
+00013590: 7965 7309 2d09 2d09 2d09 2d22 2920 2023  yes.-.-.-.-")  #
+000135a0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+000135b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000135c0: 616c 2872 6573 756c 745b 3237 5d2e 7273  al(result[27].rs
+000135d0: 7472 6970 2829 2c20 222d 0973 616d 706c  trip(), "-.sampl
+000135e0: 6531 0931 3435 3733 3837 3736 092d 092d  e1.145738776.-.-
+000135f0: 0933 2d63 6865 636b 0930 092d 092d 096e  .3-check.0.-.-.n
+00013600: 6f74 2061 6e61 6c79 7a61 626c 6509 2d09  ot analyzable.-.
+00013610: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00013620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013630: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00013640: 756c 745b 3238 5d2e 7273 7472 6970 2829  ult[28].rstrip()
+00013650: 2c20 222d 0973 616d 706c 6531 0931 3435  , "-.sample1.145
+00013660: 3733 3837 3737 092d 092d 0933 2d63 6865  738777.-.-.3-che
+00013670: 636b 0931 3936 3409 2d09 2d09 7965 7309  ck.1964.-.-.yes.
+00013680: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00013690: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000136a0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000136b0: 6573 756c 745b 3239 5d2e 7273 7472 6970  esult[29].rstrip
+000136c0: 2829 2c20 222d 0973 616d 706c 6531 0931  (), "-.sample1.1
+000136d0: 3435 3733 3837 3738 092d 092d 0933 2d63  45738778.-.-.3-c
+000136e0: 6865 636b 0931 3936 3309 2d09 2d09 7965  heck.1963.-.-.ye
+000136f0: 7309 2d09 2d09 2d09 2d22 2920 2023 206e  s.-.-.-.-")  # n
+00013700: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00013710: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013720: 2872 6573 756c 745b 3330 5d2e 7273 7472  (result[30].rstr
+00013730: 6970 2829 2c20 222d 0973 616d 706c 6531  ip(), "-.sample1
+00013740: 0931 3435 3733 3837 3739 092d 092d 0933  .145738779.-.-.3
+00013750: 2d63 6865 636b 0931 3935 3809 2d09 2d09  -check.1958.-.-.
+00013760: 7965 7309 2d09 2d09 2d09 2d22 2920 2023  yes.-.-.-.-")  #
+00013770: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00013780: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00013790: 616c 2872 6573 756c 745b 3331 5d2e 7273  al(result[31].rs
+000137a0: 7472 6970 2829 2c20 2252 4543 514c 3409  trip(), "RECQL4.
+000137b0: 7361 6d70 6c65 3109 3134 3537 3432 3531  sample1.14574251
+000137c0: 3409 4109 4709 332d 6368 6563 6b09 3009  4.A.G.3-check.0.
+000137d0: 3009 3833 3909 6e6f 7420 616e 616c 797a  0.839.not analyz
+000137e0: 6162 6c65 0970 726f 7465 696e 5f63 6f64  able.protein_cod
+000137f0: 696e 6709 7379 6e6f 6e79 6d6f 7573 5f76  ing.synonymous_v
+00013800: 6172 6961 6e74 0976 6172 6469 6374 2c6d  ariant.vardict,m
+00013810: 7574 6563 7432 092d 2229 2020 2320 6e6f  utect2.-")  # no
+00013820: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00013830: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00013840: 7265 7375 6c74 5b33 325d 2e72 7374 7269  result[32].rstri
+00013850: 7028 292c 2022 504c 4347 3209 7361 6d70  p(), "PLCG2.samp
+00013860: 6c65 3109 3831 3935 3437 3839 0943 0947  le1.81954789.C.G
+00013870: 5409 322d 696e 6465 6c09 3131 3434 0931  T.2-indel.1144.1
+00013880: 3137 3209 3239 0979 6573 0970 726f 7465  172.29.yes.prote
+00013890: 696e 5f63 6f64 696e 6709 696e 7472 6f6e  in_coding.intron
+000138a0: 5f76 6172 6961 6e74 0976 6172 6469 6374  _variant.vardict
+000138b0: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+000138c0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000138d0: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+000138e0: 5b33 335d 2e72 7374 7269 7028 292c 2022  [33].rstrip(), "
+000138f0: 414c 4b09 7361 6d70 6c65 3109 3239 3434  ALK.sample1.2944
+00013900: 3532 3832 0947 0941 0934 2d6f 7468 6572  5282.G.A.4-other
+00013910: 0935 3230 0932 3834 0933 0979 6573 0970  .520.284.3.yes.p
+00013920: 726f 7465 696e 5f63 6f64 696e 6709 7370  rotein_coding.sp
+00013930: 6c69 6365 5f72 6567 696f 6e5f 7661 7269  lice_region_vari
+00013940: 616e 7426 696e 7472 6f6e 5f76 6172 6961  ant&intron_varia
+00013950: 6e74 0976 6172 6469 6374 092d 2229 2020  nt.vardict.-")  
+00013960: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00013970: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00013980: 7561 6c28 7265 7375 6c74 5b33 345d 2e72  ual(result[34].r
+00013990: 7374 7269 7028 292c 2022 5345 5054 0973  strip(), "SEPT.s
+000139a0: 616d 706c 6531 0938 3139 3534 3738 3909  ample1.81954789.
+000139b0: 4309 4709 342d 6f74 6865 7209 3131 3434  C.G.4-other.1144
+000139c0: 0934 3432 0933 3439 0979 6573 0970 726f  .442.349.yes.pro
+000139d0: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
+000139e0: 6f6e 5f76 6172 6961 6e74 0976 6172 6469  on_variant.vardi
+000139f0: 6374 2c6d 7574 6563 7432 092d 2229 2020  ct,mutect2.-")  
+00013a00: 2320 6e6f 7161 0a0a 2020 2020 6465 6620  # noqa..    def 
+00013a10: 7465 7374 5f66 696c 7465 7265 645f 7665  test_filtered_ve
+00013a20: 705f 7265 6765 785f 6578 7472 6163 7428  p_regex_extract(
+00013a30: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+00013a40: 726f 6d20 6879 6472 615f 6765 6e65 7469  rom hydra_geneti
+00013a50: 6373 2e75 7469 6c73 2e69 6f2e 686f 7473  cs.utils.io.hots
+00013a60: 706f 745f 7265 706f 7274 2069 6d70 6f72  pot_report impor
+00013a70: 7420 6765 6e65 7261 7465 5f68 6f74 7370  t generate_hotsp
+00013a80: 6f74 5f72 6570 6f72 740a 2020 2020 2020  ot_report.      
+00013a90: 2020 6c65 7665 6c73 203d 205b 2833 3030    levels = [(300
+00013aa0: 2c20 226f 6b22 2c20 2279 6573 2229 2c20  , "ok", "yes"), 
+00013ab0: 2833 302c 2022 6c6f 7722 2c20 2279 6573  (30, "low", "yes
+00013ac0: 2229 2c20 2830 2c20 226c 6f77 222c 2022  "), (0, "low", "
+00013ad0: 6e6f 7420 616e 616c 797a 6162 6c65 2229  not analyzable")
+00013ae0: 5d0a 2020 2020 2020 2020 7365 6c66 2e6d  ].        self.m
+00013af0: 6178 4469 6666 203d 2031 3030 3030 0a0a  axDiff = 10000..
+00013b00: 2020 2020 2020 2020 7265 706f 7274 203d          report =
+00013b10: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00013b20: 6c66 2e74 656d 7064 6972 2c20 2266 696c  lf.tempdir, "fil
+00013b30: 7465 7265 642e 7265 706f 7274 2229 0a20  tered.report"). 
+00013b40: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
+00013b50: 686f 7473 706f 745f 7265 706f 7274 2822  hotspot_report("
+00013b60: 7361 6d70 6c65 3122 2c0a 2020 2020 2020  sample1",.      
 00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b80: 2020 2020 2073 656c 662e 7663 665f 7665       self.vcf_ve
-00013b90: 7020 2b20 222e 677a 222c 0a20 2020 2020  p + ".gz",.     
+00013b80: 2020 2020 2020 2020 2020 7265 706f 7274            report
+00013b90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013bc0: 6776 6366 202b 2022 2e67 7a22 2c0a 2020  gvcf + ".gz",.  
-00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013be0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013bf0: 6c66 2e72 6566 6572 656e 6365 2c0a 2020  lf.reference,.  
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013c20: 6c66 2e76 6366 5f76 6570 5f77 6f5f 7069  lf.vcf_vep_wo_pi
-00013c30: 636b 202b 2022 2e67 7a22 2c0a 2020 2020  ck + ".gz",.    
-00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 2020 2020 2020 2020 2020 2020 2274 6573              "tes
-00013c60: 7473 2f75 7469 6c73 2f66 696c 6573 2f72  ts/utils/files/r
-00013c70: 6570 6f72 745f 636f 6c75 6d6e 735f 7365  eport_columns_se
-00013c80: 6c65 6374 5f63 6f6c 756d 6e2e 7961 6d6c  lect_column.yaml
-00013c90: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
-00013ca0: 6f70 656e 2872 6570 6f72 742c 2027 7227  open(report, 'r'
-00013cb0: 2920 6173 2072 6570 6f72 745f 7265 7375  ) as report_resu
-00013cc0: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
-00013cd0: 6865 6164 203d 2072 6570 6f72 745f 7265  head = report_re
-00013ce0: 7375 6c74 2e72 6561 646c 696e 6528 290a  sult.readline().
-00013cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013d00: 2e61 7373 6572 7445 7175 616c 2868 6561  .assertEqual(hea
-00013d10: 642e 7273 7472 6970 2829 2c20 225c 7422  d.rstrip(), "\t"
-00013d20: 2e6a 6f69 6e28 5b22 7361 6d70 6c65 222c  .join(["sample",
-00013d30: 2022 6368 7222 2c20 2273 7461 7274 222c   "chr", "start",
-00013d40: 2022 7374 6f70 222c 2022 7265 6622 2c20   "stop", "ref", 
-00013d50: 2261 6c74 222c 2022 7265 706f 7274 222c  "alt", "report",
-00013d60: 2027 6776 6366 5f64 6570 7468 272c 2022   'gvcf_depth', "
-00013d70: 7265 665f 6465 7074 6822 2c20 2261 6c74  ref_depth", "alt
-00013d80: 5f64 6570 7468 222c 2027 416e 616c 797a  _depth", 'Analyz
-00013d90: 6162 6c65 272c 2027 4d69 6e5f 7265 6164  able', 'Min_read
-00013da0: 5f64 6570 7468 3330 3027 2c20 2747 656e  _depth300', 'Gen
-00013db0: 6527 2c20 2756 6172 6961 6e74 5f74 7970  e', 'Variant_typ
-00013dc0: 6527 2c20 2743 6f6e 7365 7175 656e 6365  e', 'Consequence
-00013dd0: 272c 2027 4361 6c6c 6572 7327 2c20 2743  ', 'Callers', 'C
-00013de0: 6f6d 6d65 6e74 272c 2027 4e6f 745f 456d  omment', 'Not_Em
-00013df0: 7074 7927 2c20 2745 6d70 7479 275d 2929  pty', 'Empty']))
-00013e00: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-00013e10: 2020 2020 2072 6573 756c 7420 3d20 7265       result = re
-00013e20: 706f 7274 5f72 6573 756c 742e 7265 6164  port_result.read
-00013e30: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-00013e40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00013e50: 7175 616c 286c 656e 2872 6573 756c 7429  qual(len(result)
-00013e60: 2c20 3133 290a 2020 2020 2020 2020 2020  , 13).          
-00013e70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00013e80: 616c 2872 6573 756c 745b 305d 2e72 7374  al(result[0].rst
-00013e90: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
-00013ea0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
-00013eb0: 3435 3237 3109 3239 3434 3532 3731 0947  45271.29445271.G
-00013ec0: 0941 0931 2d68 6f74 7370 6f74 0936 3230  .A.1-hotspot.620
-00013ed0: 0933 3539 0934 0979 6573 096f 6b09 414c  .359.4.yes.ok.AL
-00013ee0: 4b09 7072 6f74 6569 6e5f 636f 6469 6e67  K.protein_coding
-00013ef0: 0973 796e 6f6e 796d 6f75 735f 7661 7269  .synonymous_vari
-00013f00: 616e 7409 7661 7264 6963 7409 7265 7369  ant.vardict.resi
-00013f10: 7374 616e 6365 5f6d 7574 6174 696f 6e09  stance_mutation.
-00013f20: 414c 4b09 2d22 2920 2023 206e 6f71 610a  ALK.-")  # noqa.
-00013f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013f40: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-00013f50: 756c 745b 315d 2e72 7374 7269 7028 292c  ult[1].rstrip(),
-00013f60: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
-00013f70: 3030 372e 3133 0931 3430 3439 3833 3539  007.13.140498359
-00013f80: 0931 3430 3439 3833 3632 0943 5454 5409  .140498362.CTTT.
-00013f90: 4309 322d 696e 6465 6c09 3130 302e 3509  C.2-indel.100.5.
-00013fa0: 3237 0934 0979 6573 096c 6f77 0942 5241  27.4.yes.low.BRA
-00013fb0: 4609 7072 6f74 6569 6e5f 636f 6469 6e67  F.protein_coding
-00013fc0: 0969 6e74 726f 6e5f 7661 7269 616e 7409  .intron_variant.
-00013fd0: 6d75 7465 6374 3209 2d09 4547 4652 092d  mutect2.-.EGFR.-
-00013fe0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
-00013ff0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00014000: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
-00014010: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
-00014020: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
-00014030: 3309 3134 3034 3938 3336 3109 3134 3034  3.140498361.1404
-00014040: 3938 3336 3109 2d09 2d09 312d 686f 7473  98361.-.-.1-hots
-00014050: 706f 7409 3131 3009 2d09 2d09 7965 7309  pot.110.-.-.yes.
-00014060: 6c6f 7709 4547 4652 092d 092d 092d 092d  low.EGFR.-.-.-.-
-00014070: 092d 0945 4746 5222 2920 2020 2320 6e6f  .-.EGFR")   # no
-00014080: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-00014090: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000140a0: 7265 7375 6c74 5b33 5d2e 7273 7472 6970  result[3].rstrip
-000140b0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-000140c0: 3030 3030 3037 2e31 3309 3134 3034 3533  000007.13.140453
-000140d0: 3133 3609 3134 3034 3533 3133 3609 2d09  136.140453136.-.
-000140e0: 2d09 312d 686f 7473 706f 7409 3009 2d09  -.1-hotspot.0.-.
-000140f0: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
-00014100: 096c 6f77 0942 5241 4609 2d09 2d09 2d09  .low.BRAF.-.-.-.
-00014110: 2d09 2d09 4252 4146 2229 2020 2320 6e6f  -.-.BRAF")  # no
-00014120: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-00014130: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00014140: 7265 7375 6c74 5b34 5d2e 7273 7472 6970  result[4].rstrip
-00014150: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-00014160: 3030 3030 3037 2e31 3309 3131 3634 3132  000007.13.116412
-00014170: 3034 3309 3131 3634 3132 3034 3309 2d09  043.116412043.-.
-00014180: 2d09 312d 686f 7473 706f 7409 3009 2d09  -.1-hotspot.0.-.
-00014190: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
-000141a0: 096c 6f77 094d 4554 092d 092d 092d 092d  .low.MET.-.-.-.-
-000141b0: 092d 094d 4554 2229 2020 2320 6e6f 7161  .-.MET")  # noqa
-000141c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000141d0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-000141e0: 7375 6c74 5b35 5d2e 7273 7472 6970 2829  sult[5].rstrip()
-000141f0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-00014200: 3030 3032 2e31 3109 3239 3434 3532 3732  0002.11.29445272
-00014210: 0932 3934 3435 3237 3209 2d09 2d09 332d  .29445272.-.-.3-
-00014220: 6368 6563 6b09 3232 3109 2d09 2d09 7965  check.221.-.-.ye
-00014230: 7309 6c6f 7709 414c 4b09 2d09 2d09 2d09  s.low.ALK.-.-.-.
-00014240: 2d09 2d09 414c 4b22 2920 2023 206e 6f71  -.-.ALK")  # noq
-00014250: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00014260: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00014270: 6573 756c 745b 365d 2e72 7374 7269 7028  esult[6].rstrip(
-00014280: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-00014290: 3030 3030 322e 3131 0932 3934 3435 3237  00002.11.2944527
-000142a0: 3709 3239 3434 3532 3737 092d 092d 0933  7.29445277.-.-.3
-000142b0: 2d63 6865 636b 0931 3832 092d 092d 0979  -check.182.-.-.y
-000142c0: 6573 096c 6f77 0941 4c4b 092d 092d 092d  es.low.ALK.-.-.-
-000142d0: 092d 092d 0941 4c4b 2229 2020 2320 6e6f  .-.-.ALK")  # no
-000142e0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
-000142f0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00014300: 7265 7375 6c74 5b37 5d2e 7273 7472 6970  result[7].rstrip
-00014310: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-00014320: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
-00014330: 3736 3809 3134 3537 3338 3736 3809 4709  768.145738768.G.
-00014340: 4309 332d 6368 6563 6b09 3135 3437 0935  C.3-check.1547.5
-00014350: 0932 3709 7965 7309 6f6b 094c 5252 4331  .27.yes.ok.LRRC1
-00014360: 3409 7072 6f74 6569 6e5f 636f 6469 6e67  4.protein_coding
-00014370: 0975 7073 7472 6561 6d5f 6765 6e65 5f76  .upstream_gene_v
-00014380: 6172 6961 6e74 0976 6172 6469 6374 092d  ariant.vardict.-
-00014390: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
-000143a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000143b0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
-000143c0: 6c74 5b38 5d2e 7273 7472 6970 2829 2c20  lt[8].rstrip(), 
-000143d0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
-000143e0: 3038 2e31 3109 3134 3537 3338 3737 3609  08.11.145738776.
-000143f0: 3134 3537 3338 3737 3609 2d09 2d09 332d  145738776.-.-.3-
-00014400: 6368 6563 6b09 3009 2d09 2d09 6e6f 7420  check.0.-.-.not 
-00014410: 616e 616c 797a 6162 6c65 096c 6f77 092d  analyzable.low.-
-00014420: 092d 092d 092d 092d 092d 092d 2229 2020  .-.-.-.-.-.-")  
-00014430: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00014440: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00014450: 7561 6c28 7265 7375 6c74 5b39 5d2e 7273  ual(result[9].rs
-00014460: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-00014470: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
-00014480: 3537 3432 3531 3409 3134 3537 3432 3531  5742514.14574251
-00014490: 3409 4109 4709 332d 6368 6563 6b09 3009  4.A.G.3-check.0.
-000144a0: 3009 3833 3909 6e6f 7420 616e 616c 797a  0.839.not analyz
-000144b0: 6162 6c65 096c 6f77 0952 4543 514c 3409  able.low.RECQL4.
-000144c0: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-000144d0: 796e 6f6e 796d 6f75 735f 7661 7269 616e  ynonymous_varian
-000144e0: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
-000144f0: 3209 2d09 2d09 2d22 2920 2023 206e 6f71  2.-.-.-")  # noq
-00014500: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00014510: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00014520: 6573 756c 745b 3130 5d2e 7273 7472 6970  esult[10].rstrip
-00014530: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-00014540: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
-00014550: 3839 0938 3139 3534 3738 3909 4309 4754  89.81954789.C.GT
-00014560: 0932 2d69 6e64 656c 0931 3134 3409 3131  .2-indel.1144.11
-00014570: 3732 0932 3909 7965 7309 6f6b 0950 4c43  72.29.yes.ok.PLC
-00014580: 4732 0970 726f 7465 696e 5f63 6f64 696e  G2.protein_codin
-00014590: 6709 696e 7472 6f6e 5f76 6172 6961 6e74  g.intron_variant
-000145a0: 0976 6172 6469 6374 092d 092d 092d 2229  .vardict.-.-.-")
-000145b0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-000145c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000145d0: 4571 7561 6c28 7265 7375 6c74 5b31 315d  Equal(result[11]
-000145e0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
-000145f0: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
-00014600: 0932 3934 3435 3238 3209 3239 3434 3532  .29445282.294452
-00014610: 3832 0947 0941 0934 2d6f 7468 6572 0935  82.G.A.4-other.5
-00014620: 3230 0932 3834 0933 0979 6573 096f 6b09  20.284.3.yes.ok.
-00014630: 414c 4b09 7072 6f74 6569 6e5f 636f 6469  ALK.protein_codi
-00014640: 6e67 0973 706c 6963 655f 7265 6769 6f6e  ng.splice_region
-00014650: 5f76 6172 6961 6e74 2669 6e74 726f 6e5f  _variant&intron_
-00014660: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
-00014670: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
-00014680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014690: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-000146a0: 756c 745b 3132 5d2e 7273 7472 6970 2829  ult[12].rstrip()
-000146b0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
-000146c0: 3030 3136 2e31 3109 3831 3935 3437 3839  0016.11.81954789
-000146d0: 0938 3139 3534 3738 3909 4309 4709 342d  .81954789.C.G.4-
-000146e0: 6f74 6865 7209 3131 3434 0934 3432 0933  other.1144.442.3
-000146f0: 3439 0979 6573 096f 6b09 5345 5054 0970  49.yes.ok.SEPT.p
-00014700: 726f 7465 696e 5f63 6f64 696e 6709 696e  rotein_coding.in
-00014710: 7472 6f6e 5f76 6172 6961 6e74 0976 6172  tron_variant.var
-00014720: 6469 6374 2c6d 7574 6563 7432 092d 092d  dict,mutect2.-.-
-00014730: 092d 2229 2020 2320 6e6f 7161 0a0a 2020  .-")  # noqa..  
-00014740: 2020 6465 6620 7465 7374 5f76 6570 5f77    def test_vep_w
-00014750: 6f5f 7069 636b 5f63 686f 7365 5f74 7261  o_pick_chose_tra
-00014760: 6e73 6372 6970 7428 7365 6c66 293a 0a20  nscript(self):. 
-00014770: 2020 2020 2020 2066 726f 6d20 6879 6472         from hydr
-00014780: 615f 6765 6e65 7469 6373 2e75 7469 6c73  a_genetics.utils
-00014790: 2e69 6f2e 686f 7473 706f 745f 7265 706f  .io.hotspot_repo
-000147a0: 7274 2069 6d70 6f72 7420 6765 6e65 7261  rt import genera
-000147b0: 7465 5f68 6f74 7370 6f74 5f72 6570 6f72  te_hotspot_repor
-000147c0: 740a 2020 2020 2020 2020 6c65 7665 6c73  t.        levels
-000147d0: 203d 205b 2833 3030 2c20 226f 6b22 2c20   = [(300, "ok", 
-000147e0: 2279 6573 2229 2c20 2833 302c 2022 6c6f  "yes"), (30, "lo
-000147f0: 7722 2c20 2279 6573 2229 2c20 2830 2c20  w", "yes"), (0, 
-00014800: 226c 6f77 222c 2022 6e6f 7420 616e 616c  "low", "not anal
-00014810: 797a 6162 6c65 2229 5d0a 0a20 2020 2020  yzable")]..     
-00014820: 2020 2073 656c 662e 6d61 7844 6966 6620     self.maxDiff 
-00014830: 3d20 3130 3030 300a 0a20 2020 2020 2020  = 10000..       
-00014840: 2072 6570 6f72 7420 3d20 6f73 2e70 6174   report = os.pat
-00014850: 682e 6a6f 696e 2873 656c 662e 7465 6d70  h.join(self.temp
-00014860: 6469 722c 2022 6669 6c74 6572 6564 2e72  dir, "filtered.r
-00014870: 6570 6f72 7422 290a 2020 2020 2020 2020  eport").        
-00014880: 6765 6e65 7261 7465 5f68 6f74 7370 6f74  generate_hotspot
-00014890: 5f72 6570 6f72 7428 2273 616d 706c 6531  _report("sample1
-000148a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2020 2072 6570 6f72 742c 0a20 2020 2020     report,.     
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 2020 2020 2020 2020 2020 206c 6576 656c             level
-000148f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2073 656c 662e 686f 7473 706f 742c     self.hotspot,
-00014920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014940: 2073 656c 662e 7663 665f 7665 7020 2b20   self.vcf_vep + 
-00014950: 222e 677a 222c 0a20 2020 2020 2020 2020  ".gz",.         
-00014960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014970: 2020 2020 2020 2073 656c 662e 6776 6366         self.gvcf
-00014980: 202b 2022 2e67 7a22 2c0a 2020 2020 2020   + ".gz",.      
-00014990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000149b0: 6566 6572 656e 6365 2c0a 2020 2020 2020  eference,.      
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-000149e0: 6366 5f76 6570 5f77 6f5f 7069 636b 202b  cf_vep_wo_pick +
-000149f0: 2022 2e67 7a22 2c0a 2020 2020 2020 2020   ".gz",.        
-00014a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a10: 2020 2020 2020 2020 2274 6573 7473 2f75          "tests/u
-00014a20: 7469 6c73 2f66 696c 6573 2f72 6570 6f72  tils/files/repor
-00014a30: 745f 636f 6c75 6d6e 735f 7365 6c65 6374  t_columns_select
-00014a40: 5f63 6f6c 756d 6e32 2e79 616d 6c22 290a  _column2.yaml").
-00014a50: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00014a60: 6e28 7265 706f 7274 2c20 2772 2729 2061  n(report, 'r') a
-00014a70: 7320 7265 706f 7274 5f72 6573 756c 743a  s report_result:
-00014a80: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
-00014a90: 6420 3d20 7265 706f 7274 5f72 6573 756c  d = report_resul
-00014aa0: 742e 7265 6164 6c69 6e65 2829 0a20 2020  t.readline().   
-00014ab0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00014ac0: 7365 7274 4571 7561 6c28 6865 6164 2e72  sertEqual(head.r
-00014ad0: 7374 7269 7028 292c 2022 5c74 222e 6a6f  strip(), "\t".jo
-00014ae0: 696e 285b 2273 616d 706c 6522 2c20 2263  in(["sample", "c
-00014af0: 6872 222c 2022 7374 6172 7422 2c20 2273  hr", "start", "s
-00014b00: 746f 7022 2c20 2272 6566 222c 2022 616c  top", "ref", "al
-00014b10: 7422 2c20 2272 6570 6f72 7422 2c20 2767  t", "report", 'g
-00014b20: 7663 665f 6465 7074 6827 2c20 2272 6566  vcf_depth', "ref
-00014b30: 5f64 6570 7468 222c 2022 616c 745f 6465  _depth", "alt_de
-00014b40: 7074 6822 2c20 2741 6e61 6c79 7a61 626c  pth", 'Analyzabl
-00014b50: 6527 2c20 274d 696e 5f72 6561 645f 6465  e', 'Min_read_de
-00014b60: 7074 6833 3030 272c 2027 4765 6e65 272c  pth300', 'Gene',
-00014b70: 2022 5472 616e 7363 7269 7074 222c 2027   "Transcript", '
-00014b80: 416d 696e 6f5f 6163 6964 5f63 6861 6e67  Amino_acid_chang
-00014b90: 6527 2c20 2756 6172 6961 6e74 5f74 7970  e', 'Variant_typ
-00014ba0: 6527 2c20 2743 6f6e 7365 7175 656e 6365  e', 'Consequence
-00014bb0: 272c 2027 4361 6c6c 6572 7327 2c20 2743  ', 'Callers', 'C
-00014bc0: 6f6d 6d65 6e74 272c 2027 4e6f 745f 456d  omment', 'Not_Em
-00014bd0: 7074 7927 2c20 2745 6d70 7479 275d 2929  pty', 'Empty']))
-00014be0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-00014bf0: 2020 2020 2072 6573 756c 7420 3d20 7265       result = re
-00014c00: 706f 7274 5f72 6573 756c 742e 7265 6164  port_result.read
-00014c10: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-00014c20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00014c30: 7175 616c 286c 656e 2872 6573 756c 7429  qual(len(result)
-00014c40: 2c20 3133 290a 2020 2020 2020 2020 2020  , 13).          
-00014c50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00014c60: 616c 2872 6573 756c 745b 305d 2e72 7374  al(result[0].rst
-00014c70: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
-00014c80: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
-00014c90: 3435 3237 3109 3239 3434 3532 3731 0947  45271.29445271.G
-00014ca0: 0941 0931 2d68 6f74 7370 6f74 0936 3230  .A.1-hotspot.620
-00014cb0: 0933 3539 0934 0979 6573 096f 6b09 414c  .359.4.yes.ok.AL
-00014cc0: 4b09 4e4d 5f30 3034 3330 342e 3409 4c65  K.NM_004304.4.Le
-00014cd0: 7531 3135 3209 7072 6f74 6569 6e5f 636f  u1152.protein_co
-00014ce0: 6469 6e67 0973 796e 6f6e 796d 6f75 735f  ding.synonymous_
-00014cf0: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
-00014d00: 7265 7369 7374 616e 6365 5f6d 7574 6174  resistance_mutat
-00014d10: 696f 6e09 414c 4b09 2d22 2920 2023 206e  ion.ALK.-")  # n
-00014d20: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00014d30: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00014d40: 2872 6573 756c 745b 315d 2e72 7374 7269  (result[1].rstri
-00014d50: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
-00014d60: 5f30 3030 3030 372e 3133 0931 3430 3439  _000007.13.14049
-00014d70: 3833 3539 0931 3430 3439 3833 3632 0943  8359.140498362.C
-00014d80: 5454 5409 4309 322d 696e 6465 6c09 3130  TTT.C.2-indel.10
-00014d90: 302e 3509 3237 0934 0979 6573 096c 6f77  0.5.27.4.yes.low
-00014da0: 0942 5241 4609 584d 5f30 3035 3235 3030  .BRAF.XM_0052500
-00014db0: 3435 2e31 092d 0970 726f 7465 696e 5f63  45.1.-.protein_c
-00014dc0: 6f64 696e 6709 696e 7472 6f6e 5f76 6172  oding.intron_var
-00014dd0: 6961 6e74 096d 7574 6563 7432 092d 0945  iant.mutect2.-.E
-00014de0: 4746 5209 2d22 2920 2023 206e 6f71 610a  GFR.-")  # noqa.
-00014df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014e00: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-00014e10: 756c 745b 325d 2e72 7374 7269 7028 292c  ult[2].rstrip(),
-00014e20: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
-00014e30: 3030 372e 3133 0931 3430 3439 3833 3631  007.13.140498361
-00014e40: 0931 3430 3439 3833 3631 092d 092d 0931  .140498361.-.-.1
-00014e50: 2d68 6f74 7370 6f74 0931 3130 092d 092d  -hotspot.110.-.-
-00014e60: 0979 6573 096c 6f77 0945 4746 5209 2d09  .yes.low.EGFR.-.
-00014e70: 2d09 2d09 2d09 2d09 2d09 2d09 4547 4652  -.-.-.-.-.-.EGFR
-00014e80: 2229 2020 2023 206e 6f71 610a 2020 2020  ")   # noqa.    
-00014e90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00014ea0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-00014eb0: 335d 2e72 7374 7269 7028 292c 2022 7361  3].rstrip(), "sa
-00014ec0: 6d70 6c65 3109 4e43 5f30 3030 3030 372e  mple1.NC_000007.
-00014ed0: 3133 0931 3430 3435 3331 3336 0931 3430  13.140453136.140
-00014ee0: 3435 3331 3336 092d 092d 0931 2d68 6f74  453136.-.-.1-hot
-00014ef0: 7370 6f74 0930 092d 092d 096e 6f74 2061  spot.0.-.-.not a
-00014f00: 6e61 6c79 7a61 626c 6509 6c6f 7709 4252  nalyzable.low.BR
-00014f10: 4146 092d 092d 092d 092d 092d 092d 092d  AF.-.-.-.-.-.-.-
-00014f20: 0942 5241 4622 2920 2023 206e 6f71 610a  .BRAF")  # noqa.
-00014f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014f40: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-00014f50: 756c 745b 345d 2e72 7374 7269 7028 292c  ult[4].rstrip(),
-00014f60: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
-00014f70: 3030 372e 3133 0931 3136 3431 3230 3433  007.13.116412043
-00014f80: 0931 3136 3431 3230 3433 092d 092d 0931  .116412043.-.-.1
-00014f90: 2d68 6f74 7370 6f74 0930 092d 092d 096e  -hotspot.0.-.-.n
-00014fa0: 6f74 2061 6e61 6c79 7a61 626c 6509 6c6f  ot analyzable.lo
-00014fb0: 7709 4d45 5409 2d09 2d09 2d09 2d09 2d09  w.MET.-.-.-.-.-.
-00014fc0: 2d09 2d09 4d45 5422 2920 2023 206e 6f71  -.-.MET")  # noq
-00014fd0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00014fe0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00014ff0: 6573 756c 745b 355d 2e72 7374 7269 7028  esult[5].rstrip(
-00015000: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
-00015010: 3030 3030 322e 3131 0932 3934 3435 3237  00002.11.2944527
-00015020: 3209 3239 3434 3532 3732 092d 092d 0933  2.29445272.-.-.3
-00015030: 2d63 6865 636b 0932 3231 092d 092d 0979  -check.221.-.-.y
-00015040: 6573 096c 6f77 0941 4c4b 092d 092d 092d  es.low.ALK.-.-.-
-00015050: 092d 092d 092d 092d 0941 4c4b 2229 2020  .-.-.-.-.ALK")  
-00015060: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00015070: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00015080: 7561 6c28 7265 7375 6c74 5b36 5d2e 7273  ual(result[6].rs
-00015090: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
-000150a0: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
-000150b0: 3434 3532 3737 0932 3934 3435 3237 3709  445277.29445277.
-000150c0: 2d09 2d09 332d 6368 6563 6b09 3138 3209  -.-.3-check.182.
-000150d0: 2d09 2d09 7965 7309 6c6f 7709 414c 4b09  -.-.yes.low.ALK.
-000150e0: 2d09 2d09 2d09 2d09 2d09 2d09 2d09 414c  -.-.-.-.-.-.-.AL
-000150f0: 4b22 2920 2023 206e 6f71 610a 2020 2020  K")  # noqa.    
-00015100: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00015110: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-00015120: 375d 2e72 7374 7269 7028 292c 2022 7361  7].rstrip(), "sa
-00015130: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
-00015140: 3131 0931 3435 3733 3837 3638 0931 3435  11.145738768.145
-00015150: 3733 3837 3638 0947 0943 0933 2d63 6865  738768.G.C.3-che
-00015160: 636b 0931 3534 3709 3509 3237 0979 6573  ck.1547.5.27.yes
-00015170: 096f 6b09 4c52 5243 3134 094e 4d5f 3030  .ok.LRRC14.NM_00
-00015180: 3132 3732 3033 362e 3109 2d09 7072 6f74  1272036.1.-.prot
-00015190: 6569 6e5f 636f 6469 6e67 0975 7073 7472  ein_coding.upstr
-000151a0: 6561 6d5f 6765 6e65 5f76 6172 6961 6e74  eam_gene_variant
-000151b0: 0976 6172 6469 6374 092d 092d 092d 2229  .vardict.-.-.-")
-000151c0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
-000151d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000151e0: 4571 7561 6c28 7265 7375 6c74 5b38 5d2e  Equal(result[8].
-000151f0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
-00015200: 6531 094e 435f 3030 3030 3038 2e31 3109  e1.NC_000008.11.
-00015210: 3134 3537 3338 3737 3609 3134 3537 3338  145738776.145738
-00015220: 3737 3609 2d09 2d09 332d 6368 6563 6b09  776.-.-.3-check.
-00015230: 3009 2d09 2d09 6e6f 7420 616e 616c 797a  0.-.-.not analyz
-00015240: 6162 6c65 096c 6f77 092d 092d 092d 092d  able.low.-.-.-.-
-00015250: 092d 092d 092d 092d 092d 2229 2020 2320  .-.-.-.-.-")  # 
-00015260: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00015270: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00015280: 6c28 7265 7375 6c74 5b39 5d2e 7273 7472  l(result[9].rstr
-00015290: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
-000152a0: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
-000152b0: 3432 3531 3409 3134 3537 3432 3531 3409  42514.145742514.
-000152c0: 4109 4709 332d 6368 6563 6b09 3009 3009  A.G.3-check.0.0.
-000152d0: 3833 3909 6e6f 7420 616e 616c 797a 6162  839.not analyzab
-000152e0: 6c65 096c 6f77 0952 4543 514c 3409 4e4d  le.low.RECQL4.NM
-000152f0: 5f30 3034 3236 302e 3309 5072 6f39 3209  _004260.3.Pro92.
-00015300: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-00015310: 796e 6f6e 796d 6f75 735f 7661 7269 616e  ynonymous_varian
-00015320: 7409 7661 7264 6963 742c 6d75 7465 6374  t.vardict,mutect
-00015330: 3209 2d09 2d09 2d22 2920 2023 206e 6f71  2.-.-.-")  # noq
-00015340: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-00015350: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00015360: 6573 756c 745b 3130 5d2e 7273 7472 6970  esult[10].rstrip
-00015370: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
-00015380: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
-00015390: 3839 0938 3139 3534 3738 3909 4309 4754  89.81954789.C.GT
-000153a0: 0932 2d69 6e64 656c 0931 3134 3409 3131  .2-indel.1144.11
-000153b0: 3732 0932 3909 7965 7309 6f6b 0950 4c43  72.29.yes.ok.PLC
-000153c0: 4732 094e 4d5f 3030 3236 3631 2e33 092d  G2.NM_002661.3.-
-000153d0: 0970 726f 7465 696e 5f63 6f64 696e 6709  .protein_coding.
-000153e0: 696e 7472 6f6e 5f76 6172 6961 6e74 0976  intron_variant.v
-000153f0: 6172 6469 6374 092d 092d 092d 2229 2020  ardict.-.-.-")  
-00015400: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00015410: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00015420: 7561 6c28 7265 7375 6c74 5b31 315d 2e72  ual(result[11].r
-00015430: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
-00015440: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
-00015450: 3934 3435 3238 3209 3239 3434 3532 3832  9445282.29445282
-00015460: 0947 0941 0934 2d6f 7468 6572 0935 3230  .G.A.4-other.520
-00015470: 0932 3834 0933 0979 6573 096f 6b09 414c  .284.3.yes.ok.AL
-00015480: 4b09 4e4d 5f30 3034 3330 342e 3409 2d09  K.NM_004304.4.-.
-00015490: 7072 6f74 6569 6e5f 636f 6469 6e67 0973  protein_coding.s
-000154a0: 706c 6963 655f 7265 6769 6f6e 5f76 6172  plice_region_var
-000154b0: 6961 6e74 2669 6e74 726f 6e5f 7661 7269  iant&intron_vari
-000154c0: 616e 7409 7661 7264 6963 7409 2d09 2d09  ant.vardict.-.-.
-000154d0: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
-000154e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000154f0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
-00015500: 3132 5d2e 7273 7472 6970 2829 2c20 2273  12].rstrip(), "s
-00015510: 616d 706c 6531 094e 435f 3030 3030 3136  ample1.NC_000016
-00015520: 2e31 3109 3831 3935 3437 3839 0938 3139  .11.81954789.819
-00015530: 3534 3738 3909 4309 4709 342d 6f74 6865  54789.C.G.4-othe
-00015540: 7209 3131 3434 0934 3432 0933 3439 0979  r.1144.442.349.y
-00015550: 6573 096f 6b09 5345 5054 094e 4d5f 3030  es.ok.SEPT.NM_00
-00015560: 3236 3631 2e33 092d 0970 726f 7465 696e  2661.3.-.protein
-00015570: 5f63 6f64 696e 6709 696e 7472 6f6e 5f76  _coding.intron_v
-00015580: 6172 6961 6e74 0976 6172 6469 6374 2c6d  ariant.vardict,m
-00015590: 7574 6563 7432 092d 092d 092d 2229 2020  utect2.-.-.-")  
-000155a0: 2320 6e6f 7161 0a0a 0a69 6620 5f5f 6e61  # noqa...if __na
-000155b0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
-000155c0: 5f27 3a0a 2020 2020 696d 706f 7274 206c  _':.    import l
-000155d0: 6f67 6769 6e67 0a20 2020 2069 6d70 6f72  ogging.    impor
-000155e0: 7420 7379 730a 2020 2020 6c6f 6767 696e  t sys.    loggin
-000155f0: 672e 6261 7369 6343 6f6e 6669 6728 6c65  g.basicConfig(le
-00015600: 7665 6c3d 6c6f 6767 696e 672e 4352 4954  vel=logging.CRIT
-00015610: 4943 414c 2c20 7374 7265 616d 3d73 7973  ICAL, stream=sys
-00015620: 2e73 7464 6f75 742c 2066 6f72 6d61 743d  .stdout, format=
-00015630: 2725 286d 6573 7361 6765 2973 2729 0a20  '%(message)s'). 
-00015640: 2020 2075 6e69 7474 6573 742e 6d61 696e     unittest.main
-00015650: 2829 0a                                  ().
+00013bb0: 2020 6c65 7665 6c73 2c0a 2020 2020 2020    levels,.      
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00013be0: 6f74 7370 6f74 2c0a 2020 2020 2020 2020  otspot,.        
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 2020 2020 2020 7365 6c66 2e76 6366          self.vcf
+00013c10: 5f76 6570 202b 2022 2e67 7a22 2c0a 2020  _vep + ".gz",.  
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013c40: 6c66 2e67 7663 6620 2b20 222e 677a 222c  lf.gvcf + ".gz",
+00013c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2073 656c 662e 7265 6665 7265 6e63 652c   self.reference,
+00013c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ca0: 2073 656c 662e 7663 665f 7665 705f 776f   self.vcf_vep_wo
+00013cb0: 5f70 6963 6b20 2b20 222e 677a 222c 0a20  _pick + ".gz",. 
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013ce0: 7465 7374 732f 7574 696c 732f 6669 6c65  tests/utils/file
+00013cf0: 732f 7265 706f 7274 5f63 6f6c 756d 6e73  s/report_columns
+00013d00: 5f76 6570 5f72 6567 6578 5f65 7874 7261  _vep_regex_extra
+00013d10: 6374 2e79 616d 6c22 290a 2020 2020 2020  ct.yaml").      
+00013d20: 2020 7769 7468 206f 7065 6e28 7265 706f    with open(repo
+00013d30: 7274 2c20 2772 2729 2061 7320 7265 706f  rt, 'r') as repo
+00013d40: 7274 5f72 6573 756c 743a 0a20 2020 2020  rt_result:.     
+00013d50: 2020 2020 2020 2068 6561 6420 3d20 7265         head = re
+00013d60: 706f 7274 5f72 6573 756c 742e 7265 6164  port_result.read
+00013d70: 6c69 6e65 2829 0a20 2020 2020 2020 2020  line().         
+00013d80: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00013d90: 7561 6c28 6865 6164 2e72 7374 7269 7028  ual(head.rstrip(
+00013da0: 292c 2022 5c74 222e 6a6f 696e 285b 2273  ), "\t".join(["s
+00013db0: 616d 706c 6522 2c20 2263 6872 222c 2022  ample", "chr", "
+00013dc0: 7374 6172 7422 2c20 2273 746f 7022 2c20  start", "stop", 
+00013dd0: 2272 6566 222c 2022 616c 7422 2c20 2272  "ref", "alt", "r
+00013de0: 6570 6f72 7422 2c20 2767 7663 665f 6465  eport", 'gvcf_de
+00013df0: 7074 6827 2c20 2772 6566 5f64 6570 7468  pth', 'ref_depth
+00013e00: 272c 2027 616c 745f 6465 7074 6827 2c20  ', 'alt_depth', 
+00013e10: 2772 7327 5d29 2920 2023 206e 6f71 610a  'rs']))  # noqa.
+00013e20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00013e30: 6c74 203d 2072 6570 6f72 745f 7265 7375  lt = report_resu
+00013e40: 6c74 2e72 6561 646c 696e 6573 2829 0a20  lt.readlines(). 
+00013e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013e60: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00013e70: 7265 7375 6c74 292c 2033 3529 0a20 2020  result), 35).   
+00013e80: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013e90: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00013ea0: 5b30 5d2e 7273 7472 6970 2829 2c20 2273  [0].rstrip(), "s
+00013eb0: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
+00013ec0: 2e31 3109 3239 3434 3532 3731 0932 3934  .11.29445271.294
+00013ed0: 3435 3237 3109 4709 4109 312d 686f 7473  45271.G.A.1-hots
+00013ee0: 706f 7409 3632 3009 3335 3909 3409 2d22  pot.620.359.4.-"
+00013ef0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00013f00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00013f10: 7445 7175 616c 2872 6573 756c 745b 315d  tEqual(result[1]
+00013f20: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00013f30: 6c65 3109 4e43 5f30 3030 3030 372e 3133  le1.NC_000007.13
+00013f40: 0931 3430 3439 3833 3539 0931 3430 3439  .140498359.14049
+00013f50: 3833 3632 0943 5454 5409 4309 322d 696e  8362.CTTT.C.2-in
+00013f60: 6465 6c09 3130 302e 3509 3237 0934 0972  del.100.5.27.4.r
+00013f70: 7331 3237 3434 3630 3137 3722 2920 2023  s1274460177")  #
+00013f80: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00013f90: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00013fa0: 616c 2872 6573 756c 745b 325d 2e72 7374  al(result[2].rst
+00013fb0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00013fc0: 4e43 5f30 3030 3030 372e 3133 0931 3430  NC_000007.13.140
+00013fd0: 3439 3833 3631 0931 3430 3439 3833 3631  498361.140498361
+00013fe0: 092d 092d 0931 2d68 6f74 7370 6f74 0931  .-.-.1-hotspot.1
+00013ff0: 3130 092d 092d 092d 2229 2020 2023 206e  10.-.-.-")   # n
+00014000: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00014010: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014020: 2872 6573 756c 745b 335d 2e72 7374 7269  (result[3].rstri
+00014030: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00014040: 5f30 3030 3030 372e 3133 0931 3430 3435  _000007.13.14045
+00014050: 3331 3336 0931 3430 3435 3331 3336 092d  3136.140453136.-
+00014060: 092d 0931 2d68 6f74 7370 6f74 0930 092d  .-.1-hotspot.0.-
+00014070: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00014080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014090: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+000140a0: 6c74 5b34 5d2e 7273 7472 6970 2829 2c20  lt[4].rstrip(), 
+000140b0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+000140c0: 3037 2e31 3309 3131 3634 3132 3034 3309  07.13.116412043.
+000140d0: 3131 3634 3132 3034 3309 2d09 2d09 312d  116412043.-.-.1-
+000140e0: 686f 7473 706f 7409 3009 2d09 2d09 2d22  hotspot.0.-.-.-"
+000140f0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00014100: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00014110: 7445 7175 616c 2872 6573 756c 745b 355d  tEqual(result[5]
+00014120: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00014130: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
+00014140: 0932 3934 3435 3237 3109 3239 3434 3532  .29445271.294452
+00014150: 3731 092d 092d 0933 2d63 6865 636b 0936  71.-.-.3-check.6
+00014160: 3230 092d 092d 092d 2229 0a20 2020 2020  20.-.-.-").     
+00014170: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014180: 7274 4571 7561 6c28 7265 7375 6c74 5b36  rtEqual(result[6
+00014190: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+000141a0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+000141b0: 3109 3239 3434 3532 3732 0932 3934 3435  1.29445272.29445
+000141c0: 3237 3209 2d09 2d09 332d 6368 6563 6b09  272.-.-.3-check.
+000141d0: 3232 3109 2d09 2d09 2d22 2920 2023 206e  221.-.-.-")  # n
+000141e0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+000141f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014200: 2872 6573 756c 745b 375d 2e72 7374 7269  (result[7].rstri
+00014210: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00014220: 5f30 3030 3030 322e 3131 0932 3934 3435  _000002.11.29445
+00014230: 3237 3309 3239 3434 3532 3733 092d 092d  273.29445273.-.-
+00014240: 0933 2d63 6865 636b 0936 3238 092d 092d  .3-check.628.-.-
+00014250: 092d 2229 0a20 2020 2020 2020 2020 2020  .-").           
+00014260: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00014270: 6c28 7265 7375 6c74 5b38 5d2e 7273 7472  l(result[8].rstr
+00014280: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+00014290: 435f 3030 3030 3032 2e31 3109 3239 3434  C_000002.11.2944
+000142a0: 3532 3734 0932 3934 3435 3237 3409 2d09  5274.29445274.-.
+000142b0: 2d09 332d 6368 6563 6b09 3631 3809 2d09  -.3-check.618.-.
+000142c0: 2d09 2d22 290a 2020 2020 2020 2020 2020  -.-").          
+000142d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000142e0: 616c 2872 6573 756c 745b 395d 2e72 7374  al(result[9].rst
+000142f0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00014300: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+00014310: 3435 3237 3509 3239 3434 3532 3735 092d  45275.29445275.-
+00014320: 092d 0933 2d63 6865 636b 0936 3038 092d  .-.3-check.608.-
+00014330: 092d 092d 2229 0a20 2020 2020 2020 2020  .-.-").         
+00014340: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00014350: 7561 6c28 7265 7375 6c74 5b31 305d 2e72  ual(result[10].r
+00014360: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+00014370: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
+00014380: 3934 3435 3237 3609 3239 3434 3532 3736  9445276.29445276
+00014390: 092d 092d 0933 2d63 6865 636b 0936 3231  .-.-.3-check.621
+000143a0: 092d 092d 092d 2229 0a20 2020 2020 2020  .-.-.-").       
+000143b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000143c0: 4571 7561 6c28 7265 7375 6c74 5b31 315d  Equal(result[11]
+000143d0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+000143e0: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
+000143f0: 0932 3934 3435 3237 3709 3239 3434 3532  .29445277.294452
+00014400: 3737 092d 092d 0933 2d63 6865 636b 0931  77.-.-.3-check.1
+00014410: 3832 092d 092d 092d 2229 2020 2320 6e6f  82.-.-.-")  # no
+00014420: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00014430: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00014440: 7265 7375 6c74 5b31 325d 2e72 7374 7269  result[12].rstri
+00014450: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00014460: 5f30 3030 3030 322e 3131 0932 3934 3435  _000002.11.29445
+00014470: 3237 3809 3239 3434 3532 3738 092d 092d  278.29445278.-.-
+00014480: 0933 2d63 6865 636b 0935 3530 092d 092d  .3-check.550.-.-
+00014490: 092d 2229 0a20 2020 2020 2020 2020 2020  .-").           
+000144a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000144b0: 6c28 7265 7375 6c74 5b31 335d 2e72 7374  l(result[13].rst
+000144c0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+000144d0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+000144e0: 3435 3237 3909 3239 3434 3532 3739 092d  45279.29445279.-
+000144f0: 092d 0933 2d63 6865 636b 0935 3934 092d  .-.3-check.594.-
+00014500: 092d 092d 2229 0a20 2020 2020 2020 2020  .-.-").         
+00014510: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00014520: 7561 6c28 7265 7375 6c74 5b31 345d 2e72  ual(result[14].r
+00014530: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+00014540: 3109 4e43 5f30 3030 3030 322e 3131 0932  1.NC_000002.11.2
+00014550: 3934 3435 3238 3009 3239 3434 3532 3830  9445280.29445280
+00014560: 092d 092d 0933 2d63 6865 636b 0935 3339  .-.-.3-check.539
+00014570: 092d 092d 092d 2229 0a20 2020 2020 2020  .-.-.-").       
+00014580: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00014590: 4571 7561 6c28 7265 7375 6c74 5b31 355d  Equal(result[15]
+000145a0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+000145b0: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
+000145c0: 0932 3934 3435 3238 3109 3239 3434 3532  .29445281.294452
+000145d0: 3831 092d 092d 0933 2d63 6865 636b 0935  81.-.-.3-check.5
+000145e0: 3236 092d 092d 092d 2229 0a20 2020 2020  26.-.-.-").     
+000145f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014600: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
+00014610: 365d 2e72 7374 7269 7028 292c 2022 7361  6].rstrip(), "sa
+00014620: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
+00014630: 3131 0931 3435 3733 3837 3635 0931 3435  11.145738765.145
+00014640: 3733 3837 3635 092d 092d 0933 2d63 6865  738765.-.-.3-che
+00014650: 636b 0931 3631 3609 2d09 2d09 2d22 290a  ck.1616.-.-.-").
+00014660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014670: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00014680: 756c 745b 3137 5d2e 7273 7472 6970 2829  ult[17].rstrip()
+00014690: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+000146a0: 3030 3038 2e31 3109 3134 3537 3338 3736  0008.11.14573876
+000146b0: 3609 3134 3537 3338 3736 3609 2d09 2d09  6.145738766.-.-.
+000146c0: 332d 6368 6563 6b09 3136 3139 092d 092d  3-check.1619.-.-
+000146d0: 092d 2229 0a20 2020 2020 2020 2020 2020  .-").           
+000146e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000146f0: 6c28 7265 7375 6c74 5b31 385d 2e72 7374  l(result[18].rst
+00014700: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00014710: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+00014720: 3733 3837 3637 0931 3435 3733 3837 3637  738767.145738767
+00014730: 092d 092d 0933 2d63 6865 636b 0931 3539  .-.-.3-check.159
+00014740: 3509 2d09 2d09 2d22 290a 2020 2020 2020  5.-.-.-").      
+00014750: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00014760: 7445 7175 616c 2872 6573 756c 745b 3139  tEqual(result[19
+00014770: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00014780: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+00014790: 3109 3134 3537 3338 3736 3809 3134 3537  1.145738768.1457
+000147a0: 3338 3736 3809 4709 4309 332d 6368 6563  38768.G.C.3-chec
+000147b0: 6b09 3135 3437 0935 0932 3709 7273 3131  k.1547.5.27.rs11
+000147c0: 3334 3838 3032 3222 2920 2023 206e 6f71  3488022")  # noq
+000147d0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000147e0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000147f0: 6573 756c 745b 3230 5d2e 7273 7472 6970  esult[20].rstrip
+00014800: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00014810: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
+00014820: 3736 3909 3134 3537 3338 3736 3909 2d09  769.145738769.-.
+00014830: 2d09 332d 6368 6563 6b09 3136 3434 092d  -.3-check.1644.-
+00014840: 092d 092d 2229 0a20 2020 2020 2020 2020  .-.-").         
+00014850: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00014860: 7561 6c28 7265 7375 6c74 5b32 315d 2e72  ual(result[21].r
+00014870: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+00014880: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
+00014890: 3435 3733 3837 3730 0931 3435 3733 3837  45738770.1457387
+000148a0: 3730 092d 092d 0933 2d63 6865 636b 0931  70.-.-.3-check.1
+000148b0: 3636 3709 2d09 2d09 2d22 290a 2020 2020  667.-.-.-").    
+000148c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000148d0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+000148e0: 3232 5d2e 7273 7472 6970 2829 2c20 2273  22].rstrip(), "s
+000148f0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+00014900: 2e31 3109 3134 3537 3338 3737 3109 3134  .11.145738771.14
+00014910: 3537 3338 3737 3109 2d09 2d09 332d 6368  5738771.-.-.3-ch
+00014920: 6563 6b09 3136 3835 092d 092d 092d 2229  eck.1685.-.-.-")
+00014930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014940: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00014950: 7375 6c74 5b32 335d 2e72 7374 7269 7028  sult[23].rstrip(
+00014960: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+00014970: 3030 3030 382e 3131 0931 3435 3733 3837  00008.11.1457387
+00014980: 3732 0931 3435 3733 3837 3732 092d 092d  72.145738772.-.-
+00014990: 0933 2d63 6865 636b 0931 3638 3909 2d09  .3-check.1689.-.
+000149a0: 2d09 2d22 290a 2020 2020 2020 2020 2020  -.-").          
+000149b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000149c0: 616c 2872 6573 756c 745b 3234 5d2e 7273  al(result[24].rs
+000149d0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+000149e0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+000149f0: 3537 3338 3737 3309 3134 3537 3338 3737  5738773.14573877
+00014a00: 3309 2d09 2d09 332d 6368 6563 6b09 3139  3.-.-.3-check.19
+00014a10: 3430 092d 092d 092d 2229 0a20 2020 2020  40.-.-.-").     
+00014a20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014a30: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
+00014a40: 355d 2e72 7374 7269 7028 292c 2022 7361  5].rstrip(), "sa
+00014a50: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
+00014a60: 3131 0931 3435 3733 3837 3734 0931 3435  11.145738774.145
+00014a70: 3733 3837 3734 092d 092d 0933 2d63 6865  738774.-.-.3-che
+00014a80: 636b 0931 3934 3009 2d09 2d09 2d22 290a  ck.1940.-.-.-").
+00014a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014aa0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00014ab0: 756c 745b 3236 5d2e 7273 7472 6970 2829  ult[26].rstrip()
+00014ac0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00014ad0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00014ae0: 3509 3134 3537 3338 3737 3509 2d09 2d09  5.145738775.-.-.
+00014af0: 332d 6368 6563 6b09 3139 3633 092d 092d  3-check.1963.-.-
+00014b00: 092d 2229 0a20 2020 2020 2020 2020 2020  .-").           
+00014b10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00014b20: 6c28 7265 7375 6c74 5b32 375d 2e72 7374  l(result[27].rst
+00014b30: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00014b40: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+00014b50: 3733 3837 3736 0931 3435 3733 3837 3736  738776.145738776
+00014b60: 092d 092d 0933 2d63 6865 636b 0930 092d  .-.-.3-check.0.-
+00014b70: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00014b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014b90: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00014ba0: 6c74 5b32 385d 2e72 7374 7269 7028 292c  lt[28].rstrip(),
+00014bb0: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+00014bc0: 3030 382e 3131 0931 3435 3733 3837 3737  008.11.145738777
+00014bd0: 0931 3435 3733 3837 3737 092d 092d 0933  .145738777.-.-.3
+00014be0: 2d63 6865 636b 0931 3936 3409 2d09 2d09  -check.1964.-.-.
+00014bf0: 2d22 290a 2020 2020 2020 2020 2020 2020  -").            
+00014c00: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014c10: 2872 6573 756c 745b 3239 5d2e 7273 7472  (result[29].rstr
+00014c20: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+00014c30: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
+00014c40: 3338 3737 3809 3134 3537 3338 3737 3809  38778.145738778.
+00014c50: 2d09 2d09 332d 6368 6563 6b09 3139 3633  -.-.3-check.1963
+00014c60: 092d 092d 092d 2229 0a20 2020 2020 2020  .-.-.-").       
+00014c70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00014c80: 4571 7561 6c28 7265 7375 6c74 5b33 305d  Equal(result[30]
+00014c90: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00014ca0: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00014cb0: 0931 3435 3733 3837 3739 0931 3435 3733  .145738779.14573
+00014cc0: 3837 3739 092d 092d 0933 2d63 6865 636b  8779.-.-.3-check
+00014cd0: 0931 3935 3809 2d09 2d09 2d22 290a 2020  .1958.-.-.-").  
+00014ce0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00014cf0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00014d00: 745b 3331 5d2e 7273 7472 6970 2829 2c20  t[31].rstrip(), 
+00014d10: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+00014d20: 3038 2e31 3109 3134 3537 3432 3531 3409  08.11.145742514.
+00014d30: 3134 3537 3432 3531 3409 4109 4709 332d  145742514.A.G.3-
+00014d40: 6368 6563 6b09 3009 3009 3833 3909 7273  check.0.0.839.rs
+00014d50: 3237 3231 3139 3022 2920 2023 206e 6f71  2721190")  # noq
+00014d60: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00014d70: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00014d80: 6573 756c 745b 3332 5d2e 7273 7472 6970  esult[32].rstrip
+00014d90: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00014da0: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
+00014db0: 3839 0938 3139 3534 3738 3909 4309 4754  89.81954789.C.GT
+00014dc0: 0932 2d69 6e64 656c 0931 3134 3409 3131  .2-indel.1144.11
+00014dd0: 3732 0932 3909 2d22 2920 2023 206e 6f71  72.29.-")  # noq
+00014de0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00014df0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00014e00: 6573 756c 745b 3333 5d2e 7273 7472 6970  esult[33].rstrip
+00014e10: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00014e20: 3030 3030 3032 2e31 3109 3239 3434 3532  000002.11.294452
+00014e30: 3832 0932 3934 3435 3238 3209 4709 4109  82.29445282.G.A.
+00014e40: 342d 6f74 6865 7209 3532 3009 3238 3409  4-other.520.284.
+00014e50: 3309 7273 3133 3035 3138 3331 3530 2229  3.rs1305183150")
+00014e60: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00014e70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00014e80: 4571 7561 6c28 7265 7375 6c74 5b33 345d  Equal(result[34]
+00014e90: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00014ea0: 6c65 3109 4e43 5f30 3030 3031 362e 3131  le1.NC_000016.11
+00014eb0: 0938 3139 3534 3738 3909 3831 3935 3437  .81954789.819547
+00014ec0: 3839 0943 0947 0934 2d6f 7468 6572 0931  89.C.G.4-other.1
+00014ed0: 3134 3409 3434 3209 3334 3909 7273 3132  144.442.349.rs12
+00014ee0: 3434 3631 3237 2229 2020 2320 6e6f 7161  446127")  # noqa
+00014ef0: 0a0a 2020 2020 6465 6620 7465 7374 5f66  ..    def test_f
+00014f00: 696c 7465 7265 645f 6d75 7461 7469 6f6e  iltered_mutation
+00014f10: 5f63 6f6d 6269 6e65 5f63 6f6c 756d 6e73  _combine_columns
+00014f20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014f30: 6672 6f6d 2068 7964 7261 5f67 656e 6574  from hydra_genet
+00014f40: 6963 732e 7574 696c 732e 696f 2e68 6f74  ics.utils.io.hot
+00014f50: 7370 6f74 5f72 6570 6f72 7420 696d 706f  spot_report impo
+00014f60: 7274 2067 656e 6572 6174 655f 686f 7473  rt generate_hots
+00014f70: 706f 745f 7265 706f 7274 0a20 2020 2020  pot_report.     
+00014f80: 2020 206c 6576 656c 7320 3d20 5b28 3330     levels = [(30
+00014f90: 302c 2022 6f6b 222c 2022 7965 7322 292c  0, "ok", "yes"),
+00014fa0: 2028 3330 2c20 226c 6f77 222c 2022 7965   (30, "low", "ye
+00014fb0: 7322 292c 2028 302c 2022 6c6f 7722 2c20  s"), (0, "low", 
+00014fc0: 226e 6f74 2061 6e61 6c79 7a61 626c 6522  "not analyzable"
+00014fd0: 295d 0a0a 2020 2020 2020 2020 7365 6c66  )]..        self
+00014fe0: 2e6d 6178 4469 6666 203d 2031 3030 3030  .maxDiff = 10000
+00014ff0: 0a0a 2020 2020 2020 2020 7265 706f 7274  ..        report
+00015000: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00015010: 7365 6c66 2e74 656d 7064 6972 2c20 2266  self.tempdir, "f
+00015020: 696c 7465 7265 642e 7265 706f 7274 2229  iltered.report")
+00015030: 0a20 2020 2020 2020 2067 656e 6572 6174  .        generat
+00015040: 655f 686f 7473 706f 745f 7265 706f 7274  e_hotspot_report
+00015050: 2822 7361 6d70 6c65 3122 2c0a 2020 2020  ("sample1",.    
+00015060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015070: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00015080: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150a0: 2020 2020 6c65 7665 6c73 2c0a 2020 2020      levels,.    
+000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000150d0: 2e68 6f74 7370 6f74 2c0a 2020 2020 2020  .hotspot,.      
+000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150f0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+00015100: 6366 5f76 6570 202b 2022 2e67 7a22 2c0a  cf_vep + ".gz",.
+00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015130: 7365 6c66 2e67 7663 6620 2b20 222e 677a  self.gvcf + ".gz
+00015140: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 2020 2073 656c 662e 7265 6665 7265 6e63     self.referenc
+00015170: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 2073 656c 662e 7663 665f 7665 705f     self.vcf_vep_
+000151a0: 776f 5f70 6963 6b20 2b20 222e 677a 2229  wo_pick + ".gz")
+000151b0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+000151c0: 7844 6966 6620 3d20 3130 3030 300a 0a20  xDiff = 10000.. 
+000151d0: 2020 2020 2020 2023 2056 6172 6961 6e74         # Variant
+000151e0: 730a 2020 2020 2020 2020 2320 6368 7232  s.        # chr2
+000151f0: 0932 3934 3435 3237 3109 2e09 4709 4120  .29445271...G.A 
+00015200: 2028 3129 0a20 2020 2020 2020 2023 2063   (1).        # c
+00015210: 6872 3209 3239 3434 3532 3832 092e 0947  hr2.29445282...G
+00015220: 0941 2020 286f 7468 6572 290a 2020 2020  .A  (other).    
+00015230: 2020 2020 2320 6368 7237 0931 3430 3439      # chr7.14049
+00015240: 3833 3539 092e 0943 5454 5409 4320 2833  8359...CTTT.C (3
+00015250: 290a 2020 2020 2020 2020 2320 6368 7238  ).        # chr8
+00015260: 0931 3435 3733 3837 3638 092e 0947 0943  .145738768...G.C
+00015270: 2028 3629 0a20 2020 2020 2020 2023 2063   (6).        # c
+00015280: 6872 3809 3134 3537 3432 3531 3409 2e09  hr8.145742514...
+00015290: 4109 470a 2020 2020 2020 2020 2320 6368  A.G.        # ch
+000152a0: 7231 3620 3831 3935 3437 3839 092e 0943  r16 81954789...C
+000152b0: 0947 540a 2020 2020 2020 2020 2320 6368  .GT.        # ch
+000152c0: 7231 3609 3831 3935 3437 3839 092e 0943  r16.81954789...C
+000152d0: 0947 0a20 2020 2020 2020 2023 0a20 2020  .G.        #.   
+000152e0: 2020 2020 2023 2048 6f74 7370 6f74 0a20       # Hotspot. 
+000152f0: 2020 2020 2020 2023 2031 202d 204e 435f         # 1 - NC_
+00015300: 3030 3030 3032 2e31 3120 2032 3934 3435  000002.11  29445
+00015310: 3237 3120 2020 2032 3934 3435 3237 3120  271    29445271 
+00015320: 2020 2068 6f74 7370 6f74 0a20 2020 2020     hotspot.     
+00015330: 2020 2023 2032 202d 204e 435f 3030 3030     # 2 - NC_0000
+00015340: 3032 2e31 3120 2032 3934 3435 3237 3120  02.11  29445271 
+00015350: 2020 2032 3934 3435 3238 3120 2020 2072     29445281    r
+00015360: 6567 696f 6e5f 616c 6c0a 2020 2020 2020  egion_all.      
+00015370: 2020 2320 3320 2d20 4e43 5f30 3030 3030    # 3 - NC_00000
+00015380: 372e 3133 2020 3134 3034 3938 3336 3120  7.13  140498361 
+00015390: 2020 3134 3034 3938 3336 3120 2020 686f    140498361   ho
+000153a0: 7473 706f 7420 2023 2053 686f 756c 6420  tspot  # Should 
+000153b0: 7468 6973 206f 6e65 2062 6520 7072 696e  this one be prin
+000153c0: 7465 6420 6576 656e 7468 6f75 6768 2061  ted eventhough a
+000153d0: 2069 6e64 656c 206f 7665 726c 6170 7320   indel overlaps 
+000153e0: 6974 3f0a 2020 2020 2020 2020 2320 3420  it?.        # 4 
+000153f0: 2d20 4e43 5f30 3030 3030 372e 3133 2020  - NC_000007.13  
+00015400: 3134 3034 3533 3133 3620 2020 3134 3034  140453136   1404
+00015410: 3533 3133 3620 2020 686f 7473 706f 740a  53136   hotspot.
+00015420: 2020 2020 2020 2020 2320 3520 2d20 4e43          # 5 - NC
+00015430: 5f30 3030 3030 372e 3133 2020 3131 3634  _000007.13  1164
+00015440: 3132 3034 3320 2020 3131 3634 3132 3034  12043   11641204
+00015450: 3320 2020 686f 7473 706f 740a 2020 2020  3   hotspot.    
+00015460: 2020 2020 2320 3620 2d20 4e43 5f30 3030      # 6 - NC_000
+00015470: 3030 382e 3131 2020 3134 3537 3338 3736  008.11  14573876
+00015480: 3520 2020 2031 3435 3733 3837 3739 2020  5    145738779  
+00015490: 2020 7265 6769 6f6e 5f61 6c6c 0a20 2020    region_all.   
+000154a0: 2020 2020 2023 2037 202d 204e 435f 3030       # 7 - NC_00
+000154b0: 3030 3038 2e31 3120 2031 3435 3734 3235  0008.11  1457425
+000154c0: 3130 2020 2020 3134 3537 3432 3532 3420  10    145742524 
+000154d0: 2020 2072 6567 696f 6e0a 2020 2020 2020     region.      
+000154e0: 2020 2320 3820 2d20 4e43 5f30 3030 3031    # 8 - NC_00001
+000154f0: 362e 3131 2020 3831 3935 3437 3835 2020  6.11  81954785  
+00015500: 2020 3831 3935 3437 3935 2020 2020 696e    81954795    in
+00015510: 6465 6c0a 2020 2020 2020 2020 230a 2020  del.        #.  
+00015520: 2020 2020 2020 7265 706f 7274 203d 206f        report = o
+00015530: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+00015540: 2e74 656d 7064 6972 2c20 2266 696c 7465  .tempdir, "filte
+00015550: 7265 642e 7265 706f 7274 2229 0a20 2020  red.report").   
+00015560: 2020 2020 2067 656e 6572 6174 655f 686f       generate_ho
+00015570: 7473 706f 745f 7265 706f 7274 2822 7361  tspot_report("sa
+00015580: 6d70 6c65 3122 2c0a 2020 2020 2020 2020  mple1",.        
+00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155a0: 2020 2020 2020 2020 7265 706f 7274 2c0a          report,.
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155d0: 6c65 7665 6c73 2c0a 2020 2020 2020 2020  levels,.        
+000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155f0: 2020 2020 2020 2020 7365 6c66 2e68 6f74          self.hot
+00015600: 7370 6f74 2c0a 2020 2020 2020 2020 2020  spot,.          
+00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015620: 2020 2020 2020 7365 6c66 2e76 6366 5f76        self.vcf_v
+00015630: 6570 202b 2022 2e67 7a22 2c0a 2020 2020  ep + ".gz",.    
+00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015660: 2e67 7663 6620 2b20 222e 677a 222c 0a20  .gvcf + ".gz",. 
+00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015690: 656c 662e 7265 6665 7265 6e63 652c 0a20  elf.reference,. 
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000156c0: 656c 662e 7663 665f 7665 705f 776f 5f70  elf.vcf_vep_wo_p
+000156d0: 6963 6b20 2b20 222e 677a 222c 0a20 2020  ick + ".gz",.   
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156f0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+00015700: 7374 732f 7574 696c 732f 6669 6c65 732f  sts/utils/files/
+00015710: 7265 706f 7274 5f63 6f6c 756d 6e73 5f63  report_columns_c
+00015720: 6f6d 6269 6e65 5f63 6f6c 756d 6e73 2e79  ombine_columns.y
+00015730: 616d 6c22 290a 2020 2020 2020 2020 7769  aml").        wi
+00015740: 7468 206f 7065 6e28 7265 706f 7274 2c20  th open(report, 
+00015750: 2772 2729 2061 7320 7265 706f 7274 5f72  'r') as report_r
+00015760: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+00015770: 2020 2068 6561 6420 3d20 7265 706f 7274     head = report
+00015780: 5f72 6573 756c 742e 7265 6164 6c69 6e65  _result.readline
+00015790: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+000157a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000157b0: 6865 6164 2e72 7374 7269 7028 292c 2022  head.rstrip(), "
+000157c0: 5c74 222e 6a6f 696e 285b 2273 616d 706c  \t".join(["sampl
+000157d0: 6522 2c20 2263 6872 222c 2022 7374 6172  e", "chr", "star
+000157e0: 7422 2c20 2273 746f 7022 2c20 2272 6566  t", "stop", "ref
+000157f0: 222c 2022 616c 7422 2c20 2272 6570 6f72  ", "alt", "repor
+00015800: 7422 2c20 2767 7663 665f 6465 7074 6827  t", 'gvcf_depth'
+00015810: 2c20 2272 6566 5f64 6570 7468 222c 2022  , "ref_depth", "
+00015820: 616c 745f 6465 7074 6822 2c20 2741 6e61  alt_depth", 'Ana
+00015830: 6c79 7a61 626c 6527 2c20 274d 696e 5f72  lyzable', 'Min_r
+00015840: 6561 645f 6465 7074 6833 3030 272c 2027  ead_depth300', '
+00015850: 4765 6e65 5f76 6570 3b68 6f74 7370 6f74  Gene_vep;hotspot
+00015860: 272c 2027 5661 7269 616e 745f 7479 7065  ', 'Variant_type
+00015870: 272c 2027 436f 6e73 6571 7565 6e63 6527  ', 'Consequence'
+00015880: 2c20 2743 616c 6c65 7273 272c 2027 436f  , 'Callers', 'Co
+00015890: 6d6d 656e 7427 5d29 2920 2023 206e 6f71  mment']))  # noq
+000158a0: 610a 2020 2020 2020 2020 2020 2020 7265  a.            re
+000158b0: 7375 6c74 203d 2072 6570 6f72 745f 7265  sult = report_re
+000158c0: 7375 6c74 2e72 6561 646c 696e 6573 2829  sult.readlines()
+000158d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000158e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+000158f0: 6e28 7265 7375 6c74 292c 2033 3529 0a20  n(result), 35). 
+00015900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015910: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00015920: 6c74 5b30 5d2e 7273 7472 6970 2829 2c20  lt[0].rstrip(), 
+00015930: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+00015940: 3032 2e31 3109 3239 3434 3532 3731 0932  02.11.29445271.2
+00015950: 3934 3435 3237 3109 4709 4109 312d 686f  9445271.G.A.1-ho
+00015960: 7473 706f 7409 3632 3009 3335 392e 3030  tspot.620.359.00
+00015970: 0934 0979 6573 096f 6b09 414c 4b3b 414c  .4.yes.ok.ALK;AL
+00015980: 4b09 7072 6f74 6569 6e5f 636f 6469 6e67  K.protein_coding
+00015990: 0973 796e 6f6e 796d 6f75 735f 7661 7269  .synonymous_vari
+000159a0: 616e 7409 7661 7264 6963 7409 7265 7369  ant.vardict.resi
+000159b0: 7374 616e 6365 5f6d 7574 6174 696f 6e22  stance_mutation"
+000159c0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+000159d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000159e0: 7445 7175 616c 2872 6573 756c 745b 315d  tEqual(result[1]
+000159f0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00015a00: 6c65 3109 4e43 5f30 3030 3030 372e 3133  le1.NC_000007.13
+00015a10: 0931 3430 3439 3833 3539 0931 3430 3439  .140498359.14049
+00015a20: 3833 3632 0943 5454 5409 4309 322d 696e  8362.CTTT.C.2-in
+00015a30: 6465 6c09 3130 302e 3509 3237 2e30 3009  del.100.5.27.00.
+00015a40: 3409 7965 7309 6c6f 7709 4252 4146 3b45  4.yes.low.BRAF;E
+00015a50: 4746 5209 7072 6f74 6569 6e5f 636f 6469  GFR.protein_codi
+00015a60: 6e67 0969 6e74 726f 6e5f 7661 7269 616e  ng.intron_varian
+00015a70: 7409 6d75 7465 6374 3209 2d22 2920 2023  t.mutect2.-")  #
+00015a80: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00015a90: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00015aa0: 616c 2872 6573 756c 745b 325d 2e72 7374  al(result[2].rst
+00015ab0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00015ac0: 4e43 5f30 3030 3030 372e 3133 0931 3430  NC_000007.13.140
+00015ad0: 3439 3833 3631 0931 3430 3439 3833 3631  498361.140498361
+00015ae0: 092d 092d 0931 2d68 6f74 7370 6f74 0931  .-.-.1-hotspot.1
+00015af0: 3130 092d 092d 0979 6573 096c 6f77 092d  10.-.-.yes.low.-
+00015b00: 3b45 4746 5209 2d09 2d09 2d09 2d22 2920  ;EGFR.-.-.-.-") 
+00015b10: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00015b20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00015b30: 4571 7561 6c28 7265 7375 6c74 5b33 5d2e  Equal(result[3].
+00015b40: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00015b50: 6531 094e 435f 3030 3030 3037 2e31 3309  e1.NC_000007.13.
+00015b60: 3134 3034 3533 3133 3609 3134 3034 3533  140453136.140453
+00015b70: 3133 3609 2d09 2d09 312d 686f 7473 706f  136.-.-.1-hotspo
+00015b80: 7409 3009 2d09 2d09 6e6f 7420 616e 616c  t.0.-.-.not anal
+00015b90: 797a 6162 6c65 096c 6f77 092d 3b42 5241  yzable.low.-;BRA
+00015ba0: 4609 2d09 2d09 2d09 2d22 2920 2023 206e  F.-.-.-.-")  # n
+00015bb0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00015bc0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00015bd0: 2872 6573 756c 745b 345d 2e72 7374 7269  (result[4].rstri
+00015be0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00015bf0: 5f30 3030 3030 372e 3133 0931 3136 3431  _000007.13.11641
+00015c00: 3230 3433 0931 3136 3431 3230 3433 092d  2043.116412043.-
+00015c10: 092d 0931 2d68 6f74 7370 6f74 0930 092d  .-.1-hotspot.0.-
+00015c20: 092d 096e 6f74 2061 6e61 6c79 7a61 626c  .-.not analyzabl
+00015c30: 6509 6c6f 7709 2d3b 4d45 5409 2d09 2d09  e.low.-;MET.-.-.
+00015c40: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00015c50: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015c60: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00015c70: 745b 355d 2e72 7374 7269 7028 292c 2022  t[5].rstrip(), "
+00015c80: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00015c90: 322e 3131 0932 3934 3435 3237 3109 3239  2.11.29445271.29
+00015ca0: 3434 3532 3731 092d 092d 0933 2d63 6865  445271.-.-.3-che
+00015cb0: 636b 0936 3230 092d 092d 0979 6573 096f  ck.620.-.-.yes.o
+00015cc0: 6b09 2d3b 414c 4b09 2d09 2d09 2d09 2d22  k.-;ALK.-.-.-.-"
+00015cd0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00015ce0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00015cf0: 7445 7175 616c 2872 6573 756c 745b 365d  tEqual(result[6]
+00015d00: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00015d10: 6c65 3109 4e43 5f30 3030 3030 322e 3131  le1.NC_000002.11
+00015d20: 0932 3934 3435 3237 3209 3239 3434 3532  .29445272.294452
+00015d30: 3732 092d 092d 0933 2d63 6865 636b 0932  72.-.-.3-check.2
+00015d40: 3231 092d 092d 0979 6573 096c 6f77 092d  21.-.-.yes.low.-
+00015d50: 3b41 4c4b 092d 092d 092d 092d 2229 2020  ;ALK.-.-.-.-")  
+00015d60: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00015d70: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00015d80: 7561 6c28 7265 7375 6c74 5b37 5d2e 7273  ual(result[7].rs
+00015d90: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00015da0: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
+00015db0: 3434 3532 3733 0932 3934 3435 3237 3309  445273.29445273.
+00015dc0: 2d09 2d09 332d 6368 6563 6b09 3632 3809  -.-.3-check.628.
+00015dd0: 2d09 2d09 7965 7309 6f6b 092d 3b41 4c4b  -.-.yes.ok.-;ALK
+00015de0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00015df0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00015e00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00015e10: 7265 7375 6c74 5b38 5d2e 7273 7472 6970  result[8].rstrip
+00015e20: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00015e30: 3030 3030 3032 2e31 3109 3239 3434 3532  000002.11.294452
+00015e40: 3734 0932 3934 3435 3237 3409 2d09 2d09  74.29445274.-.-.
+00015e50: 332d 6368 6563 6b09 3631 3809 2d09 2d09  3-check.618.-.-.
+00015e60: 7965 7309 6f6b 092d 3b41 4c4b 092d 092d  yes.ok.-;ALK.-.-
+00015e70: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00015e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015e90: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00015ea0: 6c74 5b39 5d2e 7273 7472 6970 2829 2c20  lt[9].rstrip(), 
+00015eb0: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+00015ec0: 3032 2e31 3109 3239 3434 3532 3735 0932  02.11.29445275.2
+00015ed0: 3934 3435 3237 3509 2d09 2d09 332d 6368  9445275.-.-.3-ch
+00015ee0: 6563 6b09 3630 3809 2d09 2d09 7965 7309  eck.608.-.-.yes.
+00015ef0: 6f6b 092d 3b41 4c4b 092d 092d 092d 092d  ok.-;ALK.-.-.-.-
+00015f00: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00015f10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00015f20: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
+00015f30: 305d 2e72 7374 7269 7028 292c 2022 7361  0].rstrip(), "sa
+00015f40: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+00015f50: 3131 0932 3934 3435 3237 3609 3239 3434  11.29445276.2944
+00015f60: 3532 3736 092d 092d 0933 2d63 6865 636b  5276.-.-.3-check
+00015f70: 0936 3231 092d 092d 0979 6573 096f 6b09  .621.-.-.yes.ok.
+00015f80: 2d3b 414c 4b09 2d09 2d09 2d09 2d22 2920  -;ALK.-.-.-.-") 
+00015f90: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00015fa0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00015fb0: 7175 616c 2872 6573 756c 745b 3131 5d2e  qual(result[11].
+00015fc0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00015fd0: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
+00015fe0: 3239 3434 3532 3737 0932 3934 3435 3237  29445277.2944527
+00015ff0: 3709 2d09 2d09 332d 6368 6563 6b09 3138  7.-.-.3-check.18
+00016000: 3209 2d09 2d09 7965 7309 6c6f 7709 2d3b  2.-.-.yes.low.-;
+00016010: 414c 4b09 2d09 2d09 2d09 2d22 2920 2023  ALK.-.-.-.-")  #
+00016020: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00016030: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00016040: 616c 2872 6573 756c 745b 3132 5d2e 7273  al(result[12].rs
+00016050: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00016060: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
+00016070: 3434 3532 3738 0932 3934 3435 3237 3809  445278.29445278.
+00016080: 2d09 2d09 332d 6368 6563 6b09 3535 3009  -.-.3-check.550.
+00016090: 2d09 2d09 7965 7309 6f6b 092d 3b41 4c4b  -.-.yes.ok.-;ALK
+000160a0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+000160b0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000160c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000160d0: 7265 7375 6c74 5b31 335d 2e72 7374 7269  result[13].rstri
+000160e0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+000160f0: 5f30 3030 3030 322e 3131 0932 3934 3435  _000002.11.29445
+00016100: 3237 3909 3239 3434 3532 3739 092d 092d  279.29445279.-.-
+00016110: 0933 2d63 6865 636b 0935 3934 092d 092d  .3-check.594.-.-
+00016120: 0979 6573 096f 6b09 2d3b 414c 4b09 2d09  .yes.ok.-;ALK.-.
+00016130: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00016140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016150: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00016160: 756c 745b 3134 5d2e 7273 7472 6970 2829  ult[14].rstrip()
+00016170: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00016180: 3030 3032 2e31 3109 3239 3434 3532 3830  0002.11.29445280
+00016190: 0932 3934 3435 3238 3009 2d09 2d09 332d  .29445280.-.-.3-
+000161a0: 6368 6563 6b09 3533 3909 2d09 2d09 7965  check.539.-.-.ye
+000161b0: 7309 6f6b 092d 3b41 4c4b 092d 092d 092d  s.ok.-;ALK.-.-.-
+000161c0: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+000161d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000161e0: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+000161f0: 5b31 355d 2e72 7374 7269 7028 292c 2022  [15].rstrip(), "
+00016200: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00016210: 322e 3131 0932 3934 3435 3238 3109 3239  2.11.29445281.29
+00016220: 3434 3532 3831 092d 092d 0933 2d63 6865  445281.-.-.3-che
+00016230: 636b 0935 3236 092d 092d 0979 6573 096f  ck.526.-.-.yes.o
+00016240: 6b09 2d3b 414c 4b09 2d09 2d09 2d09 2d22  k.-;ALK.-.-.-.-"
+00016250: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00016260: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00016270: 7445 7175 616c 2872 6573 756c 745b 3136  tEqual(result[16
+00016280: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00016290: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+000162a0: 3109 3134 3537 3338 3736 3509 3134 3537  1.145738765.1457
+000162b0: 3338 3736 3509 2d09 2d09 332d 6368 6563  38765.-.-.3-chec
+000162c0: 6b09 3136 3136 092d 092d 0979 6573 096f  k.1616.-.-.yes.o
+000162d0: 6b09 2d3b 2d09 2d09 2d09 2d09 2d22 2920  k.-;-.-.-.-.-") 
+000162e0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+000162f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00016300: 7175 616c 2872 6573 756c 745b 3137 5d2e  qual(result[17].
+00016310: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00016320: 6531 094e 435f 3030 3030 3038 2e31 3109  e1.NC_000008.11.
+00016330: 3134 3537 3338 3736 3609 3134 3537 3338  145738766.145738
+00016340: 3736 3609 2d09 2d09 332d 6368 6563 6b09  766.-.-.3-check.
+00016350: 3136 3139 092d 092d 0979 6573 096f 6b09  1619.-.-.yes.ok.
+00016360: 2d3b 2d09 2d09 2d09 2d09 2d22 2920 2023  -;-.-.-.-.-")  #
+00016370: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00016380: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00016390: 616c 2872 6573 756c 745b 3138 5d2e 7273  al(result[18].rs
+000163a0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+000163b0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+000163c0: 3537 3338 3736 3709 3134 3537 3338 3736  5738767.14573876
+000163d0: 3709 2d09 2d09 332d 6368 6563 6b09 3135  7.-.-.3-check.15
+000163e0: 3935 092d 092d 0979 6573 096f 6b09 2d3b  95.-.-.yes.ok.-;
+000163f0: 2d09 2d09 2d09 2d09 2d22 2920 2023 206e  -.-.-.-.-")  # n
+00016400: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00016410: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00016420: 2872 6573 756c 745b 3139 5d2e 7273 7472  (result[19].rstr
+00016430: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+00016440: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
+00016450: 3338 3736 3809 3134 3537 3338 3736 3809  38768.145738768.
+00016460: 4709 4309 332d 6368 6563 6b09 3135 3437  G.C.3-check.1547
+00016470: 0935 2e30 3009 3237 0979 6573 096f 6b09  .5.00.27.yes.ok.
+00016480: 4c52 5243 3134 3b2d 0970 726f 7465 696e  LRRC14;-.protein
+00016490: 5f63 6f64 696e 6709 7570 7374 7265 616d  _coding.upstream
+000164a0: 5f67 656e 655f 7661 7269 616e 7409 7661  _gene_variant.va
+000164b0: 7264 6963 7409 2d22 2920 2023 206e 6f71  rdict.-")  # noq
+000164c0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000164d0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000164e0: 6573 756c 745b 3230 5d2e 7273 7472 6970  esult[20].rstrip
+000164f0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00016500: 3030 3030 3038 2e31 3109 3134 3537 3338  000008.11.145738
+00016510: 3736 3909 3134 3537 3338 3736 3909 2d09  769.145738769.-.
+00016520: 2d09 332d 6368 6563 6b09 3136 3434 092d  -.3-check.1644.-
+00016530: 092d 0979 6573 096f 6b09 2d3b 2d09 2d09  .-.yes.ok.-;-.-.
+00016540: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00016550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016560: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00016570: 756c 745b 3231 5d2e 7273 7472 6970 2829  ult[21].rstrip()
+00016580: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00016590: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+000165a0: 3009 3134 3537 3338 3737 3009 2d09 2d09  0.145738770.-.-.
+000165b0: 332d 6368 6563 6b09 3136 3637 092d 092d  3-check.1667.-.-
+000165c0: 0979 6573 096f 6b09 2d3b 2d09 2d09 2d09  .yes.ok.-;-.-.-.
+000165d0: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+000165e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000165f0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00016600: 745b 3232 5d2e 7273 7472 6970 2829 2c20  t[22].rstrip(), 
+00016610: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+00016620: 3038 2e31 3109 3134 3537 3338 3737 3109  08.11.145738771.
+00016630: 3134 3537 3338 3737 3109 2d09 2d09 332d  145738771.-.-.3-
+00016640: 6368 6563 6b09 3136 3835 092d 092d 0979  check.1685.-.-.y
+00016650: 6573 096f 6b09 2d3b 2d09 2d09 2d09 2d09  es.ok.-;-.-.-.-.
+00016660: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+00016670: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00016680: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00016690: 3233 5d2e 7273 7472 6970 2829 2c20 2273  23].rstrip(), "s
+000166a0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+000166b0: 2e31 3109 3134 3537 3338 3737 3209 3134  .11.145738772.14
+000166c0: 3537 3338 3737 3209 2d09 2d09 332d 6368  5738772.-.-.3-ch
+000166d0: 6563 6b09 3136 3839 092d 092d 0979 6573  eck.1689.-.-.yes
+000166e0: 096f 6b09 2d3b 2d09 2d09 2d09 2d09 2d22  .ok.-;-.-.-.-.-"
+000166f0: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00016700: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00016710: 7445 7175 616c 2872 6573 756c 745b 3234  tEqual(result[24
+00016720: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00016730: 706c 6531 094e 435f 3030 3030 3038 2e31  ple1.NC_000008.1
+00016740: 3109 3134 3537 3338 3737 3309 3134 3537  1.145738773.1457
+00016750: 3338 3737 3309 2d09 2d09 332d 6368 6563  38773.-.-.3-chec
+00016760: 6b09 3139 3430 092d 092d 0979 6573 096f  k.1940.-.-.yes.o
+00016770: 6b09 2d3b 2d09 2d09 2d09 2d09 2d22 2920  k.-;-.-.-.-.-") 
+00016780: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00016790: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000167a0: 7175 616c 2872 6573 756c 745b 3235 5d2e  qual(result[25].
+000167b0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+000167c0: 6531 094e 435f 3030 3030 3038 2e31 3109  e1.NC_000008.11.
+000167d0: 3134 3537 3338 3737 3409 3134 3537 3338  145738774.145738
+000167e0: 3737 3409 2d09 2d09 332d 6368 6563 6b09  774.-.-.3-check.
+000167f0: 3139 3430 092d 092d 0979 6573 096f 6b09  1940.-.-.yes.ok.
+00016800: 2d3b 2d09 2d09 2d09 2d09 2d22 2920 2023  -;-.-.-.-.-")  #
+00016810: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00016820: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00016830: 616c 2872 6573 756c 745b 3236 5d2e 7273  al(result[26].rs
+00016840: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00016850: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+00016860: 3537 3338 3737 3509 3134 3537 3338 3737  5738775.14573877
+00016870: 3509 2d09 2d09 332d 6368 6563 6b09 3139  5.-.-.3-check.19
+00016880: 3633 092d 092d 0979 6573 096f 6b09 2d3b  63.-.-.yes.ok.-;
+00016890: 2d09 2d09 2d09 2d09 2d22 2920 2023 206e  -.-.-.-.-")  # n
+000168a0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+000168b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000168c0: 2872 6573 756c 745b 3237 5d2e 7273 7472  (result[27].rstr
+000168d0: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+000168e0: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
+000168f0: 3338 3737 3609 3134 3537 3338 3737 3609  38776.145738776.
+00016900: 2d09 2d09 332d 6368 6563 6b09 3009 2d09  -.-.3-check.0.-.
+00016910: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
+00016920: 096c 6f77 092d 3b2d 092d 092d 092d 092d  .low.-;-.-.-.-.-
+00016930: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00016940: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00016950: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
+00016960: 385d 2e72 7374 7269 7028 292c 2022 7361  8].rstrip(), "sa
+00016970: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
+00016980: 3131 0931 3435 3733 3837 3737 0931 3435  11.145738777.145
+00016990: 3733 3837 3737 092d 092d 0933 2d63 6865  738777.-.-.3-che
+000169a0: 636b 0931 3936 3409 2d09 2d09 7965 7309  ck.1964.-.-.yes.
+000169b0: 6f6b 092d 3b2d 092d 092d 092d 092d 2229  ok.-;-.-.-.-.-")
+000169c0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+000169d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000169e0: 4571 7561 6c28 7265 7375 6c74 5b32 395d  Equal(result[29]
+000169f0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00016a00: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00016a10: 0931 3435 3733 3837 3738 0931 3435 3733  .145738778.14573
+00016a20: 3837 3738 092d 092d 0933 2d63 6865 636b  8778.-.-.3-check
+00016a30: 0931 3936 3309 2d09 2d09 7965 7309 6f6b  .1963.-.-.yes.ok
+00016a40: 092d 3b2d 092d 092d 092d 092d 2229 2020  .-;-.-.-.-.-")  
+00016a50: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00016a60: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00016a70: 7561 6c28 7265 7375 6c74 5b33 305d 2e72  ual(result[30].r
+00016a80: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+00016a90: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
+00016aa0: 3435 3733 3837 3739 0931 3435 3733 3837  45738779.1457387
+00016ab0: 3739 092d 092d 0933 2d63 6865 636b 0931  79.-.-.3-check.1
+00016ac0: 3935 3809 2d09 2d09 7965 7309 6f6b 092d  958.-.-.yes.ok.-
+00016ad0: 3b2d 092d 092d 092d 092d 2229 2020 2320  ;-.-.-.-.-")  # 
+00016ae0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00016af0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016b00: 6c28 7265 7375 6c74 5b33 315d 2e72 7374  l(result[31].rst
+00016b10: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00016b20: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+00016b30: 3734 3235 3134 0931 3435 3734 3235 3134  742514.145742514
+00016b40: 0941 0947 0933 2d63 6865 636b 0930 0930  .A.G.3-check.0.0
+00016b50: 2e30 3009 3833 3909 6e6f 7420 616e 616c  .00.839.not anal
+00016b60: 797a 6162 6c65 096c 6f77 0952 4543 514c  yzable.low.RECQL
+00016b70: 343b 2d09 7072 6f74 6569 6e5f 636f 6469  4;-.protein_codi
+00016b80: 6e67 0973 796e 6f6e 796d 6f75 735f 7661  ng.synonymous_va
+00016b90: 7269 616e 7409 7661 7264 6963 742c 6d75  riant.vardict,mu
+00016ba0: 7465 6374 3209 2d22 2920 2023 206e 6f71  tect2.-")  # noq
+00016bb0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00016bc0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00016bd0: 6573 756c 745b 3332 5d2e 7273 7472 6970  esult[32].rstrip
+00016be0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00016bf0: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
+00016c00: 3839 0938 3139 3534 3738 3909 4309 4754  89.81954789.C.GT
+00016c10: 0932 2d69 6e64 656c 0931 3134 3409 3131  .2-indel.1144.11
+00016c20: 3732 2e30 3009 3239 0979 6573 096f 6b09  72.00.29.yes.ok.
+00016c30: 504c 4347 323b 2d09 7072 6f74 6569 6e5f  PLCG2;-.protein_
+00016c40: 636f 6469 6e67 0969 6e74 726f 6e5f 7661  coding.intron_va
+00016c50: 7269 616e 7409 7661 7264 6963 7409 2d22  riant.vardict.-"
+00016c60: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00016c70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00016c80: 7445 7175 616c 2872 6573 756c 745b 3333  tEqual(result[33
+00016c90: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00016ca0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+00016cb0: 3109 3239 3434 3532 3832 0932 3934 3435  1.29445282.29445
+00016cc0: 3238 3209 4709 4109 342d 6f74 6865 7209  282.G.A.4-other.
+00016cd0: 3532 3009 3238 342e 3030 0933 0979 6573  520.284.00.3.yes
+00016ce0: 096f 6b09 414c 4b3b 2d09 7072 6f74 6569  .ok.ALK;-.protei
+00016cf0: 6e5f 636f 6469 6e67 0973 706c 6963 655f  n_coding.splice_
+00016d00: 7265 6769 6f6e 5f76 6172 6961 6e74 2669  region_variant&i
+00016d10: 6e74 726f 6e5f 7661 7269 616e 7409 7661  ntron_variant.va
+00016d20: 7264 6963 7409 2d22 2920 2023 206e 6f71  rdict.-")  # noq
+00016d30: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+00016d40: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00016d50: 6573 756c 745b 3334 5d2e 7273 7472 6970  esult[34].rstrip
+00016d60: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+00016d70: 3030 3030 3136 2e31 3109 3831 3935 3437  000016.11.819547
+00016d80: 3839 0938 3139 3534 3738 3909 4309 4709  89.81954789.C.G.
+00016d90: 342d 6f74 6865 7209 3131 3434 0934 3432  4-other.1144.442
+00016da0: 2e30 3009 3334 3909 7965 7309 6f6b 09c2  .00.349.yes.ok..
+00016db0: b453 4550 543b 2d09 7072 6f74 6569 6e5f  .SEPT;-.protein_
+00016dc0: 636f 6469 6e67 0969 6e74 726f 6e5f 7661  coding.intron_va
+00016dd0: 7269 616e 7409 7661 7264 6963 742c 6d75  riant.vardict,mu
+00016de0: 7465 6374 3209 2d22 2920 2023 206e 6f71  tect2.-")  # noq
+00016df0: 610a 0a20 2020 2020 2020 2072 6570 6f72  a..        repor
+00016e00: 7420 3d20 6f73 2e70 6174 682e 6a6f 696e  t = os.path.join
+00016e10: 2873 656c 662e 7465 6d70 6469 722c 2022  (self.tempdir, "
+00016e20: 6669 6c74 6572 6564 2e72 6570 6f72 7422  filtered.report"
+00016e30: 290a 2020 2020 2020 2020 6765 6e65 7261  ).        genera
+00016e40: 7465 5f68 6f74 7370 6f74 5f72 6570 6f72  te_hotspot_repor
+00016e50: 7428 2273 616d 706c 6531 222c 0a20 2020  t("sample1",.   
+00016e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e70: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00016e80: 6f72 742c 0a20 2020 2020 2020 2020 2020  ort,.           
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ea0: 2020 2020 206c 6576 656c 732c 0a20 2020       levels,.   
+00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ec0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016ed0: 662e 686f 7473 706f 742c 0a20 2020 2020  f.hotspot,.     
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016f00: 7663 665f 7665 7020 2b20 222e 677a 222c  vcf_vep + ".gz",
+00016f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f30: 2073 656c 662e 6776 6366 202b 2022 2e67   self.gvcf + ".g
+00016f40: 7a22 2c0a 2020 2020 2020 2020 2020 2020  z",.            
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f60: 2020 2020 7365 6c66 2e72 6566 6572 656e      self.referen
+00016f70: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f90: 2020 2020 7365 6c66 2e76 6366 5f76 6570      self.vcf_vep
+00016fa0: 5f77 6f5f 7069 636b 202b 2022 2e67 7a22  _wo_pick + ".gz"
+00016fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 2020 2274 6573 7473 2f75 7469 6c73 2f66    "tests/utils/f
+00016fe0: 696c 6573 2f72 6570 6f72 745f 636f 6c75  iles/report_colu
+00016ff0: 6d6e 735f 636f 6d62 696e 655f 636f 6c75  mns_combine_colu
+00017000: 6d6e 735f 6d75 6c74 695f 6c65 7665 6c2e  mns_multi_level.
+00017010: 7961 6d6c 2229 0a20 2020 2020 2020 2077  yaml").        w
+00017020: 6974 6820 6f70 656e 2872 6570 6f72 742c  ith open(report,
+00017030: 2027 7227 2920 6173 2072 6570 6f72 745f   'r') as report_
+00017040: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
+00017050: 2020 2020 6865 6164 203d 2072 6570 6f72      head = repor
+00017060: 745f 7265 7375 6c74 2e72 6561 646c 696e  t_result.readlin
+00017070: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00017080: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00017090: 2868 6561 642e 7273 7472 6970 2829 2c20  (head.rstrip(), 
+000170a0: 225c 7422 2e6a 6f69 6e28 5b22 7361 6d70  "\t".join(["samp
+000170b0: 6c65 222c 2022 6368 7222 2c20 2273 7461  le", "chr", "sta
+000170c0: 7274 222c 2022 7374 6f70 222c 2022 7265  rt", "stop", "re
+000170d0: 6622 2c20 2261 6c74 222c 2022 7265 706f  f", "alt", "repo
+000170e0: 7274 222c 2027 6776 6366 5f64 6570 7468  rt", 'gvcf_depth
+000170f0: 272c 2022 7265 665f 6465 7074 6822 2c20  ', "ref_depth", 
+00017100: 2261 6c74 5f64 6570 7468 222c 2027 416e  "alt_depth", 'An
+00017110: 616c 797a 6162 6c65 272c 2027 4d69 6e5f  alyzable', 'Min_
+00017120: 7265 6164 5f64 6570 7468 3330 3027 2c20  read_depth300', 
+00017130: 2747 656e 655f 7665 703b 686f 7473 706f  'Gene_vep;hotspo
+00017140: 745f 6161 3a63 6473 272c 2027 5661 7269  t_aa:cds', 'Vari
+00017150: 616e 745f 7479 7065 272c 2027 436f 6e73  ant_type', 'Cons
+00017160: 6571 7565 6e63 6527 2c20 2743 616c 6c65  equence', 'Calle
+00017170: 7273 272c 2027 436f 6d6d 656e 7427 5d29  rs', 'Comment'])
+00017180: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00017190: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
+000171a0: 6570 6f72 745f 7265 7375 6c74 2e72 6561  eport_result.rea
+000171b0: 646c 696e 6573 2829 0a20 2020 2020 2020  dlines().       
+000171c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000171d0: 4571 7561 6c28 6c65 6e28 7265 7375 6c74  Equal(len(result
+000171e0: 292c 2033 3529 0a20 2020 2020 2020 2020  ), 35).         
+000171f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00017200: 7561 6c28 7265 7375 6c74 5b30 5d2e 7273  ual(result[0].rs
+00017210: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017220: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
+00017230: 3434 3532 3731 0932 3934 3435 3237 3109  445271.29445271.
+00017240: 4709 4109 312d 686f 7473 706f 7409 3632  G.A.1-hotspot.62
+00017250: 3009 3335 3909 3409 7965 7309 6f6b 0941  0.359.4.yes.ok.A
+00017260: 4c4b 3b70 2e43 3131 3536 3a63 2e47 3334  LK;p.C1156:c.G34
+00017270: 3637 0970 726f 7465 696e 5f63 6f64 696e  67.protein_codin
+00017280: 6709 7379 6e6f 6e79 6d6f 7573 5f76 6172  g.synonymous_var
+00017290: 6961 6e74 0976 6172 6469 6374 0972 6573  iant.vardict.res
+000172a0: 6973 7461 6e63 655f 6d75 7461 7469 6f6e  istance_mutation
+000172b0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+000172c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000172d0: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
+000172e0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+000172f0: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
+00017300: 3309 3134 3034 3938 3335 3909 3134 3034  3.140498359.1404
+00017310: 3938 3336 3209 4354 5454 0943 0932 2d69  98362.CTTT.C.2-i
+00017320: 6e64 656c 0931 3030 2e35 0932 3709 3409  ndel.100.5.27.4.
+00017330: 7965 7309 6c6f 7709 4252 4146 3b70 2e45  yes.low.BRAF;p.E
+00017340: 3734 363a 632e 4732 3233 3609 7072 6f74  746:c.G2236.prot
+00017350: 6569 6e5f 636f 6469 6e67 0969 6e74 726f  ein_coding.intro
+00017360: 6e5f 7661 7269 616e 7409 6d75 7465 6374  n_variant.mutect
+00017370: 3209 2d22 2920 2023 206e 6f71 610a 2020  2.-")  # noqa.  
+00017380: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017390: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+000173a0: 745b 325d 2e72 7374 7269 7028 292c 2022  t[2].rstrip(), "
+000173b0: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+000173c0: 372e 3133 0931 3430 3439 3833 3631 0931  7.13.140498361.1
+000173d0: 3430 3439 3833 3631 092d 092d 0931 2d68  40498361.-.-.1-h
+000173e0: 6f74 7370 6f74 0931 3130 092d 092d 0979  otspot.110.-.-.y
+000173f0: 6573 096c 6f77 092d 3b70 2e45 3734 363a  es.low.-;p.E746:
+00017400: 632e 4732 3233 3609 2d09 2d09 2d09 2d22  c.G2236.-.-.-.-"
+00017410: 2920 2020 2320 6e6f 7161 0a20 2020 2020  )   # noqa.     
+00017420: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00017430: 7274 4571 7561 6c28 7265 7375 6c74 5b33  rtEqual(result[3
+00017440: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00017450: 706c 6531 094e 435f 3030 3030 3037 2e31  ple1.NC_000007.1
+00017460: 3309 3134 3034 3533 3133 3609 3134 3034  3.140453136.1404
+00017470: 3533 3133 3609 2d09 2d09 312d 686f 7473  53136.-.-.1-hots
+00017480: 706f 7409 3009 2d09 2d09 6e6f 7420 616e  pot.0.-.-.not an
+00017490: 616c 797a 6162 6c65 096c 6f77 092d 3b70  alyzable.low.-;p
+000174a0: 2e56 3630 303a 632e 5431 3739 3909 2d09  .V600:c.T1799.-.
+000174b0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+000174c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000174d0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+000174e0: 756c 745b 345d 2e72 7374 7269 7028 292c  ult[4].rstrip(),
+000174f0: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+00017500: 3030 372e 3133 0931 3136 3431 3230 3433  007.13.116412043
+00017510: 0931 3136 3431 3230 3433 092d 092d 0931  .116412043.-.-.1
+00017520: 2d68 6f74 7370 6f74 0930 092d 092d 096e  -hotspot.0.-.-.n
+00017530: 6f74 2061 6e61 6c79 7a61 626c 6509 6c6f  ot analyzable.lo
+00017540: 7709 2d3b 702e 4431 3032 383a 632e 4733  w.-;p.D1028:c.G3
+00017550: 3038 3209 2d09 2d09 2d09 2d22 2920 2023  082.-.-.-.-")  #
+00017560: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00017570: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017580: 616c 2872 6573 756c 745b 355d 2e72 7374  al(result[5].rst
+00017590: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+000175a0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+000175b0: 3435 3237 3109 3239 3434 3532 3731 092d  45271.29445271.-
+000175c0: 092d 0933 2d63 6865 636b 0936 3230 092d  .-.3-check.620.-
+000175d0: 092d 0979 6573 096f 6b09 2d3b 702e 4331  .-.yes.ok.-;p.C1
+000175e0: 3135 363a 632e 4733 3436 3709 2d09 2d09  156:c.G3467.-.-.
+000175f0: 2d09 2d22 2920 2023 206e 6f71 610a 2020  -.-")  # noqa.  
+00017600: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017610: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+00017620: 745b 365d 2e72 7374 7269 7028 292c 2022  t[6].rstrip(), "
+00017630: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00017640: 322e 3131 0932 3934 3435 3237 3209 3239  2.11.29445272.29
+00017650: 3434 3532 3732 092d 092d 0933 2d63 6865  445272.-.-.3-che
+00017660: 636b 0932 3231 092d 092d 0979 6573 096c  ck.221.-.-.yes.l
+00017670: 6f77 092d 3b70 2e43 3131 3536 3a63 2e47  ow.-;p.C1156:c.G
+00017680: 3334 3637 092d 092d 092d 092d 2229 2020  3467.-.-.-.-")  
+00017690: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+000176a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000176b0: 7561 6c28 7265 7375 6c74 5b37 5d2e 7273  ual(result[7].rs
+000176c0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+000176d0: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
+000176e0: 3434 3532 3733 0932 3934 3435 3237 3309  445273.29445273.
+000176f0: 2d09 2d09 332d 6368 6563 6b09 3632 3809  -.-.3-check.628.
+00017700: 2d09 2d09 7965 7309 6f6b 092d 3b70 2e43  -.-.yes.ok.-;p.C
+00017710: 3131 3536 3a63 2e47 3334 3637 092d 092d  1156:c.G3467.-.-
+00017720: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00017730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017740: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00017750: 6c74 5b38 5d2e 7273 7472 6970 2829 2c20  lt[8].rstrip(), 
+00017760: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+00017770: 3032 2e31 3109 3239 3434 3532 3734 0932  02.11.29445274.2
+00017780: 3934 3435 3237 3409 2d09 2d09 332d 6368  9445274.-.-.3-ch
+00017790: 6563 6b09 3631 3809 2d09 2d09 7965 7309  eck.618.-.-.yes.
+000177a0: 6f6b 092d 3b70 2e43 3131 3536 3a63 2e47  ok.-;p.C1156:c.G
+000177b0: 3334 3637 092d 092d 092d 092d 2229 2020  3467.-.-.-.-")  
+000177c0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+000177d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000177e0: 7561 6c28 7265 7375 6c74 5b39 5d2e 7273  ual(result[9].rs
+000177f0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017800: 094e 435f 3030 3030 3032 2e31 3109 3239  .NC_000002.11.29
+00017810: 3434 3532 3735 0932 3934 3435 3237 3509  445275.29445275.
+00017820: 2d09 2d09 332d 6368 6563 6b09 3630 3809  -.-.3-check.608.
+00017830: 2d09 2d09 7965 7309 6f6b 092d 3b70 2e43  -.-.yes.ok.-;p.C
+00017840: 3131 3536 3a63 2e47 3334 3637 092d 092d  1156:c.G3467.-.-
+00017850: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+00017860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017870: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00017880: 6c74 5b31 305d 2e72 7374 7269 7028 292c  lt[10].rstrip(),
+00017890: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+000178a0: 3030 322e 3131 0932 3934 3435 3237 3609  002.11.29445276.
+000178b0: 3239 3434 3532 3736 092d 092d 0933 2d63  29445276.-.-.3-c
+000178c0: 6865 636b 0936 3231 092d 092d 0979 6573  heck.621.-.-.yes
+000178d0: 096f 6b09 2d3b 702e 4331 3135 363a 632e  .ok.-;p.C1156:c.
+000178e0: 4733 3436 3709 2d09 2d09 2d09 2d22 2920  G3467.-.-.-.-") 
+000178f0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00017900: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00017910: 7175 616c 2872 6573 756c 745b 3131 5d2e  qual(result[11].
+00017920: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+00017930: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
+00017940: 3239 3434 3532 3737 0932 3934 3435 3237  29445277.2944527
+00017950: 3709 2d09 2d09 332d 6368 6563 6b09 3138  7.-.-.3-check.18
+00017960: 3209 2d09 2d09 7965 7309 6c6f 7709 2d3b  2.-.-.yes.low.-;
+00017970: 702e 4331 3135 363a 632e 4733 3436 3709  p.C1156:c.G3467.
+00017980: 2d09 2d09 2d09 2d22 2920 2023 206e 6f71  -.-.-.-")  # noq
+00017990: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000179a0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000179b0: 6573 756c 745b 3132 5d2e 7273 7472 6970  esult[12].rstrip
+000179c0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+000179d0: 3030 3030 3032 2e31 3109 3239 3434 3532  000002.11.294452
+000179e0: 3738 0932 3934 3435 3237 3809 2d09 2d09  78.29445278.-.-.
+000179f0: 332d 6368 6563 6b09 3535 3009 2d09 2d09  3-check.550.-.-.
+00017a00: 7965 7309 6f6b 092d 3b70 2e43 3131 3536  yes.ok.-;p.C1156
+00017a10: 3a63 2e47 3334 3637 092d 092d 092d 092d  :c.G3467.-.-.-.-
+00017a20: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00017a30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00017a40: 7274 4571 7561 6c28 7265 7375 6c74 5b31  rtEqual(result[1
+00017a50: 335d 2e72 7374 7269 7028 292c 2022 7361  3].rstrip(), "sa
+00017a60: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+00017a70: 3131 0932 3934 3435 3237 3909 3239 3434  11.29445279.2944
+00017a80: 3532 3739 092d 092d 0933 2d63 6865 636b  5279.-.-.3-check
+00017a90: 0935 3934 092d 092d 0979 6573 096f 6b09  .594.-.-.yes.ok.
+00017aa0: 2d3b 702e 4331 3135 363a 632e 4733 3436  -;p.C1156:c.G346
+00017ab0: 3709 2d09 2d09 2d09 2d22 2920 2023 206e  7.-.-.-.-")  # n
+00017ac0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00017ad0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00017ae0: 2872 6573 756c 745b 3134 5d2e 7273 7472  (result[14].rstr
+00017af0: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+00017b00: 435f 3030 3030 3032 2e31 3109 3239 3434  C_000002.11.2944
+00017b10: 3532 3830 0932 3934 3435 3238 3009 2d09  5280.29445280.-.
+00017b20: 2d09 332d 6368 6563 6b09 3533 3909 2d09  -.3-check.539.-.
+00017b30: 2d09 7965 7309 6f6b 092d 3b70 2e43 3131  -.yes.ok.-;p.C11
+00017b40: 3536 3a63 2e47 3334 3637 092d 092d 092d  56:c.G3467.-.-.-
+00017b50: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+00017b60: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00017b70: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00017b80: 5b31 355d 2e72 7374 7269 7028 292c 2022  [15].rstrip(), "
+00017b90: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00017ba0: 322e 3131 0932 3934 3435 3238 3109 3239  2.11.29445281.29
+00017bb0: 3434 3532 3831 092d 092d 0933 2d63 6865  445281.-.-.3-che
+00017bc0: 636b 0935 3236 092d 092d 0979 6573 096f  ck.526.-.-.yes.o
+00017bd0: 6b09 2d3b 702e 4331 3135 363a 632e 4733  k.-;p.C1156:c.G3
+00017be0: 3436 3709 2d09 2d09 2d09 2d22 2920 2023  467.-.-.-.-")  #
+00017bf0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00017c00: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017c10: 616c 2872 6573 756c 745b 3136 5d2e 7273  al(result[16].rs
+00017c20: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017c30: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+00017c40: 3537 3338 3736 3509 3134 3537 3338 3736  5738765.14573876
+00017c50: 3509 2d09 2d09 332d 6368 6563 6b09 3136  5.-.-.3-check.16
+00017c60: 3136 092d 092d 0979 6573 096f 6b09 2d3b  16.-.-.yes.ok.-;
+00017c70: 2d3a 2d09 2d09 2d09 2d09 2d22 2920 2023  -:-.-.-.-.-")  #
+00017c80: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00017c90: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017ca0: 616c 2872 6573 756c 745b 3137 5d2e 7273  al(result[17].rs
+00017cb0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017cc0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+00017cd0: 3537 3338 3736 3609 3134 3537 3338 3736  5738766.14573876
+00017ce0: 3609 2d09 2d09 332d 6368 6563 6b09 3136  6.-.-.3-check.16
+00017cf0: 3139 092d 092d 0979 6573 096f 6b09 2d3b  19.-.-.yes.ok.-;
+00017d00: 2d3a 2d09 2d09 2d09 2d09 2d22 2920 2023  -:-.-.-.-.-")  #
+00017d10: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00017d20: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017d30: 616c 2872 6573 756c 745b 3138 5d2e 7273  al(result[18].rs
+00017d40: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017d50: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+00017d60: 3537 3338 3736 3709 3134 3537 3338 3736  5738767.14573876
+00017d70: 3709 2d09 2d09 332d 6368 6563 6b09 3135  7.-.-.3-check.15
+00017d80: 3935 092d 092d 0979 6573 096f 6b09 2d3b  95.-.-.yes.ok.-;
+00017d90: 2d3a 2d09 2d09 2d09 2d09 2d22 2920 2023  -:-.-.-.-.-")  #
+00017da0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00017db0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017dc0: 616c 2872 6573 756c 745b 3139 5d2e 7273  al(result[19].rs
+00017dd0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00017de0: 094e 435f 3030 3030 3038 2e31 3109 3134  .NC_000008.11.14
+00017df0: 3537 3338 3736 3809 3134 3537 3338 3736  5738768.14573876
+00017e00: 3809 4709 4309 332d 6368 6563 6b09 3135  8.G.C.3-check.15
+00017e10: 3437 0935 0932 3709 7965 7309 6f6b 094c  47.5.27.yes.ok.L
+00017e20: 5252 4331 343b 2d3a 2d09 7072 6f74 6569  RRC14;-:-.protei
+00017e30: 6e5f 636f 6469 6e67 0975 7073 7472 6561  n_coding.upstrea
+00017e40: 6d5f 6765 6e65 5f76 6172 6961 6e74 0976  m_gene_variant.v
+00017e50: 6172 6469 6374 092d 2229 2020 2320 6e6f  ardict.-")  # no
+00017e60: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00017e70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00017e80: 7265 7375 6c74 5b32 305d 2e72 7374 7269  result[20].rstri
+00017e90: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00017ea0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00017eb0: 3837 3639 0931 3435 3733 3837 3639 092d  8769.145738769.-
+00017ec0: 092d 0933 2d63 6865 636b 0931 3634 3409  .-.3-check.1644.
+00017ed0: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00017ee0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00017ef0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00017f00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00017f10: 7265 7375 6c74 5b32 315d 2e72 7374 7269  result[21].rstri
+00017f20: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00017f30: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00017f40: 3837 3730 0931 3435 3733 3837 3730 092d  8770.145738770.-
+00017f50: 092d 0933 2d63 6865 636b 0931 3636 3709  .-.3-check.1667.
+00017f60: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00017f70: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00017f80: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00017f90: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00017fa0: 7265 7375 6c74 5b32 325d 2e72 7374 7269  result[22].rstri
+00017fb0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00017fc0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00017fd0: 3837 3731 0931 3435 3733 3837 3731 092d  8771.145738771.-
+00017fe0: 092d 0933 2d63 6865 636b 0931 3638 3509  .-.3-check.1685.
+00017ff0: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00018000: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00018010: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00018020: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00018030: 7265 7375 6c74 5b32 335d 2e72 7374 7269  result[23].rstri
+00018040: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00018050: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00018060: 3837 3732 0931 3435 3733 3837 3732 092d  8772.145738772.-
+00018070: 092d 0933 2d63 6865 636b 0931 3638 3909  .-.3-check.1689.
+00018080: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00018090: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+000180a0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000180b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000180c0: 7265 7375 6c74 5b32 345d 2e72 7374 7269  result[24].rstri
+000180d0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+000180e0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+000180f0: 3837 3733 0931 3435 3733 3837 3733 092d  8773.145738773.-
+00018100: 092d 0933 2d63 6865 636b 0931 3934 3009  .-.3-check.1940.
+00018110: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00018120: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00018130: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00018140: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00018150: 7265 7375 6c74 5b32 355d 2e72 7374 7269  result[25].rstri
+00018160: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00018170: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00018180: 3837 3734 0931 3435 3733 3837 3734 092d  8774.145738774.-
+00018190: 092d 0933 2d63 6865 636b 0931 3934 3009  .-.3-check.1940.
+000181a0: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+000181b0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+000181c0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000181d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000181e0: 7265 7375 6c74 5b32 365d 2e72 7374 7269  result[26].rstri
+000181f0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00018200: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00018210: 3837 3735 0931 3435 3733 3837 3735 092d  8775.145738775.-
+00018220: 092d 0933 2d63 6865 636b 0931 3936 3309  .-.3-check.1963.
+00018230: 2d09 2d09 7965 7309 6f6b 092d 3b2d 3a2d  -.-.yes.ok.-;-:-
+00018240: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00018250: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00018260: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00018270: 7265 7375 6c74 5b32 375d 2e72 7374 7269  result[27].rstri
+00018280: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00018290: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+000182a0: 3837 3736 0931 3435 3733 3837 3736 092d  8776.145738776.-
+000182b0: 092d 0933 2d63 6865 636b 0930 092d 092d  .-.3-check.0.-.-
+000182c0: 096e 6f74 2061 6e61 6c79 7a61 626c 6509  .not analyzable.
+000182d0: 6c6f 7709 2d3b 2d3a 2d09 2d09 2d09 2d09  low.-;-:-.-.-.-.
+000182e0: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+000182f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00018300: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00018310: 3238 5d2e 7273 7472 6970 2829 2c20 2273  28].rstrip(), "s
+00018320: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+00018330: 2e31 3109 3134 3537 3338 3737 3709 3134  .11.145738777.14
+00018340: 3537 3338 3737 3709 2d09 2d09 332d 6368  5738777.-.-.3-ch
+00018350: 6563 6b09 3139 3634 092d 092d 0979 6573  eck.1964.-.-.yes
+00018360: 096f 6b09 2d3b 2d3a 2d09 2d09 2d09 2d09  .ok.-;-:-.-.-.-.
+00018370: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+00018380: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00018390: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+000183a0: 3239 5d2e 7273 7472 6970 2829 2c20 2273  29].rstrip(), "s
+000183b0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+000183c0: 2e31 3109 3134 3537 3338 3737 3809 3134  .11.145738778.14
+000183d0: 3537 3338 3737 3809 2d09 2d09 332d 6368  5738778.-.-.3-ch
+000183e0: 6563 6b09 3139 3633 092d 092d 0979 6573  eck.1963.-.-.yes
+000183f0: 096f 6b09 2d3b 2d3a 2d09 2d09 2d09 2d09  .ok.-;-:-.-.-.-.
+00018400: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+00018410: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00018420: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00018430: 3330 5d2e 7273 7472 6970 2829 2c20 2273  30].rstrip(), "s
+00018440: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+00018450: 2e31 3109 3134 3537 3338 3737 3909 3134  .11.145738779.14
+00018460: 3537 3338 3737 3909 2d09 2d09 332d 6368  5738779.-.-.3-ch
+00018470: 6563 6b09 3139 3538 092d 092d 0979 6573  eck.1958.-.-.yes
+00018480: 096f 6b09 2d3b 2d3a 2d09 2d09 2d09 2d09  .ok.-;-:-.-.-.-.
+00018490: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+000184a0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000184b0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+000184c0: 3331 5d2e 7273 7472 6970 2829 2c20 2273  31].rstrip(), "s
+000184d0: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+000184e0: 2e31 3109 3134 3537 3432 3531 3409 3134  .11.145742514.14
+000184f0: 3537 3432 3531 3409 4109 4709 332d 6368  5742514.A.G.3-ch
+00018500: 6563 6b09 3009 3009 3833 3909 6e6f 7420  eck.0.0.839.not 
+00018510: 616e 616c 797a 6162 6c65 096c 6f77 0952  analyzable.low.R
+00018520: 4543 514c 343b 2d3a 2d09 7072 6f74 6569  ECQL4;-:-.protei
+00018530: 6e5f 636f 6469 6e67 0973 796e 6f6e 796d  n_coding.synonym
+00018540: 6f75 735f 7661 7269 616e 7409 7661 7264  ous_variant.vard
+00018550: 6963 742c 6d75 7465 6374 3209 2d22 2920  ict,mutect2.-") 
+00018560: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00018570: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00018580: 7175 616c 2872 6573 756c 745b 3332 5d2e  qual(result[32].
+00018590: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+000185a0: 6531 094e 435f 3030 3030 3136 2e31 3109  e1.NC_000016.11.
+000185b0: 3831 3935 3437 3839 0938 3139 3534 3738  81954789.8195478
+000185c0: 3909 4309 4754 0932 2d69 6e64 656c 0931  9.C.GT.2-indel.1
+000185d0: 3134 3409 3131 3732 0932 3909 7965 7309  144.1172.29.yes.
+000185e0: 6f6b 0950 4c43 4732 3b2d 3a2d 0970 726f  ok.PLCG2;-:-.pro
+000185f0: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
+00018600: 6f6e 5f76 6172 6961 6e74 0976 6172 6469  on_variant.vardi
+00018610: 6374 092d 2229 2020 2320 6e6f 7161 0a20  ct.-")  # noqa. 
+00018620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018630: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00018640: 6c74 5b33 335d 2e72 7374 7269 7028 292c  lt[33].rstrip(),
+00018650: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+00018660: 3030 322e 3131 0932 3934 3435 3238 3209  002.11.29445282.
+00018670: 3239 3434 3532 3832 0947 0941 0934 2d6f  29445282.G.A.4-o
+00018680: 7468 6572 0935 3230 0932 3834 0933 0979  ther.520.284.3.y
+00018690: 6573 096f 6b09 414c 4b3b 2d3a 2d09 7072  es.ok.ALK;-:-.pr
+000186a0: 6f74 6569 6e5f 636f 6469 6e67 0973 706c  otein_coding.spl
+000186b0: 6963 655f 7265 6769 6f6e 5f76 6172 6961  ice_region_varia
+000186c0: 6e74 2669 6e74 726f 6e5f 7661 7269 616e  nt&intron_varian
+000186d0: 7409 7661 7264 6963 7409 2d22 2920 2023  t.vardict.-")  #
+000186e0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+000186f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00018700: 616c 2872 6573 756c 745b 3334 5d2e 7273  al(result[34].rs
+00018710: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+00018720: 094e 435f 3030 3030 3136 2e31 3109 3831  .NC_000016.11.81
+00018730: 3935 3437 3839 0938 3139 3534 3738 3909  954789.81954789.
+00018740: 4309 4709 342d 6f74 6865 7209 3131 3434  C.G.4-other.1144
+00018750: 0934 3432 0933 3439 0979 6573 096f 6b09  .442.349.yes.ok.
+00018760: 5345 5054 3b2d 3a2d 0970 726f 7465 696e  SEPT;-:-.protein
+00018770: 5f63 6f64 696e 6709 696e 7472 6f6e 5f76  _coding.intron_v
+00018780: 6172 6961 6e74 0976 6172 6469 6374 2c6d  ariant.vardict,m
+00018790: 7574 6563 7432 092d 2229 2020 2320 6e6f  utect2.-")  # no
+000187a0: 7161 0a0a 2020 2020 6465 6620 7465 7374  qa..    def test
+000187b0: 5f66 696c 7465 7265 645f 6d75 7461 7469  _filtered_mutati
+000187c0: 6f6e 5f73 656c 6563 745f 6f6e 655f 636f  on_select_one_co
+000187d0: 6c75 6d6e 7328 7365 6c66 293a 0a20 2020  lumns(self):.   
+000187e0: 2020 2020 2066 726f 6d20 6879 6472 615f       from hydra_
+000187f0: 6765 6e65 7469 6373 2e75 7469 6c73 2e69  genetics.utils.i
+00018800: 6f2e 686f 7473 706f 745f 7265 706f 7274  o.hotspot_report
+00018810: 2069 6d70 6f72 7420 6765 6e65 7261 7465   import generate
+00018820: 5f68 6f74 7370 6f74 5f72 6570 6f72 740a  _hotspot_report.
+00018830: 2020 2020 2020 2020 6c65 7665 6c73 203d          levels =
+00018840: 205b 2833 3030 2c20 226f 6b22 2c20 2279   [(300, "ok", "y
+00018850: 6573 2229 2c20 2833 302c 2022 6c6f 7722  es"), (30, "low"
+00018860: 2c20 2279 6573 2229 2c20 2830 2c20 226c  , "yes"), (0, "l
+00018870: 6f77 222c 2022 6e6f 7420 616e 616c 797a  ow", "not analyz
+00018880: 6162 6c65 2229 5d0a 0a20 2020 2020 2020  able")]..       
+00018890: 2073 656c 662e 6d61 7844 6966 6620 3d20   self.maxDiff = 
+000188a0: 3130 3030 300a 0a20 2020 2020 2020 2072  10000..        r
+000188b0: 6570 6f72 7420 3d20 6f73 2e70 6174 682e  eport = os.path.
+000188c0: 6a6f 696e 2873 656c 662e 7465 6d70 6469  join(self.tempdi
+000188d0: 722c 2022 6669 6c74 6572 6564 2e72 6570  r, "filtered.rep
+000188e0: 6f72 7422 290a 2020 2020 2020 2020 6765  ort").        ge
+000188f0: 6e65 7261 7465 5f68 6f74 7370 6f74 5f72  nerate_hotspot_r
+00018900: 6570 6f72 7428 2273 616d 706c 6531 222c  eport("sample1",
+00018910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018930: 2072 6570 6f72 742c 0a20 2020 2020 2020   report,.       
+00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018950: 2020 2020 2020 2020 206c 6576 656c 732c           levels,
+00018960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018980: 2073 656c 662e 686f 7473 706f 742c 0a20   self.hotspot,. 
+00018990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000189b0: 656c 662e 7663 665f 7665 7020 2b20 222e  elf.vcf_vep + ".
+000189c0: 677a 222c 0a20 2020 2020 2020 2020 2020  gz",.           
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189e0: 2020 2020 2073 656c 662e 6776 6366 202b       self.gvcf +
+000189f0: 2022 2e67 7a22 2c0a 2020 2020 2020 2020   ".gz",.        
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00018a20: 6572 656e 6365 2c0a 2020 2020 2020 2020  erence,.        
+00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a40: 2020 2020 2020 2020 7365 6c66 2e76 6366          self.vcf
+00018a50: 5f76 6570 5f77 6f5f 7069 636b 202b 2022  _vep_wo_pick + "
+00018a60: 2e67 7a22 2c0a 2020 2020 2020 2020 2020  .gz",.          
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a80: 2020 2020 2020 2274 6573 7473 2f75 7469        "tests/uti
+00018a90: 6c73 2f66 696c 6573 2f72 6570 6f72 745f  ls/files/report_
+00018aa0: 636f 6c75 6d6e 735f 7365 6c65 6374 5f63  columns_select_c
+00018ab0: 6f6c 756d 6e2e 7961 6d6c 2229 0a20 2020  olumn.yaml").   
+00018ac0: 2020 2020 2077 6974 6820 6f70 656e 2872       with open(r
+00018ad0: 6570 6f72 742c 2027 7227 2920 6173 2072  eport, 'r') as r
+00018ae0: 6570 6f72 745f 7265 7375 6c74 3a0a 2020  eport_result:.  
+00018af0: 2020 2020 2020 2020 2020 6865 6164 203d            head =
+00018b00: 2072 6570 6f72 745f 7265 7375 6c74 2e72   report_result.r
+00018b10: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
+00018b20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00018b30: 7445 7175 616c 2868 6561 642e 7273 7472  tEqual(head.rstr
+00018b40: 6970 2829 2c20 225c 7422 2e6a 6f69 6e28  ip(), "\t".join(
+00018b50: 5b22 7361 6d70 6c65 222c 2022 6368 7222  ["sample", "chr"
+00018b60: 2c20 2273 7461 7274 222c 2022 7374 6f70  , "start", "stop
+00018b70: 222c 2022 7265 6622 2c20 2261 6c74 222c  ", "ref", "alt",
+00018b80: 2022 7265 706f 7274 222c 2027 6776 6366   "report", 'gvcf
+00018b90: 5f64 6570 7468 272c 2022 7265 665f 6465  _depth', "ref_de
+00018ba0: 7074 6822 2c20 2261 6c74 5f64 6570 7468  pth", "alt_depth
+00018bb0: 222c 2027 416e 616c 797a 6162 6c65 272c  ", 'Analyzable',
+00018bc0: 2027 4d69 6e5f 7265 6164 5f64 6570 7468   'Min_read_depth
+00018bd0: 3330 3027 2c20 2747 656e 6527 2c20 2756  300', 'Gene', 'V
+00018be0: 6172 6961 6e74 5f74 7970 6527 2c20 2743  ariant_type', 'C
+00018bf0: 6f6e 7365 7175 656e 6365 272c 2027 4361  onsequence', 'Ca
+00018c00: 6c6c 6572 7327 2c20 2743 6f6d 6d65 6e74  llers', 'Comment
+00018c10: 272c 2027 4e6f 745f 456d 7074 7927 2c20  ', 'Not_Empty', 
+00018c20: 2745 6d70 7479 275d 2929 2020 2320 6e6f  'Empty']))  # no
+00018c30: 7161 0a20 2020 2020 2020 2020 2020 2072  qa.            r
+00018c40: 6573 756c 7420 3d20 7265 706f 7274 5f72  esult = report_r
+00018c50: 6573 756c 742e 7265 6164 6c69 6e65 7328  esult.readlines(
+00018c60: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00018c70: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00018c80: 656e 2872 6573 756c 7429 2c20 3335 290a  en(result), 35).
+00018c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018ca0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00018cb0: 756c 745b 305d 2e72 7374 7269 7028 292c  ult[0].rstrip(),
+00018cc0: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+00018cd0: 3030 322e 3131 0932 3934 3435 3237 3109  002.11.29445271.
+00018ce0: 3239 3434 3532 3731 0947 0941 0931 2d68  29445271.G.A.1-h
+00018cf0: 6f74 7370 6f74 0936 3230 0933 3539 0934  otspot.620.359.4
+00018d00: 0979 6573 096f 6b09 414c 4b09 7072 6f74  .yes.ok.ALK.prot
+00018d10: 6569 6e5f 636f 6469 6e67 0973 796e 6f6e  ein_coding.synon
+00018d20: 796d 6f75 735f 7661 7269 616e 7409 7661  ymous_variant.va
+00018d30: 7264 6963 7409 7265 7369 7374 616e 6365  rdict.resistance
+00018d40: 5f6d 7574 6174 696f 6e09 414c 4b09 2d22  _mutation.ALK.-"
+00018d50: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+00018d60: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00018d70: 7445 7175 616c 2872 6573 756c 745b 315d  tEqual(result[1]
+00018d80: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00018d90: 6c65 3109 4e43 5f30 3030 3030 372e 3133  le1.NC_000007.13
+00018da0: 0931 3430 3439 3833 3539 0931 3430 3439  .140498359.14049
+00018db0: 3833 3632 0943 5454 5409 4309 322d 696e  8362.CTTT.C.2-in
+00018dc0: 6465 6c09 3130 302e 3509 3237 0934 0979  del.100.5.27.4.y
+00018dd0: 6573 096c 6f77 0942 5241 4609 7072 6f74  es.low.BRAF.prot
+00018de0: 6569 6e5f 636f 6469 6e67 0969 6e74 726f  ein_coding.intro
+00018df0: 6e5f 7661 7269 616e 7409 6d75 7465 6374  n_variant.mutect
+00018e00: 3209 2d09 4547 4652 092d 2229 2020 2320  2.-.EGFR.-")  # 
+00018e10: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00018e20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00018e30: 6c28 7265 7375 6c74 5b32 5d2e 7273 7472  l(result[2].rstr
+00018e40: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+00018e50: 435f 3030 3030 3037 2e31 3309 3134 3034  C_000007.13.1404
+00018e60: 3938 3336 3109 3134 3034 3938 3336 3109  98361.140498361.
+00018e70: 2d09 2d09 312d 686f 7473 706f 7409 3131  -.-.1-hotspot.11
+00018e80: 3009 2d09 2d09 7965 7309 6c6f 7709 4547  0.-.-.yes.low.EG
+00018e90: 4652 092d 092d 092d 092d 092d 0945 4746  FR.-.-.-.-.-.EGF
+00018ea0: 5222 2920 2020 2320 6e6f 7161 0a20 2020  R")   # noqa.   
+00018eb0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00018ec0: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00018ed0: 5b33 5d2e 7273 7472 6970 2829 2c20 2273  [3].rstrip(), "s
+00018ee0: 616d 706c 6531 094e 435f 3030 3030 3037  ample1.NC_000007
+00018ef0: 2e31 3309 3134 3034 3533 3133 3609 3134  .13.140453136.14
+00018f00: 3034 3533 3133 3609 2d09 2d09 312d 686f  0453136.-.-.1-ho
+00018f10: 7473 706f 7409 3009 2d09 2d09 6e6f 7420  tspot.0.-.-.not 
+00018f20: 616e 616c 797a 6162 6c65 096c 6f77 0942  analyzable.low.B
+00018f30: 5241 4609 2d09 2d09 2d09 2d09 2d09 4252  RAF.-.-.-.-.-.BR
+00018f40: 4146 2229 2020 2320 6e6f 7161 0a20 2020  AF")  # noqa.   
+00018f50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00018f60: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00018f70: 5b34 5d2e 7273 7472 6970 2829 2c20 2273  [4].rstrip(), "s
+00018f80: 616d 706c 6531 094e 435f 3030 3030 3037  ample1.NC_000007
+00018f90: 2e31 3309 3131 3634 3132 3034 3309 3131  .13.116412043.11
+00018fa0: 3634 3132 3034 3309 2d09 2d09 312d 686f  6412043.-.-.1-ho
+00018fb0: 7473 706f 7409 3009 2d09 2d09 6e6f 7420  tspot.0.-.-.not 
+00018fc0: 616e 616c 797a 6162 6c65 096c 6f77 094d  analyzable.low.M
+00018fd0: 4554 092d 092d 092d 092d 092d 094d 4554  ET.-.-.-.-.-.MET
+00018fe0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00018ff0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00019000: 7274 4571 7561 6c28 7265 7375 6c74 5b35  rtEqual(result[5
+00019010: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+00019020: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+00019030: 3109 3239 3434 3532 3731 0932 3934 3435  1.29445271.29445
+00019040: 3237 3109 2d09 2d09 332d 6368 6563 6b09  271.-.-.3-check.
+00019050: 3632 3009 2d09 2d09 7965 7309 6f6b 0941  620.-.-.yes.ok.A
+00019060: 4c4b 092d 092d 092d 092d 092d 0941 4c4b  LK.-.-.-.-.-.ALK
+00019070: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+00019080: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00019090: 7274 4571 7561 6c28 7265 7375 6c74 5b36  rtEqual(result[6
+000190a0: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+000190b0: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+000190c0: 3109 3239 3434 3532 3732 0932 3934 3435  1.29445272.29445
+000190d0: 3237 3209 2d09 2d09 332d 6368 6563 6b09  272.-.-.3-check.
+000190e0: 3232 3109 2d09 2d09 7965 7309 6c6f 7709  221.-.-.yes.low.
+000190f0: 414c 4b09 2d09 2d09 2d09 2d09 2d09 414c  ALK.-.-.-.-.-.AL
+00019100: 4b22 2920 2023 206e 6f71 610a 2020 2020  K")  # noqa.    
+00019110: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00019120: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00019130: 375d 2e72 7374 7269 7028 292c 2022 7361  7].rstrip(), "sa
+00019140: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+00019150: 3131 0932 3934 3435 3237 3309 3239 3434  11.29445273.2944
+00019160: 3532 3733 092d 092d 0933 2d63 6865 636b  5273.-.-.3-check
+00019170: 0936 3238 092d 092d 0979 6573 096f 6b09  .628.-.-.yes.ok.
+00019180: 414c 4b09 2d09 2d09 2d09 2d09 2d09 414c  ALK.-.-.-.-.-.AL
+00019190: 4b22 2920 2023 206e 6f71 610a 2020 2020  K")  # noqa.    
+000191a0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000191b0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+000191c0: 385d 2e72 7374 7269 7028 292c 2022 7361  8].rstrip(), "sa
+000191d0: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+000191e0: 3131 0932 3934 3435 3237 3409 3239 3434  11.29445274.2944
+000191f0: 3532 3734 092d 092d 0933 2d63 6865 636b  5274.-.-.3-check
+00019200: 0936 3138 092d 092d 0979 6573 096f 6b09  .618.-.-.yes.ok.
+00019210: 414c 4b09 2d09 2d09 2d09 2d09 2d09 414c  ALK.-.-.-.-.-.AL
+00019220: 4b22 2920 2023 206e 6f71 610a 2020 2020  K")  # noqa.    
+00019230: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00019240: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+00019250: 395d 2e72 7374 7269 7028 292c 2022 7361  9].rstrip(), "sa
+00019260: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+00019270: 3131 0932 3934 3435 3237 3509 3239 3434  11.29445275.2944
+00019280: 3532 3735 092d 092d 0933 2d63 6865 636b  5275.-.-.3-check
+00019290: 0936 3038 092d 092d 0979 6573 096f 6b09  .608.-.-.yes.ok.
+000192a0: 414c 4b09 2d09 2d09 2d09 2d09 2d09 414c  ALK.-.-.-.-.-.AL
+000192b0: 4b22 2920 2023 206e 6f71 610a 2020 2020  K")  # noqa.    
+000192c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000192d0: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+000192e0: 3130 5d2e 7273 7472 6970 2829 2c20 2273  10].rstrip(), "s
+000192f0: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
+00019300: 2e31 3109 3239 3434 3532 3736 0932 3934  .11.29445276.294
+00019310: 3435 3237 3609 2d09 2d09 332d 6368 6563  45276.-.-.3-chec
+00019320: 6b09 3632 3109 2d09 2d09 7965 7309 6f6b  k.621.-.-.yes.ok
+00019330: 0941 4c4b 092d 092d 092d 092d 092d 0941  .ALK.-.-.-.-.-.A
+00019340: 4c4b 2229 2020 2320 6e6f 7161 0a20 2020  LK")  # noqa.   
+00019350: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00019360: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+00019370: 5b31 315d 2e72 7374 7269 7028 292c 2022  [11].rstrip(), "
+00019380: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+00019390: 322e 3131 0932 3934 3435 3237 3709 3239  2.11.29445277.29
+000193a0: 3434 3532 3737 092d 092d 0933 2d63 6865  445277.-.-.3-che
+000193b0: 636b 0931 3832 092d 092d 0979 6573 096c  ck.182.-.-.yes.l
+000193c0: 6f77 0941 4c4b 092d 092d 092d 092d 092d  ow.ALK.-.-.-.-.-
+000193d0: 0941 4c4b 2229 2020 2320 6e6f 7161 0a20  .ALK")  # noqa. 
+000193e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000193f0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+00019400: 6c74 5b31 325d 2e72 7374 7269 7028 292c  lt[12].rstrip(),
+00019410: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+00019420: 3030 322e 3131 0932 3934 3435 3237 3809  002.11.29445278.
+00019430: 3239 3434 3532 3738 092d 092d 0933 2d63  29445278.-.-.3-c
+00019440: 6865 636b 0935 3530 092d 092d 0979 6573  heck.550.-.-.yes
+00019450: 096f 6b09 414c 4b09 2d09 2d09 2d09 2d09  .ok.ALK.-.-.-.-.
+00019460: 2d09 414c 4b22 2920 2023 206e 6f71 610a  -.ALK")  # noqa.
+00019470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019480: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019490: 756c 745b 3133 5d2e 7273 7472 6970 2829  ult[13].rstrip()
+000194a0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+000194b0: 3030 3032 2e31 3109 3239 3434 3532 3739  0002.11.29445279
+000194c0: 0932 3934 3435 3237 3909 2d09 2d09 332d  .29445279.-.-.3-
+000194d0: 6368 6563 6b09 3539 3409 2d09 2d09 7965  check.594.-.-.ye
+000194e0: 7309 6f6b 0941 4c4b 092d 092d 092d 092d  s.ok.ALK.-.-.-.-
+000194f0: 092d 0941 4c4b 2229 2020 2320 6e6f 7161  .-.ALK")  # noqa
+00019500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019510: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00019520: 7375 6c74 5b31 345d 2e72 7374 7269 7028  sult[14].rstrip(
+00019530: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+00019540: 3030 3030 322e 3131 0932 3934 3435 3238  00002.11.2944528
+00019550: 3009 3239 3434 3532 3830 092d 092d 0933  0.29445280.-.-.3
+00019560: 2d63 6865 636b 0935 3339 092d 092d 0979  -check.539.-.-.y
+00019570: 6573 096f 6b09 414c 4b09 2d09 2d09 2d09  es.ok.ALK.-.-.-.
+00019580: 2d09 2d09 414c 4b22 2920 2023 206e 6f71  -.-.ALK")  # noq
+00019590: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+000195a0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+000195b0: 6573 756c 745b 3135 5d2e 7273 7472 6970  esult[15].rstrip
+000195c0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+000195d0: 3030 3030 3032 2e31 3109 3239 3434 3532  000002.11.294452
+000195e0: 3831 0932 3934 3435 3238 3109 2d09 2d09  81.29445281.-.-.
+000195f0: 332d 6368 6563 6b09 3532 3609 2d09 2d09  3-check.526.-.-.
+00019600: 7965 7309 6f6b 0941 4c4b 092d 092d 092d  yes.ok.ALK.-.-.-
+00019610: 092d 092d 0941 4c4b 2229 2020 2320 6e6f  .-.-.ALK")  # no
+00019620: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00019630: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00019640: 7265 7375 6c74 5b31 365d 2e72 7374 7269  result[16].rstri
+00019650: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00019660: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00019670: 3837 3635 0931 3435 3733 3837 3635 092d  8765.145738765.-
+00019680: 092d 0933 2d63 6865 636b 0931 3631 3609  .-.3-check.1616.
+00019690: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+000196a0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+000196b0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000196c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000196d0: 7265 7375 6c74 5b31 375d 2e72 7374 7269  result[17].rstri
+000196e0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+000196f0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00019700: 3837 3636 0931 3435 3733 3837 3636 092d  8766.145738766.-
+00019710: 092d 0933 2d63 6865 636b 0931 3631 3909  .-.3-check.1619.
+00019720: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+00019730: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+00019740: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+00019750: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00019760: 7265 7375 6c74 5b31 385d 2e72 7374 7269  result[18].rstri
+00019770: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00019780: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00019790: 3837 3637 0931 3435 3733 3837 3637 092d  8767.145738767.-
+000197a0: 092d 0933 2d63 6865 636b 0931 3539 3509  .-.3-check.1595.
+000197b0: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+000197c0: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+000197d0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+000197e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000197f0: 7265 7375 6c74 5b31 395d 2e72 7374 7269  result[19].rstri
+00019800: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+00019810: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+00019820: 3837 3638 0931 3435 3733 3837 3638 0947  8768.145738768.G
+00019830: 0943 0933 2d63 6865 636b 0931 3534 3709  .C.3-check.1547.
+00019840: 3509 3237 0979 6573 096f 6b09 4c52 5243  5.27.yes.ok.LRRC
+00019850: 3134 0970 726f 7465 696e 5f63 6f64 696e  14.protein_codin
+00019860: 6709 7570 7374 7265 616d 5f67 656e 655f  g.upstream_gene_
+00019870: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
+00019880: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000198a0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+000198b0: 756c 745b 3230 5d2e 7273 7472 6970 2829  ult[20].rstrip()
+000198c0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+000198d0: 3030 3038 2e31 3109 3134 3537 3338 3736  0008.11.14573876
+000198e0: 3909 3134 3537 3338 3736 3909 2d09 2d09  9.145738769.-.-.
+000198f0: 332d 6368 6563 6b09 3136 3434 092d 092d  3-check.1644.-.-
+00019900: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019910: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019930: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019940: 756c 745b 3231 5d2e 7273 7472 6970 2829  ult[21].rstrip()
+00019950: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019960: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019970: 3009 3134 3537 3338 3737 3009 2d09 2d09  0.145738770.-.-.
+00019980: 332d 6368 6563 6b09 3136 3637 092d 092d  3-check.1667.-.-
+00019990: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+000199a0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+000199b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000199c0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+000199d0: 756c 745b 3232 5d2e 7273 7472 6970 2829  ult[22].rstrip()
+000199e0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+000199f0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019a00: 3109 3134 3537 3338 3737 3109 2d09 2d09  1.145738771.-.-.
+00019a10: 332d 6368 6563 6b09 3136 3835 092d 092d  3-check.1685.-.-
+00019a20: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019a30: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019a50: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019a60: 756c 745b 3233 5d2e 7273 7472 6970 2829  ult[23].rstrip()
+00019a70: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019a80: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019a90: 3209 3134 3537 3338 3737 3209 2d09 2d09  2.145738772.-.-.
+00019aa0: 332d 6368 6563 6b09 3136 3839 092d 092d  3-check.1689.-.-
+00019ab0: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019ac0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019ad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019ae0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019af0: 756c 745b 3234 5d2e 7273 7472 6970 2829  ult[24].rstrip()
+00019b00: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019b10: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019b20: 3309 3134 3537 3338 3737 3309 2d09 2d09  3.145738773.-.-.
+00019b30: 332d 6368 6563 6b09 3139 3430 092d 092d  3-check.1940.-.-
+00019b40: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019b50: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019b70: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019b80: 756c 745b 3235 5d2e 7273 7472 6970 2829  ult[25].rstrip()
+00019b90: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019ba0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019bb0: 3409 3134 3537 3338 3737 3409 2d09 2d09  4.145738774.-.-.
+00019bc0: 332d 6368 6563 6b09 3139 3430 092d 092d  3-check.1940.-.-
+00019bd0: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019be0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019bf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019c00: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019c10: 756c 745b 3236 5d2e 7273 7472 6970 2829  ult[26].rstrip()
+00019c20: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019c30: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019c40: 3509 3134 3537 3338 3737 3509 2d09 2d09  5.145738775.-.-.
+00019c50: 332d 6368 6563 6b09 3139 3633 092d 092d  3-check.1963.-.-
+00019c60: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+00019c70: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+00019c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019c90: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+00019ca0: 756c 745b 3237 5d2e 7273 7472 6970 2829  ult[27].rstrip()
+00019cb0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+00019cc0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+00019cd0: 3609 3134 3537 3338 3737 3609 2d09 2d09  6.145738776.-.-.
+00019ce0: 332d 6368 6563 6b09 3009 2d09 2d09 6e6f  3-check.0.-.-.no
+00019cf0: 7420 616e 616c 797a 6162 6c65 096c 6f77  t analyzable.low
+00019d00: 092d 092d 092d 092d 092d 092d 092d 2229  .-.-.-.-.-.-.-")
+00019d10: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00019d20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00019d30: 4571 7561 6c28 7265 7375 6c74 5b32 385d  Equal(result[28]
+00019d40: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00019d50: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00019d60: 0931 3435 3733 3837 3737 0931 3435 3733  .145738777.14573
+00019d70: 3837 3737 092d 092d 0933 2d63 6865 636b  8777.-.-.3-check
+00019d80: 0931 3936 3409 2d09 2d09 7965 7309 6f6b  .1964.-.-.yes.ok
+00019d90: 092d 092d 092d 092d 092d 092d 092d 2229  .-.-.-.-.-.-.-")
+00019da0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00019db0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00019dc0: 4571 7561 6c28 7265 7375 6c74 5b32 395d  Equal(result[29]
+00019dd0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00019de0: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00019df0: 0931 3435 3733 3837 3738 0931 3435 3733  .145738778.14573
+00019e00: 3837 3738 092d 092d 0933 2d63 6865 636b  8778.-.-.3-check
+00019e10: 0931 3936 3309 2d09 2d09 7965 7309 6f6b  .1963.-.-.yes.ok
+00019e20: 092d 092d 092d 092d 092d 092d 092d 2229  .-.-.-.-.-.-.-")
+00019e30: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00019e40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00019e50: 4571 7561 6c28 7265 7375 6c74 5b33 305d  Equal(result[30]
+00019e60: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00019e70: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00019e80: 0931 3435 3733 3837 3739 0931 3435 3733  .145738779.14573
+00019e90: 3837 3739 092d 092d 0933 2d63 6865 636b  8779.-.-.3-check
+00019ea0: 0931 3935 3809 2d09 2d09 7965 7309 6f6b  .1958.-.-.yes.ok
+00019eb0: 092d 092d 092d 092d 092d 092d 092d 2229  .-.-.-.-.-.-.-")
+00019ec0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+00019ed0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00019ee0: 4571 7561 6c28 7265 7375 6c74 5b33 315d  Equal(result[31]
+00019ef0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+00019f00: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+00019f10: 0931 3435 3734 3235 3134 0931 3435 3734  .145742514.14574
+00019f20: 3235 3134 0941 0947 0933 2d63 6865 636b  2514.A.G.3-check
+00019f30: 0930 0930 0938 3339 096e 6f74 2061 6e61  .0.0.839.not ana
+00019f40: 6c79 7a61 626c 6509 6c6f 7709 5245 4351  lyzable.low.RECQ
+00019f50: 4c34 0970 726f 7465 696e 5f63 6f64 696e  L4.protein_codin
+00019f60: 6709 7379 6e6f 6e79 6d6f 7573 5f76 6172  g.synonymous_var
+00019f70: 6961 6e74 0976 6172 6469 6374 2c6d 7574  iant.vardict,mut
+00019f80: 6563 7432 092d 092d 092d 2229 2020 2320  ect2.-.-.-")  # 
+00019f90: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00019fa0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00019fb0: 6c28 7265 7375 6c74 5b33 325d 2e72 7374  l(result[32].rst
+00019fc0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+00019fd0: 4e43 5f30 3030 3031 362e 3131 0938 3139  NC_000016.11.819
+00019fe0: 3534 3738 3909 3831 3935 3437 3839 0943  54789.81954789.C
+00019ff0: 0947 5409 322d 696e 6465 6c09 3131 3434  .GT.2-indel.1144
+0001a000: 0931 3137 3209 3239 0979 6573 096f 6b09  .1172.29.yes.ok.
+0001a010: 504c 4347 3209 7072 6f74 6569 6e5f 636f  PLCG2.protein_co
+0001a020: 6469 6e67 0969 6e74 726f 6e5f 7661 7269  ding.intron_vari
+0001a030: 616e 7409 7661 7264 6963 7409 2d09 2d09  ant.vardict.-.-.
+0001a040: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+0001a050: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001a060: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0001a070: 3333 5d2e 7273 7472 6970 2829 2c20 2273  33].rstrip(), "s
+0001a080: 616d 706c 6531 094e 435f 3030 3030 3032  ample1.NC_000002
+0001a090: 2e31 3109 3239 3434 3532 3832 0932 3934  .11.29445282.294
+0001a0a0: 3435 3238 3209 4709 4109 342d 6f74 6865  45282.G.A.4-othe
+0001a0b0: 7209 3532 3009 3238 3409 3309 7965 7309  r.520.284.3.yes.
+0001a0c0: 6f6b 0941 4c4b 0970 726f 7465 696e 5f63  ok.ALK.protein_c
+0001a0d0: 6f64 696e 6709 7370 6c69 6365 5f72 6567  oding.splice_reg
+0001a0e0: 696f 6e5f 7661 7269 616e 7426 696e 7472  ion_variant&intr
+0001a0f0: 6f6e 5f76 6172 6961 6e74 0976 6172 6469  on_variant.vardi
+0001a100: 6374 092d 092d 092d 2229 2020 2320 6e6f  ct.-.-.-")  # no
+0001a110: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+0001a120: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001a130: 7265 7375 6c74 5b33 345d 2e72 7374 7269  result[34].rstri
+0001a140: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0001a150: 5f30 3030 3031 362e 3131 0938 3139 3534  _000016.11.81954
+0001a160: 3738 3909 3831 3935 3437 3839 0943 0947  789.81954789.C.G
+0001a170: 0934 2d6f 7468 6572 0931 3134 3409 3434  .4-other.1144.44
+0001a180: 3209 3334 3909 7965 7309 6f6b 0953 4550  2.349.yes.ok.SEP
+0001a190: 5409 7072 6f74 6569 6e5f 636f 6469 6e67  T.protein_coding
+0001a1a0: 0969 6e74 726f 6e5f 7661 7269 616e 7409  .intron_variant.
+0001a1b0: 7661 7264 6963 742c 6d75 7465 6374 3209  vardict,mutect2.
+0001a1c0: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+0001a1d0: 0a20 2020 2064 6566 2074 6573 745f 7665  .    def test_ve
+0001a1e0: 705f 776f 5f70 6963 6b5f 6368 6f73 655f  p_wo_pick_chose_
+0001a1f0: 7472 616e 7363 7269 7074 2873 656c 6629  transcript(self)
+0001a200: 3a0a 2020 2020 2020 2020 6672 6f6d 2068  :.        from h
+0001a210: 7964 7261 5f67 656e 6574 6963 732e 7574  ydra_genetics.ut
+0001a220: 696c 732e 696f 2e68 6f74 7370 6f74 5f72  ils.io.hotspot_r
+0001a230: 6570 6f72 7420 696d 706f 7274 2067 656e  eport import gen
+0001a240: 6572 6174 655f 686f 7473 706f 745f 7265  erate_hotspot_re
+0001a250: 706f 7274 0a20 2020 2020 2020 206c 6576  port.        lev
+0001a260: 656c 7320 3d20 5b28 3330 302c 2022 6f6b  els = [(300, "ok
+0001a270: 222c 2022 7965 7322 292c 2028 3330 2c20  ", "yes"), (30, 
+0001a280: 226c 6f77 222c 2022 7965 7322 292c 2028  "low", "yes"), (
+0001a290: 302c 2022 6c6f 7722 2c20 226e 6f74 2061  0, "low", "not a
+0001a2a0: 6e61 6c79 7a61 626c 6522 295d 0a0a 2020  nalyzable")]..  
+0001a2b0: 2020 2020 2020 7365 6c66 2e6d 6178 4469        self.maxDi
+0001a2c0: 6666 203d 2031 3030 3030 0a0a 2020 2020  ff = 10000..    
+0001a2d0: 2020 2020 7265 706f 7274 203d 206f 732e      report = os.
+0001a2e0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e74  path.join(self.t
+0001a2f0: 656d 7064 6972 2c20 2266 696c 7465 7265  empdir, "filtere
+0001a300: 642e 7265 706f 7274 2229 0a20 2020 2020  d.report").     
+0001a310: 2020 2067 656e 6572 6174 655f 686f 7473     generate_hots
+0001a320: 706f 745f 7265 706f 7274 2822 7361 6d70  pot_report("samp
+0001a330: 6c65 3122 2c0a 2020 2020 2020 2020 2020  le1",.          
+0001a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a350: 2020 2020 2020 7265 706f 7274 2c0a 2020        report,.  
+0001a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a370: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0001a380: 7665 6c73 2c0a 2020 2020 2020 2020 2020  vels,.          
+0001a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3a0: 2020 2020 2020 7365 6c66 2e68 6f74 7370        self.hotsp
+0001a3b0: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
+0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3d0: 2020 2020 7365 6c66 2e76 6366 5f76 6570      self.vcf_vep
+0001a3e0: 202b 2022 2e67 7a22 2c0a 2020 2020 2020   + ".gz",.      
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a400: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+0001a410: 7663 6620 2b20 222e 677a 222c 0a20 2020  vcf + ".gz",.   
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a430: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a440: 662e 7265 6665 7265 6e63 652c 0a20 2020  f.reference,.   
+0001a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a470: 662e 7663 665f 7665 705f 776f 5f70 6963  f.vcf_vep_wo_pic
+0001a480: 6b20 2b20 222e 677a 222c 0a20 2020 2020  k + ".gz",.     
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2020 2020 2020 2020 2020 2022 7465 7374             "test
+0001a4b0: 732f 7574 696c 732f 6669 6c65 732f 7265  s/utils/files/re
+0001a4c0: 706f 7274 5f63 6f6c 756d 6e73 5f73 656c  port_columns_sel
+0001a4d0: 6563 745f 636f 6c75 6d6e 322e 7961 6d6c  ect_column2.yaml
+0001a4e0: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+0001a4f0: 6f70 656e 2872 6570 6f72 742c 2027 7227  open(report, 'r'
+0001a500: 2920 6173 2072 6570 6f72 745f 7265 7375  ) as report_resu
+0001a510: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
+0001a520: 6865 6164 203d 2072 6570 6f72 745f 7265  head = report_re
+0001a530: 7375 6c74 2e72 6561 646c 696e 6528 290a  sult.readline().
+0001a540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a550: 2e61 7373 6572 7445 7175 616c 2868 6561  .assertEqual(hea
+0001a560: 642e 7273 7472 6970 2829 2c20 225c 7422  d.rstrip(), "\t"
+0001a570: 2e6a 6f69 6e28 5b22 7361 6d70 6c65 222c  .join(["sample",
+0001a580: 2022 6368 7222 2c20 2273 7461 7274 222c   "chr", "start",
+0001a590: 2022 7374 6f70 222c 2022 7265 6622 2c20   "stop", "ref", 
+0001a5a0: 2261 6c74 222c 2022 7265 706f 7274 222c  "alt", "report",
+0001a5b0: 2027 6776 6366 5f64 6570 7468 272c 2022   'gvcf_depth', "
+0001a5c0: 7265 665f 6465 7074 6822 2c20 2261 6c74  ref_depth", "alt
+0001a5d0: 5f64 6570 7468 222c 2027 416e 616c 797a  _depth", 'Analyz
+0001a5e0: 6162 6c65 272c 2027 4d69 6e5f 7265 6164  able', 'Min_read
+0001a5f0: 5f64 6570 7468 3330 3027 2c20 2747 656e  _depth300', 'Gen
+0001a600: 6527 2c20 2254 7261 6e73 6372 6970 7422  e', "Transcript"
+0001a610: 2c20 2741 6d69 6e6f 5f61 6369 645f 6368  , 'Amino_acid_ch
+0001a620: 616e 6765 272c 2027 5661 7269 616e 745f  ange', 'Variant_
+0001a630: 7479 7065 272c 2027 436f 6e73 6571 7565  type', 'Conseque
+0001a640: 6e63 6527 2c20 2743 616c 6c65 7273 272c  nce', 'Callers',
+0001a650: 2027 436f 6d6d 656e 7427 2c20 274e 6f74   'Comment', 'Not
+0001a660: 5f45 6d70 7479 272c 2027 456d 7074 7927  _Empty', 'Empty'
+0001a670: 5d29 2920 2023 206e 6f71 610a 2020 2020  ]))  # noqa.    
+0001a680: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0001a690: 2072 6570 6f72 745f 7265 7375 6c74 2e72   report_result.r
+0001a6a0: 6561 646c 696e 6573 2829 0a20 2020 2020  eadlines().     
+0001a6b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001a6c0: 7274 4571 7561 6c28 6c65 6e28 7265 7375  rtEqual(len(resu
+0001a6d0: 6c74 292c 2033 3529 0a20 2020 2020 2020  lt), 35).       
+0001a6e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001a6f0: 4571 7561 6c28 7265 7375 6c74 5b30 5d2e  Equal(result[0].
+0001a700: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+0001a710: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
+0001a720: 3239 3434 3532 3731 0932 3934 3435 3237  29445271.2944527
+0001a730: 3109 4709 4109 312d 686f 7473 706f 7409  1.G.A.1-hotspot.
+0001a740: 3632 3009 3335 3909 3409 7965 7309 6f6b  620.359.4.yes.ok
+0001a750: 0941 4c4b 094e 4d5f 3030 3433 3034 2e34  .ALK.NM_004304.4
+0001a760: 094c 6575 3131 3532 0970 726f 7465 696e  .Leu1152.protein
+0001a770: 5f63 6f64 696e 6709 7379 6e6f 6e79 6d6f  _coding.synonymo
+0001a780: 7573 5f76 6172 6961 6e74 0976 6172 6469  us_variant.vardi
+0001a790: 6374 0972 6573 6973 7461 6e63 655f 6d75  ct.resistance_mu
+0001a7a0: 7461 7469 6f6e 0941 4c4b 092d 2229 2020  tation.ALK.-")  
+0001a7b0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+0001a7c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001a7d0: 7561 6c28 7265 7375 6c74 5b31 5d2e 7273  ual(result[1].rs
+0001a7e0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+0001a7f0: 094e 435f 3030 3030 3037 2e31 3309 3134  .NC_000007.13.14
+0001a800: 3034 3938 3335 3909 3134 3034 3938 3336  0498359.14049836
+0001a810: 3209 4354 5454 0943 0932 2d69 6e64 656c  2.CTTT.C.2-indel
+0001a820: 0931 3030 2e35 0932 3709 3409 7965 7309  .100.5.27.4.yes.
+0001a830: 6c6f 7709 4252 4146 0958 4d5f 3030 3532  low.BRAF.XM_0052
+0001a840: 3530 3034 352e 3109 2d09 7072 6f74 6569  50045.1.-.protei
+0001a850: 6e5f 636f 6469 6e67 0969 6e74 726f 6e5f  n_coding.intron_
+0001a860: 7661 7269 616e 7409 6d75 7465 6374 3209  variant.mutect2.
+0001a870: 2d09 4547 4652 092d 2229 2020 2320 6e6f  -.EGFR.-")  # no
+0001a880: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+0001a890: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001a8a0: 7265 7375 6c74 5b32 5d2e 7273 7472 6970  result[2].rstrip
+0001a8b0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+0001a8c0: 3030 3030 3037 2e31 3309 3134 3034 3938  000007.13.140498
+0001a8d0: 3336 3109 3134 3034 3938 3336 3109 2d09  361.140498361.-.
+0001a8e0: 2d09 312d 686f 7473 706f 7409 3131 3009  -.1-hotspot.110.
+0001a8f0: 2d09 2d09 7965 7309 6c6f 7709 4547 4652  -.-.yes.low.EGFR
+0001a900: 092d 092d 092d 092d 092d 092d 092d 0945  .-.-.-.-.-.-.-.E
+0001a910: 4746 5222 2920 2020 2320 6e6f 7161 0a20  GFR")   # noqa. 
+0001a920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a930: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0001a940: 6c74 5b33 5d2e 7273 7472 6970 2829 2c20  lt[3].rstrip(), 
+0001a950: 2273 616d 706c 6531 094e 435f 3030 3030  "sample1.NC_0000
+0001a960: 3037 2e31 3309 3134 3034 3533 3133 3609  07.13.140453136.
+0001a970: 3134 3034 3533 3133 3609 2d09 2d09 312d  140453136.-.-.1-
+0001a980: 686f 7473 706f 7409 3009 2d09 2d09 6e6f  hotspot.0.-.-.no
+0001a990: 7420 616e 616c 797a 6162 6c65 096c 6f77  t analyzable.low
+0001a9a0: 0942 5241 4609 2d09 2d09 2d09 2d09 2d09  .BRAF.-.-.-.-.-.
+0001a9b0: 2d09 2d09 4252 4146 2229 2020 2320 6e6f  -.-.BRAF")  # no
+0001a9c0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+0001a9d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001a9e0: 7265 7375 6c74 5b34 5d2e 7273 7472 6970  result[4].rstrip
+0001a9f0: 2829 2c20 2273 616d 706c 6531 094e 435f  (), "sample1.NC_
+0001aa00: 3030 3030 3037 2e31 3309 3131 3634 3132  000007.13.116412
+0001aa10: 3034 3309 3131 3634 3132 3034 3309 2d09  043.116412043.-.
+0001aa20: 2d09 312d 686f 7473 706f 7409 3009 2d09  -.1-hotspot.0.-.
+0001aa30: 2d09 6e6f 7420 616e 616c 797a 6162 6c65  -.not analyzable
+0001aa40: 096c 6f77 094d 4554 092d 092d 092d 092d  .low.MET.-.-.-.-
+0001aa50: 092d 092d 092d 094d 4554 2229 2020 2320  .-.-.-.MET")  # 
+0001aa60: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+0001aa70: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001aa80: 6c28 7265 7375 6c74 5b35 5d2e 7273 7472  l(result[5].rstr
+0001aa90: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+0001aaa0: 435f 3030 3030 3032 2e31 3109 3239 3434  C_000002.11.2944
+0001aab0: 3532 3731 0932 3934 3435 3237 3109 2d09  5271.29445271.-.
+0001aac0: 2d09 332d 6368 6563 6b09 3632 3009 2d09  -.3-check.620.-.
+0001aad0: 2d09 7965 7309 6f6b 0941 4c4b 092d 092d  -.yes.ok.ALK.-.-
+0001aae0: 092d 092d 092d 092d 092d 0941 4c4b 2229  .-.-.-.-.-.ALK")
+0001aaf0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+0001ab00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001ab10: 4571 7561 6c28 7265 7375 6c74 5b36 5d2e  Equal(result[6].
+0001ab20: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+0001ab30: 6531 094e 435f 3030 3030 3032 2e31 3109  e1.NC_000002.11.
+0001ab40: 3239 3434 3532 3732 0932 3934 3435 3237  29445272.2944527
+0001ab50: 3209 2d09 2d09 332d 6368 6563 6b09 3232  2.-.-.3-check.22
+0001ab60: 3109 2d09 2d09 7965 7309 6c6f 7709 414c  1.-.-.yes.low.AL
+0001ab70: 4b09 2d09 2d09 2d09 2d09 2d09 2d09 2d09  K.-.-.-.-.-.-.-.
+0001ab80: 414c 4b22 2920 2023 206e 6f71 610a 2020  ALK")  # noqa.  
+0001ab90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0001aba0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
+0001abb0: 745b 375d 2e72 7374 7269 7028 292c 2022  t[7].rstrip(), "
+0001abc0: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0001abd0: 322e 3131 0932 3934 3435 3237 3309 3239  2.11.29445273.29
+0001abe0: 3434 3532 3733 092d 092d 0933 2d63 6865  445273.-.-.3-che
+0001abf0: 636b 0936 3238 092d 092d 0979 6573 096f  ck.628.-.-.yes.o
+0001ac00: 6b09 414c 4b09 2d09 2d09 2d09 2d09 2d09  k.ALK.-.-.-.-.-.
+0001ac10: 2d09 2d09 414c 4b22 2920 2023 206e 6f71  -.-.ALK")  # noq
+0001ac20: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+0001ac30: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+0001ac40: 6573 756c 745b 385d 2e72 7374 7269 7028  esult[8].rstrip(
+0001ac50: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+0001ac60: 3030 3030 322e 3131 0932 3934 3435 3237  00002.11.2944527
+0001ac70: 3409 3239 3434 3532 3734 092d 092d 0933  4.29445274.-.-.3
+0001ac80: 2d63 6865 636b 0936 3138 092d 092d 0979  -check.618.-.-.y
+0001ac90: 6573 096f 6b09 414c 4b09 2d09 2d09 2d09  es.ok.ALK.-.-.-.
+0001aca0: 2d09 2d09 2d09 2d09 414c 4b22 2920 2023  -.-.-.-.ALK")  #
+0001acb0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+0001acc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001acd0: 616c 2872 6573 756c 745b 395d 2e72 7374  al(result[9].rst
+0001ace0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0001acf0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+0001ad00: 3435 3237 3509 3239 3434 3532 3735 092d  45275.29445275.-
+0001ad10: 092d 0933 2d63 6865 636b 0936 3038 092d  .-.3-check.608.-
+0001ad20: 092d 0979 6573 096f 6b09 414c 4b09 2d09  .-.yes.ok.ALK.-.
+0001ad30: 2d09 2d09 2d09 2d09 2d09 2d09 414c 4b22  -.-.-.-.-.-.ALK"
+0001ad40: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+0001ad50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001ad60: 7445 7175 616c 2872 6573 756c 745b 3130  tEqual(result[10
+0001ad70: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0001ad80: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0001ad90: 3109 3239 3434 3532 3736 0932 3934 3435  1.29445276.29445
+0001ada0: 3237 3609 2d09 2d09 332d 6368 6563 6b09  276.-.-.3-check.
+0001adb0: 3632 3109 2d09 2d09 7965 7309 6f6b 0941  621.-.-.yes.ok.A
+0001adc0: 4c4b 092d 092d 092d 092d 092d 092d 092d  LK.-.-.-.-.-.-.-
+0001add0: 0941 4c4b 2229 2020 2320 6e6f 7161 0a20  .ALK")  # noqa. 
+0001ade0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001adf0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0001ae00: 6c74 5b31 315d 2e72 7374 7269 7028 292c  lt[11].rstrip(),
+0001ae10: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0001ae20: 3030 322e 3131 0932 3934 3435 3237 3709  002.11.29445277.
+0001ae30: 3239 3434 3532 3737 092d 092d 0933 2d63  29445277.-.-.3-c
+0001ae40: 6865 636b 0931 3832 092d 092d 0979 6573  heck.182.-.-.yes
+0001ae50: 096c 6f77 0941 4c4b 092d 092d 092d 092d  .low.ALK.-.-.-.-
+0001ae60: 092d 092d 092d 0941 4c4b 2229 2020 2320  .-.-.-.ALK")  # 
+0001ae70: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+0001ae80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001ae90: 6c28 7265 7375 6c74 5b31 325d 2e72 7374  l(result[12].rst
+0001aea0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0001aeb0: 4e43 5f30 3030 3030 322e 3131 0932 3934  NC_000002.11.294
+0001aec0: 3435 3237 3809 3239 3434 3532 3738 092d  45278.29445278.-
+0001aed0: 092d 0933 2d63 6865 636b 0935 3530 092d  .-.3-check.550.-
+0001aee0: 092d 0979 6573 096f 6b09 414c 4b09 2d09  .-.yes.ok.ALK.-.
+0001aef0: 2d09 2d09 2d09 2d09 2d09 2d09 414c 4b22  -.-.-.-.-.-.ALK"
+0001af00: 2920 2023 206e 6f71 610a 2020 2020 2020  )  # noqa.      
+0001af10: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001af20: 7445 7175 616c 2872 6573 756c 745b 3133  tEqual(result[13
+0001af30: 5d2e 7273 7472 6970 2829 2c20 2273 616d  ].rstrip(), "sam
+0001af40: 706c 6531 094e 435f 3030 3030 3032 2e31  ple1.NC_000002.1
+0001af50: 3109 3239 3434 3532 3739 0932 3934 3435  1.29445279.29445
+0001af60: 3237 3909 2d09 2d09 332d 6368 6563 6b09  279.-.-.3-check.
+0001af70: 3539 3409 2d09 2d09 7965 7309 6f6b 0941  594.-.-.yes.ok.A
+0001af80: 4c4b 092d 092d 092d 092d 092d 092d 092d  LK.-.-.-.-.-.-.-
+0001af90: 0941 4c4b 2229 2020 2320 6e6f 7161 0a20  .ALK")  # noqa. 
+0001afa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001afb0: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0001afc0: 6c74 5b31 345d 2e72 7374 7269 7028 292c  lt[14].rstrip(),
+0001afd0: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0001afe0: 3030 322e 3131 0932 3934 3435 3238 3009  002.11.29445280.
+0001aff0: 3239 3434 3532 3830 092d 092d 0933 2d63  29445280.-.-.3-c
+0001b000: 6865 636b 0935 3339 092d 092d 0979 6573  heck.539.-.-.yes
+0001b010: 096f 6b09 414c 4b09 2d09 2d09 2d09 2d09  .ok.ALK.-.-.-.-.
+0001b020: 2d09 2d09 2d09 414c 4b22 2920 2023 206e  -.-.-.ALK")  # n
+0001b030: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+0001b040: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001b050: 2872 6573 756c 745b 3135 5d2e 7273 7472  (result[15].rstr
+0001b060: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+0001b070: 435f 3030 3030 3032 2e31 3109 3239 3434  C_000002.11.2944
+0001b080: 3532 3831 0932 3934 3435 3238 3109 2d09  5281.29445281.-.
+0001b090: 2d09 332d 6368 6563 6b09 3532 3609 2d09  -.3-check.526.-.
+0001b0a0: 2d09 7965 7309 6f6b 0941 4c4b 092d 092d  -.yes.ok.ALK.-.-
+0001b0b0: 092d 092d 092d 092d 092d 0941 4c4b 2229  .-.-.-.-.-.ALK")
+0001b0c0: 2020 2320 6e6f 7161 0a20 2020 2020 2020    # noqa.       
+0001b0d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001b0e0: 4571 7561 6c28 7265 7375 6c74 5b31 365d  Equal(result[16]
+0001b0f0: 2e72 7374 7269 7028 292c 2022 7361 6d70  .rstrip(), "samp
+0001b100: 6c65 3109 4e43 5f30 3030 3030 382e 3131  le1.NC_000008.11
+0001b110: 0931 3435 3733 3837 3635 0931 3435 3733  .145738765.14573
+0001b120: 3837 3635 092d 092d 0933 2d63 6865 636b  8765.-.-.3-check
+0001b130: 0931 3631 3609 2d09 2d09 7965 7309 6f6b  .1616.-.-.yes.ok
+0001b140: 092d 092d 092d 092d 092d 092d 092d 092d  .-.-.-.-.-.-.-.-
+0001b150: 092d 2229 2020 2320 6e6f 7161 0a20 2020  .-")  # noqa.   
+0001b160: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0001b170: 7365 7274 4571 7561 6c28 7265 7375 6c74  sertEqual(result
+0001b180: 5b31 375d 2e72 7374 7269 7028 292c 2022  [17].rstrip(), "
+0001b190: 7361 6d70 6c65 3109 4e43 5f30 3030 3030  sample1.NC_00000
+0001b1a0: 382e 3131 0931 3435 3733 3837 3636 0931  8.11.145738766.1
+0001b1b0: 3435 3733 3837 3636 092d 092d 0933 2d63  45738766.-.-.3-c
+0001b1c0: 6865 636b 0931 3631 3909 2d09 2d09 7965  heck.1619.-.-.ye
+0001b1d0: 7309 6f6b 092d 092d 092d 092d 092d 092d  s.ok.-.-.-.-.-.-
+0001b1e0: 092d 092d 092d 2229 2020 2320 6e6f 7161  .-.-.-")  # noqa
+0001b1f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001b200: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+0001b210: 7375 6c74 5b31 385d 2e72 7374 7269 7028  sult[18].rstrip(
+0001b220: 292c 2022 7361 6d70 6c65 3109 4e43 5f30  ), "sample1.NC_0
+0001b230: 3030 3030 382e 3131 0931 3435 3733 3837  00008.11.1457387
+0001b240: 3637 0931 3435 3733 3837 3637 092d 092d  67.145738767.-.-
+0001b250: 0933 2d63 6865 636b 0931 3539 3509 2d09  .3-check.1595.-.
+0001b260: 2d09 7965 7309 6f6b 092d 092d 092d 092d  -.yes.ok.-.-.-.-
+0001b270: 092d 092d 092d 092d 092d 2229 2020 2320  .-.-.-.-.-")  # 
+0001b280: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+0001b290: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001b2a0: 6c28 7265 7375 6c74 5b31 395d 2e72 7374  l(result[19].rst
+0001b2b0: 7269 7028 292c 2022 7361 6d70 6c65 3109  rip(), "sample1.
+0001b2c0: 4e43 5f30 3030 3030 382e 3131 0931 3435  NC_000008.11.145
+0001b2d0: 3733 3837 3638 0931 3435 3733 3837 3638  738768.145738768
+0001b2e0: 0947 0943 0933 2d63 6865 636b 0931 3534  .G.C.3-check.154
+0001b2f0: 3709 3509 3237 0979 6573 096f 6b09 4c52  7.5.27.yes.ok.LR
+0001b300: 5243 3134 094e 4d5f 3030 3132 3732 3033  RC14.NM_00127203
+0001b310: 362e 3109 2d09 7072 6f74 6569 6e5f 636f  6.1.-.protein_co
+0001b320: 6469 6e67 0975 7073 7472 6561 6d5f 6765  ding.upstream_ge
+0001b330: 6e65 5f76 6172 6961 6e74 0976 6172 6469  ne_variant.vardi
+0001b340: 6374 092d 092d 092d 2229 2020 2320 6e6f  ct.-.-.-")  # no
+0001b350: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+0001b360: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001b370: 7265 7375 6c74 5b32 305d 2e72 7374 7269  result[20].rstri
+0001b380: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0001b390: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+0001b3a0: 3837 3639 0931 3435 3733 3837 3639 092d  8769.145738769.-
+0001b3b0: 092d 0933 2d63 6865 636b 0931 3634 3409  .-.3-check.1644.
+0001b3c0: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+0001b3d0: 092d 092d 092d 092d 092d 092d 2229 2020  .-.-.-.-.-.-")  
+0001b3e0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+0001b3f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001b400: 7561 6c28 7265 7375 6c74 5b32 315d 2e72  ual(result[21].r
+0001b410: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0001b420: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
+0001b430: 3435 3733 3837 3730 0931 3435 3733 3837  45738770.1457387
+0001b440: 3730 092d 092d 0933 2d63 6865 636b 0931  70.-.-.3-check.1
+0001b450: 3636 3709 2d09 2d09 7965 7309 6f6b 092d  667.-.-.yes.ok.-
+0001b460: 092d 092d 092d 092d 092d 092d 092d 092d  .-.-.-.-.-.-.-.-
+0001b470: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+0001b480: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001b490: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
+0001b4a0: 325d 2e72 7374 7269 7028 292c 2022 7361  2].rstrip(), "sa
+0001b4b0: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
+0001b4c0: 3131 0931 3435 3733 3837 3731 0931 3435  11.145738771.145
+0001b4d0: 3733 3837 3731 092d 092d 0933 2d63 6865  738771.-.-.3-che
+0001b4e0: 636b 0931 3638 3509 2d09 2d09 7965 7309  ck.1685.-.-.yes.
+0001b4f0: 6f6b 092d 092d 092d 092d 092d 092d 092d  ok.-.-.-.-.-.-.-
+0001b500: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+0001b510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001b520: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0001b530: 6c74 5b32 335d 2e72 7374 7269 7028 292c  lt[23].rstrip(),
+0001b540: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0001b550: 3030 382e 3131 0931 3435 3733 3837 3732  008.11.145738772
+0001b560: 0931 3435 3733 3837 3732 092d 092d 0933  .145738772.-.-.3
+0001b570: 2d63 6865 636b 0931 3638 3909 2d09 2d09  -check.1689.-.-.
+0001b580: 7965 7309 6f6b 092d 092d 092d 092d 092d  yes.ok.-.-.-.-.-
+0001b590: 092d 092d 092d 092d 2229 2020 2320 6e6f  .-.-.-.-")  # no
+0001b5a0: 7161 0a20 2020 2020 2020 2020 2020 2073  qa.            s
+0001b5b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001b5c0: 7265 7375 6c74 5b32 345d 2e72 7374 7269  result[24].rstri
+0001b5d0: 7028 292c 2022 7361 6d70 6c65 3109 4e43  p(), "sample1.NC
+0001b5e0: 5f30 3030 3030 382e 3131 0931 3435 3733  _000008.11.14573
+0001b5f0: 3837 3733 0931 3435 3733 3837 3733 092d  8773.145738773.-
+0001b600: 092d 0933 2d63 6865 636b 0931 3934 3009  .-.3-check.1940.
+0001b610: 2d09 2d09 7965 7309 6f6b 092d 092d 092d  -.-.yes.ok.-.-.-
+0001b620: 092d 092d 092d 092d 092d 092d 2229 2020  .-.-.-.-.-.-")  
+0001b630: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+0001b640: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001b650: 7561 6c28 7265 7375 6c74 5b32 355d 2e72  ual(result[25].r
+0001b660: 7374 7269 7028 292c 2022 7361 6d70 6c65  strip(), "sample
+0001b670: 3109 4e43 5f30 3030 3030 382e 3131 0931  1.NC_000008.11.1
+0001b680: 3435 3733 3837 3734 0931 3435 3733 3837  45738774.1457387
+0001b690: 3734 092d 092d 0933 2d63 6865 636b 0931  74.-.-.3-check.1
+0001b6a0: 3934 3009 2d09 2d09 7965 7309 6f6b 092d  940.-.-.yes.ok.-
+0001b6b0: 092d 092d 092d 092d 092d 092d 092d 092d  .-.-.-.-.-.-.-.-
+0001b6c0: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+0001b6d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001b6e0: 7274 4571 7561 6c28 7265 7375 6c74 5b32  rtEqual(result[2
+0001b6f0: 365d 2e72 7374 7269 7028 292c 2022 7361  6].rstrip(), "sa
+0001b700: 6d70 6c65 3109 4e43 5f30 3030 3030 382e  mple1.NC_000008.
+0001b710: 3131 0931 3435 3733 3837 3735 0931 3435  11.145738775.145
+0001b720: 3733 3837 3735 092d 092d 0933 2d63 6865  738775.-.-.3-che
+0001b730: 636b 0931 3936 3309 2d09 2d09 7965 7309  ck.1963.-.-.yes.
+0001b740: 6f6b 092d 092d 092d 092d 092d 092d 092d  ok.-.-.-.-.-.-.-
+0001b750: 092d 092d 2229 2020 2320 6e6f 7161 0a20  .-.-")  # noqa. 
+0001b760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001b770: 6173 7365 7274 4571 7561 6c28 7265 7375  assertEqual(resu
+0001b780: 6c74 5b32 375d 2e72 7374 7269 7028 292c  lt[27].rstrip(),
+0001b790: 2022 7361 6d70 6c65 3109 4e43 5f30 3030   "sample1.NC_000
+0001b7a0: 3030 382e 3131 0931 3435 3733 3837 3736  008.11.145738776
+0001b7b0: 0931 3435 3733 3837 3736 092d 092d 0933  .145738776.-.-.3
+0001b7c0: 2d63 6865 636b 0930 092d 092d 096e 6f74  -check.0.-.-.not
+0001b7d0: 2061 6e61 6c79 7a61 626c 6509 6c6f 7709   analyzable.low.
+0001b7e0: 2d09 2d09 2d09 2d09 2d09 2d09 2d09 2d09  -.-.-.-.-.-.-.-.
+0001b7f0: 2d22 2920 2023 206e 6f71 610a 2020 2020  -")  # noqa.    
+0001b800: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001b810: 6572 7445 7175 616c 2872 6573 756c 745b  ertEqual(result[
+0001b820: 3238 5d2e 7273 7472 6970 2829 2c20 2273  28].rstrip(), "s
+0001b830: 616d 706c 6531 094e 435f 3030 3030 3038  ample1.NC_000008
+0001b840: 2e31 3109 3134 3537 3338 3737 3709 3134  .11.145738777.14
+0001b850: 3537 3338 3737 3709 2d09 2d09 332d 6368  5738777.-.-.3-ch
+0001b860: 6563 6b09 3139 3634 092d 092d 0979 6573  eck.1964.-.-.yes
+0001b870: 096f 6b09 2d09 2d09 2d09 2d09 2d09 2d09  .ok.-.-.-.-.-.-.
+0001b880: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+0001b890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b8a0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0001b8b0: 756c 745b 3239 5d2e 7273 7472 6970 2829  ult[29].rstrip()
+0001b8c0: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0001b8d0: 3030 3038 2e31 3109 3134 3537 3338 3737  0008.11.14573877
+0001b8e0: 3809 3134 3537 3338 3737 3809 2d09 2d09  8.145738778.-.-.
+0001b8f0: 332d 6368 6563 6b09 3139 3633 092d 092d  3-check.1963.-.-
+0001b900: 0979 6573 096f 6b09 2d09 2d09 2d09 2d09  .yes.ok.-.-.-.-.
+0001b910: 2d09 2d09 2d09 2d09 2d22 2920 2023 206e  -.-.-.-.-")  # n
+0001b920: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+0001b930: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001b940: 2872 6573 756c 745b 3330 5d2e 7273 7472  (result[30].rstr
+0001b950: 6970 2829 2c20 2273 616d 706c 6531 094e  ip(), "sample1.N
+0001b960: 435f 3030 3030 3038 2e31 3109 3134 3537  C_000008.11.1457
+0001b970: 3338 3737 3909 3134 3537 3338 3737 3909  38779.145738779.
+0001b980: 2d09 2d09 332d 6368 6563 6b09 3139 3538  -.-.3-check.1958
+0001b990: 092d 092d 0979 6573 096f 6b09 2d09 2d09  .-.-.yes.ok.-.-.
+0001b9a0: 2d09 2d09 2d09 2d09 2d09 2d09 2d22 2920  -.-.-.-.-.-.-") 
+0001b9b0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+0001b9c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001b9d0: 7175 616c 2872 6573 756c 745b 3331 5d2e  qual(result[31].
+0001b9e0: 7273 7472 6970 2829 2c20 2273 616d 706c  rstrip(), "sampl
+0001b9f0: 6531 094e 435f 3030 3030 3038 2e31 3109  e1.NC_000008.11.
+0001ba00: 3134 3537 3432 3531 3409 3134 3537 3432  145742514.145742
+0001ba10: 3531 3409 4109 4709 332d 6368 6563 6b09  514.A.G.3-check.
+0001ba20: 3009 3009 3833 3909 6e6f 7420 616e 616c  0.0.839.not anal
+0001ba30: 797a 6162 6c65 096c 6f77 0952 4543 514c  yzable.low.RECQL
+0001ba40: 3409 4e4d 5f30 3034 3236 302e 3309 5072  4.NM_004260.3.Pr
+0001ba50: 6f39 3209 7072 6f74 6569 6e5f 636f 6469  o92.protein_codi
+0001ba60: 6e67 0973 796e 6f6e 796d 6f75 735f 7661  ng.synonymous_va
+0001ba70: 7269 616e 7409 7661 7264 6963 742c 6d75  riant.vardict,mu
+0001ba80: 7465 6374 3209 2d09 2d09 2d22 2920 2023  tect2.-.-.-")  #
+0001ba90: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+0001baa0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001bab0: 616c 2872 6573 756c 745b 3332 5d2e 7273  al(result[32].rs
+0001bac0: 7472 6970 2829 2c20 2273 616d 706c 6531  trip(), "sample1
+0001bad0: 094e 435f 3030 3030 3136 2e31 3109 3831  .NC_000016.11.81
+0001bae0: 3935 3437 3839 0938 3139 3534 3738 3909  954789.81954789.
+0001baf0: 4309 4754 0932 2d69 6e64 656c 0931 3134  C.GT.2-indel.114
+0001bb00: 3409 3131 3732 0932 3909 7965 7309 6f6b  4.1172.29.yes.ok
+0001bb10: 0950 4c43 4732 094e 4d5f 3030 3236 3631  .PLCG2.NM_002661
+0001bb20: 2e33 092d 0970 726f 7465 696e 5f63 6f64  .3.-.protein_cod
+0001bb30: 696e 6709 696e 7472 6f6e 5f76 6172 6961  ing.intron_varia
+0001bb40: 6e74 0976 6172 6469 6374 092d 092d 092d  nt.vardict.-.-.-
+0001bb50: 2229 2020 2320 6e6f 7161 0a20 2020 2020  ")  # noqa.     
+0001bb60: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001bb70: 7274 4571 7561 6c28 7265 7375 6c74 5b33  rtEqual(result[3
+0001bb80: 335d 2e72 7374 7269 7028 292c 2022 7361  3].rstrip(), "sa
+0001bb90: 6d70 6c65 3109 4e43 5f30 3030 3030 322e  mple1.NC_000002.
+0001bba0: 3131 0932 3934 3435 3238 3209 3239 3434  11.29445282.2944
+0001bbb0: 3532 3832 0947 0941 0934 2d6f 7468 6572  5282.G.A.4-other
+0001bbc0: 0935 3230 0932 3834 0933 0979 6573 096f  .520.284.3.yes.o
+0001bbd0: 6b09 414c 4b09 4e4d 5f30 3034 3330 342e  k.ALK.NM_004304.
+0001bbe0: 3409 2d09 7072 6f74 6569 6e5f 636f 6469  4.-.protein_codi
+0001bbf0: 6e67 0973 706c 6963 655f 7265 6769 6f6e  ng.splice_region
+0001bc00: 5f76 6172 6961 6e74 2669 6e74 726f 6e5f  _variant&intron_
+0001bc10: 7661 7269 616e 7409 7661 7264 6963 7409  variant.vardict.
+0001bc20: 2d09 2d09 2d22 2920 2023 206e 6f71 610a  -.-.-")  # noqa.
+0001bc30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001bc40: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+0001bc50: 756c 745b 3334 5d2e 7273 7472 6970 2829  ult[34].rstrip()
+0001bc60: 2c20 2273 616d 706c 6531 094e 435f 3030  , "sample1.NC_00
+0001bc70: 3030 3136 2e31 3109 3831 3935 3437 3839  0016.11.81954789
+0001bc80: 0938 3139 3534 3738 3909 4309 4709 342d  .81954789.C.G.4-
+0001bc90: 6f74 6865 7209 3131 3434 0934 3432 0933  other.1144.442.3
+0001bca0: 3439 0979 6573 096f 6b09 5345 5054 094e  49.yes.ok.SEPT.N
+0001bcb0: 4d5f 3030 3236 3631 2e33 092d 0970 726f  M_002661.3.-.pro
+0001bcc0: 7465 696e 5f63 6f64 696e 6709 696e 7472  tein_coding.intr
+0001bcd0: 6f6e 5f76 6172 6961 6e74 0976 6172 6469  on_variant.vardi
+0001bce0: 6374 2c6d 7574 6563 7432 092d 092d 092d  ct,mutect2.-.-.-
+0001bcf0: 2229 2020 2320 6e6f 7161 0a0a 0a69 6620  ")  # noqa...if 
+0001bd00: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+0001bd10: 6169 6e5f 5f27 3a0a 2020 2020 696d 706f  ain__':.    impo
+0001bd20: 7274 206c 6f67 6769 6e67 0a20 2020 2069  rt logging.    i
+0001bd30: 6d70 6f72 7420 7379 730a 2020 2020 6c6f  mport sys.    lo
+0001bd40: 6767 696e 672e 6261 7369 6343 6f6e 6669  gging.basicConfi
+0001bd50: 6728 6c65 7665 6c3d 6c6f 6767 696e 672e  g(level=logging.
+0001bd60: 4352 4954 4943 414c 2c20 7374 7265 616d  CRITICAL, stream
+0001bd70: 3d73 7973 2e73 7464 6f75 742c 2066 6f72  =sys.stdout, for
+0001bd80: 6d61 743d 2725 286d 6573 7361 6765 2973  mat='%(message)s
+0001bd90: 2729 0a20 2020 2075 6e69 7474 6573 742e  ').    unittest.
+0001bda0: 6d61 696e 2829 0a                        main().
```

### Comparing `hydra_genetics-2.0.1/tests/utils/models/test_hotspot.py` & `hydra_genetics-3.0.0/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/test_misc.py` & `hydra_genetics-3.0.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/test_resources.py` & `hydra_genetics-3.0.0/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/test_samples.py` & `hydra_genetics-3.0.0/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/tests/utils/test_units.py` & `hydra_genetics-3.0.0/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `hydra_genetics-2.0.1/versioneer.py` & `hydra_genetics-3.0.0/versioneer.py`

 * *Files identical despite different names*

