# Comparing `tmp/nucflag-0.0.5.tar.gz` & `tmp/nucflag-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucflag-0.0.5.tar", last modified: Sun May 19 13:35:17 2024, max compression
+gzip compressed data, was "nucflag-0.0.6.tar", last modified: Thu May 30 17:56:48 2024, max compression
```

## Comparing `nucflag-0.0.5.tar` & `nucflag-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 13:35:17.495545 nucflag-0.0.5/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1078 2024-05-04 03:49:09.000000 nucflag-0.0.5/LICENSE
--rw-r--r--   0 koisland  (1000) koisland  (1000)     6421 2024-05-19 13:35:17.495545 nucflag-0.0.5/PKG-INFO
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     5873 2024-05-19 10:08:26.000000 nucflag-0.0.5/README.md
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 13:35:17.491545 nucflag-0.0.5/nucflag/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        0 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/__init__.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     9239 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/classifier.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      586 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/config.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      140 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/constants.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     2743 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/io.py
--rwxrwxr-x   0 koisland  (1000) koisland  (1000)     5912 2024-05-19 13:35:09.000000 nucflag-0.0.5/nucflag/main.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      627 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/misassembly.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     2623 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/plot.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1112 2024-05-19 10:08:26.000000 nucflag-0.0.5/nucflag/region.py
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 13:35:17.495545 nucflag-0.0.5/nucflag.egg-info/
--rw-r--r--   0 koisland  (1000) koisland  (1000)     6421 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/PKG-INFO
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      446 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/SOURCES.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        1 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/dependency_links.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       46 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/entry_points.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/requires.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)        8 2024-05-19 13:35:17.000000 nucflag-0.0.5/nucflag.egg-info/top_level.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)      824 2024-05-19 13:35:09.000000 nucflag-0.0.5/pyproject.toml
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       91 2024-05-04 03:49:09.000000 nucflag-0.0.5/requirements.txt
--rw-rw-r--   0 koisland  (1000) koisland  (1000)       38 2024-05-19 13:35:17.495545 nucflag-0.0.5/setup.cfg
-drwxrwxr-x   0 koisland  (1000) koisland  (1000)        0 2024-05-19 13:35:17.495545 nucflag-0.0.5/test/
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1046 2024-05-19 13:35:10.000000 nucflag-0.0.5/test/test_nucplot.py
--rw-rw-r--   0 koisland  (1000) koisland  (1000)     1433 2024-05-19 10:08:26.000000 nucflag-0.0.5/test/test_region.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-30 17:56:48.506456 nucflag-0.0.6/
+-rw-rw-r--   0 keith     (1000) keith     (1000)     1078 2024-05-28 14:08:45.000000 nucflag-0.0.6/LICENSE
+-rw-r--r--   0 keith     (1000) keith     (1000)     6854 2024-05-30 17:56:48.506456 nucflag-0.0.6/PKG-INFO
+-rw-rw-r--   0 keith     (1000) keith     (1000)     6306 2024-05-30 17:54:48.000000 nucflag-0.0.6/README.md
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-30 17:56:48.506456 nucflag-0.0.6/nucflag/
+-rw-rw-r--   0 keith     (1000) keith     (1000)        0 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/__init__.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)     9802 2024-05-30 17:40:45.000000 nucflag-0.0.6/nucflag/classifier.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)      586 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/config.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)      140 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/constants.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)     2743 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/io.py
+-rwxrwxr-x   0 keith     (1000) keith     (1000)     6251 2024-05-30 17:40:45.000000 nucflag-0.0.6/nucflag/main.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)      627 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/misassembly.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)     2623 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/plot.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)     1112 2024-05-28 14:08:45.000000 nucflag-0.0.6/nucflag/region.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-30 17:56:48.506456 nucflag-0.0.6/nucflag.egg-info/
+-rw-r--r--   0 keith     (1000) keith     (1000)     6854 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/PKG-INFO
+-rw-rw-r--   0 keith     (1000) keith     (1000)      446 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/SOURCES.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)        1 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/dependency_links.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)       46 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/entry_points.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)       91 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/requires.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)        8 2024-05-30 17:56:48.000000 nucflag-0.0.6/nucflag.egg-info/top_level.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)      824 2024-05-30 17:38:53.000000 nucflag-0.0.6/pyproject.toml
+-rw-rw-r--   0 keith     (1000) keith     (1000)       91 2024-05-28 14:08:45.000000 nucflag-0.0.6/requirements.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)       38 2024-05-30 17:56:48.506456 nucflag-0.0.6/setup.cfg
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-30 17:56:48.506456 nucflag-0.0.6/test/
+-rw-rw-r--   0 keith     (1000) keith     (1000)     1046 2024-05-28 14:08:45.000000 nucflag-0.0.6/test/test_nucplot.py
+-rw-rw-r--   0 keith     (1000) keith     (1000)     1433 2024-05-28 14:08:45.000000 nucflag-0.0.6/test/test_region.py
```

### Comparing `nucflag-0.0.5/LICENSE` & `nucflag-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/PKG-INFO` & `nucflag-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,35 @@
-Metadata-Version: 2.1
-Name: nucflag
-Version: 0.0.5
-Summary: NucFlag misassembly identifier.
-Author-email: Keith Oshima <oshimak@pennmedicine.upenn.edu>, "Mitchell R. Vollger" <mrvollger@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/logsdon-lab/NucFlag
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: numpy==1.26.4
-Requires-Dist: polars==0.20.16
-Requires-Dist: portion==2.4.2
-Requires-Dist: pysam==0.22.0
-Requires-Dist: scipy==1.12.0
-
 # `NucFlag`
 [![CI](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml/badge.svg)](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/nucflag)](https://pypi.org/project/nucflag/)
 
 Fork of [`NucFreq`](https://github.com/mrvollger/NucFreq). Script for making nucleotide frequency plots and marking misassemblies.
 
 ![Labeled Misassemblies](docs/imgs/misassemblies.png)
 
 ## Usage
 ```bash
 pip install nucflag
 ```
 
 ```
-usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
-               [--ignore_regions IGNORE_REGIONS]
+usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [--output_cov_dir OUTPUT_COV_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG] [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_BAM, --input_bam INPUT_BAM
                         Input bam file. Must be indexed. (default: None)
   -b INPUT_REGIONS, --input_regions INPUT_REGIONS
                         Bed file with regions to check. (default: None)
   -d OUTPUT_PLOT_DIR, --output_plot_dir OUTPUT_PLOT_DIR
                         Output plot dir. (default: None)
+  --output_cov_dir OUTPUT_COV_DIR
+                        Output coverage dir. Generates coverage bed files per region. Gzipped by default. (default: None)
   -o OUTPUT_MISASM, --output_misasm OUTPUT_MISASM
                         Output bed file with misassembled regions. (default: <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-8'>)
   -s OUTPUT_STATUS, --output_status OUTPUT_STATUS
                         Bed file with status of contigs. With format: contig start end misassembled|good (default: None)
   -r [REGIONS ...], --regions [REGIONS ...]
                         Regions with the format: (.+):(\d+)-(\d+) (default: None)
   -t THREADS, --threads THREADS
@@ -101,14 +85,17 @@
 thr_collapse_het_ratio = 0.1
 
 [gaps]
 # Allow gaps up to this length.
 thr_max_allowed_gap_size = 1000
 ```
 
+## Workflow
+For an end-to-end workflow, see [`Snakemake-NucFlag`](https://github.com/logsdon-lab/Snakemake-NucFlag).
+
 ## Build
 To build from source.
 ```bash
 git clone git@github.com:logsdon-lab/NucFlag.git && cd NucFlag
 make venv && make build && make install
 ```
 
@@ -123,27 +110,30 @@
 ```bash
 source venv/bin/activate
 make test
 ```
 
 Or try the test example directly.
 ```bash
-nucflag -i test/HG00096_hifi_test.bam -b test/test.bed -c test/config.toml
+nucflag -i test/standard/HG00096_hifi.bam -b test/standard/region.bed -c test/config.toml
 ```
 ```
 haplotype2-0000133:3021508-8691473      3314093 3324276 MISJOIN
 haplotype2-0000133:3021508-8691473      4126277 4142368 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      4566798 4683011 GAP
 haplotype2-0000133:3021508-8691473      5737835 5747246 MISJOIN
 haplotype2-0000133:3021508-8691473      6067838 6072601 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      6607947 6639102 MISJOIN
 haplotype2-0000133:3021508-8691473      7997560 8069465 COLLAPSE_VAR
 ```
 
-Test workflow using `data/` dir.
+Test workflow using `data/` dir. Requires:
+1. `bam` files of alignment of HGSVC3 HiFi reads to full assembly.
+2. `bed` files of centromere + 500kbp regions.
+
 ```bash
 snakemake \
 -s test/workflow/Snakefile \
 -j 12 \
 --executor cluster-generic \
 --cluster-generic-submit-cmd "bsub -q epistasis_normal -n {threads} -o /dev/null" \
 --use-conda -p
```

### Comparing `nucflag-0.0.5/README.md` & `nucflag-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+Metadata-Version: 2.1
+Name: nucflag
+Version: 0.0.6
+Summary: NucFlag misassembly identifier.
+Author-email: Keith Oshima <oshimak@pennmedicine.upenn.edu>, "Mitchell R. Vollger" <mrvollger@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/logsdon-lab/NucFlag
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: numpy==1.26.4
+Requires-Dist: polars==0.20.16
+Requires-Dist: portion==2.4.2
+Requires-Dist: pysam==0.22.0
+Requires-Dist: scipy==1.12.0
+
 # `NucFlag`
 [![CI](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml/badge.svg)](https://github.com/logsdon-lab/NucFlag/actions/workflows/main.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/nucflag)](https://pypi.org/project/nucflag/)
 
 Fork of [`NucFreq`](https://github.com/mrvollger/NucFreq). Script for making nucleotide frequency plots and marking misassemblies.
 
 ![Labeled Misassemblies](docs/imgs/misassemblies.png)
 
 ## Usage
 ```bash
 pip install nucflag
 ```
 
 ```
-usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
-               [--ignore_regions IGNORE_REGIONS]
+usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [--output_cov_dir OUTPUT_COV_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG] [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_BAM, --input_bam INPUT_BAM
                         Input bam file. Must be indexed. (default: None)
   -b INPUT_REGIONS, --input_regions INPUT_REGIONS
                         Bed file with regions to check. (default: None)
   -d OUTPUT_PLOT_DIR, --output_plot_dir OUTPUT_PLOT_DIR
                         Output plot dir. (default: None)
+  --output_cov_dir OUTPUT_COV_DIR
+                        Output coverage dir. Generates coverage bed files per region. Gzipped by default. (default: None)
   -o OUTPUT_MISASM, --output_misasm OUTPUT_MISASM
                         Output bed file with misassembled regions. (default: <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-8'>)
   -s OUTPUT_STATUS, --output_status OUTPUT_STATUS
                         Bed file with status of contigs. With format: contig start end misassembled|good (default: None)
   -r [REGIONS ...], --regions [REGIONS ...]
                         Regions with the format: (.+):(\d+)-(\d+) (default: None)
   -t THREADS, --threads THREADS
@@ -84,14 +102,17 @@
 thr_collapse_het_ratio = 0.1
 
 [gaps]
 # Allow gaps up to this length.
 thr_max_allowed_gap_size = 1000
 ```
 
+## Workflow
+For an end-to-end workflow, see [`Snakemake-NucFlag`](https://github.com/logsdon-lab/Snakemake-NucFlag).
+
 ## Build
 To build from source.
 ```bash
 git clone git@github.com:logsdon-lab/NucFlag.git && cd NucFlag
 make venv && make build && make install
 ```
 
@@ -106,27 +127,30 @@
 ```bash
 source venv/bin/activate
 make test
 ```
 
 Or try the test example directly.
 ```bash
-nucflag -i test/HG00096_hifi_test.bam -b test/test.bed -c test/config.toml
+nucflag -i test/standard/HG00096_hifi.bam -b test/standard/region.bed -c test/config.toml
 ```
 ```
 haplotype2-0000133:3021508-8691473      3314093 3324276 MISJOIN
 haplotype2-0000133:3021508-8691473      4126277 4142368 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      4566798 4683011 GAP
 haplotype2-0000133:3021508-8691473      5737835 5747246 MISJOIN
 haplotype2-0000133:3021508-8691473      6067838 6072601 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      6607947 6639102 MISJOIN
 haplotype2-0000133:3021508-8691473      7997560 8069465 COLLAPSE_VAR
 ```
 
-Test workflow using `data/` dir.
+Test workflow using `data/` dir. Requires:
+1. `bam` files of alignment of HGSVC3 HiFi reads to full assembly.
+2. `bed` files of centromere + 500kbp regions.
+
 ```bash
 snakemake \
 -s test/workflow/Snakefile \
 -j 12 \
 --executor cluster-generic \
 --cluster-generic-submit-cmd "bsub -q epistasis_normal -n {threads} -o /dev/null" \
 --use-conda -p
```

### Comparing `nucflag-0.0.5/nucflag/classifier.py` & `nucflag-0.0.6/nucflag/classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import sys
+import gzip
 import pysam
+import shutil
 import scipy.signal
 
 import numpy as np
 import polars as pl
 import portion as pt
 import matplotlib.pyplot as plt
 
@@ -229,14 +231,15 @@
     # TODO: false dupes
     return lf.collect(), filtered_misassemblies
 
 
 def classify_plot_assembly(
     input_bam: str,
     output_dir: str | None,
+    output_cov_dir: str | None,
     threads: int,
     contig: str,
     start: int,
     end: int,
     config: dict[str, Any],
     ignored_regions: list[Region] | None,
 ) -> pl.DataFrame:
@@ -253,20 +256,33 @@
         config=config,
         ignored_regions=ignored_regions,
     )
 
     if output_dir:
         _ = plot_coverage(df_group_labeled, misassemblies, contig)
 
-        sys.stderr.write(f"Plotted {contig_name}.\n")
+        sys.stderr.write(f"Plotting {contig_name}.\n")
 
         output_plot = os.path.join(output_dir, f"{contig_name}.png")
         plt.tight_layout()
         plt.savefig(output_plot, dpi=PLOT_DPI)
 
+    if output_cov_dir:
+        sys.stderr.write(f"Writing coverage bed file for {contig_name}.\n")
+
+        output_bed = os.path.join(output_cov_dir, f"{contig_name}.bed")
+        df_group_labeled.write_csv(output_bed, separator="\t")
+
+        sys.stderr.write(f"Compressing coverage bed file for {contig_name}.\n")
+        with open(output_bed, "rb") as f_in:
+            with gzip.open(f"{output_bed}.gz", "wb") as f_out:
+                shutil.copyfileobj(f_in, f_out)
+
+        os.remove(output_bed)
+
     df_misassemblies = pl.DataFrame(
         [
             (contig_name, interval.lower, interval.upper, misasm)
             for misasm, intervals in misassemblies.items()
             for interval in intervals
         ],
         schema=["contig", "start", "stop", "misassembly"],
```

### Comparing `nucflag-0.0.5/nucflag/config.py` & `nucflag-0.0.6/nucflag/config.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/nucflag/io.py` & `nucflag-0.0.6/nucflag/io.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/nucflag/main.py` & `nucflag-0.0.6/nucflag/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,19 @@
     parser.add_argument(
         "-d",
         "--output_plot_dir",
         default=None,
         help="Output plot dir.",
     )
     parser.add_argument(
+        "--output_cov_dir",
+        default=None,
+        help="Output coverage dir. Generates coverage bed files per region. Gzipped by default.",
+    )
+    parser.add_argument(
         "-o",
         "--output_misasm",
         default=sys.stdout,
         type=argparse.FileType("wt"),
         help="Output bed file with misassembled regions.",
     )
     parser.add_argument(
@@ -96,14 +101,16 @@
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.output_plot_dir:
         os.makedirs(args.output_plot_dir, exist_ok=True)
+    if args.output_cov_dir:
+        os.makedirs(args.output_cov_dir, exist_ok=True)
 
     if isinstance(args.config, io.IOBase):
         # Fill missing config. Keep user config.
         config = DEF_CONFIG | tomllib.load(args.config)
     else:
         config = DEF_CONFIG | args.config
 
@@ -134,14 +141,15 @@
     # Set text size
     matplotlib.rcParams.update({"font.size": PLOT_FONT_SIZE})
 
     # for region in regions:
     #     classify_plot_assembly(
     #         args.input_bam,
     #         args.output_plot_dir,
+    #         args.output_cov_dir,
     #         args.threads,
     #         *region,
     #         config,
     #         (
     #             ignored_regions["all"]
     #             if "all" in ignored_regions
     #             else ignored_regions.get(region[0])
@@ -151,14 +159,15 @@
     with mp.Pool(processes=args.processes) as pool:
         results = pool.starmap(
             classify_plot_assembly,
             [
                 (
                     args.input_bam,
                     args.output_plot_dir,
+                    args.output_cov_dir,
                     args.threads,
                     *region,
                     config,
                     # "all" takes precedence.
                     (
                         ignored_regions["all"]
                         if "all" in ignored_regions
```

### Comparing `nucflag-0.0.5/nucflag/misassembly.py` & `nucflag-0.0.6/nucflag/misassembly.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/nucflag/plot.py` & `nucflag-0.0.6/nucflag/plot.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/nucflag/region.py` & `nucflag-0.0.6/nucflag/region.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/nucflag.egg-info/PKG-INFO` & `nucflag-0.0.6/nucflag.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucflag
-Version: 0.0.5
+Version: 0.0.6
 Summary: NucFlag misassembly identifier.
 Author-email: Keith Oshima <oshimak@pennmedicine.upenn.edu>, "Mitchell R. Vollger" <mrvollger@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/logsdon-lab/NucFlag
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,27 +25,28 @@
 
 ## Usage
 ```bash
 pip install nucflag
 ```
 
 ```
-usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG]
-               [--ignore_regions IGNORE_REGIONS]
+usage: nucflag [-h] -i INPUT_BAM [-b INPUT_REGIONS] [-d OUTPUT_PLOT_DIR] [--output_cov_dir OUTPUT_COV_DIR] [-o OUTPUT_MISASM] [-s OUTPUT_STATUS] [-r [REGIONS ...]] [-t THREADS] [-p PROCESSES] [-c CONFIG] [--ignore_regions IGNORE_REGIONS]
 
 Use per-base read coverage to classify/plot misassemblies.
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_BAM, --input_bam INPUT_BAM
                         Input bam file. Must be indexed. (default: None)
   -b INPUT_REGIONS, --input_regions INPUT_REGIONS
                         Bed file with regions to check. (default: None)
   -d OUTPUT_PLOT_DIR, --output_plot_dir OUTPUT_PLOT_DIR
                         Output plot dir. (default: None)
+  --output_cov_dir OUTPUT_COV_DIR
+                        Output coverage dir. Generates coverage bed files per region. Gzipped by default. (default: None)
   -o OUTPUT_MISASM, --output_misasm OUTPUT_MISASM
                         Output bed file with misassembled regions. (default: <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-8'>)
   -s OUTPUT_STATUS, --output_status OUTPUT_STATUS
                         Bed file with status of contigs. With format: contig start end misassembled|good (default: None)
   -r [REGIONS ...], --regions [REGIONS ...]
                         Regions with the format: (.+):(\d+)-(\d+) (default: None)
   -t THREADS, --threads THREADS
@@ -101,14 +102,17 @@
 thr_collapse_het_ratio = 0.1
 
 [gaps]
 # Allow gaps up to this length.
 thr_max_allowed_gap_size = 1000
 ```
 
+## Workflow
+For an end-to-end workflow, see [`Snakemake-NucFlag`](https://github.com/logsdon-lab/Snakemake-NucFlag).
+
 ## Build
 To build from source.
 ```bash
 git clone git@github.com:logsdon-lab/NucFlag.git && cd NucFlag
 make venv && make build && make install
 ```
 
@@ -123,27 +127,30 @@
 ```bash
 source venv/bin/activate
 make test
 ```
 
 Or try the test example directly.
 ```bash
-nucflag -i test/HG00096_hifi_test.bam -b test/test.bed -c test/config.toml
+nucflag -i test/standard/HG00096_hifi.bam -b test/standard/region.bed -c test/config.toml
 ```
 ```
 haplotype2-0000133:3021508-8691473      3314093 3324276 MISJOIN
 haplotype2-0000133:3021508-8691473      4126277 4142368 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      4566798 4683011 GAP
 haplotype2-0000133:3021508-8691473      5737835 5747246 MISJOIN
 haplotype2-0000133:3021508-8691473      6067838 6072601 COLLAPSE_VAR
 haplotype2-0000133:3021508-8691473      6607947 6639102 MISJOIN
 haplotype2-0000133:3021508-8691473      7997560 8069465 COLLAPSE_VAR
 ```
 
-Test workflow using `data/` dir.
+Test workflow using `data/` dir. Requires:
+1. `bam` files of alignment of HGSVC3 HiFi reads to full assembly.
+2. `bed` files of centromere + 500kbp regions.
+
 ```bash
 snakemake \
 -s test/workflow/Snakefile \
 -j 12 \
 --executor cluster-generic \
 --cluster-generic-submit-cmd "bsub -q epistasis_normal -n {threads} -o /dev/null" \
 --use-conda -p
```

### Comparing `nucflag-0.0.5/pyproject.toml` & `nucflag-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.setuptools.packages.find]
 include = ["nucflag*"]
 exclude = ["docs*", "test*"]
 
 [project]
 name = "nucflag"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Keith Oshima", email = "oshimak@pennmedicine.upenn.edu"},
     {name = "Mitchell R. Vollger", email = "mrvollger@gmail.com"},
 ]
 description = "NucFlag misassembly identifier."
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `nucflag-0.0.5/test/test_nucplot.py` & `nucflag-0.0.6/test/test_nucplot.py`

 * *Files identical despite different names*

### Comparing `nucflag-0.0.5/test/test_region.py` & `nucflag-0.0.6/test/test_region.py`

 * *Files identical despite different names*

