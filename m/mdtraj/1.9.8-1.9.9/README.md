# Comparing `tmp/mdtraj-1.9.8.tar.gz` & `tmp/mdtraj-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdtraj-1.9.8.tar", last modified: Sun Jul  2 15:28:45 2023, max compression
+gzip compressed data, was "mdtraj-1.9.9.tar", last modified: Sat Jul 22 15:19:59 2023, max compression
```

## Comparing `mdtraj-1.9.8.tar` & `mdtraj-1.9.9.tar`

### file list

```diff
@@ -1,364 +1,364 @@
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.541586 mdtraj-1.9.8/
--rw-r--r--   0 mattthompson   (501) staff       (20)    26530 2022-10-27 15:00:02.000000 mdtraj-1.9.8/LICENSE
--rw-r--r--   0 mattthompson   (501) staff       (20)      184 2022-10-27 15:00:02.000000 mdtraj-1.9.8/MANIFEST.in
--rw-r--r--   0 mattthompson   (501) staff       (20)     1515 2023-07-02 15:28:45.541231 mdtraj-1.9.8/PKG-INFO
--rw-r--r--   0 mattthompson   (501) staff       (20)     3238 2022-11-06 01:55:17.000000 mdtraj-1.9.8/README.md
--rw-r--r--   0 mattthompson   (501) staff       (20)    16701 2022-11-06 01:55:17.000000 mdtraj-1.9.8/basesetup.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.415771 mdtraj-1.9.8/examples/
--rw-r--r--   0 mattthompson   (501) staff       (20)       20 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/.gitignore
--rw-r--r--   0 mattthompson   (501) staff       (20)   145051 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/1vii_3frames.pdb
--rw-r--r--   0 mattthompson   (501) staff       (20)    32402 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/ala2.h5
--rw-r--r--   0 mattthompson   (501) staff       (20)     7181 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/atom-selection.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3331 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/centroids.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3363 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/clustering.ipynb
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.416827 mdtraj-1.9.8/examples/data/
--rw-r--r--   0 mattthompson   (501) staff       (20)    98115 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/data/frame0.h5
--rw-r--r--   0 mattthompson   (501) staff       (20)    72416 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/data/frame0.xtc
--rw-r--r--   0 mattthompson   (501) staff       (20)     1749 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/data/native.pdb
--rw-r--r--   0 mattthompson   (501) staff       (20)     2880 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/hbonds.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3267 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/iterload.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     4954 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/native-contact.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     2064 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/nmr.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     4194 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/principal-components.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     2714 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/ramachandran-plot.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3943 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/rmsd-benchmark.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     2316 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/rmsd-drift.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3989 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/simulation-with-openmm.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3547 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/solvent-accessible-surface-area.ipynb
--rw-r--r--   0 mattthompson   (501) staff       (20)     3087 2022-11-06 01:55:17.000000 mdtraj-1.9.8/examples/test_examples.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5324 2022-10-27 15:00:02.000000 mdtraj-1.9.8/examples/two-pass-clustering.ipynb
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.417459 mdtraj-1.9.8/mdtraj/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2628 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/__init__.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.430320 mdtraj-1.9.8/mdtraj/core/
--rw-r--r--   0 mattthompson   (501) staff       (20)        0 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/core/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    15631 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/core/element.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13043 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/core/residue_names.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    15006 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/core/selection.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    61206 2023-06-10 19:37:18.000000 mdtraj-1.9.8/mdtraj/core/topology.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    81628 2023-06-10 19:37:18.000000 mdtraj-1.9.8/mdtraj/core/trajectory.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.440682 mdtraj-1.9.8/mdtraj/formats/
--rw-r--r--   0 mattthompson   (501) staff       (20)      695 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    33372 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/amberrst.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13744 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/arc.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.441707 mdtraj-1.9.8/mdtraj/formats/binpos/
--rw-r--r--   0 mattthompson   (501) staff       (20)   569104 2023-07-02 15:28:41.000000 mdtraj-1.9.8/mdtraj/formats/binpos/binpos.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    18845 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/binpos/binpos.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)      747 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/binposlib.pxd
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.442853 mdtraj-1.9.8/mdtraj/formats/binpos/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)      507 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/include/binposplugin.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1237 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/include/largefiles.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    38579 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/include/molfile_plugin.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/include/vmdplugin.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.443075 mdtraj-1.9.8/mdtraj/formats/binpos/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)     6989 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/binpos/src/binposplugin.c
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.443973 mdtraj-1.9.8/mdtraj/formats/dcd/
--rw-r--r--   0 mattthompson   (501) staff       (20)   614294 2023-07-02 15:28:41.000000 mdtraj-1.9.8/mdtraj/formats/dcd/dcd.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    25481 2023-02-10 16:09:23.000000 mdtraj-1.9.8/mdtraj/formats/dcd/dcd.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)     1100 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/dcdlib.pxd
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.445340 mdtraj-1.9.8/mdtraj/formats/dcd/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2480 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/dcdplugin.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/endianswap.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    10996 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/fastio.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1237 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/largefiles.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    38579 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/molfile_plugin.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/include/vmdplugin.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.445561 mdtraj-1.9.8/mdtraj/formats/dcd/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)    39616 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dcd/src/dcdplugin.c
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.446684 mdtraj-1.9.8/mdtraj/formats/dtr/
--rw-r--r--   0 mattthompson   (501) staff       (20)   633885 2023-07-02 15:28:41.000000 mdtraj-1.9.8/mdtraj/formats/dtr/dtr.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    29095 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/dtr/dtr.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)     1163 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/dtrlib.pxd
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.447768 mdtraj-1.9.8/mdtraj/formats/dtr/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)    10359 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/include/dtrplugin.hxx
--rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/include/endianswap.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    39114 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/include/molfile_plugin.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2734 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/include/vmddir.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/include/vmdplugin.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.447975 mdtraj-1.9.8/mdtraj/formats/dtr/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)    70106 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/dtr/src/dtrplugin.cxx
--rw-r--r--   0 mattthompson   (501) staff       (20)    21010 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/gro.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    11184 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/gsd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    40764 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/hdf5.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5880 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/hoomdxml.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    23510 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/lammpstrj.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    17956 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/lh5.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    18399 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/mdcrd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9937 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/mol2.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    23226 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/netcdf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2835 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/openmmxml.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.448954 mdtraj-1.9.8/mdtraj/formats/pdb/
--rw-r--r--   0 mattthompson   (501) staff       (20)     1131 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/pdb/__init__.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.449881 mdtraj-1.9.8/mdtraj/formats/pdb/data/
--rw-r--r--   0 mattthompson   (501) staff       (20)     9967 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/pdb/data/pdbNames.xml
--rw-r--r--   0 mattthompson   (501) staff       (20)    24621 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/pdb/data/residues.xml
--rw-r--r--   0 mattthompson   (501) staff       (20)    30983 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/pdb/pdbfile.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    37300 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/pdb/pdbstructure.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13010 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/pdbx.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9202 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/prmtop.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9757 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/psf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1089 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/registry.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.451002 mdtraj-1.9.8/mdtraj/formats/tng/
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.394786 mdtraj-1.9.8/mdtraj/formats/tng/include/
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.454408 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2470 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/bwlzh.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      769 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/bwt.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2218 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/coder.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      514 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/dict.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1214 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/fixpoint.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      939 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/huffman.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      694 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/lz77.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      492 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/merge_sort.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1023 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/mtf.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      897 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/my64bit.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      586 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/rle.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     8905 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/tng_compress.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      601 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/vals16.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      718 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/warnmalloc.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      881 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/compression/widemuldiv.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.456358 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/
--rw-r--r--   0 mattthompson   (501) staff       (20)     4144 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/md5.h
--rw-r--r--   0 mattthompson   (501) staff       (20)   231837 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    67062 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io.hpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     1427 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io_fwd.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      399 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/include/tng/version.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.394987 mdtraj-1.9.8/mdtraj/formats/tng/src/
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.461243 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/
--rw-r--r--   0 mattthompson   (501) staff       (20)    26450 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/bwlzh.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    10102 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/bwt.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    15356 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/coder.c
--rw-r--r--   0 mattthompson   (501) staff       (20)      972 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/dict.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     2395 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/fixpoint.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    16577 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/huffman.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    15124 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/huffmem.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    10956 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/lz77.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     3397 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/merge_sort.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     6523 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/mtf.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     2073 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/rle.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    69288 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/tng_compress.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     1801 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/vals16.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     1047 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/warnmalloc.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     6472 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/widemuldiv.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    54276 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/xtc2.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    72060 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/compression/xtc3.c
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.462066 mdtraj-1.9.8/mdtraj/formats/tng/src/lib/
--rw-r--r--   0 mattthompson   (501) staff       (20)    13168 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/lib/md5.c
--rw-r--r--   0 mattthompson   (501) staff       (20)   607623 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/tng/src/lib/tng_io.c
--rw-r--r--   0 mattthompson   (501) staff       (20)   810249 2023-07-02 15:28:41.000000 mdtraj-1.9.8/mdtraj/formats/tng/tng.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    27834 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/tng/tng.pyx
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.467119 mdtraj-1.9.8/mdtraj/formats/xtc/
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.470054 mdtraj-1.9.8/mdtraj/formats/xtc/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)     8092 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/ms_stdint.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1247 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/trr_header.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      336 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/xdr_seek.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    23588 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2341 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile_trr.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2226 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile_xtc.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.471019 mdtraj-1.9.8/mdtraj/formats/xtc/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)     1453 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/src/xdr_seek.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    65257 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    15569 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile_trr.c
--rw-r--r--   0 mattthompson   (501) staff       (20)     4160 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile_xtc.c
--rw-r--r--   0 mattthompson   (501) staff       (20)  1002858 2023-07-02 15:28:42.000000 mdtraj-1.9.8/mdtraj/formats/xtc/trr.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    34762 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/xtc/trr.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)      985 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/trrlib.pxd
--rw-r--r--   0 mattthompson   (501) staff       (20)      793 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/formats/xtc/xdrlib.pxd
--rw-r--r--   0 mattthompson   (501) staff       (20)   936221 2023-07-02 15:28:42.000000 mdtraj-1.9.8/mdtraj/formats/xtc/xtc.c
--rw-r--r--   0 mattthompson   (501) staff       (20)    32028 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/xtc/xtc.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)    14121 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/formats/xyzfile.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.480271 mdtraj-1.9.8/mdtraj/geometry/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2412 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9825 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/alignment.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4301 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/angle.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13688 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/contact.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    23759 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/dihedral.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    19163 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/distance.py
--rw-r--r--   0 mattthompson   (501) staff       (20)   933749 2023-07-02 15:28:42.000000 mdtraj-1.9.8/mdtraj/geometry/drid.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     5063 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/drid.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)     3484 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/dssp.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    18311 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/hbond.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.494334 mdtraj-1.9.8/mdtraj/geometry/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)      320 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/dridkernels.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     3224 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/include/geometry.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      577 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/math_patch.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     3161 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/moments.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1413 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/msvccompat.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      230 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/neighborlist.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      261 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/neighbors.hpp
--rw-r--r--   0 mattthompson   (501) staff       (20)      326 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/sasa.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2714 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/include/vectorize.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    14549 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/include/vectorize_generic.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    15330 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/include/vectorize_neon.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    14042 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/include/vectorize_sse.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    20595 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/internal.py
--rw-r--r--   0 mattthompson   (501) staff       (20)   821217 2023-07-02 15:28:43.000000 mdtraj-1.9.8/mdtraj/geometry/neighborlist.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     3870 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/neighborlist.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)   854410 2023-07-02 15:28:43.000000 mdtraj-1.9.8/mdtraj/geometry/neighbors.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     5773 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/neighbors.pyx
--rwxr-xr-x   0 mattthompson   (501) staff       (20)    12604 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/order.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8022 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/rdf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2799 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/rg.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10018 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/sasa.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5326 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/shape.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.499944 mdtraj-1.9.8/mdtraj/geometry/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)  1159797 2023-07-02 15:28:44.000000 mdtraj-1.9.8/mdtraj/geometry/src/_geometry.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    11457 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/src/_geometry.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)     2409 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/dridkernels.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    15199 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/dssp.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    17473 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/src/geometry.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     6762 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/image_molecules.pxi
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.500546 mdtraj-1.9.8/mdtraj/geometry/src/kernels/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2605 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/kernels/anglekernels.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2888 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/kernels/dihedralkernels.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     7443 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/src/kernels/distancekernels.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     3791 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/moments.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    18175 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/neighborlist.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     2802 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/neighbors.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     9345 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/geometry/src/sasa.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     6591 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/geometry/thermodynamic_properties.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13392 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/io.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.501147 mdtraj-1.9.8/mdtraj/nmr/
--rw-r--r--   0 mattthompson   (501) staff       (20)      275 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/nmr/__init__.py
--rwxr-xr-x   0 mattthompson   (501) staff       (20)     8005 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/nmr/scalar_couplings.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    12252 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/nmr/shift_wrappers.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.502282 mdtraj-1.9.8/mdtraj/reporters/
--rw-r--r--   0 mattthompson   (501) staff       (20)      204 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/reporters/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10849 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/reporters/basereporter.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2555 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/reporters/dcdreporter.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/reporters/hdf5reporter.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3211 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/reporters/netcdfreporter.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5168 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/reporters/xtcreporter.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.504025 mdtraj-1.9.8/mdtraj/rmsd/
--rw-r--r--   0 mattthompson   (501) staff       (20)   527581 2023-07-02 15:28:44.000000 mdtraj-1.9.8/mdtraj/rmsd/_lprmsd.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    14170 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/_lprmsd.pyx
--rw-r--r--   0 mattthompson   (501) staff       (20)  1255926 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj/rmsd/_rmsd.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    32149 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/_rmsd.pyx
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.506343 mdtraj-1.9.8/mdtraj/rmsd/include/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2091 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/Munkres.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      250 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/center.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      254 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/euclidean_permutation.hpp
--rw-r--r--   0 mattthompson   (501) staff       (20)      234 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/fancy_index.hpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     1336 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/msvccompat.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      426 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/rotation.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    62135 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/sse_swizzle.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      810 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/theobald_rmsd.h
--rw-r--r--   0 mattthompson   (501) staff       (20)      825 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/include/util_arm.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     7125 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/include/util_sse.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.511014 mdtraj-1.9.8/mdtraj/rmsd/src/
--rw-r--r--   0 mattthompson   (501) staff       (20)     8636 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/Munkres.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)      234 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/center.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     4220 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/center_arm.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     1219 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/center_generic.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     4013 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/center_sse.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2272 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/euclidean_permutation.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     1520 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/fancy_index.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)      534 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/rotation.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)     5696 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/rotation_arm.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     3316 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/rotation_generic.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     6060 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/rotation_sse.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    10882 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd.cpp
--rw-r--r--   0 mattthompson   (501) staff       (20)    10253 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_arm.h
--rw-r--r--   0 mattthompson   (501) staff       (20)     2375 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_generic.h
--rw-r--r--   0 mattthompson   (501) staff       (20)    11547 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_sse.h
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.512295 mdtraj-1.9.8/mdtraj/scripts/
--rw-r--r--   0 mattthompson   (501) staff       (20)        0 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/scripts/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    20690 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/scripts/mdconvert.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8485 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/scripts/mdinspect.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.513389 mdtraj-1.9.8/mdtraj/testing/
--rw-r--r--   0 mattthompson   (501) staff       (20)     1142 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/testing/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    17166 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/testing/docscrape.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     7568 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/testing/docstrings.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     7047 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/testing/testing.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.516066 mdtraj-1.9.8/mdtraj/utils/
--rw-r--r--   0 mattthompson   (501) staff       (20)     3764 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1073 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/contextmanagers.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6995 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/delay_import.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4835 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/rotation.py
--rw-r--r--   0 mattthompson   (501) staff       (20)      440 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/singleton.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    20588 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/six.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.520318 mdtraj-1.9.8/mdtraj/utils/unit/
--rw-r--r--   0 mattthompson   (501) staff       (20)     6911 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/__init__.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3953 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/basedimension.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6929 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/baseunit.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2171 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/constants.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    21553 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/doctests.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13259 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/mymatrix.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6789 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/prefix.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    32230 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/quantity.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2372 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/standard_dimensions.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    26390 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/unit.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    13674 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/unit_definitions.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4600 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/unit_math.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5693 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/unit/unit_operators.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8245 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/unitcell.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8147 2022-10-27 15:00:02.000000 mdtraj-1.9.8/mdtraj/utils/validation.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1899 2022-11-06 01:55:17.000000 mdtraj-1.9.8/mdtraj/utils/zipped.py
--rw-r--r--   0 mattthompson   (501) staff       (20)      191 2023-07-02 15:28:32.000000 mdtraj-1.9.8/mdtraj/version.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.428260 mdtraj-1.9.8/mdtraj.egg-info/
--rw-r--r--   0 mattthompson   (501) staff       (20)     1515 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/PKG-INFO
--rw-r--r--   0 mattthompson   (501) staff       (20)     9750 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/SOURCES.txt
--rw-r--r--   0 mattthompson   (501) staff       (20)        1 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/dependency_links.txt
--rw-r--r--   0 mattthompson   (501) staff       (20)      116 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/entry_points.txt
--rw-r--r--   0 mattthompson   (501) staff       (20)        1 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/not-zip-safe
--rw-r--r--   0 mattthompson   (501) staff       (20)       38 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/requires.txt
--rw-r--r--   0 mattthompson   (501) staff       (20)        7 2023-07-02 15:28:45.000000 mdtraj-1.9.8/mdtraj.egg-info/top_level.txt
--rw-r--r--   0 mattthompson   (501) staff       (20)      338 2022-11-06 01:55:17.000000 mdtraj-1.9.8/pyproject.toml
--rw-r--r--   0 mattthompson   (501) staff       (20)       38 2023-07-02 15:28:45.541653 mdtraj-1.9.8/setup.cfg
--rw-r--r--   0 mattthompson   (501) staff       (20)    12764 2023-07-02 15:23:33.000000 mdtraj-1.9.8/setup.py
-drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-02 15:28:45.540897 mdtraj-1.9.8/tests/
--rw-r--r--   0 mattthompson   (501) staff       (20)     2333 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_alignment.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1543 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_angles.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1984 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_arc.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5182 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_binpos.py
--rw-r--r--   0 mattthompson   (501) staff       (20)      364 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_capi.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4391 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_contact.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1409 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_crd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9126 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_dcd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6980 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_dihedral.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10577 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_distance.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1032 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_docstrings.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2342 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_drid.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2862 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_dssp.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     9789 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_dtr.py
--rw-r--r--   0 mattthompson   (501) staff       (20)      913 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_element.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    15738 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_geometry.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4359 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_gro.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3075 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_gsd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5884 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_hbonds.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10187 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_hdf5.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2181 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_hoomdxml.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4978 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_io.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3556 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_lammpstrj.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4056 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_lh5.py
--rw-r--r--   0 mattthompson   (501) staff       (20)      796 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_load.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4012 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_lprmsd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     7326 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_mdconvert.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4365 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_mdcrd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     5786 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_mol2.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1178 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_neighborlist.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1848 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_neighbors.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8120 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_netcdf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3466 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_nmr.py
--rwxr-xr-x   0 mattthompson   (501) staff       (20)     5287 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_order.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    11681 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_pdb.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     2869 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_pdbx.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1751 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_prmtop.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4872 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_psf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1071 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_quaternion.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     7863 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_rdf.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10137 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_reporter.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     4202 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_restart.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     8893 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_rmsd.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1382 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_rmsd_memmap.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6328 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_sasa.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    10462 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_selection.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3289 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_shape.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6431 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_thermodynamic_properties.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1708 2023-06-10 20:05:00.000000 mdtraj-1.9.8/tests/test_tng.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    11347 2022-11-06 01:55:17.000000 mdtraj-1.9.8/tests/test_topology.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    27665 2023-06-10 20:02:15.000000 mdtraj-1.9.8/tests/test_trajectory.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    15530 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_trr.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     6192 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_utils.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1415 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_xml.py
--rw-r--r--   0 mattthompson   (501) staff       (20)    12672 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_xtc.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     3549 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_xyz.py
--rw-r--r--   0 mattthompson   (501) staff       (20)     1002 2022-10-27 15:00:03.000000 mdtraj-1.9.8/tests/test_zipped.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.552866 mdtraj-1.9.9/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    26530 2022-10-27 15:00:02.000000 mdtraj-1.9.9/LICENSE
+-rw-r--r--   0 mattthompson   (501) staff       (20)      184 2022-10-27 15:00:02.000000 mdtraj-1.9.9/MANIFEST.in
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1515 2023-07-22 15:19:59.552660 mdtraj-1.9.9/PKG-INFO
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3655 2023-07-18 04:26:08.000000 mdtraj-1.9.9/README.md
+-rw-r--r--   0 mattthompson   (501) staff       (20)    16701 2022-11-06 01:55:17.000000 mdtraj-1.9.9/basesetup.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.453639 mdtraj-1.9.9/examples/
+-rw-r--r--   0 mattthompson   (501) staff       (20)       20 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/.gitignore
+-rw-r--r--   0 mattthompson   (501) staff       (20)   145051 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/1vii_3frames.pdb
+-rw-r--r--   0 mattthompson   (501) staff       (20)    32402 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/ala2.h5
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7181 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/atom-selection.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3331 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/centroids.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3363 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/clustering.ipynb
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.454589 mdtraj-1.9.9/examples/data/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    98115 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/data/frame0.h5
+-rw-r--r--   0 mattthompson   (501) staff       (20)    72416 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/data/frame0.xtc
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1749 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/data/native.pdb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2880 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/hbonds.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3267 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/iterload.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4954 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/native-contact.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2064 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/nmr.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4194 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/principal-components.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2714 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/ramachandran-plot.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3943 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/rmsd-benchmark.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2316 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/rmsd-drift.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3989 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/simulation-with-openmm.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3547 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/solvent-accessible-surface-area.ipynb
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3087 2022-11-06 01:55:17.000000 mdtraj-1.9.9/examples/test_examples.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5324 2022-10-27 15:00:02.000000 mdtraj-1.9.9/examples/two-pass-clustering.ipynb
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.455273 mdtraj-1.9.9/mdtraj/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2628 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/__init__.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.469004 mdtraj-1.9.9/mdtraj/core/
+-rw-r--r--   0 mattthompson   (501) staff       (20)        0 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/core/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15631 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/core/element.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13043 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/core/residue_names.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15006 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/core/selection.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    61206 2023-06-10 19:37:18.000000 mdtraj-1.9.9/mdtraj/core/topology.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    81628 2023-06-10 19:37:18.000000 mdtraj-1.9.9/mdtraj/core/trajectory.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.474066 mdtraj-1.9.9/mdtraj/formats/
+-rw-r--r--   0 mattthompson   (501) staff       (20)      695 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    33372 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/amberrst.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13744 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/arc.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.475227 mdtraj-1.9.9/mdtraj/formats/binpos/
+-rw-r--r--   0 mattthompson   (501) staff       (20)   568749 2023-07-22 15:19:54.000000 mdtraj-1.9.9/mdtraj/formats/binpos/binpos.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    18845 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/binpos/binpos.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)      747 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/binposlib.pxd
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.476091 mdtraj-1.9.9/mdtraj/formats/binpos/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)      507 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/include/binposplugin.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1237 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/include/largefiles.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    38579 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/include/molfile_plugin.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/include/vmdplugin.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.476261 mdtraj-1.9.9/mdtraj/formats/binpos/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6989 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/binpos/src/binposplugin.c
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.477068 mdtraj-1.9.9/mdtraj/formats/dcd/
+-rw-r--r--   0 mattthompson   (501) staff       (20)   614920 2023-07-22 15:19:55.000000 mdtraj-1.9.9/mdtraj/formats/dcd/dcd.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    25481 2023-02-10 16:09:23.000000 mdtraj-1.9.9/mdtraj/formats/dcd/dcd.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1100 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/dcdlib.pxd
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.478297 mdtraj-1.9.9/mdtraj/formats/dcd/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2480 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/dcdplugin.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/endianswap.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10996 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/fastio.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1237 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/largefiles.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    38579 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/molfile_plugin.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/include/vmdplugin.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.478495 mdtraj-1.9.9/mdtraj/formats/dcd/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    39616 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dcd/src/dcdplugin.c
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.479388 mdtraj-1.9.9/mdtraj/formats/dtr/
+-rw-r--r--   0 mattthompson   (501) staff       (20)   634501 2023-07-22 15:19:55.000000 mdtraj-1.9.9/mdtraj/formats/dtr/dtr.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    29095 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/dtr/dtr.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1163 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/dtrlib.pxd
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.480268 mdtraj-1.9.9/mdtraj/formats/dtr/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10359 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/include/dtrplugin.hxx
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/include/endianswap.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    39114 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/include/molfile_plugin.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2734 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/include/vmddir.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6252 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/include/vmdplugin.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.480472 mdtraj-1.9.9/mdtraj/formats/dtr/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    70106 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/dtr/src/dtrplugin.cxx
+-rw-r--r--   0 mattthompson   (501) staff       (20)    21010 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/gro.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    11184 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/gsd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    40764 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/hdf5.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5880 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/hoomdxml.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    23510 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/lammpstrj.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    17956 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/lh5.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    18399 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/mdcrd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9937 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/mol2.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    23226 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/netcdf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2835 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/openmmxml.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.481241 mdtraj-1.9.9/mdtraj/formats/pdb/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1131 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/pdb/__init__.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.482076 mdtraj-1.9.9/mdtraj/formats/pdb/data/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9967 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/pdb/data/pdbNames.xml
+-rw-r--r--   0 mattthompson   (501) staff       (20)    24621 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/pdb/data/residues.xml
+-rw-r--r--   0 mattthompson   (501) staff       (20)    30983 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/pdb/pdbfile.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    37300 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/pdb/pdbstructure.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13010 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/pdbx.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9202 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/prmtop.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9757 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/psf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1089 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/registry.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.483116 mdtraj-1.9.9/mdtraj/formats/tng/
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.435918 mdtraj-1.9.9/mdtraj/formats/tng/include/
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.486135 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2470 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/bwlzh.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      769 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/bwt.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2218 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/coder.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      514 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/dict.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1214 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/fixpoint.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      939 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/huffman.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      694 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/lz77.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      492 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/merge_sort.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1023 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/mtf.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      897 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/my64bit.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      586 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/rle.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8905 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/tng_compress.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      601 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/vals16.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      718 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/warnmalloc.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      881 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/compression/widemuldiv.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.488010 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4144 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/md5.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)   231837 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    67062 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io.hpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1427 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io_fwd.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      399 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/include/tng/version.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.436140 mdtraj-1.9.9/mdtraj/formats/tng/src/
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.491628 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    26450 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/bwlzh.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10102 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/bwt.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15356 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/coder.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)      972 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/dict.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2395 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/fixpoint.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    16577 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/huffman.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15124 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/huffmem.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10956 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/lz77.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3397 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/merge_sort.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6523 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/mtf.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2073 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/rle.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    69288 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/tng_compress.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1801 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/vals16.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1047 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/warnmalloc.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6472 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/widemuldiv.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    54276 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/xtc2.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    72060 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/compression/xtc3.c
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.492098 mdtraj-1.9.9/mdtraj/formats/tng/src/lib/
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13168 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/lib/md5.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)   607623 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/tng/src/lib/tng_io.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)   809886 2023-07-22 15:19:55.000000 mdtraj-1.9.9/mdtraj/formats/tng/tng.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    27834 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/tng/tng.pyx
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.495180 mdtraj-1.9.9/mdtraj/formats/xtc/
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.498247 mdtraj-1.9.9/mdtraj/formats/xtc/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8092 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/ms_stdint.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1247 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/trr_header.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      336 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/xdr_seek.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    23588 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2341 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile_trr.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2226 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile_xtc.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.498986 mdtraj-1.9.9/mdtraj/formats/xtc/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1453 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/src/xdr_seek.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    65257 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15569 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile_trr.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4160 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile_xtc.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)  1003484 2023-07-22 15:19:55.000000 mdtraj-1.9.9/mdtraj/formats/xtc/trr.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    34762 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/xtc/trr.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)      985 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/trrlib.pxd
+-rw-r--r--   0 mattthompson   (501) staff       (20)      793 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/formats/xtc/xdrlib.pxd
+-rw-r--r--   0 mattthompson   (501) staff       (20)   936847 2023-07-22 15:19:56.000000 mdtraj-1.9.9/mdtraj/formats/xtc/xtc.c
+-rw-r--r--   0 mattthompson   (501) staff       (20)    32028 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/xtc/xtc.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)    14121 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/formats/xyzfile.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.507953 mdtraj-1.9.9/mdtraj/geometry/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2412 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9825 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/alignment.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4301 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/angle.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13688 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/contact.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    23759 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/dihedral.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    19163 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/distance.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)   934917 2023-07-22 15:19:56.000000 mdtraj-1.9.9/mdtraj/geometry/drid.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5063 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/drid.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3484 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/dssp.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    18311 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/hbond.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.509964 mdtraj-1.9.9/mdtraj/geometry/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)      320 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/dridkernels.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3224 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/include/geometry.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      577 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/math_patch.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3161 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/moments.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1413 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/msvccompat.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      230 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/neighborlist.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      261 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/neighbors.hpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)      326 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/sasa.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2714 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/include/vectorize.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    14549 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/include/vectorize_generic.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15330 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/include/vectorize_neon.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    14042 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/include/vectorize_sse.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    20595 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/internal.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)   822395 2023-07-22 15:19:56.000000 mdtraj-1.9.9/mdtraj/geometry/neighborlist.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3870 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/neighborlist.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)   855588 2023-07-22 15:19:57.000000 mdtraj-1.9.9/mdtraj/geometry/neighbors.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5773 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/neighbors.pyx
+-rwxr-xr-x   0 mattthompson   (501) staff       (20)    12604 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/order.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8022 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/rdf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2799 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/rg.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10018 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/sasa.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5326 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/shape.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.512599 mdtraj-1.9.9/mdtraj/geometry/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)  1160450 2023-07-22 15:19:58.000000 mdtraj-1.9.9/mdtraj/geometry/src/_geometry.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    11457 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/src/_geometry.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2409 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/dridkernels.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15199 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/dssp.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    17473 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/src/geometry.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6762 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/image_molecules.pxi
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.513086 mdtraj-1.9.9/mdtraj/geometry/src/kernels/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2605 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/kernels/anglekernels.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2888 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/kernels/dihedralkernels.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7443 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/src/kernels/distancekernels.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3791 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/moments.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    18175 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/neighborlist.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2802 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/neighbors.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9345 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/geometry/src/sasa.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6591 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/geometry/thermodynamic_properties.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13392 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/io.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.513777 mdtraj-1.9.9/mdtraj/nmr/
+-rw-r--r--   0 mattthompson   (501) staff       (20)      275 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/nmr/__init__.py
+-rwxr-xr-x   0 mattthompson   (501) staff       (20)     8005 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/nmr/scalar_couplings.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    12252 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/nmr/shift_wrappers.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.515222 mdtraj-1.9.9/mdtraj/reporters/
+-rw-r--r--   0 mattthompson   (501) staff       (20)      204 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/reporters/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10849 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/reporters/basereporter.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2555 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/reporters/dcdreporter.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4749 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/reporters/hdf5reporter.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3211 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/reporters/netcdfreporter.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5168 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/reporters/xtcreporter.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.517759 mdtraj-1.9.9/mdtraj/rmsd/
+-rw-r--r--   0 mattthompson   (501) staff       (20)   528188 2023-07-22 15:19:58.000000 mdtraj-1.9.9/mdtraj/rmsd/_lprmsd.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    14170 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/_lprmsd.pyx
+-rw-r--r--   0 mattthompson   (501) staff       (20)  1257154 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj/rmsd/_rmsd.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    32149 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/_rmsd.pyx
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.529479 mdtraj-1.9.9/mdtraj/rmsd/include/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2091 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/Munkres.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      250 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/center.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      254 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/euclidean_permutation.hpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)      234 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/fancy_index.hpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1336 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/msvccompat.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      426 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/rotation.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    62135 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/sse_swizzle.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      810 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/theobald_rmsd.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)      825 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/include/util_arm.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7125 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/include/util_sse.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.532202 mdtraj-1.9.9/mdtraj/rmsd/src/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8636 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/Munkres.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)      234 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/center.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4220 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/center_arm.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1219 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/center_generic.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4013 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/center_sse.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2272 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/euclidean_permutation.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1520 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/fancy_index.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)      534 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/rotation.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5696 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/rotation_arm.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3316 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/rotation_generic.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6060 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/rotation_sse.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10882 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd.cpp
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10253 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_arm.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2375 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_generic.h
+-rw-r--r--   0 mattthompson   (501) staff       (20)    11547 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_sse.h
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.532695 mdtraj-1.9.9/mdtraj/scripts/
+-rw-r--r--   0 mattthompson   (501) staff       (20)        0 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/scripts/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    20690 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/scripts/mdconvert.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8485 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/scripts/mdinspect.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.533438 mdtraj-1.9.9/mdtraj/testing/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1142 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/testing/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    17166 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/testing/docscrape.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7568 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/testing/docstrings.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7047 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/testing/testing.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.535629 mdtraj-1.9.9/mdtraj/utils/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3764 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1073 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/contextmanagers.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6995 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/delay_import.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4835 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/rotation.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)      440 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/singleton.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    20588 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/six.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.538999 mdtraj-1.9.9/mdtraj/utils/unit/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6911 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/__init__.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3953 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/basedimension.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6929 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/baseunit.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2171 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/constants.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    21553 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/doctests.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13259 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/mymatrix.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6789 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/prefix.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    32230 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/quantity.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2372 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/standard_dimensions.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    26390 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/unit.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    13674 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/unit_definitions.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4600 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/unit_math.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5693 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/unit/unit_operators.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8245 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/unitcell.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8147 2022-10-27 15:00:02.000000 mdtraj-1.9.9/mdtraj/utils/validation.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1899 2022-11-06 01:55:17.000000 mdtraj-1.9.9/mdtraj/utils/zipped.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)      191 2023-07-22 15:19:53.000000 mdtraj-1.9.9/mdtraj/version.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.467099 mdtraj-1.9.9/mdtraj.egg-info/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1515 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/PKG-INFO
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9750 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/SOURCES.txt
+-rw-r--r--   0 mattthompson   (501) staff       (20)        1 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/dependency_links.txt
+-rw-r--r--   0 mattthompson   (501) staff       (20)      116 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/entry_points.txt
+-rw-r--r--   0 mattthompson   (501) staff       (20)        1 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/not-zip-safe
+-rw-r--r--   0 mattthompson   (501) staff       (20)       38 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/requires.txt
+-rw-r--r--   0 mattthompson   (501) staff       (20)        7 2023-07-22 15:19:59.000000 mdtraj-1.9.9/mdtraj.egg-info/top_level.txt
+-rw-r--r--   0 mattthompson   (501) staff       (20)      174 2023-07-18 17:54:33.000000 mdtraj-1.9.9/pyproject.toml
+-rw-r--r--   0 mattthompson   (501) staff       (20)       38 2023-07-22 15:19:59.552913 mdtraj-1.9.9/setup.cfg
+-rw-r--r--   0 mattthompson   (501) staff       (20)    12764 2023-07-22 15:17:13.000000 mdtraj-1.9.9/setup.py
+drwxr-xr-x   0 mattthompson   (501) staff       (20)        0 2023-07-22 15:19:59.552372 mdtraj-1.9.9/tests/
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2333 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_alignment.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1543 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_angles.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1984 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_arc.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5182 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_binpos.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)      364 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_capi.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4391 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_contact.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1409 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_crd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9126 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_dcd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6980 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_dihedral.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10577 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_distance.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1032 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_docstrings.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2342 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_drid.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2862 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_dssp.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     9789 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_dtr.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)      913 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_element.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15738 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_geometry.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4359 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_gro.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3075 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_gsd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5884 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_hbonds.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10187 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_hdf5.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2181 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_hoomdxml.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4978 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_io.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3556 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_lammpstrj.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4056 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_lh5.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)      796 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_load.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4012 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_lprmsd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7326 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_mdconvert.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4365 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_mdcrd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     5786 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_mol2.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1178 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_neighborlist.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1848 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_neighbors.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8120 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_netcdf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3466 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_nmr.py
+-rwxr-xr-x   0 mattthompson   (501) staff       (20)     5287 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_order.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    11681 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_pdb.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     2869 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_pdbx.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1751 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_prmtop.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4872 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_psf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1071 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_quaternion.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     7863 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_rdf.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10137 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_reporter.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     4202 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_restart.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     8893 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_rmsd.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1382 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_rmsd_memmap.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6328 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_sasa.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    10462 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_selection.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3289 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_shape.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6431 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_thermodynamic_properties.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1708 2023-06-10 20:05:00.000000 mdtraj-1.9.9/tests/test_tng.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    11347 2022-11-06 01:55:17.000000 mdtraj-1.9.9/tests/test_topology.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    27665 2023-06-10 20:02:15.000000 mdtraj-1.9.9/tests/test_trajectory.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    15530 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_trr.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     6192 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_utils.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1415 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_xml.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)    12672 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_xtc.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     3549 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_xyz.py
+-rw-r--r--   0 mattthompson   (501) staff       (20)     1002 2022-10-27 15:00:03.000000 mdtraj-1.9.9/tests/test_zipped.py
```

### Comparing `mdtraj-1.9.8/LICENSE` & `mdtraj-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/PKG-INFO` & `mdtraj-1.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdtraj
-Version: 1.9.8
+Version: 1.9.9
 Summary: MDTraj: A modern, open library for the analysis of molecular dynamics trajectories
 Home-page: http://mdtraj.org
 Download-URL: https://github.com/rmcgibbo/mdtraj/releases/latest
 Author: Robert McGibbon
 Author-email: rmcgibbo@gmail.com
 License: LGPLv2.1+
 Platform: Linux
```

### Comparing `mdtraj-1.9.8/README.md` & `mdtraj-1.9.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 ## Note on current project status
 
-Hi there!
+TLDR: MDTraj is currently undergoing a transition to new maintainers (the Folding@home consortium).
+Please bear with us as we slowly respond to issues and clean up.
 
-MDTraj is a project that I (@rmcgibbo) primarily developed between 2013 and 2016 while I was a
-graduate student. That was a long time ago! I've moved on, and no longer use MDTraj in my
-current role. Most of the other contributors from that time have similarly moved on. I do
-respond to github issues and pull requests from time to time, but my bandwidth is limited so
-don't expect to necessarily get a response on github issues from me. (Also **please** don't
-email me with support requests).
-
-MDTraj is looking for new maintainers! I would be happy to transfer ownership and responsibility
-of the code base to another group of maintainers. Please reach out to me if you're interested in
-taking over the project.
+Hello!
+
+For anybody wondering, the MDTraj repo is currently undergoing a transition to new maintainers;
+The Folding@home consortium (@FoldingAtHome) will now be taking over support, maintainence
+and management of MDTraj with @xuhuihuang leading repo management, and @mattwthompson, @apayne97,
+and myself (@sukritsingh) helping to manage and maintain this repo more directly.
+
+Existing supporters, contributors, etc. are all welcome to contribute as much as they wish.
+The intention behind this transition is to ensure MDTraj receives continued support.
+
+As we are slowly transitioning to this new support, please bear with us as we slowly respond
+to issues, clean up any PRs, etc.
+
+I have opened a [Discussions page](https://github.com/mdtraj/mdtraj/discussions) on github
+for folks asking for help with code issues/not getting things working. Our hope is that the
+issues page will be for discrete bugs, feature requests, related discussions etc., but this
+is very flexible!
 
 Best,
 
-Robert T. McGibbon (@rmcgibbo)
+Sukrit Singh (@sukritsingh)
 
-May 2, 2022
+July 6th, 2023
 
 --------------------------------
 
 ## MDTraj: an open-source library for analysis of molecular dynamics trajectories
 
 [![Build Status](https://github.com/mdtraj/mdtraj/actions/workflows/main.yaml/badge.svg)](https://github.com/mdtraj/mdtraj/actions)
 [![PyPI Version](https://badge.fury.io/py/mdtraj.svg)](https://pypi.python.org/pypi/mdtraj)
```

### Comparing `mdtraj-1.9.8/basesetup.py` & `mdtraj-1.9.9/basesetup.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/1vii_3frames.pdb` & `mdtraj-1.9.9/examples/1vii_3frames.pdb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/ala2.h5` & `mdtraj-1.9.9/examples/ala2.h5`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/atom-selection.ipynb` & `mdtraj-1.9.9/examples/atom-selection.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/centroids.ipynb` & `mdtraj-1.9.9/examples/centroids.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/clustering.ipynb` & `mdtraj-1.9.9/examples/clustering.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/data/frame0.h5` & `mdtraj-1.9.9/examples/data/frame0.h5`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/data/frame0.xtc` & `mdtraj-1.9.9/examples/data/frame0.xtc`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/data/native.pdb` & `mdtraj-1.9.9/examples/data/native.pdb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/hbonds.ipynb` & `mdtraj-1.9.9/examples/hbonds.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/iterload.ipynb` & `mdtraj-1.9.9/examples/iterload.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/native-contact.ipynb` & `mdtraj-1.9.9/examples/native-contact.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/nmr.ipynb` & `mdtraj-1.9.9/examples/nmr.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/principal-components.ipynb` & `mdtraj-1.9.9/examples/principal-components.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/ramachandran-plot.ipynb` & `mdtraj-1.9.9/examples/ramachandran-plot.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/rmsd-benchmark.ipynb` & `mdtraj-1.9.9/examples/rmsd-benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/rmsd-drift.ipynb` & `mdtraj-1.9.9/examples/rmsd-drift.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/simulation-with-openmm.ipynb` & `mdtraj-1.9.9/examples/simulation-with-openmm.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/solvent-accessible-surface-area.ipynb` & `mdtraj-1.9.9/examples/solvent-accessible-surface-area.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/test_examples.py` & `mdtraj-1.9.9/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/examples/two-pass-clustering.ipynb` & `mdtraj-1.9.9/examples/two-pass-clustering.ipynb`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/__init__.py` & `mdtraj-1.9.9/mdtraj/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/core/element.py` & `mdtraj-1.9.9/mdtraj/core/element.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/core/residue_names.py` & `mdtraj-1.9.9/mdtraj/core/residue_names.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/core/selection.py` & `mdtraj-1.9.9/mdtraj/core/selection.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/core/topology.py` & `mdtraj-1.9.9/mdtraj/core/topology.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/core/trajectory.py` & `mdtraj-1.9.9/mdtraj/core/trajectory.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/__init__.py` & `mdtraj-1.9.9/mdtraj/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/amberrst.py` & `mdtraj-1.9.9/mdtraj/formats/amberrst.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/arc.py` & `mdtraj-1.9.9/mdtraj/formats/arc.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/binpos.c` & `mdtraj-1.9.9/mdtraj/formats/binpos/binpos.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/formats/binpos/include/",
             "mdtraj/formats/binpos/",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "mdtraj.formats.binpos",
         "sources": [
             "mdtraj/formats/binpos/binpos.pyx",
             "mdtraj/formats/binpos/src/binposplugin.c"
         ]
     },
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -111,15 +111,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -395,17 +395,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -475,14 +472,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1057,177 +1059,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1255,42 +1257,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6mdtraj_7formats_6binpos_BINPOSTrajectoryFile;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1836,30 +1838,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -7161,15 +7163,15 @@
   __Pyx_AddTraceback("mdtraj.formats.binpos.BINPOSTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7178,29 +7180,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7211,15 +7213,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7228,29 +7230,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7261,15 +7263,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7278,29 +7280,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7311,15 +7313,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7328,29 +7330,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7361,15 +7363,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7378,29 +7380,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7411,89 +7413,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7501,33 +7503,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7535,96 +7537,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7640,15 +7642,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7656,53 +7658,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -7710,30 +7712,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7748,15 +7750,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7772,15 +7774,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7788,53 +7790,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -7842,30 +7844,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7880,15 +7882,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7904,15 +7906,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7920,53 +7922,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -7974,30 +7976,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8012,176 +8014,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8203,15 +8205,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_6binpos_BINPOSTrajectoryFile(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -8690,26 +8692,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -8821,39 +8823,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -9301,15 +9303,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_binpos_line_60, __pyx_kp_u_load_binpos_filename_top_None_st) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12167,18 +12169,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -12224,22 +12226,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/binpos.pyx` & `mdtraj-1.9.9/mdtraj/formats/binpos/binpos.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/binposlib.pxd` & `mdtraj-1.9.9/mdtraj/formats/binpos/binposlib.pxd`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/include/largefiles.h` & `mdtraj-1.9.9/mdtraj/formats/binpos/include/largefiles.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/include/molfile_plugin.h` & `mdtraj-1.9.9/mdtraj/formats/binpos/include/molfile_plugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/include/vmdplugin.h` & `mdtraj-1.9.9/mdtraj/formats/binpos/include/vmdplugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/binpos/src/binposplugin.c` & `mdtraj-1.9.9/mdtraj/formats/binpos/src/binposplugin.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/dcd.c` & `mdtraj-1.9.9/mdtraj/formats/dcd/dcd.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/formats/dcd/include/",
             "mdtraj/formats/dcd/",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "mdtraj.formats.dcd",
         "sources": [
             "mdtraj/formats/dcd/dcd.pyx",
             "mdtraj/formats/dcd/src/dcdplugin.c"
         ]
     },
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -111,15 +111,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -395,17 +395,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -475,14 +472,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1057,177 +1059,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1255,42 +1257,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6mdtraj_7formats_3dcd_DCDTrajectoryFile;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1620,14 +1622,31 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
@@ -1738,30 +1757,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3170,15 +3189,15 @@
  *             if self.fh is NULL:
  *                 raise IOError("Could not open file: %s" % filename)
  *             assert self.n_atoms > 0, 'DCD Corruption: n_atoms was not positive'             # <<<<<<<<<<<<<<
  *             assert self.n_frames >= 0, 'DCD corruption: n_frames < 0'
  *             self.is_open = True
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_self->n_atoms > 0) != 0))) {
         PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_DCD_Corruption_n_atoms_was_not_p);
         __PYX_ERR(0, 222, __pyx_L1_error)
       }
     }
     #endif
 
@@ -3186,15 +3205,15 @@
  *                 raise IOError("Could not open file: %s" % filename)
  *             assert self.n_atoms > 0, 'DCD Corruption: n_atoms was not positive'
  *             assert self.n_frames >= 0, 'DCD corruption: n_frames < 0'             # <<<<<<<<<<<<<<
  *             self.is_open = True
  *         elif str(mode) == 'w':
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_self->n_frames >= 0) != 0))) {
         PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_DCD_corruption_n_frames_0);
         __PYX_ERR(0, 223, __pyx_L1_error)
       }
     }
     #endif
 
@@ -3588,15 +3607,15 @@
  *         is delayed until the first call to write()
  *         """
  *         assert not self.is_open and self._needs_write_initialization             # <<<<<<<<<<<<<<
  * 
  *         self.n_atoms = n_atoms
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = ((!(__pyx_v_self->is_open != 0)) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L3_bool_binop_done;
     }
     __pyx_t_2 = (__pyx_v_self->_needs_write_initialization != 0);
@@ -8197,15 +8216,15 @@
   __Pyx_AddTraceback("mdtraj.formats.dcd.DCDTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8214,29 +8233,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8247,15 +8266,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8264,29 +8283,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8297,15 +8316,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8314,29 +8333,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8347,15 +8366,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8364,29 +8383,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8397,15 +8416,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8414,29 +8433,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8447,89 +8466,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8537,33 +8556,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8571,96 +8590,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8676,15 +8695,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8692,53 +8711,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -8746,30 +8765,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8784,15 +8803,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8808,15 +8827,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8824,53 +8843,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -8878,30 +8897,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8916,15 +8935,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8940,15 +8959,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8956,53 +8975,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -9010,30 +9029,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9048,176 +9067,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9243,15 +9262,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_3dcd_DCDTrajectoryFile(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -9817,26 +9836,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -9869,14 +9888,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -9969,39 +9993,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10460,15 +10484,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_dcd_line_71, __pyx_kp_u_load_dcd_filename_top_None_strid) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12683,18 +12707,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -12740,22 +12764,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/dcd.pyx` & `mdtraj-1.9.9/mdtraj/formats/dcd/dcd.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/dcdlib.pxd` & `mdtraj-1.9.9/mdtraj/formats/dcd/dcdlib.pxd`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/dcdplugin.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/dcdplugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/endianswap.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/endianswap.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/fastio.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/fastio.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/largefiles.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/largefiles.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/molfile_plugin.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/molfile_plugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/include/vmdplugin.h` & `mdtraj-1.9.9/mdtraj/formats/dcd/include/vmdplugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dcd/src/dcdplugin.c` & `mdtraj-1.9.9/mdtraj/formats/dcd/src/dcdplugin.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/dtr.cpp` & `mdtraj-1.9.9/mdtraj/formats/dtr/dtr.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "DESRES_READ_TIMESTEP2",
                 1
             ]
         ],
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/formats/dtr/include/",
             "mdtraj/formats/dtr/",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj.formats.dtr",
         "sources": [
             "mdtraj/formats/dtr/dtr.pyx",
             "mdtraj/formats/dtr/src/dtrplugin.cxx"
         ]
@@ -42,16 +42,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -118,15 +118,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -416,17 +416,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -496,14 +493,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1078,177 +1080,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1276,42 +1278,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6mdtraj_7formats_3dtr_DTRTrajectoryFile;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1642,14 +1644,31 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
@@ -1765,30 +1784,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3521,15 +3540,15 @@
  *             if self.fh is NULL:
  *                 raise IOError("Could not open file: %s" % filename)
  *             assert self.n_atoms > 0, 'dtr Corruption: n_atoms was not positive'             # <<<<<<<<<<<<<<
  *             read_timestep_metadata(self.fh, &self.metadata)
  *             self.n_frames = self.metadata.count
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_self->n_atoms > 0) != 0))) {
         PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_dtr_Corruption_n_atoms_was_not_p);
         __PYX_ERR(0, 284, __pyx_L1_error)
       }
     }
     #endif
 
@@ -3959,15 +3978,15 @@
  *         is delayed until the first call to write()
  *         """
  *         assert not self.is_open and self._needs_write_initialization             # <<<<<<<<<<<<<<
  * 
  *         self.n_atoms = n_atoms
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = ((!(__pyx_v_self->is_open != 0)) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L3_bool_binop_done;
     }
     __pyx_t_2 = (__pyx_v_self->_needs_write_initialization != 0);
@@ -8512,15 +8531,15 @@
   __Pyx_AddTraceback("mdtraj.formats.dtr.DTRTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8529,29 +8548,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8562,15 +8581,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8579,29 +8598,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8612,15 +8631,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8629,29 +8648,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8662,15 +8681,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8679,29 +8698,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8712,15 +8731,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8729,29 +8748,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8762,89 +8781,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8852,33 +8871,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8886,96 +8905,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8991,15 +9010,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9007,53 +9026,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -9061,30 +9080,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9099,15 +9118,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9123,15 +9142,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9139,53 +9158,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -9193,30 +9212,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9231,15 +9250,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9255,15 +9274,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9271,53 +9290,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -9325,30 +9344,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9363,176 +9382,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9558,15 +9577,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_3dtr_DTRTrajectoryFile(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -10145,26 +10164,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -10232,14 +10251,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -10322,39 +10346,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10855,15 +10879,15 @@
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_dtr_line_85, __pyx_kp_u_load_dtr_filename_top_None_strid) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_stk_line_163, __pyx_kp_u_load_dtr_filename_top_None_strid_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -13169,18 +13193,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -13226,22 +13250,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/dtr.pyx` & `mdtraj-1.9.9/mdtraj/formats/dtr/dtr.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/dtrlib.pxd` & `mdtraj-1.9.9/mdtraj/formats/dtr/dtrlib.pxd`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/include/dtrplugin.hxx` & `mdtraj-1.9.9/mdtraj/formats/dtr/include/dtrplugin.hxx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/include/endianswap.h` & `mdtraj-1.9.9/mdtraj/formats/dtr/include/endianswap.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/include/molfile_plugin.h` & `mdtraj-1.9.9/mdtraj/formats/dtr/include/molfile_plugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/include/vmddir.h` & `mdtraj-1.9.9/mdtraj/formats/dtr/include/vmddir.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/include/vmdplugin.h` & `mdtraj-1.9.9/mdtraj/formats/dtr/include/vmdplugin.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/dtr/src/dtrplugin.cxx` & `mdtraj-1.9.9/mdtraj/formats/dtr/src/dtrplugin.cxx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/gro.py` & `mdtraj-1.9.9/mdtraj/formats/gro.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/gsd.py` & `mdtraj-1.9.9/mdtraj/formats/gsd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/hdf5.py` & `mdtraj-1.9.9/mdtraj/formats/hdf5.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/hoomdxml.py` & `mdtraj-1.9.9/mdtraj/formats/hoomdxml.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/lammpstrj.py` & `mdtraj-1.9.9/mdtraj/formats/lammpstrj.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/lh5.py` & `mdtraj-1.9.9/mdtraj/formats/lh5.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/mdcrd.py` & `mdtraj-1.9.9/mdtraj/formats/mdcrd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/mol2.py` & `mdtraj-1.9.9/mdtraj/formats/mol2.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/netcdf.py` & `mdtraj-1.9.9/mdtraj/formats/netcdf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/openmmxml.py` & `mdtraj-1.9.9/mdtraj/formats/openmmxml.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdb/__init__.py` & `mdtraj-1.9.9/mdtraj/formats/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdb/data/pdbNames.xml` & `mdtraj-1.9.9/mdtraj/formats/pdb/data/pdbNames.xml`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdb/data/residues.xml` & `mdtraj-1.9.9/mdtraj/formats/pdb/data/residues.xml`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdb/pdbfile.py` & `mdtraj-1.9.9/mdtraj/formats/pdb/pdbfile.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdb/pdbstructure.py` & `mdtraj-1.9.9/mdtraj/formats/pdb/pdbstructure.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/pdbx.py` & `mdtraj-1.9.9/mdtraj/formats/pdbx.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/prmtop.py` & `mdtraj-1.9.9/mdtraj/formats/prmtop.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/psf.py` & `mdtraj-1.9.9/mdtraj/formats/psf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/registry.py` & `mdtraj-1.9.9/mdtraj/formats/registry.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/bwlzh.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/bwlzh.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/bwt.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/bwt.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/coder.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/coder.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/dict.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/dict.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/fixpoint.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/fixpoint.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/huffman.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/huffman.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/lz77.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/lz77.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/mtf.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/mtf.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/my64bit.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/my64bit.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/rle.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/rle.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/tng_compress.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/tng_compress.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/vals16.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/vals16.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/warnmalloc.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/warnmalloc.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/compression/widemuldiv.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/compression/widemuldiv.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/tng/md5.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/tng/md5.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io.hpp` & `mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io.hpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/include/tng/tng_io_fwd.h` & `mdtraj-1.9.9/mdtraj/formats/tng/include/tng/tng_io_fwd.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/bwlzh.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/bwlzh.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/bwt.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/bwt.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/coder.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/coder.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/dict.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/dict.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/fixpoint.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/fixpoint.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/huffman.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/huffman.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/huffmem.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/huffmem.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/lz77.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/lz77.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/merge_sort.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/merge_sort.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/mtf.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/mtf.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/rle.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/rle.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/tng_compress.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/tng_compress.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/vals16.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/vals16.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/warnmalloc.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/warnmalloc.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/widemuldiv.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/widemuldiv.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/xtc2.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/xtc2.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/compression/xtc3.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/compression/xtc3.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/lib/md5.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/lib/md5.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/src/lib/tng_io.c` & `mdtraj-1.9.9/mdtraj/formats/tng/src/lib/tng_io.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/tng.c` & `mdtraj-1.9.9/mdtraj/formats/tng/tng.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "USE_ZLIB",
                 1
             ]
         ],
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "mdtraj/formats/tng/include/tng/tng_io.h"
         ],
         "include_dirs": [
             "mdtraj/formats/tng/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/include",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "libraries": [
             "z"
         ],
         "library_dirs": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib"
         ],
         "name": "mdtraj.formats.tng",
         "sources": [
             "mdtraj/formats/tng/tng.pyx",
             "mdtraj/formats/tng/src/compression/dict.c",
             "mdtraj/formats/tng/src/compression/bwt.c",
             "mdtraj/formats/tng/src/compression/tng_compress.c",
@@ -61,16 +61,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -137,15 +137,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -421,17 +421,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -501,14 +498,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1083,177 +1085,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1286,42 +1288,42 @@
 struct __pyx_obj_6mdtraj_7formats_3tng_TNGTrajectoryFile;
 struct __pyx_obj_6mdtraj_7formats_3tng___pyx_scope_struct___read_topology;
 struct __pyx_obj_6mdtraj_7formats_3tng___pyx_scope_struct_1_genexpr;
 struct __pyx_obj_6mdtraj_7formats_3tng___pyx_scope_struct_2_genexpr;
 struct __pyx_obj_6mdtraj_7formats_3tng___pyx_scope_struct_3_read;
 struct __pyx_obj_6mdtraj_7formats_3tng___pyx_scope_struct_4_genexpr;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1964,30 +1966,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -10389,15 +10391,15 @@
   __Pyx_AddTraceback("mdtraj.formats.tng.TNGTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10406,29 +10408,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10439,15 +10441,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10456,29 +10458,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10489,15 +10491,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10506,29 +10508,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10539,15 +10541,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10556,29 +10558,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10589,15 +10591,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10606,29 +10608,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10639,89 +10641,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -10729,33 +10731,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -10763,96 +10765,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10868,15 +10870,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -10884,53 +10886,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -10938,30 +10940,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10976,15 +10978,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11000,15 +11002,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11016,53 +11018,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -11070,30 +11072,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11108,15 +11110,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11132,15 +11134,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11148,53 +11150,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -11202,30 +11204,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11240,176 +11242,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -11435,15 +11437,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_3tng_TNGTrajectoryFile(PyObject *o) {
   struct __pyx_obj_6mdtraj_7formats_3tng_TNGTrajectoryFile *p = (struct __pyx_obj_6mdtraj_7formats_3tng_TNGTrajectoryFile *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -12745,26 +12747,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -12916,39 +12918,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -13429,15 +13431,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_tng_line_145, __pyx_kp_u_load_tng_filename_top_None_strid) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16102,18 +16104,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -16159,22 +16161,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/tng/tng.pyx` & `mdtraj-1.9.9/mdtraj/formats/tng/tng.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/include/ms_stdint.h` & `mdtraj-1.9.9/mdtraj/formats/xtc/include/ms_stdint.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/include/trr_header.h` & `mdtraj-1.9.9/mdtraj/formats/xtc/include/trr_header.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile.h` & `mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile_trr.h` & `mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/include/xdrfile_xtc.h` & `mdtraj-1.9.9/mdtraj/formats/xtc/include/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/src/xdr_seek.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/src/xdr_seek.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile_trr.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/src/xdrfile_xtc.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/src/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/trr.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/trr.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/formats/xtc/include/",
             "mdtraj/formats/xtc/",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "mdtraj.formats.trr",
         "sources": [
             "mdtraj/formats/xtc/trr.pyx",
             "mdtraj/formats/xtc/src/xdrfile.c",
             "mdtraj/formats/xtc/src/xdr_seek.c",
             "mdtraj/formats/xtc/src/xdrfile_trr.c"
@@ -37,16 +37,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -113,15 +113,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -397,17 +397,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -477,14 +474,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1061,177 +1063,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1282,42 +1284,42 @@
 struct __pyx_obj_6mdtraj_7formats_3trr_TRRTrajectoryFile;
 struct __pyx_obj_6mdtraj_7formats_3trr___pyx_scope_struct___estimate_n_frames_from_filesize;
 struct __pyx_obj_6mdtraj_7formats_3trr___pyx_scope_struct_1_genexpr;
 struct __pyx_obj_6mdtraj_7formats_3trr___pyx_scope_struct_2__calc_len_and_offsets;
 struct __pyx_obj_6mdtraj_7formats_3trr___pyx_scope_struct_3_genexpr;
 struct __pyx_obj_6mdtraj_7formats_3trr___pyx_scope_struct_4_genexpr;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1945,14 +1947,31 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* DivInt[__pyx_t_6mdtraj_7formats_3trr_int64_t].proto */
 static CYTHON_INLINE __pyx_t_6mdtraj_7formats_3trr_int64_t __Pyx_div___pyx_t_6mdtraj_7formats_3trr_int64_t(__pyx_t_6mdtraj_7formats_3trr_int64_t, __pyx_t_6mdtraj_7formats_3trr_int64_t);
 
 /* UnaryNegOverflows.proto */
 #define UNARY_NEG_WOULD_OVERFLOW(x)\
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
@@ -1985,30 +2004,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -6932,16 +6951,16 @@
   PyArrayObject *__pyx_v_lambd_stride = 0;
   PyArrayObject *__pyx_v_box_stride = 0;
   PyArrayObject *__pyx_v_vel = 0;
   PyArrayObject *__pyx_v_forces = 0;
   PyArrayObject *__pyx_v_xyz_buffer = 0;
   PyArrayObject *__pyx_v_vel_buffer = 0;
   PyArrayObject *__pyx_v_forces_buffer = 0;
-  void *__pyx_v_frame_vel;
-  void *__pyx_v_frame_forces;
+  rvec *__pyx_v_frame_vel;
+  rvec *__pyx_v_frame_forces;
   CYTHON_UNUSED PyObject *__pyx_v__ = NULL;
   int __pyx_v_seek_status;
   PyObject *__pyx_v_vel_return = NULL;
   PyObject *__pyx_v_forces_return = NULL;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_box;
   __Pyx_Buffer __pyx_pybuffer_box;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_box_stride;
@@ -11054,16 +11073,16 @@
 }
 
 static PyObject *__pyx_pf_6mdtraj_7formats_3trr_17TRRTrajectoryFile_18_write(struct __pyx_obj_6mdtraj_7formats_3trr_TRRTrajectoryFile *__pyx_v_self, PyArrayObject *__pyx_v_xyz, PyArrayObject *__pyx_v_time, PyArrayObject *__pyx_v_step, PyArrayObject *__pyx_v_box, PyArrayObject *__pyx_v_lambd, PyArrayObject *__pyx_v_vel, PyArrayObject *__pyx_v_forces) {
   int __pyx_v_n_frames;
   int __pyx_v_n_atoms;
   int __pyx_v_status;
   int __pyx_v_i;
-  rvec *__pyx_v_write_vel;
-  rvec *__pyx_v_write_forces;
+  void *__pyx_v_write_vel;
+  void *__pyx_v_write_forces;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_box;
   __Pyx_Buffer __pyx_pybuffer_box;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_forces;
   __Pyx_Buffer __pyx_pybuffer_forces;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lambd;
   __Pyx_Buffer __pyx_pybuffer_lambd;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_step;
@@ -11188,15 +11207,15 @@
  * 
  *         # all same length
  *         assert n_frames == len(box) == len(step) == len(time) == len(lambd)             # <<<<<<<<<<<<<<
  * 
  *         if vel is not None:
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_box)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 666, __pyx_L1_error)
     __pyx_t_2 = (__pyx_v_n_frames == __pyx_t_1);
     if (__pyx_t_2) {
       __pyx_t_3 = PyObject_Length(((PyObject *)__pyx_v_step)); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 666, __pyx_L1_error)
       __pyx_t_2 = (__pyx_t_1 == __pyx_t_3);
       if (__pyx_t_2) {
         __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_time)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 666, __pyx_L1_error)
@@ -11229,15 +11248,15 @@
  * 
  *         if vel is not None:
  *             assert n_frames == len(vel)             # <<<<<<<<<<<<<<
  *         if forces is not None:
  *             assert n_frames == len(forces)
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_vel)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 669, __pyx_L1_error)
       if (unlikely(!((__pyx_v_n_frames == __pyx_t_1) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(0, 669, __pyx_L1_error)
       }
     }
     #endif
@@ -11266,15 +11285,15 @@
  *             assert n_frames == len(vel)
  *         if forces is not None:
  *             assert n_frames == len(forces)             # <<<<<<<<<<<<<<
  * 
  *         for i in range(n_frames):
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_forces)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 671, __pyx_L1_error)
       if (unlikely(!((__pyx_v_n_frames == __pyx_t_1) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(0, 671, __pyx_L1_error)
       }
     }
     #endif
@@ -13732,15 +13751,15 @@
   __Pyx_AddTraceback("mdtraj.formats.trr.TRRTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13749,29 +13768,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13782,15 +13801,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13799,29 +13818,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13832,15 +13851,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13849,29 +13868,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13882,15 +13901,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13899,29 +13918,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13932,15 +13951,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13949,29 +13968,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13982,89 +14001,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -14072,33 +14091,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -14106,96 +14125,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14211,15 +14230,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -14227,53 +14246,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -14281,30 +14300,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14319,15 +14338,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14343,15 +14362,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14359,53 +14378,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -14413,30 +14432,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14451,15 +14470,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14475,15 +14494,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14491,53 +14510,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -14545,30 +14564,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14583,176 +14602,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14779,15 +14798,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_3trr_TRRTrajectoryFile(PyObject *o) {
   struct __pyx_obj_6mdtraj_7formats_3trr_TRRTrajectoryFile *p = (struct __pyx_obj_6mdtraj_7formats_3trr_TRRTrajectoryFile *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16008,26 +16027,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -16082,14 +16101,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   __pyx_umethod_PyDict_Type_pop.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1_5 = PyFloat_FromDouble(1.5); if (unlikely(!__pyx_float_1_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_neg_1eneg_10 = PyFloat_FromDouble(-1e-10); if (unlikely(!__pyx_float_neg_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -16221,39 +16245,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -16801,15 +16825,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_trr_line_80, __pyx_kp_u_load_trr_filename_top_None_strid) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19895,18 +19919,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -19952,22 +19976,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/trr.pyx` & `mdtraj-1.9.9/mdtraj/formats/xtc/trr.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/trrlib.pxd` & `mdtraj-1.9.9/mdtraj/formats/xtc/trrlib.pxd`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/xdrlib.pxd` & `mdtraj-1.9.9/mdtraj/formats/xtc/xdrlib.pxd`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/xtc.c` & `mdtraj-1.9.9/mdtraj/formats/xtc/xtc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/formats/xtc/include/",
             "mdtraj/formats/xtc/",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "mdtraj.formats.xtc",
         "sources": [
             "mdtraj/formats/xtc/xtc.pyx",
             "mdtraj/formats/xtc/src/xdrfile.c",
             "mdtraj/formats/xtc/src/xdr_seek.c",
             "mdtraj/formats/xtc/src/xdrfile_xtc.c"
@@ -37,16 +37,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -113,15 +113,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -397,17 +397,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -477,14 +474,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1060,177 +1062,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1278,42 +1280,42 @@
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6mdtraj_7formats_3xtc_XTCTrajectoryFile;
 struct __pyx_obj_6mdtraj_7formats_3xtc___pyx_scope_struct___calc_len_and_offsets;
 struct __pyx_obj_6mdtraj_7formats_3xtc___pyx_scope_struct_1_genexpr;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1884,14 +1886,31 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* ModInt[__pyx_t_6mdtraj_7formats_3xtc_int64_t].proto */
 static CYTHON_INLINE __pyx_t_6mdtraj_7formats_3xtc_int64_t __Pyx_mod___pyx_t_6mdtraj_7formats_3xtc_int64_t(__pyx_t_6mdtraj_7formats_3xtc_int64_t, __pyx_t_6mdtraj_7formats_3xtc_int64_t);
 
 /* DivInt[__pyx_t_6mdtraj_7formats_3xtc_int64_t].proto */
 static CYTHON_INLINE __pyx_t_6mdtraj_7formats_3xtc_int64_t __Pyx_div___pyx_t_6mdtraj_7formats_3xtc_int64_t(__pyx_t_6mdtraj_7formats_3xtc_int64_t, __pyx_t_6mdtraj_7formats_3xtc_int64_t);
 
 /* UnaryNegOverflows.proto */
@@ -1945,30 +1964,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -9637,15 +9656,15 @@
  * 
  *         # all same shape
  *         assert n_frames == len(box) == len(step) == len(time) == len(prec)             # <<<<<<<<<<<<<<
  *         for i in range(n_frames):
  *             status = xdrlib.write_xtc(self.fh, n_atoms, step[i], time[i], <xdrlib.matrix>&box[i, 0, 0], <xdrlib.rvec*>&xyz[i, 0, 0], prec[i])
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_box)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 594, __pyx_L1_error)
     __pyx_t_2 = (__pyx_v_n_frames == __pyx_t_1);
     if (__pyx_t_2) {
       __pyx_t_3 = PyObject_Length(((PyObject *)__pyx_v_step)); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 594, __pyx_L1_error)
       __pyx_t_2 = (__pyx_t_1 == __pyx_t_3);
       if (__pyx_t_2) {
         __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_time)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 594, __pyx_L1_error)
@@ -10585,15 +10604,15 @@
  *             filesize = os.stat(self.filename).st_size
  *             byte_offset = XTC_SHORT_HEADER_SIZE + XTC_SHORT_BYTES_PER_ATOM*self.n_atoms
  *             assert filesize % byte_offset == 0, ("filesize(%i) not divideable"             # <<<<<<<<<<<<<<
  *                                                  " by bytes per frames(%i)"
  *                                                  % (filesize, byte_offset))
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(__pyx_cur_scope->__pyx_v_byte_offset == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
         __PYX_ERR(0, 652, __pyx_L1_error)
       }
       if (unlikely(!((__Pyx_mod___pyx_t_6mdtraj_7formats_3xtc_int64_t(__pyx_v_filesize, __pyx_cur_scope->__pyx_v_byte_offset) == 0) != 0))) {
 
         /* "mdtraj/formats/xtc/xtc.pyx":654
@@ -10789,15 +10808,15 @@
  *         else:
  *             offsets = np.empty(self.approx_n_frames, dtype=np.int64)
  *             assert len(offsets) >= 1             # <<<<<<<<<<<<<<
  * 
  *             try:
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       __pyx_t_13 = PyObject_Length(((PyObject *)__pyx_v_offsets)); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 660, __pyx_L1_error)
       if (unlikely(!((__pyx_t_13 >= 1) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(0, 660, __pyx_L1_error)
       }
     }
     #endif
@@ -12321,15 +12340,15 @@
   __Pyx_AddTraceback("mdtraj.formats.xtc.XTCTrajectoryFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12338,29 +12357,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12371,15 +12390,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12388,29 +12407,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -12421,15 +12440,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12438,29 +12457,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -12471,15 +12490,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12488,29 +12507,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -12521,15 +12540,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12538,29 +12557,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -12571,89 +12590,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -12661,33 +12680,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -12695,96 +12714,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12800,15 +12819,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -12816,53 +12835,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -12870,30 +12889,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12908,15 +12927,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12932,15 +12951,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -12948,53 +12967,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -13002,30 +13021,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13040,15 +13059,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13064,15 +13083,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13080,53 +13099,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -13134,30 +13153,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13172,176 +13191,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -13368,15 +13387,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6mdtraj_7formats_3xtc_XTCTrajectoryFile(PyObject *o) {
   struct __pyx_obj_6mdtraj_7formats_3xtc_XTCTrajectoryFile *p = (struct __pyx_obj_6mdtraj_7formats_3xtc_XTCTrajectoryFile *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -14244,26 +14263,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -14318,14 +14337,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   __pyx_umethod_PyDict_Type_pop.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1_5 = PyFloat_FromDouble(1.5); if (unlikely(!__pyx_float_1_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1000_0 = PyFloat_FromDouble(1000.0); if (unlikely(!__pyx_float_1000_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_4_74462831e_00 = PyFloat_FromDouble(4.74462831e+00); if (unlikely(!__pyx_float_4_74462831e_00)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_9_93733050e_01 = PyFloat_FromDouble(9.93733050e+01); if (unlikely(!__pyx_float_9_93733050e_01)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -14437,39 +14461,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15062,15 +15086,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_load_xtc_line_112, __pyx_kp_u_load_xtc_filename_top_None_strid) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18170,18 +18194,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -18227,22 +18251,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/formats/xtc/xtc.pyx` & `mdtraj-1.9.9/mdtraj/formats/xtc/xtc.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/formats/xyzfile.py` & `mdtraj-1.9.9/mdtraj/formats/xyzfile.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/__init__.py` & `mdtraj-1.9.9/mdtraj/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/alignment.py` & `mdtraj-1.9.9/mdtraj/geometry/alignment.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/angle.py` & `mdtraj-1.9.9/mdtraj/geometry/angle.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/contact.py` & `mdtraj-1.9.9/mdtraj/geometry/contact.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/dihedral.py` & `mdtraj-1.9.9/mdtraj/geometry/dihedral.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/distance.py` & `mdtraj-1.9.9/mdtraj/geometry/distance.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/drid.cpp` & `mdtraj-1.9.9/mdtraj/geometry/drid.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "mdtraj/geometry/include/dridkernels.h"
         ],
@@ -14,15 +14,15 @@
             "--std=c++11",
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/geometry/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj.geometry.drid",
         "sources": [
             "mdtraj/geometry/drid.pyx",
             "mdtraj/geometry/src/dridkernels.cpp",
             "mdtraj/geometry/src/moments.cpp"
@@ -37,16 +37,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -113,15 +113,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -411,17 +411,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -491,14 +488,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1628,14 +1630,31 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* IncludeStringH.proto */
@@ -3918,15 +3937,15 @@
  *     n_atom_indices = len(atom_indices)
  *     result = np.zeros((n_frames, n_atom_indices, 3))
  *     assert n_dims == 3             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n_frames):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_n_dims == 3) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 124, __pyx_L1_error)
     }
   }
   #endif
 
@@ -11492,15 +11511,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -17454,15 +17473,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -17639,15 +17658,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -17770,15 +17789,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18023,15 +18042,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18659,14 +18678,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   /* InitThreads.init */
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `mdtraj-1.9.8/mdtraj/geometry/drid.pyx` & `mdtraj-1.9.9/mdtraj/geometry/drid.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/dssp.py` & `mdtraj-1.9.9/mdtraj/geometry/dssp.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/hbond.py` & `mdtraj-1.9.9/mdtraj/geometry/hbond.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/geometry.h` & `mdtraj-1.9.9/mdtraj/geometry/include/geometry.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/math_patch.h` & `mdtraj-1.9.9/mdtraj/geometry/include/math_patch.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/moments.h` & `mdtraj-1.9.9/mdtraj/geometry/include/moments.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/msvccompat.h` & `mdtraj-1.9.9/mdtraj/geometry/include/msvccompat.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/vectorize.h` & `mdtraj-1.9.9/mdtraj/geometry/include/vectorize.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/vectorize_generic.h` & `mdtraj-1.9.9/mdtraj/geometry/include/vectorize_generic.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/vectorize_neon.h` & `mdtraj-1.9.9/mdtraj/geometry/include/vectorize_neon.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/include/vectorize_sse.h` & `mdtraj-1.9.9/mdtraj/geometry/include/vectorize_sse.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/internal.py` & `mdtraj-1.9.9/mdtraj/geometry/internal.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/neighborlist.cpp` & `mdtraj-1.9.9/mdtraj/geometry/neighborlist.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "mdtraj/geometry/include/neighborlist.h"
         ],
@@ -14,15 +14,15 @@
             "--std=c++11",
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/geometry/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj.geometry.neighborlist",
         "sources": [
             "mdtraj/geometry/neighborlist.pyx",
             "mdtraj/geometry/src/neighborlist.cpp"
         ]
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -112,15 +112,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -410,17 +410,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -490,14 +487,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1712,14 +1714,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -10197,15 +10216,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -15951,15 +15970,15 @@
  * 
  *     if type.typegroup == 'S':
  *         assert type.fields != NULL             # <<<<<<<<<<<<<<
  *         assert type.fields.type != NULL
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_type->fields != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(1, 1471, __pyx_L1_error)
       }
     }
     #endif
 
@@ -15967,15 +15986,15 @@
  *     if type.typegroup == 'S':
  *         assert type.fields != NULL
  *         assert type.fields.type != NULL             # <<<<<<<<<<<<<<
  * 
  *         if type.flags & __PYX_BUF_FLAGS_PACKED_STRUCT:
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_type->fields->type != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(1, 1472, __pyx_L1_error)
       }
     }
     #endif
 
@@ -16279,15 +16298,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -16464,15 +16483,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -16595,15 +16614,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16848,15 +16867,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -17463,14 +17482,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `mdtraj-1.9.8/mdtraj/geometry/neighborlist.pyx` & `mdtraj-1.9.9/mdtraj/geometry/neighborlist.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/neighbors.cpp` & `mdtraj-1.9.9/mdtraj/geometry/neighbors.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "mdtraj/geometry/include/neighbors.hpp"
         ],
@@ -14,15 +14,15 @@
             "--std=c++11",
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/geometry/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj.geometry.neighbors",
         "sources": [
             "mdtraj/geometry/neighbors.pyx",
             "mdtraj/geometry/src/neighbors.cpp"
         ]
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -112,15 +112,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -410,17 +410,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -490,14 +487,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1715,14 +1717,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
@@ -10759,15 +10778,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -16513,15 +16532,15 @@
  * 
  *     if type.typegroup == 'S':
  *         assert type.fields != NULL             # <<<<<<<<<<<<<<
  *         assert type.fields.type != NULL
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_type->fields != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(1, 1471, __pyx_L1_error)
       }
     }
     #endif
 
@@ -16529,15 +16548,15 @@
  *     if type.typegroup == 'S':
  *         assert type.fields != NULL
  *         assert type.fields.type != NULL             # <<<<<<<<<<<<<<
  * 
  *         if type.flags & __PYX_BUF_FLAGS_PACKED_STRUCT:
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_type->fields->type != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(1, 1472, __pyx_L1_error)
       }
     }
     #endif
 
@@ -16841,15 +16860,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -17026,15 +17045,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -17157,15 +17176,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -17410,15 +17429,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18061,14 +18080,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `mdtraj-1.9.8/mdtraj/geometry/neighbors.pyx` & `mdtraj-1.9.9/mdtraj/geometry/neighbors.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/order.py` & `mdtraj-1.9.9/mdtraj/geometry/order.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/rdf.py` & `mdtraj-1.9.9/mdtraj/geometry/rdf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/rg.py` & `mdtraj-1.9.9/mdtraj/geometry/rg.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/sasa.py` & `mdtraj-1.9.9/mdtraj/geometry/sasa.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/shape.py` & `mdtraj-1.9.9/mdtraj/geometry/shape.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/_geometry.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/_geometry.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "mdtraj/geometry/include/geometry.h",
             "mdtraj/geometry/include/math_patch.h",
             "mdtraj/geometry/include/sasa.h",
             "mdtraj/geometry/src/kernels/anglekernels.h",
             "mdtraj/geometry/src/kernels/dihedralkernels.h",
             "mdtraj/geometry/src/kernels/distancekernels.h"
         ],
@@ -25,15 +25,15 @@
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/geometry/include",
             "mdtraj/geometry/src/kernels",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj.geometry._geometry",
         "sources": [
             "mdtraj/geometry/src/_geometry.pyx",
             "mdtraj/geometry/src/sasa.cpp",
             "mdtraj/geometry/src/dssp.cpp",
@@ -49,16 +49,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -125,15 +125,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -423,17 +423,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -503,14 +500,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1163,177 +1165,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1364,42 +1366,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2006,14 +2008,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
@@ -2039,30 +2058,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -8075,15 +8094,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8092,29 +8111,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8125,15 +8144,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8142,29 +8161,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8175,15 +8194,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8192,29 +8211,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8225,15 +8244,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8242,29 +8261,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8275,15 +8294,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8292,29 +8311,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8325,89 +8344,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8415,33 +8434,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -8449,96 +8468,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8554,15 +8573,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8570,53 +8589,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
@@ -8624,30 +8643,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8662,15 +8681,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8686,15 +8705,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8702,53 +8721,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
@@ -8756,30 +8775,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8794,15 +8813,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8818,15 +8837,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8834,53 +8853,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
@@ -8888,30 +8907,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8926,176 +8945,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16564,15 +16583,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(3, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -22291,15 +22310,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -22476,15 +22495,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -22607,15 +22626,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -22860,15 +22879,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23289,26 +23308,26 @@
  *         for atom in anchor_molecules[next_anchor]:
  *             frame_positions[atom] -= offset
  */
   __pyx_tuple__6 = PyTuple_Pack(2, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 947, __pyx_L1_error)
@@ -23759,14 +23778,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -23885,39 +23909,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -26595,18 +26619,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -26652,22 +26676,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/_geometry.pyx` & `mdtraj-1.9.9/mdtraj/geometry/src/_geometry.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/dridkernels.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/dridkernels.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/dssp.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/dssp.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/geometry.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/geometry.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/image_molecules.pxi` & `mdtraj-1.9.9/mdtraj/geometry/src/image_molecules.pxi`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/kernels/anglekernels.h` & `mdtraj-1.9.9/mdtraj/geometry/src/kernels/anglekernels.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/kernels/dihedralkernels.h` & `mdtraj-1.9.9/mdtraj/geometry/src/kernels/dihedralkernels.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/kernels/distancekernels.h` & `mdtraj-1.9.9/mdtraj/geometry/src/kernels/distancekernels.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/moments.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/moments.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/neighborlist.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/neighborlist.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/neighbors.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/neighbors.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/src/sasa.cpp` & `mdtraj-1.9.9/mdtraj/geometry/src/sasa.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/geometry/thermodynamic_properties.py` & `mdtraj-1.9.9/mdtraj/geometry/thermodynamic_properties.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/io.py` & `mdtraj-1.9.9/mdtraj/io.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/nmr/scalar_couplings.py` & `mdtraj-1.9.9/mdtraj/nmr/scalar_couplings.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/nmr/shift_wrappers.py` & `mdtraj-1.9.9/mdtraj/nmr/shift_wrappers.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/reporters/basereporter.py` & `mdtraj-1.9.9/mdtraj/reporters/basereporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/reporters/dcdreporter.py` & `mdtraj-1.9.9/mdtraj/reporters/dcdreporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/reporters/hdf5reporter.py` & `mdtraj-1.9.9/mdtraj/reporters/hdf5reporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/reporters/netcdfreporter.py` & `mdtraj-1.9.9/mdtraj/reporters/netcdfreporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/reporters/xtcreporter.py` & `mdtraj-1.9.9/mdtraj/reporters/xtcreporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/_lprmsd.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/_lprmsd.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "mdtraj/rmsd/include/Munkres.h",
             "mdtraj/rmsd/include/euclidean_permutation.hpp",
             "mdtraj/rmsd/include/fancy_index.hpp"
         ],
         "extra_compile_args": [
             "-msse2",
             "-mssse3",
@@ -22,15 +22,15 @@
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/rmsd",
             "mdtraj/rmsd/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj._lprmsd",
         "sources": [
             "mdtraj/rmsd/_lprmsd.pyx",
             "mdtraj/rmsd/src/theobald_rmsd.cpp",
             "mdtraj/rmsd/src/rotation.cpp",
@@ -49,16 +49,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -125,15 +125,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -423,17 +423,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -503,14 +500,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1094,177 +1096,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1291,42 +1293,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1632,14 +1634,31 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* PyObjectFormatAndDecref.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f);
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f);
 
@@ -1709,30 +1728,30 @@
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -5031,15 +5050,15 @@
  * 
  * def _validate_shapes(target, reference, frame):
  *     assert (target.xyz.ndim == 3) and (reference.xyz.ndim == 3) and \             # <<<<<<<<<<<<<<
  *            (target.xyz.shape[2]) == 3 and (reference.xyz.shape[2] == 3)
  *     if not (target.xyz.shape[1]  == reference.xyz.shape[1]):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_target, __pyx_n_s_xyz); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_t_3, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
@@ -6186,15 +6205,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_rslt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6203,29 +6222,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6236,15 +6255,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6253,29 +6272,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6286,15 +6305,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6303,29 +6322,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6336,15 +6355,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6353,29 +6372,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6386,15 +6405,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6403,29 +6422,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6436,89 +6455,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -6526,33 +6545,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":925
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -6560,96 +6579,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":931
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6665,15 +6684,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6681,53 +6700,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":940
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
@@ -6735,30 +6754,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":938
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":937
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6773,15 +6792,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6797,15 +6816,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6813,53 +6832,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":946
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -6867,30 +6886,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":944
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":943
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6905,15 +6924,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6929,15 +6948,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6945,53 +6964,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":952
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -6999,30 +7018,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":950
+    /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":949
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7037,176 +7056,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":975
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":963
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":990
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1000
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1007
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+/* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1014
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7678,26 +7697,26 @@
  * 
  *     return permute_groups
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_permute_groups_must_be_mutually); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 947, __pyx_L1_error)
@@ -7767,14 +7786,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   /* InitThreads.init */
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
@@ -7833,47 +7857,47 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8155,15 +8179,15 @@
  * from cython.parallel cimport prange
  * np.import_array()
  * assert sizeof(np.int32_t) == sizeof(int)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!(((sizeof(__pyx_t_5numpy_int32_t)) == (sizeof(int))) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 38, __pyx_L1_error)
     }
   }
   #endif
 
@@ -10154,18 +10178,18 @@
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -10211,22 +10235,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/_lprmsd.pyx` & `mdtraj-1.9.9/mdtraj/rmsd/_lprmsd.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/_rmsd.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/_rmsd.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "mdtraj/rmsd/include/center.h"
         ],
@@ -14,15 +14,15 @@
             "--std=c++11",
             "-Wno-unused-function",
             "-Wno-unreachable-code",
             "-Wno-sign-compare"
         ],
         "include_dirs": [
             "mdtraj/rmsd/include",
-            "/Users/mattthompson/mambaforge/envs/mdtraj-dev/lib/python3.11/site-packages/numpy/core/include"
+            "/Users/mattthompson/mambaforge/envs/ib-dev/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "mdtraj._rmsd",
         "sources": [
             "mdtraj/rmsd/_rmsd.pyx",
             "mdtraj/rmsd/src/theobald_rmsd.cpp",
             "mdtraj/rmsd/src/rotation.cpp",
@@ -38,16 +38,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -114,15 +114,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -412,17 +412,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -492,14 +489,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1521,14 +1523,31 @@
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
 
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* PyObjectFormatAndDecref.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f);
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f);
 
@@ -1784,30 +1803,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3247,15 +3266,15 @@
  * 
  *     # Error checks
  *     assert (target.xyz.ndim == 3) and (reference.xyz.ndim == 3) and (target.xyz.shape[2]) == 3 and (reference.xyz.shape[2] == 3)             # <<<<<<<<<<<<<<
  *     if not ((target.xyz.shape[1]  == reference.xyz.shape[1]) or
  *             (len(ref_atom_indices) == len(atom_indices))):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_target, __pyx_n_s_xyz); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ndim); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_7, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -5065,15 +5084,15 @@
  * 
  *     # Error checks
  *     assert (target.xyz.ndim == 3) and (reference.xyz.ndim == 3) and (target.xyz.shape[2]) == 3 and (reference.xyz.shape[2] == 3)             # <<<<<<<<<<<<<<
  *     if not ((target.xyz.shape[1]  == reference.xyz.shape[1]) or
  *             (len(ref_atom_indices) == len(atom_indices))):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_target, __pyx_n_s_xyz); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_ndim); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_t_4, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
@@ -7153,15 +7172,15 @@
  * 
  * def _center_inplace_atom_major(float[:, :, ::1] xyz not None):
  *     assert xyz.shape[2] == 3             # <<<<<<<<<<<<<<
  *     cdef float[:] traces = np.empty(xyz.shape[0], dtype=np.float32)
  *     inplace_center_and_trace_atom_major(&xyz[0,0,0], &traces[0], xyz.shape[0], xyz.shape[1])
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!(((__pyx_v_xyz.shape[2]) == 3) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 403, __pyx_L1_error)
     }
   }
   #endif
 
@@ -7506,15 +7525,15 @@
  *     cdef float msd
  * 
  *     assert xyz1.ndim == 3 and xyz2.ndim == 3 and xyz1.shape[1] == 3 and xyz2.shape[1] == 3             # <<<<<<<<<<<<<<
  *     if not (xyz1.shape[2]  == xyz2.shape[2]):
  *         raise ValueError("Input arrays must have same number of atoms. "
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_xyz1, 3, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_t_3, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
@@ -8206,15 +8225,15 @@
  *     cdef float msd
  * 
  *     assert xyz1.ndim == 3 and xyz2.ndim == 3 and xyz1.shape[2] == 3 and xyz2.shape[2] == 3             # <<<<<<<<<<<<<<
  *     if not (xyz1.shape[1]  == xyz2.shape[1]):
  *         raise ValueError("Input arrays must have same number of atoms. "
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_xyz1, 3, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_t_3, __pyx_int_3, 3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
@@ -9586,15 +9605,15 @@
  *         The rotation matrix for each of the alignments
  *     """
  *     assert (xyz_align1.shape[2] == 3) and (xyz_align2.shape[2] == 3)             # <<<<<<<<<<<<<<
  *     assert (xyz_displ1.shape[2] == 3) and (xyz_displ2.shape[2] == 3)
  *     if not ((xyz_align1.shape[1] % 4 == 0) & (xyz_align2.shape[1] % 4 == 0)):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = (((__pyx_v_xyz_align1.shape[2]) == 3) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L3_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_xyz_align2.shape[2]) == 3) != 0);
@@ -9611,15 +9630,15 @@
  *     """
  *     assert (xyz_align1.shape[2] == 3) and (xyz_align2.shape[2] == 3)
  *     assert (xyz_displ1.shape[2] == 3) and (xyz_displ2.shape[2] == 3)             # <<<<<<<<<<<<<<
  *     if not ((xyz_align1.shape[1] % 4 == 0) & (xyz_align2.shape[1] % 4 == 0)):
  *         raise ValueError("Input arrays must have middle dimension of 4*n, "
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = (((__pyx_v_xyz_displ1.shape[2]) == 3) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_xyz_displ2.shape[2]) == 3) != 0);
@@ -17682,15 +17701,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -23409,15 +23428,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -23594,15 +23613,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -23725,15 +23744,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23978,15 +23997,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -24792,14 +24811,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   /* InitThreads.init */
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
@@ -24924,29 +24948,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -27818,18 +27842,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -27875,22 +27899,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/_rmsd.pyx` & `mdtraj-1.9.9/mdtraj/rmsd/_rmsd.pyx`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/Munkres.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/Munkres.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/msvccompat.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/msvccompat.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/sse_swizzle.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/sse_swizzle.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/theobald_rmsd.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/theobald_rmsd.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/util_arm.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/util_arm.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/include/util_sse.h` & `mdtraj-1.9.9/mdtraj/rmsd/include/util_sse.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/Munkres.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/src/Munkres.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/center_arm.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/center_arm.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/center_generic.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/center_generic.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/center_sse.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/center_sse.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/euclidean_permutation.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/src/euclidean_permutation.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/fancy_index.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/src/fancy_index.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/rotation.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/src/rotation.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/rotation_arm.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/rotation_arm.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/rotation_generic.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/rotation_generic.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/rotation_sse.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/rotation_sse.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd.cpp` & `mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd.cpp`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_arm.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_arm.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_generic.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_generic.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/rmsd/src/theobald_rmsd_sse.h` & `mdtraj-1.9.9/mdtraj/rmsd/src/theobald_rmsd_sse.h`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/scripts/mdconvert.py` & `mdtraj-1.9.9/mdtraj/scripts/mdconvert.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/scripts/mdinspect.py` & `mdtraj-1.9.9/mdtraj/scripts/mdinspect.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/testing/__init__.py` & `mdtraj-1.9.9/mdtraj/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/testing/docscrape.py` & `mdtraj-1.9.9/mdtraj/testing/docscrape.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/testing/docstrings.py` & `mdtraj-1.9.9/mdtraj/testing/docstrings.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/testing/testing.py` & `mdtraj-1.9.9/mdtraj/testing/testing.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/__init__.py` & `mdtraj-1.9.9/mdtraj/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/contextmanagers.py` & `mdtraj-1.9.9/mdtraj/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/delay_import.py` & `mdtraj-1.9.9/mdtraj/utils/delay_import.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/rotation.py` & `mdtraj-1.9.9/mdtraj/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/six.py` & `mdtraj-1.9.9/mdtraj/utils/six.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/__init__.py` & `mdtraj-1.9.9/mdtraj/utils/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/basedimension.py` & `mdtraj-1.9.9/mdtraj/utils/unit/basedimension.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/baseunit.py` & `mdtraj-1.9.9/mdtraj/utils/unit/baseunit.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/constants.py` & `mdtraj-1.9.9/mdtraj/utils/unit/constants.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/doctests.py` & `mdtraj-1.9.9/mdtraj/utils/unit/doctests.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/mymatrix.py` & `mdtraj-1.9.9/mdtraj/utils/unit/mymatrix.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/prefix.py` & `mdtraj-1.9.9/mdtraj/utils/unit/prefix.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/quantity.py` & `mdtraj-1.9.9/mdtraj/utils/unit/quantity.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/standard_dimensions.py` & `mdtraj-1.9.9/mdtraj/utils/unit/standard_dimensions.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/unit.py` & `mdtraj-1.9.9/mdtraj/utils/unit/unit.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/unit_definitions.py` & `mdtraj-1.9.9/mdtraj/utils/unit/unit_definitions.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/unit_math.py` & `mdtraj-1.9.9/mdtraj/utils/unit/unit_math.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unit/unit_operators.py` & `mdtraj-1.9.9/mdtraj/utils/unit/unit_operators.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/unitcell.py` & `mdtraj-1.9.9/mdtraj/utils/unitcell.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/validation.py` & `mdtraj-1.9.9/mdtraj/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj/utils/zipped.py` & `mdtraj-1.9.9/mdtraj/utils/zipped.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/mdtraj.egg-info/PKG-INFO` & `mdtraj-1.9.9/mdtraj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdtraj
-Version: 1.9.8
+Version: 1.9.9
 Summary: MDTraj: A modern, open library for the analysis of molecular dynamics trajectories
 Home-page: http://mdtraj.org
 Download-URL: https://github.com/rmcgibbo/mdtraj/releases/latest
 Author: Robert McGibbon
 Author-email: rmcgibbo@gmail.com
 License: LGPLv2.1+
 Platform: Linux
```

### Comparing `mdtraj-1.9.8/mdtraj.egg-info/SOURCES.txt` & `mdtraj-1.9.9/mdtraj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/setup.py` & `mdtraj-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     sys.argv.remove('--disable-openmp')
     disable_openmp = True
 except ValueError:
     disable_openmp = False
 
 
 ##########################
-VERSION = "1.9.8"
+VERSION = "1.9.9"
 ISRELEASED = True
 __version__ = VERSION
 ##########################
 
 
 CLASSIFIERS = """\
 Development Status :: 5 - Production/Stable
```

### Comparing `mdtraj-1.9.8/tests/test_alignment.py` & `mdtraj-1.9.9/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_angles.py` & `mdtraj-1.9.9/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_arc.py` & `mdtraj-1.9.9/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_binpos.py` & `mdtraj-1.9.9/tests/test_binpos.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_contact.py` & `mdtraj-1.9.9/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_crd.py` & `mdtraj-1.9.9/tests/test_crd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_dcd.py` & `mdtraj-1.9.9/tests/test_dcd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_dihedral.py` & `mdtraj-1.9.9/tests/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_distance.py` & `mdtraj-1.9.9/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_docstrings.py` & `mdtraj-1.9.9/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_drid.py` & `mdtraj-1.9.9/tests/test_drid.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_dssp.py` & `mdtraj-1.9.9/tests/test_dssp.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_dtr.py` & `mdtraj-1.9.9/tests/test_dtr.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_element.py` & `mdtraj-1.9.9/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_geometry.py` & `mdtraj-1.9.9/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_gro.py` & `mdtraj-1.9.9/tests/test_gro.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_gsd.py` & `mdtraj-1.9.9/tests/test_gsd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_hbonds.py` & `mdtraj-1.9.9/tests/test_hbonds.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_hdf5.py` & `mdtraj-1.9.9/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_hoomdxml.py` & `mdtraj-1.9.9/tests/test_hoomdxml.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_io.py` & `mdtraj-1.9.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_lammpstrj.py` & `mdtraj-1.9.9/tests/test_lammpstrj.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_lh5.py` & `mdtraj-1.9.9/tests/test_lh5.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_load.py` & `mdtraj-1.9.9/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_lprmsd.py` & `mdtraj-1.9.9/tests/test_lprmsd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_mdconvert.py` & `mdtraj-1.9.9/tests/test_mdconvert.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_mdcrd.py` & `mdtraj-1.9.9/tests/test_mdcrd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_mol2.py` & `mdtraj-1.9.9/tests/test_mol2.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_neighborlist.py` & `mdtraj-1.9.9/tests/test_neighborlist.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_neighbors.py` & `mdtraj-1.9.9/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_netcdf.py` & `mdtraj-1.9.9/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_nmr.py` & `mdtraj-1.9.9/tests/test_nmr.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_order.py` & `mdtraj-1.9.9/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_pdb.py` & `mdtraj-1.9.9/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_pdbx.py` & `mdtraj-1.9.9/tests/test_pdbx.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_prmtop.py` & `mdtraj-1.9.9/tests/test_prmtop.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_psf.py` & `mdtraj-1.9.9/tests/test_psf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_quaternion.py` & `mdtraj-1.9.9/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_rdf.py` & `mdtraj-1.9.9/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_reporter.py` & `mdtraj-1.9.9/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_restart.py` & `mdtraj-1.9.9/tests/test_restart.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_rmsd.py` & `mdtraj-1.9.9/tests/test_rmsd.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_rmsd_memmap.py` & `mdtraj-1.9.9/tests/test_rmsd_memmap.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_sasa.py` & `mdtraj-1.9.9/tests/test_sasa.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_selection.py` & `mdtraj-1.9.9/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_shape.py` & `mdtraj-1.9.9/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_thermodynamic_properties.py` & `mdtraj-1.9.9/tests/test_thermodynamic_properties.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_tng.py` & `mdtraj-1.9.9/tests/test_tng.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_topology.py` & `mdtraj-1.9.9/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_trajectory.py` & `mdtraj-1.9.9/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_trr.py` & `mdtraj-1.9.9/tests/test_trr.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_utils.py` & `mdtraj-1.9.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_xml.py` & `mdtraj-1.9.9/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_xtc.py` & `mdtraj-1.9.9/tests/test_xtc.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_xyz.py` & `mdtraj-1.9.9/tests/test_xyz.py`

 * *Files identical despite different names*

### Comparing `mdtraj-1.9.8/tests/test_zipped.py` & `mdtraj-1.9.9/tests/test_zipped.py`

 * *Files identical despite different names*

