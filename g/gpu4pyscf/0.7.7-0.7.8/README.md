# Comparing `tmp/gpu4pyscf-0.7.7.tar.gz` & `tmp/gpu4pyscf-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpu4pyscf-0.7.7.tar", last modified: Wed May 15 06:45:05 2024, max compression
+gzip compressed data, was "gpu4pyscf-0.7.8.tar", last modified: Thu May 30 04:13:06 2024, max compression
```

## Comparing `gpu4pyscf-0.7.7.tar` & `gpu4pyscf-0.7.8.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/cc/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24054 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/cc/ccsd_incore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/df/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/cderi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/df.py
--rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/df_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24763 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30903 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)    67266 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/int3c2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21779 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/gen_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    75748 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/numint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/radi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/fci/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/fci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/fci/direct_spin1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/gto/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/gto/mole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42163 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cublas.py
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cupy_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cusolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cutensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/mp/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/dfmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/mp2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/polarizability.py
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/shielding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/chelpg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/scf/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/_response_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/cphf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    38454 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/int4c2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/ucphf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/uhf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/_attach_solvent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4469 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.462331 gpu4pyscf-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 04:13:06.462331 gpu4pyscf-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.446331 gpu4pyscf-0.7.8/gpu4pyscf/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.450331 gpu4pyscf-0.7.8/gpu4pyscf/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24054 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/cc/ccsd_incore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.450331 gpu4pyscf-0.7.8/gpu4pyscf/df/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/cderi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/df_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.450331 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.450331 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25261 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30769 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67871 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/df/int3c2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.454331 gpu4pyscf-0.7.8/gpu4pyscf/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21865 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/gen_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/libxc_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76439 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/radi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/xc_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/dft/xc_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.454331 gpu4pyscf-0.7.8/gpu4pyscf/fci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/fci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/fci/direct_spin1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.454331 gpu4pyscf-0.7.8/gpu4pyscf/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.454331 gpu4pyscf-0.7.8/gpu4pyscf/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/gto/mole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.454331 gpu4pyscf-0.7.8/gpu4pyscf/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25367 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42481 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/hessian/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/cublas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/cupy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/cusolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/cutensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/dftd4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/mp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/mp/dfmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/mp/mp2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/properties/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/properties/polarizability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/properties/shielding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/qmmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/qmmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/qmmm/chelpg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/scf/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/cphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38290 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/int4c2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/ucphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/scf/uhf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.458331 gpu4pyscf-0.7.8/gpu4pyscf/solvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/_attach_solvent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.462331 gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.462331 gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/smd_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/gpu4pyscf/solvent/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 04:13:06.446331 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 04:13:06.000000 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-30 04:13:06.000000 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 04:13:06.000000 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 04:13:06.000000 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 04:13:06.000000 gpu4pyscf-0.7.8/gpu4pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 04:13:06.462331 gpu4pyscf-0.7.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4469 2024-05-30 04:13:05.000000 gpu4pyscf-0.7.8/setup.py
```

### Comparing `gpu4pyscf-0.7.7/LICENSE` & `gpu4pyscf-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/MANIFEST.in` & `gpu4pyscf-0.7.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/README.md` & `gpu4pyscf-0.7.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,18 @@
 > [!NOTE]
 > The compiled binary packages support compute capability 6.0 and later (Pascal and later, such as Tesla P100, RTX 10 series and later).
 
 Run ```nvidia-smi``` in your terminal to check the installed CUDA version.
 
 Choose the proper package based on your CUDA environment.
 
-| Platform      | Command                               |
-----------------| --------------------------------------|
-| **CUDA 11.x** |  ```pip3 install gpu4pyscf-cuda11x``` |
-| **CUDA 12.x** |  ```pip3 install gpu4pyscf-cuda12x``` |
-
-```cuTensor``` is **highly recommended** for accelerating tensor contractions.
-
-For **CUDA 11.x**, ```pip3 install cutensor-cu11``` (requires CuPy V13.0 and later)
-
-For **CUDA 12.x**, ```pip3 install cutensor-cu12``` (requires CuPy V13.0 and later)
+| Platform      | Command                               | cutensor (**highly recommended**)|
+----------------| --------------------------------------|----------------------------------|
+| **CUDA 11.x** |  ```pip3 install gpu4pyscf-cuda11x``` | ```pip3 install cutensor-cu11``` |
+| **CUDA 12.x** |  ```pip3 install gpu4pyscf-cuda12x``` | ```pip3 install cutensor-cu12``` |
 
 Compilation
 --------
 One can compile the package with
 ```sh
 git clone https://github.com/pyscf/gpu4pyscf.git
 cd gpu4pyscf
@@ -37,28 +31,29 @@
 export PYTHONPATH="${PYTHONPATH}:${CURRENT_PATH}"
 ```
 Then install cutensor for acceleration
 ```sh
 pip3 install cutensor-cu11
 ```
 
-The package also provides multiple dockerfiles in ```dockerfiles```. One can use them as references to create the compilation envrionment. 
+The package also provides multiple dockerfiles in ```dockerfiles```. One can use them as references to create the compilation envrionment.
 
 Features
 --------
 - Density fitting scheme and direct SCF scheme;
 - SCF, analytical Gradient, and analytical Hessian calculations for Hartree-Fock and DFT;
 - LDA, GGA, mGGA, hybrid, and range-separated functionals via [libXC](https://gitlab.com/libxc/libxc/-/tree/master/);
 - Geometry optimization and transition state search via [geomeTRIC](https://geometric.readthedocs.io/en/latest/);
 - Dispersion corrections via [DFTD3](https://github.com/dftd3/simple-dftd3) and [DFTD4](https://github.com/dftd4/dftd4);
 - Nonlocal functional correction (vv10) for SCF and gradient;
 - ECP is supported and calculated on CPU;
 - PCM models, SMD model, their analytical gradients, and semi-analytical Hessian matrix;
-- Unrestricted Hartree-Fock and Unrestricted DFT, gradient, and Hessian
-- MP2/DF-MP2 and CCSD (experimental)
+- Unrestricted Hartree-Fock and Unrestricted DFT, gradient, and Hessian;
+- MP2/DF-MP2 and CCSD (experimental);
+- Polarizability, IR, and NMR shielding
 
 Limitations
 --------
 - Rys roots up to 9 for density fitting scheme and direct scf scheme;
 - Atomic basis up to g orbitals;
 - Auxiliary basis up to i orbitals;
 - Density fitting scheme up to ~168 atoms with def2-tzvpd basis, bounded by CPU memory;
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/__config__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/__config__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/cc/ccsd_incore.py` & `gpu4pyscf-0.7.8/gpu4pyscf/cc/ccsd_incore.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/cderi.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/cderi.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/df.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/df.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 from gpu4pyscf.df import int3c2e, df_jk
 from gpu4pyscf.lib import logger
 from gpu4pyscf import __config__
 from cupyx import scipy
 
 MIN_BLK_SIZE = getattr(__config__, 'min_ao_blksize', 128)
 ALIGNED = getattr(__config__, 'ao_aligned', 32)
-LINEAR_DEP_TOL = incore.LINEAR_DEP_THR
+
+# TODO: reuse the setting in pyscf 2.6
+LINEAR_DEP_THR = 1e-6#incore.LINEAR_DEP_THR
+GROUP_SIZE = 256
 
 class DF(lib.StreamObject):
     from gpu4pyscf.lib.utils import to_gpu, device
 
     _keys = {'intopt', 'mol', 'auxmol'}
 
     def __init__(self, mol, auxbasis=None):
@@ -79,25 +82,25 @@
             with auxmol.with_range_coulomb(omega):
                 j2c_cpu = auxmol.intor('int2c2e', hermi=1)
         else:
             j2c_cpu = auxmol.intor('int2c2e', hermi=1)
         j2c = cupy.asarray(j2c_cpu, order='C')
         t0 = log.timer_debug1('2c2e', *t0)
         intopt = int3c2e.VHFOpt(mol, auxmol, 'int2e')
-        intopt.build(direct_scf_tol, diag_block_with_triu=False, aosym=True, group_size=256)
+        intopt.build(direct_scf_tol, diag_block_with_triu=False, aosym=True, group_size=GROUP_SIZE)
         log.timer_debug1('prepare intopt', *t0)
         self.j2c = j2c.copy()
 
         j2c = take_last2d(j2c, intopt.aux_ao_idx)
         try:
             self.cd_low = cholesky(j2c)
             self.cd_low = tag_array(self.cd_low, tag='cd')
         except Exception:
             w, v = cupy.linalg.eigh(j2c)
-            idx = w > LINEAR_DEP_TOL
+            idx = w > LINEAR_DEP_THR
             self.cd_low = (v[:,idx] / cupy.sqrt(w[idx]))
             self.cd_low = tag_array(self.cd_low, tag='eig')
 
         v = w = None
         naux = self.naux = self.cd_low.shape[1]
         log.debug('size of aux basis %d', naux)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/df_jk.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/df_jk.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
     vj = None
     vk = None
     ao_idx = dfobj.intopt.ao_idx
     dms = take_last2d(dms, ao_idx)
 
     rows = dfobj.intopt.cderi_row
     cols = dfobj.intopt.cderi_col
+    
     if with_j:
         dm_sparse = dms[:,rows,cols]
         dm_sparse[:, dfobj.intopt.cderi_diag] *= .5
         vj = cupy.zeros_like(dms)
 
     if with_k:
         vk = cupy.zeros_like(dms)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/grad/rhf.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,47 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
 import numpy
 import cupy
 from cupyx.scipy.linalg import solve_triangular
 from pyscf import scf
-from gpu4pyscf.df import int3c2e
-from gpu4pyscf.lib.cupy_helper import print_mem_info, tag_array, unpack_tril, contract, load_library, take_last2d
+from gpu4pyscf.df import int3c2e, df
+from gpu4pyscf.lib.cupy_helper import (print_mem_info, tag_array,
+unpack_tril, contract, load_library, take_last2d, cholesky)
 from gpu4pyscf.grad import rhf as rhf_grad
 from gpu4pyscf import __config__
 from gpu4pyscf.lib import logger
 
 libcupy_helper = load_library('libcupy_helper')
 
+LINEAR_DEP_THRESHOLD = df.LINEAR_DEP_THR
 MIN_BLK_SIZE = getattr(__config__, 'min_ao_blksize', 128)
 ALIGNED = getattr(__config__, 'ao_aligned', 64)
 
+def _gen_metric_solver(int2c, decompose_j2c='CD', lindep=LINEAR_DEP_THRESHOLD):
+    ''' generate a solver to solve Ax = b, RHS must be in (n,....) '''
+    if decompose_j2c.upper() == 'CD':
+        try:
+            j2c = cholesky(int2c, lower=True)
+            def j2c_solver(v):
+                return solve_triangular(j2c, v, overwrite_b=False)
+            return j2c_solver
+
+        except Exception:
+            pass
+
+    w, v = cupy.linalg.eigh(int2c)
+    mask = w > lindep
+    v1 = v[:,mask]
+    j2c = cupy.dot(v1/w[mask], v1.conj().T)
+    def j2c_solver(b): # noqa: F811
+        return j2c.dot(b.reshape(j2c.shape[0],-1)).reshape(b.shape)
+    return j2c_solver
+
 def get_jk(mf_grad, mol=None, dm0=None, hermi=0, with_j=True, with_k=True, omega=None):
     if mol is None: mol = mf_grad.mol
     #TODO: dm has to be the SCF density matrix in this version.  dm should be
     # extended to any 1-particle density matrix
 
     if(dm0 is None): dm0 = mf_grad.base.make_rdm1()
     mf = mf_grad.base
@@ -46,15 +68,14 @@
             dfobj = mf_grad.base.with_df
             with_df = dfobj._rsh_df[key] = copy.copy(dfobj).reset()
 
     auxmol = with_df.auxmol
     if not hasattr(with_df, 'intopt') or with_df._cderi is None:
         with_df.build(omega=omega)
     intopt = with_df.intopt
-
     naux = with_df.naux
 
     log = logger.new_logger(mol, mol.verbose)
     t0 = (logger.process_clock(), logger.perf_counter())
 
     if isinstance(mf_grad.base, scf.rohf.ROHF):
         raise NotImplementedError()
@@ -140,15 +161,14 @@
 
     nao_cart = intopt.mol.nao
     block_size = with_df.get_blksize(nao=nao_cart)
     intopt.clear()
     # rebuild with aosym
     intopt.build(mf.direct_scf_tol, diag_block_with_triu=True, aosym=False,
                  group_size_aux=block_size)#, group_size=block_size)
-
     if not intopt._mol.cart:
         # sph2cart for ao
         cart2sph = intopt.cart2sph
         orbo_cart = cart2sph @ orbo
         dm_cart = cart2sph @ dm @ cart2sph.T
     else:
         dm_cart = dm
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/grad/rks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/grad/uhf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/grad/uks.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Args:
         ks_grad : grad.uhf.Gradients or grad.uks.Gradients object
     '''
     if mol is None: mol = ks_grad.mol
     if dm is None: dm = ks_grad.base.make_rdm1()
     t0 = (logger.process_clock(), logger.perf_counter())
-
+    
     mf = ks_grad.base
     ni = mf._numint
     if ks_grad.grids is not None:
         grids = ks_grad.grids
     else:
         grids = mf.grids
 
@@ -127,15 +127,15 @@
 
     if ks_grad.auxbasis_response:
         logger.debug1(ks_grad, 'sum(auxbasis response) %s', e1_aux.sum(axis=0))
     else:
         e1_aux = None
 
     vxc = tag_array(vxc, aux=e1_aux)
-
+    
     return vxc
 
 
 class Gradients(uks_grad.Gradients):
 
     _keys = {'with_df', 'auxbasis_response'}
 
@@ -159,8 +159,8 @@
 
     def extra_force(self, atom_id, envs):
         e1 = uks_grad.Gradients.extra_force(self, atom_id, envs)
         if self.auxbasis_response:
             e1 += envs['dvhf'].aux[atom_id]
         return e1
 
-Grad = Gradients
+Grad = Gradients
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/rhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 [1] Efficient implementation of the analytic second derivatives of
     Hartree-Fock and hybrid DFT energies: a detailed analysis of different
     approximations.  Dmytro Bykov, Taras Petrenko, Robert Izsak, Simone
     Kossmann, Ute Becker, Edward Valeev, Frank Neese. Mol. Phys. 113, 1961 (2015)
 '''
 
 
-
 import numpy
 import cupy
 import numpy as np
-from pyscf import lib, df
-from pyscf.df.grad.rhf import LINEAR_DEP_THRESHOLD
+from pyscf import lib
+from pyscf.df.incore import LINEAR_DEP_THR
 from gpu4pyscf.grad import rhf as rhf_grad
 from gpu4pyscf.hessian import rhf as rhf_hess
 from gpu4pyscf.lib.cupy_helper import (
-    contract, tag_array, release_gpu_stack, print_mem_info, take_last2d, pinv)
-from gpu4pyscf.df import int3c2e
+    contract, tag_array, get_avail_mem, release_gpu_stack, print_mem_info, take_last2d, pinv)
+from gpu4pyscf.df import int3c2e, df
 from gpu4pyscf.lib import logger
+from gpu4pyscf import __config__
+from gpu4pyscf.df.grad.rhf import _gen_metric_solver
 
+LINEAR_DEP_THRESHOLD = df.LINEAR_DEP_THR
 BLKSIZE = 256
+ALIGNED = getattr(__config__, 'ao_aligned', 32)
 
 def partial_hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
                       atmlst=None, max_memory=4000, verbose=None):
     e1, ej, ek = _partial_hess_ejk(hessobj, mo_energy, mo_coeff, mo_occ,
                                    atmlst, max_memory, verbose, True)
     return e1 + ej - ek
 
@@ -97,88 +100,97 @@
     mocc_2 = mocc_2[ao_idx, :]
     dm0 = take_last2d(dm0, ao_idx)
     dm0_tag = tag_array(dm0, occ_coeff=mocc_2)
 
     int2c = cupy.asarray(int2c, order='C')
     int2c = take_last2d(int2c, aux_ao_idx)
     int2c_inv = pinv(int2c, lindep=LINEAR_DEP_THRESHOLD)
+    solve_j2c = _gen_metric_solver(int2c)
     int2c = None
 
     int2c_ip1 = cupy.asarray(int2c_ip1, order='C')
     int2c_ip1 = take_last2d(int2c_ip1, aux_ao_idx)
 
     hj_ao_ao = cupy.zeros([nao,nao,3,3])
     hk_ao_ao = cupy.zeros([nao,nao,3,3])
     if hessobj.auxbasis_response:
         hj_ao_aux = cupy.zeros([nao,naux,3,3])
         hk_ao_aux = cupy.zeros([nao,naux,3,3])
 
     #  int3c contributions
     wj, wk_P__ = int3c2e.get_int3c2e_jk(mol, auxmol, dm0_tag, omega=omega)
-    rhoj0_P = contract('pq,q->p', int2c_inv, wj)
-    rhok0_P__ = contract('pq,qij->pij', int2c_inv, wk_P__)
+    rhoj0_P = solve_j2c(wj)
+    rhok0_P__ = solve_j2c(wk_P__)
     wj = wk_P__ = None
     t1 = log.timer_debug1('intermediate variables with int3c2e', *t1)
 
     # int3c_ip2 contributions
     wj_ip2, wk_ip2_P__ = int3c2e.get_int3c2e_ip2_wjk(intopt, dm0_tag, omega=omega)
     t1 = log.timer_debug1('interdeidate variables with int3c2e_ip2', *t1)
 
     #  int3c_ip1 contributions
     wj1_P, wk1_Pko = int3c2e.get_int3c2e_ip1_wjk(intopt, dm0_tag, omega=omega)
-    rhoj1_P = contract('pq,ipx->iqx', int2c_inv, wj1_P)
+    #rhoj1_P = contract('pq,pix->qix', int2c_inv, wj1_P)
+    rhoj1_P = solve_j2c(wj1_P)
 
-    hj_ao_ao += 4.0*contract('ipx,jpy->ijxy', rhoj1_P, wj1_P)   # (10|0)(0|0)(0|01)
+    hj_ao_ao += 4.0*contract('pix,pjy->ijxy', rhoj1_P, wj1_P)   # (10|0)(0|0)(0|01)
     wj1_P = None
     if hessobj.auxbasis_response:
         wj0_01 = contract('ypq,q->yp', int2c_ip1, rhoj0_P)
-        wj1_01 = contract('yqp,ipx->iqxy', int2c_ip1, rhoj1_P)
-        hj_ao_aux += contract('ipx,py->ipxy', rhoj1_P, wj_ip2)   # (10|0)(1|00)
-        hj_ao_aux -= contract('ipx,yp->ipxy', rhoj1_P, wj0_01)   # (10|0)(1|0)(0|00)
+        wj1_01 = contract('yqp,pix->iqxy', int2c_ip1, rhoj1_P)
+        hj_ao_aux += contract('pix,py->ipxy', rhoj1_P, wj_ip2)   # (10|0)(1|00)
+        hj_ao_aux -= contract('pix,yp->ipxy', rhoj1_P, wj0_01)   # (10|0)(1|0)(0|00)
         hj_ao_aux -= contract('q,iqxy->iqxy', rhoj0_P, wj1_01)   # (10|0)(0|1)(0|00)
         wj1_01 = None
     rhoj1_P = None
 
-    int2c_ip1_inv = contract('yqp,pr->yqr', int2c_ip1, int2c_inv)
     if with_k:
-        for i0, i1 in lib.prange(0,nao,64):
-            wk1_Pko_islice = cupy.asarray(wk1_Pko[i0:i1])
-            rhok1_Pko = contract('pq,iqox->ipox', int2c_inv, wk1_Pko_islice)
-            for k0, k1 in lib.prange(0,nao,64):
-                wk1_Pko_kslice = cupy.asarray(wk1_Pko[k0:k1])
+        mem_avail = get_avail_mem()
+        nocc = mocc.shape[1]
+        slice_size = naux*nocc*9   # largest slice of intermediate variables
+        blksize = int(mem_avail*0.2/8/slice_size/ALIGNED) * ALIGNED
+        for i0, i1 in lib.prange(0,nao,blksize):
+            wk1_Pko_islice = cupy.asarray(wk1_Pko[:,i0:i1])
+            #rhok1_Pko = contract('pq,qiox->piox', int2c_inv, wk1_Pko_islice)
+            rhok1_Pko = solve_j2c(wk1_Pko_islice)
+            wk1_Pko_islice = None
+            for k0, k1 in lib.prange(0,nao,blksize):
+                wk1_Pko_kslice = cupy.asarray(wk1_Pko[:,k0:k1])
 
                 # (10|0)(0|10) without response of RI basis
-                vk2_ip1_ip1 = contract('ipox,kpoy->ikxy', rhok1_Pko, wk1_Pko_kslice)
+                vk2_ip1_ip1 = contract('piox,pkoy->ikxy', rhok1_Pko, wk1_Pko_kslice)
                 hk_ao_ao[i0:i1,k0:k1] += contract('ikxy,ik->ikxy', vk2_ip1_ip1, dm0[i0:i1,k0:k1])
                 vk2_ip1_ip1 = None
 
                 # (10|0)(0|01) without response of RI basis
-                bra = contract('ipox,ko->ipkx', rhok1_Pko, mocc_2[k0:k1])
-                ket = contract('kpoy,io->kpiy', wk1_Pko_kslice, mocc_2[i0:i1])
-                hk_ao_ao[i0:i1,k0:k1] += contract('ipkx,kpiy->ikxy', bra, ket)
+                bra = contract('piox,ko->pikx', rhok1_Pko, mocc_2[k0:k1])
+                ket = contract('pkoy,io->pkiy', wk1_Pko_kslice, mocc_2[i0:i1])
+                hk_ao_ao[i0:i1,k0:k1] += contract('pikx,pkiy->ikxy', bra, ket)
                 bra = ket = None
             wk1_Pko_kslice = None
             if hessobj.auxbasis_response:
                 # (10|0)(1|00)
-                wk_ip2_Ipo = contract('porx,io->iprx', wk_ip2_P__, mocc_2[i0:i1])
-                hk_ao_aux[i0:i1] += contract('ipox,ipoy->ipxy', rhok1_Pko, wk_ip2_Ipo)
+                wk_ip2_Ipo = contract('porx,io->pirx', wk_ip2_P__, mocc_2[i0:i1])
+                hk_ao_aux[i0:i1] += contract('piox,pioy->ipxy', rhok1_Pko, wk_ip2_Ipo)
                 wk_ip2_Ipo = None
 
                 # (10|0)(1|0)(0|00)
                 rhok0_P_I = contract('qor,ir->qoi', rhok0_P__, mocc_2[i0:i1])
-                wk1_P_I = contract('ypq,qoi->ipoy', int2c_ip1, rhok0_P_I)
-                hk_ao_aux[i0:i1] -= contract("ipox,ipoy->ipxy", rhok1_Pko, wk1_P_I)
-                wk1_P_I = rhok1_Pko = None
+                wk1_P_I = contract('ypq,qoi->pioy', int2c_ip1, rhok0_P_I)
+                hk_ao_aux[i0:i1] -= contract("piox,pioy->ipxy", rhok1_Pko, wk1_P_I)
+                wk1_P_I = None
 
                 # (10|0)(0|1)(0|00)
-                for q0,q1 in lib.prange(0,naux,64):
-                    wk1_I = contract('yqp,ipox->iqoxy', int2c_ip1_inv[:,q0:q1], wk1_Pko_islice)
-                    hk_ao_aux[i0:i1,q0:q1] -= contract('qoi,iqoxy->iqxy', rhok0_P_I[q0:q1], wk1_I)
+                #for q0,q1 in lib.prange(0,naux,64):
+                wk1_I = contract('yqp,piox->qioxy', int2c_ip1, rhok1_Pko)
+                hk_ao_aux[i0:i1] -= contract('qoi,qioxy->iqxy', rhok0_P_I, wk1_I)
+                #wk1_I = contract('piox,qoi->ipqx', rhok1_Pko, rhok0_P_I)
+                #hk_ao_aux[i0:i1] -= contract('ipqx,yqp->iqxy', wk1_I, int2c_ip1)
                 wk1_I = rhok0_P_I = None
-            wk1_Pko_islice = None
+
     wk1_Pko = None
     t1 = log.timer_debug1('intermediate variables with int3c2e_ip1', *t1)
 
     cupy.get_default_memory_pool().free_all_blocks()
     #  int3c_ipip1 contributions
     hj_ao_diag, hk_ao_diag = int3c2e.get_int3c2e_ipip1_hjk(intopt, rhoj0_P, rhok0_P__, dm0_tag, omega=omega, with_k=with_k)
     hj_ao_diag *= 2.0
@@ -245,14 +257,15 @@
         int2c_ip1ip2 = None
 
     cupy.get_default_memory_pool().free_all_blocks()
     release_gpu_stack()
     # aux-aux pair
     if hessobj.auxbasis_response > 1:
         wj0_10 = contract('ypq,p->ypq', int2c_ip1, rhoj0_P)
+        int2c_ip1_inv = contract('yqp,pr->yqr', int2c_ip1, int2c_inv)
 
         rhoj0_10 = contract('p,xpq->xpq', rhoj0_P, int2c_ip1_inv)     # (1|0)(0|00)
         hj_aux_aux += .5 * contract('xpr,yqr->pqxy', rhoj0_10, wj0_10)  # (00|0)(1|0), (0|1)(0|00)
         hj_aux_aux +=      contract('xpq,yq->pqxy',  rhoj0_10, wj0_01)  # (00|0)(1|0), (1|0)(0|00)
         rhoj0_10 = rhoj0_P = None
 
         rhoj1 = contract('px,pq->xpq', wj_ip2, int2c_inv)             # (0|0)(1|00)
@@ -444,29 +457,30 @@
 
     mocc = mocc[ao_idx, :]
     mo_coeff = mo_coeff[ao_idx,:]
     dm0 = take_last2d(dm0, ao_idx)
     dm0_tag = tag_array(dm0, occ_coeff=mocc)
 
     int2c = take_last2d(int2c, aux_ao_idx)
-    int2c_inv = pinv(int2c, lindep=LINEAR_DEP_THRESHOLD)
+    solve_j2c = _gen_metric_solver(int2c)
     int2c = None
 
     wj, wk_Pl_ = int3c2e.get_int3c2e_wjk(mol, auxmol, dm0_tag, omega=omega)
-    rhoj0 = contract('pq,q->p', int2c_inv, wj)
+    rhoj0 = solve_j2c(wj)
+
     wj = None
     if isinstance(wk_Pl_, cupy.ndarray):
-        rhok0_Pl_ = contract('pq,qio->pio', int2c_inv, wk_Pl_)
+        rhok0_Pl_ = solve_j2c(wk_Pl_)
     else:
         rhok0_Pl_ = np.empty_like(wk_Pl_)
         for p0, p1 in lib.prange(0,nao,64):
             wk_tmp = cupy.asarray(wk_Pl_[:,p0:p1])
-            rhok0_Pl_[:,p0:p1] = contract('pq,qio->pio', int2c_inv, wk_tmp).get()
+            rhok0_Pl_[:,p0:p1] = solve_j2c(wk_tmp).get()
         wk_tmp = None
-    wk_Pl_ = int2c_inv = None
+    wk_Pl_ = None
 
     # -----------------------------
     # int3c_ip1 contributions
     # ------------------------------
     cupy.get_default_memory_pool().free_all_blocks()
     fn = int3c2e.get_int3c2e_ip1_vjk
     vj1_buf, vk1_buf, vj1_ao, vk1_ao = fn(intopt, rhoj0, rhok0_Pl_, dm0_tag, aoslices, omega=omega)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/rks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/uhf.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,25 @@
 '''
 
 
 
 import numpy
 import cupy
 import numpy as np
-from pyscf import lib, df
+from pyscf import lib
 from gpu4pyscf.grad import rhf as rhf_grad
 from gpu4pyscf.hessian import uhf as uhf_hess
 from gpu4pyscf.hessian import rhf as rhf_hess
-from gpu4pyscf.lib.cupy_helper import contract, tag_array, release_gpu_stack, print_mem_info, take_last2d
-from gpu4pyscf.df import int3c2e
+from gpu4pyscf.lib.cupy_helper import (
+    contract, tag_array, release_gpu_stack, print_mem_info, take_last2d, pinv)
+from gpu4pyscf.df import int3c2e, df
 from gpu4pyscf.lib import logger
+from gpu4pyscf.df.grad.rhf import _gen_metric_solver
 
+LINEAR_DEP_THRESHOLD = df.LINEAR_DEP_THR
 BLKSIZE = 256
 
 def partial_hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
                       atmlst=None, max_memory=4000, verbose=None):
     e1, ej, ek = _partial_hess_ejk(hessobj, mo_energy, mo_coeff, mo_occ,
                                    atmlst, max_memory, verbose, True)
     return e1 + ej - ek
@@ -101,110 +104,111 @@
     moccb = moccb[ao_idx, :]
     dm0a = take_last2d(dm0a, ao_idx)
     dm0b = take_last2d(dm0b, ao_idx)
     dm0a_tag = tag_array(dm0a, occ_coeff=mocca)
     dm0b_tag = tag_array(dm0b, occ_coeff=moccb)
     int2c = cupy.asarray(int2c, order='C')
     int2c = take_last2d(int2c, aux_ao_idx)
-    int2c_inv = cupy.linalg.pinv(int2c, rcond=1e-12)
+    int2c_inv = pinv(int2c, lindep=LINEAR_DEP_THRESHOLD)
+    solve_j2c = _gen_metric_solver(int2c)
     int2c = None
 
     int2c_ip1 = cupy.asarray(int2c_ip1, order='C')
     int2c_ip1 = take_last2d(int2c_ip1, aux_ao_idx)
 
     hj_ao_ao = cupy.zeros([nao,nao,3,3])
     hk_ao_ao = cupy.zeros([nao,nao,3,3])
     if hessobj.auxbasis_response:
         hj_ao_aux = cupy.zeros([nao,naux,3,3])
         hk_ao_aux = cupy.zeros([nao,naux,3,3])
 
     #  int3c contributions
     wja, wka_P__ = int3c2e.get_int3c2e_jk(mol, auxmol, dm0a_tag, omega=omega)
     wjb, wkb_P__ = int3c2e.get_int3c2e_jk(mol, auxmol, dm0b_tag, omega=omega)
-    rhoj0_P = contract('pq,q->p', int2c_inv, wja + wjb)
-    rhok0a_P__ = contract('pq,qij->pij', int2c_inv, wka_P__)
-    rhok0b_P__ = contract('pq,qij->pij', int2c_inv, wkb_P__)
+    rhoj0_P = solve_j2c(wja + wjb)
+    rhok0a_P__ = solve_j2c(wka_P__)
+    rhok0b_P__ = solve_j2c(wkb_P__)
     wja = wjb = wka_P__ = wkb_P__ = None
     t1 = log.timer_debug1('intermediate variables with int3c2e', *t1)
 
     # int3c_ip2 contributions
     wja_ip2, wka_ip2_P__ = int3c2e.get_int3c2e_ip2_wjk(intopt, dm0a_tag, omega=omega)
     wjb_ip2, wkb_ip2_P__ = int3c2e.get_int3c2e_ip2_wjk(intopt, dm0b_tag, omega=omega)
     wj_ip2 = wja_ip2 + wjb_ip2
     t1 = log.timer_debug1('interdeidate variables with int3c2e_ip2', *t1)
 
     #  int3c_ip1 contributions
     wj1a_P, wk1a_Pko = int3c2e.get_int3c2e_ip1_wjk(intopt, dm0a_tag, omega=omega)
     wj1b_P, wk1b_Pko = int3c2e.get_int3c2e_ip1_wjk(intopt, dm0b_tag, omega=omega)
     wj1_P = wj1a_P + wj1b_P
-    rhoj1_P = contract('pq,ipx->iqx', int2c_inv, wj1_P)
+    rhoj1_P = solve_j2c(wj1_P)
 
-    hj_ao_ao += 4.0*contract('ipx,jpy->ijxy', rhoj1_P, wj1_P)   # (10|0)(0|0)(0|01)
+    hj_ao_ao += 4.0*contract('pix,pjy->ijxy', rhoj1_P, wj1_P)   # (10|0)(0|0)(0|01)
     wj1_P = None
     if hessobj.auxbasis_response:
         wj0_01 = contract('ypq,q->yp', int2c_ip1, rhoj0_P)
-        wj1_01 = contract('yqp,ipx->iqxy', int2c_ip1, rhoj1_P)
-        hj_ao_aux += contract('ipx,py->ipxy', rhoj1_P, wj_ip2)   # (10|0)(1|00)
-        hj_ao_aux -= contract('ipx,yp->ipxy', rhoj1_P, wj0_01)   # (10|0)(1|0)(0|00)
+        wj1_01 = contract('yqp,pix->iqxy', int2c_ip1, rhoj1_P)
+        hj_ao_aux += contract('pix,py->ipxy', rhoj1_P, wj_ip2)   # (10|0)(1|00)
+        hj_ao_aux -= contract('pix,yp->ipxy', rhoj1_P, wj0_01)   # (10|0)(1|0)(0|00)
         hj_ao_aux -= contract('q,iqxy->iqxy', rhoj0_P, wj1_01)   # (10|0)(0|1)(0|00)
         wj1_01 = None
     rhoj1_P = None
 
-    int2c_ip1_inv = contract('yqp,pr->yqr', int2c_ip1, int2c_inv)
     if with_k:
         for i0, i1 in lib.prange(0,nao,64):
-            wk1a_Pko_islice = cupy.asarray(wk1a_Pko[i0:i1])
-            wk1b_Pko_islice = cupy.asarray(wk1b_Pko[i0:i1])
-            rhok1a_Pko = contract('pq,iqox->ipox', int2c_inv, wk1a_Pko_islice)
-            rhok1b_Pko = contract('pq,iqox->ipox', int2c_inv, wk1b_Pko_islice)
+            wk1a_Pko_islice = cupy.asarray(wk1a_Pko[:,i0:i1])
+            wk1b_Pko_islice = cupy.asarray(wk1b_Pko[:,i0:i1])
+            rhok1a_Pko = solve_j2c(wk1a_Pko_islice)
+            rhok1b_Pko = solve_j2c(wk1b_Pko_islice)
+            wk1a_Pko_islice = wk1b_Pko_islice = None
             for k0, k1 in lib.prange(0,nao,64):
-                wk1a_Pko_kslice = cupy.asarray(wk1a_Pko[k0:k1])
-                wk1b_Pko_kslice = cupy.asarray(wk1b_Pko[k0:k1])
+                wk1a_Pko_kslice = cupy.asarray(wk1a_Pko[:,k0:k1])
+                wk1b_Pko_kslice = cupy.asarray(wk1b_Pko[:,k0:k1])
 
                 # (10|0)(0|10) without response of RI basis
-                vk2_ip1_ip1 = contract('ipox,kpoy->ikxy', rhok1a_Pko, wk1a_Pko_kslice)
+                vk2_ip1_ip1 = contract('piox,pkoy->ikxy', rhok1a_Pko, wk1a_Pko_kslice)
                 hk_ao_ao[i0:i1,k0:k1] += contract('ikxy,ik->ikxy', vk2_ip1_ip1, dm0a[i0:i1,k0:k1])
-                vk2_ip1_ip1 = contract('ipox,kpoy->ikxy', rhok1b_Pko, wk1b_Pko_kslice)
+                vk2_ip1_ip1 = contract('piox,pkoy->ikxy', rhok1b_Pko, wk1b_Pko_kslice)
                 hk_ao_ao[i0:i1,k0:k1] += contract('ikxy,ik->ikxy', vk2_ip1_ip1, dm0b[i0:i1,k0:k1])
                 vk2_ip1_ip1 = None
 
                 # (10|0)(0|01) without response of RI basis
-                bra = contract('ipox,ko->ipkx', rhok1a_Pko, mocca[k0:k1])
-                ket = contract('kpoy,io->kpiy', wk1a_Pko_kslice, mocca[i0:i1])
-                hk_ao_ao[i0:i1,k0:k1] += contract('ipkx,kpiy->ikxy', bra, ket)
-                bra = contract('ipox,ko->ipkx', rhok1b_Pko, moccb[k0:k1])
-                ket = contract('kpoy,io->kpiy', wk1b_Pko_kslice, moccb[i0:i1])
-                hk_ao_ao[i0:i1,k0:k1] += contract('ipkx,kpiy->ikxy', bra, ket)
+                bra = contract('piox,ko->pikx', rhok1a_Pko, mocca[k0:k1])
+                ket = contract('pkoy,io->pkiy', wk1a_Pko_kslice, mocca[i0:i1])
+                hk_ao_ao[i0:i1,k0:k1] += contract('pikx,pkiy->ikxy', bra, ket)
+                bra = contract('piox,ko->pikx', rhok1b_Pko, moccb[k0:k1])
+                ket = contract('pkoy,io->pkiy', wk1b_Pko_kslice, moccb[i0:i1])
+                hk_ao_ao[i0:i1,k0:k1] += contract('pikx,pkiy->ikxy', bra, ket)
                 bra = ket = None
             wk1a_Pko_kslice = wk1a_Pko_kslice = None
             if hessobj.auxbasis_response:
                 # (10|0)(1|00)
-                wk_ip2_Ipo = contract('porx,io->iprx', wka_ip2_P__, mocca[i0:i1])
-                hk_ao_aux[i0:i1] += contract('ipox,ipoy->ipxy', rhok1a_Pko, wk_ip2_Ipo)
-                wk_ip2_Ipo = contract('porx,io->iprx', wkb_ip2_P__, moccb[i0:i1])
-                hk_ao_aux[i0:i1] += contract('ipox,ipoy->ipxy', rhok1b_Pko, wk_ip2_Ipo)
+                wk_ip2_Ipo = contract('porx,io->pirx', wka_ip2_P__, mocca[i0:i1])
+                hk_ao_aux[i0:i1] += contract('piox,pioy->ipxy', rhok1a_Pko, wk_ip2_Ipo)
+                wk_ip2_Ipo = contract('porx,io->pirx', wkb_ip2_P__, moccb[i0:i1])
+                hk_ao_aux[i0:i1] += contract('piox,pioy->ipxy', rhok1b_Pko, wk_ip2_Ipo)
                 wk_ip2_Ipo = None
 
                 # (10|0)(1|0)(0|00)
                 rhok0a_P_I = contract('qor,ir->qoi', rhok0a_P__, mocca[i0:i1])
-                wk1_P_I = contract('ypq,qoi->ipoy', int2c_ip1, rhok0a_P_I)
-                hk_ao_aux[i0:i1] -= contract("ipox,ipoy->ipxy", rhok1a_Pko, wk1_P_I)
+                wk1_P_I = contract('ypq,qoi->pioy', int2c_ip1, rhok0a_P_I)
+                hk_ao_aux[i0:i1] -= contract("piox,pioy->ipxy", rhok1a_Pko, wk1_P_I)
                 rhok0b_P_I = contract('qor,ir->qoi', rhok0b_P__, moccb[i0:i1])
-                wk1_P_I = contract('ypq,qoi->ipoy', int2c_ip1, rhok0b_P_I)
-                hk_ao_aux[i0:i1] -= contract("ipox,ipoy->ipxy", rhok1b_Pko, wk1_P_I)
-                wk1_P_I = rhok1a_Pko = rhok1b_Pko = None
+                wk1_P_I = contract('ypq,qoi->pioy', int2c_ip1, rhok0b_P_I)
+                hk_ao_aux[i0:i1] -= contract("piox,pioy->ipxy", rhok1b_Pko, wk1_P_I)
+                wk1_P_I = None
 
                 # (10|0)(0|1)(0|00)
                 for q0,q1 in lib.prange(0,naux,64):
-                    wk1_I = contract('yqp,ipox->iqoxy', int2c_ip1_inv[:,q0:q1], wk1a_Pko_islice)
-                    hk_ao_aux[i0:i1,q0:q1] -= contract('qoi,iqoxy->iqxy', rhok0a_P_I[q0:q1], wk1_I)
-                    wk1_I = contract('yqp,ipox->iqoxy', int2c_ip1_inv[:,q0:q1], wk1b_Pko_islice)
-                    hk_ao_aux[i0:i1,q0:q1] -= contract('qoi,iqoxy->iqxy', rhok0b_P_I[q0:q1], wk1_I)
+                    wk1_I = contract('yqp,piox->qioxy', int2c_ip1[:,q0:q1], rhok1a_Pko)
+                    hk_ao_aux[i0:i1,q0:q1] -= contract('qoi,qioxy->iqxy', rhok0a_P_I[q0:q1], wk1_I)
+                    wk1_I = contract('yqp,piox->qioxy', int2c_ip1[:,q0:q1], rhok1b_Pko)
+                    hk_ao_aux[i0:i1,q0:q1] -= contract('qoi,qioxy->iqxy', rhok0b_P_I[q0:q1], wk1_I)
                 wk1_I = rhok0a_P_I = rhok0b_P_I = None
-            wk1a_Pko_islice = wk1b_Pko_islice = None
+        rhok1a_Pko = rhok1b_Pko = None
     wk1a_Pko = wk1b_Pko = None
     t1 = log.timer_debug1('intermediate variables with int3c2e_ip1', *t1)
 
     cupy.get_default_memory_pool().free_all_blocks()
     #  int3c_ipip1 contributions
     fn = int3c2e.get_int3c2e_ipip1_hjk
     hja_ao_diag, hka_ao_diag = fn(intopt, rhoj0_P, rhok0a_P__, dm0a_tag, omega=omega, with_k=with_k)
@@ -282,14 +286,15 @@
         int2c_ip1ip2 = None
 
     cupy.get_default_memory_pool().free_all_blocks()
     release_gpu_stack()
     # aux-aux pair
     if hessobj.auxbasis_response > 1:
         wj0_10 = contract('ypq,p->ypq', int2c_ip1, rhoj0_P)
+        int2c_ip1_inv = contract('yqp,pr->yqr', int2c_ip1, int2c_inv)
 
         rhoj0_10 = contract('p,xpq->xpq', rhoj0_P, int2c_ip1_inv)     # (1|0)(0|00)
         hj_aux_aux += .5 * contract('xpr,yqr->pqxy', rhoj0_10, wj0_10)  # (00|0)(1|0), (0|1)(0|00)
         hj_aux_aux +=      contract('xpq,yq->pqxy',  rhoj0_10, wj0_01)  # (00|0)(1|0), (1|0)(0|00)
         rhoj0_10 = rhoj0_P = None
 
         rhoj1 = contract('px,pq->xpq', wj_ip2, int2c_inv)             # (0|0)(1|00)
@@ -503,43 +508,43 @@
     moccb = moccb[ao_idx, :]
     mo_coeff = mo_coeff[:, ao_idx,:]
     dm0a = take_last2d(dm0a, ao_idx)
     dm0b = take_last2d(dm0b, ao_idx)
     dm0 = dm0a + dm0b
 
     int2c = take_last2d(int2c, aux_ao_idx)
-    int2c_inv = cupy.linalg.pinv(int2c, rcond=1e-12)
+    solve_j2c = _gen_metric_solver(int2c)
     int2c = None
 
     fn = int3c2e.get_int3c2e_wjk
     dm0_tag = tag_array(dm0, occ_coeff=mocca)
     wj, wka_Pl_ = fn(mol, auxmol, dm0_tag, omega=omega)
     dm0_tag = tag_array(dm0, occ_coeff=moccb)
     wj, wkb_Pl_ = fn(mol, auxmol, dm0_tag, omega=omega)
-    rhoj0 = contract('pq,q->p', int2c_inv, wj)
+    rhoj0 = solve_j2c(wj)
     wj = None
 
     if isinstance(wka_Pl_, cupy.ndarray):
-        rhok0a_Pl_ = contract('pq,qio->pio', int2c_inv, wka_Pl_)
+        rhok0a_Pl_ = solve_j2c(wka_Pl_)
     else:
         rhok0a_Pl_ = np.empty_like(wka_Pl_)
         for p0, p1 in lib.prange(0,nao,64):
             wk_tmp = cupy.asarray(wka_Pl_[:,p0:p1])
-            rhok0a_Pl_[:,p0:p1] = contract('pq,qio->pio', int2c_inv, wk_tmp).get()
+            rhok0a_Pl_[:,p0:p1] = solve_j2c(wk_tmp).get()
         wk_tmp = None
 
     if isinstance(wkb_Pl_, cupy.ndarray):
-        rhok0b_Pl_ = contract('pq,qio->pio', int2c_inv, wkb_Pl_)
+        rhok0b_Pl_ = solve_j2c(wkb_Pl_)
     else:
         rhok0b_Pl_ = np.empty_like(wkb_Pl_)
         for p0, p1 in lib.prange(0,nao,64):
             wk_tmp = cupy.asarray(wkb_Pl_[:,p0:p1])
-            rhok0b_Pl_[:,p0:p1] = contract('pq,qio->pio', int2c_inv, wk_tmp).get()
+            rhok0b_Pl_[:,p0:p1] = solve_j2c(wk_tmp).get()
         wk_tmp = None
-    wka_Pl_ = wkb_Pl_ = int2c_inv = None
+    wka_Pl_ = wkb_Pl_ = None
 
     # -----------------------------
     # int3c_ip1 contributions
     # ------------------------------
     cupy.get_default_memory_pool().free_all_blocks()
     fn = int3c2e.get_int3c2e_ip1_vjk
     dm0_tag = tag_array(dm0, occ_coeff=mocca)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/hessian/uks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/df/int3c2e.py` & `gpu4pyscf-0.7.8/gpu4pyscf/df/int3c2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,19 @@
                     bs[:,gto.PTR_EXP] = np.arange(pexp, pexp+nprim)
                     bs[:,gto.PTR_COEFF] = np.arange(pcoeff, pcoeff+nprim)
                     bas_of_ia.append(bs)
 
             bas_of_ia = np.vstack(bas_of_ia)
             bas_templates[key] = bas_of_ia
         _bas.append(bas_of_ia)
-
+    
     pmol = copy.copy(mol)
+    pmol.output = mol.output
+    pmol.verbose = mol.verbose
+    pmol.stdout = mol.stdout
     pmol.cart = True
     pmol._bas = np.asarray(np.vstack(_bas), dtype=np.int32)
     pmol._env = _env
     return pmol
 
 def make_fake_mol():
     '''
@@ -122,14 +125,15 @@
 
     return fakemol
 
 class VHFOpt(_vhf.VHFOpt):
     def __init__(self, mol, auxmol, intor, prescreen='CVHFnoscreen',
                  qcondname='CVHFsetnr_direct_scf', dmcondname=None):
         # use local basis_seg_contraction for efficiency
+        # TODO: switch _mol and mol
         self.mol = basis_seg_contraction(mol,allow_replica=True)
         self.auxmol = basis_seg_contraction(auxmol, allow_replica=True)
         self._mol = mol
         self._auxmol = auxmol
 
         '''
         # Note mol._bas will be sorted in .build() method. VHFOpt should be
@@ -167,15 +171,16 @@
         self.log_qs = None
         self.aux_log_qs = None
 
     init_cvhf_direct = _vhf.VHFOpt.init_cvhf_direct
 
     def clear(self):
         _vhf.VHFOpt.__del__(self)
-        libgvhf.GINTdel_basis_prod(ctypes.byref(self.bpcache))
+        if self.bpcache is not None:
+            libgvhf.GINTdel_basis_prod(ctypes.byref(self.bpcache))
         return self
 
     def __del__(self):
         try:
             self.clear()
         except AttributeError:
             pass
@@ -183,76 +188,82 @@
     def build(self, cutoff=1e-14, group_size=None,
               group_size_aux=None, diag_block_with_triu=False, aosym=False):
         '''
         int3c2e is based on int2e with (ao,ao|aux,1)
         a tot_mol is created with concatenating [mol, fake_mol, aux_mol]
         we will pair (ao,ao) and (aux,1) separately.
         '''
-        cput0 = logger.init_timer(self.mol)
-        sorted_mol, sorted_idx, uniq_l_ctr, l_ctr_counts = sort_mol(self.mol)
+        _mol = self._mol
+        _auxmol = self._auxmol
+        mol = self.mol
+        auxmol = self.auxmol
+
+        log = logger.new_logger(_mol, _mol.verbose)
+        cput0 = log.init_timer()
+        sorted_mol, sorted_idx, uniq_l_ctr, l_ctr_counts = sort_mol(mol, log=log)
         if group_size is not None :
             uniq_l_ctr, l_ctr_counts = _split_l_ctr_groups(uniq_l_ctr, l_ctr_counts, group_size)
 
         # sort fake mol
         fake_mol = make_fake_mol()
-        _, _, fake_uniq_l_ctr, fake_l_ctr_counts = sort_mol(fake_mol)
+        _, _, fake_uniq_l_ctr, fake_l_ctr_counts = sort_mol(fake_mol, log=log)
 
         # sort auxiliary mol
-        sorted_auxmol, sorted_aux_idx, aux_uniq_l_ctr, aux_l_ctr_counts = sort_mol(self.auxmol)
+        sorted_auxmol, sorted_aux_idx, aux_uniq_l_ctr, aux_l_ctr_counts = sort_mol(auxmol, log=log)
         if group_size_aux is not None:
             aux_uniq_l_ctr, aux_l_ctr_counts = _split_l_ctr_groups(aux_uniq_l_ctr, aux_l_ctr_counts, group_size_aux)
 
         tot_mol = sorted_mol + fake_mol + sorted_auxmol
         tot_mol.cart = True
         self.tot_mol = tot_mol
 
         # Initialize vhfopt after reordering mol._bas
         _vhf.VHFOpt.__init__(self, sorted_mol, self._intor, self._prescreen,
                              self._qcondname, self._dmcondname)
         self.direct_scf_tol = cutoff
 
         # TODO: is it more accurate to filter with overlap_cond (or exp_cond)?
         q_cond = self.get_q_cond()
-        cput1 = logger.timer_debug1(sorted_mol, 'Initialize q_cond', *cput0)
+        cput1 = log.timer_debug1('Initialize q_cond', *cput0)
         l_ctr_offsets = np.append(0, np.cumsum(l_ctr_counts))
         log_qs, pair2bra, pair2ket = get_pairing(
             l_ctr_offsets, l_ctr_offsets, q_cond,
             diag_block_with_triu=diag_block_with_triu, aosym=aosym)
         self.log_qs = log_qs.copy()
-        cput1 = logger.timer_debug1(sorted_mol, 'Get pairing', *cput1)
+        cput1 = log.timer_debug1('Get pairing', *cput1)
 
         # contraction coefficient for ao basis
         cart_ao_loc = sorted_mol.ao_loc_nr(cart=True)
         sph_ao_loc = sorted_mol.ao_loc_nr(cart=False)
         self.cart_ao_loc = [cart_ao_loc[cp] for cp in l_ctr_offsets]
         self.sph_ao_loc = [sph_ao_loc[cp] for cp in l_ctr_offsets]
         self.angular = [l[0] for l in uniq_l_ctr]
 
-        cart_ao_loc = self.mol.ao_loc_nr(cart=True)
-        sph_ao_loc = self.mol.ao_loc_nr(cart=False)
+        cart_ao_loc = mol.ao_loc_nr(cart=True)
+        sph_ao_loc = mol.ao_loc_nr(cart=False)
         nao = sph_ao_loc[-1]
         ao_idx = np.array_split(np.arange(nao), sph_ao_loc[1:-1])
         self.sph_ao_idx = np.hstack([ao_idx[i] for i in sorted_idx])
-
+        
         # cartesian ao index
         nao = cart_ao_loc[-1]
         ao_idx = np.array_split(np.arange(nao), cart_ao_loc[1:-1])
         self.cart_ao_idx = np.hstack([ao_idx[i] for i in sorted_idx])
         ncart = cart_ao_loc[-1]
         nsph = sph_ao_loc[-1]
         self.cart2sph = block_c2s_diag(ncart, nsph, self.angular, l_ctr_counts)
-
-        if self._mol.cart:
+        
+        if _mol.cart:
             inv_idx = np.argsort(self.cart_ao_idx, kind='stable').astype(np.int32)
             self.coeff = cupy.eye(ncart)[:,inv_idx]
         else:
             inv_idx = np.argsort(self.sph_ao_idx, kind='stable').astype(np.int32)
             self.coeff = self.cart2sph[:, inv_idx]
-        cput1 = logger.timer_debug1(sorted_mol, 'AO cart2sph coeff', *cput1)
-
+        cput1 = log.timer_debug1('AO cart2sph coeff', *cput1)
+        
         # pairing auxiliary basis with fake basis set
         fake_l_ctr_offsets = np.append(0, np.cumsum(fake_l_ctr_counts))
         fake_l_ctr_offsets += l_ctr_offsets[-1]
         aux_l_ctr_offsets = np.append(0, np.cumsum(aux_l_ctr_counts))
 
         # contraction coefficient for auxiliary basis
         cart_aux_loc = sorted_auxmol.ao_loc_nr(cart=True)
@@ -271,31 +282,31 @@
         naux = cart_aux_loc[-1]
         ao_idx = np.array_split(np.arange(naux), cart_aux_loc[1:-1])
         self.cart_aux_idx = np.hstack([ao_idx[i] for i in sorted_aux_idx])
         ncart = cart_aux_loc[-1]
         nsph = sph_aux_loc[-1]
         self.aux_cart2sph = block_c2s_diag(ncart, nsph, self.aux_angular, aux_l_ctr_counts)
 
-        if self._auxmol.cart:
+        if _auxmol.cart:
             inv_idx = np.argsort(self.cart_aux_idx, kind='stable').astype(np.int32)
             self.aux_coeff = cupy.eye(ncart)[:,inv_idx]
         else:
             inv_idx = np.argsort(self.sph_aux_idx, kind='stable').astype(np.int32)
             self.aux_coeff = self.aux_cart2sph[:, inv_idx]
         aux_l_ctr_offsets += fake_l_ctr_offsets[-1]
-        cput1 = logger.timer_debug1(tot_mol, 'aux cart2sph coeff', *cput1)
+        cput1 = log.timer_debug1('aux cart2sph coeff', *cput1)
 
-        ao_loc = sorted_mol.ao_loc_nr(cart=self._mol.cart)
+        ao_loc = sorted_mol.ao_loc_nr(cart=_mol.cart)
         self.ao_pairs_row, self.ao_pairs_col = get_ao_pairs(pair2bra, pair2ket, ao_loc)
         cderi_row = cupy.hstack(self.ao_pairs_row)
         cderi_col = cupy.hstack(self.ao_pairs_col)
         self.cderi_row = cderi_row
         self.cderi_col = cderi_col
         self.cderi_diag = cupy.argwhere(cderi_row == cderi_col)[:,0]
-        cput1 = logger.timer_debug1(tot_mol, 'Get AO pairs', *cput1)
+        cput1 = log.timer_debug1('Get AO pairs', *cput1)
 
         aux_pair2bra = []
         aux_pair2ket = []
         aux_log_qs = []
         for p0, p1 in zip(aux_l_ctr_offsets[:-1], aux_l_ctr_offsets[1:]):
             aux_pair2bra.append(np.arange(p0,p1,dtype=np.int32))
             aux_pair2ket.append(fake_l_ctr_offsets[0] * np.ones(p1-p0, dtype=np.int32))
@@ -329,31 +340,31 @@
             ao_loc.ctypes.data_as(ctypes.c_void_p),
             bas_pair2shls.ctypes.data_as(ctypes.c_void_p),
             bas_pairs_locs.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(ncptype),
             tot_mol._atm.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(tot_mol.natm),
             tot_mol._bas.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(tot_mol.nbas),
             tot_mol._env.ctypes.data_as(ctypes.c_void_p))
 
-        cput1 = logger.timer_debug1(tot_mol, 'Initialize GPU cache', *cput1)
+        cput1 = log.timer_debug1('Initialize GPU cache', *cput1)
         self.bas_pairs_locs = bas_pairs_locs
         ncptype = len(self.log_qs)
         self.aosym = aosym
         if aosym:
             self.cp_idx, self.cp_jdx = np.tril_indices(ncptype)
         else:
             nl = int(round(np.sqrt(ncptype)))
             self.cp_idx, self.cp_jdx = np.unravel_index(np.arange(ncptype), (nl, nl))
 
-        if self._mol.cart:
+        if _mol.cart:
             self.ao_loc = self.cart_ao_loc
             self.ao_idx = self.cart_ao_idx
         else:
             self.ao_loc = self.sph_ao_loc
             self.ao_idx = self.sph_ao_idx
-        if self._auxmol.cart:
+        if _auxmol.cart:
             self.aux_ao_loc = self.cart_aux_loc
             self.aux_ao_idx = self.cart_aux_idx
         else:
             self.aux_ao_loc = self.sph_aux_loc
             self.aux_ao_idx = self.sph_aux_idx
 
         self.rev_ao_idx = np.argsort(self.ao_idx, kind='stable').astype(np.int32)
@@ -898,42 +909,42 @@
     get wj and wk for int3c2e_ip1
     '''
     nao = len(intopt.ao_idx)
     naux = len(intopt.aux_ao_idx)
     orbo = cupy.asarray(dm0_tag.occ_coeff, order='C')
     nocc = orbo.shape[1]
 
-    wj = cupy.zeros([nao,naux,3])
+    wj = cupy.zeros([naux,nao,3])
     avail_mem = get_avail_mem()
     use_gpu_memory = True
     if nao*naux*nocc*3*8 < 0.4*avail_mem:
         try:
-            wk = cupy.empty([nao,naux,nocc,3])
+            wk = cupy.empty([naux,nao,nocc,3])
         except Exception:
             use_gpu_memory = False
     else:
         use_gpu_memory = False
 
     if not use_gpu_memory:
         mem = cupy.cuda.alloc_pinned_memory(nao*naux*nocc*3*8)
-        wk = np.ndarray([nao,naux,nocc,3], dtype=np.float64, order='C', buffer=mem)
+        wk = np.ndarray([naux,nao,nocc,3], dtype=np.float64, order='C', buffer=mem)
 
     # TODO: async data transfer
     ncp_ij = len(intopt.log_qs)
     count = 0
     for i0,i1,j0,j1,k0,k1,int3c_blk in loop_int3c2e_general(intopt, ip_type='ip1', omega=omega):
         if count % ncp_ij == 0:
-            wk_tmp = cupy.zeros([nao, k1-k0, nocc, 3])
-        wj[i0:i1,k0:k1] += contract('xpji,ij->ipx', int3c_blk, dm0_tag[i0:i1,j0:j1])
-        wk_tmp[i0:i1,:] += contract('xpji,jo->ipox', int3c_blk, orbo[j0:j1])
+            wk_tmp = cupy.zeros([k1-k0,nao,nocc,3])
+        wj[k0:k1,i0:i1] += contract('xpji,ij->pix', int3c_blk, dm0_tag[i0:i1,j0:j1])
+        wk_tmp[:,i0:i1] += contract('xpji,jo->piox', int3c_blk, orbo[j0:j1])
         if (count+1) % ncp_ij == 0:
             if use_gpu_memory:
-                wk[:,k0:k1] = wk_tmp
+                wk[k0:k1] = wk_tmp
             else:
-                wk[:,k0:k1] = wk_tmp.get()
+                wk[k0:k1] = wk_tmp.get()
         count += 1
     return wj, wk
 
 def get_int3c2e_ip2_wjk(intopt, dm0_tag, with_k=True, omega=None):
     '''
     get wj and wk for int3c2e_ip2
     '''
@@ -1041,14 +1052,17 @@
     '''
     calculate int1e_ipiprinv contribution
     '''
     coords = mol.atom_coords()
     charges = cupy.asarray(mol.atom_charges(), dtype=np.float64)
 
     fakemol = gto.fakemol_for_charges(coords)
+    fakemol.output = mol.output
+    fakemol.verbose = mol.verbose
+    fakemol.stdout = mol.stdout
     intopt = VHFOpt(mol, fakemol, 'int2e')
     intopt.build(1e-14, diag_block_with_triu=True, aosym=False, group_size=BLKSIZE, group_size_aux=BLKSIZE)
     ao_idx = intopt.ao_idx
     dm = take_last2d(cupy.asarray(dm), ao_idx)
 
     natm = mol.natm
     nao = mol.nao
@@ -1334,28 +1348,33 @@
     contract 'int1e_iprinv', with density matrix
     xijk,ij->kx
     '''
     natm = mol.natm
     coords = mol.atom_coords()
     charges = cupy.asarray(mol.atom_charges(), dtype=np.float64)
     fakemol = gto.fakemol_for_charges(coords)
+    fakemol.output = mol.output
+    fakemol.verbose = mol.verbose
+    fakemol.stdout = mol.stdout
     intopt = VHFOpt(mol, fakemol, 'int2e')
     intopt.build(1e-14, diag_block_with_triu=True, aosym=False, group_size=BLKSIZE, group_size_aux=BLKSIZE)
     dm0_sorted = take_last2d(dm0, intopt.ao_idx)
     dh1e = cupy.zeros([natm,3])
     for i0,i1,j0,j1,k0,k1,int3c_blk in loop_int3c2e_general(intopt, ip_type='ip1'):
         dh1e[k0:k1,:3] += contract('xkji,ij->kx', int3c_blk, dm0_sorted[i0:i1,j0:j1])
     return 2.0 * contract('kx,k->kx', dh1e, -charges)
 
 def get_d2h1e(mol, dm0):
     natm = mol.natm
     coords = mol.atom_coords()
     charges = cupy.asarray(mol.atom_charges(), dtype=np.float64)
     fakemol = gto.fakemol_for_charges(coords)
-
+    fakemol.output = mol.output
+    fakemol.stdout = mol.stdout
+    fakemol.verbose = mol.verbose
     nao = mol.nao
     d2h1e_diag = cupy.zeros([natm,9])
     d2h1e_offdiag = cupy.zeros([natm, nao, 9])
     intopt = VHFOpt(mol, fakemol, 'int2e')
     intopt.build(1e-14, diag_block_with_triu=True, aosym=False, group_size=BLKSIZE, group_size_aux=BLKSIZE)
     dm0_sorted = take_last2d(dm0, intopt.ao_idx)
     for i0,i1,j0,j1,k0,k1,int3c_blk in loop_int3c2e_general(intopt, ip_type='ipip1'):
@@ -1584,29 +1603,31 @@
     intopt = VHFOpt(mol, auxmol, 'int2e')
     intopt.build(direct_scf_tol, diag_block_with_triu=True, aosym=True)
     int2c = get_int2c2e_sorted(mol, auxmol, intopt=intopt)
     aux_idx = np.argsort(intopt.aux_ao_idx)
     int2c = int2c[np.ix_(aux_idx, aux_idx)]
     return int2c
 
-def sort_mol(mol0, cart=True):
+def sort_mol(mol0, cart=True, log=None):
     '''
     # Sort basis according to angular momentum and contraction patterns so
     # as to group the basis functions to blocks in GPU kernel.
     '''
+    if log is None:
+        log = logger.new_logger(mol0, mol0.verbose)
     mol = mol0.copy(deep=True)
     l_ctrs = mol._bas[:,[gto.ANG_OF, gto.NPRIM_OF]]
-
+    
     uniq_l_ctr, _, inv_idx, l_ctr_counts = np.unique(
         l_ctrs, return_index=True, return_inverse=True, return_counts=True, axis=0)
-
+    
     if mol.verbose >= logger.DEBUG:
-        logger.debug1(mol, 'Number of shells for each [l, nctr] group')
+        log.debug1('Number of shells for each [l, nctr] group')
         for l_ctr, n in zip(uniq_l_ctr, l_ctr_counts):
-            logger.debug(mol, '    %s : %s', l_ctr, n)
+            log.debug('    %s : %s', l_ctr, n)
 
     sorted_idx = np.argsort(inv_idx, kind='stable').astype(np.int32)
 
     # Sort basis inplace
     mol._bas = mol._bas[sorted_idx]
     return mol, sorted_idx, uniq_l_ctr, l_ctr_counts
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/gen_grid.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/gen_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,20 +68,21 @@
 
     Returns:
         A list has the same length as rads. The list element is the number of
         grids over angular part for each radial grid.
     '''
 # In SG1 the ang grids for the five regions
 #            6  38 86  194 86
-    leb_ngrid = numpy.array([6, 38, 86, 194, 86])
-    alphas = numpy.array((
+    leb_ngrid = cupy.array([6, 38, 86, 194, 86])
+    alphas = cupy.array((
         (0.25  , 0.5, 1.0, 4.5),
         (0.1667, 0.5, 0.9, 3.5),
         (0.1   , 0.4, 0.8, 2.5)))
     r_atom = radii[nuc] + 1e-200
+    rads = cupy.asarray(rads)
     if nuc <= 2:  # H, He
         place = ((rads/r_atom).reshape(-1,1) > alphas[0]).sum(axis=1)
     elif nuc <= 10:  # Li - Ne
         place = ((rads/r_atom).reshape(-1,1) > alphas[1]).sum(axis=1)
     else:
         place = ((rads/r_atom).reshape(-1,1) > alphas[2]).sum(axis=1)
     return leb_ngrid[place]
@@ -115,15 +116,15 @@
     if n_ang < 50:
         return numpy.repeat(n_ang, len(rads))
     elif n_ang == 50:
         leb_l = numpy.array([1, 2, 2, 2, 1])
     else:
         idx = numpy.where(leb_ngrid==n_ang)[0][0]
         leb_l = numpy.array([1, 3, idx-1, idx, idx-1])
-    r_atom = radii[nuc].get() + 1e-200
+    r_atom = radii[nuc] + 1e-200
     if nuc <= 2:  # H, He
         place = ((rads/r_atom).reshape(-1,1) > alphas[0]).sum(axis=1)
     elif nuc <= 10:  # Li - Ne
         place = ((rads/r_atom).reshape(-1,1) > alphas[1]).sum(axis=1)
     else:
         place = ((rads/r_atom).reshape(-1,1) > alphas[2]).sum(axis=1)
     angs = leb_l[place]
@@ -240,15 +241,15 @@
 
             if callable(prune):
                 angs = prune(chg, rad, n_ang)
             else:
                 angs = [n_ang] * n_rad
             logger.debug(mol, 'atom %s rad-grids = %d, ang-grids = %s',
                          symb, n_rad, angs)
-
+            if isinstance(angs, cupy.ndarray): angs = angs.get()
             angs = numpy.array(angs)
             coords = []
             vol = []
             for n in sorted(set(angs)):
                 grid = numpy.empty((n,4))
                 libdft.MakeAngularGrid(grid.ctypes.data_as(ctypes.c_void_p),
                                        ctypes.c_int(n))
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/gks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/gks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/libxc.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc_structs.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/libxc_structs.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/numint.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/numint.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,26 +60,27 @@
         ao_loc_slice:      offsets of ao slices to be evaluated
         ctr_offsets_slice: offsets of contraction patterns
     Returns:
         ao: comp x nao_slice x ngrids, ao is in C-contiguous
     '''
     opt = getattr(ni, 'gdftopt', None)
     with_opt = True
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, coords)
         opt = ni.gdftopt
         with_opt = False
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
 
     if shls_slice is None:
-        shls_slice = cupy.arange(mol.nbas, dtype=np.int32)
+        shls_slice = cupy.arange(_sorted_mol.nbas, dtype=np.int32)
         ctr_offsets = opt.l_ctr_offsets
         ctr_offsets_slice = opt.l_ctr_offsets
-        ao_loc_slice = cupy.asarray(mol.ao_loc_nr())
-        nao_slice = mol.nao
+        ao_loc_slice = cupy.asarray(_sorted_mol.ao_loc_nr())
+        nao_slice = _sorted_mol.nao
     else:
         ctr_offsets = opt.l_ctr_offsets
 
     nctr = ctr_offsets.size - 1
     ngrids = coords.shape[0]
     coords = cupy.asarray(coords.T, order='C')
     comp = (deriv+1)*(deriv+2)*(deriv+3)//6
@@ -92,42 +93,42 @@
         else:
             out[:] = 0
     else:
         if out is None:
             out = cupy.empty((comp, nao_slice, ngrids), order='C')
 
     if not with_opt:
-        # mol may be different to _GDFTOpt.mol.
-        # nao should be consistent with the _GDFTOpt.mol object
+        # mol may be different to _GDFTOpt._sorted_mol.
+        # nao should be consistent with the _GDFTOpt._sorted_mol object
         coeff = cupy.asarray(opt.coeff)
         with opt.gdft_envs_cache():
             err = libgdft.GDFTeval_gto(
                 ctypes.cast(stream.ptr, ctypes.c_void_p),
                 ctypes.cast(out.data.ptr, ctypes.c_void_p),
-                ctypes.c_int(deriv), ctypes.c_int(opt.mol.cart),
+                ctypes.c_int(deriv), ctypes.c_int(_sorted_mol.cart),
                 ctypes.cast(coords.data.ptr, ctypes.c_void_p), ctypes.c_int(ngrids),
                 ctypes.cast(shls_slice.data.ptr, ctypes.c_void_p),
                 ctypes.cast(ao_loc_slice.data.ptr, ctypes.c_void_p),
                 ctypes.c_int(nao_slice),
                 ctr_offsets.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(nctr),
                 ctr_offsets_slice.ctypes.data_as(ctypes.c_void_p),
-                mol._bas.ctypes.data_as(ctypes.c_void_p))
+                _sorted_mol._bas.ctypes.data_as(ctypes.c_void_p))
             out = contract('nig,ij->njg', out, coeff).transpose([0,2,1])
     else:
         err = libgdft.GDFTeval_gto(
             ctypes.cast(stream.ptr, ctypes.c_void_p),
             ctypes.cast(out.data.ptr, ctypes.c_void_p),
-            ctypes.c_int(deriv), ctypes.c_int(opt.mol.cart),
+            ctypes.c_int(deriv), ctypes.c_int(_sorted_mol.cart),
             ctypes.cast(coords.data.ptr, ctypes.c_void_p), ctypes.c_int(ngrids),
             ctypes.cast(shls_slice.data.ptr, ctypes.c_void_p),
             ctypes.cast(ao_loc_slice.data.ptr, ctypes.c_void_p),
             ctypes.c_int(nao_slice),
             ctr_offsets.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(nctr),
             ctr_offsets_slice.ctypes.data_as(ctypes.c_void_p),
-            mol._bas.ctypes.data_as(ctypes.c_void_p))
+            _sorted_mol._bas.ctypes.data_as(ctypes.c_void_p))
     if err != 0:
         raise RuntimeError('CUDA Error in evaluating AO')
 
     if deriv == 0:
         out = out[0]
     return out
 
@@ -442,22 +443,22 @@
     return exc,vxc
 
 def nr_rks(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
            max_memory=2000, verbose=None):
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_coeff = getattr(dms, 'mo_coeff', None)
     mo_occ = getattr(dms,'mo_occ', None)
-
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dm_shape = dms.shape
     #dms = [coeff @ dm @ coeff.T for dm in dms.reshape(-1,nao0,nao0)]
     dms = dms.reshape(-1,nao0,nao0)
     dms = take_last2d(dms, opt.ao_idx)
@@ -465,25 +466,15 @@
 
     if mo_coeff is not None:
         mo_coeff = mo_coeff[opt.ao_idx]
 
     nelec = cupy.zeros(nset)
     excsum = cupy.zeros(nset)
     vmat = cupy.zeros((nset, nao, nao))
-    '''
-    ao_loc = mol.ao_loc_nr()
-    if USE_SPARSITY == 1:
-        nbins = NBINS * 2 - int(NBINS * np.log(ni.cutoff) / np.log(grids.cutoff))
-        pair2shls, pairs_locs = _make_pairs2shls_idx(ni.pair_mask, opt.l_bas_offsets, hermi)
-        if hermi:
-            pair2shls_full, pairs_locs_full = _make_pairs2shls_idx(ni.pair_mask,
-                                                               opt.l_bas_offsets)
-        else:
-            pair2shls_full, pairs_locs_full = pair2shls, pairs_locs
-    '''
+
     release_gpu_stack()
     if xctype == 'LDA':
         ao_deriv = 0
     else:
         ao_deriv = 1
     with_lapl = MGGA_DENSITY_LAPL
     ngrids = grids.weights.size
@@ -494,26 +485,25 @@
     else:
         if with_lapl:
             rho_tot = cupy.empty([nset,6,ngrids])
         else:
             rho_tot = cupy.empty([nset,5,ngrids])
     p0 = p1 = 0
     t1 = t0 = log.init_timer()
-    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+    for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         p1 = p0 + weight.size
         for i in range(nset):
             if mo_coeff is None:
-                rho_tot[i,:,p0:p1] = eval_rho(mol, ao_mask, dms[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
+                rho_tot[i,:,p0:p1] = eval_rho(_sorted_mol, ao_mask, dms[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
             else:
                 mo_coeff_mask = mo_coeff[idx,:]
-                rho_tot[i,:,p0:p1] = eval_rho2(mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
+                rho_tot[i,:,p0:p1] = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
         p0 = p1
         t1 = log.timer_debug2('eval rho slice', *t1)
     t0 = log.timer_debug1('eval rho', *t0)
-
     wv = []
     for i in range(nset):
         if xctype == 'LDA':
             exc, vxc = ni.eval_xc_eff(xc_code, rho_tot[i][0], deriv=1, xctype=xctype)[:2]
         else:
             exc, vxc = ni.eval_xc_eff(xc_code, rho_tot[i], deriv=1, xctype=xctype)[:2]
         vxc = cupy.asarray(vxc, order='C')
@@ -526,15 +516,15 @@
             wv[i][0] *= .5
         if xctype == 'MGGA':
             wv[i][[0,4]] *= .5
     t0 = log.timer_debug1('eval vxc', *t0)
 
     t1 = t0
     p0 = p1 = 0
-    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+    for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         p1 = p0 + weight.size
         for i in range(nset):
             if xctype == 'LDA':
                 if USE_SPARSITY == 2:
                     aow = _scale_ao(ao_mask, wv[i][0,p0:p1])
                     add_sparse(vmat[i], ao_mask.dot(aow.T), idx)
                 else:
@@ -669,22 +659,23 @@
     return rho_group
 
 def nr_rks_group(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
            max_memory=2000, verbose=None):
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_coeff = getattr(dms, 'mo_coeff', None)
     mo_occ = getattr(dms,'mo_occ', None)
 
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dm_shape = dms.shape
     #dms = [coeff @ dm @ coeff.T for dm in dms.reshape(-1,nao0,nao0)]
     dms = dms.reshape(-1,nao0,nao0)
     dms = take_last2d(dms, opt.ao_idx)
@@ -711,22 +702,22 @@
     else:
         if with_lapl:
             rho_tot = cupy.empty([nset,6,ngrids])
         else:
             rho_tot = cupy.empty([nset,5,ngrids])
     p0 = p1 = 0
     t1 = t0 = log.init_timer()
-    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+    for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         p1 = p0 + weight.size
         for i in range(nset):
             if mo_coeff is None:
-                rho_tot[i,:,p0:p1] = eval_rho(mol, ao_mask, dms[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
+                rho_tot[i,:,p0:p1] = eval_rho(_sorted_mol, ao_mask, dms[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
             else:
                 mo_coeff_mask = mo_coeff[idx,:]
-                rho_tot[i,:,p0:p1] = eval_rho2(mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
+                rho_tot[i,:,p0:p1] = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
         p0 = p1
         t1 = log.timer_debug2('eval rho slice', *t1)
     t0 = log.timer_debug1('eval rho', *t0)
 
     wv = []
     for i in range(nset):
         if xctype == 'LDA':
@@ -743,15 +734,15 @@
             wv[i][0] *= .5
         if xctype == 'MGGA':
             wv[i][[0,4]] *= .5
     t0 = log.timer_debug1('eval vxc', *t0)
 
     t1 = t0
     p0 = p1 = 0
-    for ao_mask_group, idx_group, weight_group, _ in ni.grouped_block_loop(mol, grids, nao, ao_deriv):
+    for ao_mask_group, idx_group, weight_group, _ in ni.grouped_block_loop(_sorted_mol, grids, nao, ao_deriv):
         p0_raw = p0
         for i in range(nset):
             p0 = p0_raw
             if xctype == 'LDA':
                 aow_group = []
                 for weight, ao_mask in zip(weight_group, ao_mask_group):
                     p1 = p0 + weight.size
@@ -816,22 +807,22 @@
     return nelec, excsum, vmat
 
 def nr_uks(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
            max_memory=2000, verbose=None):
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_coeff = getattr(dms, 'mo_coeff', None)
     mo_occ = getattr(dms,'mo_occ', None)
-
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dma, dmb = dms
     dm_shape = dma.shape
     dma = cupy.asarray(dma).reshape(-1,nao0,nao0)
     dmb = cupy.asarray(dmb).reshape(-1,nao0,nao0)
     dma = [coeff @ dm @ coeff.T for dm in dma]
@@ -849,24 +840,24 @@
     release_gpu_stack()
     if xctype == 'LDA':
         ao_deriv = 0
     else:
         ao_deriv = 1
     with_lapl = MGGA_DENSITY_LAPL
 
-    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+    for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         for i in range(nset):
             t0 = log.init_timer()
             if mo_coeff is None:
-                rho_a = eval_rho(mol, ao_mask, dma[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
-                rho_b = eval_rho(mol, ao_mask, dmb[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
+                rho_a = eval_rho(_sorted_mol, ao_mask, dma[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
+                rho_b = eval_rho(_sorted_mol, ao_mask, dmb[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
             else:
                 mo_coeff_mask = mo_coeff[:, idx,:]
-                rho_a = eval_rho2(mol, ao_mask, mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl)
-                rho_b = eval_rho2(mol, ao_mask, mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl)
+                rho_a = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl)
+                rho_b = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl)
 
             rho = cupy.stack([rho_a, rho_b], axis=0)
             exc, vxc = ni.eval_xc_eff(xc_code, rho, deriv=1, xctype=xctype)[:2]
             t1 = log.timer_debug1('eval vxc', *t0)
             if xctype == 'LDA':
                 den_a = rho_a * weight
                 den_b = rho_b * weight
@@ -926,40 +917,41 @@
         vmatb = vmatb[0]
     vmat = cupy.asarray([vmata, vmatb])
     return nelec, excsum, vmat
 
 
 def get_rho(ni, mol, dm, grids, max_memory=2000, verbose=None):
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
-    mol = opt.mol
-    log = logger.new_logger(mol, verbose)
+    mol = None
+    _sorted_mol = opt._sorted_mol
+    log = logger.new_logger(ni, verbose)
     coeff = cupy.asarray(opt.coeff)
     nao = coeff.shape[0]
     mo_coeff = getattr(dm, 'mo_coeff', None)
     mo_occ = getattr(dm,'mo_occ', None)
 
     dm = coeff @ cupy.asarray(dm) @ coeff.T
     if mo_coeff is not None:
         mo_coeff = coeff @ mo_coeff
     with_lapl = MGGA_DENSITY_LAPL
 
     ngrids = grids.weights.size
     rho = cupy.empty(ngrids)
     p0 = p1 = 0
     t1 = t0 = log.init_timer()
-    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, 0):
+    for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, 0):
         p1 = p0 + weight.size
         if mo_coeff is None:
-            rho[p0:p1] = eval_rho(mol, ao_mask, dm[np.ix_(idx,idx)], xctype='LDA', hermi=1, with_lapl=with_lapl)
+            rho[p0:p1] = eval_rho(_sorted_mol, ao_mask, dm[np.ix_(idx,idx)], xctype='LDA', hermi=1, with_lapl=with_lapl)
         else:
             mo_coeff_mask = mo_coeff[idx,:]
-            rho[p0:p1] = eval_rho2(mol, ao_mask, mo_coeff_mask, mo_occ, None, 'LDA', with_lapl)
+            rho[p0:p1] = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask, mo_occ, None, 'LDA', with_lapl)
         p0 = p1
         t1 = log.timer_debug2('eval rho slice', *t1)
     t0 = log.timer_debug1('eval rho', *t0)
 
     if FREE_CUPY_CACHE:
         dm = None
         cupy.get_default_memory_pool().free_all_blocks()
@@ -968,17 +960,19 @@
 def nr_rks_fxc(ni, mol, grids, xc_code, dm0=None, dms=None, relativity=0, hermi=0,
                rho0=None, vxc=None, fxc=None, max_memory=2000, verbose=None):
     if fxc is None:
         raise RuntimeError('fxc was not initialized')
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+
+    _sorted_mol = opt.mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dm_shape = dms.shape
     # AO basis -> gdftopt AO basis
     with_mocc = hasattr(dms, 'mo1')
     if with_mocc:
@@ -992,33 +986,33 @@
         ao_deriv = 0
     else:
         ao_deriv = 1
     with_lapl = MGGA_DENSITY_LAPL
     p0 = 0
     p1 = 0
     t1 = t0 = log.init_timer()
-    for ao, mask, weights, coords in ni.block_loop(opt.mol, grids, nao, ao_deriv):
+    for ao, mask, weights, coords in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         p0, p1 = p1, p1+len(weights)
         # precompute molecular orbitals
         if with_mocc:
             occ_coeff_mask = occ_coeff[mask]
             if xctype == 'LDA':
-                c0 = _dot_ao_dm(mol, ao, occ_coeff_mask, None, None, None)
+                c0 = _dot_ao_dm(_sorted_mol, ao, occ_coeff_mask, None, None, None)
             elif xctype == "GGA":
                 c0 = contract('nig,io->nog', ao, occ_coeff_mask)
             else: # mgga
                 c0 = contract('nig,io->nog', ao, occ_coeff_mask)
         t1 = log.timer_debug2(f'eval occ_coeff, with mocc: {with_mocc}', *t1)
         if with_mocc:
-            rho1 = eval_rho4(opt.mol, ao, c0, mo1[:,mask], xctype=xctype, with_lapl=False)
+            rho1 = eval_rho4(_sorted_mol, ao, c0, mo1[:,mask], xctype=xctype, with_lapl=False)
         else:
             # slow version
             rho1 = []
             for i in range(nset):
-                rho_tmp = eval_rho(opt.mol, ao, dms[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
+                rho_tmp = eval_rho(_sorted_mol, ao, dms[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
                 rho1.append(rho_tmp)
             rho1 = cupy.stack(rho1, axis=0)
         t1 = log.timer_debug2('eval rho', *t1)
 
         # precompute fxc_w
         if xctype == 'LDA':
             fxc_w = fxc[0,0,p0:p1] * weights
@@ -1078,18 +1072,19 @@
 def nr_uks_fxc(ni, mol, grids, xc_code, dm0=None, dms=None, relativity=0, hermi=0,
                rho0=None, vxc=None, fxc=None, max_memory=2000, verbose=None):
     if fxc is None:
         raise RuntimeError('fxc was not initialized')
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
-
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dma, dmb = dms
     dm_shape = dma.shape
     # AO basis -> gdftopt AO basis
     with_mocc = hasattr(dms, 'mo1')
     if with_mocc:
@@ -1114,42 +1109,42 @@
     if xctype == 'LDA':
         ao_deriv = 0
     else:
         ao_deriv = 1
     with_lapl = MGGA_DENSITY_LAPL
     p0 = 0
     p1 = 0
-    for ao, mask, weights, coords in ni.block_loop(opt.mol, grids, nao, ao_deriv):
+    for ao, mask, weights, coords in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         t0 = log.init_timer()
         p0, p1 = p1, p1+len(weights)
         # precompute molecular orbitals
         if with_mocc:
             occ_coeff_a_mask = occ_coeff_a[mask]
             occ_coeff_b_mask = occ_coeff_b[mask]
             if xctype == 'LDA':
-                c0_a = _dot_ao_dm(mol, ao, occ_coeff_a_mask, None, None, None)
-                c0_b = _dot_ao_dm(mol, ao, occ_coeff_b_mask, None, None, None)
+                c0_a = _dot_ao_dm(_sorted_mol, ao, occ_coeff_a_mask, None, None, None)
+                c0_b = _dot_ao_dm(_sorted_mol, ao, occ_coeff_b_mask, None, None, None)
             elif xctype == "GGA":
                 c0_a = contract('nig,io->nog', ao, occ_coeff_a_mask)
                 c0_b = contract('nig,io->nog', ao, occ_coeff_b_mask)
             else: # mgga
                 c0_a = contract('nig,io->nog', ao, occ_coeff_a_mask)
                 c0_b = contract('nig,io->nog', ao, occ_coeff_b_mask)
 
         if with_mocc:
-            rho1a = eval_rho4(opt.mol, ao, c0_a, mo1a[:,mask], xctype=xctype, with_lapl=with_lapl)
-            rho1b = eval_rho4(opt.mol, ao, c0_b, mo1b[:,mask], xctype=xctype, with_lapl=with_lapl)
+            rho1a = eval_rho4(_sorted_mol, ao, c0_a, mo1a[:,mask], xctype=xctype, with_lapl=with_lapl)
+            rho1b = eval_rho4(_sorted_mol, ao, c0_b, mo1b[:,mask], xctype=xctype, with_lapl=with_lapl)
         else:
             # slow version
             rho1a = []
             rho1b = []
             for i in range(nset):
-                rho_tmp = eval_rho(opt.mol, ao, dma[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
+                rho_tmp = eval_rho(_sorted_mol, ao, dma[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
                 rho1a.append(rho_tmp)
-                rho_tmp = eval_rho(opt.mol, ao, dmb[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
+                rho_tmp = eval_rho(_sorted_mol, ao, dmb[i][np.ix_(mask,mask)], xctype=xctype, hermi=hermi, with_lapl=with_lapl)
                 rho1b.append(rho_tmp)
             rho1a = cupy.stack(rho1a, axis=0)
             rho1b = cupy.stack(rho1b, axis=0)
         rho1 = cupy.stack([rho1a, rho1b], axis=0)
         t0 = log.timer_debug1('rho', *t0)
 
         # precompute fxc_w
@@ -1231,40 +1226,41 @@
         nelec is the number of electrons generated by numerical integration.
         excsum is the XC functional value.  vmat is the XC potential matrix in
         2D array of shape (nao,nao) where nao is the number of AO functions.
     '''
     log = logger.new_logger(mol, verbose)
     t0 = log.init_timer()
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_coeff = getattr(dms, 'mo_coeff', None)
     mo_occ = getattr(dms,'mo_occ', None)
 
     nao, nao0 = opt.coeff.shape
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     dms = [coeff @ dm @ coeff.T for dm in dms.reshape(-1,nao0,nao0)]
     assert len(dms) == 1
 
     if mo_coeff is not None:
         mo_coeff = coeff @ mo_coeff
     with_lapl = MGGA_DENSITY_LAPL
     ao_deriv = 1
     vvrho = []
     for ao, idx, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory=max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory=max_memory):
         #rho = eval_rho(opt.mol, ao, dms[0][np.ix_(mask,mask)], xctype='GGA', hermi=1)
         if mo_coeff is None:
-            rho = eval_rho(mol, ao, dms[0][np.ix_(idx,idx)], xctype='GGA', hermi=1, with_lapl=with_lapl)
+            rho = eval_rho(_sorted_mol, ao, dms[0][np.ix_(idx,idx)], xctype='GGA', hermi=1, with_lapl=with_lapl)
         else:
             mo_coeff_mask = mo_coeff[idx,:]
-            rho = eval_rho2(mol, ao, mo_coeff_mask, mo_occ, None, 'GGA', with_lapl)
+            rho = eval_rho2(_sorted_mol, ao, mo_coeff_mask, mo_occ, None, 'GGA', with_lapl)
         vvrho.append(rho)
 
     rho = cupy.hstack(vvrho)
     t1 = log.timer_debug1('eval rho', *t0)
     exc = 0
     vxc = 0
     nlc_coefs = ni.nlc_coeff(xc_code)
@@ -1280,27 +1276,24 @@
     excsum = cupy.dot(den, exc)
     vv_vxc = xc_deriv.transform_vxc(rho, vxc, 'GGA', spin=0)
     t1 = log.timer_debug1('transform vxc', *t1)
 
     vmat = cupy.zeros((nao,nao))
     p1 = 0
     for ao, mask, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory=max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory=max_memory):
         p0, p1 = p1, p1 + weight.size
         wv = vv_vxc[:,p0:p1] * weight
         wv[0] *= .5
         aow = _scale_ao(ao, wv)
         add_sparse(vmat, ao[0].dot(aow.T), mask)
     t1 = log.timer_debug1('integration', *t1)
 
     transpose_sum(vmat)
     vmat = take_last2d(vmat, opt.rev_ao_idx)
-    #vmat = vmat + vmat.T
-    #vmat = contract('pi,pq->iq', coeff, vmat)
-    #vmat = contract('qj,iq->ij', coeff, vmat)
     log.timer_debug1('eval vv10', *t0)
     return nelec, excsum, vmat
 
 def cache_xc_kernel(ni, mol, grids, xc_code, mo_coeff, mo_occ, spin=0,
                     max_memory=2000):
     log = logger.new_logger(mol, mol.verbose)
     xctype = ni._xc_type(xc_code)
@@ -1310,41 +1303,42 @@
         ao_deriv = 1
     elif xctype == 'NLC':
         raise NotImplementedError('NLC')
     else:
         ao_deriv = 0
     with_lapl = MGGA_DENSITY_LAPL
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao = coeff.shape[0]
     if spin == 0:
         mo_coeff = coeff @ mo_coeff
         rho = []
         t1 = t0 = log.init_timer()
-        for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
             mo_coeff_mask = mo_coeff[idx,:]
-            rho_slice = eval_rho2(mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
+            rho_slice = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
             rho.append(rho_slice)
             t1 = log.timer_debug2('eval rho slice', *t1)
         rho = cupy.hstack(rho)
         t0 = log.timer_debug1('eval rho in fxc', *t0)
     else:
         mo_coeff = contract('ip,npj->nij', coeff, cupy.asarray(mo_coeff))
         rhoa = []
         rhob = []
         t1 = t0 = log.init_timer()
-        for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
             mo_coeff_mask = mo_coeff[:,idx,:]
-            rhoa_slice = eval_rho2(mol, ao_mask, mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl)
-            rhob_slice = eval_rho2(mol, ao_mask, mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl)
+            rhoa_slice = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl)
+            rhob_slice = eval_rho2(_sorted_mol, ao_mask, mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl)
             rhoa.append(rhoa_slice)
             rhob.append(rhob_slice)
             t1 = log.timer_debug2('eval rho in fxc', *t1)
         #rho = (cupy.hstack(rhoa), cupy.hstack(rhob))
         rho = cupy.stack([cupy.hstack(rhoa), cupy.hstack(rhob)], axis=0)
         t0 = log.timer_debug1('eval rho in fxc', *t0)
     vxc, fxc = ni.eval_xc_eff(xc_code, rho, deriv=2, xctype=xctype)[1:3]
@@ -1522,45 +1516,46 @@
     '''
     if grids.coords is None:
         grids.build(with_non0tab=False, sort_grids=True)
     if nao is None:
         nao = mol.nao
     ngrids = grids.coords.shape[0]
     comp = (deriv+1)*(deriv+2)*(deriv+3)//6
-    log = logger.new_logger(mol, mol.verbose)
-
+    log = logger.new_logger(ni, ni.verbose)
+    
     if blksize is None:
         #cupy.get_default_memory_pool().free_all_blocks()
         mem_avail = get_avail_mem()
         blksize = int((mem_avail*.2/8/((comp+1)*nao + extra))/ ALIGNED) * ALIGNED
         blksize = min(blksize, MIN_BLK_SIZE)
         log.debug1('Available GPU mem %f Mb, block_size %d', mem_avail/1e6, blksize)
         if blksize < ALIGNED:
             raise RuntimeError('Not enough GPU memory')
 
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     with opt.gdft_envs_cache():
         block_id = 0
         t1 = log.init_timer()
         for ip0, ip1 in lib.prange(0, ngrids, blksize):
             coords = grids.coords[ip0:ip1]
             weight = grids.weights[ip0:ip1]
             t1 = log.init_timer()
             # cache ao indices
             if (block_id, blksize, ngrids) not in ni.non0ao_idx:
-                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(mol, coords, opt.l_ctr_offsets)
+                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(_sorted_mol, coords, opt.l_ctr_offsets)
 
             pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice = ni.non0ao_idx[block_id, blksize, ngrids]
             ao_mask = eval_ao(
-                ni, mol, coords, deriv,
+                ni, _sorted_mol, coords, deriv,
                 nao_slice=len(idx),
                 shls_slice=non0shl_idx,
                 ao_loc_slice=ao_loc_slice,
                 ctr_offsets_slice=ctr_offsets_slice)
 
             t1 = log.timer_debug2('evaluate ao slice', *t1)
             if pad > 0:
@@ -1592,40 +1587,41 @@
         blksize = int((mem_avail*.2/8/((comp+1)*nao + extra))/ ALIGNED) * ALIGNED
         blksize = min(blksize, MIN_BLK_SIZE)
         log.debug1('Available GPU mem %f Mb, block_size %d', mem_avail/1e6, blksize)
         if blksize < ALIGNED:
             raise RuntimeError('Not enough GPU memory')
 
     opt = getattr(ni, 'gdftopt', None)
-    if opt is None:
+    if opt is None or mol not in [opt.mol, opt._sorted_mol]:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     ao_mask_group = []
     idx_group = []
     weight_group = []
     coords_group = []
     total_used_bytes = 0
     mem_limit = get_avail_mem()
 
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     with opt.gdft_envs_cache():
         block_id = 0
         t1 = log.init_timer()
         for ip0, ip1 in lib.prange(0, ngrids, blksize):
             coords = grids.coords[ip0:ip1]
             weight = grids.weights[ip0:ip1]
             # cache ao indices
             if (block_id, blksize, ngrids) not in ni.non0ao_idx:
-                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(mol, coords, opt.l_ctr_offsets)
+                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(_sorted_mol, coords, opt.l_ctr_offsets)
 
             pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice = ni.non0ao_idx[block_id, blksize, ngrids]
 
             ao_mask = eval_ao(
-                ni, mol, coords, deriv,
+                ni, _sorted_mol, coords, deriv,
                 nao_slice=len(idx),
                 shls_slice=non0shl_idx,
                 ao_loc_slice=ao_loc_slice,
                 ctr_offsets_slice=ctr_offsets_slice)
 
             if pad > 0:
                 if deriv == 0:
@@ -1932,21 +1928,22 @@
     mat += bra[2].dot(_scale_ao(ket[2], wv).T)
     mat += bra[3].dot(_scale_ao(ket[3], wv).T)
     return mat
 
 class _GDFTOpt:
     def __init__(self, mol):
         self.envs_cache = ctypes.POINTER(_GDFTEnvsCache)()
-        self._mol = mol
+        self._sorted_mol = None       # sorted mol object based on contraction pattern
+        self.mol = mol
 
     def build(self, mol=None):
         if mol is None:
-            mol = self._mol
+            mol = self.mol
         else:
-            self._mol = mol
+            self.mol = mol
         if hasattr(mol, '_decontracted') and mol._decontracted:
             raise RuntimeError('mol object is already decontracted')
 
         pmol, coeff = basis_seg_contraction(mol, allow_replica=True)
         pmol.cart = mol.cart
         coeff = cupy.eye(mol.nao)      # without cart2sph transformation
         # Sort basis according to angular momentum and contraction patterns so
@@ -1995,15 +1992,15 @@
         ao_idx = np.hstack([ao_idx[i] for i in sorted_idx])
         assert pmol.nbas % BAS_ALIGNED == 0
         # Padding zeros to transformation coefficients
         if nao > coeff.shape[0]:
             paddings = nao - coeff.shape[0]
             coeff = np.vstack([coeff, np.zeros((paddings, coeff.shape[1]))])
         pmol._decontracted = True
-        self.mol = pmol
+        self._sorted_mol = pmol
         inv_idx = np.argsort(ao_idx, kind='stable').astype(np.int32)
         self.ao_idx = cupy.asarray(ao_idx, dtype=np.int32)
         self.rev_ao_idx = cupy.asarray(inv_idx, dtype=np.int32)
         self.coeff = coeff[ao_idx]
         self.l_ctr_offsets = np.append(0, np.cumsum(l_ctr_counts)).astype(np.int32)
         self.l_bas_offsets = np.append(0, np.cumsum(l_counts)).astype(np.int32)
         logger.debug2(mol, 'l_ctr_offsets = %s', self.l_ctr_offsets)
@@ -2012,22 +2009,22 @@
 
     @classmethod
     def from_mol(cls, mol):
         return cls(mol).build()
 
     @contextlib.contextmanager
     def gdft_envs_cache(self):
-        mol = self.mol
+        _sorted_mol = self._sorted_mol
         #ao_loc = mol.ao_loc_nr(cart=True)
-        ao_loc = mol.ao_loc_nr()
+        ao_loc = _sorted_mol.ao_loc_nr()
         libgdft.GDFTinit_envs(
             ctypes.byref(self.envs_cache), ao_loc.ctypes.data_as(ctypes.c_void_p),
-            mol._atm.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(mol.natm),
-            mol._bas.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(mol.nbas),
-            mol._env.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(mol._env.size))
+            _sorted_mol._atm.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(_sorted_mol.natm),
+            _sorted_mol._bas.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(_sorted_mol.nbas),
+            _sorted_mol._env.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(_sorted_mol._env.size))
         try:
             yield
         finally:
             libgdft.GDFTdel_envs(ctypes.byref(self.envs_cache))
 
 class _GDFTEnvsCache(ctypes.Structure):
     pass
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/radi.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/radi.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 import numpy
 import cupy
 import pyscf
 from pyscf.data import radii
 from pyscf.data.elements import charge as elements_proton
 
-BRAGG_RADII = cupy.asarray(radii.BRAGG)
+BRAGG_RADII = radii.BRAGG
 COVALENT_RADII = radii.COVALENT
-SG1RADII = cupy.asarray(pyscf.dft.radi.SG1RADII)
+SG1RADII = pyscf.dft.radi.SG1RADII
 
 gauss_chebyshev = pyscf.dft.radi.gauss_chebyshev
 treutler = pyscf.dft.radi.treutler
 
 def treutler_atomic_radii_adjust(mol, atomic_radii):
     '''Treutler atomic radii adjust function: [JCP 102, 346 (1995); DOI:10.1063/1.469408]'''
 # JCP 102, 346 (1995)
@@ -54,13 +54,14 @@
 
 def get_treutler_fac(mol, atomic_radii):
     '''
     # fac(i,j) = \frac{1}{4} ( \frac{ra(j)}{ra(i)} - \frac{ra(i)}{ra(j)}
     # fac(j,i) = -fac(i,j)
     '''
     charges = [elements_proton(x) for x in mol.elements]
-    rad = cupy.sqrt(atomic_radii[charges]) + 1e-200
+    atomic_radii = cupy.asarray(atomic_radii[charges])
+    rad = cupy.sqrt(atomic_radii) + 1e-200
     rr = rad.reshape(-1,1) * (1./rad)
     a = .25 * (rr.T - rr)
     a[a<-.5] = -.5
     a[a>0.5] = 0.5
     return a
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/rks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/rks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/roks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/roks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/uks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/uks.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,14 +124,22 @@
     get_veff = get_veff
     get_vasp = uks.get_vsap
     energy_elec = energy_elec
     energy_tot = hf.RHF.energy_tot
     init_guess_by_vsap = uks.UKS.init_guess_by_vsap
 
     to_hf = NotImplemented
+
+    def reset(self, mol=None):
+        super().reset(mol)
+        self.grids.reset(mol)
+        self.nlcgrids.reset(mol)
+        self._numint.gdftopt = None
+        return self
+
     def nuc_grad_method(self):
         from gpu4pyscf.grad import uks as uks_grad
         return uks_grad.Gradients(self)
 
     def to_cpu(self):
         from gpu4pyscf.lib import utils
         mf = uks.UKS(self.mol, xc=self.xc)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_alias.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/xc_alias.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_deriv.py` & `gpu4pyscf-0.7.8/gpu4pyscf/dft/xc_deriv.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/fci/direct_spin1.py` & `gpu4pyscf-0.7.8/gpu4pyscf/fci/direct_spin1.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/grad/dispersion.py` & `gpu4pyscf-0.7.8/gpu4pyscf/grad/dispersion.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/grad/rhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/grad/rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,14 @@
         h1mo = contract('xij,jo->xio', h1ao, orbo)
         dh1e[:,atm_id] += contract('xio,ip->xpo', h1mo, mo_coeff)
     return dh1e
 
 def as_scanner(mf_grad):
     if isinstance(mf_grad, lib.GradScanner):
         return mf_grad
-
     logger.info(mf_grad, 'Create scanner for %s', mf_grad.__class__)
     name = mf_grad.__class__.__name__ + SCF_GradScanner.__name_mixin__
     return lib.set_class(SCF_GradScanner(mf_grad),
                          (SCF_GradScanner, mf_grad.__class__), name)
 
 class SCF_GradScanner(lib.GradScanner):
     def __init__(self, g):
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/grad/rks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/grad/rks.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 MIN_BLK_SIZE = getattr(__config__, 'min_grid_blksize', 128*128)
 ALIGNED = getattr(__config__, 'grid_aligned', 16*16)
 
 libgdft = load_library('libgdft')
 libgdft.GDFT_make_dR_dao_w.restype = ctypes.c_int
 
-def _get_veff(ks_grad, mol=None, dm=None):
+def get_veff(ks_grad, mol=None, dm=None):
     '''
     First order derivative of DFT effective potential matrix (wrt electron coordinates)
 
     Args:
-        ks_grad : grad.uhf.Gradients or grad.uks.Gradients object
+        ks_grad : grad.rhf.Gradients or grad.rks.Gradients object
     '''
     if mol is None: mol = ks_grad.mol
     if dm is None: dm = ks_grad.base.make_rdm1()
     t0 = (logger.process_clock(), logger.perf_counter())
 
     mf = ks_grad.base
     ni = mf._numint
@@ -115,63 +115,57 @@
 def get_vxc(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
             max_memory=2000, verbose=None):
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    _sorted_mol = opt._sorted_mol
     mo_occ = cupy.asarray(dms.mo_occ)
     mo_coeff = cupy.asarray(dms.mo_coeff)
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms).reshape(-1,nao0,nao0)
     dms = take_last2d(dms, opt.ao_idx)
-    #dms = [cupy.einsum('pi,ij,qj->pq', coeff, dm, coeff)
-    #       for dm in dms.reshape(-1,nao0,nao0)]
-    #mo_coeff = coeff @ mo_coeff
     mo_coeff = mo_coeff[opt.ao_idx]
 
     nset = len(dms)
     assert nset == 1
-    if xctype == 'LDA':
-        ao_deriv = 1
-    else:
-        ao_deriv = 2
     vmat = cupy.zeros((nset,3,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 1
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             for idm in range(nset):
                 mo_coeff_mask = mo_coeff[idx,:]
-                rho = numint.eval_rho2(opt.mol, ao_mask[0], mo_coeff_mask, mo_occ, None, xctype)
+                rho = numint.eval_rho2(_sorted_mol, ao_mask[0], mo_coeff_mask, mo_occ, None, xctype)
                 vxc = ni.eval_xc_eff(xc_code, rho, 1, xctype=xctype)[1]
                 wv = weight * vxc[0]
                 aow = numint._scale_ao(ao_mask[0], wv)
                 vtmp = _d1_dot_(ao_mask[1:4], aow.T)
                 add_sparse(vmat[idm], vtmp, idx)
     elif xctype == 'GGA':
         ao_deriv = 2
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             for idm in range(nset):
                 mo_coeff_mask = mo_coeff[idx,:]
-                rho = numint.eval_rho2(opt.mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype)
+                rho = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype)
                 vxc = ni.eval_xc_eff(xc_code, rho, 1, xctype=xctype)[1]
                 wv = weight * vxc
                 wv[0] *= .5
                 vtmp = _gga_grad_sum_(ao_mask, wv)
                 add_sparse(vmat[idm], vtmp, idx)
     elif xctype == 'NLC':
         raise NotImplementedError('NLC')
 
     elif xctype == 'MGGA':
         ao_deriv = 2
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             for idm in range(nset):
                 mo_coeff_mask = mo_coeff[idx,:]
-                rho = numint.eval_rho2(opt.mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype, with_lapl=False)
+                rho = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype, with_lapl=False)
                 vxc = ni.eval_xc_eff(xc_code, rho, 1, xctype=xctype)[1]
                 wv = weight * vxc
                 wv[0] *= .5
                 wv[4] *= .5  # for the factor 1/2 in tau
                 vtmp = _gga_grad_sum_(ao_mask, wv)
                 vtmp += _tau_grad_dot_(ao_mask, wv[4])
                 add_sparse(vmat[idm], vtmp, idx)
@@ -190,16 +184,17 @@
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_occ = cupy.asarray(dms.mo_occ)
     mo_coeff = cupy.asarray(dms.mo_coeff)
-
-    mol = opt.mol
+    
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dms = [coeff @ dm @ coeff.T
            for dm in dms.reshape(-1,nao0,nao0)]
     mo_coeff = coeff @ mo_coeff
     nset = len(dms)
@@ -209,28 +204,28 @@
     if len(nlc_coefs) != 1:
         raise NotImplementedError('Additive NLC')
     nlc_pars, fac = nlc_coefs[0]
 
     ao_deriv = 2
     vvrho = []
     for ao_mask, mask, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory=max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory=max_memory):
         mo_coeff_mask = mo_coeff[mask]
-        rho = numint.eval_rho2(mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype, with_lapl=False)
+        rho = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask, mo_occ, None, xctype, with_lapl=False)
         vvrho.append(rho)
     rho = cupy.hstack(vvrho)
 
     vxc = numint._vv10nlc(rho, grids.coords, rho, grids.weights,
                           grids.coords, nlc_pars)[1]
     vv_vxc = xc_deriv.transform_vxc(rho, vxc, 'GGA', spin=0)
 
     vmat = cupy.zeros((3,nao,nao))
     p1 = 0
     for ao_mask, mask, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
         p0, p1 = p1, p1 + weight.size
         wv = vv_vxc[:,p0:p1] * weight
         wv[0] *= .5  # *.5 because vmat + vmat.T at the end
         vmat_tmp = _gga_grad_sum_(ao_mask, wv)
         add_sparse(vmat, vmat_tmp, mask)
 
     #vmat = contract('npq,qj->npj', vmat, coeff)
@@ -319,22 +314,21 @@
     '''Full response including the response of the grids'''
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dms = [cupy.einsum('pi,ij,qj->pq', coeff, dm, coeff)
            for dm in dms.reshape(-1,nao0,nao0)]
-    #nset = len(dms)
-    #make_rho, nset, nao = ni._gen_rho_evaluator(mol, dms.get(), hermi, False, grids)
-    #ao_loc = mol.ao_loc_nr()
 
     excsum = 0
     vmat = cupy.zeros((3,nao,nao))
     with opt.gdft_envs_cache():
         if xctype == 'LDA':
             ao_deriv = 1
         else:
@@ -348,16 +342,16 @@
 
         if block_size < ALIGNED:
             raise RuntimeError('Not enough GPU memory')
 
         for atm_id, (coords, weight, weight1) in enumerate(grids_response_cc(grids)):
             ngrids = weight.size
             for p0, p1 in lib.prange(0,ngrids,block_size):
-                ao = numint.eval_ao(ni, opt.mol, coords[p0:p1, :], ao_deriv)
-                rho = numint.eval_rho(opt.mol, ao, dms[0],
+                ao = numint.eval_ao(ni, _sorted_mol, coords[p0:p1, :], ao_deriv)
+                rho = numint.eval_rho(_sorted_mol, ao, dms[0],
                                       xctype=xctype, hermi=1, with_lapl=False)
                 vxc = ni.eval_xc_eff(xc_code, rho, 1, xctype=xctype)[1]
 
                 if xctype == 'LDA':
                     wv = weight[p0:p1] * vxc[0]
                     aow = numint._scale_ao(ao[0], wv)
                     vmat += _d1_dot_(ao[1:4], aow.T)
@@ -511,15 +505,15 @@
 
     # method
     def __init__ (self, mf):
         rhf_grad.Gradients.__init__(self, mf)
         self.grids = None
         self.nlcgrids = None
 
-    get_veff = _get_veff
+    get_veff = get_veff
     # TODO: add grid response into this function
     def extra_force(self, atom_id, envs):
         return 0
 
 Grad = Gradients
 from gpu4pyscf import dft
 dft.rks.RKS.Gradients = lib.class_as_method(Gradients)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/grad/uhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/grad/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,14 @@
         return vj.get() if vj is not None else None, \
             vk.get() if vk is not None else None
 
 def get_veff(mf_grad, mol, dm):
     vk0 = mf_grad.get_jk(mol, dm[0])[1]
     vk1 = mf_grad.get_jk(mol, dm[1])[1]
     vj0 = mf_grad.get_jk(mol, dm[0]+dm[1])[0]
-
     return vj0 - vk0 - vk1
 
 
 def make_rdm1e(mo_energy, mo_coeff, mo_occ):
     '''Energy weighted density matrix'''
     return cupy.asarray((rhf_grad_cpu.make_rdm1e(mo_energy[0], mo_coeff[0], mo_occ[0]),
                           rhf_grad_cpu.make_rdm1e(mo_energy[1], mo_coeff[1], mo_occ[1])))
@@ -298,36 +297,25 @@
 
         log.timer_debug1("get_dh1e", *t3)
         if mol.has_ecp():
             dh1e += rhf_grad.get_dh1e_ecp(mol, dm0_sf)
         t1 = log.timer_debug1('gradients of h1e', *t0)
         log.debug('Computing Gradients of NR-HF Coulomb repulsion')
         dvhf = mf_grad.get_veff(mol, dm0)
-
+        
         extra_force = cupy.zeros((len(atmlst),3))
         for k, ia in enumerate(atmlst):
             extra_force[k] += mf_grad.extra_force(ia, locals())
         log.timer_debug1('gradients of 2e part', *t1)
 
     dh = contract('xij,ij->xi', h1, dm0_sf)
     ds = contract('xij,ij->xi', s1, dme0_sf)
     delec = 2.0*(dh - ds)
     delec = cupy.asarray([cupy.sum(delec[:, p0:p1], axis=1) for p0, p1 in aoslices[:,2:]])
 
-
-    '''
-    print('dvhf')
-    print(dvhf)
-    print('dh1e')
-    print(dh1e)
-    print('delec')
-    print(delec)
-    print('extra')
-    print(extra_force)
-    '''
     de = 2.0 * dvhf + dh1e + delec + extra_force
 
     # for backward compatiability
     if(hasattr(mf, 'disp') and mf.disp is not None):
         g_disp = mf_grad.get_dispersion()
         mf_grad.grad_disp = g_disp
         mf_grad.grad_mf = de
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/grad/uks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/grad/uks.py`

 * *Files 23% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     Args:
         ks_grad : grad.uhf.Gradients or grad.uks.Gradients object
     '''
     if mol is None: mol = ks_grad.mol
     if dm is None: dm = ks_grad.base.make_rdm1()
     t0 = (logger.process_clock(), logger.perf_counter())
-
     mf = ks_grad.base
     ni = mf._numint
     if ks_grad.grids is not None:
         grids = ks_grad.grids
     else:
         grids = mf.grids
 
@@ -65,15 +64,14 @@
         if ks_grad.nlcgrids is not None:
             nlcgrids = ks_grad.nlcgrids
         else:
             nlcgrids = mf.nlcgrids
         if nlcgrids.coords is None:
             nlcgrids.build(sort_grids=True)
 
-    ni = mf._numint
     mem_now = lib.current_memory()[0]
     max_memory = max(2000, ks_grad.max_memory*.9-mem_now)
     if ks_grad.grid_response:
         exc, vxc_tmp = get_vxc_full_response(ni, mol, grids, mf.xc, dm,
                                          max_memory=max_memory,
                                          verbose=ks_grad.verbose)
         if mf.nlc or ni.libxc.is_nlc(mf.xc):
@@ -128,62 +126,64 @@
 def get_vxc(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
             max_memory=2000, verbose=None):
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    mol = None
+    _sorted_mol = opt._sorted_mol
     mo_occ = cupy.asarray(dms.mo_occ)
     mo_coeff = cupy.asarray(dms.mo_coeff)
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dms = take_last2d(dms, opt.ao_idx)
     mo_coeff = mo_coeff[:, opt.ao_idx]
 
     nset = len(dms)
     vmat = cupy.zeros((nset,3,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 1
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,idx,:]
-            rho_a = numint.eval_rho2(opt.mol, ao_mask[0], mo_coeff_mask[0], mo_occ[0], None, xctype)
-            rho_b = numint.eval_rho2(opt.mol, ao_mask[0], mo_coeff_mask[1], mo_occ[1], None, xctype)
+            rho_a = numint.eval_rho2(_sorted_mol, ao_mask[0], mo_coeff_mask[0], mo_occ[0], None, xctype)
+            rho_b = numint.eval_rho2(_sorted_mol, ao_mask[0], mo_coeff_mask[1], mo_occ[1], None, xctype)
 
             vxc = ni.eval_xc_eff(xc_code, cupy.array([rho_a,rho_b]), 1, xctype=xctype)[1]
             wv = weight * vxc[:,0]
             aow = numint._scale_ao(ao_mask[0], wv[0])
             vtmp = rks_grad._d1_dot_(ao_mask[1:4], aow.T)
             add_sparse(vmat[0], vtmp, idx)
             aow = numint._scale_ao(ao_mask[0], wv[1])
             vtmp = rks_grad._d1_dot_(ao_mask[1:4], aow.T)
             add_sparse(vmat[1], vtmp, idx)
     elif xctype == 'GGA':
         ao_deriv = 2
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,idx,:]
-            rho_a = numint.eval_rho2(opt.mol, ao_mask[:4], mo_coeff_mask[0], mo_occ[0], None, xctype)
-            rho_b = numint.eval_rho2(opt.mol, ao_mask[:4], mo_coeff_mask[1], mo_occ[1], None, xctype)
+            rho_a = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask[0], mo_occ[0], None, xctype)
+            rho_b = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask[1], mo_occ[1], None, xctype)
 
             vxc = ni.eval_xc_eff(xc_code, cupy.array([rho_a,rho_b]), 1, xctype=xctype)[1]
             wv = weight * vxc
             wv[:,0] *= .5
             vtmp = rks_grad._gga_grad_sum_(ao_mask, wv[0])
             add_sparse(vmat[0], vtmp, idx)
             vtmp = rks_grad._gga_grad_sum_(ao_mask, wv[1])
             add_sparse(vmat[1], vtmp, idx)
     elif xctype == 'NLC':
         raise NotImplementedError('NLC')
 
     elif xctype == 'MGGA':
         ao_deriv = 2
-        for ao_mask, idx, weight, _ in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+        for ao_mask, idx, weight, _ in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,idx,:]
-            rho_a = numint.eval_rho2(opt.mol, ao_mask[:10], mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl=False)
-            rho_b = numint.eval_rho2(opt.mol, ao_mask[:10], mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl=False)
+            rho_a = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask[0], mo_occ[0], None, xctype, with_lapl=False)
+            rho_b = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask[1], mo_occ[1], None, xctype, with_lapl=False)
             vxc = ni.eval_xc_eff(xc_code, cupy.array([rho_a,rho_b]), 1, xctype=xctype)[1]
             wv = weight * vxc
             wv[:,0] *= .5
             wv[:,4] *= .5  # for the factor 1/2 in tau
             vtmp = rks_grad._gga_grad_sum_(ao_mask, wv[0])
             vtmp += rks_grad._tau_grad_dot_(ao_mask, wv[0,4])
             add_sparse(vmat[0], vtmp, idx)
@@ -191,28 +191,30 @@
             vtmp += rks_grad._tau_grad_dot_(ao_mask, wv[1,4])
             add_sparse(vmat[1], vtmp, idx)
 
     vmat = take_last2d(vmat, opt.rev_ao_idx)
     exc = None
     if nset == 1:
         vmat = vmat[0]
-
+        
     # - sign because nabla_X = -nabla_x
     return exc, -cupy.array(vmat)
 
 
 def get_vxc_full_response(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
                           max_memory=2000, verbose=None):
     '''Full response including the response of the grids'''
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms)
     dms = [cupy.einsum('pi,ij,qj->pq', coeff, dm, coeff)
            for dm in dms.reshape(-1,nao0,nao0)]
 
     excsum = 0
@@ -231,25 +233,25 @@
 
         if block_size < ALIGNED:
             raise RuntimeError('Not enough GPU memory')
 
         for atm_id, (coords, weight, weight1) in enumerate(rks_grad.grids_response_cc(grids)):
             ngrids = weight.size
             for p0, p1 in lib.prange(0,ngrids,block_size):
-                ao = numint.eval_ao(ni, opt.mol, coords[p0:p1, :], ao_deriv)
+                ao = numint.eval_ao(ni, _sorted_mol, coords[p0:p1, :], ao_deriv)
                 if xctype == 'LDA':
-                    rho_a = numint.eval_rho(opt.mol, ao, dms[0],
+                    rho_a = numint.eval_rho(_sorted_mol, ao, dms[0],
                                         xctype='GGA', hermi=1, with_lapl=False)
-                    rho_b = numint.eval_rho(opt.mol, ao, dms[1],
+                    rho_b = numint.eval_rho(_sorted_mol, ao, dms[1],
                                         xctype='GGA', hermi=1, with_lapl=False)
                     vxc = ni.eval_xc_eff(xc_code, cupy.array([rho_a[0],rho_b[0]]), 1, xctype=xctype)[1]
                 else:
-                    rho_a = numint.eval_rho(opt.mol, ao, dms[0],
+                    rho_a = numint.eval_rho(_sorted_mol, ao, dms[0],
                                         xctype=xctype, hermi=1, with_lapl=False)
-                    rho_b = numint.eval_rho(opt.mol, ao, dms[1],
+                    rho_b = numint.eval_rho(_sorted_mol, ao, dms[1],
                                         xctype=xctype, hermi=1, with_lapl=False)
                     vxc = ni.eval_xc_eff(xc_code, cupy.array([rho_a,rho_b]), 1, xctype=xctype)[1]
 
                 if xctype == 'LDA':
                     wv = weight[p0:p1] * vxc[:,0]
                     aow = numint._scale_ao(ao[0], wv[0])
                     vtmp = rks_grad._d1_dot_(ao[1:4], aow.T)
@@ -295,15 +297,16 @@
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
 
     mo_occ = cupy.asarray(mo_occ)
     mo_coeff = cupy.asarray(mo_coeff)
 
-    mol = opt.mol
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     mo_coeff_0 = coeff @ mo_coeff[0]
     mo_coeff_1 = coeff @ mo_coeff[1]
     nset = 1
     assert nset == 1
 
@@ -311,30 +314,30 @@
     if len(nlc_coefs) != 1:
         raise NotImplementedError('Additive NLC')
     nlc_pars, fac = nlc_coefs[0]
 
     ao_deriv = 2
     vvrho = []
     for ao_mask, mask, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory=max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory=max_memory):
         mo_coeff_mask_0 = mo_coeff_0[mask]
         mo_coeff_mask_1 = mo_coeff_1[mask]
-        rhoa = numint.eval_rho2(mol, ao_mask[:4], mo_coeff_mask_0, mo_occ[0], None, xctype, with_lapl=False)
-        rhob = numint.eval_rho2(mol, ao_mask[:4], mo_coeff_mask_1, mo_occ[1], None, xctype, with_lapl=False)
+        rhoa = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask_0, mo_occ[0], None, xctype, with_lapl=False)
+        rhob = numint.eval_rho2(_sorted_mol, ao_mask[:4], mo_coeff_mask_1, mo_occ[1], None, xctype, with_lapl=False)
         vvrho.append(rhoa + rhob)
     rho = cupy.hstack(vvrho)
 
     vxc = numint._vv10nlc(rho, grids.coords, rho, grids.weights,
                           grids.coords, nlc_pars)[1]
     vv_vxc = xc_deriv.transform_vxc(rho, vxc, 'GGA', spin=0)
 
     vmat = cupy.zeros((3,nao,nao))
     p1 = 0
     for ao_mask, mask, weight, coords \
-            in ni.block_loop(mol, grids, nao, ao_deriv, max_memory):
+            in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
         p0, p1 = p1, p1 + weight.size
         wv = vv_vxc[:,p0:p1] * weight
         wv[0] *= .5  # *.5 because vmat + vmat.T at the end
         vmat_tmp = rks_grad._gga_grad_sum_(ao_mask, wv)
         add_sparse(vmat, vmat_tmp, mask)
 
     rev_ao_idx = opt.rev_ao_idx
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/gto/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/gto/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/gto/mole.py` & `gpu4pyscf-0.7.8/gpu4pyscf/gto/mole.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 from pyscf import gto
 
 @functools.lru_cache(20)
 def get_cart2sph(lmax=12):
     cart2sph = []
     for l in range(lmax):
         c2s = gto.mole.cart2sph(l, normalized='sp')
-        cart2sph.append(cupy.asarray(c2s, order='C'))
+        cart2sph.append(np.asarray(c2s, order='C'))
     return cart2sph
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/dispersion.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/dispersion.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/rhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pyscf.scf import _vhf
 
 # import _response_functions to load gen_response methods in SCF class
 from gpu4pyscf.scf import _response_functions  # noqa
 # import pyscf.grad.rhf to activate nuc_grad_method method
 from pyscf.grad import rhf  # noqa
 from gpu4pyscf.scf import cphf
-from gpu4pyscf.lib.cupy_helper import contract, tag_array, print_mem_info
+from gpu4pyscf.lib.cupy_helper import contract, tag_array, print_mem_info, transpose_sum
 from gpu4pyscf.lib import logger
 from gpu4pyscf.df import int3c2e
 
 def hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
               mo1=None, mo_e1=None, h1ao=None,
               atmlst=None, max_memory=4000, verbose=None):
     log = logger.new_logger(hessobj, verbose)
@@ -303,15 +303,16 @@
                 for i in range(comp):
                     lib.hermi_triu(vs[k][i], hermi=hermi, inplace=True)
             else:
                 lib.hermi_triu(vs[k], hermi=hermi, inplace=True)
     return vs
 
 def solve_mo1(mf, mo_energy, mo_coeff, mo_occ, h1mo,
-              fx=None, atmlst=None, max_memory=4000, verbose=None):
+              fx=None, atmlst=None, max_memory=4000, verbose=None,
+              max_cycle=50, level_shift=0):
     '''Solve the first order equation
     Kwargs:
         fx : function(dm_mo) => v1_mo
             A function to generate the induced potential.
             See also the function gen_vind.
     '''
     mol = mf.mol
@@ -327,15 +328,15 @@
     s1a = cupy.asarray(s1a)
 
     def _ao2mo(mat):
         tmp = contract('xij,jo->xio', mat, mocc)
         return contract('xik,ip->xpk', tmp, mo_coeff)
     cupy.get_default_memory_pool().free_all_blocks()
     # TODO: calculate blksize dynamically
-    blksize = 8
+    blksize = 48
     mo1s = [None] * mol.natm
     e1s = [None] * mol.natm
     aoslices = mol.aoslice_by_atom()
     for ia0, ia1 in lib.prange(0, len(atmlst), blksize):
         s1vo = []
         h1vo = []
         for i0 in range(ia0, ia1):
@@ -345,15 +346,15 @@
             s1ao[:,p0:p1] += s1a[:,p0:p1]
             s1ao[:,:,p0:p1] += s1a[:,p0:p1].transpose(0,2,1)
             s1vo.append(_ao2mo(s1ao))
             h1vo.append(h1mo[ia])
 
         h1vo = cupy.vstack(h1vo)
         s1vo = cupy.vstack(s1vo)
-        tol = mf.conv_tol_cpscf * (ia1 - ia0)
+        tol = mf.conv_tol_cpscf
         mo1, e1 = cphf.solve(fx, mo_energy, mo_occ, h1vo, s1vo, tol=tol, verbose=verbose)
         # Different from PySCF, mo1 is in AO
         mo1 = mo1.reshape(-1,3,nao,nocc)
         e1 = e1.reshape(-1,3,nocc,nocc)
 
         for k in range(ia1-ia0):
             ia = atmlst[k+ia0]
@@ -615,15 +616,16 @@
     def get_hcore(self, mol=None):
         if mol is None: mol = self.mol
         return get_hcore(mol)
 
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
-                         fx, atmlst, max_memory, verbose)
+                         fx, atmlst, max_memory, verbose,
+                         max_cycle=self.max_cycle, level_shift=self.level_shift)
 
     def hess_nuc(self, mol=None, atmlst=None):
         if mol is None: mol = self.mol
         return hess_nuc(mol, atmlst)
 
     def to_cpu(self):
         mf = self.base.to_cpu()
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/rks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/rks.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,26 +201,26 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
-
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     mo_coeff = coeff @ mo_coeff
     nao = mo_coeff.shape[0]
-    # TODO: check mol in opt?
+    
     vmat = cupy.zeros((6,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 2
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[mask,:]
-            rho = numint.eval_rho2(opt.mol, ao[0], mo_coeff_mask, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff_mask, mo_occ, mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, rho, 1, xctype=xctype)[1]
             wv = weight * vxc[0]
             aow = numint._scale_ao(ao[0], wv)
             for i in range(6):
                 vmat_tmp = numint._dot_ao_ao(mol, ao[i+4], aow, mask, shls_slice, ao_loc)
                 add_sparse(vmat[i], vmat_tmp, mask)
             aow = None
@@ -230,17 +230,17 @@
             aow = numint._scale_ao(ao[aoidx[0]], wv[1])
             aow+= numint._scale_ao(ao[aoidx[1]], wv[2])
             aow+= numint._scale_ao(ao[aoidx[2]], wv[3])
             return numint._dot_ao_ao(mol, aow, ao[0], mask, shls_slice, ao_loc)
 
         ao_deriv = 3
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[mask,:]
-            rho = numint.eval_rho2(opt.mol, ao[:4], mo_coeff_mask, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff_mask, mo_occ, mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, rho, 1, xctype=xctype)[1]
             wv = weight * vxc
             #:aow = numpy.einsum('npi,np->pi', ao[:4], wv[:4])
             aow = numint._scale_ao(ao[:4], wv[:4])
 
             vmat_tmp = [0]*6
             for i in range(6):
@@ -260,17 +260,17 @@
             aow = numint._scale_ao(ao[aoidx[0]], wv[1])
             aow+= numint._scale_ao(ao[aoidx[1]], wv[2])
             aow+= numint._scale_ao(ao[aoidx[2]], wv[3])
             return numint._dot_ao_ao(mol, aow, ao[0], mask, shls_slice, ao_loc)
 
         ao_deriv = 3
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[mask,:]
-            rho = numint.eval_rho2(opt.mol, ao[:10], mo_coeff_mask, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff_mask, mo_occ, mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, rho, 1, xctype=xctype)[1]
             wv = weight * vxc
             wv[4] *= .5  # for the factor 1/2 in tau
             #:aow = numpy.einsum('npi,np->pi', ao[:4], wv[:4])
             vmat_tmp = [0]*6
             aow = numint._scale_ao(ao[:4], wv[:4])
             for i in range(6):
@@ -345,15 +345,15 @@
     rho1[:,2] += numint._contract_rho1(ao[1:4,p0:p1], ao_dm0[2][p0:p1])
     rho1[:,3] += numint._contract_rho1(ao[1:4,p0:p1], ao_dm0[3][p0:p1])
 
     # *2 for |mu> DM <d_X nu|
     return rho1 * 2
 
 def _d1d2_dot_(vmat, mol, ao1, ao2, mask, ao_loc, dR1_on_bra=True):
-    shls_slice = (0, mol.nbas)
+    shls_slice = None
     if dR1_on_bra:  # (d/dR1 bra) * (d/dR2 ket)
         for d1 in range(3):
             for d2 in range(3):
                 vmat[d1,d2] += numint._dot_ao_ao(mol, ao1[d1], ao2[d2], mask,
                                                  shls_slice, ao_loc)
         #vmat += contract('xig,yjg->xyij', ao1, ao2)
     else:  # (d/dR2 bra) * (d/dR1 ket)
@@ -385,103 +385,104 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     dm0 = mf.make_rdm1(mo_coeff, mo_occ)
     dm0_sorted = take_last2d(dm0, opt.ao_idx)
-    vmat_dm = cupy.zeros((mol.natm,3,3,nao))
+    vmat_dm = cupy.zeros((_sorted_mol.natm,3,3,nao))
     ipip = cupy.zeros((3,3,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 1
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rho = numint.eval_rho2(opt.mol, ao[0], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc[0]
             aow = [numint._scale_ao(ao[i], wv) for i in range(1, 4)]
             _d1d2_dot_(ipip, mol, aow, ao[1:4], mask, ao_loc, False)
             dm0_mask = dm0_sorted[numpy.ix_(mask, mask)]
 
             ao_dm_mask = contract('nig,ij->njg', ao_mask[:4], dm0_mask)
             ao_dm0 = numint._dot_ao_dm(mol, ao[0], dm0, mask, shls_slice, ao_loc)
             wf = weight * fxc[0,0]
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 p0, p1 = aoslices[ia][2:]
                 # *2 for \nabla|ket> in rho1
                 rho1 = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0[p0:p1,:]) * 2
                 # aow ~ rho1 ~ d/dR1
                 wv = wf * rho1
                 aow = cupy.empty_like(ao_dm_mask[1:4])
                 for i in range(3):
                     aow[i] = numint._scale_ao(ao_dm_mask[0], wv[i])
                 vmat_dm[ia][:,:,mask] += contract('yjg,xjg->xyj', ao_mask[1:4], aow)
             ao_dm0 = aow = None
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             vmat_dm[ia] = vmat_dm[ia][:,:,opt.rev_ao_idx]
             p0, p1 = aoslices[ia][2:]
             vmat_dm[ia] += contract('xypq,pq->xyp', ipip[:,:,:,p0:p1], dm0[:,p0:p1])
     elif xctype == 'GGA':
         ao_deriv = 2
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rho = numint.eval_rho2(opt.mol, ao[:4], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[0] *= .5
             aow = rks_grad._make_dR_dao_w(ao, wv)
             _d1d2_dot_(ipip, mol, aow, ao[1:4], mask, ao_loc, False)
             ao_dm0 = [numint._dot_ao_dm(mol, ao[i], dm0, mask, shls_slice, ao_loc) for i in range(4)]
             wf = weight * fxc
             dm0_mask = dm0_sorted[numpy.ix_(mask, mask)]
             ao_dm_mask = contract('nig,ij->njg', ao_mask[:4], dm0_mask)
             vmat_dm_tmp = cupy.empty([3,3,nao_non0])
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1 = _make_dR_rho1(ao, ao_dm0, ia, aoslices, xctype)
                 wv = contract('xyg,sxg->syg', wf, dR_rho1)
                 wv[:,0] *= .5
                 for i in range(3):
                     aow = rks_grad._make_dR_dao_w(ao_mask, wv[i])
                     vmat_dm_tmp[i] = contract('xjg,jg->xj', aow, ao_dm_mask[0])
                 for i in range(3):
                     aow[i] = numint._scale_ao(ao_dm_mask[:4], wv[i,:4])
                 vmat_dm_tmp += contract('yjg,xjg->xyj', ao_mask[1:4], aow)
                 vmat_dm[ia][:,:,mask] += vmat_dm_tmp
             ao_dm0 = aow = None
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             vmat_dm[ia] = vmat_dm[ia][:,:,opt.rev_ao_idx]
             p0, p1 = aoslices[ia][2:]
             vmat_dm[ia] += contract('xypq,pq->xyp', ipip[:,:,:,p0:p1], dm0[:,p0:p1])
             vmat_dm[ia] += contract('yxqp,pq->xyp', ipip[:,:,p0:p1], dm0[:,p0:p1])
     elif xctype == 'MGGA':
         XX, XY, XZ = 4, 5, 6
         YX, YY, YZ = 5, 7, 8
         ZX, ZY, ZZ = 6, 8, 9
         ao_deriv = 2
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rho = numint.eval_rho2(opt.mol, ao[:10], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[0] *= .5
             wv[4] *= .25
             aow = rks_grad._make_dR_dao_w(ao, wv)
@@ -491,15 +492,15 @@
             _d1d2_dot_(ipip, mol, [aow[0], aow[1], aow[2]], [ao[XX], ao[XY], ao[XZ]], mask, ao_loc, False)
             _d1d2_dot_(ipip, mol, [aow[1], aow[3], aow[4]], [ao[YX], ao[YY], ao[YZ]], mask, ao_loc, False)
             _d1d2_dot_(ipip, mol, [aow[2], aow[4], aow[5]], [ao[ZX], ao[ZY], ao[ZZ]], mask, ao_loc, False)
             dm0_mask = dm0_sorted[numpy.ix_(mask, mask)]
             ao_dm0 = [numint._dot_ao_dm(mol, ao[i], dm0, mask, shls_slice, ao_loc) for i in range(4)]
             ao_dm_mask = contract('nig,ij->njg', ao_mask[:4], dm0_mask)
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1 = _make_dR_rho1(ao, ao_dm0, ia, aoslices, xctype)
                 wv = contract('xyg,sxg->syg', wf, dR_rho1)
                 wv[:,0] *= .5
                 wv[:,4] *= .5  # for the factor 1/2 in tau
                 vmat_dm_tmp = cupy.empty([3,3,nao_non0])
                 for i in range(3):
                     aow = rks_grad._make_dR_dao_w(ao_mask, wv[i])
@@ -525,15 +526,15 @@
                     aow[i] = numint._scale_ao(ao_dm_mask[3], wv[i,4])
                 vmat_dm_tmp[:,0] += contract('jg,xjg->xj', ao_mask[ZX], aow)
                 vmat_dm_tmp[:,1] += contract('jg,xjg->xj', ao_mask[ZY], aow)
                 vmat_dm_tmp[:,2] += contract('jg,xjg->xj', ao_mask[ZZ], aow)
 
                 vmat_dm[ia][:,:,mask] += vmat_dm_tmp
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             vmat_dm[ia] = vmat_dm[ia][:,:,opt.rev_ao_idx]
             p0, p1 = aoslices[ia][2:]
             vmat_dm[ia] += contract('xypq,pq->xyp', ipip[:,:,:,p0:p1], dm0[:,p0:p1])
             vmat_dm[ia] += contract('yxqp,pq->xyp', ipip[:,:,p0:p1], dm0[:,p0:p1])
     return vmat_dm
 
 def _get_vxc_deriv1(hessobj, mo_coeff, mo_occ, max_memory):
@@ -561,66 +562,67 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
-
+    mol = None
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     dm0 = mf.make_rdm1(mo_coeff, mo_occ)
 
     v_ip = cupy.zeros((3,nao,nao))
-    vmat = cupy.zeros((mol.natm,3,nao,nocc))
+    vmat = cupy.zeros((_sorted_mol.natm,3,nao,nocc))
     max_memory = max(2000, max_memory-vmat.size*8/1e6)
     if xctype == 'LDA':
         ao_deriv = 1
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rho = numint.eval_rho2(opt.mol, ao[0], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc[0]
             aow = numint._scale_ao(ao[0], wv)
             v_ip += rks_grad._d1_dot_(ao[1:4], aow.T)
             mo = contract('xig,ip->xpg', ao, mocc)
             ao_dm0 = numint._dot_ao_dm(mol, ao[0], dm0, mask, shls_slice, ao_loc)
             wf = weight * fxc[0,0]
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 p0, p1 = aoslices[ia][2:]
 # First order density = rho1 * 2.  *2 is not applied because + c.c. in the end
                 rho1 = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0[p0:p1,:])
                 wv = wf * rho1
                 aow = [numint._scale_ao(ao[0], wv[i]) for i in range(3)]
                 mow = [numint._scale_ao(mo[0], wv[i]) for i in range(3)]
                 vmat[ia] += rks_grad._d1_dot_(aow, mo[0].T)
                 vmat[ia] += rks_grad._d1_dot_(mow, ao[0].T).transpose([0,2,1])
             ao_dm0 = aow = None
             t1 = log.timer_debug2('integration', *t1)
     elif xctype == 'GGA':
         ao_deriv = 2
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rho = numint.eval_rho2(mol, ao[:4], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[0] *= .5
             v_ip += rks_grad._gga_grad_sum_(ao, wv)
             mo = contract('xig,ip->xpg', ao, mocc)
             ao_dm0 = [numint._dot_ao_dm(mol, ao[i], dm0, mask, shls_slice, ao_loc)
                       for i in range(4)]
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1 = _make_dR_rho1(ao, ao_dm0, ia, aoslices, xctype)
                 wv = contract('xyg,sxg->syg', wf, dR_rho1)
                 wv[:,0] *= .5
                 aow = [numint._scale_ao(ao[:4], wv[i,:4]) for i in range(3)]
                 mow = [numint._scale_ao(mo[:4], wv[i,:4]) for i in range(3)]
                 vmat[ia] += rks_grad._d1_dot_(aow, mo[0].T)
                 vmat[ia] += rks_grad._d1_dot_(mow, ao[0].T).transpose([0,2,1])
@@ -628,29 +630,29 @@
             ao_dm0 = aow = None
     elif xctype == 'MGGA':
         if grids.level < 5:
             log.warn('MGGA Hessian is sensitive to dft grids.')
         ao_deriv = 2
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rho = numint.eval_rho2(opt.mol, ao[:10], mo_coeff, mo_occ, mask, xctype)
+            rho = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff, mo_occ, mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t0)
             wv = weight * vxc
             wv[0] *= .5
             wv[4] *= .5  # for the factor 1/2 in tau
             v_ip += rks_grad._gga_grad_sum_(ao, wv)
             v_ip += rks_grad._tau_grad_dot_(ao, wv[4])
             mo = contract('xig,ip->xpg', ao, mocc)
             ao_dm0 = [numint._dot_ao_dm(mol, ao[i], dm0, mask, shls_slice, ao_loc) for i in range(4)]
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1 = _make_dR_rho1(ao, ao_dm0, ia, aoslices, xctype)
                 wv = contract('xyg,sxg->syg', wf, dR_rho1)
                 wv[:,0] *= .5
                 wv[:,4] *= .25
                 aow = [numint._scale_ao(ao[:4], wv[i,:4]) for i in range(3)]
                 mow = [numint._scale_ao(mo[:4], wv[i,:4]) for i in range(3)]
                 vmat[ia] += rks_grad._d1_dot_(aow, mo[0].T)
@@ -661,15 +663,15 @@
                     vmat[ia] += rks_grad._d1_dot_(aow, mo[j].T)
                     vmat[ia] += rks_grad._d1_dot_(mow, ao[j].T).transpose([0,2,1])
             ao_dm0 = aow = None
             t1 = log.timer_debug2('integration', *t1)
 
     vmat = -contract("kxiq,ip->kxpq", vmat, mo_coeff)
 
-    for ia in range(mol.natm):
+    for ia in range(_sorted_mol.natm):
         p0, p1 = aoslices[ia][2:]
         vmat_tmp = cupy.zeros([3,nao,nao])
         vmat_tmp[:,p0:p1] += v_ip[:,p0:p1]
         vmat_tmp[:,:,p0:p1] += v_ip[:,p0:p1].transpose(0,2,1)
 
         vmat_tmp = contract('xij,jq->xiq', vmat_tmp, mocc)
         vmat_tmp = contract('xiq,ip->xpq', vmat_tmp, mo_coeff)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/uhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,16 @@
                 for i in range(comp):
                     lib.hermi_triu(vs[k][i], hermi=hermi, inplace=True)
             else:
                 lib.hermi_triu(vs[k], hermi=hermi, inplace=True)
     return vs
 
 def solve_mo1(mf, mo_energy, mo_coeff, mo_occ, h1mo,
-              fx=None, atmlst=None, max_memory=4000, verbose=None):
+              fx=None, atmlst=None, max_memory=4000, verbose=None,
+              max_cycle=50, level_shift=0):
     '''Solve the first order equation
     Kwargs:
         fx : function(dm_mo) => v1_mo
             A function to generate the induced potential.
             See also the function gen_vind.
     '''
     mol = mf.mol
@@ -517,14 +518,15 @@
     make_h1 = make_h1
     kernel = NotImplemented
     hess = NotImplemented
 
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
-                         fx, atmlst, max_memory, verbose)
+                         fx, atmlst, max_memory, verbose,
+                         max_cycle=self.max_cycle, level_shift=self.level_shift)
 
     gen_hop = gen_hop
 
 # Inject to UHF class
 from gpu4pyscf import scf
 scf.uhf.UHF.Hessian = lib.class_as_method(Hessian)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/hessian/uks.py` & `gpu4pyscf-0.7.8/gpu4pyscf/hessian/uks.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,28 +199,29 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    _sorted_mol = opt._sorted_mol
 
     coeff = cupy.asarray(opt.coeff)
     mo_coeff = contract('nij,pi->npj', mo_coeff, coeff)
     nao = mo_coeff.shape[1]
     # TODO: check mol in opt?
     vmata = cupy.zeros((6,nao,nao))
     vmatb = cupy.zeros((6,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 2
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,mask,:]
-            rhoa = numint.eval_rho2(opt.mol, ao[0], mo_coeff_mask[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[0], mo_coeff_mask[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff_mask[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff_mask[1], mo_occ[1], mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 1, xctype=xctype)[1]
             wv = weight * vxc[:,0]
             aowa = numint._scale_ao(ao[0], wv[0])
             aowb = numint._scale_ao(ao[0], wv[1])
             for i in range(6):
                 vmat_tmp = numint._dot_ao_ao(mol, ao[i+4], aowa, mask, shls_slice, ao_loc)
                 add_sparse(vmata[i], vmat_tmp, mask)
@@ -233,18 +234,18 @@
             aow = numint._scale_ao(ao[aoidx[0]], wv[1])
             aow+= numint._scale_ao(ao[aoidx[1]], wv[2])
             aow+= numint._scale_ao(ao[aoidx[2]], wv[3])
             return numint._dot_ao_ao(mol, aow, ao[0], mask, shls_slice, ao_loc)
 
         ao_deriv = 3
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,mask,:]
-            rhoa = numint.eval_rho2(opt.mol, ao[:4], mo_coeff_mask[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[:4], mo_coeff_mask[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff_mask[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff_mask[1], mo_occ[1], mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 1, xctype=xctype)[1]
             wv = weight * vxc
             #:aow = numpy.einsum('npi,np->pi', ao[:4], wv[:4])
             aowa = numint._scale_ao(ao[:4], wv[0,:4])
             aowb = numint._scale_ao(ao[:4], wv[1,:4])
             vmata_tmp = [0]*6
             vmatb_tmp = [0]*6
@@ -272,18 +273,18 @@
             aow = numint._scale_ao(ao[aoidx[0]], wv[1])
             aow+= numint._scale_ao(ao[aoidx[1]], wv[2])
             aow+= numint._scale_ao(ao[aoidx[2]], wv[3])
             return numint._dot_ao_ao(mol, aow, ao[0], mask, shls_slice, ao_loc)
 
         ao_deriv = 3
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             mo_coeff_mask = mo_coeff[:,mask,:]
-            rhoa = numint.eval_rho2(opt.mol, ao[:10], mo_coeff_mask[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[:10], mo_coeff_mask[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff_mask[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff_mask[1], mo_occ[1], mask, xctype)
             vxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 1, xctype=xctype)[1]
             wv = weight * vxc
             wv[:,4] *= .5  # for the factor 1/2 in tau
             #:aow = numpy.einsum('npi,np->pi', ao[:4], wv[:4])
             vmata_tmp = [0]*6
             vmatb_tmp = [0]*6
             aowa = numint._scale_ao(ao[:4], wv[0,:4])
@@ -412,31 +413,33 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    _sorted_mol = opt._sorted_mol
+
     coeff = cupy.asarray(opt.coeff)
     dm0a, dm0b = mf.make_rdm1(mo_coeff, mo_occ)
     dm0a_sorted = take_last2d(dm0a, opt.ao_idx)
     dm0b_sorted = take_last2d(dm0b, opt.ao_idx)
     vmata_dm = cupy.zeros((mol.natm,3,3,nao))
     vmatb_dm = cupy.zeros((mol.natm,3,3,nao))
     ipipa = cupy.zeros((3,3,nao,nao))
     ipipb = cupy.zeros((3,3,nao,nao))
     if xctype == 'LDA':
         ao_deriv = 1
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rhoa = numint.eval_rho2(opt.mol, ao[0], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[0], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc[:,0]
             aowa = [numint._scale_ao(ao[i], wv[0]) for i in range(1, 4)]
             _d1d2_dot_(ipipa, mol, aowa, ao[1:4], mask, ao_loc, False)
             aowb = [numint._scale_ao(ao[i], wv[1]) for i in range(1, 4)]
@@ -446,15 +449,15 @@
 
             ao_dma_mask = contract('nig,ij->njg', ao_mask[:4], dm0a_mask)
             ao_dmb_mask = contract('nig,ij->njg', ao_mask[:4], dm0b_mask)
 
             ao_dm0a = numint._dot_ao_dm(mol, ao[0], dm0a, mask, shls_slice, ao_loc)
             ao_dm0b = numint._dot_ao_dm(mol, ao[0], dm0b, mask, shls_slice, ao_loc)
             wf = weight * fxc[:,0,:,0]
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 p0, p1 = aoslices[ia][2:]
                 # *2 for \nabla|ket> in rho1
                 rho1a = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0a[p0:p1,:]) * 2
                 rho1b = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0b[p0:p1,:]) * 2
                 # aow ~ rho1 ~ d/dR1
                 wv = wf[0,:,None] * rho1a
                 wv+= wf[1,:,None] * rho1b
@@ -463,29 +466,29 @@
                     aow[i] = numint._scale_ao(ao_dma_mask[0], wv[0,i])
                 vmata_dm[ia][:,:,mask] += contract('yjg,xjg->xyj', ao_mask[1:4], aow)
                 for i in range(3):
                     aow[i] = numint._scale_ao(ao_dmb_mask[0], wv[1,i])
                 vmatb_dm[ia][:,:,mask] += contract('yjg,xjg->xyj', ao_mask[1:4], aow)
             ao_dm0a = ao_dm0b = aow = None
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             p0, p1 = aoslices[ia][2:]
             vmata_dm[ia] = vmata_dm[ia][:,:,opt.rev_ao_idx]
             vmatb_dm[ia] = vmatb_dm[ia][:,:,opt.rev_ao_idx]
             vmata_dm[ia] += contract('xypq,pq->xyp', ipipa[:,:,:,p0:p1], dm0a[:,p0:p1])
             vmatb_dm[ia] += contract('xypq,pq->xyp', ipipb[:,:,:,p0:p1], dm0b[:,p0:p1])
     elif xctype == 'GGA':
         ao_deriv = 2
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rhoa = numint.eval_rho2(opt.mol, ao[:4], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[:4], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[:,0] *= .5
             aow = rks_grad._make_dR_dao_w(ao, wv[0])
             _d1d2_dot_(ipipa, mol, aow, ao[1:4], mask, ao_loc, False)
@@ -496,15 +499,15 @@
             wf = weight * fxc
             dm0a_mask = dm0a_sorted[numpy.ix_(mask, mask)]
             dm0b_mask = dm0b_sorted[numpy.ix_(mask, mask)]
             ao_dma_mask = contract('nig,ij->njg', ao_mask[:4], dm0a_mask)
             ao_dmb_mask = contract('nig,ij->njg', ao_mask[:4], dm0b_mask)
             vmata_dm_tmp = cupy.empty([3,3,nao_non0])
             vmatb_dm_tmp = cupy.empty([3,3,nao_non0])
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1a = _make_dR_rho1(ao, ao_dm0a, ia, aoslices, xctype)
                 dR_rho1b = _make_dR_rho1(ao, ao_dm0b, ia, aoslices, xctype)
                 wv = contract('xbyg,sxg->bsyg', wf[0], dR_rho1a)
                 wv+= contract('xbyg,sxg->bsyg', wf[1], dR_rho1b)
                 wv[:,:,0] *= .5
                 wva, wvb = wv
                 for i in range(3):
@@ -520,34 +523,34 @@
                     vmatb_dm_tmp[i] = contract('xjg,jg->xj', aow, ao_dmb_mask[0])
                 for i in range(3):
                     aow[i] = numint._scale_ao(ao_dmb_mask[:4], wvb[i,:4])
                 vmatb_dm_tmp += contract('yjg,xjg->xyj', ao_mask[1:4], aow)
                 vmatb_dm[ia][:,:,mask] += vmatb_dm_tmp
             ao_dm0a = ao_dm0b = aow = None
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             vmata_dm[ia] = vmata_dm[ia][:,:,opt.rev_ao_idx]
             vmatb_dm[ia] = vmatb_dm[ia][:,:,opt.rev_ao_idx]
             p0, p1 = aoslices[ia][2:]
             vmata_dm[ia] += contract('xypq,pq->xyp', ipipa[:,:,:,p0:p1], dm0a[:,p0:p1])
             vmata_dm[ia] += contract('yxqp,pq->xyp', ipipa[:,:,p0:p1], dm0a[:,p0:p1])
             vmatb_dm[ia] += contract('xypq,pq->xyp', ipipb[:,:,:,p0:p1], dm0b[:,p0:p1])
             vmatb_dm[ia] += contract('yxqp,pq->xyp', ipipb[:,:,p0:p1], dm0b[:,p0:p1])
     elif xctype == 'MGGA':
         XX, XY, XZ = 4, 5, 6
         YX, YY, YZ = 5, 7, 8
         ZX, ZY, ZZ = 6, 8, 9
         ao_deriv = 2
         t1 = log.init_timer()
         for ao_mask, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             nao_non0 = len(mask)
             ao = contract('nip,ij->njp', ao_mask, coeff[mask])
-            rhoa = numint.eval_rho2(opt.mol, ao[:10], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[:10], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa, rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[:,0] *= .5
             wv[:,4] *= .25
             aow = rks_grad._make_dR_dao_w(ao, wv[0])
@@ -567,15 +570,15 @@
             dm0a_mask = dm0a_sorted[numpy.ix_(mask, mask)]
             dm0b_mask = dm0b_sorted[numpy.ix_(mask, mask)]
             ao_dm0a = [numint._dot_ao_dm(mol, ao[i], dm0a, mask, shls_slice, ao_loc) for i in range(4)]
             ao_dm0b = [numint._dot_ao_dm(mol, ao[i], dm0b, mask, shls_slice, ao_loc) for i in range(4)]
             ao_dma_mask = contract('nig,ij->njg', ao_mask[:4], dm0a_mask)
             ao_dmb_mask = contract('nig,ij->njg', ao_mask[:4], dm0b_mask)
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1a = _make_dR_rho1(ao, ao_dm0a, ia, aoslices, xctype)
                 dR_rho1b = _make_dR_rho1(ao, ao_dm0b, ia, aoslices, xctype)
                 wv = contract('xbyg,sxg->bsyg', wf[0], dR_rho1a)
                 wv+= contract('xbyg,sxg->bsyg', wf[1], dR_rho1b)
                 wv[:,:,0] *= .5
                 wv[:,:,4] *= .5  # for the factor 1/2 in tau
                 wva, wvb = wv
@@ -635,15 +638,15 @@
                 vmatb_dm_tmp[:,0] += contract('jg,xjg->xj', ao_mask[ZX], aow)
                 vmatb_dm_tmp[:,1] += contract('jg,xjg->xj', ao_mask[ZY], aow)
                 vmatb_dm_tmp[:,2] += contract('jg,xjg->xj', ao_mask[ZZ], aow)
 
                 vmata_dm[ia][:,:,mask] += vmata_dm_tmp
                 vmatb_dm[ia][:,:,mask] += vmatb_dm_tmp
             t1 = log.timer_debug2('integration', *t1)
-        for ia in range(mol.natm):
+        for ia in range(_sorted_mol.natm):
             vmata_dm[ia] = vmata_dm[ia][:,:,opt.rev_ao_idx]
             vmatb_dm[ia] = vmatb_dm[ia][:,:,opt.rev_ao_idx]
             p0, p1 = aoslices[ia][2:]
             vmata_dm[ia] += contract('xypq,pq->xyp', ipipa[:,:,:,p0:p1], dm0a[:,p0:p1])
             vmata_dm[ia] += contract('yxqp,pq->xyp', ipipa[:,:,p0:p1], dm0a[:,p0:p1])
             vmatb_dm[ia] += contract('xypq,pq->xyp', ipipb[:,:,:,p0:p1], dm0b[:,p0:p1])
             vmatb_dm[ia] += contract('yxqp,pq->xyp', ipipb[:,:,p0:p1], dm0b[:,p0:p1])
@@ -676,45 +679,45 @@
     shls_slice = (0, mol.nbas)
     ao_loc = mol.ao_loc_nr()
 
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
-
+    _sorted_mol = opt._sorted_mol
     coeff = cupy.asarray(opt.coeff)
     dm0a, dm0b = mf.make_rdm1(mo_coeff, mo_occ)
 
     vipa = cupy.zeros((3,nao,nao))
     vipb = cupy.zeros((3,nao,nao))
-    vmata = cupy.zeros((mol.natm,3,nao,nocca))
-    vmatb = cupy.zeros((mol.natm,3,nao,noccb))
+    vmata = cupy.zeros((_sorted_mol.natm,3,nao,nocca))
+    vmatb = cupy.zeros((_sorted_mol.natm,3,nao,noccb))
     max_memory = None
     if xctype == 'LDA':
         ao_deriv = 1
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rhoa = numint.eval_rho2(opt.mol, ao[0], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[0], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[0], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc[:,0]
             aow = numint._scale_ao(ao[0], wv[0])
             vipa += rks_grad._d1_dot_(ao[1:4], aow.T)
             aow = numint._scale_ao(ao[0], wv[1])
             vipb += rks_grad._d1_dot_(ao[1:4], aow.T)
             moa = contract('xig,ip->xpg', ao, mocca)
             mob = contract('xig,ip->xpg', ao, moccb)
             ao_dm0a = numint._dot_ao_dm(mol, ao[0], dm0a, mask, shls_slice, ao_loc)
             ao_dm0b = numint._dot_ao_dm(mol, ao[0], dm0b, mask, shls_slice, ao_loc)
             wf = weight * fxc[:,0,:,0]
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 p0, p1 = aoslices[ia][2:]
 # First order density = rho1 * 2.  *2 is not applied because + c.c. in the end
                 rho1a = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0a[p0:p1,:])
                 rho1b = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0b[p0:p1,:])
                 wv = wf[0,:,None] * rho1a
                 wv+= wf[1,:,None] * rho1b
                 aow = [numint._scale_ao(ao[0], wv[0,i]) for i in range(3)]
@@ -728,33 +731,33 @@
                 vmatb[ia] += rks_grad._d1_dot_(mow, ao[0].T).transpose([0,2,1])
             ao_dm0a = ao_dm0b = aow = None
             t1 = log.timer_debug2('integration', *t1)
     elif xctype == 'GGA':
         ao_deriv = 2
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rhoa = numint.eval_rho2(mol, ao[:4], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(mol, ao[:4], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:4], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc
             wv[:,0] *= .5
             vipa += rks_grad._gga_grad_sum_(ao, wv[0])
             vipb += rks_grad._gga_grad_sum_(ao, wv[1])
             moa = contract('xig,ip->xpg', ao, mocca)
             mob = contract('xig,ip->xpg', ao, moccb)
             ao_dm0a = [numint._dot_ao_dm(mol, ao[i], dm0a, mask, shls_slice, ao_loc)
                       for i in range(4)]
             ao_dm0b = [numint._dot_ao_dm(mol, ao[i], dm0b, mask, shls_slice, ao_loc)
                       for i in range(4)]
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1a = _make_dR_rho1(ao, ao_dm0a, ia, aoslices, xctype)
                 dR_rho1b = _make_dR_rho1(ao, ao_dm0b, ia, aoslices, xctype)
                 wv = contract('xbyg,sxg->bsyg', wf[0], dR_rho1a)
                 wv+= contract('xbyg,sxg->bsyg', wf[1], dR_rho1b)
                 wv[:,:,0] *= .5
                 wva,wvb = wv
                 aow = [numint._scale_ao(ao[:4], wva[i,:4]) for i in range(3)]
@@ -770,18 +773,18 @@
             ao_dm0a = ao_dm0b = aow = None
     elif xctype == 'MGGA':
         if grids.level < 5:
             log.warn('MGGA Hessian is sensitive to dft grids.')
         ao_deriv = 2
         t1 = t0 = log.init_timer()
         for ao, mask, weight, coords \
-                in ni.block_loop(opt.mol, grids, nao, ao_deriv, max_memory):
+                in ni.block_loop(_sorted_mol, grids, nao, ao_deriv, max_memory):
             ao = contract('nip,ij->njp', ao, coeff[mask])
-            rhoa = numint.eval_rho2(opt.mol, ao[:10], mo_coeff[0], mo_occ[0], mask, xctype)
-            rhob = numint.eval_rho2(opt.mol, ao[:10], mo_coeff[1], mo_occ[1], mask, xctype)
+            rhoa = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff[0], mo_occ[0], mask, xctype)
+            rhob = numint.eval_rho2(_sorted_mol, ao[:10], mo_coeff[1], mo_occ[1], mask, xctype)
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, cupy.asarray((rhoa,rhob)), 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t0)
             wv = weight * vxc
             wv[:,0] *= .5
             wv[:,4] *= .5  # for the factor 1/2 in tau
             vipa += rks_grad._gga_grad_sum_(ao, wv[0])
@@ -790,15 +793,15 @@
             vipb += rks_grad._tau_grad_dot_(ao, wv[1,4])
 
             moa = contract('xig,ip->xpg', ao, mocca)
             mob = contract('xig,ip->xpg', ao, moccb)
             ao_dm0a = [numint._dot_ao_dm(mol, ao[i], dm0a, mask, shls_slice, ao_loc) for i in range(4)]
             ao_dm0b = [numint._dot_ao_dm(mol, ao[i], dm0b, mask, shls_slice, ao_loc) for i in range(4)]
             wf = weight * fxc
-            for ia in range(mol.natm):
+            for ia in range(_sorted_mol.natm):
                 dR_rho1a = _make_dR_rho1(ao, ao_dm0a, ia, aoslices, xctype)
                 dR_rho1b = _make_dR_rho1(ao, ao_dm0b, ia, aoslices, xctype)
                 wv = contract('xbyg,sxg->bsyg', wf[0], dR_rho1a)
                 wv+= contract('xbyg,sxg->bsyg', wf[1], dR_rho1b)
                 wv[:,:,0] *= .5
                 wv[:,:,4] *= .25
                 wva,wvb = wv
@@ -823,15 +826,15 @@
                     vmatb[ia] += rks_grad._d1_dot_(mow, ao[j].T).transpose([0,2,1])
             ao_dm0a = ao_dm0b = aow = None
             t1 = log.timer_debug2('integration', *t1)
 
     vmata = -contract("kxiq,ip->kxpq", vmata, mo_coeff[0])
     vmatb = -contract("kxiq,ip->kxpq", vmatb, mo_coeff[1])
 
-    for ia in range(mol.natm):
+    for ia in range(_sorted_mol.natm):
         p0, p1 = aoslices[ia][2:]
         vmat_tmp = cupy.zeros([3,nao,nao])
         vmat_tmp[:,p0:p1] += vipa[:,p0:p1]
         vmat_tmp[:,:,p0:p1] += vipa[:,p0:p1].transpose(0,2,1)
 
         vmat_tmp = contract('xij,jq->xiq', vmat_tmp, mocca)
         vmat_tmp = contract('xiq,ip->xpq', vmat_tmp, mo_coeff[0])
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/cublas.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/cublas.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/cupy_helper.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/cupy_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,32 @@
 from pyscf import lib
 from gpu4pyscf.lib import logger
 from gpu4pyscf.gto import mole
 from gpu4pyscf.lib.cutensor import contract
 from gpu4pyscf.lib.cusolver import eigh, cholesky  #NOQA
 
 LMAX_ON_GPU = 7
-DSOLVE_LINDEP = 1e-15
+DSOLVE_LINDEP = 1e-13
 
 c2s_l = mole.get_cart2sph(lmax=LMAX_ON_GPU)
-c2s_data = cupy.concatenate([x.ravel() for x in c2s_l])
 c2s_offset = np.cumsum([0] + [x.shape[0]*x.shape[1] for x in c2s_l])
+_data = {'c2s': None}
 
 def load_library(libname):
     try:
         _loaderpath = os.path.dirname(__file__)
         return np.ctypeslib.load_library(libname, _loaderpath)
     except OSError:
         raise
 
 libcupy_helper = load_library('libcupy_helper')
 
 pinned_memory_pool = cupy.cuda.PinnedMemoryPool()
 cupy.cuda.set_pinned_memory_allocator(pinned_memory_pool.malloc)
+
 def pin_memory(array):
     mem = cupy.cuda.alloc_pinned_memory(array.nbytes)
     ret = np.frombuffer(mem, array.dtype, array.size).reshape(array.shape)
     ret[...] = array
     return ret
 
 def release_gpu_stack():
@@ -223,28 +224,32 @@
         raise RuntimeError('failed in calculating distance matrix')
     return out
 
 def block_c2s_diag(ncart, nsph, angular, counts):
     '''
     constract a cartesian to spherical transformation of n shells
     '''
+    if _data['c2s'] is None: 
+        c2s_data = cupy.concatenate([cupy.asarray(x.ravel()) for x in c2s_l])
+        _data['c2s'] = c2s_data
+    c2s_data = _data['c2s']
 
     nshells = np.sum(counts)
-    cart2sph = cupy.zeros([ncart, nsph])
-
     rows = [np.array([0], dtype='int32')]
     cols = [np.array([0], dtype='int32')]
     offsets = []
     for l, count in zip(angular, counts):
         r, c = c2s_l[l].shape
         rows.append(rows[-1][-1] + np.arange(1,count+1, dtype='int32') * r)
         cols.append(cols[-1][-1] + np.arange(1,count+1, dtype='int32') * c)
         offsets += [c2s_offset[l]] * count
     rows = cupy.hstack(rows)
     cols = cupy.hstack(cols)
+
+    cart2sph = cupy.zeros([ncart, nsph])
     offsets = cupy.asarray(offsets, dtype='int32')
 
     stream = cupy.cuda.get_current_stream()
     err = libcupy_helper.block_diag(
         ctypes.cast(stream.ptr, ctypes.c_void_p),
         ctypes.cast(cart2sph.data.ptr, ctypes.c_void_p),
         ctypes.c_int(ncart),
@@ -397,15 +402,15 @@
     '''
     transform 'axis' of a tensor from cartesian basis into spherical basis with cutensor
     '''
     if(ang <= 1):
         if(out is not None): out[:] = t
         return t
     size = list(t.shape)
-    c2s = c2s_l[ang]
+    c2s = cupy.asarray(c2s_l[ang])
     if(not t.flags['C_CONTIGUOUS']): t = cupy.asarray(t, order='C')
     li_size = c2s.shape
     nli = size[axis] // li_size[0]
     i0 = max(1, np.prod(size[:axis]))
     i3 = max(1, np.prod(size[axis+1:]))
     out_shape = size[:axis] + [nli*li_size[1]] + size[axis+1:]
 
@@ -528,59 +533,59 @@
         axt = aop(x1)
         if axt.ndim == 1:
             axt = axt.reshape(1,ndim)
         xs.extend(x1)
         ax.extend(axt)
         if callable(callback):
             callback(cycle, xs, ax)
-
         x1 = axt.copy()
+
         for i in range(len(xs)):
             xsi = cupy.asarray(xs[i])
-            for j, axj in enumerate(axt):
-                x1[j] -= xsi * (cupy.dot(xsi.conj(), axj) / innerprod[i])
+            w = cupy.dot(axt, xsi.conj()) / innerprod[i]
+            x1 -= xsi * cupy.expand_dims(w,-1)
         axt = xsi = None
 
+        x1, rmat = _qr(x1, cupy.dot, lindep)
+        for i in range(len(x1)):
+            x1[i] *= rmat[i,i]
+
         max_innerprod = 0
         idx = []
         for i, xi in enumerate(x1):
             innerprod1 = cupy.dot(xi.conj(), xi).real
             max_innerprod = max(max_innerprod, innerprod1)
             if innerprod1 > lindep and innerprod1 > tol**2:
                 idx.append(i)
                 innerprod.append(innerprod1)
-        log.debug('krylov cycle %d  r = %g', cycle, max_innerprod**.5)
-
+        log.info(f'krylov cycle {cycle}  r = {max_innerprod**.5:.3e} {x1.shape[0]} equations')
         if max_innerprod < lindep or max_innerprod < tol**2:
             break
-
         x1 = x1[idx]
 
+    if len(idx) > 0:
+        raise RuntimeError("CPSCF failed to converge.")
+
     xs = cupy.asarray(xs)
     ax = cupy.asarray(ax)
-    nd = cycle + 1
+    nd = xs.shape[0]
 
     h = cupy.dot(xs, ax.T)
 
     # Add the contribution of I in (1+a)
     h += cupy.diag(cupy.asarray(innerprod[:nd]))
     g = cupy.zeros((nd,nroots), dtype=x1.dtype)
 
     if b.ndim == 1:
         g[0] = innerprod[0]
     else:
-        ng = min(nd, nroots)
-        g[:ng, :nroots] += cupy.dot(xs[:ng], b[:nroots].T)
-        '''
         # Restore the first nroots vectors, which are array b or b-(1+a)x0
         for i in range(min(nd, nroots)):
             xsi = cupy.asarray(xs[i])
-            for j in range(nroots):
-                g[i,j] = cupy.dot(xsi.conj(), b[j])
-        '''
+            g[i] = cupy.dot(xsi.conj(), b.T)
 
     c = cupy.linalg.solve(h, g)
     x = _gen_x0(c, cupy.asarray(xs))
     if b.ndim == 1:
         x = x[0]
 
     if x0 is not None:
@@ -597,28 +602,39 @@
     rmat = cupy.empty((nvec,nvec), order='F', dtype=dtype)
 
     nv = 0
     for i in range(nvec):
         xi = cupy.array(xs[i], copy=True)
         rmat[:,nv] = 0
         rmat[nv,nv] = 1
-        for j in range(nv):
-            prod = dot(qs[j].conj(), xi)
-            xi -= qs[j] * prod
-            rmat[:,nv] -= rmat[:,j] * prod
+
+        prod = dot(qs[:nv].conj(), xi)
+        xi -= cupy.dot(qs[:nv].T, prod)
+        rmat[:,nv] -= cupy.dot(rmat[:,:nv], prod)
+
         innerprod = dot(xi.conj(), xi).real
         norm = cupy.sqrt(innerprod)
         if innerprod > lindep:
             qs[nv] = xi/norm
             rmat[:nv+1,nv] /= norm
             nv += 1
     return qs[:nv], cupy.linalg.inv(rmat[:nv,:nv])
 
 def _gen_x0(v, xs):
-    return cupy.dot(v.T, xs)
+    ndim = v.ndim
+    if ndim == 1:
+        v = v[:,None]
+    space, nroots = v.shape
+    x0 = cupy.einsum('c,x->cx', v[space-1], cupy.asarray(xs[space-1]))
+    for i in reversed(range(space-1)):
+        xsi = cupy.asarray(xs[i])
+        x0 += cupy.expand_dims(v[i],-1) * xsi
+    if ndim == 1:
+        x0 = x0[0]
+    return x0
 
 def empty_mapped(shape, dtype=float, order='C'):
     '''(experimental)
     Returns a new, uninitialized NumPy array with the given shape and dtype.
 
     This is a convenience function which is just :func:`numpy.empty`,
     except that the underlying buffer is a pinned and mapped memory.
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/cusolver.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/cusolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,31 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import numpy as np
 import cupy
 import ctypes
-from cupy.cuda import device
 from cupy_backends.cuda.libs import cusolver
 from cupy_backends.cuda.libs import cublas
+from cupy.cuda import device
 
-libcusolver = ctypes.CDLL('libcusolver.so')
 _handle = device.get_cusolver_handle()
+libcusolver = ctypes.CDLL('libcusolver.so')
 
 CUSOLVER_EIG_TYPE_1 = 1
 CUSOLVER_EIG_TYPE_2 = 2
 CUSOLVER_EIG_TYPE_3 = 3
 
 CUSOLVER_EIG_MODE_NOVECTOR = 0
 CUSOLVER_EIG_MODE_VECTOR = 1
 
 libcusolver.cusolverDnDsygvd_bufferSize.restype = int
 libcusolver.cusolverDnDsygvd.restype = int
 
-devInfo = cupy.empty(1, dtype=np.int32)
 _buffersize = {}
 
 # https://docs.nvidia.com/cuda/cusolver/index.html#cusolverdn-t-sygvd
 libcusolver.cusolverDnDsygvd_bufferSize.argtypes = [
     ctypes.c_void_p, # handle
     ctypes.c_int,    # itype
     ctypes.c_int,    # jobz
@@ -72,15 +71,15 @@
     '''
     solve generalized eigenvalue problem
     '''
     n = h.shape[0]
     w = cupy.zeros(n)
     A = h.copy()
     B = s.copy()
-
+    
     # TODO: reuse workspace
     if n in _buffersize:
         lwork = _buffersize[n]
     else:
         lwork = ctypes.c_int()
         status = libcusolver.cusolverDnDsygvd_bufferSize(
             _handle,
@@ -92,17 +91,17 @@
             n,
             B.data.ptr,
             n,
             w.data.ptr,
             ctypes.byref(lwork)
         )
         lwork = lwork.value
-
+    
     work = cupy.empty(lwork)
-
+    devInfo = cupy.empty(1, dtype=np.int32)
     status = libcusolver.cusolverDnDsygvd(
         _handle,
         CUSOLVER_EIG_TYPE_1,
         CUSOLVER_EIG_MODE_VECTOR,
         cublas.CUBLAS_FILL_MODE_LOWER,
         n,
         A.data.ptr,
@@ -110,15 +109,15 @@
         B.data.ptr,
         n,
         w.data.ptr,
         work.data.ptr,
         lwork,
         devInfo.data.ptr
     )
-
+    
     if status != 0:
         raise RuntimeError("failed in eigh kernel")
     return w, A.T
 
 def cholesky(A):
     n = len(A)
     assert A.flags['C_CONTIGUOUS']
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/cutensor.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/cutensor.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd3.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/dftd3.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd4.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/dftd4.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/diis.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/logger.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/logger.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/lib/utils.py` & `gpu4pyscf-0.7.8/gpu4pyscf/lib/utils.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/mp/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/mp/dfmp2.py` & `gpu4pyscf-0.7.8/gpu4pyscf/mp/dfmp2.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/mp/mp2.py` & `gpu4pyscf-0.7.8/gpu4pyscf/mp/mp2.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/properties/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/properties/ir.py` & `gpu4pyscf-0.7.8/gpu4pyscf/properties/ir.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/properties/polarizability.py` & `gpu4pyscf-0.7.8/gpu4pyscf/properties/polarizability.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/properties/shielding.py` & `gpu4pyscf-0.7.8/gpu4pyscf/properties/shielding.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from gpu4pyscf.scf import cphf
 import numpy as np
-from pyscf.data import nist
 import cupy
+from pyscf.data import nist
 from pyscf.scf import _vhf, jk
 from gpu4pyscf.dft import numint
 from gpu4pyscf.lib.cupy_helper import contract, take_last2d, add_sparse
-
+from gpu4pyscf.scf import cphf
 
 def gen_vind(mf, mo_coeff, mo_occ):
     """get the induced potential. This is the same as contract the mo1 with the kernel.
 
     Args:
         mf: mean field object
         mo_coeff (numpy.array): mo coefficients
@@ -70,44 +69,46 @@
     mo_occ = getattr(dms, 'mo_occ', None)
     nao = mo_coeff.shape[1]
     
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
         opt = ni.gdftopt
+    _sorted_mol = opt._sorted_mol
+
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dms = cupy.asarray(dms).reshape(-1,nao0,nao0)
     dms = take_last2d(dms, opt.ao_idx)
     mo_coeff = mo_coeff[opt.ao_idx]
 
     vmat = cupy.zeros((3, nao, nao))
     if xctype == 'LDA':
         ao_deriv = 0
     else:
         ao_deriv = 1
 
-    for ao, index, weight, coords in ni.block_loop(opt.mol, grids, nao, ao_deriv):
+    for ao, index, weight, coords in ni.block_loop(_sorted_mol, grids, nao, ao_deriv):
         mo_coeff_mask = mo_coeff[index,:]
-        rho = numint.eval_rho2(opt.mol, ao, mo_coeff_mask, mo_occ, None, xctype)
+        rho = numint.eval_rho2(_sorted_mol, ao, mo_coeff_mask, mo_occ, None, xctype)
         vxc = ni.eval_xc_eff(xc_code, rho, deriv=1, xctype=xctype)[1]
         if xctype == 'LDA':
             wv = weight * vxc[0]
-            giao = opt.mol.eval_gto('GTOval_ig', coords.get(), comp=3)  # (#C(0 1) g) |AO>
+            giao = _sorted_mol.eval_gto('GTOval_ig', coords.get(), comp=3)  # (#C(0 1) g) |AO>
             giao = cupy.array(giao)
             giao_aux = giao[:,:,index]
             for idirect in range(3):
                 vtmp = contract('pu,p,vp->uv', giao_aux[idirect], wv, ao)
                 vtmp = cupy.ascontiguousarray(vtmp)
                 add_sparse(vmat[idirect], vtmp, index)
             
         elif xctype == 'GGA':
             wv = vxc * weight
-            giao = opt.mol.eval_gto('GTOval_ig', coords.get(), comp=3)
-            giao_nabla = opt.mol.eval_gto('GTOval_ipig', coords.get()).reshape(3, 3, -1, nao)
+            giao = _sorted_mol.eval_gto('GTOval_ig', coords.get(), comp=3)
+            giao_nabla = _sorted_mol.eval_gto('GTOval_ipig', coords.get()).reshape(3, 3, -1, nao)
             giao = cupy.array(giao)
             giao_nabla = cupy.array(giao_nabla)
             giao_aux = giao[:,:,index]
             giao_nabla_aux = giao_nabla[:,:,:,index]
             for idirect in range(3):
                 # * write like the gpu4pyscf numint part, but explicitly use the einsum
                 aow = contract('pn,p->pn', giao_aux[idirect], wv[0])
@@ -128,16 +129,14 @@
             pass
         else:
             raise NotImplementedError(
                 f'numint.nr_rks for functional {xc_code}')
 
         ao = None
 
-    # vmat = contract('pi,npq->niq', coeff, vmat)
-    # vmat = contract('qj,niq->nij', coeff, vmat)
     vmat = take_last2d(vmat, opt.rev_ao_idx)
 
     if numint.FREE_CUPY_CACHE:
         dms = None
         cupy.get_default_memory_pool().free_all_blocks()
 
     return (vmat - vmat.transpose(0, 2, 1))
@@ -223,18 +222,18 @@
     else:
         vk2 = np.empty((3, nao, nao))
         for i in range(3):
             vk2[i] = -jk.get_jk(mf.mol, s1jkdm1[i].get(), 'ijkl,jk->il')*0.5*hyb
         vk2 = cupy.array(vk2)
     h1ao += vk2
     tmp = contract('xuv,ua->xav', h1ao, mvir)
-    Veff_ai = contract('xav,vi->xai', tmp, mocc)
-    Veff_ai -= contract('xai,i->xai', s1ai, mo_energy[idx_occ])
-    Veff_ai = cupy.array(Veff_ai)
-    mo1 = cphf.solve(fx, mo_energy, mo_occ, Veff_ai, max_cycle=20, tol=1e-10)[0]
+    veff_ai = contract('xav,vi->xai', tmp, mocc)
+    veff_ai -= contract('xai,i->xai', s1ai, mo_energy[idx_occ])
+
+    mo1 = cphf.solve(fx, mo_energy, mo_occ, veff_ai, max_cycle=20, tol=1e-10)[0]
 
     shielding_d = cupy.empty((natom, 3, 3))
     shielding_p = cupy.empty((natom, 3, 3))
 
     for atm_id in range(natom):
         mf.mol.set_rinv_origin(mf.mol.atom_coord(atm_id))
         # ! imaginary part (p* | rinv cross p | )
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/qmmm/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/qmmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/qmmm/chelpg.py` & `gpu4pyscf-0.7.8/gpu4pyscf/qmmm/chelpg.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/_response_functions.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/_response_functions.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/cphf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/cphf.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,29 +52,31 @@
     '''For field independent basis. First order overlap matrix is zero'''
     log = logger.new_logger(verbose=verbose)
     t0 = (logger.process_clock(), logger.perf_counter())
 
     e_a = mo_energy[mo_occ==0]
     e_i = mo_energy[mo_occ>0]
     I, A = cupy.meshgrid(e_i, e_a)
-    e_ai = 1 / (A - I)#cupy.einsum('a,i->ai', e_a, e_i)
+    e_ai = 1 / (A - I)
     mo1base = h1 * -e_ai
+    nvir, nocc = e_ai.shape
 
     def vind_vo(mo1):
-        v = fvind(mo1.reshape(h1.shape)).reshape(h1.shape)
+        v = fvind(mo1.reshape(-1,nvir,nocc)).reshape(-1,nvir,nocc)
         v *= e_ai
-        return v.ravel()
-    mo1 = krylov(vind_vo, mo1base.ravel(),
+        return v.reshape(-1,nvir*nocc)
+    mo1 = krylov(vind_vo, mo1base.reshape(-1,nvir*nocc),
                      tol=tol, max_cycle=max_cycle, hermi=hermi, verbose=log)
     log.timer('krylov solver in CPHF', *t0)
     return mo1.reshape(h1.shape), None
 
 # h1 shape is (:,nocc+nvir,nocc)
 def solve_withs1(fvind, mo_energy, mo_occ, h1, s1,
-                 max_cycle=50, tol=1e-9, hermi=False, verbose=logger.WARN):
+                max_cycle=50, tol=1e-9, hermi=False,
+                verbose=logger.WARN, level_shift=0):
     '''For field dependent basis. First order overlap matrix is non-zero.
     The first order orbitals are set to
     C^1_{ij} = -1/2 S1
     e1 = h1 - s1*e0 + (e0_j-e0_i)*c1 + vhf[c1]
     Kwargs:
         hermi : boolean
             Whether the matrix defined by fvind is Hermitian or not.
@@ -85,42 +87,45 @@
     log = logger.new_logger(verbose=verbose)
     t0 = (logger.process_clock(), logger.perf_counter())
 
     occidx = mo_occ > 0
     viridx = mo_occ == 0
     e_a = mo_energy[viridx]
     e_i = mo_energy[occidx]
-    I, A = cupy.meshgrid(e_i, e_a)
-    e_ai = 1 / (A - I)
+    e_ai = 1 / (e_a[:,None] + level_shift - e_i)
     nvir, nocc = e_ai.shape
     nmo = nocc + nvir
 
     s1 = s1.reshape(-1,nmo,nocc)
     hs = mo1base = h1.reshape(-1,nmo,nocc) - s1*e_i
-    mo_e1 = hs[:,occidx,:].copy()
 
+    mo1base = hs.copy()
     mo1base[:,viridx] *= -e_ai
     mo1base[:,occidx] = -s1[:,occidx] * .5
 
     def vind_vo(mo1):
-        v = fvind(mo1.reshape(h1.shape)).reshape(-1,nmo,nocc)
+        mo1 = mo1.reshape(-1,nmo, nocc)
+        v = fvind(mo1).reshape(-1,nmo, nocc)
+        if level_shift != 0:
+            v -= mo1 * level_shift
         v[:,viridx,:] *= e_ai
         v[:,occidx,:] = 0
-        return v.ravel()
-    mo1 = krylov(vind_vo, mo1base.ravel(),
+        return v.reshape(-1,nmo*nocc)
+
+    mo1 = krylov(vind_vo, mo1base.reshape(-1,nmo*nocc),
                      tol=tol, max_cycle=max_cycle, hermi=hermi, verbose=log)
     mo1 = mo1.reshape(mo1base.shape)
+    mo1[:,occidx] = mo1base[:,occidx]
     log.timer('krylov solver in CPHF', *t0)
 
-    v1mo = fvind(mo1.reshape(h1.shape)).reshape(-1,nmo,nocc)
-    mo1[:,viridx] = mo1base[:,viridx] - v1mo[:,viridx]*e_ai
+    hs += fvind(mo1).reshape(mo1base.shape)
+    mo1[:,viridx] = hs[:,viridx] / (e_i - e_a[:,None])
 
     # mo_e1 has the same symmetry as the first order Fock matrix (hermitian or
     # anti-hermitian). mo_e1 = v1mo - s1*lib.direct_sum('i+j->ij',e_i,e_i)
-    It, I = cupy.meshgrid(e_i, e_i)
-    mo_e1 += mo1[:,occidx] * (I - It)#(cupy.einsum('i,j->ij', e_i, e_i)
-    mo_e1 += v1mo[:,occidx,:]
+    mo_e1 = hs[:,occidx,:]
+    mo_e1 += mo1[:,occidx] * (e_i[:,None] - e_i)
 
     if h1.ndim == 3:
         return mo1, mo_e1
     else:
         return mo1.reshape(h1.shape), mo_e1.reshape(nocc,nocc)
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/diis.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/dispersion.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/dispersion.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/ghf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/ghf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/hf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,41 +396,34 @@
     if hasattr(dm0, 'mo_coeff') and hasattr(dm0, 'mo_occ'):
         if dm0.ndim == 2:
             mo_coeff = cupy.asarray(dm0.mo_coeff)
             mo_occ = cupy.asarray(dm0.mo_occ)
             occ_coeff = cupy.asarray(mo_coeff[:,mo_occ>0])
             dm = tag_array(dm, occ_coeff=occ_coeff, mo_occ=mo_occ, mo_coeff=mo_coeff)
 
-    # use optimized workflow if possible
-    if hasattr(mf, 'init_workflow'):
-        mf.init_workflow(dm0=dm)
-        h1e = mf.h1e
-        s1e = mf.s1e
-    else:
-        h1e = cupy.asarray(mf.get_hcore(mol))
-        s1e = cupy.asarray(mf.get_ovlp(mol))
-
+    h1e = cupy.asarray(mf.get_hcore(mol))
+    s1e = cupy.asarray(mf.get_ovlp(mol))
+    
     vhf = mf.get_veff(mol, dm)
     e_tot = mf.energy_tot(dm, h1e, vhf)
     logger.info(mf, 'init E= %.15g', e_tot)
     t1 = log.timer_debug1('total prep', *t0)
     scf_conv = False
-
     if isinstance(mf.diis, lib.diis.DIIS):
         mf_diis = mf.diis
     elif mf.diis:
         assert issubclass(mf.DIIS, lib.diis.DIIS)
         mf_diis = mf.DIIS(mf, mf.diis_file)
         mf_diis.space = mf.diis_space
         mf_diis.rollback = mf.diis_space_rollback
         fock = mf.get_fock(h1e, s1e, vhf, dm)
         _, mf_diis.Corth = mf.eig(fock, s1e)
     else:
         mf_diis = None
-
+    
     for cycle in range(mf.max_cycle):
         t0 = log.init_timer()
         dm_last = dm
         last_hf_e = e_tot
 
         f = mf.get_fock(h1e, s1e, vhf, dm, cycle, mf_diis)
         t1 = log.timer_debug1('DIIS', *t0)
@@ -668,15 +661,15 @@
 
     to_gpu = utils.to_gpu
     device = utils.device
 
     _keys = {'e_disp', 'h1e', 's1e', 'e_mf', 'screen_tol', 'conv_tol_cpscf', 'disp_with_3body'}
 
     screen_tol = 1e-14
-    conv_tol_cpscf = 1e-3
+    conv_tol_cpscf = 1e-6
     DIIS = diis.SCF_DIIS
     get_jk = _get_jk
     _eigh = staticmethod(eigh)
     make_rdm1 = make_rdm1
     energy_elec = energy_elec
     get_fock = get_fock
     get_occ = get_occ
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/int4c2e.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/int4c2e.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/rohf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/rohf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/ucphf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/ucphf.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,28 +126,28 @@
     mo1base_a = hs_a.copy()
     mo1base_b = hs_b.copy()
     mo1base_a[:,viridxa] *= -eai_a
     mo1base_b[:,viridxb] *= -eai_b
     mo1base_a[:,occidxa] = -s1_a[:,occidxa] * .5
     mo1base_b[:,occidxb] = -s1_b[:,occidxb] * .5
     mo1base = cupy.hstack((mo1base_a.reshape(nset,-1), mo1base_b.reshape(nset,-1)))
-
+    
     def vind_vo(mo1):
-        mo1 = mo1.reshape(mo1base.shape)
-        v = fvind(mo1).reshape(mo1base.shape)
+        mo1 = mo1.reshape(-1,nmoa*nocca+nmob*noccb)
+        v = fvind(mo1).reshape(-1,nmoa*nocca+nmob*noccb)
         if level_shift != 0:
             v -= mo1 * level_shift
-        v1a = v[:,:nmoa*nocca].reshape(nset,nmoa,nocca)
-        v1b = v[:,nmoa*nocca:].reshape(nset,nmob,noccb)
+        v1a = v[:,:nmoa*nocca].reshape(-1,nmoa,nocca)
+        v1b = v[:,nmoa*nocca:].reshape(-1,nmob,noccb)
         v1a[:,viridxa] *= eai_a
         v1b[:,viridxb] *= eai_b
         v1a[:,occidxa] = 0
         v1b[:,occidxb] = 0
-        return v.ravel()
-    mo1 = krylov(vind_vo, mo1base.ravel(),
+        return v.reshape(-1,nmoa*nocca+nmob*noccb)
+    mo1 = krylov(vind_vo, mo1base.reshape(-1,nmoa*nocca+nmob*noccb),
                      tol=tol, max_cycle=max_cycle, hermi=hermi, verbose=log)
 
     mo1 = mo1.reshape(mo1base.shape)
     mo1_a = mo1[:,:nmoa*nocca].reshape(nset,nmoa,nocca)
     mo1_b = mo1[:,nmoa*nocca:].reshape(nset,nmob,noccb)
     mo1_a[:,occidxa] = mo1base_a[:,occidxa]
     mo1_b[:,occidxb] = mo1base_b[:,occidxb]
```

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/scf/uhf.py` & `gpu4pyscf-0.7.8/gpu4pyscf/scf/uhf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/_attach_solvent.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/_attach_solvent.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/__init__.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/pcm.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/pcm.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd_experiment.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/grad/smd_experiment.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/pcm.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/pcm.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd_experiment.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/hessian/smd_experiment.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/pcm.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/pcm.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd_experiment.py` & `gpu4pyscf-0.7.8/gpu4pyscf/solvent/smd_experiment.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/gpu4pyscf.egg-info/SOURCES.txt` & `gpu4pyscf-0.7.8/gpu4pyscf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.7/setup.py` & `gpu4pyscf-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,13 +120,13 @@
         "pytest==7.2.0",
         "pytest-cov==4.0.0",
         "pytest-cover==3.0.0",
         "pytest-coverage==0.0",
     ],
     cmdclass={'build_py': CMakeBuildPy},
     install_requires=[
-        'pyscf>=2.5.0',
+        'pyscf~=2.6.0',
         f'cupy-cuda{CUDA_VERSION}',
         'geometric',
         f'gpu4pyscf-libxc-cuda{CUDA_VERSION}',
     ]
 )
```

