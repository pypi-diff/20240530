# Comparing `tmp/pyontoenv-0.1.7a5.tar.gz` & `tmp/pyontoenv-0.1.7a6.tar.gz`

## Comparing `pyontoenv-0.1.7a5.tar` & `pyontoenv-0.1.7a6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0     1001      127      776 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/Cargo.toml
--rw-r--r--   0     1001      127  1689944 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/Brick-1.4-rc1.ttl
--rw-r--r--   0     1001      127  1599287 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/Brick-1.3.ttl
--rw-r--r--   0     1001      127     1248 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model
--rw-r--r--   0     1001      127      321 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.n3
--rw-r--r--   0     1001      127      537 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.xml
--rw-r--r--   0     1001      127      910 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   146214 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1001      127    30521 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   163975 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1001      127  1323794 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127    17472 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127  1456008 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127   104496 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1001      127  1255550 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/bacnet.ttl
--rw-r--r--   0     1001      127    44502 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/brickpatches.ttl
--rw-r--r--   0     1001      127    94738 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/dash.ttl
--rw-r--r--   0     1001      127    23951 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/dtype.xml
--rw-r--r--   0     1001      127    81761 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/rec.ttl
--rw-r--r--   0     1001      127     4069 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/recimports.ttl
--rw-r--r--   0     1001      127    11876 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/ref-schema.ttl
--rw-r--r--   0     1001      127    52899 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/shacl.ttl
--rw-r--r--   0     1001      127    15906 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/skos.ttl
--rw-r--r--   0     1001      127    61455 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/vaem.xml
--rw-r--r--   0     1001      127     1248 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/fileendings/model
--rw-r--r--   0     1001      127      321 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.n3
--rw-r--r--   0     1001      127      537 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.xml
--rw-r--r--   0     1001      127     1160 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/ont4.ttl
--rw-r--r--   0     1001      127      303 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology1.ttl
--rw-r--r--   0     1001      127      321 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology2.ttl
--rw-r--r--   0     1001      127      370 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology3.ttl
--rw-r--r--   0     1001      127      321 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology4.ttl
--rw-r--r--   0     1001      127      419 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology5.ttl
--rw-r--r--   0     1001      127      370 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/rdftest/ontology6.ttl
--rw-r--r--   0     1001      127     1160 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont4.ttl
--rw-r--r--   0     1001      127     1135 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v2/ont3.ttl
--rw-r--r--   0     1001      127     1129 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/fixtures/updates/v2/ont5.ttl
--rw-r--r--   0     1001      127     5324 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/config.rs
--rw-r--r--   0     1001      127     2180 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/consts.rs
--rw-r--r--   0     1001      127     3267 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/doctor.rs
--rw-r--r--   0     1001      127      350 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/errors.rs
--rw-r--r--   0     1001      127    31149 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/lib.rs
--rw-r--r--   0     1001      127    13820 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/ontology.rs
--rw-r--r--   0     1001      127     3521 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/policy.rs
--rw-r--r--   0     1001      127     4646 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/transform.rs
--rw-r--r--   0     1001      127     6501 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/src/util.rs
--rw-r--r--   0     1001      127    18418 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/lib/tests/ontoenv_test.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a5/python/Cargo.toml
--rw-r--r--   0     1001      127     2886 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/.gitignore
--rw-r--r--   0     1001      127      731 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/README.md
--rw-r--r--   0     1001      127       71 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/build.rs
--rw-r--r--   0     1001      127     5241 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/poetry.lock
--rw-r--r--   0     1001      127       71 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/requirements.dev.txt
--rw-r--r--   0     1001      127    14319 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/src/lib.rs
--rw-r--r--   0     1001      127      694 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/python/test.py
--rw-r--r--   0     1001      127    73227 2024-05-28 15:25:48.000000 pyontoenv-0.1.7a5/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a5/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a5/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a5/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/Cargo.toml
+-rw-r--r--   0     1001      127  1689944 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127  1599287 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model
+-rw-r--r--   0     1001      127      321 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.xml
+-rw-r--r--   0     1001      127      910 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    94738 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/dash.ttl
+-rw-r--r--   0     1001      127    23951 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/dtype.xml
+-rw-r--r--   0     1001      127    81761 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/ref-schema.ttl
+-rw-r--r--   0     1001      127    52899 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/shacl.ttl
+-rw-r--r--   0     1001      127    15906 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/skos.ttl
+-rw-r--r--   0     1001      127    61455 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/vaem.xml
+-rw-r--r--   0     1001      127     1248 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.xml
+-rw-r--r--   0     1001      127     1160 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/ont4.ttl
+-rw-r--r--   0     1001      127      303 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology1.ttl
+-rw-r--r--   0     1001      127      321 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology2.ttl
+-rw-r--r--   0     1001      127      370 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology3.ttl
+-rw-r--r--   0     1001      127      321 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology4.ttl
+-rw-r--r--   0     1001      127      419 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology5.ttl
+-rw-r--r--   0     1001      127      370 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/rdftest/ontology6.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/fixtures/updates/v2/ont5.ttl
+-rw-r--r--   0     1001      127     5324 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/errors.rs
+-rw-r--r--   0     1001      127    31136 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/lib.rs
+-rw-r--r--   0     1001      127    14000 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6501 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/src/util.rs
+-rw-r--r--   0     1001      127    17905 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/lib/tests/ontoenv_test.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a6/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/README.md
+-rw-r--r--   0     1001      127       71 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14415 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-05-30 00:53:27.000000 pyontoenv-0.1.7a6/python/test.py
+-rw-r--r--   0     1001      127    73227 2024-05-30 00:53:26.000000 pyontoenv-0.1.7a6/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a6/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a6/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a6/PKG-INFO
```

### Comparing `pyontoenv-0.1.7a5/lib/Cargo.toml` & `pyontoenv-0.1.7a6/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/Brick-1.3.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.nt` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/model.xml` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/bacnet.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/brickpatches.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/dash.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/dash.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/dtype.xml` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/dtype.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/rec.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/recimports.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/ref-schema.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/shacl.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/shacl.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/skos.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/skos.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/brick-stuff/support/vaem.xml` & `pyontoenv-0.1.7a6/lib/fixtures/brick-stuff/support/vaem.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/fileendings/model` & `pyontoenv-0.1.7a6/lib/fixtures/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.nt` & `pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/fileendings/model.xml` & `pyontoenv-0.1.7a6/lib/fixtures/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/ont1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/ont2.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/ont3.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/ont4.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont1.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont2.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont3.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v1/ont4.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v2/ont3.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/fixtures/updates/v2/ont5.ttl` & `pyontoenv-0.1.7a6/lib/fixtures/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/config.rs` & `pyontoenv-0.1.7a6/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/consts.rs` & `pyontoenv-0.1.7a6/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/doctor.rs` & `pyontoenv-0.1.7a6/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/lib.rs` & `pyontoenv-0.1.7a6/lib/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     Dataset, Graph, GraphName, NamedNode, NamedNodeRef, NamedOrBlankNode, QuadRef, SubjectRef,
 };
 use oxigraph::store::Store;
 use petgraph::graph::{Graph as DiGraph, NodeIndex};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::collections::{HashSet, VecDeque};
-use std::fs;
 use std::io::{BufReader, Write};
 use std::path::Path;
 
 // custom derive for ontologies field as vec of Ontology
 fn ontologies_ser<S>(
     ontologies: &HashMap<GraphIdentifier, Ontology>,
     s: S,
```

### Comparing `pyontoenv-0.1.7a5/lib/src/ontology.rs` & `pyontoenv-0.1.7a6/lib/src/ontology.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use oxigraph::model::{
     Graph as OxigraphGraph, GraphName, NamedNode, NamedNodeRef, Subject, SubjectRef, TermRef,
 };
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use serde_with::{serde_as, DeserializeAs, SerializeAs};
 use std::collections::HashMap;
 use std::path::PathBuf;
+use std::hash::Hash;
 //
 // custom derive for NamedNode
 fn namednode_ser<S>(namednode: &NamedNode, serializer: S) -> Result<S::Ok, S::Error>
 where
     S: serde::Serializer,
 {
     serializer.serialize_str(namednode.as_str())
@@ -23,28 +24,35 @@
 where
     D: serde::Deserializer<'de>,
 {
     let s = String::deserialize(deserializer)?;
     NamedNode::new(s).map_err(serde::de::Error::custom)
 }
 
-#[derive(Serialize, Deserialize, Eq, Debug, Clone, Hash)]
+#[derive(Serialize, Deserialize, Eq, Debug, Clone)]
 pub struct GraphIdentifier {
     location: OntologyLocation,
     #[serde(serialize_with = "namednode_ser", deserialize_with = "namednode_de")]
     name: NamedNode,
 }
 
 // equality for GraphIdentifier is based on the name and location
 impl PartialEq for GraphIdentifier {
     fn eq(&self, other: &Self) -> bool {
         self.name == other.name && self.location == other.location
     }
 }
 
+impl Hash for GraphIdentifier {
+    fn hash<H: std::hash::Hasher>(&self, state: &mut H) {
+        self.name.hash(state);
+        self.location.hash(state);
+    }
+}
+
 impl GraphIdentifier {
     pub fn location(&self) -> &OntologyLocation {
         &self.location
     }
 
     pub fn name(&self) -> NamedNodeRef {
         self.name.as_ref()
```

### Comparing `pyontoenv-0.1.7a5/lib/src/policy.rs` & `pyontoenv-0.1.7a6/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/transform.rs` & `pyontoenv-0.1.7a6/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/src/util.rs` & `pyontoenv-0.1.7a6/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/lib/tests/ontoenv_test.rs` & `pyontoenv-0.1.7a6/lib/tests/ontoenv_test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 use anyhow::Result;
-use chrono::prelude::*;
-use log::{debug, error, info, warn};
 use ontoenv::config::Config;
-use ontoenv::doctor::{Doctor, DuplicateOntology, OntologyDeclaration};
-use ontoenv::ontology::{GraphIdentifier, Ontology, OntologyLocation};
+use ontoenv::ontology::OntologyLocation;
 use ontoenv::OntoEnv;
-use oxigraph::model::{
-    Dataset, Graph, GraphName, NamedNode, NamedNodeRef, NamedOrBlankNode, QuadRef, SubjectRef,
-};
-use oxigraph::store::Store;
-use petgraph::graph::{Graph as DiGraph, NodeIndex};
-use serde::{Deserialize, Serialize};
-use std::collections::HashMap;
-use std::collections::{HashSet, VecDeque};
-use std::fs;
-use std::io::{BufReader, Write};
-use std::path::Path;
+use oxigraph::model::NamedNodeRef;
 use std::path::PathBuf;
 use tempdir::TempDir;
 
 // the tests directory contains a number of test files that are used to test the OntoEnv.
 // Each has a unique name and they all exist in a flat folder.
 // This is a macro which takes a list of strings describing the directory structure of a
 // test directory and creates a temporary directory with the given structure. The strings
@@ -226,15 +213,15 @@
 fn test_recreate() -> Result<()> {
     let dir = TempDir::new("ontoenv")?;
     setup!(&dir, { "fixtures/ont1.ttl" => "ont1.ttl", 
                    "fixtures/ont2.ttl" => "ont2.ttl",
                    "fixtures/ont3.ttl" => "ont3.ttl",
                    "fixtures/ont4.ttl" => "ont4.ttl" });
     let cfg = default_config(&dir);
-    let mut env = OntoEnv::new(cfg, false)?;
+    let env = OntoEnv::new(cfg, false)?;
     // create a new env, like above, but make sure it raises an error
     let cfg = default_config(&dir);
     let env = OntoEnv::new(cfg, false);
     assert!(env.is_err());
 
     let cfg = default_config(&dir);
     let env = OntoEnv::new(cfg, true)?;
@@ -424,15 +411,15 @@
     let mut env = OntoEnv::new(cfg, false)?;
     env.update()?;
 
     assert_eq!(env.num_graphs(), 21);
 
     let ont1 = NamedNodeRef::new("https://brickschema.org/schema/1.3/Brick")?;
     let ont_graph = env.get_ontology_by_name(ont1).unwrap();
-    let closure = env.get_dependency_closure(&ont_graph.id()).unwrap();
+    let closure = env.get_dependency_closure(ont_graph.id()).unwrap();
     assert_eq!(closure.len(), 19);
     teardown(dir);
     Ok(())
 }
 
 #[test]
 fn test_ontoenv_dag_structure() -> Result<()> {
@@ -452,35 +439,35 @@
     assert_eq!(env.num_graphs(), 6);
 
     // ont2 => {ont2, ont1}
 
     // get the graph for ontology2
     let ont2 = NamedNodeRef::new("http://example.org/ontology2")?;
     let ont_graph = env.get_ontology_by_name(ont2).unwrap();
-    let closure = env.get_dependency_closure(&ont_graph.id()).unwrap();
+    let closure = env.get_dependency_closure(ont_graph.id()).unwrap();
     assert_eq!(closure.len(), 2);
     let union = env.get_union_graph(&closure, None, None)?;
     assert_eq!(union.len(), 4);
     let union = env.get_union_graph(&closure, None, Some(false))?;
     assert_eq!(union.len(), 5);
 
     // ont3 => {ont3, ont2, ont1}
     let ont3 = NamedNodeRef::new("http://example.org/ontology3")?;
     let ont_graph = env.get_ontology_by_name(ont3).unwrap();
-    let closure = env.get_dependency_closure(&ont_graph.id()).unwrap();
+    let closure = env.get_dependency_closure(ont_graph.id()).unwrap();
     assert_eq!(closure.len(), 3);
     let union = env.get_union_graph(&closure, None, None)?;
     assert_eq!(union.len(), 5);
     let union = env.get_union_graph(&closure, None, Some(false))?;
     assert_eq!(union.len(), 8);
 
     // ont5 => {ont5, ont4, ont3, ont2, ont1}
     let ont5 = NamedNodeRef::new("http://example.org/ontology5")?;
     let ont_graph = env.get_ontology_by_name(ont5).unwrap();
-    let closure = env.get_dependency_closure(&ont_graph.id()).unwrap();
+    let closure = env.get_dependency_closure(ont_graph.id()).unwrap();
     assert_eq!(closure.len(), 5);
     let union = env.get_union_graph(&closure, None, None)?;
     assert_eq!(union.len(), 7);
     let union = env.get_union_graph(&closure, None, Some(false))?;
     // print the union
     assert_eq!(union.len(), 14);
```

### Comparing `pyontoenv-0.1.7a5/python/Cargo.toml` & `pyontoenv-0.1.7a6/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/python/.github/workflows/CI.yml` & `pyontoenv-0.1.7a6/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/python/.gitignore` & `pyontoenv-0.1.7a6/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/python/README.md` & `pyontoenv-0.1.7a6/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/python/poetry.lock` & `pyontoenv-0.1.7a6/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/python/src/lib.rs` & `pyontoenv-0.1.7a6/python/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,16 @@
     }
 
     fn import_dependencies(&self, py: Python, graph: &Bound<'_, PyAny>) -> PyResult<()> {
         let rdflib = py.import_bound("rdflib")?;
         let py_rdf_type = term_to_python(py, &rdflib, Term::NamedNode(TYPE.into()))?;
         let py_ontology = term_to_python(py, &rdflib, Term::NamedNode(ONTOLOGY.into()))?;
         let value_fun: Py<PyAny> = graph.getattr("value")?.into();
-        let ontology = value_fun.call1(py, (py_rdf_type, py_ontology))?;
+        let kwargs =  [("predicate", py_rdf_type), ("object", py_ontology)].into_py_dict_bound(py);
+        let ontology = value_fun.call_bound(py, (), Some(&kwargs))?;
 
         if ontology.is_none(py) {
             return Ok(());
         }
 
         let ontology = ontology.to_string();
```

### Comparing `pyontoenv-0.1.7a5/python/test.py` & `pyontoenv-0.1.7a6/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a5/Cargo.lock` & `pyontoenv-0.1.7a6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.7-a5"
+version = "0.1.7-a6"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1401,15 +1401,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.7-a5"
+version = "0.1.7-a6"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1719,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.7-a5"
+version = "0.1.7-a6"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.7a5/Cargo.toml` & `pyontoenv-0.1.7a6/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.7-a5"
+version = "0.1.7-a6"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -27,8 +27,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.7-a5", path = "lib" }
+ontoenv = { version = "0.1.7-a6", path = "lib" }
```

### Comparing `pyontoenv-0.1.7a5/pyproject.toml` & `pyontoenv-0.1.7a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.7a5"
+version = "0.1.7a6"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pyontoenv-0.1.7a5/PKG-INFO` & `pyontoenv-0.1.7a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.7a5
+Version: 0.1.7a6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

