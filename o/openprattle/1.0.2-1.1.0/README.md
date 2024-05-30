# Comparing `tmp/openprattle-1.0.2.tar.gz` & `tmp/openprattle-1.1.0.tar.gz`

## Comparing `openprattle-1.0.2.tar` & `openprattle-1.1.0.tar`

### file list

```diff
@@ -1,153 +1,154 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 openprattle-1.0.2/environment.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openprattle-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openprattle-1.0.2/.github/workflows/python-test.yml
--rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 openprattle-1.0.2/bin/oprattle
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 openprattle-1.0.2/openprattle/__init__.py
--rw-r--r--   0        0        0    26799 2020-02-02 00:00:00.000000 openprattle-1.0.2/openprattle/babel.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 openprattle-1.0.2/openprattle/program.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/conftest.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/test_formats.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/test_lib.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/test_prog.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.CONFIG
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.CONTCAR
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.CONTFF
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.MDFF
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.POSCAR
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.POSFF
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.VASP
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.acesin
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.adf
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.alc
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.ascii
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.bgf
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.box
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.bs
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.c3d1
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.c3d2
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cac
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.caccrt
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cache
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cacint
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.can
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cdjson
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cdx
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cdxml
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cht
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.ck
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cmlr
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cof
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.com
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.confabreport
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.copy
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.crk2d
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.crk3d
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.csr
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cssr
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.ct
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cub
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.cube
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.dalmol
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.dmol
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.dx
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.ent
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.exyz
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fa
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fasta
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.feat
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fh
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fhiaims
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fix
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fps
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fpt
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fract
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fs
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.fsa
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gamin
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gau
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gjc
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gjf
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gpr
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gr96
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gro
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gukin
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gukout
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.gzmat
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.hin
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.inchi
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.inchikey
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.inp
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.jin
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.k
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.lmpdat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.lpmd
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mcdl
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mcif
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mdl
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.ml2
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mmcif
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mmd
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mmod
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mna
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mol
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mol2
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mold
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.molden
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.molf
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.molreport
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mop
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mopcrt
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mopin
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mp
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mpc
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mpd
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mpqcin
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.mrv
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.msms
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.nul
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.nw
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.orcainp
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.outmol
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.paint
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pcjson
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pcm
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pdb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pdbqt
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.png
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pointcloud
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pov
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pqr
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.pqs
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.qcin
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.report
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.rinchi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.rsmi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.rxn
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.sd
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.sdf
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.smi
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.smiles
--rw-r--r--   0        0        0 12440484 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.stl
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.svg
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.sy2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.tdd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.text
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.therm
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.tmol
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.txt
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.txyz
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.unixyz
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.vmol
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.xed
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.xyz
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.yob
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 openprattle-1.0.2/test/data/Benzene.zin
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 openprattle-1.0.2/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 openprattle-1.0.2/LICENSE
--rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 openprattle-1.0.2/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 openprattle-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 openprattle-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 openprattle-1.1.0/environment.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openprattle-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openprattle-1.1.0/.github/workflows/python-test.yml
+-rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 openprattle-1.1.0/bin/oprattle
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 openprattle-1.1.0/openprattle/__init__.py
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 openprattle-1.1.0/openprattle/babel.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 openprattle-1.1.0/openprattle/log.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 openprattle-1.1.0/openprattle/program.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/conftest.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/test_formats.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/test_lib.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/test_prog.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.CONFIG
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.CONTCAR
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.CONTFF
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.MDFF
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.POSCAR
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.POSFF
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.VASP
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.acesin
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.adf
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.alc
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.ascii
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.bgf
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.box
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.bs
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.c3d1
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.c3d2
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cac
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.caccrt
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cache
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cacint
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.can
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cdjson
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cdx
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cdxml
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cht
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.ck
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cml
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cmlr
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cof
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.com
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.confabreport
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.copy
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.crk2d
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.crk3d
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.csr
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cssr
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.ct
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cub
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.cube
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.dalmol
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.dmol
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.dx
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.ent
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.exyz
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fa
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fasta
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.feat
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fh
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fhiaims
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fix
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fps
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fpt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fract
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fs
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.fsa
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gamin
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gau
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gjc
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gjf
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gpr
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gr96
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gro
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gukin
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gukout
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.gzmat
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.hin
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.inchi
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.inchikey
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.inp
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.jin
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.k
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.lmpdat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.lpmd
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mcdl
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mcif
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mdl
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.ml2
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mmcif
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mmd
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mmod
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mna
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mol
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mol2
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mold
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.molden
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.molf
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.molreport
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mop
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mopcrt
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mopin
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mp
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mpc
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mpd
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mpqcin
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.mrv
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.msms
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.nul
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.nw
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.orcainp
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.outmol
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.paint
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pcjson
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pcm
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pdb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pdbqt
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.png
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pointcloud
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pov
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pqr
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.pqs
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.qcin
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.report
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.rinchi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.rsmi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.rxn
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.sd
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.sdf
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.smi
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.smiles
+-rw-r--r--   0        0        0 12440484 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.stl
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.svg
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.sy2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.tdd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.text
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.therm
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.tmol
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.txt
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.txyz
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.unixyz
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.vmol
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.xed
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.xyz
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.yob
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 openprattle-1.1.0/test/data/Benzene.zin
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 openprattle-1.1.0/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 openprattle-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 openprattle-1.1.0/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 openprattle-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 openprattle-1.1.0/PKG-INFO
```

### Comparing `openprattle-1.0.2/.github/workflows/python-publish.yml` & `openprattle-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/.github/workflows/python-test.yml` & `openprattle-1.1.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/openprattle/__init__.py` & `openprattle-1.1.0/openprattle/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """A wrapper for accessing the pybel library and obabel command-line tools"""
 
 import sys
 from pathlib import Path
 
 # Version information.
 major_version = 1
-minor_version = 0
-revision = 2
+minor_version = 1
+revision = 0
 prerelease = None
 
 development = prerelease is not None
 
 __version__ = "{}.{}.{}{}".format(major_version, minor_version, revision,"-pre.{}".format(prerelease) if development else "")
 __author__ = "Oliver S. Lee"
 
@@ -37,9 +37,8 @@
     # We need to tell openbabel where its library components are.
     os.environ['BABEL_LIBDIR'] = str(Path(sys._MEIPASS, "openbabel", "lib", openbabel_version))
     
     # And also data.
     os.environ['BABEL_DATADIR'] = str(Path(sys._MEIPASS, "openbabel", "data", openbabel_version))
 
 # Convenience imports.
-from .babel import Openbabel_converter, Obabel_converter, Pybel_converter, HAVE_PYBEL,\
-    formats, Obabel_formats, Pybel_formats
+from .babel import Openbabel_converter, HAVE_PYBEL, formats
```

### Comparing `openprattle-1.0.2/openprattle/babel.py` & `openprattle-1.1.0/openprattle/babel.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import re
 import sys
 import os
 import copy
 from pathlib import Path
 import logging
 
-import openprattle
+import openprattle.log
 
 # Try and load openbabel bindings.
 HAVE_PYBEL = False
 
 try:
     from openbabel import pybel
     HAVE_PYBEL = True
 
 except ModuleNotFoundError:
     # No bindings, carry on.
-    raise
-    logging.debug("Could not load python pybel bindings; falling back to obabel executable", exc_info = True)
+    # TODO: This message is unreachable. Logging is not set to debug by default, and this module is imported before the user can ever change it.
+    logging.getLogger("openprattle").debug("Could not load python pybel bindings; falling back to obabel executable", exc_info = True)
 
 except Exception:
     # Some other error occurred; print an error but continue.
-    raise
-    logging.error("Found but could not load python pybel bindings; falling back to obabel executable", exc_info = True)
+    # TODO: Should we catch this?
+    logging.getLogger("openprattle").error("Found but could not load python pybel bindings; falling back to obabel executable", exc_info = True)
 
 # Formats that are broken with either pybel or obabel.
 # TODO: We should try and record which versions of obabel these are broken with; they may get fixed in the future. 
 FORBIDDEN = {
     "PYBEL": (
         # Results in core-dump, or an empty file depending on version.
         "cdx",
@@ -54,15 +54,15 @@
 
         Input files can be specified in one of three ways:
          - As an open file descriptor (input_file and input_file_type)
          - As an in-memory buffer, most probably a string or bytes-like object (input_file_buffer and input_file_type)
          - As a file path (input_file_path and optionally input_file_type)
         
         :param input_file: An open file descriptor in the format given by input_file_type that should be converted.
-        :param input_file_buffer: Alternartively, a buffer (unicode string or bytes) in the format given by input_file_type that should be converted.
+        :param input_file_buffer: Alternatively, a buffer (unicode string or bytes) in the format given by input_file_type that should be converted.
         :param input_file_path: Alternatively, a path to a file that should be converted.
         :param input_file_type: A shortcode identifying the format of the input file. If not given but input_file_path is given, then this will be determined automatically.
         """
         
         self.input_file = input_file
         self.input_file_buffer = input_file_buffer
         self.input_file_path = input_file_path
@@ -189,15 +189,15 @@
         raise NotImplementedError("Abstract class Babel_converter does not have a convert() method defined (inheriting classes should write their own)")
 
 
 if HAVE_PYBEL:
 
     class ObErrorLog_wrapper():
         """
-        Class for wrapping the logging begaviour of openbabel and pybel.
+        Class for wrapping the logging behaviour of openbabel and pybel.
         """
 
         def __init__(self, warnings_as_errors = True):
             """
             :param stream: The output stream to wrap.
             :param warnings_as_errors: Whether to raise an exception on obabel warnings (normally a good idea)
             """
@@ -241,15 +241,15 @@
             
             else:
                 log_levels.append((pybel.ob.obWarning, logging.WARNING))
 
             # Print any messages.
             for oblevel, level in log_levels:
                 for log in pybel.ob.obErrorLog.GetMessagesOfLevel(oblevel):
-                    logging.log(level, log)
+                    logging.getLogger("openprattle").log(level, log)
 
             # Generate exceptions.
             exceptions = []
             for oblevel in error_levels:
                 exceptions.extend([Exception("OpenBabel error:\n{}".format(log)) for log in pybel.ob.obErrorLog.GetMessagesOfLevel(oblevel)])
             
             # Chain them together.
@@ -353,15 +353,15 @@
             
             # If we got a 2D (or 1D) format, convert to 3D (but warn that we are doing so.)
             if molecule.dim != 3 and gen3D:
                 # We're missing 3D coords.
                 with ObErrorLog_wrapper(False):
                     dim = molecule.dim
 
-                logging.warning("Generating 3D coordinates from {}D file '{}'; this will scramble atom coordinates".format(dim, self.input_name))
+                logging.getLogger("openprattle").warning("Generating 3D coordinates from {}D file '{}'; this will scramble atom coordinates".format(dim, self.input_name))
                 
                 with ObErrorLog_wrapper(False):
                     molecule.localopt()
                 
             if self.add_H:
                 # Add hydrogens.
                 with ObErrorLog_wrapper(False):
@@ -419,19 +419,19 @@
             if self.input_file_type.lower() == "cdx":
                 gen3D = True
             else:
                 gen3D = False
         
         if charge is not None:
             # We can't set charge with obabel sadly.
-            logging.warning("Unable to set charge '{}' of molecule loaded from file '{}' with obabel converter".format(charge, self.input_name))
+            logging.getLogger("openprattle").warning("Unable to set charge '{}' of molecule loaded from file '{}' with obabel converter".format(charge, self.input_name))
             
         if multiplicity is not None:
             # We can't set charge with obabel sadly.
-            logging.warning("Unable to set multiplicity '{}' of molecule loaded from file '{}' with obabel converter".format(multiplicity, self.input_name))
+            logging.getLogger("openprattle").warning("Unable to set multiplicity '{}' of molecule loaded from file '{}' with obabel converter".format(multiplicity, self.input_name))
         
         # Run
         return self.run_obabel(output_file_type, output_file, gen3D = gen3D)
         
     def run_obabel(self, output_file_type, output_file, *, gen3D):
         """
         Run obabel, converting the input file wrapped by this class to the designated output_file_type.
@@ -452,15 +452,15 @@
         sig.extend([
              "-o", output_file_type,
              "-i", self.input_file_type
         ])
         
         # Add gen3D command if we've been asked to.
         if gen3D:
-            logging.warning("Generating 3D coordinates from file '{}'; this will scramble atom coordinates".format(self.input_name))
+            logging.getLogger("openprattle").warning("Generating 3D coordinates from file '{}'; this will scramble atom coordinates".format(self.input_name))
             sig.append("--gen3D")
         
         # Add H if we've been asked.    
         if self.add_H:
             sig.append("-h")
             
         # If a file to write to has been given, set it.
```

### Comparing `openprattle-1.0.2/openprattle/program.py` & `openprattle-1.1.0/openprattle/program.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import argparse
 
 import openprattle
 from openprattle import Openbabel_converter, HAVE_PYBEL, formats
+import openprattle.log
 
 def main():
     """
     Main entry point for the program.
     """
     # Get our args from the command line.
     parser = argparse.ArgumentParser(
@@ -22,19 +23,23 @@
     parser.add_argument("-M", "--multiplicity", help = "The multiplicity to set in the output format. Note that not all formats support a multiplicity", default = None, type = int)
     parser.add_argument("--gen3D", help = "Whether to optimise the input coordinates via a rapid force-field optimisation. This option is useful for converting 1D or 2D formats to 3D. The default (Auto) is to only optimise coordinates that are not already in 3 dimensions.", choices = ["True", "Auto", "False"])
     parser.add_argument("--backend", help = "Force the user of a particular backend", choices = ["Auto", "Pybel", "Obabel"])
     
     parser.add_argument("--bindings", help = "Determine whether the pybel bindings are available", action = "store_true")
     parser.add_argument("--readable", help = "List readable (input) formats", action = "store_true")
     parser.add_argument("--writable", help = "List writable (output) formats", action = "store_true")
-    parser.add_argument("--json", help = "Dump the list of readable and/or writable formats in JSON", action = "store_true")
+    parser.add_argument("--json", help = "Dump the list of readable and/or writable formats in JSON, and dump warnings and errors in JSON", action = "store_true")
     parser.add_argument("-v", "--version", action = "version", version = str(openprattle.__version__))
 
     args = parser.parse_args()
 
+    # First, setup logging.
+    if args.json:
+        openprattle.log.init_logger(True)
+
     if args.bindings:
         if HAVE_PYBEL:
             print(True)
         
         else:
             print(False)
```

### Comparing `openprattle-1.0.2/test/conftest.py` & `openprattle-1.1.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/test_formats.py` & `openprattle-1.1.0/test/test_formats.py`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/test_lib.py` & `openprattle-1.1.0/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/test_prog.py` & `openprattle-1.1.0/test/test_prog.py`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.CONFIG` & `openprattle-1.1.0/test/data/Benzene.CONFIG`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.CONTCAR` & `openprattle-1.1.0/test/data/Benzene.CONTCAR`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.CONTFF` & `openprattle-1.1.0/test/data/Benzene.CONTFF`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.MDFF` & `openprattle-1.1.0/test/data/Benzene.MDFF`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.POSCAR` & `openprattle-1.1.0/test/data/Benzene.POSCAR`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.POSFF` & `openprattle-1.1.0/test/data/Benzene.POSFF`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.VASP` & `openprattle-1.1.0/test/data/Benzene.VASP`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.acesin` & `openprattle-1.1.0/test/data/Benzene.acesin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.adf` & `openprattle-1.1.0/test/data/Benzene.adf`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.alc` & `openprattle-1.1.0/test/data/Benzene.alc`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.ascii` & `openprattle-1.1.0/test/data/Benzene.ascii`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.bgf` & `openprattle-1.1.0/test/data/Benzene.bgf`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.box` & `openprattle-1.1.0/test/data/Benzene.box`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.bs` & `openprattle-1.1.0/test/data/Benzene.bs`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.c3d1` & `openprattle-1.1.0/test/data/Benzene.c3d1`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.c3d2` & `openprattle-1.1.0/test/data/Benzene.c3d2`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cac` & `openprattle-1.1.0/test/data/Benzene.cac`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cache` & `openprattle-1.1.0/test/data/Benzene.cache`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cdjson` & `openprattle-1.1.0/test/data/Benzene.cdjson`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cdx` & `openprattle-1.1.0/test/data/Benzene.cdx`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cdxml` & `openprattle-1.1.0/test/data/Benzene.cdxml`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cif` & `openprattle-1.1.0/test/data/Benzene.cif`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cml` & `openprattle-1.1.0/test/data/Benzene.cml`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cmlr` & `openprattle-1.1.0/test/data/Benzene.cmlr`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cof` & `openprattle-1.1.0/test/data/Benzene.cof`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.com` & `openprattle-1.1.0/test/data/Benzene.com`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.copy` & `openprattle-1.1.0/test/data/Benzene.copy`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.crk2d` & `openprattle-1.1.0/test/data/Benzene.crk2d`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.crk3d` & `openprattle-1.1.0/test/data/Benzene.crk3d`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.csr` & `openprattle-1.1.0/test/data/Benzene.csr`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.cssr` & `openprattle-1.1.0/test/data/Benzene.cssr`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.ct` & `openprattle-1.1.0/test/data/Benzene.ct`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.dalmol` & `openprattle-1.1.0/test/data/Benzene.dalmol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.dmol` & `openprattle-1.1.0/test/data/Benzene.dmol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.ent` & `openprattle-1.1.0/test/data/Benzene.ent`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.exyz` & `openprattle-1.1.0/test/data/Benzene.exyz`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.fhiaims` & `openprattle-1.1.0/test/data/Benzene.fhiaims`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gamin` & `openprattle-1.1.0/test/data/Benzene.gamin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gau` & `openprattle-1.1.0/test/data/Benzene.gau`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gjc` & `openprattle-1.1.0/test/data/Benzene.gjc`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gjf` & `openprattle-1.1.0/test/data/Benzene.gjf`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gpr` & `openprattle-1.1.0/test/data/Benzene.gpr`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gr96` & `openprattle-1.1.0/test/data/Benzene.gr96`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gro` & `openprattle-1.1.0/test/data/Benzene.gro`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gukin` & `openprattle-1.1.0/test/data/Benzene.gukin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.gzmat` & `openprattle-1.1.0/test/data/Benzene.gzmat`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.hin` & `openprattle-1.1.0/test/data/Benzene.hin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.inp` & `openprattle-1.1.0/test/data/Benzene.inp`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.jin` & `openprattle-1.1.0/test/data/Benzene.jin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.lmpdat` & `openprattle-1.1.0/test/data/Benzene.lmpdat`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mcif` & `openprattle-1.1.0/test/data/Benzene.mcif`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mdl` & `openprattle-1.1.0/test/data/Benzene.mdl`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.ml2` & `openprattle-1.1.0/test/data/Benzene.ml2`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mmcif` & `openprattle-1.1.0/test/data/Benzene.mmcif`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mmd` & `openprattle-1.1.0/test/data/Benzene.mmd`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mmod` & `openprattle-1.1.0/test/data/Benzene.mmod`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mol` & `openprattle-1.1.0/test/data/Benzene.mol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mol2` & `openprattle-1.1.0/test/data/Benzene.mol2`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mold` & `openprattle-1.1.0/test/data/Benzene.mold`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.molden` & `openprattle-1.1.0/test/data/Benzene.molden`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.molf` & `openprattle-1.1.0/test/data/Benzene.molf`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.molreport` & `openprattle-1.1.0/test/data/Benzene.molreport`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mopin` & `openprattle-1.1.0/test/data/Benzene.mopin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mp` & `openprattle-1.1.0/test/data/Benzene.mp`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.mrv` & `openprattle-1.1.0/test/data/Benzene.mrv`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.nw` & `openprattle-1.1.0/test/data/Benzene.nw`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.orcainp` & `openprattle-1.1.0/test/data/Benzene.orcainp`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.outmol` & `openprattle-1.1.0/test/data/Benzene.outmol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.paint` & `openprattle-1.1.0/test/data/Benzene.paint`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pcjson` & `openprattle-1.1.0/test/data/Benzene.pcjson`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pcm` & `openprattle-1.1.0/test/data/Benzene.pcm`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pdb` & `openprattle-1.1.0/test/data/Benzene.pdb`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pdbqt` & `openprattle-1.1.0/test/data/Benzene.pdbqt`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.png` & `openprattle-1.1.0/test/data/Benzene.png`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pointcloud` & `openprattle-1.1.0/test/data/Benzene.pointcloud`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pov` & `openprattle-1.1.0/test/data/Benzene.pov`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pqr` & `openprattle-1.1.0/test/data/Benzene.pqr`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.pqs` & `openprattle-1.1.0/test/data/Benzene.pqs`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.report` & `openprattle-1.1.0/test/data/Benzene.report`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.sd` & `openprattle-1.1.0/test/data/Benzene.sd`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.sdf` & `openprattle-1.1.0/test/data/Benzene.sdf`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.stl` & `openprattle-1.1.0/test/data/Benzene.stl`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.svg` & `openprattle-1.1.0/test/data/Benzene.svg`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.sy2` & `openprattle-1.1.0/test/data/Benzene.sy2`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.tmol` & `openprattle-1.1.0/test/data/Benzene.tmol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.txyz` & `openprattle-1.1.0/test/data/Benzene.txyz`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.unixyz` & `openprattle-1.1.0/test/data/Benzene.unixyz`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.vmol` & `openprattle-1.1.0/test/data/Benzene.vmol`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.xed` & `openprattle-1.1.0/test/data/Benzene.xed`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.xyz` & `openprattle-1.1.0/test/data/Benzene.xyz`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.yob` & `openprattle-1.1.0/test/data/Benzene.yob`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/test/data/Benzene.zin` & `openprattle-1.1.0/test/data/Benzene.zin`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/.gitignore` & `openprattle-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/LICENSE` & `openprattle-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/README.md` & `openprattle-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openprattle-1.0.2/pyproject.toml` & `openprattle-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openprattle"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
     {name = "Oliver S. Lee", email = "osl@digi-chem.ac.uk"},
 ]
 description = "A convenience wrapper for seamlessly accessing the pybel library and obabel command-line tools"
 dependencies = [
     "openbabel >= 3.0.0"
 ]
@@ -21,8 +21,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/Digichem-Project/openprattle"
 Issues = "https://github.com/Digichem-Project/openprattle/issues"
 
 [project.scripts]
-oprattle = "openprattle.program:main"
+oprattle = "openprattle.program:main"
```

### Comparing `openprattle-1.0.2/PKG-INFO` & `openprattle-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprattle
-Version: 1.0.2
+Version: 1.1.0
 Summary: A convenience wrapper for seamlessly accessing the pybel library and obabel command-line tools
 Project-URL: Homepage, https://github.com/Digichem-Project/openprattle
 Project-URL: Issues, https://github.com/Digichem-Project/openprattle/issues
 Author-email: "Oliver S. Lee" <osl@digi-chem.ac.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

