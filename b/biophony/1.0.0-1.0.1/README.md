# Comparing `tmp/biophony-1.0.0.tar.gz` & `tmp/biophony-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biophony-1.0.0.tar", last modified: Fri May 17 11:37:19 2024, max compression
+gzip compressed data, was "biophony-1.0.1.tar", last modified: Thu May 30 11:24:23 2024, max compression
```

## Comparing `biophony-1.0.0.tar` & `biophony-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 pierrick  (1000) pierrick  (1000)        0 2024-05-17 11:37:19.389960 biophony-1.0.0/
--rw-------   0 pierrick  (1000) pierrick  (1000)    21782 2024-05-17 08:22:23.000000 biophony-1.0.0/LICENSE
--rw-r--r--   0 pierrick  (1000) pierrick  (1000)    27078 2024-05-17 11:37:19.389960 biophony-1.0.0/PKG-INFO
--rw-------   0 pierrick  (1000) pierrick  (1000)      139 2024-05-17 08:22:23.000000 biophony-1.0.0/README.md
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1092 2024-05-17 11:03:01.000000 biophony-1.0.0/pyproject.toml
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)       38 2024-05-17 11:37:19.389960 biophony-1.0.0/setup.cfg
-drwxrwxr-x   0 pierrick  (1000) pierrick  (1000)        0 2024-05-17 11:37:19.385960 biophony-1.0.0/src/
-drwxrwxr-x   0 pierrick  (1000) pierrick  (1000)        0 2024-05-17 11:37:19.386960 biophony-1.0.0/src/biophony/
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      517 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/__init__.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1239 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/bio_seq.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1575 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/bio_seq_gen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1543 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/bio_seq_var_gen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1477 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/elem_seq.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1425 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/elem_seq_gen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2433 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/elem_seq_var_gen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2379 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/elements.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1365 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/fasta_writer.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1348 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/fastagen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2443 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/fastavargen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     5127 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/gencov.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2444 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/genvcf.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1293 2024-05-17 11:03:01.000000 biophony-1.0.0/src/biophony/variant_maker.py
-drwxrwxr-x   0 pierrick  (1000) pierrick  (1000)        0 2024-05-17 11:37:19.388960 biophony-1.0.0/src/biophony.egg-info/
--rw-r--r--   0 pierrick  (1000) pierrick  (1000)    27078 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/PKG-INFO
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1084 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/SOURCES.txt
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)        1 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/dependency_links.txt
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      112 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/entry_points.txt
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)       87 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/requires.txt
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)        9 2024-05-17 11:37:19.000000 biophony-1.0.0/src/biophony.egg-info/top_level.txt
-drwxrwxr-x   0 pierrick  (1000) pierrick  (1000)        0 2024-05-17 11:37:19.388960 biophony-1.0.0/tests/
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      531 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_005_elements.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1021 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_010_elemseq.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      976 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_015_elemseqgen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      308 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_016_elemseqvargen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1437 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_020_bioseq.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      224 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_025_bioseqgen.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      466 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_040_variantmaker.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1913 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_090_fasta_writer.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      265 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_100_gencov.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     3370 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_150_gencov_script.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      154 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_200_genfasta.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     3801 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_250_genfasta_script.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2394 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_350_genvcf_script.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1597 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_400_genfastavariants.py
--rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1416 2024-05-17 11:03:01.000000 biophony-1.0.0/tests/test_450_genfastavariant_script.py
+drwx------   0 pierrick  (1000) pierrick  (1000)        0 2024-05-30 11:24:23.826020 biophony-1.0.1/
+-rw-------   0 pierrick  (1000) pierrick  (1000)    21782 2024-05-17 08:22:23.000000 biophony-1.0.1/LICENSE
+-rw-r--r--   0 pierrick  (1000) pierrick  (1000)    27246 2024-05-30 11:24:23.825020 biophony-1.0.1/PKG-INFO
+-rw-------   0 pierrick  (1000) pierrick  (1000)      307 2024-05-30 11:21:44.000000 biophony-1.0.1/README.md
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1092 2024-05-30 11:19:52.000000 biophony-1.0.1/pyproject.toml
+-rw-------   0 pierrick  (1000) pierrick  (1000)       38 2024-05-30 11:24:23.826020 biophony-1.0.1/setup.cfg
+drwx------   0 pierrick  (1000) pierrick  (1000)        0 2024-05-30 11:24:23.820020 biophony-1.0.1/src/
+drwx------   0 pierrick  (1000) pierrick  (1000)        0 2024-05-30 11:24:23.823020 biophony-1.0.1/src/biophony/
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      517 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/__init__.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1239 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/bio_seq.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1575 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/bio_seq_gen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1543 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/bio_seq_var_gen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1477 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/elem_seq.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1425 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/elem_seq_gen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2433 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/elem_seq_var_gen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2379 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/elements.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1365 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/fasta_writer.py
+-rw-------   0 pierrick  (1000) pierrick  (1000)     1531 2024-05-30 07:39:51.000000 biophony-1.0.1/src/biophony/fastagen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2443 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/fastavargen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     5127 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/gencov.py
+-rw-------   0 pierrick  (1000) pierrick  (1000)     2521 2024-05-30 07:39:51.000000 biophony-1.0.1/src/biophony/genvcf.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1293 2024-05-17 11:03:01.000000 biophony-1.0.1/src/biophony/variant_maker.py
+drwx------   0 pierrick  (1000) pierrick  (1000)        0 2024-05-30 11:24:23.825020 biophony-1.0.1/src/biophony.egg-info/
+-rw-r--r--   0 pierrick  (1000) pierrick  (1000)    27246 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/PKG-INFO
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1084 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)        1 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      112 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/entry_points.txt
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)       87 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/requires.txt
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)        9 2024-05-30 11:24:23.000000 biophony-1.0.1/src/biophony.egg-info/top_level.txt
+drwx------   0 pierrick  (1000) pierrick  (1000)        0 2024-05-30 11:24:23.824020 biophony-1.0.1/tests/
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      531 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_005_elements.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1021 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_010_elemseq.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      976 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_015_elemseqgen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      308 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_016_elemseqvargen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1437 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_020_bioseq.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      224 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_025_bioseqgen.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      466 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_040_variantmaker.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1913 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_090_fasta_writer.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      265 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_100_gencov.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     3370 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_150_gencov_script.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)      154 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_200_genfasta.py
+-rw-------   0 pierrick  (1000) pierrick  (1000)     4051 2024-05-30 07:39:51.000000 biophony-1.0.1/tests/test_250_genfasta_script.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     2394 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_350_genvcf_script.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1597 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_400_genfastavariants.py
+-rw-rw-r--   0 pierrick  (1000) pierrick  (1000)     1416 2024-05-17 11:03:01.000000 biophony-1.0.1/tests/test_450_genfastavariant_script.py
```

### Comparing `biophony-1.0.0/LICENSE` & `biophony-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/PKG-INFO` & `biophony-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biophony
-Version: 1.0.0
+Version: 1.0.1
 Summary: Random generation of genetic files
 Author-email: Pierrick ROGER <pierrick.roger@cea.fr>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
         
         Version 2.1 dated 2013-06-21
         
@@ -543,7 +543,14 @@
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 # Genetic sequence data files generator
 
 Used for generating data files (Coverage files, VCF files, ...) in order to
 test database design.
+
+## NEWS
+
+### 2024-05-30 v1.0.1
+
+ * gen-vcf: correct usage of file path to pass to mutation-simulator.
+ * gen-fasta: disable header tag line (comment line) by default.
```

### Comparing `biophony-1.0.0/pyproject.toml` & `biophony-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biophony"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name="Pierrick ROGER", email="pierrick.roger@cea.fr"}
 ]
 description = "Random generation of genetic files"
 license = {file="LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `biophony-1.0.0/src/biophony/__init__.py` & `biophony-1.0.1/src/biophony/__init__.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/bio_seq.py` & `biophony-1.0.1/src/biophony/bio_seq.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/bio_seq_gen.py` & `biophony-1.0.1/src/biophony/bio_seq_gen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/bio_seq_var_gen.py` & `biophony-1.0.1/src/biophony/bio_seq_var_gen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/elem_seq.py` & `biophony-1.0.1/src/biophony/elem_seq.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/elem_seq_gen.py` & `biophony-1.0.1/src/biophony/elem_seq_gen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/elem_seq_var_gen.py` & `biophony-1.0.1/src/biophony/elem_seq_var_gen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/elements.py` & `biophony-1.0.1/src/biophony/elements.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/fasta_writer.py` & `biophony-1.0.1/src/biophony/fasta_writer.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/fastagen.py` & `biophony-1.0.1/src/biophony/fastagen.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,26 +13,28 @@
         help='The length of the generated sequence.')
     parser.add_argument('--line-size', dest='line_size', default=80, type=int,
         help='Maximum number of characters on each line.')
     parser.add_argument('-e', '--elements', dest='elements', default='ACTG',
         help='The set of elements to use.')
     parser.add_argument('-s', '--seqid', dest='seqid', default='chr',
         help='SeqID.')
+    parser.add_argument('-H', '--header', dest='header', action=argparse.BooleanOptionalAction,
+        help='Add generation metadata in the fasta file header.')
     args = parser.parse_args()
     return args
 
 def fastagen_cli() -> None:
     """FASTA generation CLI.
     """
 
     args = read_args()
 
     gen = BioSeqGen(elements = Elements(args.elements),
                     seqlen = args.length, prefix_id = args.seqid)
-    writer = FastaWriter(output = sys.stdout, seq_line_len = args.line_size)
+    writer = FastaWriter(output = sys.stdout, seq_line_len = args.line_size, header= args.header)
     for seq in gen:
         writer.write_bio_seq(seq)
 
     sys.exit(0)
 
 if __name__ == '__main__':
     fastagen_cli()
```

### Comparing `biophony-1.0.0/src/biophony/fastavargen.py` & `biophony-1.0.1/src/biophony/fastavargen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/gencov.py` & `biophony-1.0.1/src/biophony/gencov.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony/genvcf.py` & `biophony-1.0.1/src/biophony/genvcf.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     try:
         # Write FASTA data if received from stdin
         if args.fasta_file == '-':
             args.fasta_file = os.path.join(tmp_dir, 'seq.fasta')
             with open(args.fasta_file, 'w', encoding="utf-8") as f:
                 for line in sys.stdin:
                     f.write(line)
+        else:
+            args.fasta_file = os.path.abspath(args.fasta_file)
 
         # Enter temp folder
         os.chdir(tmp_dir)
 
         # Call mutation-simulator script
         cmd = ["mutation-simulator", "-q", "-o", "variant", args.fasta_file,
                "args", "-sn", str(args.snp_rate), "-de", str(args.del_rate),
```

### Comparing `biophony-1.0.0/src/biophony/variant_maker.py` & `biophony-1.0.1/src/biophony/variant_maker.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/src/biophony.egg-info/PKG-INFO` & `biophony-1.0.1/src/biophony.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biophony
-Version: 1.0.0
+Version: 1.0.1
 Summary: Random generation of genetic files
 Author-email: Pierrick ROGER <pierrick.roger@cea.fr>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
         
         Version 2.1 dated 2013-06-21
         
@@ -543,7 +543,14 @@
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 # Genetic sequence data files generator
 
 Used for generating data files (Coverage files, VCF files, ...) in order to
 test database design.
+
+## NEWS
+
+### 2024-05-30 v1.0.1
+
+ * gen-vcf: correct usage of file path to pass to mutation-simulator.
+ * gen-fasta: disable header tag line (comment line) by default.
```

### Comparing `biophony-1.0.0/src/biophony.egg-info/SOURCES.txt` & `biophony-1.0.1/src/biophony.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_005_elements.py` & `biophony-1.0.1/tests/test_005_elements.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_010_elemseq.py` & `biophony-1.0.1/tests/test_010_elemseq.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_015_elemseqgen.py` & `biophony-1.0.1/tests/test_015_elemseqgen.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_020_bioseq.py` & `biophony-1.0.1/tests/test_020_bioseq.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_090_fasta_writer.py` & `biophony-1.0.1/tests/test_090_fasta_writer.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_150_gencov_script.py` & `biophony-1.0.1/tests/test_150_gencov_script.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_250_genfasta_script.py` & `biophony-1.0.1/tests/test_250_genfasta_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,105 +4,120 @@
 import re
 import subprocess
 
 script_path = os.path.realpath(__file__)
 testdir = os.path.dirname(script_path)
 cmd = ['python', '-c', 'import biophony; biophony.fastagen_cli()']
 
+
 def test_help():
     for opt in ['-h', '--help']:
         with subprocess.Popen(cmd + [opt], stdout=subprocess.PIPE) as proc:
             assert proc.wait() == 0
 
+
 def test_default():
     with subprocess.Popen(cmd, stdout=subprocess.PIPE) as proc:
         exit_code = proc.wait()
         assert exit_code == 0
         lines = proc.stdout.readlines()
         seq = ''
         for i, line in enumerate(lines):
             line = line.rstrip().decode("utf-8")
-            if i < 1:
-                assert line.startswith(";")
-            elif i == 1:
+            if i == 0:
                 assert line == ">chr1"
             else:
                 assert len(line) <= 80
                 assert re.match(r"^[ACTG]+$", line)
                 seq += line
         assert len(seq) == 1000
 
+
 def test_custom_length():
     for seq_length in [0, 1, 79, 80, 81, 457]:
         with subprocess.Popen(cmd + ['-n', str(seq_length)],
                               stdout=subprocess.PIPE) as proc:
             exit_code = proc.wait()
             assert exit_code == 0
             lines = proc.stdout.readlines()
             seq = ''
             for i, line in enumerate(lines):
                 line = line.rstrip().decode("utf-8")
-                if i < 1:
-                    assert line.startswith(";")
-                elif i == 1:
+                if i == 0:
                     assert line == ">chr1"
                 else:
                     assert len(line) <= 80
                     assert re.match(r"^[ACTG]*$", line)
                     seq += line
             assert len(seq) == seq_length
 
-def test_custome_seqid():
+
+def test_custom_seqid():
     with subprocess.Popen(cmd + ["-s", "foo"], stdout=subprocess.PIPE) as proc:
         exit_code = proc.wait()
         assert exit_code == 0
         lines = proc.stdout.readlines()
         seq = ''
         for i, line in enumerate(lines):
             line = line.rstrip().decode("utf-8")
-            if i < 1:
-                assert line.startswith(";")
-            elif i == 1:
+            if i == 0:
                 assert line == ">foo1"
             else:
                 assert len(line) <= 80
                 assert re.match(r"^[ACTG]+$", line)
                 seq += line
         assert len(seq) == 1000
 
+
 def test_custom_elements():
     with subprocess.Popen(cmd + ["-e", "ZY"], stdout=subprocess.PIPE) as proc:
         exit_code = proc.wait()
         assert exit_code == 0
         lines = proc.stdout.readlines()
         seq = ''
         for i, line in enumerate(lines):
             line = line.rstrip().decode("utf-8")
-            if i < 1:
-                assert line.startswith(";")
-            elif i == 1:
+            if i == 0:
                 assert line == ">chr1"
             else:
                 assert len(line) <= 80
                 assert re.match(r"^[YZ]+$", line)
                 seq += line
         assert len(seq) == 1000
 
-def test_custome_line_size():
+
+def test_custom_line_size():
     for line_size in [50, 100]:
         with subprocess.Popen(cmd + ["--line-size", str(line_size)],
                               stdout=subprocess.PIPE) as proc:
             exit_code = proc.wait()
             assert exit_code == 0
             lines = proc.stdout.readlines()
             seq = ''
             for i, line in enumerate(lines):
                 line = line.rstrip().decode("utf-8")
-                if i < 1:
-                    assert line.startswith(";")
-                elif i == 1:
+                if i == 0:
                     assert line == ">chr1"
                 else:
                     assert len(line) <= line_size
                     assert re.match(r"^[ACTG]+$", line)
                     seq += line
             assert len(seq) == 1000
+
+
+def test_header():
+    with subprocess.Popen(cmd + ["-H"], stdout=subprocess.PIPE) as proc:
+        exit_code = proc.wait()
+        assert exit_code == 0
+        lines = proc.stdout.readlines()
+        seq = ''
+        for i, line in enumerate(lines):
+            line = line.rstrip().decode("utf-8")
+            if i < 1:
+                assert line.startswith(";")
+            elif i == 1:
+                assert line == ">chr1"
+            else:
+                assert len(line) <= 80
+                assert re.match(r"^[ACTG]+$", line)
+                seq += line
+        assert len(seq) == 1000
```

### Comparing `biophony-1.0.0/tests/test_350_genvcf_script.py` & `biophony-1.0.1/tests/test_350_genvcf_script.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_400_genfastavariants.py` & `biophony-1.0.1/tests/test_400_genfastavariants.py`

 * *Files identical despite different names*

### Comparing `biophony-1.0.0/tests/test_450_genfastavariant_script.py` & `biophony-1.0.1/tests/test_450_genfastavariant_script.py`

 * *Files identical despite different names*

