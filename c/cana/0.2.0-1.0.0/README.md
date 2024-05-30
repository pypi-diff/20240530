# Comparing `tmp/cana-0.2.0.tar.gz` & `tmp/cana-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alien/usr/docs/school/RESEARCH/casci/CANA_rionbr/dist/.tmp-e9tqm8f9/cana-0.2.0.tar", last modified: Fri Mar 17 16:00:53 2023, max compression
+gzip compressed data, was "cana-1.0.0.tar", last modified: Thu May 30 16:56:27 2024, max compression
```

## Comparing `cana-0.2.0.tar` & `cana-1.0.0.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.450196 cana-0.2.0/
--rw-rw-r--   0 alien     (1001) alien     (1001)     1077 2022-06-30 18:23:29.000000 cana-0.2.0/LICENSE
--rw-rw-r--   0 alien     (1001) alien     (1001)      157 2022-06-30 18:23:29.000000 cana-0.2.0/MANIFEST.in
--rw-rw-r--   0 alien     (1001) alien     (1001)      827 2023-03-17 16:00:53.450196 cana-0.2.0/PKG-INFO
--rw-rw-r--   0 alien     (1001) alien     (1001)     4497 2023-03-17 13:33:05.000000 cana-0.2.0/README.md
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.418195 cana-0.2.0/cana/
--rw-rw-r--   0 alien     (1001) alien     (1001)      680 2023-03-17 12:41:52.000000 cana-0.2.0/cana/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)      652 2022-11-18 19:54:17.000000 cana-0.2.0/cana/base.py
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.418195 cana-0.2.0/cana/bns/
--rw-rw-r--   0 alien     (1001) alien     (1001)     3369 2022-11-18 19:54:17.000000 cana-0.2.0/cana/bns/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)    67066 2023-01-23 16:57:03.000000 cana-0.2.0/cana/boolean_network.py
--rw-rw-r--   0 alien     (1001) alien     (1001)    33328 2023-03-17 13:39:04.000000 cana-0.2.0/cana/boolean_node.py
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.418195 cana-0.2.0/cana/canalization/
--rw-rw-r--   0 alien     (1001) alien     (1001)        0 2022-11-18 19:54:17.000000 cana-0.2.0/cana/canalization/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)    24136 2023-03-15 20:37:05.000000 cana-0.2.0/cana/canalization/boolean_canalization.py
--rw-rw-r--   0 alien     (1001) alien     (1001)   418696 2023-03-17 13:39:04.000000 cana-0.2.0/cana/canalization/cboolean_canalization.c
--rw-rw-r--   0 alien     (1001) alien     (1001)     7126 2022-11-18 19:54:17.000000 cana-0.2.0/cana/canalization/cboolean_canalization.pyx
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.418195 cana-0.2.0/cana/control/
--rw-rw-r--   0 alien     (1001) alien     (1001)        0 2022-11-18 19:54:17.000000 cana-0.2.0/cana/control/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     7576 2022-11-18 19:54:17.000000 cana-0.2.0/cana/control/fvs.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     1888 2022-11-18 19:54:17.000000 cana-0.2.0/cana/control/mds.py
--rw-rw-r--   0 alien     (1001) alien     (1001)    11117 2022-11-18 19:54:17.000000 cana-0.2.0/cana/control/sc.py
--rw-rw-r--   0 alien     (1001) alien     (1001)   448067 2023-03-17 13:39:04.000000 cana-0.2.0/cana/cutils.c
--rw-rw-r--   0 alien     (1001) alien     (1001)     8068 2022-11-18 19:54:17.000000 cana-0.2.0/cana/cutils.pyx
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.422195 cana-0.2.0/cana/datasets/
--rw-rw-r--   0 alien     (1001) alien     (1001)        0 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     7652 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bio.py
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.422195 cana-0.2.0/cana/datasets/bns/
--rw-rw-r--   0 alien     (1001) alien     (1001)     1934 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/arabidopsis.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     2199 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/budding_yeast.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     8646 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/drosophila4.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     1639 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/fission_yeast.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     1430 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/mammalian.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     3546 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/tcr.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     1918 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bns/thelper.cnet
--rw-rw-r--   0 alien     (1001) alien     (1001)     1942 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/bools.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     3565 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/breast_cancer.txt
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.446196 cana-0.2.0/cana/datasets/cell_collective/
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3003 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Apoptosis Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     8413 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Arabidopsis thaliana Cell Cycle.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3245 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Aurora Kinase A in Neuroblastoma.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     9937 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/B bronchiseptica and T retortaeformis coinfection.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3467 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/B cell differentiation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4377 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/BT474 Breast Cell Line Long-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2945 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/BT474 Breast Cell Line Short-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3715 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Bordetella bronchiseptica.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     5837 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Bortezomib Responses in U266 Human Myeloma Cells.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3695 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle 2009.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2335 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    43624 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/CD4 T cell signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    30798 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/CD4+ T Cell Differentiation and Plasticity.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    10867 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/CD4+ T cell Differentiation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3345 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Cardiac development.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      728 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Cell Cycle Transcription by Coupled CDK and Network Oscillators.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2622 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Cholesterol Regulatory Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     5933 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Colitis-associated colon cancer.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      508 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Cortical Area Development.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1832 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Death Receptor Signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    12148 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Differentiation of T lymphocytes.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)   471559 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/EGFR & ErbB Signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    15440 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/FA BRCA pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1217 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/FGF pathway of Drosophila Signalling Pathways.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     8162 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Fanconi anemia and checkpoint recovery.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4680 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Glucose Repression Signaling 2009.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3582 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Guard Cell Abscisic Acid Signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4342 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Long-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3156 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Short-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4270 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/HGF Signaling in Keratinocytes.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     5433 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/HH Pathway of Drosophila Signaling Pathways.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)   654746 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/HIV-1 interactions with T Cell Signalling Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    21566 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Human Gonadal Sex Determination.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    74265 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/IGVH mutations in chronic lymphocytic leukemia.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    10392 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/IL-1 Signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     7879 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/IL-6 Signalling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    54733 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Influenza A Virus Replication Cycle.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2146 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Iron acquisition and oxidative stress response in aspergillus fumigatus.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      841 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Lac Operon.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    27606 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Lymphoid and myeloid cell specification and transdifferentiation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    19131 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Lymphopoiesis Regulatory Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4515 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/MAPK Cancer Cell Fate Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2248 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Mammalian Cell Cycle 2006.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2396 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Mammalian Cell Cycle.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1619 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Metabolic Interactions in the Gut Microbiome.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1188 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Neurotransmitter Signaling Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1243 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Oxidative Stress Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     4085 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/PC12 Cell Differentiation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3346 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Predicting Variabilities in Cardiac Gene.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    11572 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1599 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Processing of Spz Network from the Drosophila Signaling Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      681 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Regulation of the L-arabinose operon of Escherichia coli.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     6389 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Long-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2065 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Short-term ErbB Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3984 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Senescence Associated Secretory Phenotype.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2195 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Septation Initiation Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)   307317 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Signal Transduction in Fibroblasts.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     8726 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    59704 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Signaling in Macrophage Activation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    28981 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Stomatal Opening Model.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     7733 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T Cell Receptor Signaling.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1572 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T cell differentiation.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2422 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T-Cell Signaling 2006.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    13138 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2008.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     1492 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2011 Reduced Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    13489 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2011.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    25862 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/TOL Regulatory Network.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      539 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Toll Pathway of Drosophila Signaling Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2734 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Treatment of Castration-Resistant Prostate Cancer.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2452 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Trichostrongylus retortaeformis.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)    33796 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Tumour Cell Invasion and Migration.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      965 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/VEGF Pathway of Drosophila Signaling Pathway.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     3227 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Wg Pathway of Drosophila Signalling Pathways.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)   102559 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/cell_collective/Yeast Apoptosis.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     6079 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/drosophila_parasegment.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)      879 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/drosophila_single_cell.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)     1907 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/leukemia.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)      902 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/marques-pita_rocha.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)     7786 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/motifs.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     1699 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/thaliana.txt
--rwxrwxr-x   0 alien     (1001) alien     (1001)     2303 2022-11-18 19:54:17.000000 cana-0.2.0/cana/datasets/yeast_cell_cycle.txt
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.450196 cana-0.2.0/cana/drawing/
--rw-rw-r--   0 alien     (1001) alien     (1001)        0 2022-11-18 19:54:17.000000 cana-0.2.0/cana/drawing/__init__.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     5128 2022-11-18 19:54:17.000000 cana-0.2.0/cana/drawing/canalizing_map.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     8614 2023-01-17 18:49:38.000000 cana-0.2.0/cana/drawing/schema_vis.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     6582 2022-11-18 19:54:17.000000 cana-0.2.0/cana/random_boolean_network.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     9138 2023-03-15 15:40:19.000000 cana-0.2.0/cana/utils.py
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.418195 cana-0.2.0/cana.egg-info/
--rw-rw-r--   0 alien     (1001) alien     (1001)      827 2023-03-17 16:00:53.000000 cana-0.2.0/cana.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1001) alien     (1001)     6647 2023-03-17 16:00:53.000000 cana-0.2.0/cana.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)        1 2023-03-17 16:00:53.000000 cana-0.2.0/cana.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)        1 2022-11-18 19:54:11.000000 cana-0.2.0/cana.egg-info/not-zip-safe
--rw-rw-r--   0 alien     (1001) alien     (1001)       35 2023-03-17 16:00:53.000000 cana-0.2.0/cana.egg-info/requires.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)        5 2023-03-17 16:00:53.000000 cana-0.2.0/cana.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1001) alien     (1001)      100 2023-03-17 12:58:57.000000 cana-0.2.0/pyproject.toml
--rw-rw-r--   0 alien     (1001) alien     (1001)       38 2023-03-17 16:00:53.450196 cana-0.2.0/setup.cfg
--rw-rw-r--   0 alien     (1001) alien     (1001)     1647 2023-03-17 12:41:20.000000 cana-0.2.0/setup.py
-drwxrwxr-x   0 alien     (1001) alien     (1001)        0 2023-03-17 16:00:53.450196 cana-0.2.0/tests/
--rw-rw-r--   0 alien     (1001) alien     (1001)    14789 2023-03-15 14:40:34.000000 cana-0.2.0/tests/test_boolean_canalization.py
--rw-rw-r--   0 alien     (1001) alien     (1001)      588 2023-01-23 16:46:12.000000 cana-0.2.0/tests/test_boolean_network.py
--rw-rw-r--   0 alien     (1001) alien     (1001)    32626 2023-01-23 15:26:02.000000 cana-0.2.0/tests/test_boolean_node.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     1436 2023-01-23 16:51:40.000000 cana-0.2.0/tests/test_effectiveness_measures.py
--rw-rw-r--   0 alien     (1001) alien     (1001)     5931 2023-01-20 18:25:23.000000 cana-0.2.0/tests/test_two_symbol_symmetry.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.706214 cana-1.0.0/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1077 2024-05-30 14:59:10.000000 cana-1.0.0/LICENSE
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      157 2024-05-30 14:59:10.000000 cana-1.0.0/MANIFEST.in
+-rw-r--r--   0 fxcosta   (1000) fxcosta   (1000)      975 2024-05-30 16:56:27.706214 cana-1.0.0/PKG-INFO
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     4512 2024-05-30 14:59:10.000000 cana-1.0.0/README.md
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      712 2024-05-30 14:59:10.000000 cana-1.0.0/cana/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      685 2024-05-30 14:59:10.000000 cana-1.0.0/cana/base.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/bns/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     3416 2024-05-30 14:59:10.000000 cana-1.0.0/cana/bns/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    73525 2024-05-30 14:59:10.000000 cana-1.0.0/cana/boolean_network.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    34915 2024-05-30 14:59:10.000000 cana-1.0.0/cana/boolean_node.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/canalization/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 14:59:10.000000 cana-1.0.0/cana/canalization/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    18178 2024-05-30 14:59:10.000000 cana-1.0.0/cana/canalization/boolean_canalization.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)   423811 2024-05-30 14:59:10.000000 cana-1.0.0/cana/canalization/cboolean_canalization.c
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     7126 2024-05-30 14:59:10.000000 cana-1.0.0/cana/canalization/cboolean_canalization.pyx
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/control/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 14:59:10.000000 cana-1.0.0/cana/control/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     7693 2024-05-30 14:59:10.000000 cana-1.0.0/cana/control/fvs.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1970 2024-05-30 14:59:10.000000 cana-1.0.0/cana/control/mds.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    11314 2024-05-30 14:59:10.000000 cana-1.0.0/cana/control/sc.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)   453361 2024-05-30 14:59:10.000000 cana-1.0.0/cana/cutils.c
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     8068 2024-05-30 14:59:10.000000 cana-1.0.0/cana/cutils.pyx
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/datasets/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     8000 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bio.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.698214 cana-1.0.0/cana/datasets/bns/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1934 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/arabidopsis.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     2199 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/budding_yeast.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     8646 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/drosophila4.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1639 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/fission_yeast.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1430 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/mammalian.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     3546 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/tcr.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1918 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bns/thelper.cnet
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1969 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/bools.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     3565 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/breast_cancer.txt
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.702214 cana-1.0.0/cana/datasets/cell_collective/
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3003 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Apoptosis Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     8413 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Arabidopsis thaliana Cell Cycle.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3245 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Aurora Kinase A in Neuroblastoma.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     9937 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/B bronchiseptica and T retortaeformis coinfection.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3467 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/B cell differentiation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4377 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/BT474 Breast Cell Line Long-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2945 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/BT474 Breast Cell Line Short-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3715 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Bordetella bronchiseptica.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     5837 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Bortezomib Responses in U266 Human Myeloma Cells.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3695 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle 2009.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2335 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    43624 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/CD4 T cell signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    30798 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/CD4+ T Cell Differentiation and Plasticity.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    10867 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/CD4+ T cell Differentiation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3345 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Cardiac development.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      728 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Cell Cycle Transcription by Coupled CDK and Network Oscillators.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2622 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Cholesterol Regulatory Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     5933 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Colitis-associated colon cancer.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      508 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Cortical Area Development.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1832 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Death Receptor Signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    12148 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Differentiation of T lymphocytes.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)   471559 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/EGFR & ErbB Signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    15440 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/FA BRCA pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1217 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/FGF pathway of Drosophila Signalling Pathways.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     8162 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Fanconi anemia and checkpoint recovery.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4680 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Glucose Repression Signaling 2009.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3582 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Guard Cell Abscisic Acid Signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4342 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Long-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3156 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Short-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4270 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/HGF Signaling in Keratinocytes.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     5433 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/HH Pathway of Drosophila Signaling Pathways.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)   654746 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/HIV-1 interactions with T Cell Signalling Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    21566 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Human Gonadal Sex Determination.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    74265 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/IGVH mutations in chronic lymphocytic leukemia.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    10392 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/IL-1 Signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     7879 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/IL-6 Signalling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    54733 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Influenza A Virus Replication Cycle.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2146 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Iron acquisition and oxidative stress response in aspergillus fumigatus.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      841 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Lac Operon.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    27606 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Lymphoid and myeloid cell specification and transdifferentiation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    19131 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Lymphopoiesis Regulatory Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4515 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/MAPK Cancer Cell Fate Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2248 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Mammalian Cell Cycle 2006.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2396 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Mammalian Cell Cycle.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1619 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Metabolic Interactions in the Gut Microbiome.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1188 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Neurotransmitter Signaling Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1243 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Oxidative Stress Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     4085 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/PC12 Cell Differentiation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3346 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Predicting Variabilities in Cardiac Gene.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    11572 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1599 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Processing of Spz Network from the Drosophila Signaling Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      681 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Regulation of the L-arabinose operon of Escherichia coli.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     6389 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Long-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2065 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Short-term ErbB Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3984 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Senescence Associated Secretory Phenotype.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2195 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Septation Initiation Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)   307317 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Signal Transduction in Fibroblasts.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     8726 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    59704 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Signaling in Macrophage Activation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    28981 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Stomatal Opening Model.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     7733 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T Cell Receptor Signaling.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1572 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T cell differentiation.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2422 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T-Cell Signaling 2006.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    13138 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2008.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     1492 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2011 Reduced Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    13489 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2011.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    25862 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/TOL Regulatory Network.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      539 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Toll Pathway of Drosophila Signaling Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2734 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Treatment of Castration-Resistant Prostate Cancer.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2452 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Trichostrongylus retortaeformis.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)    33796 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Tumour Cell Invasion and Migration.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      965 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/VEGF Pathway of Drosophila Signaling Pathway.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     3227 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Wg Pathway of Drosophila Signalling Pathways.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)   102559 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/cell_collective/Yeast Apoptosis.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     6079 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/drosophila_parasegment.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)      879 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/drosophila_single_cell.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1907 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/leukemia.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      902 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/marques-pita_rocha.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     7786 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/motifs.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1699 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/thaliana.txt
+-rwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)     2303 2024-05-30 14:59:10.000000 cana-1.0.0/cana/datasets/yeast_cell_cycle.txt
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.702214 cana-1.0.0/cana/drawing/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 14:59:10.000000 cana-1.0.0/cana/drawing/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     5340 2024-05-30 14:59:10.000000 cana-1.0.0/cana/drawing/canalizing_map.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    10880 2024-05-30 14:59:10.000000 cana-1.0.0/cana/drawing/schema_vis.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     6934 2024-05-30 14:59:10.000000 cana-1.0.0/cana/random_boolean_network.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     9539 2024-05-30 14:59:10.000000 cana-1.0.0/cana/utils.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.702214 cana-1.0.0/cana.egg-info/
+-rw-r--r--   0 fxcosta   (1000) fxcosta   (1000)      975 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/PKG-INFO
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     6665 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/SOURCES.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        1 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/dependency_links.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        1 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/not-zip-safe
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)       58 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/requires.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)       11 2024-05-30 16:56:27.000000 cana-1.0.0/cana.egg-info/top_level.txt
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      191 2024-05-30 14:59:10.000000 cana-1.0.0/pyproject.toml
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)       38 2024-05-30 16:56:27.706214 cana-1.0.0/setup.cfg
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1957 2024-05-30 15:49:17.000000 cana-1.0.0/setup.py
+drwxrwxr-x   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 16:56:27.702214 cana-1.0.0/tests/
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)        0 2024-05-30 14:59:10.000000 cana-1.0.0/tests/__init__.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    14789 2024-05-30 14:59:10.000000 cana-1.0.0/tests/test_boolean_canalization.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)      588 2024-05-30 14:59:10.000000 cana-1.0.0/tests/test_boolean_network.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)    25409 2024-05-30 14:59:10.000000 cana-1.0.0/tests/test_boolean_node.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     1436 2024-05-30 14:59:10.000000 cana-1.0.0/tests/test_effectiveness_measures.py
+-rw-rw-r--   0 fxcosta   (1000) fxcosta   (1000)     5749 2024-05-30 14:59:10.000000 cana-1.0.0/tests/test_two_symbol_symmetry.py
```

### Comparing `cana-0.2.0/LICENSE` & `cana-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/PKG-INFO` & `cana-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: cana
-Version: 0.2.0
+Version: 1.0.0
 Summary: This package implements a series of methods used to study control, canalization and redundancy in Boolean networks.
 Home-page: http://github.com/rionbr/CANA
 Author: Alex Gates & Rion Brattig Correia
 Author-email: rionbr@gmail.com
 License: MIT
 Keywords: boolean networks canalization redundancy dynamical systems computational biology
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/plain
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: schematodes>=1.0.0
 
 This package implements a series of methods used to study control, canalization and redundancy in Boolean networks.
```

### Comparing `cana-0.2.0/README.md` & `cana-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 - from PYPI
 ```
     pip install cana
 ```
 
 ** Latest development release on GitHub **
 
-Pull and install the code directly from the github [project page](https://github.com/rionbr/CANA).
+Pull and install the code directly from the github [project page](https://github.com/casci-lab/CANA).
 
 ```
-    pip install git+https://github.com/rionbr/CANA
+    pip install git+https://github.com/CASCI-lab/CANA
 ```
 
 Please note that CANA uses Cython. For it to compile you may need to install the following:
 
 - `pip install Cython`
 
 Docs:
 -------
 
-The full documentation can be found at: [rionbr.github.io/CANA](https://rionbr.github.io/CANA)
+The full documentation can be found at: [casci-lab.github.io/CANA/](https://casci-lab.github.io/CANA/)
 
 
 Papers:
 ---------
 
 - A.J. Gates, R.B. Correia, X. Wang, L.M. Rocha [2021]. "[The effective graph reveals redundancy, canalization, and control pathways in biochemical regulation and signaling](https://doi.org/10.1073/pnas.2022598118)". *Proceedings of the National Academy of Sciences (PNAS)*. 118(**12**). doi: 10.1073/pnas.20225981186
 
@@ -117,8 +117,8 @@
 - Networkx 2.1 compatibility
 - Inclusion of tutorials
 - Derrida curve
 
 v.0.0.1
 - Control (FVS, MDS, CSTG) methods.
 - Canalization methods.
-- Implementation ported to public package.
+- Implementation ported to public package.
```

### Comparing `cana-0.2.0/cana/base.py` & `cana-1.0.0/cana/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-import warnings
 import functools
+import warnings
 
 
 def deprecated(func):
     """This is a decorator which can be used to mark functions as deprecated.
     It will result in a warning being emitted when the function is used.
     """
+
     @functools.wraps(func)
     def new_func(*args, **kwargs):
         warnings.warn_explicit(
-            "You've called a deprecated function. Maybe this function needs updating to the new package. {}".format(func.__name__),
+            "You've called a deprecated function. Maybe this function needs updating to the new package. {}".format(
+                func.__name__
+            ),
             category=DeprecationWarning,
             filename=func.func_code.co_filename,
-            lineno=func.func_code.co_firstlineno + 1
+            lineno=func.func_code.co_firstlineno + 1,
         )
         return func(*args, **kwargs)
+
     return new_func
```

### Comparing `cana-0.2.0/cana/bns/__init__.py` & `cana-1.0.0/cana/bns/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Alex Gates <ajgates@indiana.edu>
 #   All rights reserved.
 #   MIT license.
 import os
 import subprocess
 import tempfile
+
 from cana.utils import binstate_to_statenum
 
 _path = os.path.dirname(os.path.realpath(__file__))
 """ Make sure we know what the current directory is """
 
 
 def attractors(cnet, bnspath=_path, cleanup=True):
@@ -49,45 +50,49 @@
     # If is file, open the file
     if os.path.isfile(cnet):
         file = cnet
 
     # If string, Creates a Temporary File to be supplied to BNS
     elif isinstance(cnet, str):
         tmp = tempfile.NamedTemporaryFile(delete=cleanup)
-        with open(tmp.name, 'w') as openfile:
+        with open(tmp.name, "w") as openfile:
             openfile.write(cnet)
         tmp.file.close()
         file = tmp.name
     else:
-        raise TypeError('The cnet input should be either a file to a .cnet file or a string containing the .cnet content')
+        raise TypeError(
+            "The cnet input should be either a file to a .cnet file or a string containing the .cnet content"
+        )
 
-    cmd = [os.path.join(_path, 'bns'), file]
+    cmd = [os.path.join(bnspath, "bns"), file]
     attractors = list()
 
     try:
         p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
         current_attractor = []
-        for i, line in enumerate(p.stdout):
+        for _, line in enumerate(p.stdout):
             # Strip line
-            cleanline = line.decode('ascii').strip().replace('\n', '')
+            cleanline = line.decode("ascii").strip().replace("\n", "")
 
-            if 'Attractor' in cleanline:
+            if "Attractor" in cleanline:
                 attractors.append(current_attractor)
                 current_attractor = []
-            elif 'Node' in cleanline and 'assumed to be constant' in cleanline:
+            elif "Node" in cleanline and "assumed to be constant" in cleanline:
                 pass
-            elif 'Total' in cleanline:
+            elif "Total" in cleanline:
                 pass
-            elif 'Start searching for all atractors.' in cleanline:
+            elif "Start searching for all atractors." in cleanline:
                 pass
-            elif 'Depth' in cleanline:
+            elif "Depth" in cleanline:
                 pass
-            elif 'average' in cleanline:
+            elif "average" in cleanline:
                 pass
             elif len(cleanline) > 0:
                 current_attractor.append(binstate_to_statenum(cleanline))
 
     except OSError:
-        print("'BNS' could not be found! You must have it compiled or download the binary for your system from the 'bns' website (https://people.kth.se/~dubrova/bns.html).")
+        print(
+            "'BNS' could not be found! You must have it compiled or download the binary for your system from the 'bns' website (https://people.kth.se/~dubrova/bns.html)."
+        )
 
     return attractors
```

### Comparing `cana-0.2.0/cana/boolean_network.py` & `cana-1.0.0/cana/boolean_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,105 +9,171 @@
 #   Copyright (C) 2021 by
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Alex Gates <ajgates@indiana.edu>
 #   Thomas Parmer <tjparmer@indiana.edu>
 #   All rights reserved.
 #   MIT license.
 from collections import defaultdict
+
 try:
-    import cStringIO.StringIO as StringIO
+    import cStringIO.StringIO as StringIO  # type: ignore
 except ImportError:
     from io import StringIO
-import numpy as np
-import networkx as nx
-import random
+
+import copy
 import itertools
-from cana.boolean_node import BooleanNode
+import pickle
+import random
+import re
+import warnings
+
+import networkx as nx
+import numpy as np
+
 import cana.bns as bns
+from cana.boolean_node import BooleanNode
 from cana.control import fvs, mds, sc
-from cana.utils import *
-import warnings
-import re
-import copy
+from cana.cutils import (
+    binstate_compare,
+    binstate_pinned_to_binstate,
+    binstate_to_constantbinstate,
+    binstate_to_statenum,
+    constantbinstate_to_statenum,
+    expand_logic_line,
+    flip_binstate_bit,
+    flip_bit,
+    hamming_distance,
+    random_binstate,
+    recursive_map,
+    statenum_to_binstate,
+)
 
+# from cana.utils import *
+from cana.utils import entropy, flip_binstate_bit_set, output_transitions
 
-class BooleanNetwork:
-    """
 
-    """
+class BooleanNetwork:
+    """ """
 
-    def __init__(self, name='', Nnodes=0, logic=None, sg=None, stg=None, stg_r=None, _eg=None, attractors=None,
-                 constants={}, Nconstants=0, keep_constants=False,
-                 bin2num=binstate_to_statenum, num2bin=statenum_to_binstate,
-                 verbose=False, *args, **kwargs):
-
-        self.name = name                            # Name of the Network
-        self.Nnodes = Nnodes                        # Number of Nodes
-        self.logic = logic                          # A dict that contains the network logic {<id>:{'name':<string>,'in':<list-input-node-id>,'out':<list-output-transitions>},..}
-        self._sg = sg                               # Structure-Graph (SG)
-        self._stg = stg                             # State-Transition-Graph (STG)
-        self._stg_r = stg_r                         # State-Transition-Graph Reachability dict (STG-R)
-        self._eg = None                             # Effective Graph, computed from the effective connectivity
-        self._attractors = attractors               # Network Attractors
+    def __init__(
+        self,
+        name="",
+        Nnodes=0,
+        logic=None,
+        sg=None,
+        stg=None,
+        stg_r=None,
+        _eg=None,
+        attractors=None,
+        constants=None,
+        Nconstants=None,
+        keep_constants=False,
+        bin2num=None,
+        num2bin=None,
+        verbose=False,
+        *args,
+        **kwargs
+    ):
+        # NOTE: *args and **kwargs don't do anything. I'm not sure why they wre added here, so I'm not going to remove them.
+
+        self.name = name  # Name of the Network
+        self.Nnodes = Nnodes  # Number of Nodes
+        self.logic = logic  # A dict that contains the network logic {<id>:{'name':<string>,'in':<list-input-node-id>,'out':<list-output-transitions>},..}
+        self._sg = sg  # Structure-Graph (SG)
+        self._stg = stg  # State-Transition-Graph (STG)
+        self._stg_r = stg_r  # State-Transition-Graph Reachability dict (STG-R)
+        self._eg = _eg  # Effective Graph, computed from the effective connectivity
+        self._attractors = attractors  # Network Attractors
         #
-        self.keep_constants = keep_constants        # Keep/Include constants in some of the computations
-        #self.constants = constants                  # A dict that contains of constant variables in the network
-        #
-        self.Nstates = 2**Nnodes                    # Number of possible states in the network 2^N
+        self.keep_constants = (
+            keep_constants  # Keep/Include constants in some of the computations
+        )
+        if constants is None:
+            self.constants = {}
+        else:
+            self.constants = (
+                constants  # Keep/Include constants in some of the computations
+            )
+
+        self.Nstates = 2**Nnodes  # Number of possible states in the network 2^N
         #
         self.verbose = verbose
 
         # Intanciate BooleanNodes
-        self.name2int = {logic[i]['name']: i for i in range(Nnodes)}
-        self.Nself_loops = sum([self.name2int[logic[i]['name']] in logic[i]['in'] for i in range(Nnodes)])
+        self.name2int = {logic[i]["name"]: i for i in range(Nnodes)}
+        self.Nself_loops = sum(
+            [self.name2int[logic[i]["name"]] in logic[i]["in"] for i in range(Nnodes)]
+        )
 
         self.nodes = list()
         for i in range(Nnodes):
-            name = logic[i]['name']
-            k = len(logic[i]['in'])
-            inputs = [self.name2int[logic[j]['name']] for j in logic[i]['in']]
-            outputs = logic[i]['out']
-            node = BooleanNode(id=i, name=name, k=k, inputs=inputs, outputs=outputs, network=self)
+            name = logic[i]["name"]
+            k = len(logic[i]["in"])
+            inputs = [self.name2int[logic[j]["name"]] for j in logic[i]["in"]]
+            outputs = logic[i]["out"]
+            node = BooleanNode(
+                id=i, name=name, k=k, inputs=inputs, outputs=outputs, network=self
+            )
             self.nodes.append(node)
 
-        self.Nconstants = sum([n.constant for n in self.nodes])  # Number of constant variables
-        #
-        self.input_nodes = [i for i in range(Nnodes) if (self.nodes[i].constant or ((self.nodes[i].k == 1) and (i in self.nodes[i].inputs)))]
+        if Nconstants is None:
+            self.Nconstants = sum(
+                [n.constant for n in self.nodes]
+            )  # Number of constant variables
+        else:
+            self.Nconstants = Nconstants
+
+        self.input_nodes = [
+            i
+            for i in range(Nnodes)
+            if (
+                self.nodes[i].constant
+                or ((self.nodes[i].k == 1) and (i in self.nodes[i].inputs))
+            )
+        ]
         #
-        self.bin2num = None                      # Helper function. Converts binstate to statenum. It gets updated by `_update_trans_func`
-        self.num2bin = None                      # Helper function. Converts statenum to binstate. It gets updated by `_update_trans_func`
-        self._update_trans_func()                   # Updates helper functions and other variables
+        self.bin2num = bin2num  # Helper function. Converts binstate to statenum. It gets updated by `_update_trans_func`
+        self.num2bin = num2bin  # Helper function. Converts statenum to binstate. It gets updated by `_update_trans_func`
+        self._update_trans_func()  # Updates helper functions and other variables
 
     def __str__(self):
         node_names = [node.name for node in self.nodes]
-        return "<BNetwork(name='{name:s}', N={number_of_nodes:d}, Nodes={nodes:})>".format(name=self.name, number_of_nodes=self.Nnodes, nodes=node_names)
+        return (
+            "<BNetwork(name='{name:s}', N={number_of_nodes:d}, Nodes={nodes:})>".format(
+                name=self.name, number_of_nodes=self.Nnodes, nodes=node_names
+            )
+        )
 
     #
     # I/O Methods
     #
     @classmethod
-    def from_file(self, file, type='cnet', keep_constants=True, **kwargs):
+    def from_file(self, file, type="cnet", keep_constants=True, **kwargs):
         """
         Load the Boolean Network from a file.
 
         Args:
             file (string) : The name of a file containing the Boolean Network.
             type (string) : The type of file, either 'cnet' (default) or 'logical' for Boolean logical rules.
 
         Returns:
             BooleanNetwork (object) : The boolean network object.
 
         See also:
             :func:`from_string` :func:`from_dict`
         """
-        with open(file, 'r') as infile:
-            if type == 'cnet':
-                return self.from_string_cnet(infile.read(), keep_constants=keep_constants, **kwargs)
-            elif type == 'logical':
-                return self.from_string_boolean(infile.read(), keep_constants=keep_constants, **kwargs)
+        with open(file, "r") as infile:
+            if type == "cnet":
+                return self.from_string_cnet(
+                    infile.read(), keep_constants=keep_constants, **kwargs
+                )
+            elif type == "logical":
+                return self.from_string_boolean(
+                    infile.read(), keep_constants=keep_constants, **kwargs
+                )
 
     @classmethod
     def from_string_cnet(self, string, keep_constants=True, **kwargs):
         """
         Instanciates a Boolean Network from a string in cnet format.
 
         Args:
@@ -134,48 +200,56 @@
             :func:`from_file` :func:`from_dict`
         """
         network_file = StringIO(string)
         logic = defaultdict(dict)
 
         line = network_file.readline()
         while line != "":
-            if line[0] != '#' and line != '\n':
+            if line[0] != "#" and line != "\n":
                 # .v <#-nodes>
-                if '.v' in line:
+                if ".v" in line:
                     Nnodes = int(line.split()[1])
                     for inode in range(Nnodes):
-                        logic[inode] = {'name': '', 'in': [], 'out': []}
+                        logic[inode] = {"name": "", "in": [], "out": []}
                 # .l <node-id> <node-name>
-                elif '.l' in line:
-                    logic[int(line.split()[1]) - 1]['name'] = line.split()[2]
+                elif ".l" in line:
+                    logic[int(line.split()[1]) - 1]["name"] = line.split()[2]
                 # .n <node-id> <#-inputs> <input-node-id>
-                elif '.n' in line:
+                elif ".n" in line:
                     inode = int(line.split()[1]) - 1
                     indegree = int(line.split()[2])
                     for jnode in range(indegree):
-                        logic[inode]['in'].append(int(line.split()[3 + jnode]) - 1)
+                        logic[inode]["in"].append(int(line.split()[3 + jnode]) - 1)
 
-                    logic[inode]['out'] = [0 for i in range(2**indegree) if indegree > 0]
+                    logic[inode]["out"] = [
+                        0 for i in range(2**indegree) if indegree > 0
+                    ]
 
                     logic_line = network_file.readline().strip()
 
                     if indegree <= 0:
-                        if logic_line == '':
-                            logic[inode]['in'] = [inode]
-                            logic[inode]['out'] = [0, 1]
+                        if logic_line == "":
+                            logic[inode]["in"] = [inode]
+                            logic[inode]["out"] = [0, 1]
                         else:
-                            logic[inode]['out'] = [int(logic_line)]
+                            logic[inode]["out"] = [int(logic_line)]
                     else:
-                        while logic_line != '\n' and logic_line != '' and len(logic_line) > 1:
+                        while (
+                            logic_line != "\n"
+                            and logic_line != ""
+                            and len(logic_line) > 1
+                        ):
                             for nlogicline in expand_logic_line(logic_line):
-                                logic[inode]['out'][binstate_to_statenum(nlogicline.split()[0])] = int(nlogicline.split()[1])
+                                logic[inode]["out"][
+                                    binstate_to_statenum(nlogicline.split()[0])
+                                ] = int(nlogicline.split()[1])
                             logic_line = network_file.readline().strip()
 
                 # .e = end of file
-                elif '.e' in line:
+                elif ".e" in line:
                     break
             line = network_file.readline()
 
         return self.from_dict(logic, keep_constants=keep_constants, **kwargs)
 
     @classmethod
     def from_string_boolean(self, string, keep_constants=True, **kwargs):
@@ -204,37 +278,48 @@
         logic = defaultdict(dict)
 
         # parse lines to receive node names
         network_file = StringIO(string)
         line = network_file.readline()
         i = 0
         while line != "":
-            if line[0] == '#':
+            if line[0] == "#":
                 line = network_file.readline()
                 continue
-            logic[i] = {'name': line.split("*")[0].strip(), 'in': [], 'out': []}
+            logic[i] = {"name": line.split("*")[0].strip(), "in": [], "out": []}
             line = network_file.readline()
             i += 1
 
         # Parse lines again to determine inputs and output sequence
         network_file = StringIO(string)
         line = network_file.readline()
         i = 0
         while line != "":
-            if line[0] == '#':
+            if line[0] == "#":
                 line = network_file.readline()
                 continue
             eval_line = line.split("=")[1]  # logical condition to evaluate
             # RE checks for non-alphanumeric character before/after node name (node names are included in other node names)
             # Additional characters added to eval_line to avoid start/end of string complications
-            input_names = [logic[node]['name'] for node in logic if re.compile('\W' + logic[node]['name'] + '\W').search('*' + eval_line + '*')]
-            input_nums = [node for input in input_names for node in logic if input == logic[node]['name']]
-            logic[i]['in'] = input_nums
+            input_names = [
+                logic[node]["name"]
+                for node in logic
+                if re.compile(r"\W" + logic[node]["name"] + r"\W").search(
+                    "*" + eval_line + "*"
+                )
+            ]
+            input_nums = [
+                node
+                for input in input_names
+                for node in logic
+                if input == logic[node]["name"]
+            ]
+            logic[i]["in"] = input_nums
             # Determine output transitions
-            logic[i]['out'] = output_transitions(eval_line, input_names)
+            logic[i]["out"] = output_transitions(eval_line, input_names)
             line = network_file.readline()
             i += 1
 
         return self.from_dict(logic, keep_constants=keep_constants, **kwargs)
 
     @classmethod
     def from_dict(self, logic, keep_constants=True, **kwargs):
@@ -248,25 +333,31 @@
             (BooleanNetwork)
 
         See also:
             :func:`from_file` :func:`from_dict`
         """
         Nnodes = len(logic)
         constants = {}
-        if 'name' in kwargs:
-            name = kwargs['name']
+        if "name" in kwargs:
+            name = kwargs["name"]
         else:
-            name = ''
+            name = ""
         if keep_constants:
             for i, nodelogic in logic.items():
                 # No inputs? It's a constant!
-                if len(nodelogic['in']) == 0:
-                    constants[i] = logic[i]['out'][0]
+                if len(nodelogic["in"]) == 0:
+                    constants[i] = logic[i]["out"][0]
 
-        return BooleanNetwork(name=name, logic=logic, Nnodes=Nnodes, constants=constants, keep_constants=keep_constants)
+        return BooleanNetwork(
+            name=name,
+            logic=logic,
+            Nnodes=Nnodes,
+            constants=constants,
+            keep_constants=keep_constants,
+        )
 
     def to_cnet(self, file=None, adjust_no_input=False):
         """Outputs the network logic to ``.cnet`` format, which is similar to the Berkeley Logic Interchange Format (BLIF).
         This is the format used by BNS to compute attractors.
 
         Args:
             file (string,optional) : A string of the file to write the output to. If not supplied, a string will be returned.
@@ -280,40 +371,55 @@
         """
         # Copy
         logic = self.logic.copy()
         #
         if adjust_no_input:
             for i, data in logic.items():
                 # updates in place
-                if len(data['in']) == 0:
-                    data['in'] = [i + 1]
-                    data['out'] = [0, 1]
+                if len(data["in"]) == 0:
+                    data["in"] = [i + 1]
+                    data["out"] = [0, 1]
 
-        bns_string = '.v ' + str(self.Nnodes) + '\n' + '\n'
+        bns_string = ".v " + str(self.Nnodes) + "\n" + "\n"
         for i in range(self.Nnodes):
-            k = len(logic[i]['in'])
-            bns_string += '.n ' + str(i + 1) + " " + str(k) + " " + " ".join([str(v + 1) for v in logic[i]['in']]) + "\n"
+            k = len(logic[i]["in"])
+            bns_string += (
+                ".n "
+                + str(i + 1)
+                + " "
+                + str(k)
+                + " "
+                + " ".join([str(v + 1) for v in logic[i]["in"]])
+                + "\n"
+            )
             for statenum in range(2**k):
                 # If is a constant (TODO: This must come from the BooleanNode, not the logic)
-                if len(logic[i]['out']) == 1:
-                    bns_string += str(logic[i]['out'][statenum]) + "\n"
+                if len(logic[i]["out"]) == 1:
+                    bns_string += str(logic[i]["out"][statenum]) + "\n"
                 # Not a constant, print the state and output
                 else:
-                    bns_string += statenum_to_binstate(statenum, base=k) + " " + str(logic[i]['out'][statenum]) + "\n"
+                    bns_string += (
+                        statenum_to_binstate(statenum, base=k)
+                        + " "
+                        + str(logic[i]["out"][statenum])
+                        + "\n"
+                    )
             bns_string += "\n"
 
         if file is None:
             return bns_string
         else:
             if isinstance(file, str):
-                with open(file, 'w') as iofile:
+                with open(file, "w") as iofile:
                     iofile.write(bns_string)
                     iofile.close()
             else:
-                raise AttributeError("File format not supported. Please specify a string.")
+                raise AttributeError(
+                    "File format not supported. Please specify a string."
+                )
 
     #
     # Methods
     #
     def structural_graph(self, remove_constants=False):
         """Calculates and returns the structural graph of the boolean network.
 
@@ -322,18 +428,20 @@
 
         Returns:
             G (networkx.Digraph) : The boolean network structural graph.
         """
         self._sg = nx.DiGraph(name="Structural Graph: " + self.name)
 
         # Add Nodes
-        self._sg.add_nodes_from((i, {'label': n.name}) for i, n in enumerate(self.nodes))
+        self._sg.add_nodes_from(
+            (i, {"label": n.name}) for i, n in enumerate(self.nodes)
+        )
         for target in range(self.Nnodes):
-            for source in self.logic[target]['in']:
-                self._sg.add_edge(source, target, **{'weight': 1.})
+            for source in self.logic[target]["in"]:
+                self._sg.add_edge(source, target, **{"weight": 1.0})
 
         if remove_constants:
             self._sg.remove_nodes_from(self.get_constants().keys())
         #
         return self._sg
 
     def number_interactions(self):
@@ -374,26 +482,27 @@
         """Calculates and returns the signed interaction graph of the boolean network.  Here, edge weights denote
         if an interaction is activation (1), inhibition (-1), or cannot be classified (0).
 
         Returns:
             G (networkx.Digraph) : The boolean network structural graph.
         """
         signed_ig = nx.DiGraph(name="Signed Interaction Graph: " + self.name)
-        signed_ig.add_nodes_from((i, {'label': n.name}) for i, n in enumerate(self.nodes))
+        signed_ig.add_nodes_from(
+            (i, {"label": n.name}) for i, n in enumerate(self.nodes)
+        )
 
         for target in range(self.Nnodes):
-
             input_signs = self.nodes[target].input_signs()
 
-            for idx, source in enumerate(self.logic[target]['in']):
-                signed_ig.add_edge(source, target, **{'weight': input_signs[idx]})
+            for idx, source in enumerate(self.logic[target]["in"]):
+                signed_ig.add_edge(source, target, **{"weight": input_signs[idx]})
 
         return signed_ig
 
-    def effective_graph(self, bound='mean', threshold=None):
+    def effective_graph(self, bound="mean", threshold=None):
         """Computes and returns the effective graph of the network.
         In practive it asks each :class:`~cana.boolean_node.BooleanNode` for their :func:`~cana.boolean_node.BooleanNode.edge_effectiveness`.
 
         Args:
             bound (string) : The bound to which compute input redundancy.
                 Can be one of : ["lower", "mean", "upper", "tuple"].
                 Defaults to "mean".
@@ -404,34 +513,44 @@
             (networkx.DiGraph) : directed graph
 
         See Also:
             :func:`~cana.boolean_node.BooleanNode.edge_effectiveness`
         """
         if self._eg is None:
             if threshold is not None:
-                self._eg = nx.DiGraph(name="Effective Graph: " + self.name + "(Threshold: {threshold:.2f})".format(threshold=threshold))
+                self._eg = nx.DiGraph(
+                    name="Effective Graph: "
+                    + self.name
+                    + "(Threshold: {threshold:.2f})".format(threshold=threshold)
+                )
             else:
-                self._eg = nx.DiGraph(name="Effective Graph: " + self.name + "(Threshold: None)")
+                self._eg = nx.DiGraph(
+                    name="Effective Graph: " + self.name + "(Threshold: None)"
+                )
 
             # Add Nodes
             for i, node in enumerate(self.nodes, start=0):
-                self._eg.add_node(i, **{'label': node.name})
+                self._eg.add_node(i, **{"label": node.name})
 
             # Add Edges
             for i, node in enumerate(self.nodes, start=0):
                 e_is = node.edge_effectiveness(bound=bound)
-                
-                for inputs, e_i in zip(self.logic[i]['in'], e_is):
+
+                for inputs, e_i in zip(self.logic[i]["in"], e_is):
                     # If there is a threshold, only return those number above the threshold. Else, return all edges.
-                    if (threshold is None) or ((threshold is not None) and (e_i > threshold)):
-                        self._eg.add_edge(inputs, i, **{'weight': e_i})
+                    if (threshold is None) or (
+                        (threshold is not None) and (e_i > threshold)
+                    ):
+                        self._eg.add_edge(inputs, i, **{"weight": e_i})
 
         return self._eg
 
-    def conditional_effective_graph(self, conditioned_nodes={}, bound='mean', threshold=None):
+    def conditional_effective_graph(
+        self, conditioned_nodes={}, bound="mean", threshold=None
+    ):
         """Computes and returns the BN effective graph conditioned on some known states.
 
         Args:
             conditioned_nodes (dict) : a dictionary mapping node ids to their conditioned states.
                 dict of form { nodeid : nodestate }
             bound (string) : The bound to which compute input redundancy.
                 Can be one of : ["lower", "mean", "upper", "tuple"].
@@ -442,114 +561,165 @@
         Returns:
             (networkx.DiGraph) : directed graph
 
         See Also:
             :func:`~cana.boolean_network.BooleanNetwork.effective_graph`
         """
 
-        conditional_eg = copy.deepcopy(self.effective_graph(bound=bound, threshold=None))
+        conditional_eg = copy.deepcopy(
+            self.effective_graph(bound=bound, threshold=None)
+        )
         conditioned_subgraph = set([])
 
         # make a copy of the logic dict so we can edit it
         conditioned_logic = copy.deepcopy(self.logic)
 
         # separate input conditioned nodes and nodes that get conditioned
         all_conditioned_nodes = dict(conditioned_nodes)
         # Queue of nodes to condition
         nodes2condition = list(conditioned_nodes.keys())
 
         while len(nodes2condition) > 0:
-
             conditioned_node = nodes2condition.pop(0)
             conditioned_value = str(all_conditioned_nodes[conditioned_node])
             conditioned_subgraph.add(conditioned_node)
 
             # take all successors of the conditioned node ignoring self-loops
-            successors = [n for n in list(conditional_eg.neighbors(conditioned_node)) if n != conditioned_node]
+            successors = [
+                n
+                for n in list(conditional_eg.neighbors(conditioned_node))
+                if n != conditioned_node
+            ]
             conditioned_subgraph.update(successors)
 
             # we have to loop through all of the successors of the conditioned node and change their logic
             for n in successors:
-
                 # find the index of the conditioned node in the successor logic
-                conditioned_node_idx = conditioned_logic[n]['in'].index(conditioned_node)
+                conditioned_node_idx = conditioned_logic[n]["in"].index(
+                    conditioned_node
+                )
 
-                conditioned_subgraph.update(conditioned_logic[n]['in'])
+                conditioned_subgraph.update(conditioned_logic[n]["in"])
 
                 # the new successor inputs without the conditioned node
-                new_successor_inputs = conditioned_logic[n]['in'][:conditioned_node_idx] + conditioned_logic[n]['in'][(conditioned_node_idx + 1):]
+                new_successor_inputs = (
+                    conditioned_logic[n]["in"][:conditioned_node_idx]
+                    + conditioned_logic[n]["in"][(conditioned_node_idx + 1) :]
+                )
                 newk = len(new_successor_inputs)
 
                 # now we create a conditioned LUT as the subset of the original for which the conditioned node is fixed to its value
                 if newk == 0:
-                    new_successor_outputs = [conditioned_logic[n]['out'][binstate_to_statenum(conditioned_value)]] * 2
+                    new_successor_outputs = [
+                        conditioned_logic[n]["out"][
+                            binstate_to_statenum(conditioned_value)
+                        ]
+                    ] * 2
                 else:
                     new_successor_outputs = []
                     for sn in range(2**newk):
                         binstate = statenum_to_binstate(sn, newk)
-                        binstate = binstate[:conditioned_node_idx] + conditioned_value + binstate[conditioned_node_idx:]
-                        new_successor_outputs.append(conditioned_logic[n]['out'][binstate_to_statenum(binstate)])
+                        binstate = (
+                            binstate[:conditioned_node_idx]
+                            + conditioned_value
+                            + binstate[conditioned_node_idx:]
+                        )
+                        new_successor_outputs.append(
+                            conditioned_logic[n]["out"][binstate_to_statenum(binstate)]
+                        )
 
                 # use the new logic to calcuate a new edge effectiveness
-                new_edge_effectiveness = BooleanNode().from_output_list(new_successor_outputs).edge_effectiveness(bound=bound)
+                new_edge_effectiveness = (
+                    BooleanNode()
+                    .from_output_list(new_successor_outputs)
+                    .edge_effectiveness(bound=bound)
+                )
 
                 # and update the conditional effective graph with the new edge effectiveness values
                 for i in range(newk):
-                    conditional_eg[new_successor_inputs[i]][n]['weight'] = new_edge_effectiveness[i]
+                    conditional_eg[new_successor_inputs[i]][n][
+                        "weight"
+                    ] = new_edge_effectiveness[i]
 
                 # now update the conditioned_logic in case these nodes are further modified by additional conditioned variables
-                conditioned_logic[n]['in'] = new_successor_inputs
-                conditioned_logic[n]['out'] = new_successor_outputs
+                conditioned_logic[n]["in"] = new_successor_inputs
+                conditioned_logic[n]["out"] = new_successor_outputs
 
                 # check if we just made a constant node
-                if n not in all_conditioned_nodes and len(set(new_successor_outputs)) == 1:
+                if (
+                    n not in all_conditioned_nodes
+                    and len(set(new_successor_outputs)) == 1
+                ):
                     # in which case, add it to the conditioned set and propagate the conditioned effect
                     nodes2condition.append(n)
                     all_conditioned_nodes[n] = new_successor_outputs[0]
 
-        conditional_eg.name = "Conditioned Effective Graph: {name:s} conditioned on {nodes:s}".format(name=self.name, nodes=str(conditioned_nodes))
+        conditional_eg.name = (
+            "Conditioned Effective Graph: {name:s} conditioned on {nodes:s}".format(
+                name=self.name, nodes=str(conditioned_nodes)
+            )
+        )
         if threshold is None:
             conditional_eg.name = conditional_eg.name + " (Threshold: None)"
         else:
-            conditional_eg.name = conditional_eg.name + " (Threshold: {threshold:.2f})".format(threshold=threshold)
-            remove_edges = [(i, j) for i, j, d in conditional_eg.edges(data=True) if d['weight'] <= threshold]
+            conditional_eg.name = (
+                conditional_eg.name
+                + " (Threshold: {threshold:.2f})".format(threshold=threshold)
+            )
+            remove_edges = [
+                (i, j)
+                for i, j, d in conditional_eg.edges(data=True)
+                if d["weight"] <= threshold
+            ]
             conditional_eg.remove_edges_from(remove_edges)
 
         # add the conditional information into the effective graph object
-        dict_conditioned_subgraph = {n: (n in conditioned_subgraph) for n in conditional_eg.nodes()}
-        nx.set_node_attributes(conditional_eg, values=dict_conditioned_subgraph, name='conditioned_subgraph')
-
-        dict_all_conditioned_nodes = {n: all_conditioned_nodes.get(n, None) for n in conditional_eg.nodes()}
-        nx.set_node_attributes(conditional_eg, values=dict_all_conditioned_nodes, name='conditioned_state')
+        dict_conditioned_subgraph = {
+            n: (n in conditioned_subgraph) for n in conditional_eg.nodes()
+        }
+        nx.set_node_attributes(
+            conditional_eg,
+            values=dict_conditioned_subgraph,
+            name="conditioned_subgraph",
+        )
+
+        dict_all_conditioned_nodes = {
+            n: all_conditioned_nodes.get(n, None) for n in conditional_eg.nodes()
+        }
+        nx.set_node_attributes(
+            conditional_eg, values=dict_all_conditioned_nodes, name="conditioned_state"
+        )
 
         return conditional_eg
 
     def effective_indegrees(self):
         """Returns the in-degrees of the Effective Graph. Sorted.
 
         Returns:
             (list)
 
         See also:
             :func:`effective_outdegrees`, :func:`structural_indegrees`, :func:`structural_outdegrees`
         """
         self._check_compute_variables(eg=True)
-        return sorted([d for n, d in self._eg.in_degree(weight='weight')], reverse=True)
+        return sorted([d for n, d in self._eg.in_degree(weight="weight")], reverse=True)
 
     def effective_outdegrees(self):
         """Returns the out-degrees of the Effective Graph. Sorted.
 
         Returns:
             (list)
 
         See also:
             :func:`effective_indegrees`, :func:`structural_indegrees`, :func:`structural_outdegrees`
         """
         self._check_compute_variables(eg=True)
-        return sorted([d for n, d in self._eg.out_degree(weight='weight')], reverse=True)
+        return sorted(
+            [d for n, d in self._eg.out_degree(weight="weight")], reverse=True
+        )
 
     def activity_graph(self, threshold=None):
         """
         Returns the activity graph as proposed in
         Ghanbarnejad & Klemm (2012) EPL, 99
 
         Args:
@@ -558,41 +728,48 @@
 
         Returns:
             (networkx.DiGraph) : directed graph
 
         """
 
         if threshold is not None:
-            act_g = nx.DiGraph(name="Activity Graph: " + self.name + "(Threshold: %.2f)" % threshold)
+            act_g = nx.DiGraph(
+                name="Activity Graph: " + self.name + "(Threshold: %.2f)" % threshold
+            )
         else:
-            act_g = nx.DiGraph(name="Activity Graph: " + self.name + "(Threshold: None)")
+            act_g = nx.DiGraph(
+                name="Activity Graph: " + self.name + "(Threshold: None)"
+            )
 
         # Add Nodes
         for i, node in enumerate(self.nodes, start=0):
-            act_g.add_node(i, **{'label': node.name})
+            act_g.add_node(i, **{"label": node.name})
 
         # Add Edges
         for i, node in enumerate(self.nodes, start=0):
-
             a_is = node.activities()
-            for inputs, a_i in zip(self.logic[i]['in'], a_is):
+            for inputs, a_i in zip(self.logic[i]["in"], a_is):
                 # If there is a threshold, only return those number above the threshold. Else, return all edges.
-                if ((threshold is None) and (a_i > 0)) or ((threshold is not None) and (a_i > threshold)):
-                    act_g.add_edge(inputs, i, **{'weight': a_i})
+                if ((threshold is None) and (a_i > 0)) or (
+                    (threshold is not None) and (a_i > threshold)
+                ):
+                    act_g.add_edge(inputs, i, **{"weight": a_i})
 
         return act_g
 
     def state_transition_graph(self):
         """Creates and returns the full State Transition Graph (STG) for the Boolean Network.
 
         Returns:
             (networkx.DiGraph) : The state transition graph for the Boolean Network.
         """
-        self._stg = nx.DiGraph(name='STG: ' + self.name)
-        self._stg.add_nodes_from((i, {'label': self.num2bin(i)}) for i in range(self.Nstates))
+        self._stg = nx.DiGraph(name="STG: " + self.name)
+        self._stg.add_nodes_from(
+            (i, {"label": self.num2bin(i)}) for i in range(self.Nstates)
+        )
         for i in range(self.Nstates):
             b = self.num2bin(i)
             self._stg.add_edge(i, self.bin2num(self.step(b)))
         #
         return self._stg
 
     def stg_indegree(self):
@@ -614,25 +791,29 @@
             (string) : The stepped binary state.
         """
         # for every node:
         #   node input = breaks down initial by node input
         #   asks node to step with the input
         #   append output to list
         # joins the results from each node output
-        assert len(initial) == self.Nnodes, "The initial configuration state does not match the number of nodes"
-        return ''.join([node.step(node.input_mask(initial)) for node in self.nodes])
+        assert (
+            len(initial) == self.Nnodes
+        ), "The initial configuration state does not match the number of nodes"
+        return "".join([node.step(node.input_mask(initial)) for node in self.nodes])
 
     def trajectory(self, initial, length=2):
         """Computes the trajectory of ``length`` steps without the State Transition Graph (STG)."""
         trajectory = [initial]
         for istep in range(length):
             trajectory.append(self.step(trajectory[-1]))
         return trajectory
 
-    def trajectory_to_attractor(self, initial, precompute_attractors=True, return_attractor=False):
+    def trajectory_to_attractor(
+        self, initial, precompute_attractors=True, return_attractor=False
+    ):
         """Computes the trajectory starting at `initial` until it reaches an attracor (this is garanteed).
 
         Args:
             initial (string) : the initial binstate.
             precompute_attractors (bool) : use precomputed attractors, default True.
             return_attractor (bool) : also return the attractor reached, default False.
 
@@ -640,33 +821,35 @@
             (list) : the state trajectory between initial and the final attractor state.
             if return_attractor: (list): the attractor
         """
 
         # if the attractors are already precomputed, then we can check when we reach a known state
         if precompute_attractors:
             self._check_compute_variables(attractors=True)
-            attractor_states = [self.num2bin(s) for att in self._attractors for s in att]
+            attractor_states = [
+                self.num2bin(s) for att in self._attractors for s in att
+            ]
 
             trajectory = [initial]
-            while (trajectory[-1] not in attractor_states):
+            while trajectory[-1] not in attractor_states:
                 trajectory.append(self.step(trajectory[-1]))
 
             if return_attractor:
                 attractor = self.attractor(trajectory[-1])
 
         else:
             trajectory = [initial]
-            while (trajectory[-1] not in trajectory[:-1]):
+            while trajectory[-1] not in trajectory[:-1]:
                 trajectory.append(self.step(trajectory[-1]))
 
             # the attractor starts at the first occurence of the element
             idxatt = trajectory.index(trajectory[-1])
             if return_attractor:
                 attractor = [self.bin2num(s) for s in trajectory[idxatt:-1]]
-            trajectory = trajectory[:(idxatt + 1)]
+            trajectory = trajectory[: (idxatt + 1)]
 
         if return_attractor:
             return trajectory, attractor
         else:
             return trajectory
 
     def attractor(self, initial):
@@ -680,35 +863,39 @@
         self._check_compute_variables(attractors=True)
 
         trajectory = self.trajectory_to_attractor(initial)
         for attractor in self._attractors:
             if self.bin2num(trajectory[-1]) in attractor:
                 return attractor
 
-    def attractors(self, mode='stg'):
+    def attractors(self, mode="stg"):
         """Find the attractors of the boolean network.
 
         Args:
             mode (string) : ``stg`` or ``sat``. Defaults to ``stg``.
                 ``stg``: Uses the full State Transition Graph (STG) and identifies the attractors as strongly connected components.
                 ``bns``: Uses the SAT-based :mod:`cana.bns` to find all attractors.
         Returns:
             attractors (list) : A list containing all attractors for the boolean network.
         See also:
             :mod:`cana.bns`
         """
         self._check_compute_variables(stg=True)
 
-        if mode == 'stg':
+        if mode == "stg":
             self._attractors = [list(a) for a in nx.attracting_components(self._stg)]
 
-        elif mode == 'bns':
-            self._attractors = bns.attractors(self.to_cnet(file=None, adjust_no_input=False))
+        elif mode == "bns":
+            self._attractors = bns.attractors(
+                self.to_cnet(file=None, adjust_no_input=False)
+            )
         else:
-            raise AttributeError("Could not find the specified mode. Try 'stg' or 'bns'.")
+            raise AttributeError(
+                "Could not find the specified mode. Try 'stg' or 'bns'."
+            )
 
         self._attractors.sort(key=len, reverse=True)
         return self._attractors
 
     def network_bias(self):
         """Network Bias. The sum of individual node biases divided by the number of nodes.
         Practically, it asks each node for their own bias.
@@ -718,20 +905,21 @@
 
         See Also:
             :func:`~cana.boolean_node.BooleanNode.bias`
         """
         return sum([node.bias() for node in self.nodes]) / self.Nnodes
 
     def basin_entropy(self, base=2):
-        """
-
-        """
+        """ """
         self._check_compute_variables(stg=True)
 
-        prob_vec = np.array([len(wcc) for wcc in nx.weakly_connected_components(self._stg)]) / 2.0**self.Nnodes
+        prob_vec = (
+            np.array([len(wcc) for wcc in nx.weakly_connected_components(self._stg)])
+            / 2.0**self.Nnodes
+        )
         return entropy(prob_vec, base=base)
 
     def set_constant(self, node, constant=True, state=None):
         """Sets or unsets a node as a constant.
 
         Args:
             node (int) : The node ``id`` in the logic dict.
@@ -750,24 +938,28 @@
 
     def unset_all_constants(self):
         self.keep_constants = False
         for node in self.nodes:
             node.set_constant(constant=False)
 
     def _update_trans_func(self):
-        """Sets the correct functions to convert from binary-state format to/from numeric-state format.
-
-        """
+        """Sets the correct functions to convert from binary-state format to/from numeric-state format."""
         if self.keep_constants:
-            self.Nstates = 2**(self.Nnodes - self.Nconstants)
+            self.Nstates = 2 ** (self.Nnodes - self.Nconstants)
             # The template is a list that identifies the values of constant nodes: [None, '1', None, '0'].
-            constant_template = [None if not node.constant else node.state for node in self.nodes]
-            self.bin2num = lambda bs: constantbinstate_to_statenum(bs, constant_template)
+            constant_template = [
+                None if not node.constant else node.state for node in self.nodes
+            ]
+            self.bin2num = lambda bs: constantbinstate_to_statenum(
+                bs, constant_template
+            )
             self.num2bin = lambda sn: binstate_to_constantbinstate(
-                statenum_to_binstate(sn, base=self.Nnodes - self.Nconstants), constant_template)
+                statenum_to_binstate(sn, base=self.Nnodes - self.Nconstants),
+                constant_template,
+            )
         else:
             self.Nstates = 2**self.Nnodes
             self.bin2num = binstate_to_statenum
             self.num2bin = lambda sn: statenum_to_binstate(sn, base=self.Nnodes)
 
     #
     # Dynamical Control Methods
@@ -782,26 +974,28 @@
         Returns:
             (dict) : The STG-R in dict format.
         """
         self._check_compute_variables(stg=True)
 
         self._stg_r = {}
 
-        if (filename is None):
+        if filename is None:
             for source in self._stg:
                 self._stg_r[source] = len(self._dfs_reachable(self._stg, source)) - 1.0
         else:
             try:
-                with open(filename, 'rb') as handle:
+                with open(filename, "rb") as handle:
                     self._stg_r = pickle.load(handle)
             except IOError:
                 print("Finding STG dict")
                 for source in self._stg:
-                    self._stg_r[source] = len(self._dfs_reachable(self._stg, source)) - 1.0
-                with open(filename, 'wb') as handle:
+                    self._stg_r[source] = (
+                        len(self._dfs_reachable(self._stg, source)) - 1.0
+                    )
+                with open(filename, "wb") as handle:
                     pickle.dump(self._stg_r, handle)
         return self._stg_r
 
     def attractor_driver_nodes(self, min_dvs=1, max_dvs=4, verbose=False):
         """Get the minimum necessary driver nodes by iterating the combination of all possible driver nodes of length :math:`min <= x <= max`.
 
         Args:
@@ -838,15 +1032,19 @@
 
                 if att_reachable_from == 1.0:
                     attractor_controllers_found.append(dvs)
             # Add another driver node
             nr_dvs += 1
 
         if len(attractor_controllers_found) == 0:
-            warnings.warn("No attractor control driver variable sets found after exploring all subsets of size {:,d} to {:,d} nodes!!".format(min_dvs, max_dvs))
+            warnings.warn(
+                "No attractor control driver variable sets found after exploring all subsets of size {:,d} to {:,d} nodes!!".format(
+                    min_dvs, max_dvs
+                )
+            )
 
         return attractor_controllers_found
 
     def controlled_state_transition_graph(self, driver_nodes=[]):
         """Returns the Controlled State-Transition-Graph (CSTG).
         In practice, it copies the original STG, flips driver nodes (variables), and updates the CSTG.
 
@@ -860,19 +1058,28 @@
             :func:`attractor_driver_nodes`, :func:`controlled_attractor_graph`.
         """
         self._check_compute_variables(attractors=True)
 
         if self.keep_constants:
             for dv in driver_nodes:
                 if dv in self.get_constants():
-                    warnings.warn("Cannot control a constant variable '%s'! Skipping" % self.nodes[dv].name )
+                    warnings.warn(
+                        "Cannot control a constant variable '%s'! Skipping"
+                        % self.nodes[dv].name
+                    )
 
         # attractor_states = [s for att in self._attractors for s in att]
         cstg = copy.deepcopy(self._stg)
-        cstg.name = 'C-' + cstg.name + ' (' + ','.join(map(str, [self.nodes[dv].name for dv in driver_nodes])) + ')'
+        cstg.name = (
+            "C-"
+            + cstg.name
+            + " ("
+            + ",".join(map(str, [self.nodes[dv].name for dv in driver_nodes]))
+            + ")"
+        )
 
         # add the control pertubations applied to all other configurations
         for statenum in range(self.Nstates):
             binstate = self.num2bin(statenum)
             controlled_states = flip_binstate_bit_set(binstate, copy.copy(driver_nodes))
             controlled_states.remove(binstate)
 
@@ -897,36 +1104,72 @@
             :func:`controlled_state_transition_graph`, :func:`attractor_driver_nodes`, :func:`controlled_attractor_graph`.
         """
         self._check_compute_variables(attractors=True)
 
         if self.keep_constants:
             for dv in driver_nodes:
                 if dv in self.get_constants():
-                    warnings.warn("Cannot control a constant variable {dv:s}'! Skipping".format(dv=self.nodes[dv].name))
+                    warnings.warn(
+                        "Cannot control a constant variable {dv:s}'! Skipping".format(
+                            dv=self.nodes[dv].name
+                        )
+                    )
 
         uncontrolled_system_size = self.Nnodes - len(driver_nodes)
 
         pcstg_dict = {}
         for att in self._attractors:
-            dn_attractor_transitions = [tuple(''.join([self.num2bin(s)[dn] for dn in driver_nodes]) for s in att_edge)
-                                        for att_edge in self._stg.subgraph(att).edges()]
-
-            pcstg_states = [self.bin2num(binstate_pinned_to_binstate(
-                            statenum_to_binstate(statenum, base=uncontrolled_system_size), attsource, pinned_var=driver_nodes))
-                            for statenum in range(2**uncontrolled_system_size) for attsource, attsink in dn_attractor_transitions]
-
-            pcstg = nx.DiGraph(name='STG: ' + self.name)
-            pcstg.name = 'PC-' + pcstg.name + ' (' + ','.join(map(str, [self.nodes[dv].name for dv in driver_nodes])) + ')'
+            dn_attractor_transitions = [
+                tuple(
+                    "".join([self.num2bin(s)[dn] for dn in driver_nodes])
+                    for s in att_edge
+                )
+                for att_edge in self._stg.subgraph(att).edges()
+            ]
+
+            pcstg_states = [
+                self.bin2num(
+                    binstate_pinned_to_binstate(
+                        statenum_to_binstate(statenum, base=uncontrolled_system_size),
+                        attsource,
+                        pinned_var=driver_nodes,
+                    )
+                )
+                for statenum in range(2**uncontrolled_system_size)
+                for attsource, attsink in dn_attractor_transitions
+            ]
+
+            pcstg = nx.DiGraph(name="STG: " + self.name)
+            pcstg.name = (
+                "PC-"
+                + pcstg.name
+                + " ("
+                + ",".join(map(str, [self.nodes[dv].name for dv in driver_nodes]))
+                + ")"
+            )
 
-            pcstg.add_nodes_from((ps, {'label': ps}) for ps in pcstg_states)
+            pcstg.add_nodes_from((ps, {"label": ps}) for ps in pcstg_states)
 
             for attsource, attsink in dn_attractor_transitions:
                 for statenum in range(2**uncontrolled_system_size):
-                    initial = binstate_pinned_to_binstate(statenum_to_binstate(statenum, base=uncontrolled_system_size), attsource, pinned_var=driver_nodes)
-                    pcstg.add_edge(self.bin2num(initial), self.bin2num(self.pinned_step(initial, pinned_binstate=attsink, pinned_var=driver_nodes)))
+                    initial = binstate_pinned_to_binstate(
+                        statenum_to_binstate(statenum, base=uncontrolled_system_size),
+                        attsource,
+                        pinned_var=driver_nodes,
+                    )
+                    pcstg.add_edge(
+                        self.bin2num(initial),
+                        self.bin2num(
+                            self.pinned_step(
+                                initial,
+                                pinned_binstate=attsink,
+                                pinned_var=driver_nodes,
+                            )
+                        ),
+                    )
 
             pcstg_dict[tuple(att)] = pcstg
 
         return pcstg_dict
 
     def pinned_step(self, initial, pinned_binstate, pinned_var):
         """Steps the boolean network 1 step from the given initial input condition when the driver variables are pinned
@@ -941,15 +1184,22 @@
         """
         # for every node:
         #   node input = breaks down initial by node input
         #   asks node to step with the input
         #   append output to list
         # joins the results from each node output
         assert len(initial) == self.Nnodes
-        return ''.join([str(node.step(''.join(initial[j] for j in self.logic[i]['in']))) if not (i in pinned_var) else initial[i] for i, node in enumerate(self.nodes, start=0)])
+        return "".join(
+            [
+                str(node.step("".join(initial[j] for j in self.logic[i]["in"])))
+                if not (i in pinned_var)
+                else initial[i]
+                for i, node in enumerate(self.nodes, start=0)
+            ]
+        )
 
     def controlled_attractor_graph(self, driver_nodes=[]):
         """
         Args:
             cstg (networkx.DiGraph) : A Controlled State-Transition-Graph (CSTG)
 
         Returns:
@@ -959,42 +1209,53 @@
             :func:`attractor_driver_nodes`, :func:`controlled_state_transition_graph`.
         """
         self._check_compute_variables(attractors=True)
 
         if self.keep_constants:
             for dv in driver_nodes:
                 if dv in self.get_constants():
-                    warnings.warn("Cannot control a constant variable '%s'! Skipping" % self.nodes[dv].name )
+                    warnings.warn(
+                        "Cannot control a constant variable '%s'! Skipping"
+                        % self.nodes[dv].name
+                    )
 
         attractor_states = [s for att in self._attractors for s in att]
         cstg = copy.deepcopy(self._stg)
-        cstg.name = 'C-' + cstg.name + ' Att(' + ','.join(map(str, [self.nodes[dv].name for dv in driver_nodes])) + ')'
+        cstg.name = (
+            "C-"
+            + cstg.name
+            + " Att("
+            + ",".join(map(str, [self.nodes[dv].name for dv in driver_nodes]))
+            + ")"
+        )
 
         # add the control pertubations applied to only attractor configurations
         for statenum in attractor_states:
             binstate = self.num2bin(statenum)
             controlled_states = flip_binstate_bit_set(binstate, copy.copy(driver_nodes))
             controlled_states.remove(binstate)
 
             for constate in controlled_states:
                 cstg.add_edge(statenum, self.bin2num(constate))
 
         Nattract = len(self._attractors)
 
-        cag = nx.DiGraph(name='CAG: ' + cstg.name)
+        cag = nx.DiGraph(name="CAG: " + cstg.name)
         # Nodes
         for i, attr in enumerate(self._attractors):
-            cag.add_node(i, **{'label': '|'.join([self.num2bin(a) for a in attr])})
+            cag.add_node(i, **{"label": "|".join([self.num2bin(a) for a in attr])})
         # Edges
         for i in range(Nattract):
             ireach = self._dfs_reachable(cstg, self._attractors[i][0])
             for j in range(i + 1, Nattract):
                 if self._attractors[j][0] in ireach:
                     cag.add_edge(i, j)
-                if self._attractors[i][0] in self._dfs_reachable(cstg, self._attractors[j][0]):
+                if self._attractors[i][0] in self._dfs_reachable(
+                    cstg, self._attractors[j][0]
+                ):
                     cag.add_edge(j, i)
         return cag
 
     def mean_reachable_configurations(self, cstg):
         """Returns the Mean Fraction of Reachable Configurations
 
         Args:
@@ -1047,15 +1308,17 @@
         att_norm = (float(len(cag)) - 1.0) * len(cag)
 
         if att_norm == 0:
             # if there is only one attractor everything is reachable
             att_reachable_from = 1
         else:
             # otherwise find the reachable from each attractor
-            att_reachable_from = [len(self._dfs_reachable(cag, idxatt)) - 1.0 for idxatt in cag]
+            att_reachable_from = [
+                len(self._dfs_reachable(cag, idxatt)) - 1.0 for idxatt in cag
+            ]
             att_reachable_from = sum(att_reachable_from) / (att_norm)
 
         return att_reachable_from
 
     def fraction_pinned_attractors(self, pcstg_dict):
         """Returns the Number of Accessible Attractors
 
@@ -1107,15 +1370,24 @@
     def _dfs_reachable(self, G, source):
         """Produce nodes in a depth-first-search pre-ordering starting from source."""
         return [n for n in nx.dfs_preorder_nodes(G, source)]
 
     #
     # Feedback Vertex Set (FVS)
     #
-    def feedback_vertex_set_driver_nodes(self, graph='structural', method='grasp', max_iter=1, max_search=11, keep_self_loops=True, *args, **kwargs):
+    def feedback_vertex_set_driver_nodes(
+        self,
+        graph="structural",
+        method="grasp",
+        max_iter=1,
+        max_search=11,
+        keep_self_loops=True,
+        *args,
+        **kwargs
+    ):
         """The minimum set of necessary driver nodes to control the network based on Feedback Vertex Set (FVS) theory.
 
         Args:
             graph (string) : Which graph to perform computation
             method (string) : FVS method. ``bruteforce`` or ``grasp`` (default).
             max_iter (int) : The maximum number of iterations used by the grasp method.
             max_search (int) : The maximum number of searched used by the bruteforce method.
@@ -1127,79 +1399,108 @@
         Note:
             When computing FVS on the structural graph, you might want to use ``remove_constants=True``
             to make sure the resulting set is minimal – since constants are not controlabled by definition.
             Also, when computing on the effective graph, you can define the desired ``threshold`` level.
         """
         self._check_compute_variables(sg=True)
 
-        if graph == 'structural':
+        if graph == "structural":
             dg = self.structural_graph(*args, **kwargs)
-        elif graph == 'effective':
-            dg = self.effective_graph(mode='input', bound='mean', threshold=None, *args, **kwargs)
+        elif graph == "effective":
+            dg = self.effective_graph(
+                mode="input", bound="mean", threshold=None, *args, **kwargs
+            )
         else:
-            raise AttributeError("The graph type '%s' is not accepted. Try 'structural' or 'effective'." % graph)
+            raise AttributeError(
+                "The graph type '%s' is not accepted. Try 'structural' or 'effective'."
+                % graph
+            )
         #
-        if method == 'grasp':
-            fvssets = fvs.fvs_grasp(dg, max_iter=max_iter, keep_self_loops=keep_self_loops)
-        elif method == 'bruteforce':
-            fvssets = fvs.fvs_bruteforce(dg, max_search=max_search, keep_self_loops=keep_self_loops)
+        if method == "grasp":
+            fvssets = fvs.fvs_grasp(
+                dg, max_iter=max_iter, keep_self_loops=keep_self_loops
+            )
+        elif method == "bruteforce":
+            fvssets = fvs.fvs_bruteforce(
+                dg, max_search=max_search, keep_self_loops=keep_self_loops
+            )
         else:
-            raise AttributeError("The FVS method '%s' does not exist. Try 'grasp' or 'bruteforce'." % method)
+            raise AttributeError(
+                "The FVS method '%s' does not exist. Try 'grasp' or 'bruteforce'."
+                % method
+            )
 
         fvssets = [fvc.union(set(self.input_nodes)) for fvc in fvssets]
 
         return fvssets  # [ [self.nodes[i].name for i in fvsset] for fvsset in fvssets]
 
     #
     # Minimum Dominating Set
     #
-    def minimum_dominating_set_driver_nodes(self, graph='structural', max_search=5, keep_self_loops=True, *args, **kwargs):
+    def minimum_dominating_set_driver_nodes(
+        self, graph="structural", max_search=5, keep_self_loops=True, *args, **kwargs
+    ):
         """The minimun set of necessary driver nodes to control the network based on Minimum Dominating Set (MDS) theory.
 
         Args:
             max_search (int) : Maximum search of additional variables. Defaults to 5.
             keep_self_loops (bool) : If self-loops are used in the computation.
 
         Returns:
             (list) : A list-of-lists with MDS solution nodes.
         """
         self._check_compute_variables(sg=True)
         #
-        if graph == 'structural':
+        if graph == "structural":
             dg = self.structural_graph(*args, **kwargs)
-        elif graph == 'effective':
-            dg = self.effective_graph(mode='input', bound='mean', threshold=None, *args, **kwargs)
+        elif graph == "effective":
+            dg = self.effective_graph(
+                mode="input", bound="mean", threshold=None, *args, **kwargs
+            )
         else:
-            raise AttributeError("The graph type '%s' is not accepted. Try 'structural' or 'effective'." % graph)
+            raise AttributeError(
+                "The graph type '%s' is not accepted. Try 'structural' or 'effective'."
+                % graph
+            )
         #
 
         mdssets = mds.mds(dg, max_search=max_search, keep_self_loops=keep_self_loops)
         return mdssets  # [ [self.nodes[i].name for i in mdsset] for mdsset in mdssets]
 
     # Structural Controllability
     #
-    def structural_controllability_driver_nodes(self, graph='structural', keep_self_loops=True, *args, **kwargs):
+    def structural_controllability_driver_nodes(
+        self, graph="structural", keep_self_loops=True, *args, **kwargs
+    ):
         """The minimum set of necessary driver nodes to control the network based on Structural Controlability (SC) theory.
 
         Args:
             keep_self_loops (bool) : If self-loops are used in the computation.
 
         Returns:
             (list) : A list-of-lists with SC solution nodes.
         """
         self._check_compute_variables(sg=True)
 
-        if graph == 'structural':
+        if graph == "structural":
             dg = self.structural_graph(*args, **kwargs)
-        elif graph == 'effective':
-            dg = self.effective_graph(mode='input', bound='mean', threshold=None, *args, **kwargs)
+        elif graph == "effective":
+            dg = self.effective_graph(
+                mode="input", bound="mean", threshold=None, *args, **kwargs
+            )
         else:
-            raise AttributeError("The graph type '%s' is not accepted. Try 'structural' or 'effective'." % graph)
+            raise AttributeError(
+                "The graph type '%s' is not accepted. Try 'structural' or 'effective'."
+                % graph
+            )
         #
-        scsets = [set(scset).union(set(self.input_nodes)) for scset in sc.sc(dg, keep_self_loops=keep_self_loops)]
+        scsets = [
+            set(scset).union(set(self.input_nodes))
+            for scset in sc.sc(dg, keep_self_loops=keep_self_loops)
+        ]
         return scsets  # [ [self.nodes[i].name for i in scset] for scset in scsets]
 
     #
     # Dynamical Impact
     #
     def partial_derative_node(self, node, n_traj=10, t=1):
         """The partial derivative of node on all other nodes after t steps
@@ -1213,31 +1514,39 @@
                 if 0 then the full STG is used to calculate the true value instead of the approximation method.
 
         Returns:
             (vector) : the partial derivatives
         """
         partial = np.zeros((t, self.Nnodes), dtype=float)
         if n_traj == 0:
-            config_genderator = (self.num2bin(statenum) for statenum in range(self.Nstates))
+            config_genderator = (
+                self.num2bin(statenum) for statenum in range(self.Nstates)
+            )
             n_traj = self.Nstates
         else:
             # sample configurations
-            config_genderator = (random_binstate(self.Nnodes) for itraj in range(n_traj))
+            config_genderator = (
+                random_binstate(self.Nnodes) for itraj in range(n_traj)
+            )
 
         for config in config_genderator:
             perturbed_config = flip_binstate_bit(config, node)
             for n_step in range(t):
                 config = self.step(config)
                 perturbed_config = self.step(perturbed_config)
-                partial[n_step] += np.logical_not(binstate_compare(config, perturbed_config))
+                partial[n_step] += np.logical_not(
+                    binstate_compare(config, perturbed_config)
+                )
         partial /= n_traj
 
         return partial
 
-    def approx_dynamic_impact(self, source, n_steps=1, target_set=None, bound='mean', threshold=0.0):
+    def approx_dynamic_impact(
+        self, source, n_steps=1, target_set=None, bound="mean", threshold=0.0
+    ):
         """Use the network structure to approximate the dynamical impact of a perturbation to node for each of n_steps
         for details see: Gates et al (2020).
 
         Args:
             source (int) : the source index for perturbations
             n_steps (int) : the number of time steps
 
@@ -1254,78 +1563,86 @@
 
         Gstr = self.structural_graph()
 
         Geff = self.effective_graph(bound=bound, threshold=threshold)
 
         # the maximum path with length given by product of weights is the same as minimal path of negative log weight
         def eff_weight_func(u, v, e):
-            return -np.log(e['weight'])
+            return -np.log(e["weight"])
 
         def inv_eff_weight_func(pathlength):
             return np.exp(-pathlength)
 
-
         impact_matrix = np.zeros((2, n_steps + 1, len(target_set)))
-        impact_matrix[0, :, :] = self.Nnodes + 1  # if we can't reach the node, then the paths cant be longer than the number of nodes in the graph
+        impact_matrix[0, :, :] = (
+            self.Nnodes + 1
+        )  # if we can't reach the node, then the paths cant be longer than the number of nodes in the graph
         # note that by default: impact_matrix[1, :, :] = 0 the minimum path for nodes we cant reach in the effective graph
 
         # in the structural graph, calcluate the dijkstra shortest paths from the source to all targets that are shorter than the cufoff
-        Gstr_shortest_dist, Gstr_shortest_paths = nx.single_source_dijkstra(Gstr, source, target=None, cutoff=n_steps)
+        Gstr_shortest_dist, Gstr_shortest_paths = nx.single_source_dijkstra(
+            Gstr, source, target=None, cutoff=n_steps
+        )
         Gstr_shortest_dist = {n: int(l) for n, l in Gstr_shortest_dist.items()}
 
         # in the effective graph, calcluate the dijkstra shortest paths from the source to all targets that are shorter than the cufoff
         # where the edge weight is given by the effective weight function
-        Geff_shortest_dist, Geff_shortest_paths = nx.single_source_dijkstra(Geff, source, target=None, cutoff=n_steps, weight=eff_weight_func)
+        Geff_shortest_dist, Geff_shortest_paths = nx.single_source_dijkstra(
+            Geff, source, target=None, cutoff=n_steps, weight=eff_weight_func
+        )
 
         for itar, target in enumerate(target_set):
-
             # we dont need to worry about a path to iteself (source==target)
             # and if the target doesnt appear in the shortest path dict, then no path exists that is less than the cutoff
             if target != source and not Gstr_shortest_dist.get(target, None) is None:
-
                 # the light cone is at least as big as the number of edges in the structural shorest path
-                impact_matrix[0, list(range(Gstr_shortest_dist[target], n_steps + 1)), itar] = Gstr_shortest_dist[target]
+                impact_matrix[
+                    0, list(range(Gstr_shortest_dist[target], n_steps + 1)), itar
+                ] = Gstr_shortest_dist[target]
 
                 # if the path exists, then the number of edges (timesteps) is one less than the number of nodes
                 if not Geff_shortest_paths.get(target, None) is None:
                     eff_path_steps = len(Geff_shortest_paths[target]) - 1
                 else:
                     # or the path doesnt exist
-                    eff_path_steps = n_steps + 100 # any number bigger than the longest path to represent we cannot reach the node
-
+                    eff_path_steps = (
+                        n_steps + 100
+                    )  # any number bigger than the longest path to represent we cannot reach the node
 
                 # start by checking if the number of timesteps is less than the maximum allowable number of steps
                 if eff_path_steps <= n_steps:
-
                     # now check if the most likely effective path is longer (in terms of # of timesteps) than the structural shortest path
                     if eff_path_steps > Gstr_shortest_dist[target]:
-
                         # if it is, then we need to find another effective path constrained by the light-cone
                         # for all time steps where the most likely effective path is longer (in terms of # of timesteps)
                         # than the structural shortest path
                         for istep in range(Gstr_shortest_dist[target], eff_path_steps):
-
                             # bc the effective graph has fully redundant edges, there may actually not be a path
                             try:
-                                redo_dijkstra_dist, _ = nx.single_source_dijkstra(Geff,
+                                redo_dijkstra_dist, _ = nx.single_source_dijkstra(
+                                    Geff,
                                     source=source,
                                     target=target,
                                     cutoff=istep,
-                                    weight=eff_weight_func)
-                                impact_matrix[1, istep, itar] = inv_eff_weight_func(redo_dijkstra_dist)
+                                    weight=eff_weight_func,
+                                )
+                                impact_matrix[1, istep, itar] = inv_eff_weight_func(
+                                    redo_dijkstra_dist
+                                )
                             except nx.NetworkXNoPath:
                                 pass
 
                     # once the lightcone includes the target node on the effective shortest path,
                     # then for all other steps the effective path is the best
-                    impact_matrix[1, list(range(eff_path_steps, n_steps + 1)), itar] = inv_eff_weight_func(Geff_shortest_dist[target])
+                    impact_matrix[
+                        1, list(range(eff_path_steps, n_steps + 1)), itar
+                    ] = inv_eff_weight_func(Geff_shortest_dist[target])
 
         return impact_matrix[:, 1:]
 
-
     def dist_from_attractor(self):
         """Find the distance from attractor for each configuration.
 
         Returns:
             distance (dict). Nodes are dictionary indexes and distances the values.
         """
         self._check_compute_variables(attractors=True)
@@ -1369,74 +1686,83 @@
         """
         CMs = []
         for node in self.nodes:
             if self.keep_constants or not node.constant:
                 CMs.append(node.canalizing_map(output))
         # https://networkx.github.io/documentation/stable/reference/algorithms/generated/networkx.algorithms.operators.all.compose_all.html
         DCM = nx.compose_all(CMs)
-        DCM.name = 'DCM: %s' % (self.name)
+        DCM.name = "DCM: %s" % (self.name)
 
         if simplify:
             # Loop all threshold nodes
-            threshold_nodes = [(n, d) for n, d in DCM.nodes(data=True) if d['type'] == 'threshold']
+            threshold_nodes = [
+                (n, d) for n, d in DCM.nodes(data=True) if d["type"] == "threshold"
+            ]
             for n, d in threshold_nodes:
-
                 # Constant, remove threshold node
-                if d['tau'] == 0:
+                if d["tau"] == 0:
                     DCM.remove_node(n)
 
                 # Tau == 1
-                if d['tau'] == 1:
+                if d["tau"] == 1:
                     in_nei = list(DCM.in_edges(n))[0]
                     out_nei = list(DCM.out_edges(n))[0]
 
                     # neis = set(list(in_nei) + list(out_nei))
 
                     # Convert to self loop
-                    if (in_nei == out_nei[::-1]):
+                    if in_nei == out_nei[::-1]:
                         DCM.remove_node(n)
-                        DCM.add_edge(in_nei[0], out_nei[1], **{'type': 'simplified', 'mode': 'selfloop'})
+                        DCM.add_edge(
+                            in_nei[0],
+                            out_nei[1],
+                            **{"type": "simplified", "mode": "selfloop"}
+                        )
                     # Link variables nodes directly
-                    elif not any([DCM.nodes[tn]['type'] == 'fusion' for tn in in_nei]):
+                    elif not any([DCM.nodes[tn]["type"] == "fusion" for tn in in_nei]):
                         DCM.remove_node(n)
-                        DCM.add_edge(in_nei[0], out_nei[1], **{'type': 'simplified', 'mode': 'direct'})
+                        DCM.add_edge(
+                            in_nei[0],
+                            out_nei[1],
+                            **{"type": "simplified", "mode": "direct"}
+                        )
         # Remove Isolates
         isolates = list(nx.isolates(DCM))
         DCM.remove_nodes_from(isolates)
 
         return DCM
 
     def _check_compute_variables(self, **kwargs):
         """Recursevely check if the requested control variables are instantiated/computed.
         Otherwise computes them in order.
         """
-        if 'sg' in kwargs:
+        if "sg" in kwargs:
             if self._sg is None:
                 self._sg = self.structural_graph()
 
-        elif 'eg' in kwargs:
+        elif "eg" in kwargs:
             if self._eg is None:
                 self._eg = self.effective_graph()
 
-        elif 'stg' in kwargs:
+        elif "stg" in kwargs:
             if self._stg is None:
                 self._check_compute_variables(sg=True)
                 self._stg = self.state_transition_graph()
 
-        elif 'attractors' in kwargs:
+        elif "attractors" in kwargs:
             if self._attractors is None:
                 self._check_compute_variables(stg=True)
                 self._attractors = self.attractors()
 
-        elif 'stg_r' in kwargs:
+        elif "stg_r" in kwargs:
             if self._stg_r is None:
                 self._check_compute_variables(stg=True)
                 self._stg_r = self.state_transition_graph_reachability()
         else:
-            raise Exception('Control variable name not found. %s' % kwargs)
+            raise Exception("Control variable name not found. %s" % kwargs)
         return True
 
     #
     # Get Node Names from Ids
     #
     def _get_node_name(self, id):
         """Return the name of the node based on its id.
@@ -1445,16 +1771,20 @@
             id (int): id of the node.
 
         Returns:
             name (string): name of the node.
         """
         try:
             node = self.nodes[id]
-        except error:
-            raise AttributeError("Node with id {id:d} does not exist. {error::s}".format(id=id, error=error))
+        except Exception as error:
+            raise AttributeError(
+                "Node with id {id:d} does not exist. {error::s}".format(
+                    id=id, error=error
+                )
+            )
         else:
             return node.name
 
     def get_node_name(self, iterable=[]):
         """Return node names. Optionally, it returns only the names of the ids requested.
 
         Args:
@@ -1469,28 +1799,36 @@
         # No ids requested, return all the names
         if not len(iterable):
             return [n.name for n in self.nodes]
         # otherwise, use the recursive map to change ids to names
         else:
             return recursive_map(self._get_node_name, iterable)
 
-    def average_trajectory_length(self, nsamples=10, random_seed=None, method='random'):
+    def average_trajectory_length(self, nsamples=10, random_seed=None, method="random"):
         """The average length of trajectories from a random initial configuration to its attractor.
 
         Args:
             nsamples (int) : The number of samples per hammimg distance to get.
             random_seed (int) : The random state seed.
             method (string) : specify the method you want. either 'random' or ....
 
         Returns:
             trajlen (float) : The average trajectory length to an attractor.
         """
-        return sum(len(self.trajectory_to_attractor(random_binstate(self.Nnodes))) for isample in range(nsamples)) / nsamples
-
-    def derrida_curve(self, nsamples=10, max_hamm=None, random_seed=None, method='random'):
+        return (
+            sum(
+                len(self.trajectory_to_attractor(random_binstate(self.Nnodes)))
+                for isample in range(nsamples)
+            )
+            / nsamples
+        )
+
+    def derrida_curve(
+        self, nsamples=10, max_hamm=None, random_seed=None, method="random"
+    ):
         """The Derrida Curve (also reffered as criticality measure :math:`D_s`).
         When "mode" is set as "random" (default), it would use random sampling to estimate Derrida value
         If "mode" is set as "sensitivity", it would use c-sensitivity to calculate Derrida value (slower)
         You can refer to :cite:'kadelka2017influence' about why c-sensitivity can be used to caculate Derrida value
 
         Args:
             nsamples (int) : The number of samples per hammimg distance to get.
@@ -1505,35 +1843,53 @@
 
         if max_hamm is None or (max_hamm > self.Nnodes):
             max_hamm = self.Nnodes
 
         dx = np.linspace(0, 1, max_hamm, endpoint=True)
         dy = np.zeros(max_hamm + 1)
 
-        if method == 'random':
+        if method == "random":
             # for each possible hamming distance between the starting states
             for hamm_dist in range(1, max_hamm + 1):
-
                 # sample nsample times
                 for isample in range(nsamples):
                     rnd_config = random_binstate(self.Nnodes)
                     perturbed_var = random.sample(range(self.Nnodes), hamm_dist)
-                    perturbed_config = [flip_bit(rnd_config[ivar]) if ivar in perturbed_var else rnd_config[ivar] for ivar in range(self.Nnodes)]
-                    dy[hamm_dist] += hamming_distance(self.step(rnd_config), self.step(perturbed_config)) / self.Nnodes  # normalized Hamming Distance
+                    perturbed_config = [
+                        flip_bit(rnd_config[ivar])
+                        if ivar in perturbed_var
+                        else rnd_config[ivar]
+                        for ivar in range(self.Nnodes)
+                    ]
+                    dy[hamm_dist] += (
+                        hamming_distance(
+                            self.step(rnd_config), self.step(perturbed_config)
+                        )
+                        / self.Nnodes
+                    )  # normalized Hamming Distance
 
             dy /= nsamples
 
-        elif method == 'sensitivity':
-
+        elif method == "sensitivity":
             for hamm_dist in range(1, max_hamm + 1):
-                dy[hamm_dist] = sum([node.c_sensitivity(hamm_dist, mode='forceK', max_k=self.Nnodes) for node in self.nodes]) / self.Nnodes
+                dy[hamm_dist] = (
+                    sum(
+                        [
+                            node.c_sensitivity(
+                                hamm_dist, mode="forceK", max_k=self.Nnodes
+                            )
+                            for node in self.nodes
+                        ]
+                    )
+                    / self.Nnodes
+                )
 
         return dx, dy
 
-    def derrida_coefficient(self, nsamples=10, random_seed=None, method='random'):
+    def derrida_coefficient(self, nsamples=10, random_seed=None, method="random"):
         """The Derrida Coefficient.
         When "mode" is set as "random" (default), it would use random sampling to estimate Derrida value
         If "mode" is set as "sensitivity", it would use c-sensitivity to calculate Derrida value (slower)
         You can refer to :cite:'kadelka2017influence' about why c-sensitivity can be used to caculate Derrida value
 
         Args:
             nsamples (int) : The number of samples per hammimg distance to get.
@@ -1542,25 +1898,37 @@
 
         Returns:
             (dx,dy) (tuple) : The dx and dy of the curve.
         """
         random.seed(random_seed)
         hamm_dist = 1
 
-        if method == 'random':
+        if method == "random":
             # for each possible hamming distance between the starting states
 
             dy = 0
             # sample nsample times
             for isample in range(nsamples):
                 rnd_config = random_binstate(self.Nnodes)
                 perturbed_var = random.sample(range(self.Nnodes), hamm_dist)
-                perturbed_config = [flip_bit(rnd_config[ivar]) if ivar in perturbed_var else rnd_config[ivar] for ivar in range(self.Nnodes)]
-                dy += hamming_distance(self.step(rnd_config), self.step(perturbed_config))
+                perturbed_config = [
+                    flip_bit(rnd_config[ivar])
+                    if ivar in perturbed_var
+                    else rnd_config[ivar]
+                    for ivar in range(self.Nnodes)
+                ]
+                dy += hamming_distance(
+                    self.step(rnd_config), self.step(perturbed_config)
+                )
 
             dy /= float(nsamples)
 
-        elif method == 'sensitivity':
+        elif method == "sensitivity":
             # raise NotImplementedError
-            dy = sum([node.c_sensitivity(hamm_dist, mode='forceK', max_k=self.Nnodes) for node in self.nodes])
+            dy = sum(
+                [
+                    node.c_sensitivity(hamm_dist, mode="forceK", max_k=self.Nnodes)
+                    for node in self.nodes
+                ]
+            )
 
-        return dy / float(self.Nnodes)
+        return dy / float(self.Nnodes)
```

### Comparing `cana-0.2.0/cana/boolean_node.py` & `cana-1.0.0/cana/boolean_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,89 +9,140 @@
 #   Copyright (C) 2021 by
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Alex Gates <ajgates@gmail.com>
 #   Etienne Nzabarushimana <enzabaru@indiana.edu>
 #   All rights reserved.
 #   MIT license.
 from __future__ import division
+
+from itertools import combinations, compress, product
+from statistics import mean
+
+import networkx as nx
 import numpy as np
 import pandas as pd
-from statistics import mean
-from itertools import compress, combinations
-from cana.canalization import boolean_canalization as BCanalization
-from cana.canalization import cboolean_canalization as cBCanalization
-from cana.utils import *
-from cana.cutils import *
+
+import cana.canalization.boolean_canalization as BCanalization
+import cana.canalization.cboolean_canalization as cBCanalization
+from cana.cutils import (
+    binstate_to_statenum,
+    flip_bit,
+    outputs_to_binstates_of_given_type,
+    statenum_to_binstate,
+)
+from cana.utils import input_monotone, ncr
 
 
 class BooleanNode(object):
-    """
-    """
+    """ """
 
-    def __init__(self, id=0, name='x', k=1, inputs=[1], state=False, outputs=[0, 1], constant=False, network=None, verbose=False, *args, **kwargs):
-        self.id = id                            # the id of the node
-        self.name = name                        # the name of the node
-        self.k = k                              # k is the number of inputs
-        self.inputs = list(map(int, inputs))    # the ids of the input nodes
-        self.state = str(int(state))            # the initial state of the node. internally this is treated as a string.
+    def __init__(
+        self,
+        id=0,
+        name="x",
+        k=1,
+        inputs=[1],
+        state=False,
+        outputs=[0, 1],
+        constant=False,
+        network=None,
+        verbose=False,
+        *args,
+        **kwargs
+    ):
+        self.id = id  # the id of the node
+        self.name = name  # the name of the node
+        self.k = k  # k is the number of inputs
+        self.inputs = list(map(int, inputs))  # the ids of the input nodes
+        self.state = str(
+            int(state)
+        )  # the initial state of the node. internally this is treated as a string.
         self.outputs = list(map(str, outputs))  # the list of transition outputs
-        self.network = network                  # the BooleanNetwork object this nodes belongs to
-        self.verbose = verbose                  # verbose mode
+        self.network = network  # the BooleanNetwork object this nodes belongs to
+        self.verbose = verbose  # verbose mode
 
         # mask for inputs
         if len(self.inputs) > 0:
             self.mask = [(i in self.inputs) for i in range(max(self.inputs) + 1)]
         else:
             self.mask = []
 
         # Consistency
         if (k != 0) and (k != int(np.log2(len(outputs)))):
-            raise ValueError('Number of k (inputs) do not match the number of output transitions')
+            raise ValueError(
+                "Number of k (inputs) do not match the number of output transitions"
+            )
 
         # If all outputs are either positive or negative, the node is treated as a constant.
         if (len(set(outputs)) == 1) or (constant):
             self.set_constant(constant=True, state=outputs[0])
         else:
             self.set_constant(constant=False)
 
         # Canalization Variables
-        self._prime_implicants = None           # A tuple of negative and positive prime implicants.
-        self._two_symbols = None                # The Two Symbol (TS) Schemata
-        self._pi_coverage = None                # The Coverage of inputs by Prime Implicants schemata
-        self._ts_coverage = None                # The Coverage of inputs by Two Symbol schemata
+        self._prime_implicants = (
+            None  # A tuple of negative and positive prime implicants.
+        )
+        self._two_symbols = None  # The Two Symbol (TS) Schemata
+        self._pi_coverage = None  # The Coverage of inputs by Prime Implicants schemata
+        self._ts_coverage = None  # The Coverage of inputs by Two Symbol schemata
 
     def __str__(self):
         if len(self.outputs) > 10:
-            outputs = '[' + ','.join(map(str, self.outputs[:4])) + '...' + ','.join(map(str, self.outputs[-4:])) + ']'
+            outputs = (
+                "["
+                + ",".join(map(str, self.outputs[:4]))
+                + "..."
+                + ",".join(map(str, self.outputs[-4:]))
+                + "]"
+            )
         else:
-            outputs = '[' + ','.join(map(str, self.outputs)) + ']'
-        inputs = '[' + ','.join(map(str, self.inputs)) + ']'
+            outputs = "[" + ",".join(map(str, self.outputs)) + "]"
+        inputs = "[" + ",".join(map(str, self.inputs)) + "]"
         return "<BNode(id={id}, name='{name}', k={k}, inputs={inputs:s}, state='{state}', outputs={outputs} constant={constant})>".format(
-            id=self.id, name=self.name, k=self.k, inputs=inputs, state=self.state, outputs=outputs, constant=self.constant)
+            id=self.id,
+            name=self.name,
+            k=self.k,
+            inputs=inputs,
+            state=self.state,
+            outputs=outputs,
+            constant=self.constant,
+        )
 
     @classmethod
     def from_output_list(self, outputs=list(), *args, **kwargs):
         """Instanciate a Boolean Node from a output transition list.
 
         Args:
             outputs (list) : The transition outputs of the node.
 
         Returns:
             (BooleanNode) : the instanciated object.
 
         Example:
             >>> BooleanNode.from_output_list(outputs=[0,0,0,1], name="AND")
         """
-        id = kwargs.pop('id') if 'id' in kwargs else 0
-        name = kwargs.pop('name') if 'name' in kwargs else 'x'
+        id = kwargs.pop("id") if "id" in kwargs else 0
+        name = kwargs.pop("name") if "name" in kwargs else "x"
         k = int(np.log2(len(outputs)))
-        inputs = kwargs.pop('inputs') if 'inputs' in kwargs else [(x + 1) for x in range(k)]
-        state = kwargs.pop('state') if 'state' in kwargs else False
-
-        return BooleanNode(id=id, name=name, k=k, inputs=inputs, state=state, outputs=outputs, *args, **kwargs)
+        inputs = (
+            kwargs.pop("inputs") if "inputs" in kwargs else [(x + 1) for x in range(k)]
+        )
+        state = kwargs.pop("state") if "state" in kwargs else False
+
+        return BooleanNode(
+            id=id,
+            name=name,
+            k=k,
+            inputs=inputs,
+            state=state,
+            outputs=outputs,
+            *args,
+            **kwargs
+        )
 
     def set_constant(self, constant=True, state=None):
         """Sets whether the node is to be treated as a contant
 
         Args:
             constant (Boolean) : Whether to set or unset the node as a constant.
             state (str; optional) : The state value to which to set the node. Either '0' or '1'; default to current state value.
@@ -103,16 +154,15 @@
             self.constant = False
             self.step = self.dynamic_step
         # Set an optional value to the node
         if state is not None:
             self.state = str(int(state))
 
     def constant_step(self, input_state):
-        """Treat the node as a constant variable, always returning its state.
-        """
+        """Treat the node as a constant variable, always returning its state."""
         return self.state
 
     def dynamic_step(self, input_state):
         """Returns the output of the node based on a specific input.
 
         Args:
             input (str) : an input to the node (e.g.: '0111' -> 7).
@@ -148,36 +198,37 @@
 
         Note:
             The complete mathematical description can be found in :cite:`Marques-Pita:2013`.
 
         See also:
             :func:`effective_connectivity`, :func:`input_symmetry`, :func:`edge_redundancy`.
         """
-        # Canalization can only occur when k>= 2 (incorrect: k=1 has redundancy if constant function)
-        # NOTE: commented out by Austin Marcus 8/10/22
-        # if self.k < 2:
-        #     return 0.0
 
         self._check_compute_canalization_variables(pi_coverage=True)
 
-        if not hasattr(operator, '__call__'):
-            raise AttributeError('The operator you selected must be a function. Try "min", "statitics.mean", or "max".')
-
-        redundancy = [operator([pi.count('#') for pi in self._pi_coverage[binstate]]) for binstate in self._pi_coverage]
+        if not hasattr(operator, "__call__"):
+            raise AttributeError(
+                'The operator you selected must be a function. Try "min", "statitics.mean", or "max".'
+            )
+
+        redundancy = [
+            operator([pi.count("#") for pi in self._pi_coverage[binstate]])
+            for binstate in self._pi_coverage
+        ]
 
         k_r = sum(redundancy) / 2**self.k
 
-        if (norm):
+        if norm:
             # Normalizes
             k_r = k_r / self.k
 
         return k_r
 
-    def edge_redundancy(self, bound='mean'):
-        r""" The Edge Redundancy :math:`r_{i}` is the mean number of unnecessary inputs (or ``#``) in the Prime Implicants Look Up Table (LUT) for that input.
+    def edge_redundancy(self, bound="mean"):
+        r"""The Edge Redundancy :math:`r_{i}` is the mean number of unnecessary inputs (or ``#``) in the Prime Implicants Look Up Table (LUT) for that input.
         Since there may be more than one redescription schema for each input entry, the input redundancy is bounded by an upper and lower limit.
 
         .. math::
 
             r_i(x_i) = \frac{ \sum_{f_{\alpha} \in F} \Phi_{\theta:f_{\alpha} \in \Theta_{\theta}} (X^{\#}_{\theta_i} ) }{ |F| }
 
         where :math:`\Phi` is a function (:math:`min` or :math:`max`) and :math:`F` is the node LUT.
@@ -206,24 +257,36 @@
         pi_edge_coverage = cBCanalization.input_wildcard_coverage(self._pi_coverage)
         # Loop ever input node
         for edge, binstates2wildcard in pi_edge_coverage.items():
             # {'numstate': [matches], '10': [True,False,True,...] ...}
 
             # countslenghts = {binstate_to_statenum(binstate): ([pi=='#' for pi in pis]) for binstate,pis in binstates.items() }
             # A triplet of (min, mean, max) values
-            if bound == 'lower':
-                redundancy = sum([all(pi) for pi in binstates2wildcard.values()]) / 2**self.k  # min(r_i)
-            elif bound == 'mean' or bound == 'avg':
-                redundancy = sum([sum(pi) / len(pi) for pi in binstates2wildcard.values()]) / 2**self.k  # <r_i>
-            elif bound == 'upper':
-                redundancy = sum([any(pi) for pi in binstates2wildcard.values()]) / 2**self.k  # max(r_i)
-            elif bound == 'tuple':
-                redundancy = (sum([all(pi) for pi in binstates2wildcard.values()]) / 2**self.k, sum([any(pi) for pi in binstates2wildcard.values()]) / 2**self.k)  # (min,max)
+            if bound == "lower":
+                redundancy = (
+                    sum([all(pi) for pi in binstates2wildcard.values()]) / 2**self.k
+                )  # min(r_i)
+            elif bound == "mean" or bound == "avg":
+                redundancy = (
+                    sum([sum(pi) / len(pi) for pi in binstates2wildcard.values()])
+                    / 2**self.k
+                )  # <r_i>
+            elif bound == "upper":
+                redundancy = (
+                    sum([any(pi) for pi in binstates2wildcard.values()]) / 2**self.k
+                )  # max(r_i)
+            elif bound == "tuple":
+                redundancy = (
+                    sum([all(pi) for pi in binstates2wildcard.values()]) / 2**self.k,
+                    sum([any(pi) for pi in binstates2wildcard.values()]) / 2**self.k,
+                )  # (min,max)
             else:
-                raise AttributeError('The bound you selected does not exist. Try "upper", "mean", "lower" or "tuple".')
+                raise AttributeError(
+                    'The bound you selected does not exist. Try "upper", "mean", "lower" or "tuple".'
+                )
 
             redundancies.append(redundancy)
 
         return redundancies  # r_i
 
     def effective_connectivity(self, operator=mean, norm=True):
         r"""The Effective Connectiviy is the mean number of input nodes needed to determine the transition of the node.
@@ -245,19 +308,19 @@
 
         See Also:
             :func:`input_redundancy`, :func:`input_symmetry`, :func:`~cana.boolean_network.BooleanNetwork.effective_graph`.
         """
         k_r = self.input_redundancy(operator=operator, norm=False)
         #
         k_e = self.k - k_r
-        if (norm):
+        if norm:
             k_e = k_e / self.k
         return k_e
 
-    def edge_effectiveness(self, bound='mean'):
+    def edge_effectiveness(self, bound="mean"):
         r"""The Edge Effectiveness is the mean number of an input's states needed to determine the transition of the node.
 
         .. math::
 
             e_i(x_i) = 1 - r_i(x_i)
 
         Args:
@@ -268,143 +331,109 @@
 
         See Also:
             :func:`input_redundancy`, :func:`input_symmetry`, :func:`~cana.boolean_network.BooleanNetwork.effective_graph`.
         """
         e_i = [1.0 - x_i for x_i in self.edge_redundancy(bound=bound)]
         return e_i
 
-    def edge_symmetry(self, bound='upper'):
-        r"""Edge Symmetry is a measure of permutation redundancy of a single input.
-        Similar to the computation of Edge Effectiveness but using the Two-Symbol instead of the Prime Implicant schemata.
-
-        .. math::
-
-            s_i = \frac{ \sum_{f_{\alpha} \in F} \Phi_{\theta:f_{\alpha} \in \Theta_{\theta}} (n^{\circ}_i)}{ |F| }
-
-        where :math:`\Phi` is the function :math:`min` or :math:`max` and :math:`F` is the node LUT.
+    def symKernel_numDots(self, ts, sameSymbol=False):
+        """compute the number of variables involved in a symmetry group.
 
         Args:
-            bound (string) : The bound to which compute input symmetry.
-                Mode "node" accepts: ["lower", "upper"].
-                Mode "input" accepts: ["lower", "mean", "upper", "tuple"].
-                Defaults to "upper".
+            ts ([str, [[]], [[]]]) : two symbol schema
+            sameSymbol (bool) : whether or not to consider same-symbol symmetry
 
         Returns:
-            (float/list) : The :math:`k_s` or a list of :math:`r_i`.
-
-        See also:
-            :func:`input_redundancy`, :func:`effective_connectivity`
+            (int)
         """
-        # Canalization can only occur when k>= 2
-        if self.k < 2:
-            return [0.0]
+        if not sameSymbol:
+            groups = ts[1]
+        else:
+            groups = ts[1] + ts[2]
+        return len(set(i for group in groups for i in group))
 
+    def _input_symmetry(self, aggOp, kernel):
         self._check_compute_canalization_variables(ts_coverage=True)
 
-        symmetries = []
-        # Generate a per input coverage
-        # ex: {0: {'11': [], '10': [], '00': [], '01': []}, 1: {'11': [], '10': [], '00': [], '01': []}}
-        # ts_input_coverage = { input : { binstate: [ idxs.count(input) for schema,reps,sms in tss for idxs in reps+sms ] for binstate,tss in self._ts_coverage.items() } for input in range(self.k) }
-        ts_input_coverage = {input: {binstate: [len(idxs) if input in idxs else 0 for schema, reps, sms in tss for idxs in reps + sms] for binstate, tss in self._ts_coverage.items()} for input in range(self.k)}
-
-        # Loop ever input node
-        for input, binstates in ts_input_coverage.items():
-            # {'numstate': [number-of-ts's for each match], '10': [0, 2] ...}
-            numstates = {binstate_to_statenum(binstate): permuts for binstate, permuts in binstates.items()}
-
-            # A triplet of (min, mean, max) values
-            if bound in ['lower', 'mean', 'upper']:
-                # Min, Mean or Max
-                if bound == 'upper':
-                    minmax = max
-                elif bound == 'mean':
-                    minmax = np.mean
-                elif bound == 'lower':
-                    minmax = min
-
-                s_i = sum(minmax(permuts) if len(permuts) else 0 for permuts in numstates.values()) / 2**self.k  # min(r_s)
-
-            elif bound == 'tuple':
-                # tuple (min,max) per input, per state
-                s_i = [(min(permuts), max(permuts)) if len(permuts) else (0, 0) for permuts in numstates.values()]  # (min,max)
-            else:
-                raise AttributeError('The bound you selected does not exist. Try "upper", "mean", "lower" or "tuple".')
-            symmetries.append(s_i)
-
-        return symmetries  # s_i
-
-    def input_symmetry(self, bound='upper', norm=True):
-        r"""The Input Symmetry is a measure of permutation redundancy.
-        Similar to the computation of Input Redundancy but using the Two-Symbol instead of the Prime Implicant schemata.
+        summand = []
+        for fAlpha, fTheta in self._ts_coverage.items():
+            summand.append(aggOp(list(map(kernel, fTheta))))
+        return np.mean(summand)
 
-        .. math::
-
-            k_s = \frac{ \sum_{f_{\alpha} \in F} \Phi_{\theta:f_{\alpha} \in \Theta_{\theta}} (n^{\circ}) }{ |F| }
-
-        where :math:`\Phi` is the function :math:`min` or :math:`max` and :math:`F` is the node LUT.
+    def input_symmetry(self, aggOp="mean", kernel="numDots", sameSymbol=False):
+        """compute the input symmetry (k_s) of the boolean node, with variations via the specified functions.
+        Convenience wrapper for lower-level function.
 
         Args:
-            bound (string) : The bound to which compute input symmetry.
-                Mode "node" accepts: ["lower", "upper"].
-                Mode "input" accepts: ["lower", "mean", "upper", "tuple"].
-                Defaults to "upper".
-            norm (bool) : Normalized between [0,1].
-                Use this value when comparing nodes with different input sizes. (Defaults to "True".)
-
-                :math:`k^{*}_s(x) = \frac{ k_s(x) }{ k(x) }`.
+            aggOp : the function aggregating over all two-symbol schemata that redescribe a LUT entry
+            kernel : the function to compute on a given two-symbol schema
 
         Returns:
-            (float/list) : The :math:`k_s` or a list of :math:`r_i`.
-
-        See also:
-            :func:`input_redundancy`, :func:`effective_connectivity`
+            (float) : the mean over all LUT entries of the aggOp applied to the kernel of all two-symbol schemata that redescribe the LUT entry
         """
-        # Canalization can only occur when k>= 2
-        if self.k < 2:
-            return 0.0
+        strToOp = {"mean": np.mean, "max": max, "min": min}
+        strToKern = {"numDots": self.symKernel_numDots}
 
-        self._check_compute_canalization_variables(ts_coverage=True)
+        def kernFunc(x):
+            return strToKern[kernel](x, sameSymbol=sameSymbol)
 
-        k_s = sum(self.edge_symmetry(bound=bound)) / self.k
+        return self._input_symmetry(strToOp[aggOp], kernFunc)
 
-        if (norm):
-            k_s = k_s / self.k
+    # refactor ks for speed, avg op only
+    def input_symmetry_mean(self):
+        """compute the input symmetry (k_s) of the boolean node.
+           Specifically, computes it using the avg operator for the summand.
+           Refactoring of input_symmetry for speed.
 
-        return k_s
+        Returns:
+            (float)
+        """
+        summand = 0
+        # fTheta = a list of TS
+        for fTheta in self._ts_coverage.values():
+            inner = 0
+            for ts in fTheta:
+                inner += sum(
+                    len(i) for i in ts[1]
+                )  # assumes that indicies will ever only be in at most 1 group
+            summand += inner / len(fTheta)
+        return summand / 2**self.k
 
     def look_up_table(self):
-        """ Returns the Look Up Table (LUT)
+        """Returns the Look Up Table (LUT)
 
         Returns:
             (pandas.DataFrame): the LUT
 
         Examples:
             >>> AND = BooleanNode.from_output_list([0,0,0,1])
             >>> AND.look_up_table()
 
         See also:
             :func:`schemata_look_up_table`
 
         """
         d = []
-        if ((self.k < 2) and (self.constant is False)):
+        if (self.k < 2) and (self.constant is False):
             k = 2
         else:
             k = self.k
 
         for statenum, output in zip(range(2**k), self.outputs):
             # Binary State, Transition
             d.append((statenum_to_binstate(statenum, base=self.k), output))
 
-        df = pd.DataFrame(d, columns=['In:', 'Out:'])
+        df = pd.DataFrame(d, columns=["In:", "Out:"])
 
         return df
 
-    def schemata_look_up_table(self, type='pi', pi_symbol='#', ts_symbol_list=["\u030A", "\u032F"]):
-        """ Returns the simplified schemata Look Up Table (LUT)
+    def schemata_look_up_table(
+        self, type="pi", pi_symbol="#", ts_symbol_list=["\u030A", "\u032F"]
+    ):
+        """Returns the simplified schemata Look Up Table (LUT)
 
         Args:
             type (string) : The type of schemata to return, either Prime Implicants ``pi`` or Two-Symbol ``ts``. Defaults to 'pi'.
             pi_symbol (str) : The Prime Implicant don't care symbol. Default is ``#``.
             ts_symbol_list (list) : A list containing Two Symbol permutable symbols. Default is ``["\u030A", "\u032F"]``.
 
         Returns:
@@ -418,297 +447,397 @@
             See the full list of `combining characters <https://en.wikipedia.org/wiki/Combining_character>`_ to use other symbols as the permutation symbol.
 
         See also:
             :func:`look_up_table`
         """
         r = []
         # Prime Implicant LUT
-        if type == 'pi':
+        if type == "pi":
             self._check_compute_canalization_variables(prime_implicants=True)
 
-            pi0s = self._prime_implicants.get('0', [])
-            pi1s = self._prime_implicants.get('1', [])
+            pi0s = self._prime_implicants.get("0", [])
+            pi1s = self._prime_implicants.get("1", [])
 
             for output, pi in zip([0, 1], [pi0s, pi1s]):
                 for schemata in pi:
                     r.append((schemata, output))
 
         # Two Symbol LUT
-        elif type == 'ts':
+        elif type == "ts":
             self._check_compute_canalization_variables(two_symbols=True)
 
             ts0s, ts1s = self._two_symbols
 
             for output, ts in zip([0, 1], [ts0s, ts1s]):
                 for i, (schemata, permutables, samesymbols) in enumerate(ts):
-                    string = ''
+                    string = ""
                     if len(permutables):
-                        string += '('
+                        string += "("
                         # Permutable
                         for j, permutable in enumerate(permutables):
                             #
                             ts_symbol_unicode = ts_symbol_list[j]
                             if j > 0:
-                                string += ' | '
-                            string += u''.join([x if (k not in permutable) else u'%s%s' % (x, ts_symbol_unicode) for k, x in enumerate(schemata, start=0)])
-                        string += ')'
+                                string += " | "
+                            string += "".join(
+                                [
+                                    x
+                                    if (k not in permutable)
+                                    else "%s%s" % (x, ts_symbol_unicode)
+                                    for k, x in enumerate(schemata, start=0)
+                                ]
+                            )
+                        string += ")"
 
                     else:
-                        string += '(' + schemata + ')'
+                        string += "(" + schemata + ")"
 
                     if len(samesymbols):
-                        string += ' | ('
+                        string += " | ("
                         # Same Symbol
                         for j, samesymbol in enumerate(samesymbols):
                             ts_symbol_unicode = ts_symbol_list[j]
                             if j > 0:
-                                string += ' | '
-                            string += ''.join([x if (k not in samesymbol) else u'%s%s' % (x, ts_symbol_unicode) for k, x in enumerate(schemata, start=0)])
-                        string += ')'
+                                string += " | "
+                            string += "".join(
+                                [
+                                    x
+                                    if (k not in samesymbol)
+                                    else "%s%s" % (x, ts_symbol_unicode)
+                                    for k, x in enumerate(schemata, start=0)
+                                ]
+                            )
+                        string += ")"
                     r.append((string, output))
         else:
-            raise AttributeError('The schemata type could not be found. Try "PI" (Prime Implicants) or "TS" (Two-Symbol).')
+            raise AttributeError(
+                'The schemata type could not be found. Try "PI" (Prime Implicants) or "TS" (Two-Symbol).'
+            )
 
-        r = [(schemata.replace('2', pi_symbol), output) for schemata, output in r]
-        return pd.DataFrame(r, columns=['Input', 'Output'])
+        r = [(schemata.replace("2", pi_symbol), output) for schemata, output in r]
+        return pd.DataFrame(r, columns=["Input", "Output"])
 
     def input_mask(self, binstate):
-        """ Returns the mask applied to the binary state binstate
+        """Returns the mask applied to the binary state binstate
 
         Args:
             binstate (str) : the binary state
 
         Returns:
             output (str) : the masked state
         """
-        return ''.join(compress(binstate, self.mask))
+        return "".join(compress(binstate, self.mask))
 
     def activities(self):
+        """compute the activities of each incoming edge of the node
+        Returns:
+            (list of floats)
+        """
         return self.edge_effectiveness(bound="upper")
 
     def sensitivity(self, norm=False):
+        """compute the sensitivity of the node. Does so by summing the activities of the edges
+        Args:
+            norm (bool) : whether or not to normalize by the number of inputs (k)
+        Returns:
+            (float)
+        """
         x = sum(self.activities())
         if norm:
             return x / self.k
         else:
             return x
 
     def canalizing_map(self, output=None):
-        """ Computes the node Canalizing Map (CM).
+        """Computes the node Canalizing Map (CM).
 
         Args:
             output (int) : The output CM to return. Default is ``None``, retuning both [0,1].
 
         Returns:
             CM (networkx.DiGraph) : a directed graph representation of the CM.
 
         See Also:
             :func:`boolean_network.dynamics_canalization_map` for the DCM and :func:`drawing.draw_canalizing_map_graphviz` for plotting.
         """
         self._check_compute_canalization_variables(two_symbols=True)
 
         ts0s, ts1s = self._two_symbols
 
-        G = nx.DiGraph(name='CM: %s' % self.name)
+        G = nx.DiGraph(name="CM: %s" % self.name)
 
         # Outputs
         if output is None or output == 0:
-            G.add_node('var-{nid:d}-out-0'.format(nid=self.id), **{'label': self.name, 'type': 'variable', 'mode': 'output', 'value': 0, 'constant': self.constant, 'group': self.id})
+            G.add_node(
+                "var-{nid:d}-out-0".format(nid=self.id),
+                **{
+                    "label": self.name,
+                    "type": "variable",
+                    "mode": "output",
+                    "value": 0,
+                    "constant": self.constant,
+                    "group": self.id,
+                }
+            )
 
         if output is None or output == 1:
-            G.add_node('var-{nid:d}-out-1'.format(nid=self.id), **{'label': self.name, 'type': 'variable', 'mode': 'output', 'value': 1, 'constant': self.constant, 'group': self.id})
+            G.add_node(
+                "var-{nid:d}-out-1".format(nid=self.id),
+                **{
+                    "label": self.name,
+                    "type": "variable",
+                    "mode": "output",
+                    "value": 1,
+                    "constant": self.constant,
+                    "group": self.id,
+                }
+            )
 
         tid = 0
         for out, tspsss in zip([0, 1], self._two_symbols):
-
             # Only return the requested output
-            if ((not len(tspsss)) or ((output is not None) and (output != out))):
+            if (not len(tspsss)) or ((output is not None) and (output != out)):
                 continue
 
             for ts, ps, ss in tspsss:
-
                 lits = []
                 group0 = []
                 group1 = []
                 # group2 = []
                 # Tau is the threshold, counted as the sum of (0's and 1's literals; 0's in permutation group; 1's in permutation group)
                 nlit, ngrp0, ngrp1 = 0, 0, 0
 
                 for j in range(self.k):
                     # Is this input in any permutation group?
                     input = ts[j]
                     if not any([j in group for group in ps]):
-                        if ts[j] in ['0', '1']:
+                        if ts[j] in ["0", "1"]:
                             nlit += 1
                             source = j
                             lits.append(source)
                     else:
-                        if ts[j] == '0':
+                        if ts[j] == "0":
                             ngrp0 += 1
                             group0.append(j)
-                        elif ts[j] == '1':
+                        elif ts[j] == "1":
                             ngrp1 += 1
                             group1.append(j)
 
                 tau = nlit + ngrp0 + ngrp1
 
                 # Threshold Node
-                tname = 'thr-{tid:d}-var-{nid:d}-out-{out:d}'.format(tid=tid, nid=self.id, out=out)
+                tname = "thr-{tid:d}-var-{nid:d}-out-{out:d}".format(
+                    tid=tid, nid=self.id, out=out
+                )
                 label = "{:d}".format(tau)
-                G.add_node(tname, **{'label': label, 'type': 'threshold', 'tau': tau, 'group': self.id})
+                G.add_node(
+                    tname,
+                    **{
+                        "label": label,
+                        "type": "threshold",
+                        "tau": tau,
+                        "group": self.id,
+                    }
+                )
 
                 # Add Edges from Threshold node to output
-                xname = 'var-{nid:d}-out-{out:d}'.format(nid=self.id, out=out)
+                xname = "var-{nid:d}-out-{out:d}".format(nid=self.id, out=out)
                 if G.has_node(tname) and G.has_node(xname):
-                    G.add_edge(tname, xname, **{'type': 'out'})
+                    G.add_edge(tname, xname, **{"type": "out"})
                 else:
                     raise BaseException("Adding edge to node that does not exist.")
 
                 # Literal Edges
                 for lit in lits:
-                    iname = 'var-{nid:d}-out-{out:d}'.format(nid=self.inputs[lit], out=int(ts[lit]))
+                    iname = "var-{nid:d}-out-{out:d}".format(
+                        nid=self.inputs[lit], out=int(ts[lit])
+                    )
                     if iname not in G.nodes():
                         # Can we get the name of ther nodes? Are we attached to a network?
                         if self.network is not None:
                             ilabel = self.network.get_node_name(self.inputs[lit])[0]
                         else:
                             ilabel = str(self.inputs[lit])
                         iout = int(ts[lit])
-                        G.add_node(iname, **{'label': ilabel, 'type': 'variable', 'mode': 'input', 'value': iout, 'group': self.id})
-                    G.add_edge(iname, tname, **{'type': 'literal'})
+                        G.add_node(
+                            iname,
+                            **{
+                                "label": ilabel,
+                                "type": "variable",
+                                "mode": "input",
+                                "value": iout,
+                                "group": self.id,
+                            }
+                        )
+                    G.add_edge(iname, tname, **{"type": "literal"})
 
                 # Group0
                 for fusion in range(ngrp0):
-                    fname = 'fus-{fus:d}-thr-{thr:d}-var-{nid:d}-out-{out:d}'.format(fus=fusion, thr=tid, nid=self.id, out=0)
-                    G.add_node(fname, **{'type': 'fusion', 'group': self.id})
+                    fname = "fus-{fus:d}-thr-{thr:d}-var-{nid:d}-out-{out:d}".format(
+                        fus=fusion, thr=tid, nid=self.id, out=0
+                    )
+                    G.add_node(fname, **{"type": "fusion", "group": self.id})
                     for input in ps[0]:
-                        iname = 'var-{nid:d}-out-{out:d}'.format(nid=self.inputs[input], out=0)
+                        iname = "var-{nid:d}-out-{out:d}".format(
+                            nid=self.inputs[input], out=0
+                        )
                         if iname not in G.nodes():
                             # Can we get the name of ther nodes? Are we attached to a network?
                             if self.network is not None:
-                                ilabel = self.network.get_node_name(self.inputs[input])[0]
+                                ilabel = self.network.get_node_name(self.inputs[input])[
+                                    0
+                                ]
                             else:
                                 ilabel = str(self.inputs[input])
-                            G.add_node(iname, **{'label': ilabel, 'type': 'variable', 'mode': 'input', 'value': 0, 'group': self.id})
-                        G.add_edge(iname, fname, **{'type': 'fusing'})
-                    G.add_edge(fname, tname, **{'type': 'fused'})
+                            G.add_node(
+                                iname,
+                                **{
+                                    "label": ilabel,
+                                    "type": "variable",
+                                    "mode": "input",
+                                    "value": 0,
+                                    "group": self.id,
+                                }
+                            )
+                        G.add_edge(iname, fname, **{"type": "fusing"})
+                    G.add_edge(fname, tname, **{"type": "fused"})
 
                 # Group1
                 for fusion in range(ngrp1):
-                    fname = 'fus-{fus:d}-thr-{thr:d}-var-{nid:d}-out-{out:d}'.format(fus=fusion, thr=tid, nid=self.id, out=1)
-                    G.add_node(fname, **{'type': 'fusion', 'group': self.id})
+                    fname = "fus-{fus:d}-thr-{thr:d}-var-{nid:d}-out-{out:d}".format(
+                        fus=fusion, thr=tid, nid=self.id, out=1
+                    )
+                    G.add_node(fname, **{"type": "fusion", "group": self.id})
                     for input in ps[0]:
-                        iname = 'var-{var:d}-out-{out:d}'.format(var=self.inputs[input], out=1)
+                        iname = "var-{var:d}-out-{out:d}".format(
+                            var=self.inputs[input], out=1
+                        )
                         if iname not in G.nodes():
                             # Can we get the name of ther nodes? Are we attached to a network?
                             if self.network is not None:
-                                ilabel = self.network.get_node_name(self.inputs[input])[0]
+                                ilabel = self.network.get_node_name(self.inputs[input])[
+                                    0
+                                ]
                             else:
                                 ilabel = str(self.inputs[input])
                             iout = ts[input]
-                            G.add_node(iname, **{'label': ilabel, 'type': 'variable', 'mode': 'input', 'value': 1, 'group': self.id})
-                        G.add_edge(iname, fname, **{'type': 'fusing'})
-                    G.add_edge(fname, tname, **{'type': 'fused'})
+                            G.add_node(
+                                iname,
+                                **{
+                                    "label": ilabel,
+                                    "type": "variable",
+                                    "mode": "input",
+                                    "value": 1,
+                                    "group": self.id,
+                                }
+                            )
+                        G.add_edge(iname, fname, **{"type": "fusing"})
+                    G.add_edge(fname, tname, **{"type": "fused"})
 
                 tid += 1
 
         return G
 
     def pi_coverage(self):
-        """ Returns the :math:`F'` (Prime Implicants) binary state coverage.
+        """Returns the :math:`F'` (Prime Implicants) binary state coverage.
 
         Returns:
             (list)
 
         See also:
             :func:`ts_coverage`
         """
         self._check_compute_canalization_variables(pi_coverage=True)
         return self._pi_coverage
 
     def ts_coverage(self):
-        """ Returns the :math:`F''` (Two-Symbol schematas) binary state coverage.
+        """Returns the :math:`F''` (Two-Symbol schematas) binary state coverage.
 
         Returns:
             (list)
 
         See also:
             :func:`pi_coverage`
         """
         self._check_compute_canalization_variables(ts_coverage=True)
         return self._ts_coverage
 
     def _check_compute_canalization_variables(self, **kwargs):
-        """ Recursevely check if the requested canalization variables are instantiated/computed, otherwise computes them in order.
+        """Recursevely check if the requested canalization variables are instantiated/computed, otherwise computes them in order.
         For example: to compute `two_symbols` we need `prime_implicants` first.
         Likewise, to compute `prime_implicants` we need the `transition_density_table` first.
         """
-        if 'prime_implicants' in kwargs:
+        if "prime_implicants" in kwargs:
             if self._prime_implicants is None:
                 self._prime_implicants = dict()
                 for output in set(self.outputs):
-                    output_binstates = outputs_to_binstates_of_given_type(self.outputs, output=output, k=self.k)
-                    self._prime_implicants[output] = cBCanalization.find_implicants_qm(input_binstates=output_binstates)
+                    output_binstates = outputs_to_binstates_of_given_type(
+                        self.outputs, output=output, k=self.k
+                    )
+                    self._prime_implicants[output] = cBCanalization.find_implicants_qm(
+                        input_binstates=output_binstates
+                    )
 
-        elif 'pi_coverage' in kwargs:
+        elif "pi_coverage" in kwargs:
             self._check_compute_canalization_variables(prime_implicants=True)
             if self._pi_coverage is None:
                 self._pi_coverage = dict()
                 for output, piset in self._prime_implicants.items():
                     self._pi_coverage.update(cBCanalization.return_pi_coverage(piset))
 
                 # make sure every inputstate was covered by at least one prime implicant
                 assert len(self._pi_coverage) == 2**self.k
 
-        elif 'two_symbols' in kwargs:
+        elif "two_symbols" in kwargs:
             self._check_compute_canalization_variables(prime_implicants=True)
             if self._two_symbols is None:
                 # this is a temporary fix until we update 'find_two_symbols' to cython.
-                if '0' in self._prime_implicants:
-                    pi0 = self._prime_implicants['0']
-                    pi0 = set([pi.replace('#', '2') for pi in pi0])
+                if "0" in self._prime_implicants:
+                    pi0 = self._prime_implicants["0"]
+                    pi0 = set([pi.replace("#", "2") for pi in pi0])
                 else:
                     pi0 = []
-                if '1' in self._prime_implicants:
-                    pi1 = self._prime_implicants['1']
-                    pi1 = set([pi.replace('#', '2') for pi in pi1])
+                if "1" in self._prime_implicants:
+                    pi1 = self._prime_implicants["1"]
+                    pi1 = set([pi.replace("#", "2") for pi in pi1])
                 else:
                     pi1 = []
                 # /end fix
-                self._two_symbols = \
-                    (
-                        BCanalization.find_two_symbols_v2(k=self.k, prime_implicants=pi0),
-                        BCanalization.find_two_symbols_v2(k=self.k, prime_implicants=pi1)
-                    )
-        elif 'ts_coverage' in kwargs:
+                self._two_symbols = (
+                    BCanalization.find_two_symbols_v2(k=self.k, prime_implicants=pi0),
+                    BCanalization.find_two_symbols_v2(k=self.k, prime_implicants=pi1),
+                )
+        elif "ts_coverage" in kwargs:
             self._check_compute_canalization_variables(two_symbols=True)
             if self._ts_coverage is None:
-                self._ts_coverage = BCanalization.computes_ts_coverage(self.k, self.outputs, self._two_symbols)
+                self._ts_coverage = BCanalization.computes_ts_coverage(
+                    self.k, self.outputs, self._two_symbols
+                )
 
         else:
-            raise Exception('Canalization variable name not found. %s' % kwargs)
+            raise Exception("Canalization variable name not found. %s" % kwargs)
         return True
 
     def bias(self):
-        r""" The node bias. The sum of the boolean output transitions divided by the number of entries (:math:`2^k`) in the LUT.
+        r"""The node bias. The sum of the boolean output transitions divided by the number of entries (:math:`2^k`) in the LUT.
 
         .. math::
 
             bias(x) = \frac{ \sum_{f_{\alpha}\in F} s_{\alpha} }{ |F| }
 
         Returns:
             (float)
 
         See Also:
             :func:`~cana.boolean_network.BooleanNetwork.network_bias`
         """
         return sum(map(int, self.outputs)) / 2**self.k
 
     def c_sensitivity(self, c, mode="default", max_k=0):
-        """ Node c-sensitivity.
+        """Node c-sensitivity.
         c-sensitivity is defined as: the mean probability that changing exactly
         ``c`` variables in input variables would change output value.
         There is another mode "forceK", which will be used to calculate Derrida value.
         In that mode, it would assume the number of input variables is specified as max_k
         this methods is equivalent to Derrida value in :cite:`Kadelka:2017`, only move a normalization
         coefficient from expression of Derrida value to c-sensitivity to simplify it
 
@@ -722,39 +851,42 @@
 
         See Also:
             :func:`~cana.boolean_network.derrida_curve`
         """
         S_c_f = 0
         ic = min(c, self.k)
 
-        if mode != 'forceK':
-            for j in product('01', repeat=self.k):
+        if mode != "forceK":
+            for j in product("01", repeat=self.k):
                 origin_config = list(j)
                 for mut in combinations(range(self.k), ic):
                     mut_config = origin_config[:]
                     for i_mut in mut:
                         mut_config[i_mut] = flip_bit(mut_config[i_mut])
-                    if self.step(''.join(origin_config)) != self.step(''.join(mut_config)):
+                    if self.step("".join(origin_config)) != self.step(
+                        "".join(mut_config)
+                    ):
                         S_c_f += 1
             if S_c_f == 0:
-                return 0.
-            return S_c_f / float(ncr(self.k, c)) / float(2 ** self.k)
+                return 0.0
+            return S_c_f / float(ncr(self.k, c)) / float(2**self.k)
         else:
             assert max_k >= self.k
             for ic in range(max(1, c + self.k - max_k), min(c, self.k) + 1):
-                for j in product('01', repeat=self.k):
+                for j in product("01", repeat=self.k):
                     origin_config = list(j)
                     for mut in combinations(range(self.k), ic):
                         mut_config = origin_config[:]
                         for i_mut in mut:
                             mut_config[i_mut] = flip_bit(mut_config[i_mut])
-                        if self.step(''.join(origin_config)) != self.step(
-                                ''.join(mut_config)):
+                        if self.step("".join(origin_config)) != self.step(
+                            "".join(mut_config)
+                        ):
                             S_c_f += ncr(max_k - self.k, c - ic)
-            return S_c_f / float(ncr(max_k, c)) / float(2 ** self.k)
+            return S_c_f / float(ncr(max_k, c)) / float(2**self.k)
 
     def input_signs(self):
         """
         Determine if a each input can be considered activation (1), inhibition (-1), or neither (0).
 
         Here we test every pair of inputs that are Hamming distance 1. (see Goldreich et al 2000)
 
@@ -762,14 +894,22 @@
             (list) : The list of input signs.
 
         Example:
             >>> is_monotone(outputs=[0,0,0,1])
         """
 
         # first test if the inputs are activation inputs (more common in bio networks)
-        input_sign_list = [int(input_monotone(self.outputs, idx, activation=1)) for idx in range(self.k)]
+        input_sign_list = [
+            int(input_monotone(self.outputs, idx, activation=1))
+            for idx in range(self.k)
+        ]
 
         # for those inputs that are not activation inputs (more common in bio networks),
         # then test for inhibition
-        input_sign_list = [-1*int(input_monotone(self.outputs, idx, activation=-1)) if sign==0 else sign for idx, sign in enumerate(input_sign_list)]
+        input_sign_list = [
+            -1 * int(input_monotone(self.outputs, idx, activation=-1))
+            if sign == 0
+            else sign
+            for idx, sign in enumerate(input_sign_list)
+        ]
 
         return input_sign_list
```

### Comparing `cana-0.2.0/cana/canalization/boolean_canalization.py` & `cana-1.0.0/cana/canalization/boolean_canalization.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,45 +9,50 @@
 #   Copyright (C) 2021 by
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Alex Gates <ajgates@gmail.com>
 #   Etienne Nzabarushimana <enzabaru@indiana.edu>
 #   All rights reserved.
 #   MIT license.
 
-import numpy as np
-
 import itertools
-from .. utils import *
-
 from collections import deque
 
-__author__ = """\n""".join([
-    'Alex Gates <ajgates@umail.iu.edu>',
-    'Etienne Nzabarushimana <enzabaru@indiana.edu>',
-    'Rion Brattig Correia <rionbr@gmail.com>'
-])
+import numpy as np
+import schematodes as sc
+
+from ..cutils import binstate_to_density, statenum_to_binstate
+
+__author__ = """\n""".join(
+    [
+        "Alex Gates <ajgates@umail.iu.edu>",
+        "Etienne Nzabarushimana <enzabaru@indiana.edu>",
+        "Rion Brattig Correia <rionbr@gmail.com>",
+    ]
+)
 
 
 # Quine-McCluskey Functions
 def make_transition_density_tables(k=1, outputs=[0, 1]):
-    """ This method creates a tuple-of-lists that is used to calculate Prime Implicants in the first step of the Quine-McCluskey algorithm :cite:`Quine:1955`.
+    """This method creates a tuple-of-lists that is used to calculate Prime Implicants in the first step of the Quine-McCluskey algorithm :cite:`Quine:1955`.
     In practice it separates the positive and negative transitions (tuple), then further separates it by counting the number of 1's in each (lists).
 
     Args:
         k (int) : the ``k`` number of inputs
         outputs (list) : a list of ``[0,1]`` output for each state number.
 
     Returns:
         tables (tuple) : a tuple where [0] is the negative table and [1] is the positive table.
     """
     # make sure outputs are integers
     outputs = list(map(int, outputs))
 
     # we need to split up the LUT based on the transition (to either 0 or 1) and the density of 1s in the binstate
-    transition_density_tuple = [[[] for density in range(k + 1)] for transition in [0, 1]]
+    transition_density_tuple = [
+        [[] for density in range(k + 1)] for transition in [0, 1]
+    ]
     for statenum in range(2**k):
         binstate = statenum_to_binstate(statenum, base=k)
         density = binstate_to_density(binstate)
         transition = outputs[statenum]
         # Account for Dont-Care (2) transition states
         if transition == 2:
             transition_density_tuple[0][density].append(binstate)
@@ -55,15 +60,15 @@
         else:
             transition_density_tuple[transition][density].append(binstate)
     #
     return transition_density_tuple
 
 
 def find_implicants_qmOLD(column, verbose=False):
-    """ Finds the prime implicants (PI) using the Quine-McCluskey algorithm :cite:`Quine:1955`.
+    """Finds the prime implicants (PI) using the Quine-McCluskey algorithm :cite:`Quine:1955`.
 
     Args:
         column (list) : A list-of-lists containing the counts of ``1`` for each input.
             This is given by `make_transition_density_tables`.
 
     Returns:
         PI (set): a set of prime implicants.
@@ -79,28 +84,28 @@
 
     # repeat the following until no matches are found
     while not done:
         done = True
 
         # default everything to empty with no matches
         next_column = [set() for _ in range(N + 1)]
-        matches = [[False for _ in range(len(column[density]))] for density in range(N + 1)]
+        matches = [
+            [False for _ in range(len(column[density]))] for density in range(N + 1)
+        ]
 
         # loop through the possible densities
         for density in range(N):
-
             # compare the implicants from successive densities
             for i, implicant in enumerate(column[density]):
                 for j, candidate in enumerate(column[density + 1]):
-
                     # check if the implicants differ on only one variable
                     match = _adjacent(implicant, candidate)
                     if match:
                         matches[density][i] = matches[density + 1][j] = True
-                        matches_density = sum([var != '0' for var in match])
+                        matches_density = sum([var != "0" for var in match])
                         next_column[matches_density].add(match)
                         done = False
 
         # now add back the implicants that were not matched
         for i in range(N + 1):
             for j in range(len(matches[i])):
                 if not matches[i][j]:
@@ -127,19 +132,19 @@
     for m1, m2 in zip(imp1, imp2):
         if m1 == m2:
             match.append(m1)
         elif differences:
             return False
         else:
             differences += 1
-            match.append('2')
+            match.append("2")
     return "".join(match)
 
 
-def __pi_covers(implicant, input, symbol=['2', '#', 2]):
+def __pi_covers(implicant, input, symbol=["2", "#", 2]):
     """Determines if a minterm is covered by a specific implicant.
 
     Args:
         implicant (string): the implicant.
         minterm (string): the minterm.
 
     Returns:
@@ -200,224 +205,77 @@
         prime_implicants (list): The prime implicants computed.
 
     Returns:
         final_list (list) : The list of two-symbol schematas.
 
     Note: This is a modification of the original algorithm that can be found in Marques-Pita & Rocha [2013].
     """
-    if not len(prime_implicants):
+    if verbose or verbose_level > 0:
+        print("Finding TS schematas...")
+
+    if not prime_implicants:
         return []
 
     # If this node has no input, yet it affects other nodes (fixed variable)
     if k == 0:
         TSf = []
         for pi in prime_implicants:
             TSf.append((pi, [], []))
         return TSf
 
-    # Init
-    # n_pi = len(prime_implicants) # never used
-    pi_matrix = np.array(tuple(map(tuple, prime_implicants)), dtype=int)
-
-    # List of the Two-Symbol Schematas
-    TS = []
-
-    # Init Queue
-    Q = deque()
-    Q_history = set()
-    Q.append(pi_matrix)
-    i = 0
-
-    while len(Q):
-
-        schematas = Q.popleft()
-        n_schematas = schematas.shape[0]
-        i += 1
-
-        # count the number of [0's, 1's, 2's] in each column
-        column_counts = _count_cols_symbols(pi_matrix=schematas, verbose=verbose, verbose_level=verbose_level)
-
-        # find the possible permutation groups based on column counts
-        perm_groups = _check_col_counts(counts_matrix=column_counts, verbose=verbose, verbose_level=verbose_level)
-
-        if (perm_groups != -1): # if there are some possible permutation groups
-            for x_group in perm_groups:
-                # find the row counts by taking the transpose of the truncated schemata list
-                row_counts = _count_cols_symbols(pi_matrix=schematas[:, x_group].T, verbose=verbose, verbose_level=verbose_level)
-                # make sure all row counts are the same
-                if not (row_counts == row_counts[0]).all():
-                    perm_groups = -1 # permutation groups won't work
-
-        # cond1 = permutation groups are still possible AND schemata subset not yet added to output
-        cond1 = (perm_groups != -1) and not ((schematas.tolist(), perm_groups) in TS)
-        # cond2 = True if a valid permutation group was found
-        cond2 = False
-        if cond1:
-            # NOTE: it is possible for row and col counts to be the same but the schema should be split into 2 group-invariant symbols
-            # if none of the given perm groups work on a given schema, it will start looking at subsets of the schema
-            # but it should also try all partitions of each element in the perm group list because there may be 2 disjoint symmetries within the same schema with all identical row & col counts
-
-            # actually test if columns can be permuted arbitrarily in schemata subset
-            allowed_perm_groups = _check_schemata_permutations(schematas, perm_groups, verbose=verbose, verbose_level=verbose_level)
-            if allowed_perm_groups is not None:
-                TS.append((schematas.tolist(), allowed_perm_groups))
-                cond2 = True
-
-        # NOTE: possible that cond1 is true, but cond2 is false. The previous logic would then not parition the schema further
-        # add all subsets of of schemata of size one less than before to queue
-        if not cond1 or not cond2: # no valid perm groups were found
-            if schematas.shape[0] > 2:
-                for idxs_subset in itertools.combinations(np.arange(0, n_schematas), (n_schematas - 1)):
-                    idxs_subset = list(idxs_subset)
-                    schemata_subset = schematas[idxs_subset, :]
-                    # This schemata has already been inserted onto the Queue before?
-                    if schemata_subset.tostring() not in Q_history:
-                        Q.append(schemata_subset)
-                        Q_history.add(schemata_subset.tostring())
-    
-
-    if verbose:
-        print('>>> TWO-SYMBOLS:')
-        for i, (tss, perms) in enumerate(TS):
-            print("F''-%d: %s | Perms: %s" % (i, tss, perms))
-
-    # Simplification. Check if there are TSs that are completely contained within others.
-    # 'ts' = Two-Symbol
-    # 'cx' = Complexity
-    # 'xs' = Expanded Logic
-    TSs = {
-        i: {
-            'tss': tss,
-            'perms': perms,
-            'cx': _calc_ts_complexity(tss, perms),
-            'xl': _expand_ts_logic(tss, perms)
-        } for i, (tss, perms) in enumerate(TS)
-    }
-
-    # Loops all combinations (2) of TS
-    for (i, j) in itertools.combinations(TSs.keys(), 2):
-        try:
-            a_in_b, b_in_a = _check_schema_within_schema(TSs[i]['xl'], TSs[j]['xl'])
-        except:
-            continue
-        else:
-            cx_a = TSs[i]['cx']
-            cx_b = TSs[j]['cx']
-            # A or B contained in the other, keep only contained.
-            if a_in_b and not b_in_a:
-                del TSs[i]
-            elif b_in_a and not a_in_b:
-                del TSs[j]
-            elif a_in_b and b_in_a:
-                # Keep most complex
-                if cx_a < cx_b:
-                    del TSs[i]
-                elif cx_b < cx_a:
-                    del TSs[j]
-                else:
-                    # they are equal, delete either one
-                    del TSs[i]
-
-    if verbose:
-        print('>>> TWO-SYMBOLS (simplified):')
-        for i, (tss) in TSs.items():
-            print("F''-%d: %s | Perms: %s | CX: %s" % (i, tss['tss'], tss['perms'], tss['cx']))
-
-    # Final List (from simplified)
-    TSf = [(tss['tss'][0], tss['perms'], []) for tss in TSs.values()]
-
-    # Check if all PI are being covered. If not, include the PI on the TS list
-    if verbose:
-        print('>>> Check all PI are accounted for in the TS')
-    for i, pi in enumerate(pi_matrix, start=0):
-        if not any([_check_schema_within_schema([pi.tolist()], tss['xl'], dir='a', verbose=verbose)[0] for tss in TSs.values()]):
-            if verbose:
-                print("PI-%d '%s' Not in list, ADDING." % (i, pi.tolist()))
-            TSf.append((pi.tolist(), [], []))
-        else:
-            if verbose:
-                print("PI-%d '%s' OK." % (i, pi.tolist()))
-
-    if verbose:
-        print('>>> Check for Same-Symbol permutables')
-
-    # NEW: Step to include same-symbol permutables
-    for ts, perms, sames in TSf:
-        # Indices of permutables inputs
-        idxs = list(set([idx for idxs in perms for idx in idxs]))
-
-        # Makes the F'' into a Collum Array so it can be used by '_count_cols_symbols_vX'
-        ts_matrix = np.array([ts]).T
-
-        # Remove Inputs (columns) that already have permutable symbols. Only if there are permutables
-        if len(idxs):
-            rmask = np.array(idxs)
-            ts_matrix_left = ts_matrix[~rmask, :]
-        else:
-            ts_matrix_left = ts_matrix
-
-        if verbose and verbose_level > 10:
-            print("> F'' Original:")
-            print(ts_matrix)
-            print("> Permutables: %s" % (perms))
-            print("> F'' without permutables:")
-            print(ts_matrix_left)
-
-        counts_matrix = _count_cols_symbols(pi_matrix=ts_matrix_left.T, verbose=False, verbose_level=verbose_level)
-        perm_groups = _check_identical_cols_count_symbols_v2(counts_matrix=counts_matrix, verbose=verbose, verbose_level=verbose_level)
-        sames.extend(perm_groups)
-
-    # Step to convert the pi list to string
-    for i, (ts, perms, sames) in enumerate(TSf, start=0):
-        ts = ''.join(map(str, ts))
-        TSf[i] = (ts, perms, sames)
-
-    # Final list after all PI were accounted for
-    if verbose:
-        print('>>> TS (final list):')
-        for i, tss, sms in TSf:
-            print("TS: '%s' | Perm Idx: %s | Sms Idx: %s" % (i, tss, sms))
-
+    prime_implicants = [[int(c) for c in pi] for pi in prime_implicants]
+    tss = sc.schemer(prime_implicants, max_symbol=2)
+    TSf = []  # collect the two-symbol schemata and calculate the one-symbol symmetries
+    for c in tss:
+        representative = c.redescribed_schemata[0]
+        bubble_indices = c.bubble_indices
+        same_symbols_all = [
+            [i for i, _ in enumerate(representative) if representative[i] == x]
+            for x in [0, 1, 2]
+        ]
+        same_symbols = [x for x in same_symbols_all if len(x) > 1]
+        representative_str = "".join(map(str, representative))
+        TSf.append([representative_str, bubble_indices, same_symbols])
     return TSf
 
 
 def _calc_ts_complexity(tss, pers):
-    """ Calculates the complexity of a TS schema
+    """Calculates the complexity of a TS schema
     Complexity = (Number of Schemas + Number of Permutable Symbols + Lenght of each Permutable Symbol)
     """
     return len(tss) + sum([len(per) for ts, per in zip(tss, pers)])
 
 
 def _check_schema_within_schema(la, lb, dir=None, verbose=False):
-    """ Check is a Two-Symbol schemata is covered by another.
+    """Check is a Two-Symbol schemata is covered by another.
     This is used to simplify the number of TS schematas returned.
     The arguments for this function are generated by `_expand_ts_logic`.
 
     Args:
         tsa (list) : A list of :math:`F'` schematas that a Two-Symbol :math:`F''` schemata can cover.
         tsb (list) : A list of :math:`F'` schematas that a Two-Symbol :math:`F''` schemata can cover.
         dir (string) : The direction to check, either ``a`` or ``b`` is in the other.
             Defaults to both directions.
     """
     a_in_b, b_in_a = None, None
     #
-    if dir != 'b':
+    if dir != "b":
         a_in_b = all([(xa in lb) for xa in la])
         if verbose:
-            print('%s in %s : %s' % (la, lb, a_in_b))
-    if dir != 'a':
+            print("%s in %s : %s" % (la, lb, a_in_b))
+    if dir != "a":
         b_in_a = all([(xb in la) for xb in lb])
         if verbose:
-            print('%s in %s : %s' % (lb, la, b_in_a))
+            print("%s in %s : %s" % (lb, la, b_in_a))
     #
     return a_in_b, b_in_a
 
 
 def _expand_ts_logic(two_symbols, permut_indexes):
-    """ Expands the Two-Symbol logic to all possible prime-implicants variations being covered.
+    """Expands the Two-Symbol logic to all possible prime-implicants variations being covered.
 
     Args:
         two_symbols (list) : Two-Symbol schematas list-of-lists.
 
     Returns:
         (list) : a list of :math:`F'` covered by this Two-Symbol.
     """
@@ -431,60 +289,65 @@
     #
     while Q:
         implicant = np.array(Q.pop())
         for idxs in permut_indexes:
             # Permutation of all possible combinations of the values that are permutable.
             for vals in itertools.permutations(implicant[idxs], len(idxs)):
                 # Generate a new schema
-                _implicant = copy.copy(implicant)
+                _implicant = np.copy(implicant)
                 _implicant[idxs] = vals
                 # Insert to list of logics if not already there
-                if not(_implicant.tolist() in logics):
+                if not (_implicant.tolist() in logics):
                     logics.append(_implicant.tolist())
                     Q.append(_implicant.tolist())
     return logics
 
+
 def _check_schemata_permutations(schema, perm_groups, verbose=None, verbose_level=None):
     """
-        schematas = matrix
-        perm_groups = lists
+    schematas = matrix
+    perm_groups = lists
     """
+    if verbose or verbose_level > 0:
+        print("Verifying schemata permutations...")
     # check that all pairs specified in perm_group are still valid
     allowed_perm_groups = []
     for perm_group in perm_groups:
         for i, x in enumerate(perm_group):
             for j in range(i, len(perm_group)):
                 y = perm_group[j]
                 if not _can_swap_v3(schema, x, y):
                     return None
         allowed_perm_groups.append(perm_group)
     return allowed_perm_groups
 
+
 def _can_swap_v3(schema, i, j):
     swapped = schema.copy()
     swapped[:, [i, j]] = schema[:, [j, i]]
     for row in swapped:
         if not np.any(np.all(schema == row, axis=1)):
             return False
     return True
 
+
 def _check_col_counts(counts_matrix, verbose=False, verbose_level=0):
-    """ This function is used to find permutable symbols.
+    """This function is used to find permutable symbols.
 
     Args:
         counts_matrix (numpy.ndarray) : a matrix where rows are inputs and columns are possible input types (0,1 or #)
 
     Returns:
         perm_groups (list) : a list of the indexes that can be permuted.
     """
     if verbose and verbose_level > 30:
-        print('-- Check Col Counts (v3) --')
+        print("-- Check Col Counts (v3) --")
 
-    counts = {}         # Multi Counts
-    perm_groups = []    # A list of groups of Permutable Indexes
+    counts = {}  # Multi Counts
+    perm_groups = []  # A list of groups of Permutable Indexes
 
     for i, row in enumerate(counts_matrix, start=0):
         # a tuple (hashable) version of the row counts
         row_tuple = tuple(row)
 
         if row_tuple in counts:
             # we have seen this one before, so add it to the permutation group
@@ -495,113 +358,118 @@
         else:
             # we will skip fixed variables
             pass
 
     # Append non-constants that have permutable positions
     for col, idxs in counts.items():
         if verbose and verbose_level > 40:
-            print(col, ':', idxs)
+            print(col, ":", idxs)
 
         if len(idxs) == 1:
             return -1
         elif len(idxs) >= 1:
             perm_groups.append(idxs)
 
     if verbose and verbose_level > 40:
-        print('counts:', counts)
-        print('perm_groups:', perm_groups)
+        print("counts:", counts)
+        print("perm_groups:", perm_groups)
 
     if len(perm_groups):
         return perm_groups
     else:
         return -1
 
 
-def _check_identical_cols_count_symbols_v2(counts_matrix, verbose=False, verbose_level=0):
-    """ This function is used to find same symbol permutables. In practice it is a variance of `_check_cols_symbols_vX`
+def _check_identical_cols_count_symbols_v2(
+    counts_matrix, verbose=False, verbose_level=0
+):
+    """This function is used to find same symbol permutables. In practice it is a variance of `_check_cols_symbols_vX`
 
     Args:
         counts_matrix (numpy.ndarray) : a matrix where rows are inputs and columns are possible input types (0,1 or #)
 
     Returns:
         perm_groups (list) : a list of the indexes that can be permuted
     """
     if verbose and verbose_level > 20:
-        print('-- Check Identical Col Counts (v2) --')
+        print("-- Check Identical Col Counts (v2) --")
 
-    counts = {}         # Multi Counts
-    perm_groups = []    # A list of groups of Permutable Indexes
+    counts = {}  # Multi Counts
+    perm_groups = []  # A list of groups of Permutable Indexes
 
     for i, row in enumerate(counts_matrix, start=0):
         # a tuple (hashable) version of the row counts
         row = row.tolist()
         row_tuple = tuple(row)
 
         if verbose and verbose_level > 30:
-            print('RC: %s : %s' % (i, row_tuple))
+            print("RC: %s : %s" % (i, row_tuple))
 
         if row_tuple in counts:
             # we have seen this one before, so add it to the permutation group
             counts[row_tuple].append(i)
         else:
             # we have not seen this count before, so create a new entry for it
             counts[row_tuple] = [i]
 
     # Append non-constants that have permutable positions
     for col, idxs in counts.items():
         if verbose and verbose_level > 30:
-            print(col, ':', idxs)
+            print(col, ":", idxs)
 
         if len(idxs) >= 2:
             perm_groups.append(idxs)
 
     if verbose and verbose_level > 30:
-        print('counts:', counts)
-        print('sames_groups:', perm_groups)
+        print("counts:", counts)
+        print("sames_groups:", perm_groups)
 
     if len(perm_groups):
         return perm_groups
     else:
         return []
 
 
 def _count_cols_symbols(pi_matrix=None, verbose=False, verbose_level=0):
-    """ Given a matrix, where each row is a prime implicant, counts how many 0's, 1's and 2's are found in each column.
+    """Given a matrix, where each row is a prime implicant, counts how many 0's, 1's and 2's are found in each column.
 
     Args:
         pi_matrix (numpy.ndarray) : a matrix ``n \times k`` of ``n`` prime implicants.
 
     Returns:
         counts (numpy.ndarray) : a matrix ``n \times 3`` where the entries are counts.
     """
     if verbose and verbose_level > 20:
-        print(' -- Count Cols (v2) --')
+        print(" -- Count Cols (v2) --")
     # How many PI?
     n = pi_matrix.shape[1]
     # Instanciate count matrix
     counts = np.zeros((n, 3), dtype=int)
     for i, col in enumerate(pi_matrix.T):
         # Count how many values are found and update the matrix of counts
         val, cnt = np.unique(col, return_counts=True)
         # print(val, cnt)
         counts[i, val] = cnt
 
     return counts
 
-def __ts_covers(two_symbol, permut_indexes, input, verbose=False):
+
+def _ts_covers(two_symbol, permut_indexes, input, verbose=False):
     """Helper method to test if an input is being covered by a two symbol permuted implicant
 
     Args:
         two_symbol (string): the two_symbol implicant.
         permut_indexes (list): a list-of-lists of the implicant indexes that are permutables.
         input (string): the input string to be checked.
 
     Returns:
         x (bool): True if covered else False.
     """
+    if verbose:
+        print("Evaluating permutation coverage")
     # No permutation, just plain implicant coverage?
     if not len(permut_indexes):
         if __pi_covers(two_symbol, input):
             return True
     # There are permutations to generate and check
     else:
         # NEW METHOD: Generates the expanded logic of the Two-Symbol Schema
@@ -624,15 +492,15 @@
                 if __pi_covers(tmp, input):
                     return True
         """
     return False
 
 
 def computes_ts_coverage(k, outputs, two_symbols):
-    """ Computes the input coverage by Two Symbol schematas.
+    """Computes the input coverage by Two Symbol schematas.
 
     Args:
         k (int): the number of inputs.
         outpus (list): the list of transition outputs.
         two_symbols (list): The final list of Two Symbol permutable schematas. This is returned by `find_two_symbols`.
 
     Returns:
@@ -645,11 +513,13 @@
         output = int(outputs[statenum])
         if output == 2:
             output = [0, 1]
         else:
             output = [int(outputs[statenum])]
         for t in output:
             for implicant, permut_indxs, same_symbols_indxs in two_symbols[t]:
-                if __ts_covers(implicant, permut_indxs, binstate):
-                    covering_twosymbols.append((implicant, permut_indxs, same_symbols_indxs))
+                if _ts_covers(implicant, permut_indxs, binstate):
+                    covering_twosymbols.append(
+                        (implicant, permut_indxs, same_symbols_indxs)
+                    )
     #
     return ts_coverage
```

### Comparing `cana-0.2.0/cana/canalization/cboolean_canalization.c` & `cana-1.0.0/cana/canalization/cboolean_canalization.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "cana.canalization.cboolean_canalization",
         "sources": [
-            "cana/canalization/cboolean_canalization.pyx"
+            "/home/BU/jrozum/Documents/github/rionbr/cana/CANA/cana/canalization/cboolean_canalization.pyx"
         ]
     },
     "module_name": "cana.canalization.cboolean_canalization"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -17,17 +17,17 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
-#define CYTHON_FUTURE_DIVISION 1
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -57,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -93,18 +94,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -134,18 +139,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -157,61 +211,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -320,17 +385,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -436,35 +560,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -560,18 +684,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -588,16 +712,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -719,14 +845,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -831,15 +958,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "cana/canalization/cboolean_canalization.pyx",
+  "cboolean_canalization.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct____pi_covers;
 struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_1_genexpr;
 struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage;
 struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_3_genexpr;
@@ -1001,26 +1128,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1041,21 +1168,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1097,14 +1232,32 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* StringJoin.proto */
+#if PY_MAJOR_VERSION < 3
+#define __Pyx_PyString_Join __Pyx_PyBytes_Join
+#define __Pyx_PyBaseString_Join(s, v) (PyUnicode_CheckExact(s) ? PyUnicode_Join(s, v) : __Pyx_PyBytes_Join(s, v))
+#else
+#define __Pyx_PyString_Join PyUnicode_Join
+#define __Pyx_PyBaseString_Join PyUnicode_Join
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+    #if PY_MAJOR_VERSION < 3
+    #define __Pyx_PyBytes_Join _PyString_Join
+    #else
+    #define __Pyx_PyBytes_Join _PyBytes_Join
+    #endif
+#else
+static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
+#endif
+
 /* RaiseTooManyValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
 /* IterFinish.proto */
@@ -1184,14 +1337,21 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* StrEquals.proto */
+#if PY_MAJOR_VERSION >= 3
+#define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
+#else
+#define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
+#endif
+
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
@@ -1262,44 +1422,14 @@
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* IterNext.proto */
 #define __Pyx_PyIter_Next(obj) __Pyx_PyIter_Next2(obj, NULL)
 static CYTHON_INLINE PyObject *__Pyx_PyIter_Next2(PyObject *, PyObject *);
 
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod0.proto */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* UnpackTupleError.proto */
-static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
-
-/* UnpackTuple2.proto */
-#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
-    (likely(is_tuple || PyTuple_Check(tuple)) ?\
-        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
-            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
-            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
-        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
-static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
-    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
-static int __Pyx_unpack_tuple2_generic(
-    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
-
-/* dict_iter.proto */
-static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
-                                                   Py_ssize_t* p_orig_length, int* p_is_dict);
-static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
-                                              PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
-
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1385,14 +1515,17 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* CoroutineBase.proto */
 typedef PyObject *(*__pyx_coroutine_body_t)(PyObject *, PyThreadState *, PyObject *);
 #if CYTHON_USE_EXC_INFO_STACK
 #define __Pyx_ExcInfoStruct  _PyErr_StackItem
@@ -1504,14 +1637,15 @@
 static const char __pyx_k_b1[] = "b1";
 static const char __pyx_k_pi[] = "pi";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_zip[] = "zip";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_done[] = "done";
+static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_used[] = "used";
 static const char __pyx_k_wnum[] = "wnum";
 static const char __pyx_k_close[] = "close";
@@ -1557,40 +1691,39 @@
 static const char __pyx_k_return_pi_coverage[] = "return_pi_coverage";
 static const char __pyx_k_make_density_groups[] = "make_density_groups";
 static const char __pyx_k_statenum_to_binstate[] = "statenum_to_binstate";
 static const char __pyx_k_input_wildcard_coverage[] = "input_wildcard_coverage";
 static const char __pyx_k_expand_wildcard_schemata[] = "expand_wildcard_schemata";
 static const char __pyx_k_pi_covers_locals_genexpr[] = "__pi_covers.<locals>.genexpr";
 static const char __pyx_k_SYMMETRIC_WILDCARD_SYMBOL[] = "SYMMETRIC_WILDCARD_SYMBOL";
+static const char __pyx_k_cboolean_canalization_pyx[] = "cboolean_canalization.pyx";
 static const char __pyx_k_Cythonized_Boolean_Canalization[] = "\n(Cythonized) Boolean Canalization\n=====================\n\nFunctions to compute the Quine-McCluskey algorithm in cython for increaed computation speed.\n\n";
 static const char __pyx_k_cana_canalization_cboolean_canal[] = "cana.canalization.cboolean_canalization";
 static const char __pyx_k_input_wildcard_coverage_locals_g[] = "input_wildcard_coverage.<locals>.genexpr";
-static const char __pyx_k_cana_canalization_cboolean_canal_2[] = "cana/canalization/cboolean_canalization.pyx";
-static PyObject *__pyx_kp_u_;
-static PyObject *__pyx_kp_u_0;
-static PyObject *__pyx_kp_u_1;
+static PyObject *__pyx_kp_s_;
+static PyObject *__pyx_kp_s_0;
+static PyObject *__pyx_kp_s_1;
 static PyObject *__pyx_n_s_SYMMETRIC_WILDCARD_SYMBOL;
 static PyObject *__pyx_n_s_WILDCARD_SYMBOL;
 static PyObject *__pyx_n_s__2;
-static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_kp_u__3;
+static PyObject *__pyx_kp_s__3;
 static PyObject *__pyx_n_s_add;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_b0;
 static PyObject *__pyx_n_s_b1;
 static PyObject *__pyx_n_s_binary_density;
 static PyObject *__pyx_n_s_binary_states;
 static PyObject *__pyx_n_s_binstate;
 static PyObject *__pyx_n_s_binstate0;
 static PyObject *__pyx_n_s_binstate1;
 static PyObject *__pyx_n_s_binstate2;
 static PyObject *__pyx_n_s_cana_canalization_cboolean_canal;
-static PyObject *__pyx_kp_s_cana_canalization_cboolean_canal_2;
 static PyObject *__pyx_n_s_cana_cutils;
+static PyObject *__pyx_kp_s_cboolean_canalization_pyx;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_count;
 static PyObject *__pyx_n_s_density;
 static PyObject *__pyx_n_s_density_groups;
 static PyObject *__pyx_n_s_done;
 static PyObject *__pyx_n_s_enumerate;
@@ -1606,14 +1739,15 @@
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_input;
 static PyObject *__pyx_n_s_input_binstates;
 static PyObject *__pyx_n_s_input_to_wildcards;
 static PyObject *__pyx_n_s_input_wildcard_coverage;
 static PyObject *__pyx_n_s_input_wildcard_coverage_locals_g;
 static PyObject *__pyx_n_s_items;
+static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_make_density_groups;
 static PyObject *__pyx_n_s_matched_implicants;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_newstate;
 static PyObject *__pyx_n_s_nwildcards;
@@ -1985,16 +2119,16 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_12canalization_21cboolean_canalization_2find_wildcards(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_binstate1, PyObject *__pyx_v_binstate2) {
-  PyObject *__pyx_7genexpr__pyx_v_b0 = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_b1 = NULL;
+  PyObject *__pyx_v_b0 = NULL;
+  PyObject *__pyx_v_b1 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
@@ -2012,144 +2146,134 @@
  *     """
  *     # assert len(s1) == len(s2) , "The two binstates must have the same length"
  *     return "".join([b0 if (b0 == b1) else WILDCARD_SYMBOL for b0, b1 in zip(binstate1, binstate2)])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L5_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_binstate1);
+  __Pyx_GIVEREF(__pyx_v_binstate1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_binstate1);
+  __Pyx_INCREF(__pyx_v_binstate2);
+  __Pyx_GIVEREF(__pyx_v_binstate2);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_binstate2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_zip, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
+    __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
+    __pyx_t_5 = NULL;
+  } else {
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_v_binstate1);
-    __Pyx_GIVEREF(__pyx_v_binstate1);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_binstate1);
-    __Pyx_INCREF(__pyx_v_binstate2);
-    __Pyx_GIVEREF(__pyx_v_binstate2);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_binstate2);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_zip, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-      __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-      __pyx_t_5 = NULL;
-    } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L5_error)
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_5)) {
-        if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 49, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
-        } else {
-          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 49, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
-        }
-      } else {
-        __pyx_t_3 = __pyx_t_5(__pyx_t_2);
-        if (unlikely(!__pyx_t_3)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 49, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_3);
-      }
-      if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
-        PyObject* sequence = __pyx_t_3;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 49, __pyx_L5_error)
-        }
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_5)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
-        }
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 49, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         #endif
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else {
-        Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 49, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
-        index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_6);
-        index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 49, __pyx_L5_error)
-        __pyx_t_9 = NULL;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        goto __pyx_L9_unpacking_done;
-        __pyx_L8_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_9 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 49, __pyx_L5_error)
-        __pyx_L9_unpacking_done:;
-      }
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_b0, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_b1, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_7 = PyObject_RichCompare(__pyx_7genexpr__pyx_v_b0, __pyx_7genexpr__pyx_v_b1, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L5_error)
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 49, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (__pyx_t_10) {
-        __Pyx_INCREF(__pyx_7genexpr__pyx_v_b0);
-        __pyx_t_3 = __pyx_7genexpr__pyx_v_b0;
+        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
+    } else {
+      __pyx_t_3 = __pyx_t_5(__pyx_t_2);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 49, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
+    }
+    if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
+      PyObject* sequence = __pyx_t_3;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 49, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      if (likely(PyTuple_CheckExact(sequence))) {
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
-        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_WILDCARD_SYMBOL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_3 = __pyx_t_7;
-        __pyx_t_7 = 0;
+        __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 49, __pyx_L5_error)
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_7);
+      #else
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else {
+      Py_ssize_t index = -1;
+      __pyx_t_8 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
+      index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_6);
+      index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+      __pyx_t_9 = NULL;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      goto __pyx_L6_unpacking_done;
+      __pyx_L5_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_9 = NULL;
+      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+      __PYX_ERR(0, 49, __pyx_L1_error)
+      __pyx_L6_unpacking_done:;
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b0); __pyx_7genexpr__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b1); __pyx_7genexpr__pyx_v_b1 = 0;
-    goto __pyx_L10_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b0); __pyx_7genexpr__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b1); __pyx_7genexpr__pyx_v_b1 = 0;
-    goto __pyx_L1_error;
-    __pyx_L10_exit_scope:;
-  } /* exit inner scope */
-  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_b0, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_b1, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __pyx_t_7 = PyObject_RichCompare(__pyx_v_b0, __pyx_v_b1, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (__pyx_t_10) {
+      __Pyx_INCREF(__pyx_v_b0);
+      __pyx_t_3 = __pyx_v_b0;
+    } else {
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_WILDCARD_SYMBOL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_3 = __pyx_t_7;
+      __pyx_t_7 = 0;
+    }
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "cana/canalization/cboolean_canalization.pyx":38
@@ -2167,16 +2291,16 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("cana.canalization.cboolean_canalization.find_wildcards", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b0);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_b1);
+  __Pyx_XDECREF(__pyx_v_b0);
+  __Pyx_XDECREF(__pyx_v_b1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cana/canalization/cboolean_canalization.pyx":52
  * 
@@ -2228,15 +2352,15 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_1);
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_s_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -2774,15 +2898,15 @@
             /* "cana/canalization/cboolean_canalization.pyx":111
  * 
  *                     for idx, b0 in enumerate(binstate0):
  *                         if b0 == '0':             # <<<<<<<<<<<<<<
  *                             binstate1 = flip_binstate_bit(binstate0, idx)
  *                             if binstate1 in density_groups[density + 1]:
  */
-            __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_v_b0, __pyx_kp_u_0, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+            __pyx_t_7 = (__Pyx_PyString_Equals(__pyx_v_b0, __pyx_kp_s_0, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
             if (__pyx_t_7) {
 
               /* "cana/canalization/cboolean_canalization.pyx":112
  *                     for idx, b0 in enumerate(binstate0):
  *                         if b0 == '0':
  *                             binstate1 = flip_binstate_bit(binstate0, idx)             # <<<<<<<<<<<<<<
  *                             if binstate1 in density_groups[density + 1]:
@@ -3858,16 +3982,16 @@
       /* "cana/canalization/cboolean_canalization.pyx":170
  *             wildstates = statenum_to_binstate(wildstatenum, nwildcards)
  *             wnum = 0
  *             newstate = ''             # <<<<<<<<<<<<<<
  *             for b in schemata:
  *                 if b == WILDCARD_SYMBOL:
  */
-      __Pyx_INCREF(__pyx_kp_u_);
-      __Pyx_XDECREF_SET(__pyx_v_newstate, __pyx_kp_u_);
+      __Pyx_INCREF(__pyx_kp_s_);
+      __Pyx_XDECREF_SET(__pyx_v_newstate, __pyx_kp_s_);
 
       /* "cana/canalization/cboolean_canalization.pyx":171
  *             wnum = 0
  *             newstate = ''
  *             for b in schemata:             # <<<<<<<<<<<<<<
  *                 if b == WILDCARD_SYMBOL:
  *                     newstate += wildstates[wnum]
@@ -4540,29 +4664,29 @@
  */
 
 static PyObject *__pyx_pf_4cana_12canalization_21cboolean_canalization_16input_wildcard_coverage(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_pi_coverage) {
   struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage *__pyx_cur_scope;
   Py_ssize_t __pyx_v_k;
   PyObject *__pyx_v_input_to_wildcards = NULL;
   PyObject *__pyx_v_binstate = NULL;
-  Py_ssize_t __pyx_8genexpr2__pyx_v_i;
+  Py_ssize_t __pyx_8genexpr1__pyx_v_i;
   PyObject *__pyx_gb_4cana_12canalization_21cboolean_canalization_23input_wildcard_coverage_2generator1 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  int __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *(*__pyx_t_10)(PyObject *);
+  Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("input_wildcard_coverage", 0);
   __pyx_cur_scope = (struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage *)__pyx_tp_new_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage(__pyx_ptype_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage *)Py_None);
@@ -4597,16 +4721,16 @@
  */
   { /* enter inner scope */
     __pyx_t_2 = PyDict_New(); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_v_k;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
-      __pyx_8genexpr2__pyx_v_i = __pyx_t_5;
-      __pyx_t_1 = PyInt_FromSsize_t(__pyx_8genexpr2__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+      __pyx_8genexpr1__pyx_v_i = __pyx_t_5;
+      __pyx_t_1 = PyInt_FromSsize_t(__pyx_8genexpr1__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 214, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (unlikely(PyDict_SetItem(__pyx_t_2, (PyObject*)__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 214, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
@@ -4617,72 +4741,167 @@
   /* "cana/canalization/cboolean_canalization.pyx":215
  * 
  *     input_to_wildcards = {i: dict() for i in range(k)}
  *     for binstate, piset in pi_coverage.items():             # <<<<<<<<<<<<<<
  *         for i in range(k):
  *             input_to_wildcards[i][binstate] = tuple(pi[i] == WILDCARD_SYMBOL for pi in piset)
  */
-  __pyx_t_3 = 0;
-  if (unlikely(__pyx_v_pi_coverage == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 215, __pyx_L1_error)
-  }
-  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_pi_coverage, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_7)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi_coverage, __pyx_n_s_items); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_2);
-  __pyx_t_2 = __pyx_t_6;
-  __pyx_t_6 = 0;
-  while (1) {
-    __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_1, NULL, __pyx_t_7);
-    if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_6, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
+    __pyx_t_6 = __pyx_t_2; __Pyx_INCREF(__pyx_t_6); __pyx_t_3 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_3 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_XDECREF_SET(__pyx_v_binstate, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_piset);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_piset, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
+    __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 215, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_6))) {
+        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_6)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
+      } else {
+        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
+      }
+    } else {
+      __pyx_t_2 = __pyx_t_7(__pyx_t_6);
+      if (unlikely(!__pyx_t_2)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 215, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_2);
+    }
+    if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
+      PyObject* sequence = __pyx_t_2;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 215, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      if (likely(PyTuple_CheckExact(sequence))) {
+        __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
+      } else {
+        __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
+      }
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_8);
+      #else
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 215, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      #endif
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    } else {
+      Py_ssize_t index = -1;
+      __pyx_t_9 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 215, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_10 = Py_TYPE(__pyx_t_9)->tp_iternext;
+      index = 0; __pyx_t_1 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_1);
+      index = 1; __pyx_t_8 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_8)) goto __pyx_L7_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_8);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 215, __pyx_L1_error)
+      __pyx_t_10 = NULL;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      goto __pyx_L8_unpacking_done;
+      __pyx_L7_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_10 = NULL;
+      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+      __PYX_ERR(0, 215, __pyx_L1_error)
+      __pyx_L8_unpacking_done:;
+    }
+    __Pyx_XDECREF_SET(__pyx_v_binstate, __pyx_t_1);
     __pyx_t_1 = 0;
+    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_piset);
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_piset, __pyx_t_8);
+    __Pyx_GIVEREF(__pyx_t_8);
+    __pyx_t_8 = 0;
 
     /* "cana/canalization/cboolean_canalization.pyx":216
  *     input_to_wildcards = {i: dict() for i in range(k)}
  *     for binstate, piset in pi_coverage.items():
  *         for i in range(k):             # <<<<<<<<<<<<<<
  *             input_to_wildcards[i][binstate] = tuple(pi[i] == WILDCARD_SYMBOL for pi in piset)
  * 
  */
-    __pyx_t_5 = __pyx_v_k;
-    __pyx_t_9 = __pyx_t_5;
-    for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
-      __pyx_cur_scope->__pyx_v_i = __pyx_t_10;
+    __pyx_t_4 = __pyx_v_k;
+    __pyx_t_5 = __pyx_t_4;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_5; __pyx_t_11+=1) {
+      __pyx_cur_scope->__pyx_v_i = __pyx_t_11;
 
       /* "cana/canalization/cboolean_canalization.pyx":217
  *     for binstate, piset in pi_coverage.items():
  *         for i in range(k):
  *             input_to_wildcards[i][binstate] = tuple(pi[i] == WILDCARD_SYMBOL for pi in piset)             # <<<<<<<<<<<<<<
  * 
  *     return input_to_wildcards
  */
-      __pyx_t_1 = __pyx_pf_4cana_12canalization_21cboolean_canalization_23input_wildcard_coverage_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PySequence_Tuple(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 217, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+      __pyx_t_2 = __pyx_pf_4cana_12canalization_21cboolean_canalization_23input_wildcard_coverage_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_8 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 217, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_input_to_wildcards, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_11 = __Pyx_PyDict_GetItem(__pyx_v_input_to_wildcards, __pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 217, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_binstate, __pyx_t_8) < 0)) __PYX_ERR(0, 217, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_11, __pyx_v_binstate, __pyx_t_6) < 0)) __PYX_ERR(0, 217, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
+
+    /* "cana/canalization/cboolean_canalization.pyx":215
+ * 
+ *     input_to_wildcards = {i: dict() for i in range(k)}
+ *     for binstate, piset in pi_coverage.items():             # <<<<<<<<<<<<<<
+ *         for i in range(k):
+ *             input_to_wildcards[i][binstate] = tuple(pi[i] == WILDCARD_SYMBOL for pi in piset)
+ */
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "cana/canalization/cboolean_canalization.pyx":219
  *             input_to_wildcards[i][binstate] = tuple(pi[i] == WILDCARD_SYMBOL for pi in piset)
  * 
  *     return input_to_wildcards             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
@@ -4699,15 +4918,16 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("cana.canalization.cboolean_canalization.input_wildcard_coverage", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_input_to_wildcards);
   __Pyx_XDECREF(__pyx_v_binstate);
   __Pyx_XDECREF(__pyx_gb_4cana_12canalization_21cboolean_canalization_23input_wildcard_coverage_2generator1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
@@ -4819,20 +5039,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_1_genexpr *__pyx_freelist_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_1_genexpr = 0;
 
 static PyObject *__pyx_tp_new_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -4933,20 +5156,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage *__pyx_freelist_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage[8];
 static int __pyx_freecount_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage = 0;
 
 static PyObject *__pyx_tp_new_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_2_input_wildcard_coverage(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -5048,20 +5274,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_3_genexpr *__pyx_freelist_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_3_genexpr = 0;
 
 static PyObject *__pyx_tp_new_4cana_12canalization_21cboolean_canalization___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -5162,20 +5391,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 static int __pyx_import_star_set(PyObject *o, PyObject* py_name, char *name) {
@@ -5350,36 +5582,35 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
-  {&__pyx_kp_u_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 1, 0, 0},
-  {&__pyx_kp_u_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 1, 0, 0},
+  {&__pyx_kp_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 0},
+  {&__pyx_kp_s_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 0, 1, 0},
   {&__pyx_n_s_SYMMETRIC_WILDCARD_SYMBOL, __pyx_k_SYMMETRIC_WILDCARD_SYMBOL, sizeof(__pyx_k_SYMMETRIC_WILDCARD_SYMBOL), 0, 0, 1, 1},
   {&__pyx_n_s_WILDCARD_SYMBOL, __pyx_k_WILDCARD_SYMBOL, sizeof(__pyx_k_WILDCARD_SYMBOL), 0, 0, 1, 1},
   {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
-  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
+  {&__pyx_kp_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 0},
   {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
   {&__pyx_n_s_b0, __pyx_k_b0, sizeof(__pyx_k_b0), 0, 0, 1, 1},
   {&__pyx_n_s_b1, __pyx_k_b1, sizeof(__pyx_k_b1), 0, 0, 1, 1},
   {&__pyx_n_s_binary_density, __pyx_k_binary_density, sizeof(__pyx_k_binary_density), 0, 0, 1, 1},
   {&__pyx_n_s_binary_states, __pyx_k_binary_states, sizeof(__pyx_k_binary_states), 0, 0, 1, 1},
   {&__pyx_n_s_binstate, __pyx_k_binstate, sizeof(__pyx_k_binstate), 0, 0, 1, 1},
   {&__pyx_n_s_binstate0, __pyx_k_binstate0, sizeof(__pyx_k_binstate0), 0, 0, 1, 1},
   {&__pyx_n_s_binstate1, __pyx_k_binstate1, sizeof(__pyx_k_binstate1), 0, 0, 1, 1},
   {&__pyx_n_s_binstate2, __pyx_k_binstate2, sizeof(__pyx_k_binstate2), 0, 0, 1, 1},
   {&__pyx_n_s_cana_canalization_cboolean_canal, __pyx_k_cana_canalization_cboolean_canal, sizeof(__pyx_k_cana_canalization_cboolean_canal), 0, 0, 1, 1},
-  {&__pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_k_cana_canalization_cboolean_canal_2, sizeof(__pyx_k_cana_canalization_cboolean_canal_2), 0, 0, 1, 0},
   {&__pyx_n_s_cana_cutils, __pyx_k_cana_cutils, sizeof(__pyx_k_cana_cutils), 0, 0, 1, 1},
+  {&__pyx_kp_s_cboolean_canalization_pyx, __pyx_k_cboolean_canalization_pyx, sizeof(__pyx_k_cboolean_canalization_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
   {&__pyx_n_s_density, __pyx_k_density, sizeof(__pyx_k_density), 0, 0, 1, 1},
   {&__pyx_n_s_density_groups, __pyx_k_density_groups, sizeof(__pyx_k_density_groups), 0, 0, 1, 1},
   {&__pyx_n_s_done, __pyx_k_done, sizeof(__pyx_k_done), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
@@ -5395,14 +5626,15 @@
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
   {&__pyx_n_s_input_binstates, __pyx_k_input_binstates, sizeof(__pyx_k_input_binstates), 0, 0, 1, 1},
   {&__pyx_n_s_input_to_wildcards, __pyx_k_input_to_wildcards, sizeof(__pyx_k_input_to_wildcards), 0, 0, 1, 1},
   {&__pyx_n_s_input_wildcard_coverage, __pyx_k_input_wildcard_coverage, sizeof(__pyx_k_input_wildcard_coverage), 0, 0, 1, 1},
   {&__pyx_n_s_input_wildcard_coverage_locals_g, __pyx_k_input_wildcard_coverage_locals_g, sizeof(__pyx_k_input_wildcard_coverage_locals_g), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
+  {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_make_density_groups, __pyx_k_make_density_groups, sizeof(__pyx_k_make_density_groups), 0, 0, 1, 1},
   {&__pyx_n_s_matched_implicants, __pyx_k_matched_implicants, sizeof(__pyx_k_matched_implicants), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_newstate, __pyx_k_newstate, sizeof(__pyx_k_newstate), 0, 0, 1, 1},
   {&__pyx_n_s_nwildcards, __pyx_k_nwildcards, sizeof(__pyx_k_nwildcards), 0, 0, 1, 1},
@@ -5449,120 +5681,120 @@
  * def make_density_groups(input_binstates):             # <<<<<<<<<<<<<<
  *     """
  *     """
  */
   __pyx_tuple__4 = PyTuple_Pack(4, __pyx_n_s_input_binstates, __pyx_n_s_density_groups, __pyx_n_s_binstate, __pyx_n_s_density); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_make_density_groups, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_make_density_groups, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":38
  * 
  * 
  * def find_wildcards(binstate1, binstate2):             # <<<<<<<<<<<<<<
  *     """
  *     Compare two binary states and replace any differing bits by a wildcard.
  */
   __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_binstate1, __pyx_n_s_binstate2, __pyx_n_s_b0, __pyx_n_s_b1); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_find_wildcards, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_find_wildcards, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":52
  * 
  * 
  * def binary_density(binstate):             # <<<<<<<<<<<<<<
  *     """
  *     Find the density (number of 1s) for a term with possible wildcards.
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_binstate); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_binary_density, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_binary_density, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 52, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":59
  * 
  * 
  * def replace_wildcard(binstate, idx):             # <<<<<<<<<<<<<<
  *     """
  *     Return the binary state with a wildcard at the idx position.
  */
   __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_s_binstate, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_replace_wildcard, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_replace_wildcard, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 59, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":66
  * 
  * 
  * def find_implicants_qm(input_binstates, verbose=False):             # <<<<<<<<<<<<<<
  *     """ Finds the prime implicants (PI) using the Quine-McCluskey algorithm :cite:`Quine:1955`.
  * 
  */
   __pyx_tuple__12 = PyTuple_Pack(13, __pyx_n_s_input_binstates, __pyx_n_s_verbose, __pyx_n_s_matched_implicants, __pyx_n_s_done, __pyx_n_s_density_groups, __pyx_n_s_used, __pyx_n_s_density, __pyx_n_s_binstate0, __pyx_n_s_idx, __pyx_n_s_b0, __pyx_n_s_binstate1, __pyx_n_s_groups, __pyx_n_s_prime_implicants); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_find_implicants_qm, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_find_implicants_qm, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 66, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":137
  * 
  * 
  * def __pi_covers(implicant, binstate):             # <<<<<<<<<<<<<<
  *     """Determines if a binarystate is covered by a specific implicant.
  *     Args:
  */
   __pyx_tuple__14 = PyTuple_Pack(4, __pyx_n_s_implicant, __pyx_n_s_binstate, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_pi_covers, 137, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_pi_covers, 137, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 137, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":149
  * 
  * 
  * def expand_wildcard_schemata(schemata):             # <<<<<<<<<<<<<<
  *     """
  *     Expand a wildcard schemata to list all binary states it covers.
  */
   __pyx_tuple__16 = PyTuple_Pack(8, __pyx_n_s_schemata, __pyx_n_s_nwildcards, __pyx_n_s_binary_states, __pyx_n_s_wildstatenum, __pyx_n_s_wildstates, __pyx_n_s_wnum, __pyx_n_s_newstate, __pyx_n_s_b); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_expand_wildcard_schemata, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_expand_wildcard_schemata, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 149, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":181
  * 
  * 
  * def return_pi_coverage(prime_implicants):             # <<<<<<<<<<<<<<
  *     """Computes the binary states coverage by Prime Implicant schematas.
  * 
  */
   __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_prime_implicants, __pyx_n_s_pi_coverage, __pyx_n_s_pi, __pyx_n_s_binstate); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_return_pi_coverage, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_return_pi_coverage, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 181, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":201
  * 
  * 
  * def input_wildcard_coverage(pi_coverage):             # <<<<<<<<<<<<<<
  *     """Computes the binary states coverage by Prime Implicant schematas.
  * 
  */
   __pyx_tuple__20 = PyTuple_Pack(9, __pyx_n_s_pi_coverage, __pyx_n_s_k, __pyx_n_s_input_to_wildcards, __pyx_n_s_binstate, __pyx_n_s_piset, __pyx_n_s_i, __pyx_n_s_i, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_canalization_cboolean_canal_2, __pyx_n_s_input_wildcard_coverage, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cboolean_canalization_pyx, __pyx_n_s_input_wildcard_coverage, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -5832,15 +6064,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_cana__canalization__cboolean_canalization) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5878,37 +6110,37 @@
  * WILDCARD_SYMBOL = '#'
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s__2);
   __Pyx_GIVEREF(__pyx_n_s__2);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__2);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_cana_cutils, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_cana_cutils, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "cana/canalization/cboolean_canalization.pyx":17
  * from cana.cutils import *
  * 
  * WILDCARD_SYMBOL = '#'             # <<<<<<<<<<<<<<
  * SYMMETRIC_WILDCARD_SYMBOL = '*'
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WILDCARD_SYMBOL, __pyx_kp_u__3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WILDCARD_SYMBOL, __pyx_kp_s__3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":18
  * 
  * WILDCARD_SYMBOL = '#'
  * SYMMETRIC_WILDCARD_SYMBOL = '*'             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SYMMETRIC_WILDCARD_SYMBOL, __pyx_kp_u__2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SYMMETRIC_WILDCARD_SYMBOL, __pyx_n_s__2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
 
   /* "cana/canalization/cboolean_canalization.pyx":24
  * # Quine-McCluskey Functions
  * #
  * def make_density_groups(input_binstates):             # <<<<<<<<<<<<<<
  *     """
  *     """
@@ -6569,14 +6801,21 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* StringJoin */
+#if !CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
+    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
+}
+#endif
+
 /* RaiseTooManyValuesToUnpack */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
     PyErr_Format(PyExc_ValueError,
                  "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
 }
 
 /* RaiseNeedMoreValuesToUnpack */
@@ -6623,18 +6862,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* SliceObject */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
@@ -6940,15 +7177,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -6986,15 +7223,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -7123,15 +7360,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -7344,307 +7581,14 @@
         if (likely(next))
             return next;
     }
 #endif
     return __Pyx_PyIter_Next2Default(defval);
 }
 
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (descr != NULL) {
-        *method = descr;
-        return 0;
-    }
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
-#endif
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
-/* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
-    PyObject *method = NULL, *result = NULL;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_CallOneArg(method, obj);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) goto bad;
-    result = __Pyx_PyObject_CallNoArg(method);
-    Py_DECREF(method);
-bad:
-    return result;
-}
-
-/* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* UnpackTupleError */
-static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
-    if (t == Py_None) {
-      __Pyx_RaiseNoneNotIterableError();
-    } else if (PyTuple_GET_SIZE(t) < index) {
-      __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
-    } else {
-      __Pyx_RaiseTooManyValuesError(index);
-    }
-}
-
-/* UnpackTuple2 */
-static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
-        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
-    PyObject *value1 = NULL, *value2 = NULL;
-#if CYTHON_COMPILING_IN_PYPY
-    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
-    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
-#else
-    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
-    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
-#endif
-    if (decref_tuple) {
-        Py_DECREF(tuple);
-    }
-    *pvalue1 = value1;
-    *pvalue2 = value2;
-    return 0;
-#if CYTHON_COMPILING_IN_PYPY
-bad:
-    Py_XDECREF(value1);
-    Py_XDECREF(value2);
-    if (decref_tuple) { Py_XDECREF(tuple); }
-    return -1;
-#endif
-}
-static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
-                                       int has_known_size, int decref_tuple) {
-    Py_ssize_t index;
-    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
-    iternextfunc iternext;
-    iter = PyObject_GetIter(tuple);
-    if (unlikely(!iter)) goto bad;
-    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
-    iternext = Py_TYPE(iter)->tp_iternext;
-    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
-    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
-    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
-    Py_DECREF(iter);
-    *pvalue1 = value1;
-    *pvalue2 = value2;
-    return 0;
-unpacking_failed:
-    if (!has_known_size && __Pyx_IterFinish() == 0)
-        __Pyx_RaiseNeedMoreValuesError(index);
-bad:
-    Py_XDECREF(iter);
-    Py_XDECREF(value1);
-    Py_XDECREF(value2);
-    if (decref_tuple) { Py_XDECREF(tuple); }
-    return -1;
-}
-
-/* dict_iter */
-static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
-                                                   Py_ssize_t* p_orig_length, int* p_source_is_dict) {
-    is_dict = is_dict || likely(PyDict_CheckExact(iterable));
-    *p_source_is_dict = is_dict;
-    if (is_dict) {
-#if !CYTHON_COMPILING_IN_PYPY
-        *p_orig_length = PyDict_Size(iterable);
-        Py_INCREF(iterable);
-        return iterable;
-#elif PY_MAJOR_VERSION >= 3
-        static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
-        PyObject **pp = NULL;
-        if (method_name) {
-            const char *name = PyUnicode_AsUTF8(method_name);
-            if (strcmp(name, "iteritems") == 0) pp = &py_items;
-            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
-            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
-            if (pp) {
-                if (!*pp) {
-                    *pp = PyUnicode_FromString(name + 4);
-                    if (!*pp)
-                        return NULL;
-                }
-                method_name = *pp;
-            }
-        }
-#endif
-    }
-    *p_orig_length = 0;
-    if (method_name) {
-        PyObject* iter;
-        iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
-        if (!iterable)
-            return NULL;
-#if !CYTHON_COMPILING_IN_PYPY
-        if (PyTuple_CheckExact(iterable) || PyList_CheckExact(iterable))
-            return iterable;
-#endif
-        iter = PyObject_GetIter(iterable);
-        Py_DECREF(iterable);
-        return iter;
-    }
-    return PyObject_GetIter(iterable);
-}
-static CYTHON_INLINE int __Pyx_dict_iter_next(
-        PyObject* iter_obj, CYTHON_NCP_UNUSED Py_ssize_t orig_length, CYTHON_NCP_UNUSED Py_ssize_t* ppos,
-        PyObject** pkey, PyObject** pvalue, PyObject** pitem, int source_is_dict) {
-    PyObject* next_item;
-#if !CYTHON_COMPILING_IN_PYPY
-    if (source_is_dict) {
-        PyObject *key, *value;
-        if (unlikely(orig_length != PyDict_Size(iter_obj))) {
-            PyErr_SetString(PyExc_RuntimeError, "dictionary changed size during iteration");
-            return -1;
-        }
-        if (unlikely(!PyDict_Next(iter_obj, ppos, &key, &value))) {
-            return 0;
-        }
-        if (pitem) {
-            PyObject* tuple = PyTuple_New(2);
-            if (unlikely(!tuple)) {
-                return -1;
-            }
-            Py_INCREF(key);
-            Py_INCREF(value);
-            PyTuple_SET_ITEM(tuple, 0, key);
-            PyTuple_SET_ITEM(tuple, 1, value);
-            *pitem = tuple;
-        } else {
-            if (pkey) {
-                Py_INCREF(key);
-                *pkey = key;
-            }
-            if (pvalue) {
-                Py_INCREF(value);
-                *pvalue = value;
-            }
-        }
-        return 1;
-    } else if (PyTuple_CheckExact(iter_obj)) {
-        Py_ssize_t pos = *ppos;
-        if (unlikely(pos >= PyTuple_GET_SIZE(iter_obj))) return 0;
-        *ppos = pos + 1;
-        next_item = PyTuple_GET_ITEM(iter_obj, pos);
-        Py_INCREF(next_item);
-    } else if (PyList_CheckExact(iter_obj)) {
-        Py_ssize_t pos = *ppos;
-        if (unlikely(pos >= PyList_GET_SIZE(iter_obj))) return 0;
-        *ppos = pos + 1;
-        next_item = PyList_GET_ITEM(iter_obj, pos);
-        Py_INCREF(next_item);
-    } else
-#endif
-    {
-        next_item = PyIter_Next(iter_obj);
-        if (unlikely(!next_item)) {
-            return __Pyx_IterFinish();
-        }
-    }
-    if (pitem) {
-        *pitem = next_item;
-    } else if (pkey && pvalue) {
-        if (__Pyx_unpack_tuple2(next_item, pkey, pvalue, source_is_dict, source_is_dict, 1))
-            return -1;
-    } else if (pkey) {
-        *pkey = next_item;
-    } else {
-        *pvalue = next_item;
-    }
-    return 1;
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -7744,15 +7688,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -7774,15 +7718,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -7868,41 +7812,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -7913,34 +7864,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -8677,28 +8643,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8790,14 +8756,110 @@
     PyErr_SetExcInfo(*type, *value, *tb);
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (descr != NULL) {
+        *method = descr;
+        return 0;
+    }
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'%.50s' object has no attribute '%U'",
+                 tp->tp_name, name);
+#else
+                 "'%.50s' object has no attribute '%.400s'",
+                 tp->tp_name, PyString_AS_STRING(name));
+#endif
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
 /* PyObjectCallMethod1 */
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
 }
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
@@ -8811,14 +8873,20 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -8982,17 +9050,21 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -9772,20 +9844,23 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
@@ -9797,19 +9872,41 @@
 static CYTHON_INLINE int __Pyx_StrEq(const char *s1, const char *s2) {
     while (*s1 != '\0' && *s1 == *s2) { s1++; s2++; }
     return *s1 == *s2;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -10059,14 +10156,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `cana-0.2.0/cana/canalization/cboolean_canalization.pyx` & `cana-1.0.0/cana/canalization/cboolean_canalization.pyx`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/control/fvs.py` & `cana-1.0.0/cana/control/fvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 The NP-complete Feedback Vertex Set (FVS) problem is defined as the minimum number of vertices
 that need to be removed from a directed graph so that the resulting graph has no direct cycle. :cite:`Pardalos:1998` :cite:`Mochizuki:2013`.
 
 Two methods are implemented here. A bruteforce and the Greedy Randomized Adaptive Search Procedure (GRASP) method by :cite:`Pardalos:1998`.
 
 """
+import copy
+import itertools
+
 #   Copyright (C) 2021 by
 #   Alex Gates <ajgates42@gmail.com>
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   All rights reserved.
 #   MIT license.
 import networkx as nx
 import numpy as np
-import itertools
-import copy
 
 
 #
 # GRASP method
 #
 def fvs_grasp(directed_graph, max_iter=100, keep_self_loops=True):
     """The Feedback Vertex Set GRASP implementation.
@@ -47,15 +48,15 @@
     root_var = _root_variables(directed_graph, keep_self_loops=keep_self_loops)
     S = S.union(root_var)
 
     minfvc = set([frozenset(directed_graph.nodes())])
 
     reduced_graph = directed_graph.copy()
 
-    for i_iter in range(max_iter):
+    for _ in range(max_iter):
         alpha = np.random.random()
         S = _construct_greedy_randomized_solution(reduced_graph, alpha, S)
         S = _local_search(directed_graph.copy(), S)
         compare_set = next(iter(minfvc))
         if len(S) == len(compare_set):
             minfvc.add(frozenset(S))
         elif len(S) < len(compare_set):
@@ -98,95 +99,99 @@
 
     else:
         FVC_sets = []
         nonfvc_variables = set(directed_graph.nodes()) - minfvc
 
         num_additional_var = 0
         while num_additional_var <= max_search and len(FVC_sets) == 0:
-            for an_combo in itertools.combinations(nonfvc_variables, num_additional_var):
+            for an_combo in itertools.combinations(
+                nonfvc_variables, num_additional_var
+            ):
                 possible_fvs = minfvc.union(an_combo)
 
                 if _is_acyclic(_graph_minus(directed_graph, possible_fvs)):
                     FVC_sets.append(possible_fvs)
 
             num_additional_var += 1
 
         return FVC_sets
 
 
 def _graph_minus(graph, nodeset):
-    """
-    """
+    """ """
     newgraph = nx.DiGraph()
-    for (n1, n2) in graph.edges():
+    for n1, n2 in graph.edges():
         if n1 not in nodeset and n2 not in nodeset:
             newgraph.add_edge(n1, n2)
 
     for n in graph.nodes():
         if n not in nodeset:
             newgraph.add_node(n)
 
     return newgraph
 
 
 def _is_acyclic(graph):
-    """
-    """
+    """ """
     return nx.is_directed_acyclic_graph(graph)
 
 
 def _in0out0(directed_graph, S):
-    """
-    """
-    remove_set = set([n for n in directed_graph.nodes()
-                      if (directed_graph.in_degree(n) == 0 or directed_graph.out_degree(n) == 0)])
+    """ """
+    remove_set = set(
+        [
+            n
+            for n in directed_graph.nodes()
+            if (directed_graph.in_degree(n) == 0 or directed_graph.out_degree(n) == 0)
+        ]
+    )
     directed_graph.remove_nodes_from(remove_set)
     S = S.union(remove_set)
     return directed_graph, S, len(remove_set) == 0
 
 
 def _in1(directed_graph):
-    """
-    """
-    remove_set = set([n for n in directed_graph.nodes() if (directed_graph.in_degree(n) == 1)])
+    """ """
+    remove_set = set(
+        [n for n in directed_graph.nodes() if (directed_graph.in_degree(n) == 1)]
+    )
 
     for u in remove_set:
         v = list(directed_graph.predecessors(u))[0]
         directed_graph.add_edges_from([(v, w) for w in directed_graph.successors(u)])
     directed_graph.remove_nodes_from(remove_set)
     return directed_graph, len(remove_set) == 0
 
 
 def _out1(directed_graph):
-    """
-    """
-    remove_set = set([n for n in directed_graph.nodes() if (directed_graph.out_degree(n) == 1)])
+    """ """
+    remove_set = set(
+        [n for n in directed_graph.nodes() if (directed_graph.out_degree(n) == 1)]
+    )
 
     for u in remove_set:
         v = list(directed_graph.successors(u))[0]
         directed_graph.add_edges_from([(w, v) for w in directed_graph.predecessors(u)])
     directed_graph.remove_nodes_from(remove_set)
 
     return directed_graph, len(remove_set) == 0
 
 
 def _selfloop(directed_graph, S):
-    """
-    """
+    """ """
     remove_set = list(nx.nodes_with_selfloops(directed_graph))
 
     S = S.union(set(remove_set))
 
     directed_graph.remove_nodes_from(remove_set)
     return directed_graph, S, len(remove_set) == 0
 
 
 def _reduce_instance_size(directed_graph, S):
-    """
-    """
+    """ """
     all_done = False
 
     while not all_done:
         all_done = True
 
         reduced_graph, S, no_change = _selfloop(directed_graph, S)
         all_done *= no_change
@@ -200,43 +205,42 @@
         reduced_graph, no_change = _out1(reduced_graph)
         all_done *= no_change
 
     return reduced_graph, S
 
 
 def _restricted_candidate_list(directed_graph, alpha):
-    """
-    """
+    """ """
     nodelist = directed_graph.nodes()
 
-    G = np.multiply(directed_graph.in_degree(nodelist), directed_graph.out_degree(nodelist))
+    G = np.multiply(
+        directed_graph.in_degree(nodelist), directed_graph.out_degree(nodelist)
+    )
     Gmin = min(G)
     Gmax = max(G)
 
     return np.array(nodelist)[G >= (Gmin + alpha * (Gmax - Gmin))]
 
 
 def _construct_greedy_randomized_solution(directed_graph, alpha, S):
-    """"
-    """
+    """ " """
     reduced_graph, S = _reduce_instance_size(directed_graph, S)
 
     while len(reduced_graph) > 0:
         RCL = set(_restricted_candidate_list(reduced_graph, alpha))
         s = np.random.choice(RCL)
         S.add(s)
         reduced_graph.remove_node(s)
         reduced_graph, S = _reduce_instance_size(reduced_graph, S)
 
     return S
 
 
 def _local_search(directed_graph, S):
-    """
-    """
+    """ """
     keep_going = True
 
     while keep_going:
         keep_going = False
         for localnode in S:
             remove_set = S.copy()
             remove_set.discard(localnode)
@@ -247,11 +251,16 @@
                 keep_going = True
                 break
 
     return S
 
 
 def _root_variables(directed_graph, keep_self_loops=True):
-    """
-    """
-    return set([n for n in directed_graph.nodes()
-                if (directed_graph.in_degree(n) == 0) or ((not keep_self_loops) and (directed_graph.neighbors(n) == [n]))])
+    """ """
+    return set(
+        [
+            n
+            for n in directed_graph.nodes()
+            if (directed_graph.in_degree(n) == 0)
+            or ((not keep_self_loops) and (directed_graph.neighbors(n) == [n]))
+        ]
+    )
```

### Comparing `cana-0.2.0/cana/control/mds.py` & `cana-1.0.0/cana/control/mds.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 
     if len(_get_dominated_set(directed_graph, root_var)) == N:
         return [root_var]
     else:
         MDS_sets = []
         nonroot_variables = set(directed_graph.nodes()) - set(root_var)
         for num_additional_var in range(1, max_search):
-            for an_combo in itertools.combinations(nonroot_variables, num_additional_var):
+            for an_combo in itertools.combinations(
+                nonroot_variables, num_additional_var
+            ):
                 possible_dvs = root_var.union(an_combo)
                 if len(_get_dominated_set(directed_graph, possible_dvs)) == N:
                     MDS_sets.append(possible_dvs)
             if len(MDS_sets) > 0:
                 break
         return MDS_sets
 
@@ -51,11 +53,16 @@
     dominatedset = set(dominatingset)
     for dn in dominatingset:
         dominatedset.update(directed_graph.neighbors(dn))
     return dominatedset
 
 
 def _root_variables(directed_graph, keep_self_loops=True):
-    """
-    """
-    return set([n for n in directed_graph.nodes()
-                if (directed_graph.in_degree(n) == 0) or ((not keep_self_loops) and (directed_graph.neighbors(n) == [n]))])
+    """ """
+    return set(
+        [
+            n
+            for n in directed_graph.nodes()
+            if (directed_graph.in_degree(n) == 0)
+            or ((not keep_self_loops) and (directed_graph.neighbors(n) == [n]))
+        ]
+    )
```

### Comparing `cana-0.2.0/cana/control/sc.py` & `cana-1.0.0/cana/control/sc.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,26 @@
     Returns:
         (list) : A list of sets with the driver nodes.
 
     See also:
         If you only need the size of the set, see :func:`sc_min_size`.
     """
     # get the bipartite represenation of the directed graph
-    bipartite_graph, vertex_out, vertex_in = _directed_to_bipartite(directed_graph, keep_self_loops=keep_self_loops)
+    bipartite_graph, vertex_out, vertex_in = _directed_to_bipartite(
+        directed_graph, keep_self_loops=keep_self_loops
+    )
 
     # do the maximum matching on the bipartite representation
-    max_matching = nx.bipartite.hopcroft_karp_matching(bipartite_graph, top_nodes=vertex_out)
-
-    all_max_matchings = _enumerate_maximum_matchings(bipartite_graph, vertex_out, vertex_in, max_matching)
+    max_matching = nx.bipartite.hopcroft_karp_matching(
+        bipartite_graph, top_nodes=vertex_out
+    )
+
+    all_max_matchings = _enumerate_maximum_matchings(
+        bipartite_graph, vertex_out, vertex_in, max_matching
+    )
 
     sc_sets = []
     for M in all_max_matchings:
         # find the vertex set whose in-coming vertices were matched
         matched_incoming = set(vertex_in) & set(M.keys())
         matched_original_vertices = set([sink[0] for sink in matched_incoming])
         new_dv_set = sorted(set(directed_graph.nodes()) - matched_original_vertices)
@@ -59,15 +65,17 @@
     Returns:
         (int) : The number of driver variables necessary to render the graph structurally controlled.
 
     See also:
         :func:`sc`
     """
     # get the bipartite represenation of the directed graph
-    bipartite_graph, vertex_out, vertex_in = _directed_to_bipartite(directed_graph, keep_self_loops=keep_self_loops)
+    bipartite_graph, _, vertex_in = _directed_to_bipartite(
+        directed_graph, keep_self_loops=keep_self_loops
+    )
 
     # do the maximum matching on the bipartite representation
     max_matching = nx.bipartite.hopcroft_karp_matching(bipartite_graph)
 
     # find the vertex set whose in-coming vertices were matched
     matched_incoming = set(vertex_in) & set(max_matching.keys())
     matched_original_vertices = set([sink[0] for sink in matched_incoming])
@@ -107,15 +115,15 @@
     bipartite_graph.add_nodes_from(vertex_in, bipartite=1)
 
     # add the edges
     for n in directed_graph.nodes():
         for v in directed_graph.successors(n):
             if keep_self_loops:
                 bipartite_graph.add_edge((n, True), (v, False))
-            elif (n != v):
+            elif n != v:
                 bipartite_graph.add_edge((n, True), (v, False))
 
     return bipartite_graph, vertex_out, vertex_in
 
 
 def _bipartite_to_directed(bipartite_graph):
     """Recover the directed graph from its bipartite representation.
@@ -149,15 +157,17 @@
         Could not find the original paper to cite here.
     """
     # this is the first matching in our list
     matchings_list = [max_matching]
 
     D = _make_matching_digraph(bipartite_graph, vertex_out, vertex_in, max_matching)
     D = _trim_unnecessary_edges(D)
-    matchings_list = _enumerate_maximum_matchings_iter(bipartite_graph, vertex_out, vertex_in, max_matching, D, matchings_list)
+    matchings_list = _enumerate_maximum_matchings_iter(
+        bipartite_graph, vertex_out, vertex_in, max_matching, D, matchings_list
+    )
 
     return matchings_list
 
 
 def _make_matching_digraph(bipartite_graph, U, V, M):
     """
     @@@ Uno (1999) ???
@@ -183,29 +193,28 @@
                 # otherwise, place a directed edge from V to U
                 matching_digraph.add_edge(v, u)
 
     return matching_digraph
 
 
 def _trim_unnecessary_edges(matching_digraph):
-    """
-    """
-    scc_subgraphs = [matching_digraph.subgraph(scc) for scc in nx.strongly_connected_components(matching_digraph)]
+    """ """
+    scc_subgraphs = [
+        matching_digraph.subgraph(scc)
+        for scc in nx.strongly_connected_components(matching_digraph)
+    ]
     trimmed_graph = scc_subgraphs[0]
     for next_subgraph in scc_subgraphs[1:]:
         trimmed_graph = nx.union(trimmed_graph, next_subgraph)
     return trimmed_graph
 
 
 def _enumerate_maximum_matchings_iter(G, U, V, M, D, matchings_list):
-    """
-
-    """
+    """ """
     if len(G) > 0 and not (D is None):
-
         # find the cycles in the matching digraph
         cycles = [c for c in nx.simple_cycles(D)]
 
         if len(cycles) > 0:
             # swap the edges in the cycle
             e, Mprime = _swap_edges_in_cycle(cycles[0], M)
             # this creates a new maximum matching, see if we already have it or add it
@@ -213,50 +222,59 @@
                 matchings_list.append(Mprime)
 
             # now we have two subpromblems which result in new iterations
             # Problem plus:
             Gplus, Uplus, Vplus, Mplus = _make_graph_plus(G, U, V, M, e)
             Dplus = _make_matching_digraph(Gplus, Uplus, Vplus, Mplus)
             Dplus = _trim_unnecessary_edges(Dplus)
-            matchings_list = _enumerate_maximum_matchings_iter(Gplus, Uplus, Vplus, Mplus, Dplus, matchings_list)
+            matchings_list = _enumerate_maximum_matchings_iter(
+                Gplus, Uplus, Vplus, Mplus, Dplus, matchings_list
+            )
 
             # and Problem minus:
             Gminus = _make_graph_minus(G, e)
             Dminus = _make_matching_digraph(Gminus, U, V, Mprime)
             Dminus = _trim_unnecessary_edges(Dminus)
-            matchings_list = _enumerate_maximum_matchings_iter(Gminus, U, V, Mprime, Dminus, matchings_list)
+            matchings_list = _enumerate_maximum_matchings_iter(
+                Gminus, U, V, Mprime, Dminus, matchings_list
+            )
 
         else:
             # if there are no cycles call the iter again without the matching digraph
-            matchings_list = _enumerate_maximum_matchings_iter(G, U, V, M, None, matchings_list)
+            matchings_list = _enumerate_maximum_matchings_iter(
+                G, U, V, M, None, matchings_list
+            )
 
     elif len(G) > 0:
         path = _find_path_length_two(G, V, M)
         if not (path is None):
             # swap edges in the path
             e, Mprime = _swap_edges_in_path(path, M)
             # this creates a new maximum matching, see if we already have it or add it
             if Mprime not in matchings_list:
                 matchings_list.append(Mprime)
 
             # now we have two subpromblems which result in new iterations
             # Problem plus:
             Gplus, Uplus, Vplus, Mplus = _make_graph_plus(G, U, V, M, e)
-            matchings_list = _enumerate_maximum_matchings_iter(Gplus, Uplus, Vplus, Mprime, None, matchings_list)
+            matchings_list = _enumerate_maximum_matchings_iter(
+                Gplus, Uplus, Vplus, Mprime, None, matchings_list
+            )
 
             # Problem minus with M:
             Gminus = _make_graph_minus(G, e)
-            matchings_list = _enumerate_maximum_matchings_iter(Gminus, U, V, M, None, matchings_list)
+            matchings_list = _enumerate_maximum_matchings_iter(
+                Gminus, U, V, M, None, matchings_list
+            )
 
     return matchings_list
 
 
 def _make_graph_plus(G, U, V, M, e):
-    """
-    """
+    """ """
     Gplus = G.copy()
     # remove the two endpoints and all adjacent edges
     Gplus.remove_node(e[0])
     Gplus.remove_node(e[1])
 
     Uplus = set(U)
     Vplus = set(V)
@@ -269,45 +287,41 @@
 
     Mplus = dict(M)
 
     return Gplus, Uplus, Vplus, Mplus
 
 
 def _make_graph_minus(G, e):
-    """
-    """
+    """ """
     Gminus = G.copy()
     # remove the edge
     Gminus.remove_edge(e[0], e[1])
 
     return Gminus
 
 
 def _find_path_length_two(G, V, M):
-    """
-    """
+    """ """
     path = None
     for v in _listminus(V, M.keys()):
         for u in G.neighbors(v):
             for w in G.neighbors(u):
                 if w in M and M[w] == u:
                     path = [v, u, w]
                     break
     return path
 
 
 def _listminus(list1, list2):
-    """
-    """
+    """ """
     return [a for a in list1 if a not in list2]
 
 
 def _swap_edges_in_cycle(cycle, M):
-    """
-    """
+    """ """
     Mprime = dict(M)
     e = None
     cycle = cycle + [cycle[0]]
     for i in range(len(cycle) - 1):
         if cycle[i] in Mprime:
             if M[cycle[i]] == cycle[i + 1]:
                 e = (cycle[i], cycle[i + 1])
@@ -317,16 +331,15 @@
                 e = (cycle[i], cycle[i - 1])
                 Mprime[cycle[i]] = cycle[i + 1]
                 Mprime[cycle[i + 1]] = Mprime[cycle[i]]
     return e, Mprime
 
 
 def _swap_edges_in_path(path, M):
-    """
-    """
+    """ """
     Mprime = dict(M)
     e = (path[2], path[1])
     m = Mprime[path[2]]
     del Mprime[path[2]]
     del Mprime[m]
     Mprime[path[0]] = path[1]
     Mprime[path[1]] = path[0]
```

### Comparing `cana-0.2.0/cana/cutils.c` & `cana-1.0.0/cana/cutils.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "cana.cutils",
         "sources": [
-            "cana/cutils.pyx"
+            "/home/BU/jrozum/Documents/github/rionbr/cana/CANA/cana/cutils.pyx"
         ]
     },
     "module_name": "cana.cutils"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -17,17 +17,17 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
-#define CYTHON_FUTURE_DIVISION 1
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -57,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -93,18 +94,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -134,18 +139,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -157,61 +211,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -320,17 +385,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -436,35 +560,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -560,18 +684,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -588,16 +712,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -719,14 +845,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -831,15 +958,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "cana/cutils.pyx",
+  "cutils.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_4cana_6cutils___pyx_scope_struct__expand_logic_line;
 
 /* "cana/cutils.pyx":237
  * 
@@ -988,21 +1115,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1043,26 +1178,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1121,28 +1256,53 @@
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
                                                int is_list, int wraparound, int boundscheck);
 
+/* StringJoin.proto */
+#if PY_MAJOR_VERSION < 3
+#define __Pyx_PyString_Join __Pyx_PyBytes_Join
+#define __Pyx_PyBaseString_Join(s, v) (PyUnicode_CheckExact(s) ? PyUnicode_Join(s, v) : __Pyx_PyBytes_Join(s, v))
+#else
+#define __Pyx_PyString_Join PyUnicode_Join
+#define __Pyx_PyBaseString_Join PyUnicode_Join
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+    #if PY_MAJOR_VERSION < 3
+    #define __Pyx_PyBytes_Join _PyString_Join
+    #else
+    #define __Pyx_PyBytes_Join _PyBytes_Join
+    #endif
+#else
+static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
+#endif
+
 /* PyNumberPow2.proto */
 #define __Pyx_PyNumber_InPlacePowerOf2(a, b, c) __Pyx__PyNumber_PowerOf2(a, b, c, 1)
 #define __Pyx_PyNumber_PowerOf2(a, b, c) __Pyx__PyNumber_PowerOf2(a, b, c, 0)
 static PyObject* __Pyx__PyNumber_PowerOf2(PyObject *two, PyObject *exp, PyObject *none, int inplace);
 
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* StrEquals.proto */
+#if PY_MAJOR_VERSION >= 3
+#define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
+#else
+#define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
+#endif
+
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
@@ -1495,14 +1655,15 @@
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_ipin[] = "ipin";
 static const char __pyx_k_ireg[] = "ireg";
 static const char __pyx_k_iter[] = "__iter__";
 static const char __pyx_k_ivar[] = "ivar";
+static const char __pyx_k_join[] = "join";
 static const char __pyx_k_line[] = "line";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_close[] = "close";
@@ -1527,23 +1688,23 @@
 static const char __pyx_k_binstate[] = "binstate";
 static const char __pyx_k_flip_bit[] = "flip_bit";
 static const char __pyx_k_statenum[] = "statenum";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_binstate1[] = "binstate1";
 static const char __pyx_k_binstate2[] = "binstate2";
 static const char __pyx_k_itertools[] = "itertools";
+static const char __pyx_k_cutils_pyx[] = "cutils.pyx";
 static const char __pyx_k_pinned_var[] = "pinned_var";
 static const char __pyx_k_cana_cutils[] = "cana.cutils";
 static const char __pyx_k_insert_char[] = "_insert_char";
 static const char __pyx_k_random_seed[] = "random_seed";
 static const char __pyx_k_zip_longest[] = "zip_longest";
 static const char __pyx_k_new_binstate[] = "new_binstate";
 static const char __pyx_k_total_length[] = "total_length";
 static const char __pyx_k_recursive_map[] = "recursive_map";
-static const char __pyx_k_cana_cutils_pyx[] = "cana/cutils.pyx";
 static const char __pyx_k_pinned_binstate[] = "pinned_binstate";
 static const char __pyx_k_random_binstate[] = "random_binstate";
 static const char __pyx_k_binstate_compare[] = "binstate_compare";
 static const char __pyx_k_constantbinstate[] = "constantbinstate";
 static const char __pyx_k_hamming_distance[] = "hamming_distance";
 static const char __pyx_k_constant_template[] = "constant_template";
 static const char __pyx_k_expand_logic_line[] = "expand_logic_line";
@@ -1566,26 +1727,26 @@
 static const char __pyx_k_Binary_state_length_and_index_po[] = "Binary state '{}' length and index position '{}' mismatch.";
 static const char __pyx_k_Converts_from_binary_state_to_de[] = "Converts from binary state to density\n\n    Args:\n        binstate (string) : The binary state\n\n    Returns:\n        int\n\n    Example:\n        >>> binstate_to_density('1110')\n        >>> 3\n    ";
 static const char __pyx_k_Converts_from_state_number_to_de[] = "Converts from state number to density\n\n    Args:\n        statenum (int): The state number\n\n    Returns:\n        int: The density of ``1`` in that specific binary state number.\n\n    Example:\n        >>> statenum_to_binstate(14, base=2)\n        >>> '1110'\n        >>> statenum_to_density(14)\n        >>> 3\n    ";
 static const char __pyx_k_The_two_strings_must_have_the_sa[] = "The two strings must have the same length";
 static const char __pyx_k_This_generator_expands_a_logic_l[] = "This generator expands a logic line containing ``-`` (ie. ``00- 0`` or ``0-0 1``) to a series of logic lines containing only ``0`` and ``1``.\n\n    Args:\n        line (string) : The logic line. Format is <binary-state><space><output>.\n\n    Returns:\n        generator : a series of logic lines\n\n    Example:\n        >>> expand_logic_line('1-- 0')\n        >>> 100 0\n        >>> 101 0\n        >>> 110 0\n        >>> 111 0\n    ";
 static const char __pyx_k_expand_logic_line_locals__insert[] = "expand_logic_line.<locals>._insert_char";
 static const char __pyx_k_outputs_to_binstates_of_given_ty[] = "outputs_to_binstates_of_given_type";
-static PyObject *__pyx_kp_u_0;
-static PyObject *__pyx_kp_u_1;
-static PyObject *__pyx_kp_u_Binary_state_length_and_index_po;
+static PyObject *__pyx_kp_s_0;
+static PyObject *__pyx_kp_s_1;
+static PyObject *__pyx_kp_s_Binary_state_length_and_index_po;
 static PyObject *__pyx_kp_u_Calculates_the_hamming_distance;
 static PyObject *__pyx_kp_u_Converts_from_binary_state_to_de;
 static PyObject *__pyx_kp_u_Converts_from_state_number_to_de;
-static PyObject *__pyx_kp_u_The_two_strings_must_have_the_sa;
+static PyObject *__pyx_kp_s_The_two_strings_must_have_the_sa;
 static PyObject *__pyx_kp_u_This_generator_expands_a_logic_l;
 static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_kp_u__10;
-static PyObject *__pyx_kp_u__3;
-static PyObject *__pyx_kp_u__8;
+static PyObject *__pyx_kp_s__10;
+static PyObject *__pyx_kp_s__3;
+static PyObject *__pyx_kp_s__8;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_b0;
 static PyObject *__pyx_n_s_b1;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bin;
 static PyObject *__pyx_n_s_binstate;
 static PyObject *__pyx_n_s_binstate1;
@@ -1593,24 +1754,24 @@
 static PyObject *__pyx_n_s_binstate_compare;
 static PyObject *__pyx_n_s_binstate_pinned_to_binstate;
 static PyObject *__pyx_n_s_binstate_to_constantbinstate;
 static PyObject *__pyx_n_s_binstate_to_density;
 static PyObject *__pyx_kp_u_binstate_to_density_line_181;
 static PyObject *__pyx_n_s_binstate_to_statenum;
 static PyObject *__pyx_n_s_bit;
-static PyObject *__pyx_kp_u_bit_type_format_must_be_either;
+static PyObject *__pyx_kp_s_bit_type_format_must_be_either;
 static PyObject *__pyx_n_s_cana_cutils;
-static PyObject *__pyx_kp_s_cana_cutils_pyx;
 static PyObject *__pyx_n_s_choice;
 static PyObject *__pyx_n_s_chunks;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_constant_template;
 static PyObject *__pyx_n_s_constantbinstate;
 static PyObject *__pyx_n_s_constantbinstate_to_statenum;
+static PyObject *__pyx_kp_s_cutils_pyx;
 static PyObject *__pyx_n_s_d;
 static PyObject *__pyx_n_s_expand_logic_line;
 static PyObject *__pyx_kp_u_expand_logic_line_line_237;
 static PyObject *__pyx_n_s_expand_logic_line_locals__insert;
 static PyObject *__pyx_n_s_f;
 static PyObject *__pyx_n_s_flip_binstate_bit;
 static PyObject *__pyx_n_s_flip_bit;
@@ -1621,17 +1782,18 @@
 static PyObject *__pyx_n_s_idx;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_insert_char;
 static PyObject *__pyx_n_s_iorig;
 static PyObject *__pyx_n_s_ipin;
 static PyObject *__pyx_n_s_ireg;
 static PyObject *__pyx_n_s_istate;
-static PyObject *__pyx_n_u_iter;
+static PyObject *__pyx_n_s_iter;
 static PyObject *__pyx_n_s_itertools;
 static PyObject *__pyx_n_s_ivar;
+static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_la;
 static PyObject *__pyx_n_s_lb;
 static PyObject *__pyx_n_s_lc;
 static PyObject *__pyx_n_s_length;
 static PyObject *__pyx_n_s_line;
 static PyObject *__pyx_n_s_line1;
@@ -1801,15 +1963,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_recursive_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_f, PyObject *__pyx_v_d) {
-  PyObject *__pyx_7genexpr__pyx_v_x = NULL;
+  PyObject *__pyx_v_x = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
@@ -1829,152 +1991,144 @@
  *         d (iterable) : the iterable to which f will be applied itemwise.
  *     """
  *     return [not hasattr(x, "__iter__") and f(x) or recursive_map(f, x) for x in d]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (likely(PyList_CheckExact(__pyx_v_d)) || PyTuple_CheckExact(__pyx_v_d)) {
-      __pyx_t_2 = __pyx_v_d; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
-      __pyx_t_4 = NULL;
-    } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_d); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L5_error)
-    }
-    for (;;) {
-      if (likely(!__pyx_t_4)) {
-        if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 12, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        } else {
-          if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 12, __pyx_L5_error)
-          #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          #endif
-        }
-      } else {
-        __pyx_t_5 = __pyx_t_4(__pyx_t_2);
-        if (unlikely(!__pyx_t_5)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 12, __pyx_L5_error)
-          }
-          break;
-        }
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (likely(PyList_CheckExact(__pyx_v_d)) || PyTuple_CheckExact(__pyx_v_d)) {
+    __pyx_t_2 = __pyx_v_d; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_4 = NULL;
+  } else {
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_d); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_4)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+        #else
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-      }
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_x, __pyx_t_5);
-      __pyx_t_5 = 0;
-      __pyx_t_6 = __Pyx_HasAttr(__pyx_7genexpr__pyx_v_x, __pyx_n_u_iter); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 12, __pyx_L5_error)
-      __pyx_t_7 = (!(__pyx_t_6 != 0));
-      if (!__pyx_t_7) {
-        goto __pyx_L9_next_or;
-      } else {
-      }
-      __Pyx_INCREF(__pyx_v_f);
-      __pyx_t_9 = __pyx_v_f; __pyx_t_10 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_10);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-        }
-      }
-      __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_7genexpr__pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_7genexpr__pyx_v_x);
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 12, __pyx_L5_error)
-      if (!__pyx_t_7) {
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        #endif
       } else {
-        __Pyx_INCREF(__pyx_t_8);
-        __pyx_t_5 = __pyx_t_8;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        goto __pyx_L8_bool_binop_done;
+        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+        #else
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        #endif
       }
-      __pyx_L9_next_or:;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_recursive_map); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 12, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_10);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_11 = 1;
+    } else {
+      __pyx_t_5 = __pyx_t_4(__pyx_t_2);
+      if (unlikely(!__pyx_t_5)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 12, __pyx_L1_error)
         }
+        break;
       }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_f, __pyx_7genexpr__pyx_v_x};
-        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L5_error)
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_f, __pyx_7genexpr__pyx_v_x};
-        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L5_error)
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_8);
-      } else
-      #endif
-      {
-        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 12, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (__pyx_t_10) {
-          __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
-        }
-        __Pyx_INCREF(__pyx_v_f);
-        __Pyx_GIVEREF(__pyx_v_f);
-        PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_v_f);
-        __Pyx_INCREF(__pyx_7genexpr__pyx_v_x);
-        __Pyx_GIVEREF(__pyx_7genexpr__pyx_v_x);
-        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_7genexpr__pyx_v_x);
-        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_GOTREF(__pyx_t_5);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_x, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = __Pyx_HasAttr(__pyx_v_x, __pyx_n_s_iter); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
+    __pyx_t_7 = (!(__pyx_t_6 != 0));
+    if (!__pyx_t_7) {
+      goto __pyx_L6_next_or;
+    } else {
+    }
+    __Pyx_INCREF(__pyx_v_f);
+    __pyx_t_9 = __pyx_v_f; __pyx_t_10 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
       }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    }
+    __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_x);
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+    if (!__pyx_t_7) {
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    } else {
       __Pyx_INCREF(__pyx_t_8);
       __pyx_t_5 = __pyx_t_8;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_L8_bool_binop_done:;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 12, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      goto __pyx_L5_bool_binop_done;
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
-    goto __pyx_L11_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
-    goto __pyx_L1_error;
-    __pyx_L11_exit_scope:;
-  } /* exit inner scope */
+    __pyx_L6_next_or:;
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_recursive_map); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_10 = NULL;
+    __pyx_t_11 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __pyx_t_11 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_9)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_f, __pyx_v_x};
+      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_GOTREF(__pyx_t_8);
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_v_f, __pyx_v_x};
+      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_GOTREF(__pyx_t_8);
+    } else
+    #endif
+    {
+      __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 12, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_12);
+      if (__pyx_t_10) {
+        __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
+      }
+      __Pyx_INCREF(__pyx_v_f);
+      __Pyx_GIVEREF(__pyx_v_f);
+      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_v_f);
+      __Pyx_INCREF(__pyx_v_x);
+      __Pyx_GIVEREF(__pyx_v_x);
+      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_v_x);
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 12, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_INCREF(__pyx_t_8);
+    __pyx_t_5 = __pyx_t_8;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_L5_bool_binop_done:;
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":5
  * 
  * 
@@ -1991,15 +2145,15 @@
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("cana.cutils.recursive_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x);
+  __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cana/cutils.pyx":15
  * 
@@ -2475,15 +2629,15 @@
  *             new_binstate[istate] = binstate[ireg]
  *             ireg += 1
  *     return ''.join(new_binstate)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyUnicode_Join(__pyx_kp_u__3, __pyx_v_new_binstate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyString_Join(__pyx_kp_s__3, __pyx_v_new_binstate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":67
  * 
@@ -2580,15 +2734,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_8statenum_to_output_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_statenum, PyObject *__pyx_v_base) {
-  PyObject *__pyx_8genexpr1__pyx_v_i = NULL;
+  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -2604,119 +2758,111 @@
  *         :attr:'statenum_to_binstate'
  *     """
  *     return [int(i) for i in statenum_to_binstate(statenum, base)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_statenum_to_binstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_5 = 1;
-      }
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_statenum_to_binstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_statenum, __pyx_v_base};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_statenum, __pyx_v_base};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-    } else
-    #endif
-    {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_statenum, __pyx_v_base};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_statenum, __pyx_v_base};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  {
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_statenum);
+    __Pyx_GIVEREF(__pyx_v_statenum);
+    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_statenum);
+    __Pyx_INCREF(__pyx_v_base);
+    __Pyx_GIVEREF(__pyx_v_base);
+    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_base);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
+    __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
+    __pyx_t_8 = NULL;
+  } else {
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_8)) {
+      if (likely(PyList_CheckExact(__pyx_t_3))) {
+        if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
+      } else {
+        if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
       }
-      __Pyx_INCREF(__pyx_v_statenum);
-      __Pyx_GIVEREF(__pyx_v_statenum);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_statenum);
-      __Pyx_INCREF(__pyx_v_base);
-      __Pyx_GIVEREF(__pyx_v_base);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_base);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-      __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
-      __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L5_error)
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_8)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_8(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 108, __pyx_L5_error)
-          }
-          break;
+      __pyx_t_2 = __pyx_t_8(__pyx_t_3);
+      if (unlikely(!__pyx_t_2)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 108, __pyx_L1_error)
         }
-        __Pyx_GOTREF(__pyx_t_2);
+        break;
       }
-      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_i, __pyx_t_2);
-      __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_8genexpr1__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 108, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_i); __pyx_8genexpr1__pyx_v_i = 0;
-    goto __pyx_L8_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_i); __pyx_8genexpr1__pyx_v_i = 0;
-    goto __pyx_L1_error;
-    __pyx_L8_exit_scope:;
-  } /* exit inner scope */
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
+    __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":95
  * 
  * 
@@ -2731,15 +2877,15 @@
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("cana.cutils.statenum_to_output_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_i);
+  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cana/cutils.pyx":111
  * 
@@ -2823,15 +2969,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_10outputs_to_binstates_of_given_type(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_outputs, PyObject *__pyx_v_output, PyObject *__pyx_v_k) {
-  PyObject *__pyx_8genexpr2__pyx_v_statenum = NULL;
+  PyObject *__pyx_v_statenum = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
@@ -2849,130 +2995,122 @@
  * 
  *     """
  *     return [statenum_to_binstate(statenum, k) for statenum in range(2**k) if outputs[statenum] == output]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_v_k, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L5_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_v_k, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
+    __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
+    __pyx_t_5 = NULL;
+  } else {
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-      __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-      __pyx_t_5 = NULL;
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_5)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      } else {
+        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
     } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L5_error)
+      __pyx_t_3 = __pyx_t_5(__pyx_t_2);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 125, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
     }
+    __Pyx_XDECREF_SET(__pyx_v_statenum, __pyx_t_3);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_outputs, __pyx_v_statenum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_3, __pyx_v_output, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_5)) {
-        if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 125, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
-        } else {
-          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 125, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (__pyx_t_7) {
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_statenum_to_binstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_8 = NULL;
+      __pyx_t_9 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_8)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_9 = 1;
         }
-      } else {
-        __pyx_t_3 = __pyx_t_5(__pyx_t_2);
-        if (unlikely(!__pyx_t_3)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 125, __pyx_L5_error)
-          }
-          break;
+      }
+      #if CYTHON_FAST_PYCALL
+      if (PyFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_v_statenum, __pyx_v_k};
+        __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_GOTREF(__pyx_t_6);
+      } else
+      #endif
+      #if CYTHON_FAST_PYCCALL
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_v_statenum, __pyx_v_k};
+        __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_GOTREF(__pyx_t_6);
+      } else
+      #endif
+      {
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        if (__pyx_t_8) {
+          __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
-        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_INCREF(__pyx_v_statenum);
+        __Pyx_GIVEREF(__pyx_v_statenum);
+        PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_v_statenum);
+        __Pyx_INCREF(__pyx_v_k);
+        __Pyx_GIVEREF(__pyx_v_k);
+        PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_k);
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_statenum, __pyx_t_3);
-      __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_outputs, __pyx_8genexpr2__pyx_v_statenum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = PyObject_RichCompare(__pyx_t_3, __pyx_v_output, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 125, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 125, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (__pyx_t_7) {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_statenum_to_binstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = NULL;
-        __pyx_t_9 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-          __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-          if (likely(__pyx_t_8)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-            __Pyx_INCREF(__pyx_t_8);
-            __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_3, function);
-            __pyx_t_9 = 1;
-          }
-        }
-        #if CYTHON_FAST_PYCALL
-        if (PyFunction_Check(__pyx_t_3)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_8genexpr2__pyx_v_statenum, __pyx_v_k};
-          __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-          __Pyx_GOTREF(__pyx_t_6);
-        } else
-        #endif
-        #if CYTHON_FAST_PYCCALL
-        if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_8genexpr2__pyx_v_statenum, __pyx_v_k};
-          __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-          __Pyx_GOTREF(__pyx_t_6);
-        } else
-        #endif
-        {
-          __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          if (__pyx_t_8) {
-            __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
-          }
-          __Pyx_INCREF(__pyx_8genexpr2__pyx_v_statenum);
-          __Pyx_GIVEREF(__pyx_8genexpr2__pyx_v_statenum);
-          PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_8genexpr2__pyx_v_statenum);
-          __Pyx_INCREF(__pyx_v_k);
-          __Pyx_GIVEREF(__pyx_v_k);
-          PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_k);
-          __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_6);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 125, __pyx_L5_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      }
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_statenum); __pyx_8genexpr2__pyx_v_statenum = 0;
-    goto __pyx_L9_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_statenum); __pyx_8genexpr2__pyx_v_statenum = 0;
-    goto __pyx_L1_error;
-    __pyx_L9_exit_scope:;
-  } /* exit inner scope */
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":111
  * 
  * 
@@ -2988,15 +3126,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("cana.cutils.outputs_to_binstates_of_given_type", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_statenum);
+  __Pyx_XDECREF(__pyx_v_statenum);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cana/cutils.pyx":128
  * 
@@ -3037,33 +3175,33 @@
   /* "cana/cutils.pyx":137
  *         same as input: The flipped bit
  *     """
  *     if isinstance(bit, str):             # <<<<<<<<<<<<<<
  *         return '0' if (bit == '1') else '1'
  *     elif isinstance(bit, int) or isinstance(bit, bool):
  */
-  __pyx_t_1 = PyUnicode_Check(__pyx_v_bit); 
+  __pyx_t_1 = PyString_Check(__pyx_v_bit); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "cana/cutils.pyx":138
  *     """
  *     if isinstance(bit, str):
  *         return '0' if (bit == '1') else '1'             # <<<<<<<<<<<<<<
  *     elif isinstance(bit, int) or isinstance(bit, bool):
  *         return 0 if (bit == 1) else 1
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_bit, __pyx_kp_u_1, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyString_Equals(__pyx_v_bit, __pyx_kp_s_1, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
     if (__pyx_t_2) {
-      __Pyx_INCREF(__pyx_kp_u_0);
-      __pyx_t_3 = __pyx_kp_u_0;
+      __Pyx_INCREF(__pyx_kp_s_0);
+      __pyx_t_3 = __pyx_kp_s_0;
     } else {
-      __Pyx_INCREF(__pyx_kp_u_1);
-      __pyx_t_3 = __pyx_kp_u_1;
+      __Pyx_INCREF(__pyx_kp_s_1);
+      __pyx_t_3 = __pyx_kp_s_1;
     }
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "cana/cutils.pyx":137
  *         same as input: The flipped bit
@@ -3276,15 +3414,15 @@
     /* "cana/cutils.pyx":159
  *         """
  *     if idx + 1 > len(binstate):
  *         raise TypeError("Binary state '{}' length and index position '{}' mismatch.".format(binstate, idx))             # <<<<<<<<<<<<<<
  *     return binstate[:idx] + flip_bit(binstate[idx]) + binstate[idx + 1:]
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Binary_state_length_and_index_po, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Binary_state_length_and_index_po, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -3671,16 +3809,16 @@
   /* "cana/cutils.pyx":203
  *     """
  *     # This function is being used in the boolean_network._update_trans_func
  *     constantbinstate = ''             # <<<<<<<<<<<<<<
  *     iorig = 0
  *     for value in constant_template:
  */
-  __Pyx_INCREF(__pyx_kp_u__3);
-  __pyx_v_constantbinstate = __pyx_kp_u__3;
+  __Pyx_INCREF(__pyx_kp_s__3);
+  __pyx_v_constantbinstate = __pyx_kp_s__3;
 
   /* "cana/cutils.pyx":204
  *     # This function is being used in the boolean_network._update_trans_func
  *     constantbinstate = ''
  *     iorig = 0             # <<<<<<<<<<<<<<
  *     for value in constant_template:
  *         if value is None:
@@ -3789,15 +3927,15 @@
  *             iorig += 1
  *         else:
  *             constantbinstate += str(value)             # <<<<<<<<<<<<<<
  * 
  *     return constantbinstate
  */
     /*else*/ {
-      __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 210, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 210, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_constantbinstate, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF_SET(__pyx_v_constantbinstate, __pyx_t_4);
       __pyx_t_4 = 0;
     }
@@ -3921,15 +4059,15 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_22constantbinstate_to_statenum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_constantbinstate, PyObject *__pyx_v_constant_template) {
   PyObject *__pyx_v_binstate = NULL;
-  Py_ssize_t __pyx_8genexpr3__pyx_v_ivar;
+  Py_ssize_t __pyx_v_ivar;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -3944,35 +4082,33 @@
   /* "cana/cutils.pyx":220
  *         Documentation
  *     """
  *     binstate = ''.join([constantbinstate[ivar] for ivar in range(len(constant_template)) if constant_template[ivar] is None])             # <<<<<<<<<<<<<<
  *     return binstate_to_statenum(binstate)
  * 
  */
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyObject_Length(__pyx_v_constant_template); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
-    __pyx_t_3 = __pyx_t_2;
-    for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-      __pyx_8genexpr3__pyx_v_ivar = __pyx_t_4;
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_constant_template, __pyx_8genexpr3__pyx_v_ivar, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyObject_Length(__pyx_v_constant_template); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = __pyx_t_2;
+  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
+    __pyx_v_ivar = __pyx_t_4;
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_constant_template, __pyx_v_ivar, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = (__pyx_t_5 == Py_None);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_7 = (__pyx_t_6 != 0);
+    if (__pyx_t_7) {
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_constantbinstate, __pyx_v_ivar, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = (__pyx_t_5 == Py_None);
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 220, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_7 = (__pyx_t_6 != 0);
-      if (__pyx_t_7) {
-        __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_constantbinstate, __pyx_8genexpr3__pyx_v_ivar, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 220, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      }
     }
-  } /* exit inner scope */
-  __pyx_t_5 = PyUnicode_Join(__pyx_kp_u__3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+  }
+  __pyx_t_5 = __Pyx_PyString_Join(__pyx_kp_s__3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_binstate = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "cana/cutils.pyx":221
  *     """
@@ -4100,15 +4236,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_24random_binstate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_length, PyObject *__pyx_v_random_seed) {
-  CYTHON_UNUSED PyObject *__pyx_8genexpr4__pyx_v_bit = NULL;
+  CYTHON_UNUSED PyObject *__pyx_v_bit = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
@@ -4153,102 +4289,94 @@
  *     """
  *     random.seed(random_seed)
  *     return "".join([random.choice(['0', '1']) for bit in range(length)])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-      __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-      __pyx_t_5 = NULL;
-    } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L5_error)
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_5)) {
-        if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
-        } else {
-          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L5_error)
-          #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          #endif
-        }
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
+    __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
+    __pyx_t_5 = NULL;
+  } else {
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_5)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
       } else {
-        __pyx_t_3 = __pyx_t_5(__pyx_t_2);
-        if (unlikely(!__pyx_t_3)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 234, __pyx_L5_error)
-          }
-          break;
-        }
+        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
+        #endif
       }
-      __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_bit, __pyx_t_3);
-      __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_random); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_choice); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_INCREF(__pyx_kp_u_0);
-      __Pyx_GIVEREF(__pyx_kp_u_0);
-      PyList_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_0);
-      __Pyx_INCREF(__pyx_kp_u_1);
-      __Pyx_GIVEREF(__pyx_kp_u_1);
-      PyList_SET_ITEM(__pyx_t_6, 1, __pyx_kp_u_1);
-      __pyx_t_8 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
-        if (likely(__pyx_t_8)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-          __Pyx_INCREF(__pyx_t_8);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_7, function);
+    } else {
+      __pyx_t_3 = __pyx_t_5(__pyx_t_2);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 234, __pyx_L1_error)
         }
+        break;
       }
-      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 234, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_bit); __pyx_8genexpr4__pyx_v_bit = 0;
-    goto __pyx_L8_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_bit); __pyx_8genexpr4__pyx_v_bit = 0;
-    goto __pyx_L1_error;
-    __pyx_L8_exit_scope:;
-  } /* exit inner scope */
-  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u__3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_bit, __pyx_t_3);
+    __pyx_t_3 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_random); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_choice); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_INCREF(__pyx_kp_s_0);
+    __Pyx_GIVEREF(__pyx_kp_s_0);
+    PyList_SET_ITEM(__pyx_t_6, 0, __pyx_kp_s_0);
+    __Pyx_INCREF(__pyx_kp_s_1);
+    __Pyx_GIVEREF(__pyx_kp_s_1);
+    PyList_SET_ITEM(__pyx_t_6, 1, __pyx_kp_s_1);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":224
@@ -4266,15 +4394,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("cana.cutils.random_binstate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_bit);
+  __Pyx_XDECREF(__pyx_v_bit);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_4cana_6cutils_28generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "cana/cutils.pyx":237
@@ -4489,15 +4617,15 @@
  *             lc.append(lb[i])
  *         lc.append(la[-1])
  *         return ''.join(lc)             # <<<<<<<<<<<<<<
  * 
  *     line1, line2 = line.split()
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__3, __pyx_v_lc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__3, __pyx_v_lc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":254
  *     """
@@ -4660,15 +4788,15 @@
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u__8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__8);
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s__8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s__8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_chunks = __pyx_t_1;
   __pyx_t_1 = 0;
@@ -4760,15 +4888,15 @@
  *         for i in product(*[('0', '1')] * (len(chunks) - 1)):
  *             yield _insert_char(chunks, i) + ' ' + line2             # <<<<<<<<<<<<<<
  *     else:
  *         for i in [line]:
  */
       __pyx_t_3 = __pyx_pf_4cana_6cutils_17expand_logic_line__insert_char(__pyx_cur_scope->__pyx_v__insert_char, __pyx_cur_scope->__pyx_v_chunks, __pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_kp_u__10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_kp_s__10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_cur_scope->__pyx_v_line2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
@@ -4975,16 +5103,16 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_29binstate_compare(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_binstate1, PyObject *__pyx_v_binstate2) {
-  PyObject *__pyx_8genexpr5__pyx_v_b0 = NULL;
-  PyObject *__pyx_8genexpr5__pyx_v_b1 = NULL;
+  PyObject *__pyx_v_b0 = NULL;
+  PyObject *__pyx_v_b1 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -5002,168 +5130,158 @@
  *         c (list, bool) : a list of comparisons
  *     """
  *     return [(b0 == b1) for b0, b1 in zip_longest(binstate1, binstate2)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_zip_longest); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L5_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_zip_longest); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_binstate1, __pyx_v_binstate2};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_binstate1, __pyx_v_binstate2};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  {
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_binstate1);
+    __Pyx_GIVEREF(__pyx_v_binstate1);
+    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_binstate1);
+    __Pyx_INCREF(__pyx_v_binstate2);
+    __Pyx_GIVEREF(__pyx_v_binstate2);
+    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_binstate2);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
+    __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
+    __pyx_t_8 = NULL;
+  } else {
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_5 = 1;
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 281, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_8)) {
+      if (likely(PyList_CheckExact(__pyx_t_3))) {
+        if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 281, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
+      } else {
+        if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 281, __pyx_L1_error)
+        #else
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        #endif
       }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_binstate1, __pyx_v_binstate2};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_binstate1, __pyx_v_binstate2};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-    } else
-    #endif
-    {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    } else {
+      __pyx_t_2 = __pyx_t_8(__pyx_t_3);
+      if (unlikely(!__pyx_t_2)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 281, __pyx_L1_error)
+        }
+        break;
       }
-      __Pyx_INCREF(__pyx_v_binstate1);
-      __Pyx_GIVEREF(__pyx_v_binstate1);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_binstate1);
-      __Pyx_INCREF(__pyx_v_binstate2);
-      __Pyx_GIVEREF(__pyx_v_binstate2);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_binstate2);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-      __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
-      __pyx_t_8 = NULL;
-    } else {
-      __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 281, __pyx_L5_error)
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_8)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 281, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 281, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_8(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 281, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_2);
+    if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
+      PyObject* sequence = __pyx_t_2;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 281, __pyx_L1_error)
       }
-      if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-        PyObject* sequence = __pyx_t_2;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 281, __pyx_L5_error)
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
-        }
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_4);
-        #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      if (likely(PyTuple_CheckExact(sequence))) {
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
-        Py_ssize_t index = -1;
-        __pyx_t_9 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 281, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_10 = Py_TYPE(__pyx_t_9)->tp_iternext;
-        index = 0; __pyx_t_6 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_6);
-        index = 1; __pyx_t_4 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_4)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_4);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 281, __pyx_L5_error)
-        __pyx_t_10 = NULL;
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        goto __pyx_L9_unpacking_done;
-        __pyx_L8_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_10 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 281, __pyx_L5_error)
-        __pyx_L9_unpacking_done:;
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_b0, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_b1, __pyx_t_4);
-      __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_8genexpr5__pyx_v_b0, __pyx_8genexpr5__pyx_v_b1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L5_error)
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 281, __pyx_L5_error)
+        __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
+      }
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_4);
+      #else
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    } else {
+      Py_ssize_t index = -1;
+      __pyx_t_9 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_10 = Py_TYPE(__pyx_t_9)->tp_iternext;
+      index = 0; __pyx_t_6 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_6);
+      index = 1; __pyx_t_4 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_4);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_10 = NULL;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      goto __pyx_L6_unpacking_done;
+      __pyx_L5_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_10 = NULL;
+      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+      __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_L6_unpacking_done:;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b0); __pyx_8genexpr5__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b1); __pyx_8genexpr5__pyx_v_b1 = 0;
-    goto __pyx_L10_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b0); __pyx_8genexpr5__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b1); __pyx_8genexpr5__pyx_v_b1 = 0;
-    goto __pyx_L1_error;
-    __pyx_L10_exit_scope:;
-  } /* exit inner scope */
+    __Pyx_XDECREF_SET(__pyx_v_b0, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_b1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_b0, __pyx_v_b1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "cana/cutils.pyx":272
  * 
  * 
@@ -5179,16 +5297,16 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("cana.cutils.binstate_compare", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b0);
-  __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_b1);
+  __Pyx_XDECREF(__pyx_v_b0);
+  __Pyx_XDECREF(__pyx_v_b1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cana/cutils.pyx":284
  * 
@@ -5261,16 +5379,16 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4cana_6cutils_31hamming_distance(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s1, PyObject *__pyx_v_s2) {
-  PyObject *__pyx_8genexpr6__pyx_v_b0 = NULL;
-  PyObject *__pyx_8genexpr6__pyx_v_b1 = NULL;
+  PyObject *__pyx_v_b0 = NULL;
+  PyObject *__pyx_v_b1 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -5292,180 +5410,170 @@
  *     return sum([(b0 != b1) for b0, b1 in zip_longest(s1, s2)])
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     __pyx_t_1 = PyObject_Length(__pyx_v_s1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 298, __pyx_L1_error)
     __pyx_t_2 = PyObject_Length(__pyx_v_s2); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 298, __pyx_L1_error)
     if (unlikely(!((__pyx_t_1 == __pyx_t_2) != 0))) {
-      PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_The_two_strings_must_have_the_sa);
+      PyErr_SetObject(PyExc_AssertionError, __pyx_kp_s_The_two_strings_must_have_the_sa);
       __PYX_ERR(0, 298, __pyx_L1_error)
     }
   }
   #endif
 
   /* "cana/cutils.pyx":299
  *     """
  *     assert len(s1) == len(s2), "The two strings must have the same length"
  *     return sum([(b0 != b1) for b0, b1 in zip_longest(s1, s2)])             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_zip_longest); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_7 = 1;
-      }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_5)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_s1, __pyx_v_s2};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_s1, __pyx_v_s2};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GOTREF(__pyx_t_4);
-    } else
-    #endif
-    {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      if (__pyx_t_6) {
-        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
-      }
-      __Pyx_INCREF(__pyx_v_s1);
-      __Pyx_GIVEREF(__pyx_v_s1);
-      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_s1);
-      __Pyx_INCREF(__pyx_v_s2);
-      __Pyx_GIVEREF(__pyx_v_s2);
-      PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_s2);
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_zip_longest); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_7 = 1;
     }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
-      __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_2 = 0;
-      __pyx_t_9 = NULL;
-    } else {
-      __pyx_t_2 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_9 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L5_error)
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_s1, __pyx_v_s2};
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_s1, __pyx_v_s2};
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  {
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (__pyx_t_6) {
+      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_9)) {
-        if (likely(PyList_CheckExact(__pyx_t_5))) {
-          if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_5)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 299, __pyx_L5_error)
-          #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          #endif
-        } else {
-          if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 299, __pyx_L5_error)
-          #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          #endif
-        }
-      } else {
-        __pyx_t_4 = __pyx_t_9(__pyx_t_5);
-        if (unlikely(!__pyx_t_4)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 299, __pyx_L5_error)
-          }
-          break;
-        }
+    __Pyx_INCREF(__pyx_v_s1);
+    __Pyx_GIVEREF(__pyx_v_s1);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_s1);
+    __Pyx_INCREF(__pyx_v_s2);
+    __Pyx_GIVEREF(__pyx_v_s2);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_s2);
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
+    __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_2 = 0;
+    __pyx_t_9 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_9 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_9)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_5)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 299, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-      }
-      if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
-        PyObject* sequence = __pyx_t_4;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 299, __pyx_L5_error)
-        }
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
-        }
-        __Pyx_INCREF(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_6);
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 299, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 299, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
         #endif
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_9(__pyx_t_5);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 299, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
+      PyObject* sequence = __pyx_t_4;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 299, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      if (likely(PyTuple_CheckExact(sequence))) {
+        __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
-        Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 299, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
-        index = 0; __pyx_t_8 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_8)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_8);
-        index = 1; __pyx_t_6 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_6);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 299, __pyx_L5_error)
-        __pyx_t_11 = NULL;
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        goto __pyx_L9_unpacking_done;
-        __pyx_L8_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __pyx_t_11 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 299, __pyx_L5_error)
-        __pyx_L9_unpacking_done:;
-      }
-      __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_b0, __pyx_t_8);
-      __pyx_t_8 = 0;
-      __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_b1, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __pyx_t_4 = PyObject_RichCompare(__pyx_8genexpr6__pyx_v_b0, __pyx_8genexpr6__pyx_v_b1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L5_error)
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 299, __pyx_L5_error)
+        __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
+      }
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_6);
+      #else
+      __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 299, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      #endif
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b0); __pyx_8genexpr6__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b1); __pyx_8genexpr6__pyx_v_b1 = 0;
-    goto __pyx_L10_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b0); __pyx_8genexpr6__pyx_v_b0 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b1); __pyx_8genexpr6__pyx_v_b1 = 0;
-    goto __pyx_L1_error;
-    __pyx_L10_exit_scope:;
-  } /* exit inner scope */
+    } else {
+      Py_ssize_t index = -1;
+      __pyx_t_10 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 299, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
+      index = 0; __pyx_t_8 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_8)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_8);
+      index = 1; __pyx_t_6 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_6);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+      __pyx_t_11 = NULL;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      goto __pyx_L6_unpacking_done;
+      __pyx_L5_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_11 = NULL;
+      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+      __PYX_ERR(0, 299, __pyx_L1_error)
+      __pyx_L6_unpacking_done:;
+    }
+    __Pyx_XDECREF_SET(__pyx_v_b0, __pyx_t_8);
+    __pyx_t_8 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_b1, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_b0, __pyx_v_b1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
@@ -5484,16 +5592,16 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("cana.cutils.hamming_distance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b0);
-  __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_b1);
+  __Pyx_XDECREF(__pyx_v_b0);
+  __Pyx_XDECREF(__pyx_v_b1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static struct __pyx_obj_4cana_6cutils___pyx_scope_struct__expand_logic_line *__pyx_freelist_4cana_6cutils___pyx_scope_struct__expand_logic_line[8];
 static int __pyx_freecount_4cana_6cutils___pyx_scope_struct__expand_logic_line = 0;
@@ -5613,20 +5721,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -5667,26 +5778,26 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 1, 0, 0},
-  {&__pyx_kp_u_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 1, 0, 0},
-  {&__pyx_kp_u_Binary_state_length_and_index_po, __pyx_k_Binary_state_length_and_index_po, sizeof(__pyx_k_Binary_state_length_and_index_po), 0, 1, 0, 0},
+  {&__pyx_kp_s_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 0, 1, 0},
+  {&__pyx_kp_s_Binary_state_length_and_index_po, __pyx_k_Binary_state_length_and_index_po, sizeof(__pyx_k_Binary_state_length_and_index_po), 0, 0, 1, 0},
   {&__pyx_kp_u_Calculates_the_hamming_distance, __pyx_k_Calculates_the_hamming_distance, sizeof(__pyx_k_Calculates_the_hamming_distance), 0, 1, 0, 0},
   {&__pyx_kp_u_Converts_from_binary_state_to_de, __pyx_k_Converts_from_binary_state_to_de, sizeof(__pyx_k_Converts_from_binary_state_to_de), 0, 1, 0, 0},
   {&__pyx_kp_u_Converts_from_state_number_to_de, __pyx_k_Converts_from_state_number_to_de, sizeof(__pyx_k_Converts_from_state_number_to_de), 0, 1, 0, 0},
-  {&__pyx_kp_u_The_two_strings_must_have_the_sa, __pyx_k_The_two_strings_must_have_the_sa, sizeof(__pyx_k_The_two_strings_must_have_the_sa), 0, 1, 0, 0},
+  {&__pyx_kp_s_The_two_strings_must_have_the_sa, __pyx_k_The_two_strings_must_have_the_sa, sizeof(__pyx_k_The_two_strings_must_have_the_sa), 0, 0, 1, 0},
   {&__pyx_kp_u_This_generator_expands_a_logic_l, __pyx_k_This_generator_expands_a_logic_l, sizeof(__pyx_k_This_generator_expands_a_logic_l), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-  {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
+  {&__pyx_kp_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 0},
+  {&__pyx_kp_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 0},
+  {&__pyx_kp_s__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 0, 1, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_b0, __pyx_k_b0, sizeof(__pyx_k_b0), 0, 0, 1, 1},
   {&__pyx_n_s_b1, __pyx_k_b1, sizeof(__pyx_k_b1), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bin, __pyx_k_bin, sizeof(__pyx_k_bin), 0, 0, 1, 1},
   {&__pyx_n_s_binstate, __pyx_k_binstate, sizeof(__pyx_k_binstate), 0, 0, 1, 1},
   {&__pyx_n_s_binstate1, __pyx_k_binstate1, sizeof(__pyx_k_binstate1), 0, 0, 1, 1},
@@ -5694,24 +5805,24 @@
   {&__pyx_n_s_binstate_compare, __pyx_k_binstate_compare, sizeof(__pyx_k_binstate_compare), 0, 0, 1, 1},
   {&__pyx_n_s_binstate_pinned_to_binstate, __pyx_k_binstate_pinned_to_binstate, sizeof(__pyx_k_binstate_pinned_to_binstate), 0, 0, 1, 1},
   {&__pyx_n_s_binstate_to_constantbinstate, __pyx_k_binstate_to_constantbinstate, sizeof(__pyx_k_binstate_to_constantbinstate), 0, 0, 1, 1},
   {&__pyx_n_s_binstate_to_density, __pyx_k_binstate_to_density, sizeof(__pyx_k_binstate_to_density), 0, 0, 1, 1},
   {&__pyx_kp_u_binstate_to_density_line_181, __pyx_k_binstate_to_density_line_181, sizeof(__pyx_k_binstate_to_density_line_181), 0, 1, 0, 0},
   {&__pyx_n_s_binstate_to_statenum, __pyx_k_binstate_to_statenum, sizeof(__pyx_k_binstate_to_statenum), 0, 0, 1, 1},
   {&__pyx_n_s_bit, __pyx_k_bit, sizeof(__pyx_k_bit), 0, 0, 1, 1},
-  {&__pyx_kp_u_bit_type_format_must_be_either, __pyx_k_bit_type_format_must_be_either, sizeof(__pyx_k_bit_type_format_must_be_either), 0, 1, 0, 0},
+  {&__pyx_kp_s_bit_type_format_must_be_either, __pyx_k_bit_type_format_must_be_either, sizeof(__pyx_k_bit_type_format_must_be_either), 0, 0, 1, 0},
   {&__pyx_n_s_cana_cutils, __pyx_k_cana_cutils, sizeof(__pyx_k_cana_cutils), 0, 0, 1, 1},
-  {&__pyx_kp_s_cana_cutils_pyx, __pyx_k_cana_cutils_pyx, sizeof(__pyx_k_cana_cutils_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
   {&__pyx_n_s_chunks, __pyx_k_chunks, sizeof(__pyx_k_chunks), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_constant_template, __pyx_k_constant_template, sizeof(__pyx_k_constant_template), 0, 0, 1, 1},
   {&__pyx_n_s_constantbinstate, __pyx_k_constantbinstate, sizeof(__pyx_k_constantbinstate), 0, 0, 1, 1},
   {&__pyx_n_s_constantbinstate_to_statenum, __pyx_k_constantbinstate_to_statenum, sizeof(__pyx_k_constantbinstate_to_statenum), 0, 0, 1, 1},
+  {&__pyx_kp_s_cutils_pyx, __pyx_k_cutils_pyx, sizeof(__pyx_k_cutils_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 1, 1},
   {&__pyx_n_s_expand_logic_line, __pyx_k_expand_logic_line, sizeof(__pyx_k_expand_logic_line), 0, 0, 1, 1},
   {&__pyx_kp_u_expand_logic_line_line_237, __pyx_k_expand_logic_line_line_237, sizeof(__pyx_k_expand_logic_line_line_237), 0, 1, 0, 0},
   {&__pyx_n_s_expand_logic_line_locals__insert, __pyx_k_expand_logic_line_locals__insert, sizeof(__pyx_k_expand_logic_line_locals__insert), 0, 0, 1, 1},
   {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
   {&__pyx_n_s_flip_binstate_bit, __pyx_k_flip_binstate_bit, sizeof(__pyx_k_flip_binstate_bit), 0, 0, 1, 1},
   {&__pyx_n_s_flip_bit, __pyx_k_flip_bit, sizeof(__pyx_k_flip_bit), 0, 0, 1, 1},
@@ -5722,17 +5833,18 @@
   {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_insert_char, __pyx_k_insert_char, sizeof(__pyx_k_insert_char), 0, 0, 1, 1},
   {&__pyx_n_s_iorig, __pyx_k_iorig, sizeof(__pyx_k_iorig), 0, 0, 1, 1},
   {&__pyx_n_s_ipin, __pyx_k_ipin, sizeof(__pyx_k_ipin), 0, 0, 1, 1},
   {&__pyx_n_s_ireg, __pyx_k_ireg, sizeof(__pyx_k_ireg), 0, 0, 1, 1},
   {&__pyx_n_s_istate, __pyx_k_istate, sizeof(__pyx_k_istate), 0, 0, 1, 1},
-  {&__pyx_n_u_iter, __pyx_k_iter, sizeof(__pyx_k_iter), 0, 1, 0, 1},
+  {&__pyx_n_s_iter, __pyx_k_iter, sizeof(__pyx_k_iter), 0, 0, 1, 1},
   {&__pyx_n_s_itertools, __pyx_k_itertools, sizeof(__pyx_k_itertools), 0, 0, 1, 1},
   {&__pyx_n_s_ivar, __pyx_k_ivar, sizeof(__pyx_k_ivar), 0, 0, 1, 1},
+  {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_la, __pyx_k_la, sizeof(__pyx_k_la), 0, 0, 1, 1},
   {&__pyx_n_s_lb, __pyx_k_lb, sizeof(__pyx_k_lb), 0, 0, 1, 1},
   {&__pyx_n_s_lc, __pyx_k_lc, sizeof(__pyx_k_lc), 0, 0, 1, 1},
   {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
   {&__pyx_n_s_line, __pyx_k_line, sizeof(__pyx_k_line), 0, 0, 1, 1},
   {&__pyx_n_s_line1, __pyx_k_line1, sizeof(__pyx_k_line1), 0, 0, 1, 1},
@@ -5812,241 +5924,241 @@
   /* "cana/cutils.pyx":142
  *         return 0 if (bit == 1) else 1
  *     else:
  *         raise TypeError("'bit' type format must be either 'string', 'int' or 'boolean'")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_bit_type_format_must_be_either); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_bit_type_format_must_be_either); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "cana/cutils.pyx":254
  *     """
  *     # helper function for expand_logic_line
  *     def _insert_char(la, lb):             # <<<<<<<<<<<<<<
  *         lc = []
  *         for i in range(len(lb)):
  */
   __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_la, __pyx_n_s_lb, __pyx_n_s_lc, __pyx_n_s_i); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_insert_char, 254, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_insert_char, 254, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 254, __pyx_L1_error)
 
   /* "cana/cutils.pyx":265
  *     chunks = line1.split('-')
  *     if len(chunks) > 1:
  *         for i in product(*[('0', '1')] * (len(chunks) - 1)):             # <<<<<<<<<<<<<<
  *             yield _insert_char(chunks, i) + ' ' + line2
  *     else:
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_u_0, __pyx_kp_u_1); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_s_0, __pyx_kp_s_1); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "cana/cutils.pyx":5
  * 
  * 
  * def recursive_map(f, d):             # <<<<<<<<<<<<<<
  *     """Normal python map, but recursive
  * 
  */
   __pyx_tuple__11 = PyTuple_Pack(3, __pyx_n_s_f, __pyx_n_s_d, __pyx_n_s_x); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_recursive_map, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_recursive_map, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 5, __pyx_L1_error)
 
   /* "cana/cutils.pyx":15
  * 
  * 
  * def binstate_to_statenum(binstate):             # <<<<<<<<<<<<<<
  *     """Converts from binary state to state number.
  * 
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_binstate); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_binstate_to_statenum, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_binstate_to_statenum, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 15, __pyx_L1_error)
 
   /* "cana/cutils.pyx":38
  * 
  * 
  * def statenum_to_binstate(statenum, base):             # <<<<<<<<<<<<<<
  *     """Converts an interger into the binary string.
  * 
  */
   __pyx_tuple__15 = PyTuple_Pack(2, __pyx_n_s_statenum, __pyx_n_s_base); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_statenum_to_binstate, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_statenum_to_binstate, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "cana/cutils.pyx":67
  * 
  * 
  * def binstate_pinned_to_binstate(binstate, pinned_binstate, pinned_var):             # <<<<<<<<<<<<<<
  *     """Combines two binstates based on the locations of pinned variables.
  * 
  */
   __pyx_tuple__17 = PyTuple_Pack(8, __pyx_n_s_binstate, __pyx_n_s_pinned_binstate, __pyx_n_s_pinned_var, __pyx_n_s_total_length, __pyx_n_s_new_binstate, __pyx_n_s_ipin, __pyx_n_s_ireg, __pyx_n_s_istate); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_binstate_pinned_to_binstate, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_binstate_pinned_to_binstate, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 67, __pyx_L1_error)
 
   /* "cana/cutils.pyx":95
  * 
  * 
  * def statenum_to_output_list(statenum, base):             # <<<<<<<<<<<<<<
  *     """Converts an interger into a list of 0 and 1, thus can feed to BooleanNode.from_output_list()
  * 
  */
   __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_statenum, __pyx_n_s_base, __pyx_n_s_i); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_statenum_to_output_list, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_statenum_to_output_list, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 95, __pyx_L1_error)
 
   /* "cana/cutils.pyx":111
  * 
  * 
  * def outputs_to_binstates_of_given_type(outputs, output, k):             # <<<<<<<<<<<<<<
  *     """Converts a node output list into a list of binary states given a specific output type.
  *     For instance, for the `AND` boolean function, with outputs `[0, 0, 0, 1]`
  */
   __pyx_tuple__21 = PyTuple_Pack(4, __pyx_n_s_outputs, __pyx_n_s_output, __pyx_n_s_k, __pyx_n_s_statenum); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_outputs_to_binstates_of_given_ty, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_outputs_to_binstates_of_given_ty, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 111, __pyx_L1_error)
 
   /* "cana/cutils.pyx":128
  * 
  * 
  * def flip_bit(bit):             # <<<<<<<<<<<<<<
  *     """Flips the binary value of a state.
  * 
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_s_bit); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_flip_bit, 128, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_flip_bit, 128, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 128, __pyx_L1_error)
 
   /* "cana/cutils.pyx":145
  * 
  * 
  * def flip_binstate_bit(binstate, idx):             # <<<<<<<<<<<<<<
  *     """Flips the binary value of a bit in a binary state.
  *         Args:
  */
   __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_binstate, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_flip_binstate_bit, 145, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_flip_binstate_bit, 145, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 145, __pyx_L1_error)
 
   /* "cana/cutils.pyx":163
  * 
  * 
  * def statenum_to_density(statenum):             # <<<<<<<<<<<<<<
  *     """Converts from state number to density
  * 
  */
   __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_statenum); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_statenum_to_density, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_statenum_to_density, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 163, __pyx_L1_error)
 
   /* "cana/cutils.pyx":181
  * 
  * 
  * def binstate_to_density(binstate):             # <<<<<<<<<<<<<<
  *     """Converts from binary state to density
  * 
  */
   __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_binstate); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_binstate_to_density, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_binstate_to_density, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 181, __pyx_L1_error)
 
   /* "cana/cutils.pyx":197
  * 
  * 
  * def binstate_to_constantbinstate(binstate, constant_template):             # <<<<<<<<<<<<<<
  *     """
  *     Todo:
  */
   __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_binstate, __pyx_n_s_constant_template, __pyx_n_s_constantbinstate, __pyx_n_s_iorig, __pyx_n_s_value); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_binstate_to_constantbinstate, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_binstate_to_constantbinstate, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 197, __pyx_L1_error)
 
   /* "cana/cutils.pyx":215
  * 
  * 
  * def constantbinstate_to_statenum(constantbinstate, constant_template):             # <<<<<<<<<<<<<<
  *     """
  *     Todo:
  */
   __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_constantbinstate, __pyx_n_s_constant_template, __pyx_n_s_binstate, __pyx_n_s_ivar); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_constantbinstate_to_statenum, 215, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_constantbinstate_to_statenum, 215, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 215, __pyx_L1_error)
 
   /* "cana/cutils.pyx":224
  * 
  * 
  * def random_binstate(length, random_seed=None):             # <<<<<<<<<<<<<<
  *     """Generates a random binary state of a given length
  * 
  */
   __pyx_tuple__35 = PyTuple_Pack(3, __pyx_n_s_length, __pyx_n_s_random_seed, __pyx_n_s_bit); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_random_binstate, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_random_binstate, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 224, __pyx_L1_error)
 
   /* "cana/cutils.pyx":237
  * 
  * 
  * def expand_logic_line(line):             # <<<<<<<<<<<<<<
  *     """This generator expands a logic line containing ``-`` (ie. ``00- 0`` or ``0-0 1``) to a series of logic lines containing only ``0`` and ``1``.
  * 
  */
   __pyx_tuple__37 = PyTuple_Pack(7, __pyx_n_s_line, __pyx_n_s_insert_char, __pyx_n_s_insert_char, __pyx_n_s_line1, __pyx_n_s_line2, __pyx_n_s_chunks, __pyx_n_s_i); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_expand_logic_line, 237, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_expand_logic_line, 237, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 237, __pyx_L1_error)
 
   /* "cana/cutils.pyx":272
  * 
  * 
  * def binstate_compare(binstate1, binstate2):             # <<<<<<<<<<<<<<
  *     """Compare each element in two binary states
  * 
  */
   __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_binstate1, __pyx_n_s_binstate2, __pyx_n_s_b0, __pyx_n_s_b1); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_binstate_compare, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_binstate_compare, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 272, __pyx_L1_error)
 
   /* "cana/cutils.pyx":284
  * 
  * 
  * def hamming_distance(s1, s2):             # <<<<<<<<<<<<<<
  *     """Calculates the hamming distance between two configurations strings.
  * 
  */
   __pyx_tuple__40 = PyTuple_Pack(4, __pyx_n_s_s1, __pyx_n_s_s2, __pyx_n_s_b0, __pyx_n_s_b1); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cana_cutils_pyx, __pyx_n_s_hamming_distance, 284, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cutils_pyx, __pyx_n_s_hamming_distance, 284, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -6292,15 +6404,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_cana__cutils) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6331,15 +6443,15 @@
   #endif
 
   /* "cana/cutils.pyx":1
  * import random             # <<<<<<<<<<<<<<
  * from itertools import product, zip_longest
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "cana/cutils.pyx":2
  * import random
  * from itertools import product, zip_longest             # <<<<<<<<<<<<<<
@@ -6350,15 +6462,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_product);
   __Pyx_GIVEREF(__pyx_n_s_product);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_product);
   __Pyx_INCREF(__pyx_n_s_zip_longest);
   __Pyx_GIVEREF(__pyx_n_s_zip_longest);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_zip_longest);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_itertools, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_itertools, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_product); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_product, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_zip_longest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
@@ -7312,15 +7424,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -7511,14 +7623,21 @@
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
+/* StringJoin */
+#if !CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
+    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
+}
+#endif
+
 /* PyNumberPow2 */
 static PyObject* __Pyx__PyNumber_PowerOf2(PyObject *two, PyObject *exp, PyObject *none, int inplace) {
 #if !CYTHON_COMPILING_IN_PYPY
     Py_ssize_t shiftby;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(exp))) {
         shiftby = PyInt_AS_LONG(exp);
@@ -7582,15 +7701,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -7939,28 +8058,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8497,14 +8616,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -8565,20 +8692,23 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -8626,15 +8756,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -8694,18 +8824,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
@@ -8821,15 +8949,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -8851,15 +8979,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -8945,41 +9073,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -8990,34 +9125,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -9786,14 +9936,20 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -9957,17 +10113,21 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -10747,38 +10907,63 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -11028,14 +11213,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `cana-0.2.0/cana/cutils.pyx` & `cana-1.0.0/cana/cutils.pyx`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bio.py` & `cana-1.0.0/cana/datasets/bio.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,172 +11,204 @@
 #   Alex Gates <ajgates42@gmail.com>
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Xuan Wang <xw47@indiana.edu>
 #   Thomas Parmer <tjparmer@indiana.edu>
 #   All rights reserved.
 #   MIT license.
 import os
-from .. boolean_network import BooleanNetwork
 
+from ..boolean_network import BooleanNetwork
 
 _path = os.path.dirname(os.path.realpath(__file__))
 """ Make sure we know what the current directory is """
 
 
 def THALIANA():
     """Boolean network model of the control of flower morphogenesis in Arabidopsis thaliana
 
     The network is defined in :cite:`Chaos:2006`.
 
     Returns:
         (BooleanNetwork)
     """
-    return BooleanNetwork.from_file(_path + '/thaliana.txt', name="Arabidopsis thaliana", keep_constants=True)
+    return BooleanNetwork.from_file(
+        _path + "/thaliana.txt", name="Arabidopsis thaliana", keep_constants=True
+    )
 
 
 def DROSOPHILA(cells=1):
     """Drosophila melanogaster boolean model.
     This was firt defined in :cite:`Albert:2008`.
-    Two models are available in CANA, the original parasegment (4 cells) and a single cell simplification of the model.
-    In the original parasegment model, some nodes receive inputs from neighboring cells.
-    In the single cell model, they are condensed (nhhnHH) and treated as constants.
+    Two models are available in CANA, the original parasegment (4 cells) and a
+    single cell simplification of the model. In the original parasegment model,
+    some nodes receive inputs from neighboring cells. In the single cell model,
+    they are condensed (nhhnHH) and treated as constants.
 
     Args:
         cells (int) : Which model to return. Accepts either 1 or 4. Default is 1.
 
     Returns:
         (BooleanNetwork)
     """
     if cells == 1:
-        return BooleanNetwork.from_file(_path + '/drosophila_single_cell.txt', name="Drosophila melanogaster (single cell)", keep_constants=True)
+        return BooleanNetwork.from_file(
+            _path + "/drosophila_single_cell.txt",
+            name="Drosophila melanogaster (single cell)",
+            keep_constants=True,
+        )
     elif cells == 4:
-        return BooleanNetwork.from_file(_path + '/drosophila_parasegment.txt', name='Drosophila melanogaster (parasegment)', keep_constants=True)
+        return BooleanNetwork.from_file(
+            _path + "/drosophila_parasegment.txt",
+            name="Drosophila melanogaster (parasegment)",
+            keep_constants=True,
+        )
     else:
-        raise AttributeError('Only drosophila single cell (cells=1) or parasegment (cells=4) models available.')
+        raise AttributeError(
+            "Only drosophila single cell (cells=1) or parasegment (cells=4) models available."
+        )
 
 
 def BUDDING_YEAST():
     """
 
     The network is defined in :cite:`Fangting:2004`.
 
     Returns:
         (BooleanNetwork)
     """
-    return BooleanNetwork.from_file(_path + '/yeast_cell_cycle.txt', name="Budding Yeast Cell Cycle", keep_constants=True)
+    return BooleanNetwork.from_file(
+        _path + "/yeast_cell_cycle.txt",
+        name="Budding Yeast Cell Cycle",
+        keep_constants=True,
+    )
 
 
 def MARQUESPITA():
     """Boolean network used for the Two-Symbol schemata example.
 
     The network is defined in :cite:`Marques-Pita:2013`.
 
     Returns:
         (BooleanNetwork)
     """
-    return BooleanNetwork.from_file(_path + '/marques-pita_rocha.txt', name="Marques-Pita & Rocha", keep_constants=True)
+    return BooleanNetwork.from_file(
+        _path + "/marques-pita_rocha.txt",
+        name="Marques-Pita & Rocha",
+        keep_constants=True,
+    )
 
 
 def LEUKEMIA():
     """Boolean network model of survival signaling in T-LGL leukemia
 
     The network is defined in :cite:`Zhang:2008`.
 
     Returns:
         (BooleanNetwork)
     """
-    return BooleanNetwork.from_file(_path + '/leukemia.txt', type='logical', name="T-LGL Leukemia", keep_constants=True)
+    return BooleanNetwork.from_file(
+        _path + "/leukemia.txt",
+        type="logical",
+        name="T-LGL Leukemia",
+        keep_constants=True,
+    )
 
 
 def BREAST_CANCER():
     """Boolean network model of signal transduction in ER+ breast cancer
 
     The network is defined in :cite:`Zanudo:2017`.
 
     Returns:
         (BooleanNetwork)
     """
-    return BooleanNetwork.from_file(_path + '/breast_cancer.txt', type='logical', name="ER+ Breast Cancer", keep_constants=True)
+    return BooleanNetwork.from_file(
+        _path + "/breast_cancer.txt",
+        type="logical",
+        name="ER+ Breast Cancer",
+        keep_constants=True,
+    )
 
 
 _cell_collective_models = [
-    'Apoptosis Network',
-    'Arabidopsis thaliana Cell Cycle',
-    'Aurora Kinase A in Neuroblastoma',
-    'B bronchiseptica and T retortaeformis coinfection',
-    'B cell differentiation',
-    'Bordetella bronchiseptica',
-    'Bortezomib Responses in U266 Human Myeloma Cells',
-    'BT474 Breast Cell Line Long-term ErbB Network',
-    'BT474 Breast Cell Line Short-term ErbB Network',
-    'Budding Yeast Cell Cycle 2009',
-    'Budding Yeast Cell Cycle',
-    'Cardiac development',
-    'CD4 T cell signaling',
-    'CD4+ T Cell Differentiation and Plasticity',
-    'CD4+ T cell Differentiation',
-    'Cell Cycle Transcription by Coupled CDK and Network Oscillators',
-    'Cholesterol Regulatory Pathway',
-    'Colitis-associated colon cancer',
-    'Cortical Area Development',
-    'Death Receptor Signaling',
-    'Differentiation of T lymphocytes',
-    'EGFR & ErbB Signaling',
-    'FA BRCA pathway',
-    'Fanconi anemia and checkpoint recovery',
-    'FGF pathway of Drosophila Signalling Pathways',
-    'Glucose Repression Signaling 2009',
-    'Guard Cell Abscisic Acid Signaling',
-    'HCC1954 Breast Cell Line Long-term ErbB Network',
-    'HCC1954 Breast Cell Line Short-term ErbB Network',
-    'HGF Signaling in Keratinocytes',
-    'HH Pathway of Drosophila Signaling Pathways',
-    'HIV-1 interactions with T Cell Signalling Pathway',
-    'Human Gonadal Sex Determination',
-    'IGVH mutations in chronic lymphocytic leukemia',
-    'IL-1 Signaling',
-    'IL-6 Signalling',
-    'Influenza A Virus Replication Cycle',
-    'Iron acquisition and oxidative stress response in aspergillus fumigatus',
-    'Lac Operon',
-    'Lymphoid and myeloid cell specification and transdifferentiation',
-    'Lymphopoiesis Regulatory Network',
-    'Mammalian Cell Cycle 2006',
-    'Mammalian Cell Cycle',
-    'MAPK Cancer Cell Fate Network',
-    'Metabolic Interactions in the Gut Microbiome',
-    'Neurotransmitter Signaling Pathway',
-    'Oxidative Stress Pathway',
-    'PC12 Cell Differentiation',
-    'Predicting Variabilities in Cardiac Gene',
-    'Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia',
-    'Processing of Spz Network from the Drosophila Signaling Pathway',
-    'Regulation of the L-arabinose operon of Escherichia coli',
-    'Senescence Associated Secretory Phenotype',
-    'Septation Initiation Network',
-    'Signal Transduction in Fibroblasts',
-    'Signaling in Macrophage Activation',
-    'Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598',
-    'SKBR3 Breast Cell Line Long-term ErbB Network',
-    'SKBR3 Breast Cell Line Short-term ErbB Network',
-    'Stomatal Opening Model',
-    'T cell differentiation',
-    'T Cell Receptor Signaling',
-    'T-Cell Signaling 2006',
-    'T-LGL Survival Network 2008',
-    'T-LGL Survival Network 2011 Reduced Network',
-    'T-LGL Survival Network 2011',
-    'TOL Regulatory Network',
-    'Toll Pathway of Drosophila Signaling Pathway',
-    'Treatment of Castration-Resistant Prostate Cancer',
-    'Trichostrongylus retortaeformis',
-    'Tumour Cell Invasion and Migration',
-    'VEGF Pathway of Drosophila Signaling Pathway',
-    'Wg Pathway of Drosophila Signalling Pathways',
-    'Yeast Apoptosis']
+    "Apoptosis Network",
+    "Arabidopsis thaliana Cell Cycle",
+    "Aurora Kinase A in Neuroblastoma",
+    "B bronchiseptica and T retortaeformis coinfection",
+    "B cell differentiation",
+    "Bordetella bronchiseptica",
+    "Bortezomib Responses in U266 Human Myeloma Cells",
+    "BT474 Breast Cell Line Long-term ErbB Network",
+    "BT474 Breast Cell Line Short-term ErbB Network",
+    "Budding Yeast Cell Cycle 2009",
+    "Budding Yeast Cell Cycle",
+    "Cardiac development",
+    "CD4 T cell signaling",
+    "CD4+ T Cell Differentiation and Plasticity",
+    "CD4+ T cell Differentiation",
+    "Cell Cycle Transcription by Coupled CDK and Network Oscillators",
+    "Cholesterol Regulatory Pathway",
+    "Colitis-associated colon cancer",
+    "Cortical Area Development",
+    "Death Receptor Signaling",
+    "Differentiation of T lymphocytes",
+    "EGFR & ErbB Signaling",
+    "FA BRCA pathway",
+    "Fanconi anemia and checkpoint recovery",
+    "FGF pathway of Drosophila Signalling Pathways",
+    "Glucose Repression Signaling 2009",
+    "Guard Cell Abscisic Acid Signaling",
+    "HCC1954 Breast Cell Line Long-term ErbB Network",
+    "HCC1954 Breast Cell Line Short-term ErbB Network",
+    "HGF Signaling in Keratinocytes",
+    "HH Pathway of Drosophila Signaling Pathways",
+    "HIV-1 interactions with T Cell Signalling Pathway",
+    "Human Gonadal Sex Determination",
+    "IGVH mutations in chronic lymphocytic leukemia",
+    "IL-1 Signaling",
+    "IL-6 Signalling",
+    "Influenza A Virus Replication Cycle",
+    "Iron acquisition and oxidative stress response in aspergillus fumigatus",
+    "Lac Operon",
+    "Lymphoid and myeloid cell specification and transdifferentiation",
+    "Lymphopoiesis Regulatory Network",
+    "Mammalian Cell Cycle 2006",
+    "Mammalian Cell Cycle",
+    "MAPK Cancer Cell Fate Network",
+    "Metabolic Interactions in the Gut Microbiome",
+    "Neurotransmitter Signaling Pathway",
+    "Oxidative Stress Pathway",
+    "PC12 Cell Differentiation",
+    "Predicting Variabilities in Cardiac Gene",
+    "Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia",
+    "Processing of Spz Network from the Drosophila Signaling Pathway",
+    "Regulation of the L-arabinose operon of Escherichia coli",
+    "Senescence Associated Secretory Phenotype",
+    "Septation Initiation Network",
+    "Signal Transduction in Fibroblasts",
+    "Signaling in Macrophage Activation",
+    "Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598",
+    "SKBR3 Breast Cell Line Long-term ErbB Network",
+    "SKBR3 Breast Cell Line Short-term ErbB Network",
+    "Stomatal Opening Model",
+    "T cell differentiation",
+    "T Cell Receptor Signaling",
+    "T-Cell Signaling 2006",
+    "T-LGL Survival Network 2008",
+    "T-LGL Survival Network 2011 Reduced Network",
+    "T-LGL Survival Network 2011",
+    "TOL Regulatory Network",
+    "Toll Pathway of Drosophila Signaling Pathway",
+    "Treatment of Castration-Resistant Prostate Cancer",
+    "Trichostrongylus retortaeformis",
+    "Tumour Cell Invasion and Migration",
+    "VEGF Pathway of Drosophila Signaling Pathway",
+    "Wg Pathway of Drosophila Signalling Pathways",
+    "Yeast Apoptosis",
+]
 
 
 def load_cell_collective_model(name=None):
     """Loads one of the Cell Collective :cite:`Helikar:2012` models.
     Models collected on Aug 2020.
 
     Args:
@@ -185,23 +217,29 @@
             "Wg Pathway of Drosophila Signalling Pathways", "Yeast Apoptosis"]
 
     Returns:
         (BooleanNetwork)
 
     Note:
         See source code for full list of models. Credits to Xuan Wang for compiling these models.
-        We are working on making a Cell Collective direct loader. 
+        We are working on making a Cell Collective direct loader.
     """
 
     #
     if name not in _cell_collective_models:
         models_str = "'" + "','".join(_cell_collective_models) + "'"
-        raise TypeError('Model name could not be found. Please specify one of the following models: {models:s}.'.format(models=models_str))
+        raise TypeError(
+            "Model name could not be found. Please specify one of the following models: {models:s}.".format(
+                models=models_str
+            )
+        )
     else:
-        return BooleanNetwork.from_file(_path + '/cell_collective/' + name + '.txt', name=name, keep_constants=True)
+        return BooleanNetwork.from_file(
+            _path + "/cell_collective/" + name + ".txt", name=name, keep_constants=True
+        )
 
 
 def load_all_cell_collective_models():
     """Load all the Cell Collective models, instanciating +70 models.
 
     Returns:
         (list)
```

### Comparing `cana-0.2.0/cana/datasets/bns/arabidopsis.cnet` & `cana-1.0.0/cana/datasets/bns/arabidopsis.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/budding_yeast.cnet` & `cana-1.0.0/cana/datasets/bns/budding_yeast.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/drosophila4.cnet` & `cana-1.0.0/cana/datasets/bns/drosophila4.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/fission_yeast.cnet` & `cana-1.0.0/cana/datasets/bns/fission_yeast.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/mammalian.cnet` & `cana-1.0.0/cana/datasets/bns/mammalian.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/tcr.cnet` & `cana-1.0.0/cana/datasets/bns/tcr.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bns/thelper.cnet` & `cana-1.0.0/cana/datasets/bns/thelper.cnet`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/bools.py` & `cana-1.0.0/cana/datasets/bools.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 #   Copyright (C) 2021 by
 #   Alex Gates <ajgates42@gmail.com>
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   All rights reserved.
 #   MIT license.
-from .. boolean_network import BooleanNode
+from ..boolean_network import BooleanNode
 
 
 def AND():
     """AND boolean node.
 
     .. code::
 
@@ -95,15 +95,17 @@
         011 : 1
         100 : 1
         101 : 0
         110 : 1
         111 : 0
 
     """
-    return BooleanNode.from_output_list(outputs=[0, 1, 0, 1, 1, 0, 1, 0], name="RULE 90")
+    return BooleanNode.from_output_list(
+        outputs=[0, 1, 0, 1, 1, 0, 1, 0], name="RULE 90"
+    )
 
 
 def RULE110():
     """RULE 110 celular automata node.
 
     .. code::
 
@@ -113,8 +115,10 @@
         011 : 1
         100 : 0
         101 : 1
         110 : 1
         111 : 0
 
     """
-    return BooleanNode.from_output_list(outputs=[0, 1, 1, 1, 0, 1, 1, 0], name="RULE 110")
+    return BooleanNode.from_output_list(
+        outputs=[0, 1, 1, 1, 0, 1, 1, 0], name="RULE 110"
+    )
```

### Comparing `cana-0.2.0/cana/datasets/breast_cancer.txt` & `cana-1.0.0/cana/datasets/breast_cancer.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Apoptosis Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/Apoptosis Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Arabidopsis thaliana Cell Cycle.txt` & `cana-1.0.0/cana/datasets/cell_collective/Arabidopsis thaliana Cell Cycle.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Aurora Kinase A in Neuroblastoma.txt` & `cana-1.0.0/cana/datasets/cell_collective/Aurora Kinase A in Neuroblastoma.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/B bronchiseptica and T retortaeformis coinfection.txt` & `cana-1.0.0/cana/datasets/cell_collective/B bronchiseptica and T retortaeformis coinfection.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/B cell differentiation.txt` & `cana-1.0.0/cana/datasets/cell_collective/B cell differentiation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/BT474 Breast Cell Line Long-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/BT474 Breast Cell Line Long-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/BT474 Breast Cell Line Short-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/BT474 Breast Cell Line Short-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Bordetella bronchiseptica.txt` & `cana-1.0.0/cana/datasets/cell_collective/Bordetella bronchiseptica.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Bortezomib Responses in U266 Human Myeloma Cells.txt` & `cana-1.0.0/cana/datasets/cell_collective/Bortezomib Responses in U266 Human Myeloma Cells.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle 2009.txt` & `cana-1.0.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle 2009.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle.txt` & `cana-1.0.0/cana/datasets/cell_collective/Budding Yeast Cell Cycle.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/CD4 T cell signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/CD4 T cell signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/CD4+ T Cell Differentiation and Plasticity.txt` & `cana-1.0.0/cana/datasets/cell_collective/CD4+ T Cell Differentiation and Plasticity.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/CD4+ T cell Differentiation.txt` & `cana-1.0.0/cana/datasets/cell_collective/CD4+ T cell Differentiation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Cardiac development.txt` & `cana-1.0.0/cana/datasets/cell_collective/Cardiac development.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Cell Cycle Transcription by Coupled CDK and Network Oscillators.txt` & `cana-1.0.0/cana/datasets/cell_collective/Cell Cycle Transcription by Coupled CDK and Network Oscillators.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Cholesterol Regulatory Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/Cholesterol Regulatory Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Colitis-associated colon cancer.txt` & `cana-1.0.0/cana/datasets/cell_collective/Colitis-associated colon cancer.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Death Receptor Signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/Death Receptor Signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Differentiation of T lymphocytes.txt` & `cana-1.0.0/cana/datasets/cell_collective/Differentiation of T lymphocytes.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/EGFR & ErbB Signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/EGFR & ErbB Signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/FA BRCA pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/FA BRCA pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/FGF pathway of Drosophila Signalling Pathways.txt` & `cana-1.0.0/cana/datasets/cell_collective/FGF pathway of Drosophila Signalling Pathways.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Fanconi anemia and checkpoint recovery.txt` & `cana-1.0.0/cana/datasets/cell_collective/Fanconi anemia and checkpoint recovery.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Glucose Repression Signaling 2009.txt` & `cana-1.0.0/cana/datasets/cell_collective/Glucose Repression Signaling 2009.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Guard Cell Abscisic Acid Signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/Guard Cell Abscisic Acid Signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Long-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Long-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Short-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/HCC1954 Breast Cell Line Short-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/HGF Signaling in Keratinocytes.txt` & `cana-1.0.0/cana/datasets/cell_collective/HGF Signaling in Keratinocytes.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/HH Pathway of Drosophila Signaling Pathways.txt` & `cana-1.0.0/cana/datasets/cell_collective/HH Pathway of Drosophila Signaling Pathways.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/HIV-1 interactions with T Cell Signalling Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/HIV-1 interactions with T Cell Signalling Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Human Gonadal Sex Determination.txt` & `cana-1.0.0/cana/datasets/cell_collective/Human Gonadal Sex Determination.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/IGVH mutations in chronic lymphocytic leukemia.txt` & `cana-1.0.0/cana/datasets/cell_collective/IGVH mutations in chronic lymphocytic leukemia.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/IL-1 Signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/IL-1 Signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/IL-6 Signalling.txt` & `cana-1.0.0/cana/datasets/cell_collective/IL-6 Signalling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Influenza A Virus Replication Cycle.txt` & `cana-1.0.0/cana/datasets/cell_collective/Influenza A Virus Replication Cycle.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Iron acquisition and oxidative stress response in aspergillus fumigatus.txt` & `cana-1.0.0/cana/datasets/cell_collective/Iron acquisition and oxidative stress response in aspergillus fumigatus.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Lac Operon.txt` & `cana-1.0.0/cana/datasets/cell_collective/Lac Operon.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Lymphoid and myeloid cell specification and transdifferentiation.txt` & `cana-1.0.0/cana/datasets/cell_collective/Lymphoid and myeloid cell specification and transdifferentiation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Lymphopoiesis Regulatory Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/Lymphopoiesis Regulatory Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/MAPK Cancer Cell Fate Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/MAPK Cancer Cell Fate Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Mammalian Cell Cycle 2006.txt` & `cana-1.0.0/cana/datasets/cell_collective/Mammalian Cell Cycle 2006.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Mammalian Cell Cycle.txt` & `cana-1.0.0/cana/datasets/cell_collective/Mammalian Cell Cycle.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Metabolic Interactions in the Gut Microbiome.txt` & `cana-1.0.0/cana/datasets/cell_collective/Metabolic Interactions in the Gut Microbiome.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Neurotransmitter Signaling Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/Neurotransmitter Signaling Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Oxidative Stress Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/Oxidative Stress Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/PC12 Cell Differentiation.txt` & `cana-1.0.0/cana/datasets/cell_collective/PC12 Cell Differentiation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Predicting Variabilities in Cardiac Gene.txt` & `cana-1.0.0/cana/datasets/cell_collective/Predicting Variabilities in Cardiac Gene.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia.txt` & `cana-1.0.0/cana/datasets/cell_collective/Pro-inflammatory Tumor Microenvironment in Acute Lymphoblastic Leukemia.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Processing of Spz Network from the Drosophila Signaling Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/Processing of Spz Network from the Drosophila Signaling Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Regulation of the L-arabinose operon of Escherichia coli.txt` & `cana-1.0.0/cana/datasets/cell_collective/Regulation of the L-arabinose operon of Escherichia coli.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Long-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Long-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Short-term ErbB Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/SKBR3 Breast Cell Line Short-term ErbB Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Senescence Associated Secretory Phenotype.txt` & `cana-1.0.0/cana/datasets/cell_collective/Senescence Associated Secretory Phenotype.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Septation Initiation Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/Septation Initiation Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Signal Transduction in Fibroblasts.txt` & `cana-1.0.0/cana/datasets/cell_collective/Signal Transduction in Fibroblasts.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598.txt` & `cana-1.0.0/cana/datasets/cell_collective/Signaling Pathway for Butanol Production in Clostridium beijerinckii NRRL B-598.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Signaling in Macrophage Activation.txt` & `cana-1.0.0/cana/datasets/cell_collective/Signaling in Macrophage Activation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Stomatal Opening Model.txt` & `cana-1.0.0/cana/datasets/cell_collective/Stomatal Opening Model.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T Cell Receptor Signaling.txt` & `cana-1.0.0/cana/datasets/cell_collective/T Cell Receptor Signaling.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T cell differentiation.txt` & `cana-1.0.0/cana/datasets/cell_collective/T cell differentiation.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T-Cell Signaling 2006.txt` & `cana-1.0.0/cana/datasets/cell_collective/T-Cell Signaling 2006.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2008.txt` & `cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2008.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2011 Reduced Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2011 Reduced Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/T-LGL Survival Network 2011.txt` & `cana-1.0.0/cana/datasets/cell_collective/T-LGL Survival Network 2011.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/TOL Regulatory Network.txt` & `cana-1.0.0/cana/datasets/cell_collective/TOL Regulatory Network.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Toll Pathway of Drosophila Signaling Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/Toll Pathway of Drosophila Signaling Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Treatment of Castration-Resistant Prostate Cancer.txt` & `cana-1.0.0/cana/datasets/cell_collective/Treatment of Castration-Resistant Prostate Cancer.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Trichostrongylus retortaeformis.txt` & `cana-1.0.0/cana/datasets/cell_collective/Trichostrongylus retortaeformis.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Tumour Cell Invasion and Migration.txt` & `cana-1.0.0/cana/datasets/cell_collective/Tumour Cell Invasion and Migration.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/VEGF Pathway of Drosophila Signaling Pathway.txt` & `cana-1.0.0/cana/datasets/cell_collective/VEGF Pathway of Drosophila Signaling Pathway.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Wg Pathway of Drosophila Signalling Pathways.txt` & `cana-1.0.0/cana/datasets/cell_collective/Wg Pathway of Drosophila Signalling Pathways.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/cell_collective/Yeast Apoptosis.txt` & `cana-1.0.0/cana/datasets/cell_collective/Yeast Apoptosis.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/drosophila_parasegment.txt` & `cana-1.0.0/cana/datasets/drosophila_parasegment.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/drosophila_single_cell.txt` & `cana-1.0.0/cana/datasets/drosophila_single_cell.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/leukemia.txt` & `cana-1.0.0/cana/datasets/leukemia.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/marques-pita_rocha.txt` & `cana-1.0.0/cana/datasets/marques-pita_rocha.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/motifs.py` & `cana-1.0.0/cana/datasets/motifs.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,10 +283,10 @@
 
     elif name == "4tree":
         graph.add_edge(0, 1)
         graph.add_edge(1, 2)
         graph.add_edge(1, 3)
 
     else:
-        raise TypeError('The motif name could not be found.')
+        raise TypeError("The motif name could not be found.")
 
     return graph
```

### Comparing `cana-0.2.0/cana/datasets/thaliana.txt` & `cana-1.0.0/cana/datasets/thaliana.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/datasets/yeast_cell_cycle.txt` & `cana-1.0.0/cana/datasets/yeast_cell_cycle.txt`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/cana/random_boolean_network.py` & `cana-1.0.0/cana/random_boolean_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,107 +2,135 @@
 """
 Random Boolean Network
 ======================
 
 Methods to generate random ensembles of Boolean networks.
 
 """
+import random
+import re
+
 #   Copyright (C) 2021 by
 #   Alex Gates <ajgates@indiana.edu>
 #   Rion Brattig Correia <rionbr@gmail.com>
 #   Thomas Parmer <tjparmer@indiana.edu>
 #   All rights reserved.
 #   MIT license.
-from collections import defaultdict, Counter
+from collections import Counter, defaultdict
+from io import StringIO
+
 import networkx as nx
-import random
+
 from cana.boolean_network import BooleanNetwork
-import re
-from io import StringIO
 from cana.utils import output_transitions
 
 
-def regular_boolean_network(N=10, K=2, bias=0.5, bias_constraint='soft', keep_constants=True, remove_multiedges=True, niter_remove=1000):
+def regular_boolean_network(
+    N=10,
+    K=2,
+    bias=0.5,
+    bias_constraint="soft",
+    keep_constants=True,
+    remove_multiedges=True,
+    niter_remove=1000,
+):
     """
     TODO: description
     """
     din = [K] * N  # in-degree distrubtion
     dout = [K] * N  # out-degree distrubtion
 
     regular_graph = nx.directed_configuration_model(din, dout)
 
     # the configuration graph creates a multigraph with self loops
     # the self loops are OK, but we should only have one copy of each edge
     if remove_multiedges:
-        regular_graph = _remove_duplicate_edges(graph=regular_graph, niter_remove=niter_remove)
+        regular_graph = _remove_duplicate_edges(
+            graph=regular_graph, niter_remove=niter_remove
+        )
 
     # A dict that contains the network logic {<id>:{'name':<string>,'in':<list-input-node-id>,'out':<list-output-transitions>},..}
     bn_dict = {
         node: {
-            'name': str(node),
-            'in': sorted([n for n in regular_graph.predecessors(node)]),
-            'out': random_automata_table(regular_graph.in_degree(node), bias, bias_constraint)
-        } for node in range(N)
+            "name": str(node),
+            "in": sorted([n for n in regular_graph.predecessors(node)]),
+            "out": random_automata_table(
+                regular_graph.in_degree(node), bias, bias_constraint
+            ),
+        }
+        for node in range(N)
     }
 
-    return BooleanNetwork.from_dict(bn_dict)
+    return BooleanNetwork.from_dict(bn_dict, keep_constants=keep_constants)
 
 
-def er_boolean_network(N=10, p=0.2, bias=0.5, bias_constraint='soft', remove_multiedges=True, niter_remove=1000):
+def er_boolean_network(
+    N=10,
+    p=0.2,
+    bias=0.5,
+    bias_constraint="soft",
+    remove_multiedges=True,
+    niter_remove=1000,
+):
     """
     TODO: description
     """
     er_graph = nx.erdos_renyi_graph(N, p, directed=True)
 
     # the configuration graph creates a multigraph with self loops
     # the self loops are OK, but we should only have one copy of each edge
     if remove_multiedges:
         er_graph = _remove_duplicate_edges(graph=er_graph, niter_remove=niter_remove)
 
     # A dict that contains the network logic {<id>:{'name':<string>,'in':<list-input-node-id>,'out':<list-output-transitions>},..}
     bn_dict = {
         node: {
-            'name': str(node),
-            'in': sorted([n for n in er_graph.predecessors(node)]),
-            'out': random_automata_table(er_graph.in_degree(node), bias, bias_constraint)
-        } for node in range(N)
+            "name": str(node),
+            "in": sorted([n for n in er_graph.predecessors(node)]),
+            "out": random_automata_table(
+                er_graph.in_degree(node), bias, bias_constraint
+            ),
+        }
+        for node in range(N)
     }
 
     return BooleanNetwork.from_dict(bn_dict)
 
 
-def random_automata_table(indegree, bias, bias_constraint='soft'):
+def random_automata_table(indegree, bias, bias_constraint="soft"):
     """
     TODO: description
     """
-    if bias_constraint == 'soft':
+    if bias_constraint == "soft":
         return [int(random.random() < bias) for b in range(2**indegree)]
 
-    elif bias_constraint == 'hard':
+    elif bias_constraint == "hard":
         n_ones = int(bias * (2**indegree))
         output = [0] * (2**indegree - n_ones) + [1] * n_ones
         random.shuffle(output)
         return output
 
-    elif bias_constraint == 'soft_no_constant':
+    elif bias_constraint == "soft_no_constant":
         output = [int(random.random() < bias) for b in range(2**indegree)]
         if sum(output) == 0:
             output[0] = 1
             random.shuffle(output)
         return output
 
 
 def _remove_duplicate_edges(graph, niter_remove=100):
     """
     TODO: description
     """
     edge_list = list(graph.edges())
     edge_frequency = Counter(edge_list)
 
-    duplicate_edges = [edge for edge, num_edge in edge_frequency.items() if num_edge > 1]
+    duplicate_edges = [
+        edge for edge, num_edge in edge_frequency.items() if num_edge > 1
+    ]
 
     iremove_iter = 0
     while len(duplicate_edges) > 0 and iremove_iter < niter_remove:
         for dedge in duplicate_edges:
             if edge_frequency[dedge] > 1:
                 switch_edge = random.choice(edge_list)
 
@@ -116,19 +144,24 @@
                 edge_frequency[switch_edge] -= 1
 
                 edge_frequency[(dedge[0], switch_edge[1])] += 1
                 edge_frequency[(switch_edge[0], dedge[1])] += 1
 
                 edge_list = list(graph.edges())
 
-        duplicate_edges = [edge for edge, num_edge in edge_frequency.items() if num_edge > 1]
+        duplicate_edges = [
+            edge for edge, num_edge in edge_frequency.items() if num_edge > 1
+        ]
         iremove_iter += 1
 
     if iremove_iter >= niter_remove:
-        print("Warning: multi-edges were not successfully removed after %s iterations!!" % str(iremove_iter))
+        print(
+            "Warning: multi-edges were not successfully removed after %s iterations!!"
+            % str(iremove_iter)
+        )
 
     return graph
 
 
 def from_string_boolean(self, string, keep_constants=True, **kwargs):
     """
     Instanciates a Boolean Network from a Boolean update rules format.
@@ -155,38 +188,45 @@
     logic = defaultdict(dict)
 
     # parse lines to receive node names
     network_file = StringIO(string)
     line = network_file.readline()
     i = 0
     while line != "":
-        if line[0] == '#':
+        if line[0] == "#":
             line = network_file.readline()
             continue
-        logic[i] = {
-            'name': line.split("*")[0].strip(),
-            'in': [],
-            'out': []
-        }
+        logic[i] = {"name": line.split("*")[0].strip(), "in": [], "out": []}
         line = network_file.readline()
         i += 1
 
     # Parse lines again to determine inputs and output sequence
     network_file = StringIO(string)
     line = network_file.readline()
     i = 0
     while line != "":
-        if line[0] == '#':
+        if line[0] == "#":
             line = network_file.readline()
             continue
         eval_line = line.split("=")[1]  # logical condition to evaluate
         # RE checks for non-alphanumeric character before/after node name (node names are included in other node names)
         # Additional characters added to eval_line to avoid start/end of string complications
-        input_names = [logic[node]['name'] for node in logic if re.compile('\W' + logic[node]['name'] + '\W').search('*' + eval_line + '*')]
-        input_nums = [node for input in input_names for node in logic if input == logic[node]['name']]
-        logic[i]['in'] = input_nums
+        input_names = [
+            logic[node]["name"]
+            for node in logic
+            if re.compile(r"\W" + logic[node]["name"] + r"\W").search(
+                "*" + eval_line + "*"
+            )
+        ]
+        input_nums = [
+            node
+            for input in input_names
+            for node in logic
+            if input == logic[node]["name"]
+        ]
+        logic[i]["in"] = input_nums
         # Determine output transitions
-        logic[i]['out'] = output_transitions(eval_line, input_names)
+        logic[i]["out"] = output_transitions(eval_line, input_names)
         line = network_file.readline()
         i += 1
 
     return self.from_dict(logic, keep_constants=keep_constants, **kwargs)
```

### Comparing `cana-0.2.0/cana/utils.py` & `cana-1.0.0/cana/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import networkx as nx
-import numpy as np
-from itertools import takewhile
 import copy
 import math
 import operator as op
 from functools import reduce
-from cana.cutils import *
+from itertools import takewhile
+
+import networkx as nx
+import numpy as np
+
+from cana.cutils import binstate_to_statenum, flip_binstate_bit, statenum_to_binstate
 
 
 def flip_bitset_in_strstates(strstates, idxs):
     """Flips the binary value for a set of bits in a binary state.
 
     Args:
         binstate (string) : The binary state to flip.
@@ -32,34 +34,44 @@
         binstate (string) : The binary state to flip.
         idxs (int) : The indexes of the bits to flip.
 
     Returns:
         (list) : The flipped states
     """
     flipset = []
-    if (len(idxs) != 0):
+    if len(idxs) != 0:
         fb = idxs.pop()
         flipset.extend(flip_binstate_bit_set(binstate, copy.copy(idxs)))
-        flipset.extend(flip_binstate_bit_set(flip_binstate_bit(binstate, fb), copy.copy(idxs)))
+        flipset.extend(
+            flip_binstate_bit_set(flip_binstate_bit(binstate, fb), copy.copy(idxs))
+        )
     else:
         flipset.append(binstate)
     return flipset
 
+
 def negate_LUT_input(outputs, idx):
     """For a LUT defined by the output list, it negates the input.
 
     Args:
         outputs (list) : The output list defining the LUT.
         idxs (int) : The indexes of the input to negate.
 
     Returns:
         (list) : The new output with input idx negated
     """
     k = int(np.log2(len(outputs)))
-    return [outputs[binstate_to_statenum(flip_binstate_bit(statenum_to_binstate(istate, k), idx))] for istate in range(len(outputs))]
+    return [
+        outputs[
+            binstate_to_statenum(
+                flip_binstate_bit(statenum_to_binstate(istate, k), idx)
+            )
+        ]
+        for istate in range(len(outputs))
+    ]
 
 
 def print_logic_table(outputs):
     """Print Logic Table
 
     Args:
         outputs (list) : The transition outputs of the function.
@@ -76,23 +88,23 @@
 
     """
     k = int(math.log(len(outputs)) / math.log(2))
     for statenum in range(2**k):
         print(statenum_to_binstate(statenum, base=k) + " : " + str(outputs[statenum]))
 
 
-def entropy(prob_vector, logbase=2.):
+def entropy(prob_vector, logbase=2.0):
     """Calculates the entropy given a probability vector
 
     Todo:
         This should be calculated using ``scipy.entropy``
     """
     prob_vector = np.array(prob_vector)
     pos_prob_vector = prob_vector[prob_vector > 0]
-    return - np.sum(pos_prob_vector * np.log(pos_prob_vector) / np.log(logbase))
+    return -np.sum(pos_prob_vector * np.log(pos_prob_vector) / np.log(logbase))
 
 
 def ncr(n, r):
     """Return the combination number.
     The combination of selecting `r` items from `n` iterms, order doesn't matter.
 
     Args:
@@ -157,21 +169,21 @@
             111
 
         A variable is dynamically created for each member of the input list
         and assigned the corresponding value from each trail string.
         The original eval_line is then evaluated with each assignment
         which results in the output list [0, 0, 1, 0, 1, 0, 1, 0]
     """
-    total = 2**len(input_list)  # Total combinations to try
+    total = 2 ** len(input_list)  # Total combinations to try
     output_list = []
     for i in range(total):
         trial_string = statenum_to_binstate(i, len(input_list))
         # Evaluate trial_string by assigning value to each input variable
         for j, input in enumerate(input_list):
-            exec(input + '=' + trial_string[j])
+            exec(input + "=" + trial_string[j])
         output_list.append(int(eval(eval_line)))
 
     return output_list
 
 
 def seq_upto(seq, obj):
     """
@@ -193,39 +205,39 @@
             dist[node] = min(pairs)
         else:
             dist[node] = (0, node)
 
     return dist
 
 
-def pathlength(p, weights, rule='sum'):
+def pathlength(p, weights, rule="sum"):
     """Calculate the length of path p, with weighted edges, given the length rule of:
 
     Ars:
         weights:
 
         rule (str):
             'sum' - sum of edge weights along path
             'prod' - product of edge weights along path
             'min' - minimum of edge weights along path (weakest-link)
             'max' - maximum of edge weights along path
 
     TODO: update description
     """
-    if rule == 'sum':
+    if rule == "sum":
         return sum(weights[(p[ie], p[ie + 1])] for ie in range(len(p) - 1))
-    elif rule == 'prod':
+    elif rule == "prod":
         return np.prod([weights[(p[ie], p[ie + 1])] for ie in range(len(p) - 1)])
-    elif rule == 'min':
+    elif rule == "min":
         return min(weights[(p[ie], p[ie + 1])] for ie in range(len(p) - 1))
-    elif rule == 'max':
+    elif rule == "max":
         return max(weights[(p[ie], p[ie + 1])] for ie in range(len(p) - 1))
 
 
-def function_monotone(outputs, method='exact', nsamples=100, random_seed=None):
+def function_monotone(outputs, method="exact", nsamples=100, random_seed=None):
     """
     Determine if a given LUT is monotone.
 
     Here we test every pair of inputs that are Hamming distance 1. (see Goldreich et al 2000)
 
     Args:
         outputs (list) : The transition outputs of the function.
@@ -238,28 +250,29 @@
 
     Returns:
         (Bool) : True if monotone.
 
     Example:
         >>> is_monotone(outputs=[0,0,0,1])
     """
-    random.seed(random_seed)
+    # np.random.seed(random_seed)
 
     k = int(np.log2(len(outputs)))
 
     # for all input configurations
     for input_confignum in range(2**k):
-
         input_configbin = statenum_to_binstate(input_confignum, k)
 
         # for all input states that are 0
         for idx, state in enumerate(input_configbin):
-            if state == '0':
+            if state == "0":
                 # we flip the 0 and check for monotone along the edge
-                next_confignum = binstate_to_statenum(flip_binstate_bit(input_configbin, idx))
+                next_confignum = binstate_to_statenum(
+                    flip_binstate_bit(input_configbin, idx)
+                )
 
                 # if the monotone property fails
                 if outputs[input_confignum] > outputs[next_confignum]:
                     return False
     return True
 
 
@@ -283,24 +296,34 @@
     """
 
     k = int(np.log2(len(outputs)))
 
     if k == 1:
         return True
     else:
-
         monotone_configs = []
         # for all input configurations
-        for input_confignum in range(2**(k - 1)):
-
+        for input_confignum in range(2 ** (k - 1)):
             other_input_configbin = statenum_to_binstate(input_confignum, k - 1)
 
-            input_confignum_0 = binstate_to_statenum(other_input_configbin[:input_idx] + '0' + other_input_configbin[input_idx:])
-
-            input_confignum_1 = binstate_to_statenum(other_input_configbin[:input_idx] + '1' + other_input_configbin[input_idx:])
+            input_confignum_0 = binstate_to_statenum(
+                other_input_configbin[:input_idx]
+                + "0"
+                + other_input_configbin[input_idx:]
+            )
+
+            input_confignum_1 = binstate_to_statenum(
+                other_input_configbin[:input_idx]
+                + "1"
+                + other_input_configbin[input_idx:]
+            )
 
             if activation == 1:
-                monotone_configs.append(outputs[input_confignum_0] <= outputs[input_confignum_1])
+                monotone_configs.append(
+                    outputs[input_confignum_0] <= outputs[input_confignum_1]
+                )
             elif activation == -1:
-                monotone_configs.append(outputs[input_confignum_0] >= outputs[input_confignum_1])
+                monotone_configs.append(
+                    outputs[input_confignum_0] >= outputs[input_confignum_1]
+                )
 
         return all(monotone_configs)
```

### Comparing `cana-0.2.0/cana.egg-info/PKG-INFO` & `cana-1.0.0/cana.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: cana
-Version: 0.2.0
+Version: 1.0.0
 Summary: This package implements a series of methods used to study control, canalization and redundancy in Boolean networks.
 Home-page: http://github.com/rionbr/CANA
 Author: Alex Gates & Rion Brattig Correia
 Author-email: rionbr@gmail.com
 License: MIT
 Keywords: boolean networks canalization redundancy dynamical systems computational biology
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/plain
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: schematodes>=1.0.0
 
 This package implements a series of methods used to study control, canalization and redundancy in Boolean networks.
```

### Comparing `cana-0.2.0/cana.egg-info/SOURCES.txt` & `cana-1.0.0/cana.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -117,12 +117,13 @@
 cana/datasets/cell_collective/Tumour Cell Invasion and Migration.txt
 cana/datasets/cell_collective/VEGF Pathway of Drosophila Signaling Pathway.txt
 cana/datasets/cell_collective/Wg Pathway of Drosophila Signalling Pathways.txt
 cana/datasets/cell_collective/Yeast Apoptosis.txt
 cana/drawing/__init__.py
 cana/drawing/canalizing_map.py
 cana/drawing/schema_vis.py
+tests/__init__.py
 tests/test_boolean_canalization.py
 tests/test_boolean_network.py
 tests/test_boolean_node.py
 tests/test_effectiveness_measures.py
 tests/test_two_symbol_symmetry.py
```

### Comparing `cana-0.2.0/tests/test_boolean_canalization.py` & `cana-1.0.0/tests/test_boolean_canalization.py`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/tests/test_boolean_network.py` & `cana-1.0.0/tests/test_boolean_network.py`

 * *Files identical despite different names*

### Comparing `cana-0.2.0/tests/test_boolean_node.py` & `cana-1.0.0/tests/test_boolean_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # Tests for ``boolean_node.py``
 # These tests were manually calculated by Luis M. Rocha and implemented by Rion B. Correia.
 #
 from cana.datasets.bools import CONTRADICTION, AND, OR, XOR, COPYx1, RULE90, RULE110
 from cana.utils import *
 from cana.boolean_node import BooleanNode
+import numpy as np
 
 
 #
 # Test Input Redundancy
 #
 
 def test_input_redundancy_constant():
@@ -357,232 +358,14 @@
     e_ji, true_e_ji = n.edge_effectiveness(bound='upper'), [0.25, 0.75, 0.75]
     assert (e_ji == true_e_ji), ('Input Redundancy (input,upper bound) for RULE110 node does not match. %s != %s' % (e_ji, true_e_ji))
     e_ji, true_e_ji = n.edge_effectiveness(bound='mean'), [0.375, 0.875, 0.875]
     assert (e_ji == true_e_ji), ('Input Redundancy (input,mean) for RULE110 node does not match. %s != %s' % (e_ji, true_e_ji))
     e_ji, true_e_ji = n.edge_effectiveness(bound='lower'), [0.5, 1., 1.]
     assert (e_ji == true_e_ji), ('Input Redundancy (input,lower bound) for RULE110 node does not match. %s != %s' % (e_ji, true_e_ji))
 
-
-#
-# Test Edge Symmetry
-#
-
-# AND
-def test_edge_symmetry_AND():
-    """Test Edge Symmetry - AND"""
-    n = AND()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (upper) for AND node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (mean) for AND node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (lower) for AND node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(2, 2)] * 4, [(2, 2)] * 4]
-    assert (k_s == true_k_s), ('Edge symmetry (tuples) for AND node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# OR
-def test_edge_symmetry_OR():
-    """Test Edge Symmetry - OR"""
-    n = OR()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for OR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for OR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for OR node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(2, 2)] * 4, [(2, 2)] * 4]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# XOR
-def test_edge_symmetry_XOR():
-    """Test Edge Symmetry - XOR"""
-    n = XOR()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(2, 2)] * 4, [(2, 2)] * 4]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# CONTRADICTION
-def test_edge_symmetry_CONTRADICTION():
-    """Test Edge Symmetry - CONTRADICTION"""
-    n = CONTRADICTION()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [2., 2.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(2, 2)] * 4, [(2, 2)] * 4]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# COPYx1
-def test_edge_symmetry_COPYx1():
-    """Test Edge Symmetry - COPYx1"""
-    n = COPYx1()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [0., 0.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [0., 0.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [0., 0.]
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(0, 0)] * 4, [(0, 0)] * 4]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# RULE90
-def test_edge_symmetry_RULE90():
-    """Test Edge Symmetry - RULE90"""
-    n = RULE90()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [8 / 4, 0., 8 / 4]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [8 / 4., 0., 8 / 4]
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [8 / 4., 0., 8 / 4]
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(2, 2)] * 8, [(0, 0)] * 8, [(2, 2)] * 8]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# RULE110
-def test_input_symmetry_RULE110():
-    """Test Edge Symmetry - RULE110"""
-    n = RULE110()
-    k_s, true_k_s = n.edge_symmetry(bound='upper'), [13 / 8, 17 / 8, 17 / 8]
-    assert (k_s == true_k_s), ('Input Symmetry (input,upper bound) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='mean'), [0.95833333333333326, 1.8333333333333333, 1.8333333333333333]  # NOT SURE ITS CORRECT!!!
-    assert (k_s == true_k_s), ('Input Symmetry (input,mean) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.edge_symmetry(bound='lower'), [0.375, 1.375, 1.375]  # NOT SURE ITS CORRECT!!!
-    assert (k_s == true_k_s), ('Input Symmetry (input,lower bound) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.edge_symmetry(bound='tuple'), [[(0, 0), (0, 2), (0, 2), (0, 2), (0, 0), (0, 2), (0, 2), (3, 3)], [(2, 2), (2, 2), (0, 2), (0, 2), (2, 2), (2, 2), (0, 2), (3, 3)], [(2, 2), (0, 2), (2, 2), (0, 2), (2, 2), (0, 2), (2, 2), (3, 3)]]
-    assert (k_s == true_k_s), ('Input Redundancy (input,tuples) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-
-
-#
-# Test Input Symmetry
-#
-
-# AND
-def test_input_symmetry_AND():
-    """Test Input Symmetry - AND"""
-    n = AND()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for AND node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for AND node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for AND node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for AND node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# OR
-def test_input_symmetry_OR():
-    """Test Input Symmetry - OR"""
-    n = OR()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for OR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for OR node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for OR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for OR node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# XOR
-def test_input_symmetry_XOR():
-    """Test Input Symmetry - XOR"""
-    n = XOR()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for XOR node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# CONTRADICTION
-def test_input_symmetry_CONTRADICTION():
-    """Test Input Symmetry - CONTRADICTION"""
-    n = CONTRADICTION()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 8 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (8 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for CONTRADICTION node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# COPYx1
-def test_input_symmetry_COPYx1():
-    """Test Input Symmetry - COPYx1"""
-    n = COPYx1()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 0 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 0 / 4
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (0 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (0 / 4) / 2
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for COPYx1 node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# RULE90
-def test_input_symmetry_RULE90():
-    """Test Input Symmetry - RULE90"""
-    n = RULE90()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), 4 / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), 4 / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), (4 / 3) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), (4 / 3) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for RULE90 node does not match. %s != %s' % (k_s, true_k_s))
-
-
-# RULE110
-def test_input_symmetry_RULE110():
-    """Test Input Symmetry - RULE110"""
-    n = RULE110()
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=False), (13 / 8 + 17 / 8 + 17 / 8) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=False), (3 / 8 + 11 / 8 + 11 / 8) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-
-    k_s, true_k_s = n.input_symmetry(bound='upper', norm=True), ((13 / 8 + 17 / 8 + 17 / 8) / 3) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,upper bound,normed) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-    k_s, true_k_s = n.input_symmetry(bound='lower', norm=True), ((3 / 8 + 11 / 8 + 11 / 8) / 3) / 3
-    assert (k_s == true_k_s), ('Input Symmetry (node,lower bound,normed) for RULE110 node does not match. %s != %s' % (k_s, true_k_s))
-
 #
 # Test Sensitivity
 #
 def test_sensitivity_AND():
     """Test Sensitivity - AND"""
     n = AND()
     s, true_s = n.c_sensitivity(1), 1 / 2
@@ -602,7 +385,86 @@
     assert isclose(s, true_s), ('c-sensitivity(1) for XOR does not match, %s != %s' % (s, true_s))
     s, true_s = n.c_sensitivity(2), 0.
     assert isclose(s, true_s), ('c-sensitivity(2) for XOR does not match, %s != %s' % (s, true_s))
     s, true_s = n.c_sensitivity(1, 'forceK', 3), 2 / 3
     assert isclose(s, true_s), ("c-sensitivity(1,'forceK',3) for XOR does not match, %s != %s" % (s, true_s))
     s, true_s = n.c_sensitivity(2, 'forceK', 3), 2 / 3
     assert isclose(s, true_s), ("c-sensitivity(2,'forceK',3) for XOR does not match, %s != %s" % (s, true_s))
+
+# input symmetry tests (new)
+def test_input_symmetry_AND():
+    n = AND()
+    k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots"), 3.0/2
+    assert (k_s == true_k_s), f"Input symmetry: AND (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots"), 3.0/2
+    assert (k_s == true_k_s), f"Input symmetry: AND (max): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry_mean(), 3.0/2
+    assert (k_s == true_k_s), f"Input symmetry simp: AND (mean): returned {k_s}, true value is {true_k_s}"
+
+    # k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: AND (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: AND (max, sameSymbol): returned {k_s}, true value is {true_k_s}"
+
+def test_input_symmetry_XOR():
+    n = XOR()
+    k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots"), 1.0
+    assert (k_s == true_k_s), f"Input symmetry: XOR (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry_mean(), 1.0
+    assert (k_s == true_k_s), f"Input symmetry simp: XOR (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots"), 1.0
+    assert (k_s == true_k_s), f"Input symmetry: XOR (max): returned {k_s}, true value is {true_k_s}"
+
+    # k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: XOR (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry_mean(), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry simp: XOR (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: XOR (max, sameSymbol): returned {k_s}, true value is {true_k_s}"
+
+def test_input_symmetry_COPYx1():
+    n = COPYx1()
+    k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots"), 0
+    assert (k_s == true_k_s), f"Input symmetry: COPYx1 (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry_mean(), 0
+    assert (k_s == true_k_s), f"Input symmetry simp: COPYx1 (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots"), 0
+    assert (k_s == true_k_s), f"Input symmetry: COPYx1 (max): returned {k_s}, true value is {true_k_s}"
+
+    # k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots", sameSymbol=True), 0.0
+    # assert (k_s == true_k_s), f"Input symmetry: COPYx1 (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry_mean(), 0.0
+    # assert (k_s == true_k_s), f"Input symmetry simp: COPYx1 (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 0.0
+    # assert (k_s == true_k_s), f"Input symmetry: COPYx1 (max, sameSymbol): returned {k_s}, true value is {true_k_s}"
+
+def test_input_symmetry_RULE90():
+    n = RULE90()
+    k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots"), 1.0
+    assert (k_s == true_k_s), f"Input symmetry: RULE90 (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry_mean(), 1.0
+    assert (k_s == true_k_s), f"Input symmetry simp: RULE90 (mean): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 1.0
+    assert (k_s == true_k_s), f"Input symmetry: RULE90 (max): returned {k_s}, true value is {true_k_s}"
+
+    # k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: RULE90 (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry_mean(), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry simp: RULE90 (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 2.0
+    # assert (k_s == true_k_s), f"Input symmetry: RULE90 (max, sameSymbol): returned {k_s}, true value is {true_k_s}"
+
+def test_input_symmetry_SBF():
+    n = BooleanNode(outputs=list("0111" + "0"*12), k=4)
+    k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots"), 1.6875
+    assert (k_s == true_k_s), f"Input symmetry: SBF (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry_mean(), 1.6875
+    assert (k_s == true_k_s), f"Input symmetry simp: SBF (mean): returned {k_s}, true value is {true_k_s}"
+    k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots"), 1.875
+    assert (k_s == true_k_s), f"Input symmetry: SBF (max): returned {k_s}, true value is {true_k_s}"
+
+    # k_s, true_k_s = n.input_symmetry(aggOp="mean", kernel="numDots", sameSymbol=True), 4.0
+    # assert (k_s == true_k_s), f"Input symmetry: SBF (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry_mean(), 4.0
+    # assert (k_s == true_k_s), f"Input symmetry simp: SBF (mean, sameSymbol): returned {k_s}, true value is {true_k_s}"
+    # k_s, true_k_s = n.input_symmetry(aggOp="max", kernel="numDots", sameSymbol=True), 4.0
+    # assert (k_s == true_k_s), f"Input symmetry: SBF (max, sameSymbol): returned {k_s}, true value is {true_k_s}"
```

### Comparing `cana-0.2.0/tests/test_effectiveness_measures.py` & `cana-1.0.0/tests/test_effectiveness_measures.py`

 * *Files identical despite different names*

