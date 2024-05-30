# Comparing `tmp/bonsai_prp-0.8.3.tar.gz` & `tmp/bonsai_prp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai_prp-0.8.3.tar", last modified: Tue May 21 07:22:35 2024, max compression
+gzip compressed data, was "bonsai_prp-0.9.0.tar", last modified: Thu May 30 13:29:31 2024, max compression
```

## Comparing `bonsai_prp-0.8.3.tar` & `bonsai_prp-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.087234 bonsai_prp-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 07:22:35.087234 bonsai_prp-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.083234 bonsai_prp-0.8.3/bonsai_prp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 07:22:35.000000 bonsai_prp-0.8.3/bonsai_prp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.079234 bonsai_prp-0.8.3/prp/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.083234 bonsai_prp-0.8.3/prp/models/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/phenotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.083234 bonsai_prp-0.8.3/prp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.083234 bonsai_prp-0.8.3/prp/parse/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/mykrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/resfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/serotypefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/tbprofiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/phenotype/virulencefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/prp/parse/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:22:35.087234 bonsai_prp-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:35.083234 bonsai_prp-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-21 07:22:25.000000 bonsai_prp-0.8.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/bonsai_prp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 13:29:31.000000 bonsai_prp-0.9.0/bonsai_prp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.311885 bonsai_prp-0.9.0/prp/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.311885 bonsai_prp-0.9.0/prp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/phenotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/prp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/prp/parse/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/mykrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/resfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/serotypefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/shigapass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/tbprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/phenotype/virulencefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/prp/parse/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:29:31.315885 bonsai_prp-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-30 13:29:20.000000 bonsai_prp-0.9.0/tests/test_cli.py
```

### Comparing `bonsai_prp-0.8.3/LICENSE` & `bonsai_prp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/PKG-INFO` & `bonsai_prp-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.3
+Version: 0.9.0
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.3/README.md` & `bonsai_prp-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/bonsai_prp.egg-info/PKG-INFO` & `bonsai_prp-0.9.0/bonsai_prp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.3
+Version: 0.9.0
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.3/bonsai_prp.egg-info/SOURCES.txt` & `bonsai_prp-0.9.0/bonsai_prp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 prp/parse/utils.py
 prp/parse/variant.py
 prp/parse/phenotype/__init__.py
 prp/parse/phenotype/amrfinder.py
 prp/parse/phenotype/mykrobe.py
 prp/parse/phenotype/resfinder.py
 prp/parse/phenotype/serotypefinder.py
+prp/parse/phenotype/shigapass.py
 prp/parse/phenotype/tbprofiler.py
 prp/parse/phenotype/virulencefinder.py
 tests/test_cli.py
```

### Comparing `bonsai_prp-0.8.3/prp/cli.py` & `bonsai_prp-0.9.0/prp/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     parse_mlst_results,
     parse_mykrobe_amr_pred,
     parse_mykrobe_lineage_results,
     parse_postalignqc_results,
     parse_quast_results,
     parse_resfinder_amr_pred,
     parse_serotypefinder_oh_typing,
+    parse_shigapass_pred,
     parse_tbprofiler_amr_pred,
     parse_tbprofiler_lineage_results,
     parse_virulencefinder_stx_typing,
     parse_virulencefinder_vir_pred,
 )
 from .parse.metadata import get_database_info, get_gb_genome_version, parse_run_info
 from .parse.species import get_mykrobe_spp_prediction
@@ -100,14 +101,15 @@
     "-s",
     "--serotypefinder",
     type=click.Path(),
     help="Serotypefinder serotype prediction results",
 )
 @click.option("-p", "--quality", type=click.Path(), help="postalignqc qc results")
 @click.option("-k", "--mykrobe", type=click.Path(), help="mykrobe results")
+@click.option("-g", "--shigapass", type=click.Path(), help="shigapass results")
 @click.option("-t", "--tbprofiler", type=click.Path(), help="tbprofiler results")
 @click.option("--bam", type=click.Path(), help="Read mapping to reference genome")
 @click.option(
     "--reference-genome-fasta", type=click.Path(), help="reference genome fasta file"
 )
 @click.option(
     "--reference-genome-gff", type=click.Path(), help="reference-genome in gff format"
@@ -135,14 +137,15 @@
     mlst,
     cgmlst,
     virulencefinder,
     resfinder,
     serotypefinder,
     quality,
     mykrobe,
+    shigapass,
     tbprofiler,
     bam,
     reference_genome_fasta,
     reference_genome_gff,
     genome_annotation,
     snv_vcf,
     sv_vcf,
@@ -225,14 +228,21 @@
     if serotypefinder:
         LOG.info("Parse serotypefinder results")
         # OH typing
         res: MethodIndex | None = parse_serotypefinder_oh_typing(serotypefinder)
         if res is not None:
             results["typing_result"].extend(res)
 
+    if shigapass:
+        LOG.info("Parse shigapass results")
+        # Shigatyping
+        res: MethodIndex | None = parse_shigapass_pred(shigapass, TypingMethod.SHIGATYPE)
+        if res is not None:
+            results["typing_result"].extend(res)
+
     # species id
     results["species_prediction"] = []
     if kraken:
         LOG.info("Parse kraken results")
         results["species_prediction"].append(parse_kraken_result(kraken))
 
     # mycobacterium tuberculosis
```

### Comparing `bonsai_prp-0.8.3/prp/models/metadata.py` & `bonsai_prp-0.9.0/prp/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/models/phenotype.py` & `bonsai_prp-0.9.0/prp/models/phenotype.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     # what information substansiate the annotation
     reference: List[str] = Field([], description="References supporting trait")
     note: str | None = Field(None, description="Note, can be used for confidence score")
     source: str | None = Field(None, description="Source of variant")
 
 
 class DatabaseReference(RWModel):
-    """Refernece to a database."""
+    """Reference to a database."""
 
     ref_database: Optional[str] = None
     ref_id: Optional[str] = None
 
 
 class GeneBase(BaseModel):
     """Container for gene information"""
@@ -181,14 +181,28 @@
     phenotypes: List[PhenotypeInfo] = []
 
 
 class SerotypeGene(GeneBase):
     """Container for serotype gene information"""
 
 
+class Shigatype(BaseModel):
+    """Container for shigatype gene information"""
+
+    rfb: Optional[str] = None
+    rfb_hits: Optional[float] = None
+    mlst: Optional[str] = None
+    flic: Optional[str] = None
+    crispr: Optional[str] = None
+    ipah: Optional[str] = None
+    predicted_serotype: Optional[str] = None
+    predicted_flex_serotype: Optional[str] = None
+    comments: Optional[str] = None
+
+
 class VirulenceGene(GeneBase, DatabaseReference):
     """Container for virulence gene information"""
 
     depth: Optional[float] = Field(
         None, description="Amount of sequence data supporting the gene."
     )
```

### Comparing `bonsai_prp-0.8.3/prp/models/qc.py` & `bonsai_prp-0.9.0/prp/models/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/models/sample.py` & `bonsai_prp-0.9.0/prp/models/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 from .typing import (
     ResultLineageBase,
     TbProfilerLineage,
     TypingMethod,
     TypingResultCgMlst,
     TypingResultGeneAllele,
     TypingResultMlst,
+    TypingResultShiga,
     TypingSoftware,
 )
 
 
 class MethodIndex(RWModel):
     """Container for key-value lookup of analytical results."""
 
     type: Union[ElementType, TypingMethod]
     software: PredictionSoftware | TypingSoftware | None
     result: Union[
         ElementTypeResult,
         TypingResultMlst,
         TypingResultCgMlst,
         TypingResultGeneAllele,
+        TypingResultShiga,
         TbProfilerLineage,
         ResultLineageBase,
     ]
 
 
 class SampleBase(RWModel):
     """Base datamodel for sample data structure"""
```

### Comparing `bonsai_prp-0.8.3/prp/models/species.py` & `bonsai_prp-0.9.0/prp/models/species.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/models/tags.py` & `bonsai_prp-0.9.0/prp/models/tags.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/models/typing.py` & `bonsai_prp-0.9.0/prp/models/typing.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import Field
 
 from .base import RWModel
-from .phenotype import SerotypeGene, VirulenceGene
+from .phenotype import SerotypeGene, VirulenceGene, Shigatype
 
 
 class TypingSoftware(Enum):
     """Container for software names."""
 
     CHEWBBACA = "chewbbaca"
     MLST = "mlst"
     TBPROFILER = "tbprofiler"
     MYKROBE = "mykrobe"
     VIRULENCEFINDER = "virulencefinder"
     SEROTYPEFINDER = "serotypefinder"
+    SHIGAPASS = "shigapass"
 
 
 class TypingMethod(Enum):
     """Valid typing methods."""
 
     MLST = "mlst"
     CGMLST = "cgmlst"
     LINEAGE = "lineage"
     STX = "stx"
     OTYPE = "O_type"
     HTYPE = "H_type"
+    SHIGATYPE = "shigatype"
 
 
 class ChewbbacaErrors(str, Enum):
     """Chewbbaca error codes."""
 
     PLOT5 = "PLOT5"
     PLOT3 = "PLOT3"
@@ -67,14 +69,18 @@
 class TypingResultCgMlst(ResultMlstBase):
     """MLST results"""
 
     n_novel: int = Field(0, alias="nNovel")
     n_missing: int = Field(0, alias="nNovel")
 
 
+class TypingResultShiga(Shigatype):
+    """Shigatype results"""
+
+
 class ResultLineageBase(RWModel):
     """Lineage results"""
 
     lineage_depth: float | None = None
     main_lineage: str
     sublineage: str
```

### Comparing `bonsai_prp-0.8.3/prp/parse/__init__.py` & `bonsai_prp-0.9.0/prp/parse/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Parse output of softwares in pipeline."""
 
 from .phenotype import (
     parse_amrfinder_amr_pred,
     parse_amrfinder_vir_pred,
     parse_mykrobe_amr_pred,
     parse_resfinder_amr_pred,
+    parse_shigapass_pred,
     parse_tbprofiler_amr_pred,
     parse_virulencefinder_vir_pred,
 )
 from .qc import parse_alignment_results, parse_postalignqc_results, parse_quast_results
 from .species import parse_kraken_result
 from .typing import (
     parse_cgmlst_results,
```

### Comparing `bonsai_prp-0.8.3/prp/parse/metadata.py` & `bonsai_prp-0.9.0/prp/parse/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/amrfinder.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/mykrobe.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/mykrobe.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/resfinder.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/resfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/serotypefinder.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/serotypefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/tbprofiler.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/tbprofiler.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/phenotype/virulencefinder.py` & `bonsai_prp-0.9.0/prp/parse/phenotype/virulencefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/qc.py` & `bonsai_prp-0.9.0/prp/parse/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/species.py` & `bonsai_prp-0.9.0/prp/parse/species.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/typing.py` & `bonsai_prp-0.9.0/prp/parse/typing.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/utils.py` & `bonsai_prp-0.9.0/prp/parse/utils.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/prp/parse/variant.py` & `bonsai_prp-0.9.0/prp/parse/variant.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/pyproject.toml` & `bonsai_prp-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.3/tests/test_cli.py` & `bonsai_prp-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

