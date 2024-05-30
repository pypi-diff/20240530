# Comparing `tmp/BioSAK-1.88.9.tar.gz` & `tmp/BioSAK-1.89.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.88.9.tar", last modified: Thu May  9 03:17:50 2024, max compression
+gzip compressed data, was "BioSAK-1.89.0.tar", last modified: Wed May 29 06:14:43 2024, max compression
```

## Comparing `BioSAK-1.88.9.tar` & `BioSAK-1.89.0.tar`

### file list

```diff
@@ -1,168 +1,155 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.961209 BioSAK-1.88.9/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.958698 BioSAK-1.88.9/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.88.9/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.88.9/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.88.9/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.88.9/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.88.9/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.88.9/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3700 2024-05-09 03:17:49.000000 BioSAK-1.88.9/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.88.9/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38573 2024-05-08 05:20:42.000000 BioSAK-1.88.9/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.88.9/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.88.9/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.88.9/BioSAK/compare_sets.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.88.9/BioSAK/count_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.88.9/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    14152 2024-05-08 15:09:54.000000 BioSAK-1.88.9/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.88.9/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.88.9/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.88.9/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4404 2024-05-09 03:17:49.000000 BioSAK-1.88.9/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.88.9/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.88.9/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.88.9/BioSAK/gbk2gff.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.88.9/BioSAK/gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.88.9/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.88.9/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.88.9/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.88.9/BioSAK/gff2chrom.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.88.9/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.88.9/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26876 2024-05-06 12:18:36.000000 BioSAK-1.88.9/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.88.9/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.88.9/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.88.9/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.88.9/BioSAK/mannwhitneyu.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.88.9/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.88.9/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8826 2024-05-06 06:13:20.000000 BioSAK-1.88.9/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.88.9/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.88.9/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.88.9/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.88.9/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.88.9/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.88.9/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.88.9/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.88.9/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.88.9/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.88.9/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1912 2024-05-06 05:46:35.000000 BioSAK-1.88.9/BioSAK/tmp_1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.88.9/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/usearch_uc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.88.9/BioSAK/wilcox.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.960678 BioSAK-1.88.9/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3763 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.88.9/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.88.9/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-09 03:17:50.960985 BioSAK-1.88.9/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.88.9/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.959668 BioSAK-1.88.9/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    78626 2024-05-08 15:03:16.000000 BioSAK-1.88.9/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-09 03:17:50.961255 BioSAK-1.88.9/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.88.9/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-29 06:14:43.261565 BioSAK-1.89.0/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-29 06:14:43.259722 BioSAK-1.89.0/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.89.0/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.89.0/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.89.0/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.89.0/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.89.0/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.89.0/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3738 2024-05-29 06:14:41.000000 BioSAK-1.89.0/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.89.0/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38573 2024-05-08 05:20:42.000000 BioSAK-1.89.0/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.89.0/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.89.0/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.89.0/BioSAK/compare_sets.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.89.0/BioSAK/count_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.89.0/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    14172 2024-05-19 02:14:02.000000 BioSAK-1.89.0/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.89.0/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.89.0/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2995 2024-05-29 06:08:14.000000 BioSAK-1.89.0/BioSAK/fastaai.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/format_converter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4406 2024-05-09 03:22:31.000000 BioSAK-1.89.0/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.89.0/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.89.0/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.89.0/BioSAK/gbk2gff.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.89.0/BioSAK/gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.89.0/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.89.0/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.89.0/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.89.0/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.89.0/BioSAK/gff2chrom.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.89.0/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.89.0/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.89.0/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.89.0/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.89.0/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.89.0/BioSAK/mannwhitneyu.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.89.0/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.89.0/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8826 2024-05-06 06:13:20.000000 BioSAK-1.89.0/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.89.0/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.89.0/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.89.0/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.89.0/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.89.0/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.89.0/BioSAK/reads2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.89.0/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.89.0/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.89.0/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5458 2024-05-09 06:31:41.000000 BioSAK-1.89.0/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1912 2024-05-06 05:46:35.000000 BioSAK-1.89.0/BioSAK/tmp_1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.89.0/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.89.0/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.89.0/BioSAK/usearch_uc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.89.0/BioSAK/wilcox.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-29 06:14:43.261026 BioSAK-1.89.0/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-29 06:14:43.000000 BioSAK-1.89.0/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3478 2024-05-29 06:14:43.000000 BioSAK-1.89.0/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-29 06:14:43.000000 BioSAK-1.89.0/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-29 06:14:43.000000 BioSAK-1.89.0/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-29 06:14:43.000000 BioSAK-1.89.0/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.89.0/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2024-05-21 02:52:10.000000 BioSAK-1.89.0/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-29 06:14:43.261319 BioSAK-1.89.0/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.89.0/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-29 06:14:43.260624 BioSAK-1.89.0/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    72018 2024-05-29 06:14:41.000000 BioSAK-1.89.0/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-29 06:14:43.261618 BioSAK-1.89.0/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.89.0/setup.py
```

### Comparing `BioSAK-1.88.9/BioSAK/BLCA_op_parser.py` & `BioSAK-1.89.0/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/BioSAK_config.py` & `BioSAK-1.89.0/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/COG2020.py` & `BioSAK-1.89.0/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.89.0/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.89.0/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/CheckM.py` & `BioSAK-1.89.0/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.89.0/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.89.0/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.89.0/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.89.0/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/Gene2Ctg.py` & `BioSAK-1.89.0/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/KEGG.py` & `BioSAK-1.89.0/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.89.0/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.89.0/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/MeanMappingDepth.py` & `BioSAK-1.89.0/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/MetaBiosample.py` & `BioSAK-1.89.0/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.89.0/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.89.0/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/NetEnzymes.py` & `BioSAK-1.89.0/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.89.0/BioSAK/manipulator_newick.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,15 @@
                                position = 'branch-top')  # non-leaf node name text setting)
 
             each_node.set_style(nlns)
 
     tree.render(tree_output, w=900, units="px", tree_style=ts)  # set figures size
 
 
-#os.chdir('/Users/songweizhi/Desktop')
 
-tree_2 = '(CF_Refined_71:0.21847,CF_Refined_170:0.41504,(((CF_Refined_7:0.63495,CF_Refined_96:0.68718)0.984:0.33915,CF_Refined_82:0.16074)0.980:0.12012,((CF_Refined_25:0.20437,CF_Refined_95:1.40476)0.367:0.60450,(((CF_Refined_86:0.37933,(CF_Refined_74:0.61406,CF_Refined_43:0.10850)1.000:0.34468)0.999:0.19175,((CF_Refined_57:0.19003,(CF_Refined_99:0.18534,CF_Refined_160:0.33153)0.861:0.04660)1.000:0.18553,(CF_Refined_78:0.64747,(CF_Refined_129:0.26317,(CF_Refined_64:0.25293,CF_Refined_100:0.10449)0.993:0.14949)0.577:0.13006)1.000:0.19231)0.998:0.16057)0.961:0.08413,((CF_Refined_155:0.18262,CF_Refined_180:0.02711)1.000:0.42318,(CF_Refined_162:0.64092,CF_Refined_131:0.36385)1.000:0.48656)0.992:0.23471)0.853:0.05581)0.955:0.08666)1.000:0.14706);'
-
-tree = Tree(tree_2, format=1)
-
-
-plot_tree(tree, 'Species_Tree', '/Users/songweizhi/Desktop/Species_Tree.png')
+# tree_2 = '(CF_Refined_71:0.21847,CF_Refined_170:0.41504,(((CF_Refined_7:0.63495,CF_Refined_96:0.68718)0.984:0.33915,CF_Refined_82:0.16074)0.980:0.12012,((CF_Refined_25:0.20437,CF_Refined_95:1.40476)0.367:0.60450,(((CF_Refined_86:0.37933,(CF_Refined_74:0.61406,CF_Refined_43:0.10850)1.000:0.34468)0.999:0.19175,((CF_Refined_57:0.19003,(CF_Refined_99:0.18534,CF_Refined_160:0.33153)0.861:0.04660)1.000:0.18553,(CF_Refined_78:0.64747,(CF_Refined_129:0.26317,(CF_Refined_64:0.25293,CF_Refined_100:0.10449)0.993:0.14949)0.577:0.13006)1.000:0.19231)0.998:0.16057)0.961:0.08413,((CF_Refined_155:0.18262,CF_Refined_180:0.02711)1.000:0.42318,(CF_Refined_162:0.64092,CF_Refined_131:0.36385)1.000:0.48656)0.992:0.23471)0.853:0.05581)0.955:0.08666)1.000:0.14706);'
+#
+# tree = Tree(tree_2, format = 1)
+#
+#
+# plot_tree(tree, 'Species_Tree', 'Species_Tree.png')
```

### Comparing `BioSAK-1.88.9/BioSAK/Prodigal.py` & `BioSAK-1.89.0/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/Reads_simulator.py` & `BioSAK-1.89.0/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/RunGraphMB.py` & `BioSAK-1.89.0/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.89.0/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/SankeyTaxon.py` & `BioSAK-1.89.0/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/SubsampleLongReads.py` & `BioSAK-1.89.0/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.89.0/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/VERSION` & `BioSAK-1.89.0/BioSAK/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-1.88.9
+1.89.0
+- new modules added: fastaai
+
+1.88.15
 - fixed bugs
 
 1.88.0
 - new modules added: count_num
 
 1.87.0
 - new modules added: compare_sets
```

### Comparing `BioSAK-1.88.9/BioSAK/VisGeneFlk.py` & `BioSAK-1.89.0/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/add_desc.py` & `BioSAK-1.89.0/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/arCOG.py` & `BioSAK-1.89.0/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/bam2reads.py` & `BioSAK-1.89.0/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot.py` & `BioSAK-1.89.0/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot_last1row.R` & `BioSAK-1.89.0/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.89.0/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.89.0/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.89.0/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.89.0/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/cat_fa.py` & `BioSAK-1.89.0/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/cdd2cog.pl` & `BioSAK-1.89.0/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/checkm_marker.py` & `BioSAK-1.89.0/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/compare_sets.py` & `BioSAK-1.89.0/BioSAK/compare_sets.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/count_num.py` & `BioSAK-1.89.0/BioSAK/count_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/cross_link_seqs.py` & `BioSAK-1.89.0/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/dbCAN.py` & `BioSAK-1.89.0/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.89.0/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.89.0/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/enrich.py` & `BioSAK-1.89.0/BioSAK/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 import argparse
 import pandas as pd
 from scipy import stats
 from statsmodels.stats.multitest import multipletests
 
 
 enrich_usage = '''
-=================================== enrich example commands ===================================
+==================================== enrich example commands ====================================
 
 BioSAK enrich -i annotation_files -x txt -g grouping.txt -o output_dir
 BioSAK enrich -i annotation_files -x txt -g grouping.txt -o output_dir -bc
 
 # Note:
-1. The number of genome groups has to be TWO!!!
-2. Group name should NOT be 1 and 0. use some alphabet or words instead.
+  1. The number of genome groups has to be TWO!!!
+  2. Group name should NOT be 1 and 0. use some alphabet or words instead.
 
 # Example input files:
-https://github.com/songweizhi/BioSAK/tree/master/demo_data/enrich
+  https://github.com/songweizhi/BioSAK/tree/master/demo_data/enrich
 
 # please refers to https://doi.org/10.1038/s41396-020-00815-8 for how it works:
-Functions that are enriched in the genomes in either group are identified using Mann–Whitney 
-U tests followed by a Bonferroni correction with a p value cut-off of 0.05 being considered 
-significant. Only significantly different functions with greater than 2-fold mean differences 
-are considered to be enriched. Functions detected only in the genomes from one group type are 
-considered to be enriched if they existed in at least 50 percent of the genomes in the group.
+  Functions that are enriched in the genomes in either group are identified using Mann–Whitney 
+  U tests followed by a Bonferroni correction with a p value cut-off of 0.05 being considered 
+  significant. Only significantly different functions with greater than 2-fold mean differences 
+  are considered to be enriched. Functions detected only in the genomes from one group type are 
+  considered to be enriched if they existed in at least 50 percent of the genomes in the group.
 
-===============================================================================================
+=================================================================================================
 '''
 
 
 def sep_path_basename_ext(file_in):
 
     f_path, file_name = os.path.split(file_in)
     if f_path == '':
```

### Comparing `BioSAK-1.88.9/BioSAK/exe_cmds.py` & `BioSAK-1.89.0/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/ezaai2mat.py` & `BioSAK-1.89.0/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/fa2id.py` & `BioSAK-1.89.0/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/format_converter.py` & `BioSAK-1.89.0/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/fq2fa.py` & `BioSAK-1.89.0/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gapseq.py` & `BioSAK-1.89.0/BioSAK/gapseq.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,17 +99,17 @@
             else:
                 value_list.append('0')
         df_out_handle.write('\t'.join(value_list) + '\n')
     df_out_handle.close()
 
     # report genomes failed with GapSeq
     if len(failed_gnm_set) == 1:
-        print('It seems that %s was failed with GapSeq, thus was not included in %s.' % (list(failed_gnm_set)[0], df_out))
+        print('It seems that %s was failed with GapSeq, thus was not included in: %s.' % (list(failed_gnm_set)[0], df_out))
     elif len(failed_gnm_set) > 1:
-        print('It seems that the following genomes were failed with GapSeq, thus were not included in %s.' % df_out)
+        print('It seems that the following genomes were failed with GapSeq, thus were not included in: %s.' % df_out)
         print('\n'.join(sorted(list(failed_gnm_set))) + '\n')
 
     print('Done!')
 
 
 if __name__ == "__main__":
```

### Comparing `BioSAK-1.88.9/BioSAK/gbk2faa.py` & `BioSAK-1.89.0/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gbk2ffn.py` & `BioSAK-1.89.0/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gbk2fna.py` & `BioSAK-1.89.0/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gbk2gff.py` & `BioSAK-1.89.0/BioSAK/gbk2gff.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.89.0/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gc.py` & `BioSAK-1.89.0/BioSAK/gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.89.0/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.89.0/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.89.0/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.89.0/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.89.0/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_aa_composition.py` & `BioSAK-1.89.0/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.89.0/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_data_matrix.py` & `BioSAK-1.89.0/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_gene_depth.py` & `BioSAK-1.89.0/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_genome_GTDB.py` & `BioSAK-1.89.0/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_genome_NCBI.py` & `BioSAK-1.89.0/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.89.0/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.89.0/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_gnm_size.py` & `BioSAK-1.89.0/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.89.0/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_krona_plot.py` & `BioSAK-1.89.0/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_reads_from_sam.py` & `BioSAK-1.89.0/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.89.0/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_sankey_plot.R` & `BioSAK-1.89.0/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_top_hit.py` & `BioSAK-1.89.0/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/get_total_length.py` & `BioSAK-1.89.0/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/gff2chrom.py` & `BioSAK-1.89.0/BioSAK/gff2chrom.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/global_functions.py` & `BioSAK-1.89.0/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/hpc3.py` & `BioSAK-1.89.0/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/js_cmds.py` & `BioSAK-1.89.0/BioSAK/js_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/js_hpc3.py` & `BioSAK-1.89.0/BioSAK/js_hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/keep_best_hit.py` & `BioSAK-1.89.0/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/ko00001.keg` & `BioSAK-1.89.0/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/koala.py` & `BioSAK-1.89.0/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/link_16S_MAG.py` & `BioSAK-1.89.0/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/magabund.py` & `BioSAK-1.89.0/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/magabund2.py` & `BioSAK-1.89.0/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/manipulator_fasta.py` & `BioSAK-1.89.0/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/mannwhitneyu.py` & `BioSAK-1.89.0/BioSAK/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/mean_MAG_cov.py` & `BioSAK-1.89.0/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/merge_df.py` & `BioSAK-1.89.0/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/merge_seq.py` & `BioSAK-1.89.0/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/metaAssembly.py` & `BioSAK-1.89.0/BioSAK/metaAssembly.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/metabat2concoct.py` & `BioSAK-1.89.0/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/metabat2maxbin.py` & `BioSAK-1.89.0/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/ncbi_dataset.py` & `BioSAK-1.89.0/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.89.0/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.89.0/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/plot_mag.py` & `BioSAK-1.89.0/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/plot_sam_depth.py` & `BioSAK-1.89.0/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/plot_tree.R` & `BioSAK-1.89.0/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/prefix_file.py` & `BioSAK-1.89.0/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/prokka.py` & `BioSAK-1.89.0/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/reads2bam.py` & `BioSAK-1.89.0/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.89.0/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/rename_seq.py` & `BioSAK-1.89.0/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/rename_seqs.py` & `BioSAK-1.89.0/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/ribbon.py` & `BioSAK-1.89.0/BioSAK/ribbon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/sam2bam.py` & `BioSAK-1.89.0/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.89.0/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/select_seq.py` & `BioSAK-1.89.0/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.89.0/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/slice_seq.py` & `BioSAK-1.89.0/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/split_fasta.py` & `BioSAK-1.89.0/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/split_folder.py` & `BioSAK-1.89.0/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/split_sam.py` & `BioSAK-1.89.0/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/submitHPC.py` & `BioSAK-1.89.0/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.89.0/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/subset_tree.py` & `BioSAK-1.89.0/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/tmp_1.py` & `BioSAK-1.89.0/BioSAK/tmp_1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/top_16S_hits.py` & `BioSAK-1.89.0/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.89.0/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/transpose.py` & `BioSAK-1.89.0/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/usearch_uc.py` & `BioSAK-1.89.0/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK/wilcox.py` & `BioSAK-1.89.0/BioSAK/wilcox.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.89.0/BioSAK.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,33 @@
 setup.py
 BioSAK/BLCA_op_parser.py
 BioSAK/BioSAK_config.py
 BioSAK/COG2020.py
 BioSAK/COG_boxplot_last1row.R
 BioSAK/COG_boxplot_last2row.R
 BioSAK/CheckM.py
-BioSAK/ConvertMSA.py
 BioSAK/DnaFeaturesViewer.py
 BioSAK/FastaSplitler_by_num.py
 BioSAK/FastaSplitler_by_size.py
 BioSAK/GTDB_for_BLCA.py
 BioSAK/Gene2Ctg.py
 BioSAK/KEGG.py
 BioSAK/KEGG_boxplot_last1row.R
 BioSAK/KEGG_get_eukaryotic_kos.py
 BioSAK/KeepRemovingTmp.py
 BioSAK/MeanMappingDepth.py
 BioSAK/MetaBiosample.py
 BioSAK/MetaCHIP_phylo.hmm
 BioSAK/MetaCyc_reactions_with_ec.txt
 BioSAK/NetEnzymes.py
-BioSAK/Newick_tree_plotter.py
-BioSAK/OneLineAln.py
 BioSAK/Prodigal.py
 BioSAK/Reads_simulator.py
 BioSAK/RunGraphMB.py
 BioSAK/SILVA_for_BLCA.py
 BioSAK/SankeyTaxon.py
-BioSAK/SliceMSA.py
 BioSAK/SubsampleLongReads.py
 BioSAK/Tax4Fun2IndOTU.py
 BioSAK/VERSION
 BioSAK/VisBlastOp.py
 BioSAK/VisGeneFlk.py
 BioSAK/__init__.py
 BioSAK/add_desc.py
@@ -46,42 +42,37 @@
 BioSAK/boxplot_matrix_COG_backup.py
 BioSAK/boxplot_matrix_KEGG.py
 BioSAK/boxplot_matrix_dbCAN.py
 BioSAK/cat_fa.py
 BioSAK/cdd2cog.pl
 BioSAK/checkm_marker.py
 BioSAK/compare_sets.py
-BioSAK/compare_trees.R
-BioSAK/compare_trees.py
 BioSAK/count_num.py
 BioSAK/cross_link_seqs.py
 BioSAK/dbCAN.py
 BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
 BioSAK/dwnld_sra_reads.py
 BioSAK/enrich.py
 BioSAK/exe_cmds.py
 BioSAK/ezaai2mat.py
 BioSAK/fa2id.py
-BioSAK/fa2phy.py
-BioSAK/fa2tree.py
+BioSAK/fastaai.py
 BioSAK/format_converter.py
-BioSAK/format_leaf_name.py
 BioSAK/fq2fa.py
 BioSAK/gapseq.py
 BioSAK/gbk2faa.py
 BioSAK/gbk2ffn.py
 BioSAK/gbk2fna.py
 BioSAK/gbk2gff.py
 BioSAK/gbk_to_ffn_faa.py
 BioSAK/gc.py
 BioSAK/get_EC_from_ko_stats_D.py
 BioSAK/get_GTDB_taxon_gnm.py
 BioSAK/get_MAG_reads_long.py
 BioSAK/get_Pfam_hmms.py
-BioSAK/get_SCG_tree.py
 BioSAK/get_TopHits_taxonomy.py
 BioSAK/get_aa_composition.py
 BioSAK/get_bin_abundance copy.py
 BioSAK/get_data_matrix.py
 BioSAK/get_gene_depth.py
 BioSAK/get_genome_GTDB.py
 BioSAK/get_genome_NCBI.py
@@ -94,22 +85,19 @@
 BioSAK/get_reads_id_in_sam.py
 BioSAK/get_sankey_plot.R
 BioSAK/get_top_hit.py
 BioSAK/get_total_length.py
 BioSAK/gff2chrom.py
 BioSAK/global_functions.py
 BioSAK/hpc3.py
-BioSAK/iTOL.py
 BioSAK/js_cmds.py
 BioSAK/js_hpc3.py
 BioSAK/keep_best_hit.py
 BioSAK/ko00001.keg
 BioSAK/koala.py
-BioSAK/label_tree.R
-BioSAK/label_tree.py
 BioSAK/link_16S_MAG.py
 BioSAK/magabund.py
 BioSAK/magabund2.py
 BioSAK/manipulator_fasta.py
 BioSAK/manipulator_msa.py
 BioSAK/manipulator_newick.py
 BioSAK/manipulator_sam.py
@@ -127,15 +115,14 @@
 BioSAK/parse_mmseqs_tsv.py
 BioSAK/plot_mag.py
 BioSAK/plot_sam_depth.py
 BioSAK/plot_tree.R
 BioSAK/prefix_file.py
 BioSAK/prokka.py
 BioSAK/reads2bam.py
-BioSAK/rename_leaves.py
 BioSAK/rename_reads_for_Reago.py
 BioSAK/rename_seq.py
 BioSAK/rename_seqs.py
 BioSAK/ribbon.py
 BioSAK/sam2bam.py
 BioSAK/sampling_GTDB_gnms.py
 BioSAK/select_seq.py
```

### Comparing `BioSAK-1.88.9/LICENSE` & `BioSAK-1.89.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/README.md` & `BioSAK-1.89.0/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.9/bin/BioSAK` & `BioSAK-1.89.0/bin/BioSAK`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
        RunGraphMB              ->  Prepare input files for GraphMB
        gc                      ->  Get GC content
        get_gnm_size            ->  Get the total length of genome(s)
        get_gene_depth          ->  Get gene depth by contig depth
        MeanMappingDepth        ->  Get mean mapping depth 
        get_MAG_reads_long      ->  Extract MAG-specific long reads for reassembling
        parse_mmseqs_tsv        ->  Parse mmseqs tsv
+       fastaai                 ->  A wrapper for FastAAI
        
     Functional annotation
        KEGG                    ->  KEGG annotation
        koala                   ->  Separate the combined BlastKOALA or GhostKOALA output
        COG2020                 ->  COG annotation (v2020, by blastp/diamond)
        arCOG                   ->  COG annotation for archaea (version ar18)
        dbCAN                   ->  CAZy annotation with dbCAN
@@ -98,15 +99,14 @@
        merge_df                ->  Merge dataframes
        add_desc                ->  Add function description to input of the iTOL module
        transpose               ->  Transpose dataframe
        wilcox                  ->  Wilcoxon signed-rank test (non-parametric paired T-test)
        mannwhitneyu            ->  Mann-Whitney U rank test on two independent samples
     
     Others
-       iTOL                    ->  Prepare iTOL files
        js_cmds                 ->  Put commands in job scripts
        js_hpc3                 ->  Put commands in job scripts (HKUST hpc3)
        hpc3                    ->  Submit jobs on HKUST hpc3
        exe_cmds                ->  Execute commands with multiprocessing
        split_folder            ->  Split folder
        prefix_file             ->  Prefix file
        BestHit                 ->  Keep best blast hits (outfmt 6)
@@ -119,33 +119,36 @@
        cross_link_seqs         ->  Cross link matched regions between two sequences
        submitHPC               ->  A wrapper for submitHPC.sh
        KeepRemovingTmp         ->  Keep removing old files in a folder
        ribbon                  ->  Make a ribbon diagram
        compare_sets            ->  compare_sets
        
     1. Phylogenetic tree-related modules have been moved to TreeSAK
-    2. Use "pip3 install --upgrade BioSAK" to get the latest version
+    2. Upgrade with: pip3 install --upgrade BioSAK
+
     ''' % version(config_dict)
 
     print(help_message)
 
 
 if __name__ == '__main__':
 
-    # initialize the options parser
+    # initialize the options parser and disable warning message
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(help="--", dest='subparser_name')
-
-    # disable warning message
     warnings.filterwarnings('ignore')
 
     # parse options
     if (len(sys.argv) == 1) or (sys.argv[1] in ['-h', '-help', '--help']):
         print_main_help()
-        sys.exit(0)
+        exit()
+
+    elif sys.argv[1] in ['iTOL', 'SliceMSA', 'ConvertMSA', 'fa2phy', 'PhyloBiAssoc', 'OneLineAln']:
+        print('%s has moved to TreeSAK, program exited!' % sys.argv[1])
+        exit()
 
     elif sys.argv[1] == 'COG2020':
         from BioSAK import COG2020
         COG2020_parser = subparsers.add_parser('COG2020', description='Wrapper for COG annotation (v2020)', usage=COG2020.COG2020_parser_usage)
         COG2020_parser.add_argument('-i',                   required=True,                                  help='path to input sequences (in multi-fasta format)')
         COG2020_parser.add_argument('-x',                   required=False,                                 help='file extension')
         COG2020_parser.add_argument('-m',                   required=True,                                  help='sequence type, "N/n" for "nucleotide", "P/p" for "protein"')
@@ -210,39 +213,14 @@
         CheckM_parser.add_argument('-x',    required=False, default='fasta',     help='bin file extension')
         CheckM_parser.add_argument('-cpl',  required=False, type=float,          help='completeness cutoff (0-100)')
         CheckM_parser.add_argument('-ctm',  required=False, type=float,          help='contamination cutoff (0-100)')
         CheckM_parser.add_argument('-r',    required=False, action="store_true", help='recalculate contamination')
         args = vars(parser.parse_args())
         CheckM.CheckM(args)
 
-    elif sys.argv[1] == 'iTOL':
-        from BioSAK import iTOL
-        iTOL_parser = subparsers.add_parser('iTOL', description='Plot tree with iTOL', usage=iTOL.iTOL_usage)
-        iTOL_parser.add_argument('-Labels',          required=False, action='store_true',   help='Labels')
-        iTOL_parser.add_argument('-ColorStrip',      required=False, action='store_true',   help='ColorStrip')
-        iTOL_parser.add_argument('-ColorRange',      required=False, action='store_true',   help='ColorRange')
-        iTOL_parser.add_argument('-SimpleBar',       required=False, action='store_true',   help='SimpleBar')
-        iTOL_parser.add_argument('-Heatmap',         required=False, action='store_true',   help='Heatmap')
-        iTOL_parser.add_argument('-ExternalShape',   required=False, action='store_true',   help='ExternalShape')
-        iTOL_parser.add_argument('-Binary',          required=False, action='store_true',   help='Binary')
-        iTOL_parser.add_argument('-Connection',      required=False, action='store_true',   help='Connection')
-        iTOL_parser.add_argument('-PieChart',        required=False, action='store_true',   help='PieChart')
-        iTOL_parser.add_argument('-ll',              required=False, default=None,          help='Leaf Label')
-        iTOL_parser.add_argument('-gc',              required=False, default=None,          help='Specify Group/column Color (optional)')
-        iTOL_parser.add_argument('-cc',              required=False, default=None,          help='Specify Column Color (for ExternalShape format) (optional)')
-        iTOL_parser.add_argument('-lg',              required=False, default=None,          help='Leaf to Group')
-        iTOL_parser.add_argument('-lv',              required=False, default=None,          help='Leaf to Value')
-        iTOL_parser.add_argument('-lm',              required=False, default=None,          help='Leaf to data Matrix')
-        iTOL_parser.add_argument('-dr',              required=False, default=None,          help='Donor to Recipient')
-        iTOL_parser.add_argument('-scale',           required=False, default=None,          help='Scale Values, in format 0-3-6-9')
-        iTOL_parser.add_argument('-lt',              required=False, default=None,          help='Legend Title')
-        iTOL_parser.add_argument('-o',               required=True,                         help='Output filename')
-        args = vars(parser.parse_args())
-        iTOL.iTOL(args)
-
     elif sys.argv[1] == 'split_folder':
         from BioSAK import split_folder
         split_folder_parser = subparsers.add_parser('split_folder', description='Split folder', usage=split_folder.split_folder_parser_usage)
         split_folder_parser.add_argument('-in',             required=True,                                  help='file folder')
         split_folder_parser.add_argument('-x',              required=True,                                  help='file extension')
         split_folder_parser.add_argument('-n',              required=False, type=int,                       help='number of subfolder')
         args = vars(parser.parse_args())
@@ -498,22 +476,14 @@
         from BioSAK import sam2bam
         sam2bam_parser = subparsers.add_parser('sam2bam', usage=sam2bam.sam2bam_usage)
         sam2bam_parser.add_argument('-sam', required=True,                          help='sam file')
         sam2bam_parser.add_argument('-t',   required=False, type=int, default=1,    help='number of threads')
         args = vars(parser.parse_args())
         sam2bam.sam2bam(args)
 
-    elif sys.argv[1] == 'fa2tree':
-        from BioSAK import fa2tree
-        fa2tree_parser = subparsers.add_parser('fa2tree', usage=fa2tree.fa2tree_usage)
-        fa2tree_parser.add_argument('-seq', required=True,                          help='sequence file')
-        fa2tree_parser.add_argument('-t',   required=False, type=int, default=1,    help='number of threads, default: 1')
-        args = vars(parser.parse_args())
-        fa2tree.fa2tree(args)
-
     elif sys.argv[1] == 'BLCA_op_parser':
         from BioSAK import BLCA_op_parser
         BLCA_op_parser_parser = subparsers.add_parser('BLCA_op_parser', usage=BLCA_op_parser.BLCA_op_parser_usage)
         BLCA_op_parser_parser.add_argument('-in', required=True, help='BLCA output')
         args = vars(parser.parse_args())
         BLCA_op_parser.BLCA_op_parser(args)
 
@@ -582,24 +552,14 @@
         mean_MAG_cov_parser = subparsers.add_parser('mean_MAG_cov', usage=mean_MAG_cov.mean_MAG_cov_usage)
         mean_MAG_cov_parser.add_argument('-d', required=True, help='MetaBAT produced depth file')
         mean_MAG_cov_parser.add_argument('-b', required=True, help='bin folder')
         mean_MAG_cov_parser.add_argument('-x', required=True, help='file extension')
         args = vars(parser.parse_args())
         mean_MAG_cov.mean_MAG_cov(args)
 
-    elif sys.argv[1] == 'GTDB_tree':
-        from BioSAK import GTDB_tree
-        GTDB_tree_parser = subparsers.add_parser('GTDB_tree', usage=GTDB_tree.GTDB_tree_usage)
-        GTDB_tree_parser.add_argument('-p', required=True,                         help='output prefix')
-        GTDB_tree_parser.add_argument('-i', required=True,                         help='genome folder')
-        GTDB_tree_parser.add_argument('-x', required=True,                         help='genome file extension')
-        GTDB_tree_parser.add_argument('-t', required=False, type=int, default=1,   help='number of threads')
-        args = vars(parser.parse_args())
-        GTDB_tree.GTDB_tree(args)
-
     elif sys.argv[1] == 'exe_cmds':
         from BioSAK import exe_cmds
         exe_cmds_parser = subparsers.add_parser('exe_cmds', usage=exe_cmds.exe_cmds_usage)
         exe_cmds_parser.add_argument('-c', required=True,                       help='cmds file')
         exe_cmds_parser.add_argument('-t', required=False, type=int, default=1, help='number of threads')
         args = vars(parser.parse_args())
         exe_cmds.exe_cmds(args)
@@ -737,78 +697,26 @@
         SubsampleLongReads_parser.add_argument('-s',        required=True,                          help='separate subsample rates (1-100) with comma, e.g. 1,5,10')
         SubsampleLongReads_parser.add_argument('-o',        required=True,                          help='output directory')
         SubsampleLongReads_parser.add_argument('-fq',       required=False, action="store_true",    help='in fastq format, default: fa')
         SubsampleLongReads_parser.add_argument('-oneline',  required=False, action="store_true",    help='put sequence in single line')
         args = vars(parser.parse_args())
         SubsampleLongReads.SubsampleLongReads(args)
 
-    elif sys.argv[1] == 'OneLineAln':
-        from BioSAK import OneLineAln
-        OneLineAln_parser = subparsers.add_parser('OneLineAln', description='One-line fasta format alignments', usage=OneLineAln.OneLineAln_usage)
-        OneLineAln_parser.add_argument('-in',               required=True,                       help='input MSA in fasta format')
-        OneLineAln_parser.add_argument('-out',              required=False, default=None,        help='output file')
-        OneLineAln_parser.add_argument('-upper',            required=False, action='store_true', help='turn to uppercase')
-        args = vars(parser.parse_args())
-        OneLineAln.OneLineAln(args)
-
-    elif sys.argv[1] == 'SliceMSA':
-        from BioSAK import SliceMSA
-        SliceMSA_parser = subparsers.add_parser('SliceMSA', description='Slice MSA by column', usage=SliceMSA.SliceMSA_usage)
-        SliceMSA_parser.add_argument('-i',                  required=True,                         help='input MSA in fasta format')
-        SliceMSA_parser.add_argument('-fi',                 required=False, default='fasta',       help='format (NOT file extension) of input MSA, default: fasta')
-        SliceMSA_parser.add_argument('-s',                  required=True,                         help='columns to export, e.g. 200-300, -100, 50-')
-        SliceMSA_parser.add_argument('-o',                  required=True,                         help='output file or folder')
-        SliceMSA_parser.add_argument('-fo',                 required=False, default='fasta',       help='format of output MSA, select from fasta and phylip-relaxed, default: fasta')
-        SliceMSA_parser.add_argument('-force',              required=False, action="store_true",   help='force overwrite existing output folder')
-        args = vars(parser.parse_args())
-        SliceMSA.SliceMSA(args)
-
-    elif sys.argv[1] == 'ConvertMSA':
-        from BioSAK import ConvertMSA
-        ConvertMSA_parser = subparsers.add_parser('ConvertMSA', usage=ConvertMSA.ConvertMSA_usage)
-        ConvertMSA_parser.add_argument('-i',       required=True,                       help='input alignment')
-        ConvertMSA_parser.add_argument('-xi',      required=False, default='aln',       help='input alignment extension')
-        ConvertMSA_parser.add_argument('-fi',      required=True,                       help='input alignment format, e.g., fasta, phylip')
-        ConvertMSA_parser.add_argument('-o',       required=True,                       help='output alignment')
-        ConvertMSA_parser.add_argument('-xo',      required=False, default='aln',       help='output alignment extension')
-        ConvertMSA_parser.add_argument('-fo',      required=True,                       help='output alignment format, e.g., fasta, phylip')
-        ConvertMSA_parser.add_argument('-oneline', required=False, action="store_true", help='put sequence in single line, available if -fo is fasta')
-        ConvertMSA_parser.add_argument('-nogap',   required=False, action="store_true", help='remove gaps from alignment, available if -fo is fasta')
-        ConvertMSA_parser.add_argument('-f',       required=False, action="store_true", help='force overwrite existing output folder')
-        args = vars(parser.parse_args())
-        ConvertMSA.ConvertMSA(args)
-
-    elif sys.argv[1] == 'fa2phy':
-        from BioSAK import fa2phy
-        fa2phy_parser = subparsers.add_parser('fa2phy', usage=fa2phy.fa2phy_usage)
-        fa2phy_parser.add_argument('-i', required=True, help='input MSA in fasta format')
-        fa2phy_parser.add_argument('-o', required=True, help='output MSA in phylip format')
-        args = vars(parser.parse_args())
-        fa2phy.fa2phy(args)
-
     elif sys.argv[1] == 'metaBiosample':
         from BioSAK import MetaBiosample
         MetaBiosample_parser = subparsers.add_parser('MetaBiosample', usage=MetaBiosample.MetaBiosample_usage)
         MetaBiosample_parser.add_argument('-i',     required=True,                          help='biosample id file, one id per line')
         MetaBiosample_parser.add_argument('-a',     required=True,                          help='attributes to extract')
         MetaBiosample_parser.add_argument('-o',     required=True,                          help='output folder')
         MetaBiosample_parser.add_argument('-t',     required=False, type=int, default=1,    help='number of threads, default: 1')
         MetaBiosample_parser.add_argument('-f',     required=False, action="store_true",    help='Force overwrite existing results')
         MetaBiosample_parser.add_argument('-exe',   required=False, action="store_true",    help='execute cmds')
         args = vars(parser.parse_args())
         MetaBiosample.MetaBiosample(args)
 
-    elif sys.argv[1] == 'PhyloBiAssoc':
-        from BioSAK import PhyloBiAssoc
-        PhyloBiAssoc_parser = subparsers.add_parser('PhyloBiAssoc', usage=PhyloBiAssoc.PhyloBiAssoc_usage)
-        PhyloBiAssoc_parser.add_argument('-t', required=True, help='tree file')
-        PhyloBiAssoc_parser.add_argument('-d', required=True, help='data file')
-        args = vars(parser.parse_args())
-        PhyloBiAssoc.PhyloBiAssoc(args)
-
     elif sys.argv[1] == 'metabat2concoct':
         from BioSAK import metabat2concoct
         metabat2concoct_parser = subparsers.add_parser('metabat2concoct', usage=metabat2concoct.metabat2concoct_usage)
         metabat2concoct_parser.add_argument('-i', required=True, help='metabat depth')
         metabat2concoct_parser.add_argument('-o', required=True, help='concoct depth')
         args = vars(parser.parse_args())
         metabat2concoct.metabat2concoct(args)
@@ -927,21 +835,22 @@
         koala_parser.add_argument('-f', required=False, action="store_true",    help='force overwrite')
         args = vars(parser.parse_args())
         koala.koala(args)
 
     elif sys.argv[1] == 'subset_df':
         from BioSAK import subset_df
         subset_df_parser = subparsers.add_parser('subset_df', usage=subset_df.subset_df_usage)
-        subset_df_parser.add_argument('-i',     required=True,                          help='input file')
-        subset_df_parser.add_argument('-o',     required=True,                          help='output file')
-        subset_df_parser.add_argument('-r',     required=False, default='',             help='header of rows to keep')
-        subset_df_parser.add_argument('-c',     required=False, default='',             help='header of columns to keep')
-        subset_df_parser.add_argument('-s',     required=False, default='tab',          help='column separator, choose from tab and comma, default: tab')
-        subset_df_parser.add_argument('-b',     required=False, action='store_true',    help='write out dataframe in 0/1 format')
-        subset_df_parser.add_argument('-m',     required=False, action='store_true',    help='convert 0 to -1')
+        subset_df_parser.add_argument('-i',         required=True,                          help='input file')
+        subset_df_parser.add_argument('-o',         required=True,                          help='output file')
+        subset_df_parser.add_argument('-r',         required=False, default='',             help='header of rows to keep')
+        subset_df_parser.add_argument('-c',         required=False, default='',             help='header of columns to keep')
+        subset_df_parser.add_argument('-s',         required=False, default='tab',          help='column separator, choose from tab and comma, default: tab')
+        subset_df_parser.add_argument('-b',         required=False, action='store_true',    help='write out dataframe in 0/1 format')
+        subset_df_parser.add_argument('-m',         required=False, action='store_true',    help='convert 0 to -1')
+        subset_df_parser.add_argument('-skip1row',  required=False, action='store_true',    help='skip the 1st row of the -c/-r file')
         args = vars(parser.parse_args())
         subset_df.subset_df(args)
 
     elif sys.argv[1] == 'add_desc':
         from BioSAK import add_desc
         add_desc_parser = subparsers.add_parser('add_desc', usage=add_desc.add_desc_usage)
         add_desc_parser.add_argument('-i', required=True, help='input file ')
@@ -1039,14 +948,25 @@
         from BioSAK import count_num
         count_num_parser = subparsers.add_parser('count_num', usage=count_num.count_num_usage)
         count_num_parser.add_argument('-i', required=True, help='input file')
         count_num_parser.add_argument('-c', required=False, default=1, help='column, default: 1 (the first column)')
         args = vars(parser.parse_args())
         count_num.count_num(args)
 
+    elif sys.argv[1] == 'fastaai':
+        from BioSAK import fastaai
+        fastaai_parser = subparsers.add_parser('fastaai', usage=fastaai.fastaai_usage)
+        fastaai_parser.add_argument('-i', required=True,                          help='faa files')
+        fastaai_parser.add_argument('-x', required=False,default='faa',           help='file extension, default: faa')
+        fastaai_parser.add_argument('-o', required=True,                          help='output directory')
+        fastaai_parser.add_argument('-t', required=False, default=1, type=int,    help='number of threads, default: 1')
+        fastaai_parser.add_argument('-f', required=False, action="store_true",    help='force overwrite')
+        args = vars(parser.parse_args())
+        fastaai.fastaai(args)
+
     else:
         print('Unrecognized command: %s, program exited' % sys.argv[1])
         exit()
 
 
 upload_to_pypi_cmd = '''
```

### Comparing `BioSAK-1.88.9/setup.py` & `BioSAK-1.89.0/setup.py`

 * *Files identical despite different names*

