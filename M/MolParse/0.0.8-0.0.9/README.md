# Comparing `tmp/molparse-0.0.8.tar.gz` & `tmp/molparse-0.0.9.tar.gz`

## Comparing `molparse-0.0.8.tar` & `molparse-0.0.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rwxr-xr-x   0        0        0      206 2020-02-02 00:00:00.000000 molparse-0.0.8/moltree
--rwxr-xr-x   0        0        0     9950 2020-02-02 00:00:00.000000 molparse-0.0.8/molxvg
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/__init__.py
--rw-r--r--   0        0        0    45799 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/amber.py
--rw-r--r--   0        0        0    23795 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/amino.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/analysis.py
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/atom.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/bondlist.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/chain.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/compare.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/console_io.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/convert.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/go.py
--rw-r--r--   0        0        0    18828 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/graphing.py
--rw-r--r--   0        0        0    21492 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/group.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/gui.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/histidine.py
--rw-r--r--   0        0        0    37386 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/io.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/list.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/manipulate.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ndx.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/network.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ntp.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/nucleic.py
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/plot.py
--rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/povplot.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/residue.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/restraint.py
--rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/system.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/tree.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/version.py
--rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/xvg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/dl_poly/__init__.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/dl_poly/calculator.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/dl_poly/dl_poly_py.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/dna/__init__.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/dna/dna.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/hijack/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/hijack/hijack.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/monte/__init__.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/monte/carlo.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/monte/rand.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/monte/volumes.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/mutate/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/mutate/functional.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/mutate/link.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/mutate/protein.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ndfes/__init__.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ndfes/ndfes.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/rdkit/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/rdkit/draw.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/rdkit/features.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/rdkit/fingerprint.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/rdkit/mol.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/ALA.pdb
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/ARG.pdb
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/ASN.pdb
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/ASP.pdb
--rwxr-xr-x   0        0        0     2836 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/AT_FLAT.pdb
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/CYS.pdb
--rwxr-xr-x   0        0        0     2756 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/GC_FLAT.pdb
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/GLN.pdb
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/GLU.pdb
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/GLY.pdb
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/HIS.pdb
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/ILE.pdb
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/LEU.pdb
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/LYS.pdb
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/MET.pdb
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/PHE.pdb
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/PRO.pdb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/SER.pdb
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/THR.pdb
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/TRP.pdb
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/TYR.pdb
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/ref/VAL.pdb
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/signal/__init__.py
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/signal/fitwizard.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/signal/io.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/signal/modify.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/signal/peaks.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/sites/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/sites/site.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/styles/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/styles/styles.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/tunnel/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/tunnel/barrier.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 molparse-0.0.8/molparse/units/__init__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 molparse-0.0.8/.gitignore
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 molparse-0.0.8/README.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 molparse-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 molparse-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      206 2020-02-02 00:00:00.000000 molparse-0.0.9/moltree
+-rwxr-xr-x   0        0        0     9950 2020-02-02 00:00:00.000000 molparse-0.0.9/molxvg
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/__init__.py
+-rw-r--r--   0        0        0    45799 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/amber.py
+-rw-r--r--   0        0        0    23795 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/amino.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/analysis.py
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/atom.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/bondlist.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/chain.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/compare.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/console_io.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/convert.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/go.py
+-rw-r--r--   0        0        0    18828 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/graphing.py
+-rw-r--r--   0        0        0    21492 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/group.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/gui.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/histidine.py
+-rw-r--r--   0        0        0    37386 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/io.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/list.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/manipulate.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ndx.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/network.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ntp.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/nucleic.py
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/plot.py
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/povplot.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/residue.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/restraint.py
+-rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/system.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/tree.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/version.py
+-rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/xvg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/dl_poly/__init__.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/dl_poly/calculator.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/dl_poly/dl_poly_py.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/dna/__init__.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/dna/dna.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/hijack/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/hijack/hijack.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/monte/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/monte/carlo.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/monte/rand.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/monte/volumes.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/mutate/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/mutate/functional.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/mutate/link.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/mutate/protein.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ndfes/__init__.py
+-rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ndfes/ndfes.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/rdkit/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/rdkit/draw.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/rdkit/features.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/rdkit/fingerprint.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/rdkit/mol.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/ALA.pdb
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/ARG.pdb
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/ASN.pdb
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/ASP.pdb
+-rwxr-xr-x   0        0        0     2836 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/AT_FLAT.pdb
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/CYS.pdb
+-rwxr-xr-x   0        0        0     2756 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/GC_FLAT.pdb
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/GLN.pdb
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/GLU.pdb
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/GLY.pdb
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/HIS.pdb
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/ILE.pdb
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/LEU.pdb
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/LYS.pdb
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/MET.pdb
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/PHE.pdb
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/PRO.pdb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/SER.pdb
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/THR.pdb
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/TRP.pdb
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/TYR.pdb
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/ref/VAL.pdb
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/signal/__init__.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/signal/fitwizard.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/signal/io.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/signal/modify.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/signal/peaks.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/sites/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/sites/site.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/styles/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/styles/styles.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/tunnel/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/tunnel/barrier.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 molparse-0.0.9/molparse/units/__init__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 molparse-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 molparse-0.0.9/README.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 molparse-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 molparse-0.0.9/PKG-INFO
```

### Comparing `molparse-0.0.8/molxvg` & `molparse-0.0.9/molxvg`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/__init__.py` & `molparse-0.0.9/molparse/__init__.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/amber.py` & `molparse-0.0.9/molparse/amber.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/amino.py` & `molparse-0.0.9/molparse/amino.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/analysis.py` & `molparse-0.0.9/molparse/analysis.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/atom.py` & `molparse-0.0.9/molparse/atom.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/chain.py` & `molparse-0.0.9/molparse/chain.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/compare.py` & `molparse-0.0.9/molparse/compare.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/console_io.py` & `molparse-0.0.9/molparse/console_io.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/convert.py` & `molparse-0.0.9/molparse/convert.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/go.py` & `molparse-0.0.9/molparse/go.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/graphing.py` & `molparse-0.0.9/molparse/graphing.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/group.py` & `molparse-0.0.9/molparse/group.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/histidine.py` & `molparse-0.0.9/molparse/histidine.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/io.py` & `molparse-0.0.9/molparse/io.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/list.py` & `molparse-0.0.9/molparse/list.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/manipulate.py` & `molparse-0.0.9/molparse/manipulate.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ndx.py` & `molparse-0.0.9/molparse/ndx.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/network.py` & `molparse-0.0.9/molparse/network.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ntp.py` & `molparse-0.0.9/molparse/ntp.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/nucleic.py` & `molparse-0.0.9/molparse/nucleic.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/plot.py` & `molparse-0.0.9/molparse/plot.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/povplot.py` & `molparse-0.0.9/molparse/povplot.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/residue.py` & `molparse-0.0.9/molparse/residue.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/restraint.py` & `molparse-0.0.9/molparse/restraint.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/system.py` & `molparse-0.0.9/molparse/system.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/tree.py` & `molparse-0.0.9/molparse/tree.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/version.py` & `molparse-0.0.9/molparse/version.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/xvg.py` & `molparse-0.0.9/molparse/xvg.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/dl_poly/calculator.py` & `molparse-0.0.9/molparse/dl_poly/calculator.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/dl_poly/dl_poly_py.py` & `molparse-0.0.9/molparse/dl_poly/dl_poly_py.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/dna/dna.py` & `molparse-0.0.9/molparse/dna/dna.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/hijack/hijack.py` & `molparse-0.0.9/molparse/hijack/hijack.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/monte/carlo.py` & `molparse-0.0.9/molparse/monte/carlo.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/monte/volumes.py` & `molparse-0.0.9/molparse/monte/volumes.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/mutate/functional.py` & `molparse-0.0.9/molparse/mutate/functional.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/mutate/protein.py` & `molparse-0.0.9/molparse/mutate/protein.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ndfes/ndfes.py` & `molparse-0.0.9/molparse/ndfes/ndfes.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/rdkit/draw.py` & `molparse-0.0.9/molparse/rdkit/draw.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/rdkit/features.py` & `molparse-0.0.9/molparse/rdkit/features.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/rdkit/fingerprint.py` & `molparse-0.0.9/molparse/rdkit/fingerprint.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/rdkit/mol.py` & `molparse-0.0.9/molparse/rdkit/mol.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/ALA.pdb` & `molparse-0.0.9/molparse/ref/ALA.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/ARG.pdb` & `molparse-0.0.9/molparse/ref/ARG.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/ASN.pdb` & `molparse-0.0.9/molparse/ref/ASN.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/ASP.pdb` & `molparse-0.0.9/molparse/ref/ASP.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/AT_FLAT.pdb` & `molparse-0.0.9/molparse/ref/AT_FLAT.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/CYS.pdb` & `molparse-0.0.9/molparse/ref/CYS.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/GC_FLAT.pdb` & `molparse-0.0.9/molparse/ref/GC_FLAT.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/GLN.pdb` & `molparse-0.0.9/molparse/ref/GLN.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/GLU.pdb` & `molparse-0.0.9/molparse/ref/GLU.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/HIS.pdb` & `molparse-0.0.9/molparse/ref/HIS.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/ILE.pdb` & `molparse-0.0.9/molparse/ref/ILE.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/LEU.pdb` & `molparse-0.0.9/molparse/ref/LEU.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/LYS.pdb` & `molparse-0.0.9/molparse/ref/LYS.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/MET.pdb` & `molparse-0.0.9/molparse/ref/MET.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/PHE.pdb` & `molparse-0.0.9/molparse/ref/PHE.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/PRO.pdb` & `molparse-0.0.9/molparse/ref/PRO.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/SER.pdb` & `molparse-0.0.9/molparse/ref/SER.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/THR.pdb` & `molparse-0.0.9/molparse/ref/THR.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/TRP.pdb` & `molparse-0.0.9/molparse/ref/TRP.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/TYR.pdb` & `molparse-0.0.9/molparse/ref/TYR.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/ref/VAL.pdb` & `molparse-0.0.9/molparse/ref/VAL.pdb`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/signal/fitwizard.py` & `molparse-0.0.9/molparse/signal/fitwizard.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/signal/io.py` & `molparse-0.0.9/molparse/signal/io.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/signal/modify.py` & `molparse-0.0.9/molparse/signal/modify.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/signal/peaks.py` & `molparse-0.0.9/molparse/signal/peaks.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/sites/site.py` & `molparse-0.0.9/molparse/sites/site.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/styles/styles.py` & `molparse-0.0.9/molparse/styles/styles.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/molparse/tunnel/barrier.py` & `molparse-0.0.9/molparse/tunnel/barrier.py`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/README.md` & `molparse-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `molparse-0.0.8/pyproject.toml` & `molparse-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "MolParse"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Max Winokan", email="max@winokan.com"},
 ]
 description = "Package for parsing, writing, and modifying molecular structure files"
 readme = "README.md"
 requires-python = ">=3.9"
 requires = []
```

### Comparing `molparse-0.0.8/PKG-INFO` & `molparse-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MolParse
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for parsing, writing, and modifying molecular structure files
 Project-URL: Homepage, https://github.com/mwinokan/MolParse
 Project-URL: Bug Tracker, https://github.com/mwinokan/MolParse/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

