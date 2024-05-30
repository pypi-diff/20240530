# Comparing `tmp/yatotem2scdl-0.1.0.tar.gz` & `tmp/yatotem2scdl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatotem2scdl-0.1.0.tar", last modified: Wed May 29 15:58:45 2024, max compression
+gzip compressed data, was "yatotem2scdl-0.1.1.tar", last modified: Thu May 30 09:17:44 2024, max compression
```

## Comparing `yatotem2scdl-0.1.0.tar` & `yatotem2scdl-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:58:45.833033 yatotem2scdl-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.825033 yatotem2scdl-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/TotemMetadataHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/planDeCompte-vide.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/totem2xmlcsv.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_cas_alamarge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_etape_budgetaire.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_extraction_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_totem_budget_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.448803 yatotem2scdl-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.448803 yatotem2scdl-0.1.1/src/yatotem2scdl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/TotemMetadataHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/planDeCompte-vide.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/src/yatotem2scdl/xsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-30 09:17:38.000000 yatotem2scdl-0.1.1/src/yatotem2scdl/xsl/totem2xmlcsv.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 09:17:44.000000 yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:17:44.452803 yatotem2scdl-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-30 09:17:39.000000 yatotem2scdl-0.1.1/tests/test_cas_alamarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-30 09:17:39.000000 yatotem2scdl-0.1.1/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-30 09:17:39.000000 yatotem2scdl-0.1.1/tests/test_etape_budgetaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-30 09:17:39.000000 yatotem2scdl-0.1.1/tests/test_extraction_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-30 09:17:39.000000 yatotem2scdl-0.1.1/tests/test_totem_budget_metadata.py
```

### Comparing `yatotem2scdl-0.1.0/LICENSE` & `yatotem2scdl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/PKG-INFO` & `yatotem2scdl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatotem2scdl
-Version: 0.1.0
+Version: 0.1.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `yatotem2scdl-0.1.0/README.md` & `yatotem2scdl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/pyproject.toml` & `yatotem2scdl-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yatotem2scdl"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["lxml"]
 
 [project.scripts]
 yatotem2scdl = "yatotem2scdl.main:main"
```

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/TotemMetadataHandler.py` & `yatotem2scdl-0.1.1/src/yatotem2scdl/TotemMetadataHandler.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/conversion.py` & `yatotem2scdl-0.1.1/src/yatotem2scdl/conversion.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/data_structures.py` & `yatotem2scdl-0.1.1/src/yatotem2scdl/data_structures.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/exceptions.py` & `yatotem2scdl-0.1.1/src/yatotem2scdl/exceptions.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/main.py` & `yatotem2scdl-0.1.1/src/yatotem2scdl/main.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/totem2xmlcsv.xsl` & `yatotem2scdl-0.1.1/src/yatotem2scdl/xsl/totem2xmlcsv.xsl`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/PKG-INFO` & `yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatotem2scdl
-Version: 0.1.0
+Version: 0.1.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/SOURCES.txt` & `yatotem2scdl-0.1.1/src/yatotem2scdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/tests/test_cas_alamarge.py` & `yatotem2scdl-0.1.1/tests/test_cas_alamarge.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/tests/test_conversions.py` & `yatotem2scdl-0.1.1/tests/test_conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from csv_diff import load_csv, compare
 
 import pytest
 
 from yatotem2scdl import ConvertisseurTotemBudget, Options
 
 from data import PLANS_DE_COMPTE_PATH
-from data import test_case_dirs
+from data import examples_directories
 
 
 @pytest.mark.parametrize(
     "totem_path, expected_path",
-    [(d / "totem.xml", d / "expected.csv") for d in test_case_dirs() if isdir(d)],
+    [(d / "totem.xml", d / "expected.csv") for d in examples_directories() if isdir(d)],
 )
 def test_generation(totem_path: Path, expected_path: Path):
 
     _, candidate_file_str = tempfile.mkstemp(".csv")
     candidate_filepath = Path(candidate_file_str)
 
     xslt_custom = totem_path.parent / "totem2xmlcsv-custom.xsl"
```

### Comparing `yatotem2scdl-0.1.0/tests/test_etape_budgetaire.py` & `yatotem2scdl-0.1.1/tests/test_etape_budgetaire.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.1.0/tests/test_extraction_metadata.py` & `yatotem2scdl-0.1.1/tests/test_extraction_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from genericpath import isdir
 from pathlib import Path
 import pytest
-
-import pytest
+import time
 
 from yatotem2scdl import (
     ConvertisseurTotemBudget,
     AnneeExerciceInvalideErreur,
     EtapeBudgetaireInconnueErreur,
     ExtractionMetadataErreur,
     SiretInvalideErreur,
     TotemInvalideErreur,
+    EtapeBudgetaire,
 )
 
 from data import PLANS_DE_COMPTE_PATH, EXTRACT_METADATA_PATH
-from data import test_case_dirs
+from data import examples_directories
 
 
 @pytest.fixture
 def _convertisseur() -> ConvertisseurTotemBudget:
     return ConvertisseurTotemBudget()
 
-
 @pytest.mark.parametrize(
     "totem_path",
-    [(d / "totem.xml") for d in test_case_dirs() if isdir(d)],
+    [(d / "totem.xml") for d in examples_directories() if isdir(d)],
 )
 def test_parse_metadata_smoke(
     _convertisseur: ConvertisseurTotemBudget, totem_path: Path
 ):
 
     metadata = _convertisseur.totem_budget_metadata(
         totem_path, pdcs_dpath=PLANS_DE_COMPTE_PATH
@@ -37,14 +36,53 @@
 
     assert metadata.etape_budgetaire is not None
     assert metadata.annee_exercice is not None
     assert metadata.id_etablissement is not None
 
     # Le plan de compte peut etre None
 
+def test_parse_metadata_of_ca(_convertisseur: ConvertisseurTotemBudget):
+    totem_filep = EXTRACT_METADATA_PATH / "totem_ca_valide.xml"
+
+    metadata = _convertisseur.totem_budget_metadata(
+        totem_filep, pdcs_dpath=PLANS_DE_COMPTE_PATH
+    )
+    
+    assert metadata.annee_exercice == 2021
+    assert metadata.etape_budgetaire == EtapeBudgetaire.COMPTE_ADMIN
+    assert str(metadata.id_etablissement) == "22560001400016"
+    assert "M57/M57/" in str(metadata.plan_de_compte)
+
+def test_parse_metadata_of_cfu(_convertisseur: ConvertisseurTotemBudget):
+    totem_filep = EXTRACT_METADATA_PATH / "totem_cfu_valide.xml"
+
+    metadata = _convertisseur.totem_budget_metadata(
+        totem_filep, pdcs_dpath=PLANS_DE_COMPTE_PATH
+    )
+    
+    assert metadata.annee_exercice == 2023
+    assert metadata.etape_budgetaire == EtapeBudgetaire.CFU
+    assert str(metadata.id_etablissement) == "21560134500014"
+    assert "M57/M57_A" in str(metadata.plan_de_compte)
+
+def test_parse_metadata_performance(_convertisseur: ConvertisseurTotemBudget):
+    """
+    C'est un smoke test pour vérifier que la lecture des metadata reste relativement performante.
+    """
+    totem_filep = EXTRACT_METADATA_PATH / "totem_valid_huge.xml"
+
+    start = time.perf_counter_ns()
+    _convertisseur.totem_budget_metadata(
+        totem_filep, pdcs_dpath=PLANS_DE_COMPTE_PATH
+    )
+    end = time.perf_counter_ns()
+    elapsed_ns = end - start
+    
+    milli = 1_000_000
+    assert elapsed_ns < (80*milli), "Parser les metadata doit être une opération relativement performante."
 
 def test_parse_metadata_mauvais_siret(_convertisseur: ConvertisseurTotemBudget):
 
     totem_filep = EXTRACT_METADATA_PATH / "totem_mauvais_siret.xml"
 
     with pytest.raises(ExtractionMetadataErreur) as err:
         _convertisseur.totem_budget_metadata(totem_filep, PLANS_DE_COMPTE_PATH)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yatotem2scdl-0.1.0/tests/test_totem_budget_metadata.py` & `yatotem2scdl-0.1.1/tests/test_totem_budget_metadata.py`

 * *Files identical despite different names*

