# Comparing `tmp/patcherex2-0.1.9.tar.gz` & `tmp/patcherex2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patcherex2-0.1.9.tar", last modified: Tue Feb 27 22:54:40 2024, max compression
+gzip compressed data, was "patcherex2-0.2.0.tar", last modified: Thu May 30 01:35:46 2024, max compression
```

## Comparing `patcherex2-0.1.9.tar` & `patcherex2-0.2.0.tar`

### file list

```diff
@@ -1,102 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.044432 patcherex2-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-27 22:54:30.000000 patcherex2-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-27 22:54:40.044432 patcherex2-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-27 22:54:30.000000 patcherex2-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-27 22:54:34.000000 patcherex2-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 22:54:40.044432 patcherex2-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.028432 patcherex2-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.028432 patcherex2-0.1.9/src/patcherex2/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.028432 patcherex2-0.1.9/src/patcherex2/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.032432 patcherex2-0.1.9/src/patcherex2/components/allocation_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/allocation_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/allocation_managers/allocation_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.032432 patcherex2-0.1.9/src/patcherex2/components/assemblers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/bcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/keystone.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/keystone_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/keystone_sparc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assemblers/ppc_vle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.032432 patcherex2-0.1.9/src/patcherex2/components/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/assets/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.032432 patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/angr.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/binary_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.032432 patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/binfmt_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/ihex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.036432 patcherex2-0.1.9/src/patcherex2/components/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/bcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/clang.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/clang_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/llvm_recomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/llvm_recomp_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/compilers/ppc_vle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.036432 patcherex2-0.1.9/src/patcherex2/components/disassemblers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/disassemblers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/disassemblers/capstone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/disassemblers/capstone_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/disassemblers/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/disassemblers/ppc_vle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.036432 patcherex2-0.1.9/src/patcherex2/components/patch_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/patch_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/patch_managers/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/patch_managers/imp.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/patch_managers/patch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.036432 patcherex2-0.1.9/src/patcherex2/components/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/components/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patcherex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.040432 patcherex2-0.1.9/src/patcherex2/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/data_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/dummy_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/function_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/instruction_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/patches/raw_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.044432 patcherex2-0.1.9/src/patcherex2/targets/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_aarch64_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_arm_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_arm_linux_recomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_arm_mimxrt1052.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_i386_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_leon3_bare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_mips64_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_mips64el_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_mips_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_mipsel_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_ppc64_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_ppc64le_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_ppc_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_x86_64_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/elf_x86_64_linux_recomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/ihex_ppc_bare.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-27 22:54:30.000000 patcherex2-0.1.9/src/patcherex2/targets/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.044432 patcherex2-0.1.9/src/patcherex2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-27 22:54:40.000000 patcherex2-0.1.9/src/patcherex2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-02-27 22:54:40.000000 patcherex2-0.1.9/src/patcherex2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 22:54:40.000000 patcherex2-0.1.9/src/patcherex2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-27 22:54:40.000000 patcherex2-0.1.9/src/patcherex2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 22:54:40.000000 patcherex2-0.1.9/src/patcherex2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:54:40.044432 patcherex2-0.1.9/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9675 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_aarch64.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10341 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_i386.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_mips.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_mips64.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_mips64el.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_mipsel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_ppc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_ppc64.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_ppc64le.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-02-27 22:54:30.000000 patcherex2-0.1.9/tests/test_x86_64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.953494 patcherex2-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 01:35:43.000000 patcherex2-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-30 01:35:46.953494 patcherex2-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-30 01:35:43.000000 patcherex2-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 01:35:44.000000 patcherex2-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:35:46.953494 patcherex2-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.933494 patcherex2-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.937494 patcherex2-0.2.0/src/patcherex2/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.933494 patcherex2-0.2.0/src/patcherex2/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.937494 patcherex2-0.2.0/src/patcherex2/components/allocation_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/allocation_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/allocation_managers/allocation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.941494 patcherex2-0.2.0/src/patcherex2/components/archinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/aarch64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/amd64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/mips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/mips64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/ppc64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/ppc_vle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/sparc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/archinfo/x86.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.941494 patcherex2-0.2.0/src/patcherex2/components/assemblers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/bcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/keystone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/keystone_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/keystone_sparc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assemblers/ppc_vle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.941494 patcherex2-0.2.0/src/patcherex2/components/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/assets/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.941494 patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/angr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/binary_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.941494 patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/binfmt_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21601 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/ihex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.945494 patcherex2-0.2.0/src/patcherex2/components/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/bcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/clang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/clang_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/llvm_recomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/llvm_recomp_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/compilers/ppc_vle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.945494 patcherex2-0.2.0/src/patcherex2/components/disassemblers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/disassemblers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/disassemblers/capstone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/disassemblers/capstone_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/disassemblers/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/disassemblers/ppc_vle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.945494 patcherex2-0.2.0/src/patcherex2/components/patch_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/patch_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/patch_managers/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/patch_managers/imp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/patch_managers/patch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.945494 patcherex2-0.2.0/src/patcherex2/components/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/utils/linker_script_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/components/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patcherex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.949494 patcherex2-0.2.0/src/patcherex2/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/data_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/dummy_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/function_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/instruction_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/patches/raw_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.949494 patcherex2-0.2.0/src/patcherex2/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_aarch64_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_amd64_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_amd64_linux_recomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_arm_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_arm_linux_recomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_arm_mimxrt1052.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_leon3_bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_mips64_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_mips64el_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_mips_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_mipsel_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_ppc64_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_ppc64le_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_ppc_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/elf_x86_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/ihex_ppc_bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-30 01:35:43.000000 patcherex2-0.2.0/src/patcherex2/targets/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.953494 patcherex2-0.2.0/src/patcherex2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-30 01:35:46.000000 patcherex2-0.2.0/src/patcherex2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-30 01:35:46.000000 patcherex2-0.2.0/src/patcherex2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:35:46.000000 patcherex2-0.2.0/src/patcherex2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 01:35:46.000000 patcherex2-0.2.0/src/patcherex2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 01:35:46.000000 patcherex2-0.2.0/src/patcherex2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:35:46.953494 patcherex2-0.2.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17393 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_aarch64.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10330 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_i386.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_mips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_mips64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_mips64el.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_mipsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_ppc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_ppc64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_ppc64le.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18254 2024-05-30 01:35:43.000000 patcherex2-0.2.0/tests/test_x86_64.py
```

### Comparing `patcherex2-0.1.9/LICENSE` & `patcherex2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/PKG-INFO` & `patcherex2-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,69 @@
-Metadata-Version: 2.1
-Name: patcherex2
-Version: 0.1.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: angr
-Requires-Dist: pyelftools
-Requires-Dist: lief
-Requires-Dist: keystone-engine
-Requires-Dist: intelhex
-Requires-Dist: requests
-
-# Patcherex 2
+# Patcherex2
 
 [![Latest Release](https://img.shields.io/pypi/v/patcherex2.svg)](https://pypi.python.org/pypi/patcherex2/)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/patcherex2.svg)](https://pypistats.org/packages/patcherex2)
 [![CI](https://img.shields.io/github/actions/workflow/status/purseclab/patcherex2/ci.yml?label=CI
 )](https://github.com/purseclab/Patcherex2/actions/workflows/test.yml)
 [![License](https://img.shields.io/github/license/purseclab/patcherex2.svg)](https://github.com/purseclab/Patcherex2/blob/main/LICENSE)
 
-> [!WARNING]
-> This project is currently in its initial development stages. Please anticipate potential breaking changes. The first stable release is targeted for early March 2024.
-
-Patcherex 2 is a rewritten adaptation of the original [Patcherex](https://github.com/angr/patcherex) project, aimed at building upon its core ideas and extending its capabilities.
+Patcherex2 is a rewritten adaptation of the original [Patcherex](https://github.com/angr/patcherex) project, aimed at building upon its core ideas and extending its capabilities.
 
 ## Installation
 
-Patcherex 2 is available on PyPI and can be installed with pip:
+Patcherex2 is available on PyPI and can be installed using pip. Alternatively, you can use the provided Docker image.
 
+### pip
 ```bash
 pip install patcherex2
 ```
+<details>
+<summary>Install from latest commit</summary>
+
+```bash
+pip install git+https://github.com/purseclab/Patcherex2.git
+```
+</details>
+
+### Docker
+```bash
+docker run --rm -it -v ${PWD}:/workdir -w /workdir ghcr.io/purseclab/patcherex2
+```
+
+<details>
+<summary>Build from latest commit</summary>
+
+```bash
+docker build -t patcherex2 --platform linux/amd64 https://github.com/purseclab/Patcherex2.git
+docker run --rm -it -v ${PWD}:/workdir -w /workdir patcherex2
+```
+</details>
+
 
 ## Usage
+You can find usage examples [here](https://purseclab.github.io/Patcherex2/examples/insert_instruction_patch/).
+
+
+## Documentation
+General documentation and API reference for Patcherex2 can be found at [purseclab.github.io/Patcherex2](https://purseclab.github.io/Patcherex2/).
 
-Coming soon.
 
 ## Supported Targets
 
 |           | Linux x86 | Linux amd64 | Linux arm | Linux aarch64 | Linux PowerPC (32bit) | Linux PowerPC (64bit) | Linux PowerPCle (64bit) | Linux MIPS (32bit) | Linux MIPS (64bit) | Linux MIPSEL<br>​(32bit) | Linux MIPSEL<br>(64bit) | SPARCv8 (LEON3) | PowerPC (VLE) (IHEX)
 |-|-|-|-|-|-|-|-|-|-|-|-|-|-|
-InsertDataPatch         | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-RemoveDataPatch         | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-ModifyDataPatch         | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-InsertInstructionPatch  | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-RemoveInstructionPatch  | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-ModifyInstructionPatch  | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-InsertFunctionPatch     | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
-ModifyFunctionPatch     | 🟨 | 🟩 | 🟩 | 🟩 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | ⬜ | ⬜ |
+InsertDataPatch              | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+RemoveDataPatch              | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+ModifyDataPatch              | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+InsertInstructionPatch (ASM) | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+InsertInstructionPatch (C)   | 🟥 | 🟩 | 🟥 | 🟨 | 🟥 | 🟥 | 🟥 | 🟥 | 🟥 | 🟥 | 🟥 | 🟥 | 🟥 |
+RemoveInstructionPatch       | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+ModifyInstructionPatch       | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+InsertFunctionPatch          | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 | ⬜ | ⬜ |
+ModifyFunctionPatch          | 🟨 | 🟩 | 🟩 | 🟩 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | 🟨 | ⬜ | ⬜ |
 
 🟩 Fully Functional, 🟨 Limited Functionality, 🟥 Not Working, ⬜ Not Tested, 🟪 Work in Progress
+
+
+## Acknowledgements
+This project was developed as part of the [DARPA AMP](https://www.darpa.mil/program/assured-micropatching) program, under contract N6600120C4031.
+
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/allocation_managers/allocation_manager.py` & `patcherex2-0.2.0/src/patcherex2/components/allocation_managers/allocation_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import enum
 import logging
-from typing import List
 
 logger = logging.getLogger(__name__)
 
 
 class Block:
     subclasses = []
 
@@ -13,21 +14,21 @@
         Block.subclasses.append(cls)
 
     def __init__(self, addr: int, size: int, is_free=True) -> None:
         self.addr = addr
         self.size = size
         self.is_free = is_free
 
-    def __lt__(self, other: "Block") -> bool:
+    def __lt__(self, other: Block) -> bool:
         return self.addr < other.addr
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} addr={hex(self.addr)} size={hex(self.size)} is_free={self.is_free}>"
 
-    def coalesce(self, other: "Block") -> bool:
+    def coalesce(self, other: Block) -> bool:
         if self.is_free == other.is_free and self.addr + self.size == other.addr:
             self.size += other.size
             return True
         return False
 
 
 class FileBlock(Block):
@@ -57,21 +58,21 @@
         self, file_addr: int, mem_addr: int, size: int, is_free=True, flag=None
     ) -> None:
         super().__init__(None, size, is_free)
         self.file_addr = file_addr
         self.mem_addr = mem_addr
         self.flag = flag
 
-    def __lt__(self, other: "MappedBlock") -> bool:
+    def __lt__(self, other: MappedBlock) -> bool:
         return self.mem_addr < other.mem_addr
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} file_addr={hex(self.file_addr)} mem_addr={hex(self.mem_addr)} size={hex(self.size)} is_free={self.is_free} flag={str(self.flag)}>"
 
-    def coalesce(self, other: "MappedBlock") -> bool:
+    def coalesce(self, other: MappedBlock) -> bool:
         if (
             self.flag == other.flag
             and self.is_free == other.is_free
             and self.file_addr + self.size == other.file_addr
             and self.mem_addr + self.size == other.mem_addr
         ):
             self.size += other.size
@@ -150,32 +151,43 @@
             if best_fit.size == 0:
                 self.blocks[MappedBlock].remove(best_fit)
             return allocated_block
 
     def _create_new_mapped_block(
         self, size: int, flag=MemoryFlag.RWX, align=0x1
     ) -> bool:
-        # map 0x1000 bytes # TODO: currently we won't use available file/mem blocks, instead we create new one at the end of the file
+        # TODO: currently we won't use available file/mem blocks, instead we create new one at the end of the file
         file_addr = None
         mem_addr = None
         for block in self.blocks[FileBlock]:
             if block.size == -1:
                 file_addr = block.addr
-                block.addr += 0x1000
+                block.addr += 0x2000
         for block in self.blocks[MemoryBlock]:
             if block.size == -1:
-                # mem_addr % 0x1000 should equal to file_addr % 0x1000 TODO
-                mem_addr = block.addr + (file_addr % 0x1000)
-                block.addr = mem_addr + 0x1000
+                # NOTE: mem_addr % p_align should equal to file_addr % p_align
+                # Check `man elf` and search for `p_align` for more information
+                # FIXME: shouldn't do any assumption on component type, reimpl in a better way
+                # FIXME: even worse, importing ELF will cause circular import
+                # TODO: consider merge allocation_manager and binfmt_tool into one component
+                if self.p.binfmt_tool.__class__.__name__ == "ELF":
+                    max_seg_align = max(
+                        [segment["p_align"] for segment in self.p.binfmt_tool._segments]
+                        + [0]
+                    )
+                    mem_addr = block.addr + (file_addr % max_seg_align)
+                else:
+                    mem_addr = block.addr + (file_addr % 0x1000)
+                block.addr = mem_addr + 0x2000
         if file_addr and mem_addr:
             self.add_block(
-                MappedBlock(file_addr, mem_addr, 0x1000, is_free=True, flag=flag)
+                MappedBlock(file_addr, mem_addr, 0x2000, is_free=True, flag=flag)
             )
             self.new_mapped_blocks.append(
-                MappedBlock(file_addr, mem_addr, 0x1000, is_free=True, flag=flag)
+                MappedBlock(file_addr, mem_addr, 0x2000, is_free=True, flag=flag)
             )
             return True
         return False
 
     def allocate(self, size: int, flag=MemoryFlag.RWX, align=0x1) -> MappedBlock:
         logger.debug(
             f"allocating size: {size}, flag: {flag.__repr__()}, align: {align}"
@@ -191,15 +203,15 @@
         else:
             raise MemoryError("Insufficient memory")
 
     def free(self, block: Block) -> None:
         block.is_free = True
         self.coalesce(self.blocks[type(block)])
 
-    def coalesce(self, blocks: List[Block]) -> None:
+    def coalesce(self, blocks: list[Block]) -> None:
         for curr, next in zip(blocks, blocks[1:]):
             if curr.coalesce(next):
                 blocks.remove(next)
                 self.coalesce(blocks)
                 return
 
     def finalize(self) -> None:
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assemblers/assembler.py` & `patcherex2-0.2.0/src/patcherex2/components/assemblers/assembler.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     def _assemble(self, code: str, base=0, **kwargs) -> None:
         raise NotImplementedError()
 
     def _pre_assemble_hook(self, code: str, base=0) -> None:
         return code
 
     def assemble(self, code: str, base=0, symbols=None, **kwargs) -> None:
+        if code == "":
+            return b""
         if symbols is None:
             symbols = {}
         logger.debug(f"Assembling `{code}` at {hex(base)}")
         code = self.resolve_symbols(code, symbols=symbols)
         code = self._pre_assemble_hook(code, base=base)
 
         return self._assemble(code, base=base, **kwargs)
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assemblers/bcc.py` & `patcherex2-0.2.0/src/patcherex2/components/assemblers/bcc.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assemblers/keystone_arm.py` & `patcherex2-0.2.0/src/patcherex2/components/assemblers/keystone_arm.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assemblers/keystone_sparc.py` & `patcherex2-0.2.0/src/patcherex2/components/assemblers/keystone_sparc.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assemblers/ppc_vle.py` & `patcherex2-0.2.0/src/patcherex2/components/assemblers/ppc_vle.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/assets/assets.py` & `patcherex2-0.2.0/src/patcherex2/components/assets/assets.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/angr.py` & `patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/angr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
 import logging
-from typing import Dict, List, Optional, Union
 
 import angr
 from archinfo import ArchARM
 
 from .binary_analyzer import BinaryAnalyzer
 
 logger = logging.getLogger(__name__)
 
 
 class Angr(BinaryAnalyzer):
     def __init__(self, binary_path: str, **kwargs) -> None:
         self.binary_path = binary_path
         # self.use_pickle = kwargs.pop("use_pickle", False) # TODO: implement this
         self.angr_kwargs = kwargs.pop("angr_kwargs", {})
+        self.angr_cfg_kwargs = kwargs.pop("angr_cfg_kwargs", {})
         self._p = None
         self._cfg = None
         self._load_base = None
 
     @property
     def load_base(self) -> int:
         if self._load_base is None:
@@ -44,57 +46,78 @@
             logger.info("Loaded binary with angr")
         return self._p
 
     @property
     def cfg(self) -> angr.analyses.cfg.cfg_fast.CFGFast:
         if self._cfg is None:
             logger.info("Generating CFG with angr")
-            self._cfg = self.p.analyses.CFGFast(
-                normalize=True, data_references=True, force_complete_scan=False
-            )
+            if "normalize" not in self.angr_cfg_kwargs:
+                # NOTE: This will split basic blocks if another block jumps to the middle of the block
+                self.angr_cfg_kwargs["normalize"] = True
+            self._cfg = self.p.analyses.CFGFast(**self.angr_cfg_kwargs)
             logger.info("Generated CFG with angr")
         return self._cfg
 
     def mem_addr_to_file_offset(self, addr: int) -> int:
         addr = self.denormalize_addr(addr)
         file_addr = self.p.loader.main_object.addr_to_offset(addr)
         if file_addr is None:
             logger.error(
                 f"Cannot convert memory address {hex(addr)} to file offset, will use the memory address instead"
             )
             return addr
         return file_addr
 
-    def get_basic_block(self, addr: int) -> Dict[str, Union[int, List[int]]]:
+    def get_basic_block(self, addr: int) -> dict[str, int | list[int]]:
+        # NOTE: angr splits basic blocks at call instructions, so we need to handle this
         if self.is_thumb(addr):
             addr += 1
         addr = self.denormalize_addr(addr)
-        bb = None
-        for node in self.cfg.model.nodes():
-            if addr in node.instruction_addrs:
-                bb = node
-                break
-        assert bb is not None
-        return {
-            "start": self.normalize_addr(bb.addr),
-            "end": self.normalize_addr(bb.addr + bb.size),
-            "size": bb.size,
-            "instruction_addrs": [
-                self.normalize_addr(addr)
-                - (1 if self.is_thumb(self.normalize_addr(addr)) else 0)
-                for addr in bb.instruction_addrs
-            ],
-        }
 
-    def get_instr_bytes_at(self, addr: int) -> angr.Block:
+        func = self.p.kb.functions.function(
+            self.cfg.model.get_any_node(addr, anyaddr=True).function_address
+        )
+        ri = self.p.analyses.RegionIdentifier(func)
+        graph = ri._graph.copy()
+        ri._make_supergraph(graph)
+
+        for multinode in graph.nodes():
+            nodes = multinode.nodes if hasattr(multinode, "nodes") else [multinode]
+            start = multinode.addr
+            size = sum(node.size for node in nodes)
+            end = start + size
+
+            instr_addrs = [
+                instr_addr
+                for node in nodes
+                for instr_addr in func.get_block(node.addr).instruction_addrs
+            ]
+
+            if addr in instr_addrs:
+                return {
+                    "start": self.normalize_addr(start),
+                    "end": self.normalize_addr(end),
+                    "size": size,
+                    "instruction_addrs": [
+                        self.normalize_addr(instr_addr)
+                        - (1 if self.is_thumb(self.normalize_addr(instr_addr)) else 0)
+                        for instr_addr in instr_addrs
+                    ],
+                }
+
+        raise Exception(f"Cannot find a block containing address {hex(addr)}")
+
+    def get_instr_bytes_at(self, addr: int, num_instr=1) -> angr.Block:
         addr += 1 if self.is_thumb(addr) else 0
         addr = self.denormalize_addr(addr)
-        return self.p.factory.block(addr, num_inst=1).bytes
+        # TODO: Special handling for delay slot, when there is a call instr with delay slot
+        # angr will return both instrs, even when num_instr is 1
+        return self.p.factory.block(addr, num_inst=num_instr).bytes
 
-    def get_unused_funcs(self) -> List[Dict[str, int]]:
+    def get_unused_funcs(self) -> list[dict[str, int]]:
         logger.info("Getting unused functions with angr")
         unused_funcs = []
         assert self.cfg is not None
         for func in self.p.kb.functions.values():
             if func.size == 0:
                 continue
             for dst, _ in self.p.kb.xrefs.xrefs_by_dst.items():
@@ -106,29 +129,29 @@
                         "addr": self.normalize_addr(func.addr)
                         - (1 if self.is_thumb(self.normalize_addr(func.addr)) else 0),
                         "size": func.size,
                     }
                 )
         return unused_funcs
 
-    def get_all_symbols(self) -> Dict[str, int]:
+    def get_all_symbols(self) -> dict[str, int]:
         assert self.cfg is not None
         logger.info("Getting all symbols with angr")
         symbols = {}
         for symbol in self.p.loader.main_object.symbols:
             if not symbol.name or not symbol.is_function:
                 continue
             symbols[symbol.name] = self.normalize_addr(symbol.rebased_addr)
         for func in self.p.kb.functions.values():
             if func.is_simprocedure or func.is_alignment:
                 continue
             symbols[func.name] = self.normalize_addr(func.addr)
         return symbols
 
-    def get_function(self, name_or_addr: Union[int, str]) -> Optional[Dict[str, int]]:
+    def get_function(self, name_or_addr: int | str) -> dict[str, int] | None:
         assert self.cfg is not None
         if isinstance(name_or_addr, (str, int)):
             if isinstance(name_or_addr, int):
                 name_or_addr += 1 if self.is_thumb(name_or_addr) else 0
                 name_or_addr = self.denormalize_addr(name_or_addr)
             if name_or_addr in self.p.kb.functions:
                 func = self.p.kb.functions[name_or_addr]
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/binary_analyzers/ida.py` & `patcherex2-0.2.0/src/patcherex2/components/binary_analyzers/ida.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+from __future__ import annotations
 
 from headless_ida import HeadlessIdaRemote
 
 from .binary_analyzer import BinaryAnalyzer
 
 
 class Ida(BinaryAnalyzer):
@@ -40,15 +40,15 @@
         ]
         for lib in ida_libs:
             setattr(self, lib, self._headlessida.import_module(lib))
 
     def mem_addr_to_file_offset(self, addr: int) -> int:
         return self.ida_loader.get_fileregion_offset(addr)
 
-    def get_basic_block(self, addr: int) -> Dict[str, Union[int, List[int]]]:
+    def get_basic_block(self, addr: int) -> dict[str, int | list[int]]:
         func = self.ida_funcs.get_func(addr)
         instr_addrs = list(func.code_items())
         assert addr in instr_addrs, "Invalid address"
         flowchart = self.ida_gdl.FlowChart(f=func, flags=self.ida_gdl.FC_PREDS)
 
         for block in flowchart:
             if block.start_ea <= addr < block.end_ea:
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/binfmt_tool.py` & `patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/binfmt_tool.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/elf.py` & `patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/elf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import logging
 import os
-from typing import Optional
 
 from elftools.construct.lib import Container
 from elftools.elf.constants import P_FLAGS, SH_FLAGS
 from elftools.elf.elffile import ELFFile
 
 from ..allocation_managers.allocation_manager import (
     FileBlock,
@@ -181,15 +182,17 @@
             key=lambda x: x["p_offset"],
         )
 
         block = FileBlock(self.file_size, -1)
         self.p.allocation_manager.add_block(block)
 
         addr = load_segments[-1]["p_vaddr"] + load_segments[-1]["p_memsz"]
-        addr = (addr + 0xFFF) & ~0xFFF  # round up to 0x1000
+        # TODO: should we use the max_align of the segments?
+        max_align = max([segment["p_align"] for segment in self._segments] + [0])
+        addr = (addr + (max_align - 1)) & ~(max_align - 1)  # round up to max_align
         block = MemoryBlock(addr, -1)
         self.p.allocation_manager.add_block(block)
 
     def _init_memory_analysis(self) -> None:
         self._find_space_between_sections()
         self._find_space_between_segments()
         self._add_end_of_file_block()
@@ -338,40 +341,41 @@
                     "p_flags": 0x4,
                     "p_align": 0x1000,
                 }
             )
             self._segments.append(phdr_load_segment)
 
             # magic
+            # TODO: should we use the max_align of the segments?
             load_segments_rounded = []
             first_load_segment = None
             for segment in self._segments:
                 if segment["p_type"] == "PT_LOAD":
                     if first_load_segment is None:
                         first_load_segment = segment
                     load_segments_rounded.append(
                         (
-                            # start of the segment, round down to multiple of 0x1000
+                            # start of the segment, round down to multiple of max_align
                             (segment["p_vaddr"] - first_load_segment["p_vaddr"])
                             - (
                                 (segment["p_vaddr"] - first_load_segment["p_vaddr"])
-                                % 0x1000
+                                % max_align
                             ),
-                            # end of the segment, round up to multiple of 0x1000
+                            # end of the segment, round up to multiple of max_align
                             int(
                                 (
                                     segment["p_vaddr"]
                                     + segment["p_memsz"]
                                     - first_load_segment["p_vaddr"]
-                                    + 0x1000
+                                    + max_align
                                     - 1
                                 )
-                                / 0x1000
+                                / max_align
                             )
-                            * 0x1000,
+                            * max_align,
                         )
                     )
             load_segments_rounded = sorted(load_segments_rounded, key=lambda x: x[0])
 
             # combine overlapping load segments
             while True:
                 new_load_segments_rounded = []
@@ -398,33 +402,35 @@
                 load_segments_rounded = (
                     new_load_segments_rounded  # combined segments, run again
                 )
 
             for prev_seg, next_seg in zip(
                 load_segments_rounded[:-1], load_segments_rounded[1:]
             ):
+                # TODO: should we use the max_align of the segments?
                 potential_base = (
-                    max(prev_seg[1], self.p.binfmt_tool.file_size) + 0xFFF
-                ) & ~0xFFF  # round up to 0x1000
+                    max(prev_seg[1], self.p.binfmt_tool.file_size) + (max_align - 1)
+                ) & ~(max_align - 1)  # round up to max_align
                 if next_seg[0] - potential_base > self._elf.header["e_phentsize"] * len(
                     self._segments
                 ):  # if there is space between segments, put phdr here
                     phdr_start = potential_base
                     break
             else:
                 phdr_start = load_segments_rounded[-1][
                     1
                 ]  # otherwise put it after the last load segment
             # this is to workaround a weird issue in the dynamic linker of glibc
             # we want to make sure p_vaddr (phdr_start) == p_offset (len(ncontent))
             if phdr_start <= self.p.binfmt_tool.file_size:
+                # TODO: should we use the max_align of the segments?
                 # p_vaddr <= p_offset: pad the file (p_offset) to page size, and let p_vaddr = p_offset
                 self.p.binfmt_tool.file_size = (
-                    self.p.binfmt_tool.file_size + 0xFFF
-                ) & ~0xFFF  # round up to 0x1000
+                    self.p.binfmt_tool.file_size + (max_align - 1)
+                ) & ~(max_align - 1)  # round up to max_align
                 phdr_start = self.p.binfmt_tool.file_size
 
             # update phdr segment and its corresponding load segment
             for segment in self._segments:
                 if segment["p_type"] == "PT_PHDR" or segment == phdr_load_segment:
                     segment["p_filesz"] = self._elf.header["e_phentsize"] * len(
                         self._segments
@@ -448,15 +454,15 @@
 
             ehdr = self._elf.header
             ehdr["e_phnum"] = len(self._segments)
             ehdr["e_phoff"] = phdr_start
             new_ehdr = self._elf.structs.Elf_Ehdr.build(ehdr)
             self.p.binfmt_tool.update_binary_content(0, new_ehdr)
 
-    def save_binary(self, filename: Optional[str] = None) -> None:
+    def save_binary(self, filename: str | None = None) -> None:
         self.updated_binary_content = self.updated_binary_content.ljust(
             self.file_size, b"\x00"
         )
         for update in self.file_updates:
             self.updated_binary_content = (
                 self.updated_binary_content[: update["offset"]]
                 + update["content"]
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/binfmt_tools/ihex.py` & `patcherex2-0.2.0/src/patcherex2/components/binfmt_tools/ihex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import io
 import logging
-from typing import Optional
 
 import intelhex
 
 from .binfmt_tool import BinFmtTool
 
 logger = logging.getLogger(__name__)
 
@@ -22,15 +23,15 @@
 
     def _init_memory_analysis(self) -> None:
         pass
 
     def finalize(self) -> None:
         pass
 
-    def save_binary(self, filename: Optional[str] = None) -> None:
+    def save_binary(self, filename: str | None = None) -> None:
         for update in self.file_updates:
             self._ihex.puts(update["offset"], update["content"])
         if filename is None:
             filename = f"{self.binary_path}.patched"
         sio = io.StringIO()
         self._ihex.write_hex_file(sio, byte_count=0x20)
         final_content = sio.getvalue()
@@ -60,10 +61,22 @@
                 raise ValueError(
                     f"Cannot update offset {hex(offset)} with content {new_content}, it overlaps with a previous update"
                 )
         self.file_updates.append({"offset": offset, "content": new_content})
         if offset + len(new_content) > self.file_size:
             self.file_size = offset + len(new_content)
 
+    def get_binary_content(self, offset: int, size: int) -> bytes:
+        # check if it's in the file updates
+        for update in self.file_updates:
+            if offset >= update["offset"] and offset + size <= update["offset"] + len(
+                update["content"]
+            ):
+                return update["content"][
+                    offset - update["offset"] : offset - update["offset"] + size
+                ]
+        # otherwise read from the file
+        return self._ihex.tobinarray(start=offset, size=size)
+
     def append_to_binary_content(self, new_content: bytes) -> None:
         self.file_updates.append({"offset": self.file_size, "content": new_content})
         self.file_size += len(new_content)
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/compilers/clang_arm.py` & `patcherex2-0.2.0/src/patcherex2/components/compilers/clang_arm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+from __future__ import annotations
+
 import logging
-from typing import Dict, List, Optional
 
 from .compiler import Compiler
 
 logger = logging.getLogger(__name__)
 
 
 class ClangArm(Compiler):
     def __init__(
-        self, p, clang_version=15, compiler_flags: Optional[List[str]] = None
+        self, p, clang_version=15, compiler_flags: list[str] | None = None
     ) -> None:
         super().__init__(p)
         if compiler_flags is None:
             compiler_flags = []
         self._compiler = f"clang-{clang_version}"
         self._linker = f"ld.lld-{clang_version}"
         self._compiler_flags = compiler_flags
 
     def compile(
         self,
         code: str,
         base=0,
-        symbols: Optional[Dict[str, int]] = None,
-        extra_compiler_flags: Optional[List[str]] = None,
+        symbols: dict[str, int] | None = None,
+        extra_compiler_flags: list[str] | None = None,
         is_thumb=False,
         **kwargs,
     ) -> bytes:
         if symbols is None:
             symbols = {}
         if extra_compiler_flags is None:
             extra_compiler_flags = []
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/compilers/llvm_recomp.py` & `patcherex2-0.2.0/src/patcherex2/components/compilers/llvm_recomp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,50 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
 import subprocess
 import tempfile
-from typing import Dict, List, Optional
 
 import cle
+from elftools.elf.elffile import ELFFile
 
 from ..assets.assets import Assets
 from .clang import Clang
 
 logger = logging.getLogger(__name__)
 
 
 class LLVMRecomp(Clang):
     def __init__(
-        self, p, clang_version=15, compiler_flags: Optional[List[str]] = None
+        self, p, clang_version=15, compiler_flags: list[str] | None = None
     ) -> None:
         super().__init__(p, clang_version, compiler_flags)
         self._clang_version = clang_version
         self._assets_path = Assets("llvm_recomp").path
 
     def compile(
         self,
         code: str,
         base=0,
-        symbols: Optional[Dict[str, int]] = None,
-        extra_compiler_flags: Optional[List[str]] = None,
+        symbols: dict[str, int] | None = None,
+        extra_compiler_flags: list[str] | None = None,
         is_thumb=False,
         **kwargs,
     ) -> bytes:
         if symbols is None:
             symbols = {}
         if extra_compiler_flags is None:
             extra_compiler_flags = []
         with tempfile.TemporaryDirectory() as td:
             # source file
             with open(os.path.join(td, "code.c"), "w") as f:
                 f.write(code)
 
-            # linker script
-            _symbols = {}
-            _symbols.update(self.p.symbols)
-            _symbols.update(self.p.binary_analyzer.get_all_symbols())
-            _symbols.update(symbols)
-            linker_script = (
-                "SECTIONS { .text : SUBALIGN(0) { . = "
-                + hex(base)
-                + "; *(.text) *(.rodata) "
-            )
-            for name, addr in _symbols.items():
-                linker_script += name + " = " + hex(addr) + ";"
-            linker_script += "} /DISCARD/ : { *(.eh_frame) } }"
-            with open(os.path.join(td, "linker.ld"), "w") as f:
-                f.write(linker_script)
-
             librecomp_path = os.path.join(self._assets_path, "libRecompiler.so")
 
             # c -> ll
             try:
                 args = (
                     [self._compiler]
                     + self._compiler_flags
@@ -155,14 +141,52 @@
                         "--filetype=obj",
                     ]
                     subprocess.run(args, check=True, capture_output=True)
                 except subprocess.CalledProcessError as e:
                     logger.error(e.stderr.decode("utf-8"))
                     raise e
 
+            # linker script
+            _symbols = {}
+            _symbols.update(self.p.symbols)
+            _symbols.update(self.p.binary_analyzer.get_all_symbols())
+            _symbols.update(symbols)
+
+            with open(os.path.join(td, "obj.o"), "rb") as f:
+                elf = ELFFile(f)
+                linker_script_rodata_sections = " ".join(
+                    [
+                        f". = ALIGN({section['sh_addralign']}); *({section.name})"
+                        for section in elf.iter_sections()
+                        if section.name.startswith(".rodata")
+                    ]
+                )
+
+                # automatically add symbols like off_deadbeef, dword_deadbeef, etc.
+                for sym in elf.get_section_by_name(".symtab").iter_symbols():
+                    if (
+                        sym.entry.st_shndx == "SHN_UNDEF"
+                        and sym.name
+                        and "_" in sym.name
+                    ):
+                        try:
+                            _, addr = sym.name.split("_", 1)
+                            addr = int(addr, 16)
+                            if sym.name not in _symbols:
+                                _symbols[sym.name] = addr
+                        except ValueError:
+                            pass
+            linker_script_symbols = "".join(
+                f"{name} = {hex(addr)};" for name, addr in _symbols.items()
+            )
+
+            linker_script = f"SECTIONS {{ .patcherex2 : SUBALIGN(0) {{ . = {hex(base)}; *(.text) {linker_script_rodata_sections} {linker_script_symbols} }} }}"
+            with open(os.path.join(td, "linker.ld"), "w") as f:
+                f.write(linker_script)
+
             # link object file
             try:
                 args = [self._linker] + [
                     "-relocatable",
                     os.path.join(td, "obj.o"),
                     "-T",
                     os.path.join(td, "linker.ld"),
@@ -174,11 +198,18 @@
                 logger.error(e.stderr.decode("utf-8"))
                 raise e
 
             # extract compiled code
             ld = cle.Loader(
                 os.path.join(td, "obj_linked.o"), main_opts={"base_addr": 0x0}
             )
+
+            patcherex2_section = next(
+                (s for s in ld.main_object.sections if s.name == ".patcherex2"), None
+            )
+            compiled_start = ld.all_objects[0].entry + base
+
             compiled = ld.memory.load(
-                ld.all_objects[0].entry + base, ld.memory.max_addr
+                compiled_start,
+                patcherex2_section.memsize - compiled_start,
             )
         return compiled
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/compilers/llvm_recomp_arm.py` & `patcherex2-0.2.0/src/patcherex2/components/compilers/llvm_recomp_arm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
+
 import logging
-from typing import Dict, List, Optional
 
 from .llvm_recomp import LLVMRecomp
 
 logger = logging.getLogger(__name__)
 
 
 class LLVMRecompArm(LLVMRecomp):
     def compile(
         self,
         code: str,
         base=0,
-        symbols: Optional[Dict[str, int]] = None,
-        extra_compiler_flags: Optional[List[str]] = None,
+        symbols: dict[str, int] | None = None,
+        extra_compiler_flags: list[str] | None = None,
         is_thumb=False,
         **kwargs,
     ) -> bytes:
         if symbols is None:
             symbols = {}
         if extra_compiler_flags is None:
             extra_compiler_flags = []
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/disassemblers/capstone.py` & `patcherex2-0.2.0/src/patcherex2/components/disassemblers/capstone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Dict, List, Union
+from __future__ import annotations
 
 import capstone
 
 from .disassembler import Disassembler
 
 
 class Capstone(Disassembler):
     def __init__(self, arch: int, mode: int) -> None:
         self.cs = capstone.Cs(arch, mode)
 
-    def disassemble(
-        self, input: bytes, base=0, **kwargs
-    ) -> List[Dict[str, Union[int, str]]]:
+    def disassemble(self, input: bytes, base=0, **kwargs) -> list[dict[str, int | str]]:
         cs_insns = self.cs.disasm(input, base)
         result = []
         for insn in cs_insns:
             result.append(
                 {
                     "address": insn.address,
                     "size": insn.size,
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/disassemblers/capstone_arm.py` & `patcherex2-0.2.0/src/patcherex2/components/disassemblers/capstone_arm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+from __future__ import annotations
 
 import capstone
 
 from .disassembler import Disassembler
 
 
 class CapstoneArm(Disassembler):
@@ -14,15 +14,15 @@
         self.cs_thumb = capstone.Cs(
             capstone.CS_ARCH_ARM,
             capstone.CS_MODE_THUMB + capstone.CS_MODE_LITTLE_ENDIAN,
         )
 
     def disassemble(
         self, input: bytes, base=0, is_thumb=False, **kwargs
-    ) -> List[Dict[str, Union[int, str]]]:
+    ) -> list[dict[str, int | str]]:
         cs = self.cs_thumb if is_thumb else self.cs_arm
         cs_insns = cs.disasm(input, base)
         result = []
         for insn in cs_insns:
             result.append(
                 {
                     "address": insn.address,
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/disassemblers/ppc_vle.py` & `patcherex2-0.2.0/src/patcherex2/components/disassemblers/ppc_vle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+from __future__ import annotations
+
 import logging
 import os
 import re
 import subprocess
 import tempfile
-from typing import Dict, List, Union
 
 from ..assets.assets import Assets
 from .disassembler import Disassembler
 
 logger = logging.getLogger(__name__)
 
 
 class PpcVle(Disassembler):
     def __init__(self, p) -> None:
         self.p = p
         self.assets_path = Assets("ppc_vle").path
 
-    def disassemble(
-        self, input: bytes, base=0, **kwargs
-    ) -> List[Dict[str, Union[str, int]]]:
+    def disassemble(self, input: bytes, base=0, **kwargs) -> list[dict[str, str | int]]:
         if isinstance(input, str):
             input = bytes(map(ord, input))
         with tempfile.TemporaryDirectory() as td:
             with open(os.path.join(td, "code.bin"), "wb") as f:
                 f.write(input)
 
             try:
```

### Comparing `patcherex2-0.1.9/src/patcherex2/components/patch_managers/patch_manager.py` & `patcherex2-0.2.0/src/patcherex2/components/patch_managers/patch_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import List
+from __future__ import annotations
 
 from patcherex2.patches import Patch
 
 
 class PatchManager:
     def __init__(self) -> None:
         self.patches = []
         self.analyzed = False
 
     def add_patch(self, patch: Patch) -> None:
         self.analyzed = False
         self.patches.append(patch)
 
-    def add_patches(self, patches: List[Patch]) -> None:
+    def add_patches(self, patches: list[Patch]) -> None:
         for patch in patches:
             self.add_patch(patch)
 
     def export_patches(self, filename: str) -> None:
         raise NotImplementedError()
 
     def import_patches(self, filename: str) -> None:
```

### Comparing `patcherex2-0.1.9/src/patcherex2/patches/__init__.py` & `patcherex2-0.2.0/src/patcherex2/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/__init__.py` & `patcherex2-0.2.0/src/patcherex2/targets/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from .elf_aarch64_linux import ElfAArch64Linux
+from .elf_amd64_linux import ElfAmd64Linux
+from .elf_amd64_linux_recomp import ElfAmd64LinuxRecomp
 from .elf_arm_linux import ElfArmLinux
 from .elf_arm_linux_recomp import ElfArmLinuxRecomp
 from .elf_arm_mimxrt1052 import ElfArmMimxrt1052
-from .elf_i386_linux import ElfI386Linux
 from .elf_leon3_bare import ElfLeon3Bare
 from .elf_mips64_linux import ElfMips64Linux
 from .elf_mips64el_linux import ElfMips64elLinux
 from .elf_mips_linux import ElfMipsLinux
 from .elf_mipsel_linux import ElfMipselLinux
 from .elf_ppc64_linux import ElfPpc64Linux
 from .elf_ppc64le_linux import ElfPpc64leLinux
 from .elf_ppc_linux import ElfPpcLinux
-from .elf_x86_64_linux import ElfX8664Linux
-from .elf_x86_64_linux_recomp import ElfX8664LinuxRecomp
+from .elf_x86_linux import ElfX86Linux
 from .ihex_ppc_bare import IHexPPCBare
 from .target import Target
 
 __all__ = [
     "ElfAArch64Linux",
+    "ElfAmd64Linux",
+    "ElfAmd64LinuxRecomp",
     "ElfArmLinux",
     "ElfArmLinuxRecomp",
     "ElfArmMimxrt1052",
-    "ElfI386Linux",
     "ElfLeon3Bare",
     "ElfMips64Linux",
     "ElfMips64elLinux",
     "ElfMipsLinux",
     "ElfMipselLinux",
     "ElfPpc64Linux",
     "ElfPpc64leLinux",
     "ElfPpcLinux",
-    "ElfX8664Linux",
-    "ElfX8664LinuxRecomp",
+    "ElfX86Linux",
     "IHexPPCBare",
     "Target",
 ]
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_aarch64_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_mipsel_linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.mips import MipsInfo
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfAArch64Linux(Target):
-    NOP_BYTES = b"\x1f\x20\x03\xd5"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
-
+class ElfMipselLinux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\xb7\x00", 0x12
-            ):  # EM_AARCH64
+            if magic.startswith(b"\x7fELF\x01") and magic.startswith(
+                b"\x08\x00", 0x12
+            ):  # EM_MIPS
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
-                self.p, keystone.KS_ARCH_ARM64, keystone.KS_MODE_LITTLE_ENDIAN
+                self.p,
+                keystone.KS_ARCH_MIPS,
+                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_MIPS32,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["-target", "aarch64-linux-gnu"])
+            return Clang(self.p, compiler_flags=["--target=mipsel-linux-gnu"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
-            return Capstone(capstone.CS_ARCH_ARM64, capstone.CS_MODE_LITTLE_ENDIAN)
+            return Capstone(
+                capstone.CS_ARCH_MIPS,
+                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_MIPS32,
+            )
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
         raise NotImplementedError()
@@ -63,7 +64,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return MipsInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_arm_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_arm_linux.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.arm import ArmInfo
 from ..components.assemblers.keystone_arm import KeystoneArm
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang_arm import ClangArm
 from ..components.disassemblers.capstone_arm import CapstoneArm
 from ..components.utils.utils import Utils
 from .target import Target
 
 
 class ElfArmLinux(Target):
-    NOP_BYTES = b"\x00\xF0\x20\xE3"  # TODO: thumb
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
-
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
             if magic.startswith(b"\x7fELF") and magic.startswith(
                 b"\x28\x00", 0x12
             ):  # EM_ARM
@@ -61,7 +57,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return ArmInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_arm_linux_recomp.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_arm_linux_recomp.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_arm_mimxrt1052.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_arm_mimxrt1052.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
                 self.p.binfmt_tool.update_binary_content(
                     self._elf.header["e_shoff"] + idx * self._elf.header["e_shentsize"],
                     self._elf.structs.Elf_Shdr.build(section_header),
                 )
 
 
 class ElfArmMimxrt1052(ElfArmLinux):
+    @staticmethod
+    def detect_target(binary_path):
+        return False
+
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "default"
         if binfmt_tool == "default":
             return ELF(self.p, self.binary_path)
         if binfmt_tool == "custom":
             return CustomElf(self.p, self.binary_path)
         raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_i386_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_mips64el_linux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.mips64 import Mips64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfI386Linux(Target):
-    NOP_BYTES = b"\x90"
-    NOP_SIZE = 1
-    JMP_ASM = "jmp {dst}"
-    JMP_SIZE = 5
-
+class ElfMips64elLinux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\x03\x00", 0x12
-            ):  # EM_386
+            if magic.startswith(b"\x7fELF\x02") and magic.startswith(
+                b"\x08\x00", 0x12
+            ):  # EM_MIPS
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
-                keystone.KS_ARCH_X86,
-                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_32,
+                keystone.KS_ARCH_MIPS,
+                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_64,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["-m32"])
+            return Clang(self.p, compiler_flags=["--target=mips64el-linux-gnuabi64"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
             return Capstone(
-                capstone.CS_ARCH_X86,
-                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_32,
+                capstone.CS_ARCH_MIPS,
+                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_MIPS64,
             )
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
@@ -68,7 +64,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Mips64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_leon3_bare.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_leon3_bare.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 from ..components.allocation_managers.allocation_manager import (
     AllocationManager,
     MappedBlock,
     MemoryFlag,
 )
+from ..components.archinfo.sparc import SparcInfo
 from ..components.assemblers.bcc import Bcc as BccAssembler
 from ..components.assemblers.keystone_sparc import KeystoneSparc, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.bcc import Bcc as BccCompiler
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
@@ -26,43 +27,18 @@
             self._segments[0]["p_vaddr"],
             self._segments[0]["p_memsz"],
             is_free=False,
             flag=MemoryFlag.RWX,
         )
         self.p.allocation_manager.add_block(block)
 
-        unused_funcs = self.p.binary_analyzer.get_unused_funcs()
-
-        for func in unused_funcs:
-            file_offset = self.p.binary_analyzer.mem_addr_to_file_offset(func["addr"])
-            block = MappedBlock(
-                file_offset,
-                func["addr"],
-                func["size"],
-                is_free=True,
-                flag=MemoryFlag.RX,
-            )
-            self.p.allocation_manager.add_block(block)
-
 
 class ElfLeon3Bare(Target):
-    NOP_BYTES = b"\x01\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}\nnop"  # nop due to delay slot
-    JMP_SIZE = 8
-
     @staticmethod
     def detect_target(binary_path):
-        with open(binary_path, "rb") as f:
-            magic = f.read(0x14)
-            # NOTE: probably should not default sparc to this target, but it's fine for now
-            if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\x00\x02", 0x12
-            ):  # EM_SPARC
-                return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return KeystoneSparc(
                 self.p,
@@ -104,7 +80,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return SparcInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_mips64_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_ppc64_linux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.ppc64 import Ppc64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfMips64Linux(Target):
-    NOP_BYTES = b"\x00\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "j {dst}"
-    # NOTE: keystone will always add nop for branch delay slot, so include it in size
-    JMP_SIZE = 8
-
+class ElfPpc64Linux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF\x02") and magic.startswith(
-                b"\x00\x08", 0x12
-            ):  # EM_MIPS
+            if magic.startswith(b"\x7fELF") and magic.startswith(
+                b"\x00\x15", 0x12
+            ):  # EM_PPC64
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
-                keystone.KS_ARCH_MIPS,
-                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_64,
+                keystone.KS_ARCH_PPC,
+                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_PPC64,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["--target=mips64-linux-gnuabi64"])
+            return Clang(self.p, compiler_flags=["-target", "powerpc64-linux-gnu"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
-            return Capstone(
-                capstone.CS_ARCH_MIPS,
-                capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_MIPS64,
+            cs = Capstone(
+                capstone.CS_ARCH_PPC, capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_64
             )
+            # NOTE: Doing this because keystone expects registers to just be numbers
+            cs.cs.syntax = capstone.CS_OPT_SYNTAX_NOREGNAME
+            return cs
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
         raise NotImplementedError()
@@ -69,7 +66,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Ppc64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_mips64el_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_mips_linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.mips import MipsInfo
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfMips64elLinux(Target):
-    NOP_BYTES = b"\x00\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "j {dst}"
-    # NOTE: keystone will always add nop for branch delay slot, so include it in size
-    JMP_SIZE = 8
-
+class ElfMipsLinux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF\x02") and magic.startswith(
-                b"\x08\x00", 0x12
+            if magic.startswith(b"\x7fELF\x01") and magic.startswith(
+                b"\x00\x08", 0x12
             ):  # EM_MIPS
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
                 keystone.KS_ARCH_MIPS,
-                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_64,
+                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_MIPS32,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["--target=mips64el-linux-gnuabi64"])
+            return Clang(self.p, compiler_flags=["--target=mips-linux-gnu"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
             return Capstone(
                 capstone.CS_ARCH_MIPS,
-                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_MIPS64,
+                capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_MIPS32,
             )
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
@@ -69,7 +64,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return MipsInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_mips_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_mips64_linux.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.mips64 import Mips64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfMipsLinux(Target):
-    NOP_BYTES = b"\x00\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "j {dst}"
-    # NOTE: keystone will always add nop for branch delay slot, so include it in size
-    JMP_SIZE = 8
-
+class ElfMips64Linux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF\x01") and magic.startswith(
+            if magic.startswith(b"\x7fELF\x02") and magic.startswith(
                 b"\x00\x08", 0x12
             ):  # EM_MIPS
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
                 keystone.KS_ARCH_MIPS,
-                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_MIPS32,
+                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_64,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["--target=mips-linux-gnu"])
+            return Clang(self.p, compiler_flags=["--target=mips64-linux-gnuabi64"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
             return Capstone(
                 capstone.CS_ARCH_MIPS,
-                capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_MIPS32,
+                capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_MIPS64,
             )
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
@@ -69,7 +64,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Mips64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_mipsel_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_amd64_linux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.amd64 import Amd64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfMipselLinux(Target):
-    NOP_BYTES = b"\x00\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "j {dst}"
-    # NOTE: keystone will always add nop for branch delay slot, so include it in size
-    JMP_SIZE = 8
-
+class ElfAmd64Linux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
-            if magic.startswith(b"\x7fELF\x01") and magic.startswith(
-                b"\x08\x00", 0x12
-            ):  # EM_MIPS
+            if magic.startswith(b"\x7fELF") and magic.startswith(
+                b"\x3e\x00", 0x12
+            ):  # EM_X86_64
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
-                keystone.KS_ARCH_MIPS,
-                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_MIPS32,
+                keystone.KS_ARCH_X86,
+                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_64,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["--target=mipsel-linux-gnu"])
+            return Clang(self.p)
+        elif compiler == "clang19":
+            return Clang(self.p, clang_version=19)
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
             return Capstone(
-                capstone.CS_ARCH_MIPS,
-                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_MIPS32,
+                capstone.CS_ARCH_X86,
+                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_64,
             )
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
@@ -69,7 +66,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Amd64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_ppc64_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_x86_linux.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.x86 import X86Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfPpc64Linux(Target):
-    NOP_BYTES = b"\x60\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
-
+class ElfX86Linux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
             if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\x00\x15", 0x12
-            ):  # EM_PPC64
+                b"\x03\x00", 0x12
+            ):  # EM_386
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
-                keystone.KS_ARCH_PPC,
-                keystone.KS_MODE_BIG_ENDIAN + keystone.KS_MODE_PPC64,
+                keystone.KS_ARCH_X86,
+                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_32,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["-target", "powerpc64-linux-gnu"])
+            return Clang(self.p, compiler_flags=["-m32"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
-            cs = Capstone(
-                capstone.CS_ARCH_PPC, capstone.CS_MODE_BIG_ENDIAN + capstone.CS_MODE_64
+            return Capstone(
+                capstone.CS_ARCH_X86,
+                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_32,
             )
-            # NOTE: Doing this because keystone expects registers to just be numbers
-            cs.cs.syntax = capstone.CS_OPT_SYNTAX_NOREGNAME
-            return cs
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
         raise NotImplementedError()
@@ -70,7 +64,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return X86Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_ppc64le_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_aarch64_linux.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,63 @@
+import logging
+
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.aarch64 import Aarch64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
+logger = logging.getLogger(__name__)
 
-class ElfPpc64leLinux(Target):
-    NOP_BYTES = b"\x60\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
 
+class ElfAArch64Linux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
             if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\x15\x00", 0x12
-            ):  # EM_PPC64
+                b"\xb7\x00", 0x12
+            ):  # EM_AARCH64
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
-                self.p,
-                keystone.KS_ARCH_PPC,
-                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_PPC64,
+                self.p, keystone.KS_ARCH_ARM64, keystone.KS_MODE_LITTLE_ENDIAN
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p, compiler_flags=["-target", "powerpc64le-linux-gnu"])
+            return Clang(self.p, compiler_flags=["-target", "aarch64-linux-gnu"])
+        elif compiler == "clang19":
+            return Clang(
+                self.p,
+                compiler_flags=["-target", "aarch64-linux-gnu"],
+                clang_version=19,
+            )
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
-            cs = Capstone(
-                capstone.CS_ARCH_PPC,
-                capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_64,
-            )
-            # NOTE: Doing this because keystone expects registers to just be numbers
-            cs.cs.syntax = capstone.CS_OPT_SYNTAX_NOREGNAME
-            return cs
+            return Capstone(capstone.CS_ARCH_ARM64, capstone.CS_MODE_LITTLE_ENDIAN)
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
         raise NotImplementedError()
@@ -71,7 +69,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Aarch64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_ppc_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_ppc_linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.ppc import PpcInfo
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
 class ElfPpcLinux(Target):
-    NOP_BYTES = b"\x60\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
-
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
             if magic.startswith(b"\x7fELF") and magic.startswith(
                 b"\x00\x14", 0x12
             ):  # EM_PPC
@@ -70,7 +66,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return PpcInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_x86_64_linux.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_ppc64le_linux.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.ppc64 import Ppc64Info
 from ..components.assemblers.keystone import Keystone, keystone
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.elf import ELF
 from ..components.compilers.clang import Clang
 from ..components.disassemblers.capstone import Capstone, capstone
 from ..components.utils.utils import Utils
 from .target import Target
 
 
-class ElfX8664Linux(Target):
-    NOP_BYTES = b"\x90"
-    NOP_SIZE = 1
-    JMP_ASM = "jmp {dst}"
-    JMP_SIZE = 6
-
+class ElfPpc64leLinux(Target):
     @staticmethod
     def detect_target(binary_path):
         with open(binary_path, "rb") as f:
             magic = f.read(0x14)
             if magic.startswith(b"\x7fELF") and magic.startswith(
-                b"\x3e\x00", 0x12
-            ):  # EM_X86_64
+                b"\x15\x00", 0x12
+            ):  # EM_PPC64
                 return True
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "keystone"
         if assembler == "keystone":
             return Keystone(
                 self.p,
-                keystone.KS_ARCH_X86,
-                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_64,
+                keystone.KS_ARCH_PPC,
+                keystone.KS_MODE_LITTLE_ENDIAN + keystone.KS_MODE_PPC64,
             )
         raise NotImplementedError()
 
     def get_allocation_manager(self, allocation_manager):
         allocation_manager = allocation_manager or "default"
         if allocation_manager == "default":
             return AllocationManager(self.p)
         raise NotImplementedError()
 
     def get_compiler(self, compiler):
         compiler = compiler or "clang"
         if compiler == "clang":
-            return Clang(self.p)
+            return Clang(self.p, compiler_flags=["-target", "powerpc64le-linux-gnu"])
         raise NotImplementedError()
 
     def get_disassembler(self, disassembler):
         disassembler = disassembler or "capstone"
         if disassembler == "capstone":
-            return Capstone(
-                capstone.CS_ARCH_X86,
+            cs = Capstone(
+                capstone.CS_ARCH_PPC,
                 capstone.CS_MODE_LITTLE_ENDIAN + capstone.CS_MODE_64,
             )
+            # NOTE: Doing this because keystone expects registers to just be numbers
+            cs.cs.syntax = capstone.CS_OPT_SYNTAX_NOREGNAME
+            return cs
         raise NotImplementedError()
 
     def get_binfmt_tool(self, binfmt_tool):
         binfmt_tool = binfmt_tool or "pyelftools"
         if binfmt_tool == "pyelftools":
             return ELF(self.p, self.binary_path)
         raise NotImplementedError()
@@ -68,7 +67,13 @@
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return Ppc64Info()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/elf_x86_64_linux_recomp.py` & `patcherex2-0.2.0/src/patcherex2/targets/elf_amd64_linux_recomp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ..components.binary_analyzers.angr import Angr
 from ..components.compilers.llvm_recomp import LLVMRecomp
-from .elf_x86_64_linux import ElfX8664Linux
+from .elf_amd64_linux import ElfAmd64Linux
 
 
-class ElfX8664LinuxRecomp(ElfX8664Linux):
+class ElfAmd64LinuxRecomp(ElfAmd64Linux):
     @staticmethod
     def detect_target(binary_path):
         return False
 
     def get_compiler(self, compiler):
         compiler = compiler or "llvm_recomp"
         if compiler == "llvm_recomp":
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/ihex_ppc_bare.py` & `patcherex2-0.2.0/src/patcherex2/targets/ihex_ppc_bare.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import logging
 
 import archinfo
 
 from ..components.allocation_managers.allocation_manager import AllocationManager
+from ..components.archinfo.ppc_vle import PpcVleInfo
 from ..components.assemblers.ppc_vle import PpcVle as PpcVleAssembler
 from ..components.binary_analyzers.angr import Angr
 from ..components.binfmt_tools.ihex import IHex
 from ..components.compilers.ppc_vle import PpcVle as PpcVleCompiler
 from ..components.disassemblers.ppc_vle import PpcVle as PpcVleDisassembler
 from ..components.utils.utils import Utils
 from .target import Target
 
 logger = logging.getLogger(__name__)
 
 
 class IHexPPCBare(Target):
-    NOP_BYTES = b"\x01\x00\x00\x00"
-    NOP_SIZE = 4
-    JMP_ASM = "b {dst}"
-    JMP_SIZE = 4
-
     @staticmethod
     def detect_target(binary_path):
         return False
 
     def get_assembler(self, assembler):
         assembler = assembler or "default"
         if assembler == "default":
@@ -55,18 +51,32 @@
         raise NotImplementedError()
 
     def get_binary_analyzer(self, binary_analyzer):
         binary_analyzer = binary_analyzer or "angr"
         if binary_analyzer == "angr":
             return Angr(
                 self.binary_path,
-                arch=archinfo.ArchPcode("PowerPC:BE:32:MPC8270"),
-                auto_load_libs=False,
-                load_debug_info=True,
+                angr_kwargs={
+                    "arch": archinfo.ArchPcode("PowerPC:BE:32:MPC8270"),
+                    "auto_load_libs": False,
+                    "load_debug_info": True,
+                },
+                angr_cfg_kwargs={
+                    "normalize": True,
+                    "data_references": True,
+                    "force_smart_scan": False,
+                    "force_complete_scan": False,
+                },
             )
         raise NotImplementedError()
 
     def get_utils(self, utils):
         utils = utils or "default"
         if utils == "default":
             return Utils(self.p, self.binary_path)
         raise NotImplementedError()
+
+    def get_archinfo(self, archinfo):
+        archinfo = archinfo or "default"
+        if archinfo == "default":
+            return PpcVleInfo()
+        raise NotImplementedError()
```

### Comparing `patcherex2-0.1.9/src/patcherex2/targets/target.py` & `patcherex2-0.2.0/src/patcherex2/targets/target.py`

 * *Files identical despite different names*

### Comparing `patcherex2-0.1.9/src/patcherex2.egg-info/SOURCES.txt` & `patcherex2-0.2.0/src/patcherex2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 src/patcherex2.egg-info/PKG-INFO
 src/patcherex2.egg-info/SOURCES.txt
 src/patcherex2.egg-info/dependency_links.txt
 src/patcherex2.egg-info/requires.txt
 src/patcherex2.egg-info/top_level.txt
 src/patcherex2/components/allocation_managers/__init__.py
 src/patcherex2/components/allocation_managers/allocation_manager.py
+src/patcherex2/components/archinfo/__init__.py
+src/patcherex2/components/archinfo/aarch64.py
+src/patcherex2/components/archinfo/amd64.py
+src/patcherex2/components/archinfo/arm.py
+src/patcherex2/components/archinfo/mips.py
+src/patcherex2/components/archinfo/mips64.py
+src/patcherex2/components/archinfo/ppc.py
+src/patcherex2/components/archinfo/ppc64.py
+src/patcherex2/components/archinfo/ppc_vle.py
+src/patcherex2/components/archinfo/sparc.py
+src/patcherex2/components/archinfo/x86.py
 src/patcherex2/components/assemblers/__init__.py
 src/patcherex2/components/assemblers/assembler.py
 src/patcherex2/components/assemblers/bcc.py
 src/patcherex2/components/assemblers/keystone.py
 src/patcherex2/components/assemblers/keystone_arm.py
 src/patcherex2/components/assemblers/keystone_sparc.py
 src/patcherex2/components/assemblers/ppc_vle.py
@@ -40,38 +51,39 @@
 src/patcherex2/components/disassemblers/disassembler.py
 src/patcherex2/components/disassemblers/ppc_vle.py
 src/patcherex2/components/patch_managers/__init__.py
 src/patcherex2/components/patch_managers/builtin.py
 src/patcherex2/components/patch_managers/imp.py
 src/patcherex2/components/patch_managers/patch_manager.py
 src/patcherex2/components/utils/__init__.py
+src/patcherex2/components/utils/linker_script_parser.py
 src/patcherex2/components/utils/utils.py
 src/patcherex2/patches/__init__.py
 src/patcherex2/patches/data_patches.py
 src/patcherex2/patches/dummy_patches.py
 src/patcherex2/patches/function_patches.py
 src/patcherex2/patches/instruction_patches.py
 src/patcherex2/patches/patch.py
 src/patcherex2/patches/raw_patches.py
 src/patcherex2/targets/__init__.py
 src/patcherex2/targets/elf_aarch64_linux.py
+src/patcherex2/targets/elf_amd64_linux.py
+src/patcherex2/targets/elf_amd64_linux_recomp.py
 src/patcherex2/targets/elf_arm_linux.py
 src/patcherex2/targets/elf_arm_linux_recomp.py
 src/patcherex2/targets/elf_arm_mimxrt1052.py
-src/patcherex2/targets/elf_i386_linux.py
 src/patcherex2/targets/elf_leon3_bare.py
 src/patcherex2/targets/elf_mips64_linux.py
 src/patcherex2/targets/elf_mips64el_linux.py
 src/patcherex2/targets/elf_mips_linux.py
 src/patcherex2/targets/elf_mipsel_linux.py
 src/patcherex2/targets/elf_ppc64_linux.py
 src/patcherex2/targets/elf_ppc64le_linux.py
 src/patcherex2/targets/elf_ppc_linux.py
-src/patcherex2/targets/elf_x86_64_linux.py
-src/patcherex2/targets/elf_x86_64_linux_recomp.py
+src/patcherex2/targets/elf_x86_linux.py
 src/patcherex2/targets/ihex_ppc_bare.py
 src/patcherex2/targets/target.py
 tests/test_aarch64.py
 tests/test_arm.py
 tests/test_i386.py
 tests/test_mips.py
 tests/test_mips64.py
```

### Comparing `patcherex2-0.1.9/tests/test_aarch64.py` & `patcherex2-0.2.0/tests/test_i386.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,275 +4,301 @@
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
 
+import pytest
+
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
 class Tests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.bin_location = str(
             os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
-                "./test_binaries/aarch64",
+                "./test_binaries/x86",
             )
         )
 
     def test_raw_file_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x640, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0x2008, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_file_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0x7AB, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0x200B, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x400640, b"No")],
+            [ModifyRawBytesPatch(0x804A008, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0x7AB, b"No")],
+            [ModifyRawBytesPatch(0x200B, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyInstructionPatch(0x400570, "add x1,x0,#0x648")],
+            [
+                ModifyInstructionPatch(0x8049192, "lea edx, [0x804a00b]"),
+                ModifyInstructionPatch(0x8049198, "push edx"),
+            ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyInstructionPatch(0x778, "add x1,x1,#0x7a8")],
+            [
+                ModifyInstructionPatch(0x11C0, "lea eax, [ebx + 0xffffe008]"),
+            ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
+    def test_modify_instruction_patch2_nopie(self):
+        self.run_one(
+            "printf_nopie",
+            [ModifyInstructionPatch(0x80491A0, "mov eax, 0x0")],
+            expected_output="",
+            expected_returnCode=0,
+        )
+
+    def test_modify_instruction_patch2_pie(self):
+        self.run_one(
+            "printf_pie",
+            [ModifyInstructionPatch(0x11C9, "mov eax, 0x0")],
+            expected_output="",
+            expected_returnCode=0,
+        )
+
     def test_insert_instruction_patch_nopie(self):
         instrs = """
-            mov x8, 0x40
-            mov x0, 0x1
-            ldr x1, =0x400640
-            mov x2, 0x3
-            svc 0
+            mov eax, 0x4
+            mov ebx, 0x1
+            lea ecx, [0x804a008]
+            mov edx, 0x3
+            int 0x80
         """
         self.run_one(
             "printf_nopie",
-            [InsertInstructionPatch(0x400580, instrs)],
+            [InsertInstructionPatch(0x80491A7, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_pie(self):
         instrs = """
-            mov x8, 0x40
-            mov x0, 0x1
-            adrp x1, 0x0
-            add x1, x1, #0x7ab
-            mov x2, 0x3
-            svc 0
+            lea ecx, [ebx + 0xffffe00b]
+            mov eax, 0x4
+            mov ebx, 0x1
+            mov edx, 0x3
+            int 0x80
         """
         self.run_one(
             "printf_pie",
-            [InsertInstructionPatch(0x780, instrs)],
+            [InsertInstructionPatch(0x11D2, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_2_nopie(self):
         instrs = """
-            mov x8, 0x5d
-            mov x0, 0x32
-            svc 0
+            mov eax, 0x32
+            leave
+            ret
         """
         self.run_one(
             "printf_nopie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0x400580, "b {return_0x32}"),
+                ModifyInstructionPatch(0x80491A7, "jmp {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_insert_instruction_patch_2_pie(self):
         instrs = """
-            mov x8, 0x5d
-            mov x0, 0x32
-            svc 0
+            mov eax, 0x32
+            leave
+            ret
         """
         self.run_one(
             "printf_pie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0x780, "b {return_0x32}"),
+                ModifyInstructionPatch(0x11D2, "jmp {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_remove_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
-                RemoveInstructionPatch(0x400641, num_bytes=4),
+                RemoveInstructionPatch(0x804A009, num_bytes=1),
             ],
-            expected_output=b"H\x1f\x20\x03\xd5",
+            expected_output=b"H\x90",
             expected_returnCode=0,
         )
 
     def test_remove_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
-                RemoveInstructionPatch(0x7AC, num_bytes=4),
+                RemoveInstructionPatch(0x200C, num_bytes=1),
             ],
-            expected_output=b"H\x1f\x20\x03\xd5",
+            expected_output=b"H\x90",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyDataPatch(0x400640, b"No")],
+            [ModifyDataPatch(0x804A008, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyDataPatch(0x7AB, b"No")],
+            [ModifyDataPatch(0x200B, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_insert_data_patch_nopie(self, tlen=5):
         p1 = InsertDataPatch("added_data", b"A" * tlen)
         instrs = """
-            mov x8, 0x40
-            mov x0, 0x1
-            ldr x1, ={added_data}
-            mov x2, %s
-            svc 0
+            mov eax, 0x4
+            mov ebx, 0x1
+            lea ecx, [{added_data}]
+            mov edx, %s
+            int 0x80
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0x400580, instrs)
+        p2 = InsertInstructionPatch(0x80491A7, instrs)
         self.run_one(
             "printf_nopie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
+    @pytest.mark.skip(reason="difficult to do with pie")
     def test_insert_data_patch_pie(self, tlen=5):
         p1 = InsertDataPatch("added_data", b"A" * tlen)
         instrs = """
-            mov x8, 0x40
-            mov x0, 0x1
-            adrp x1, 0x0
-            ldr x3, ={added_data}
-            add x1, x1, x3
-            mov x2, %s
-            svc 0
+            mov eax, 0x4
+            mov ebx, 0x1
+            lea edx, [here]
+            here: and edx, 0xffff0000
+            lea ecx, [edx + {added_data}]
+            mov edx, %s
+            int 0x80
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0x780, instrs)
+        p2 = InsertInstructionPatch(0x11D2, instrs)
         self.run_one(
             "printf_pie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [RemoveDataPatch(0x400641, 1)],
+            [RemoveDataPatch(0x804A009, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [RemoveDataPatch(0x7AC, 1)],
+            [RemoveDataPatch(0x200C, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
-    def test_replace_function_patch(self):
+    def test_replace_function_patch_nopie(self):
         code = """
         int add(int a, int b){ for(;; b--, a+=2) if(b <= 0) return a; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x74C, code)],
+            [ModifyFunctionPatch(0x119D, code)],
             expected_output=b"70707070",
             expected_returnCode=0,
         )
 
+    @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference(self):
         code = """
         extern int add(int, int);
         extern int subtract(int, int);
         int multiply(int a, int b){ for(int c = 0;; b = subtract(b, 1), c = subtract(c, a)) if(b <= 0) return c; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x7D4, code)],
+            [ModifyFunctionPatch(0x11C9, code)],
             expected_output=b"-21-21",
             expected_returnCode=0,
         )
 
+    @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference_and_rodata(self):
         code = """
         extern int printf(const char *format, ...);
         int multiply(int a, int b){ printf("%sWorld %s %s %s %d\\n", "Hello ", "Hello ", "Hello ", "Hello ", a * b);printf("%sWorld\\n", "Hello "); return a * b; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x7D4, code)],
+            [ModifyFunctionPatch(0x11C9, code)],
             expected_output=b"Hello World Hello  Hello  Hello  21\nHello World\n2121",
             expected_returnCode=0,
         )
 
+    @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_insert_function_patch(self):
         insert_code = """
         int min(int a, int b) { return (a < b) ? a : b; }
         """
         replace_code = """
         extern int min(int, int);
         int max(int a, int b) { return min(a, b); }
         """
         self.run_one(
             "replace_function_patch",
             [
                 InsertFunctionPatch("min", insert_code),
-                ModifyFunctionPatch(0x724, replace_code),
+                ModifyFunctionPatch(0x1261, replace_code),
             ],
             expected_output=b"2121212121",
             expected_returnCode=0,
         )
 
     def run_one(
         self,
@@ -288,19 +314,19 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
-                ["qemu-aarch64", "-L", "/usr/aarch64-linux-gnu", tmp_file],
+                [tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
             )
             res = p.communicate(inputvalue)
             if expected_output:
                 if res[0] != expected_output:
```

### Comparing `patcherex2-0.1.9/tests/test_arm.py` & `patcherex2-0.2.0/tests/test_arm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -154,25 +155,25 @@
 
     def test_remove_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
                 RemoveInstructionPatch(0x1044B, num_bytes=4),
             ],
-            expected_output=b"\xF0\x20\xE3",
+            expected_output=b"\xf0\x20\xe3",
             expected_returnCode=0,
         )
 
     def test_remove_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
                 RemoveInstructionPatch(0x5DE, num_bytes=4),
             ],
-            expected_output=b"\xF0\x20\xE3",
+            expected_output=b"\xf0\x20\xe3",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [ModifyDataPatch(0x1044C, b"No")],
@@ -310,15 +311,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-arm", "-L", "/usr/arm-linux-gnueabihf", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_i386.py` & `patcherex2-0.2.0/tests/test_ppc64.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,267 +3,268 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
 class Tests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.bin_location = str(
             os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
-                "./test_binaries/i386",
+                "./test_binaries/ppc64",
             )
         )
 
     def test_raw_file_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x2008, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0x88F, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_file_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0x200B, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0xB74, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x804A008, b"No")],
+            [ModifyRawBytesPatch(0x1000088F, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0x200B, b"No")],
+            [ModifyRawBytesPatch(0xB74, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
-                ModifyInstructionPatch(0x8049192, "lea edx, [0x804a00b]"),
-                ModifyInstructionPatch(0x8049198, "push edx"),
+                ModifyInstructionPatch(0x1000076C, "subi 4, 4, 0x7674"),
             ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
-                ModifyInstructionPatch(0x11C0, "lea eax, [ebx + 0xffffe008]"),
+                ModifyInstructionPatch(0xA4C, "subi 4, 4, 0x738C"),
             ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_nopie(self):
         instrs = """
-            mov eax, 0x4
-            mov ebx, 0x1
-            lea ecx, [0x804a008]
-            mov edx, 0x3
-            int 0x80
+            li 0, 0x4
+            li 3, 1
+            lis 4, 0x1000088f@h
+            addi 4, 4, 0x1000088f@l
+            li 5, 0x3
+            sc
         """
         self.run_one(
             "printf_nopie",
-            [InsertInstructionPatch(0x80491A7, instrs)],
+            [InsertInstructionPatch(0x10000774, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_pie(self):
         instrs = """
-            lea ecx, [ebx + 0xffffe00b]
-            mov eax, 0x4
-            mov ebx, 0x1
-            mov edx, 0x3
-            int 0x80
+            li 0, 0x4
+            li 3, 1
+            addi 4, 4, 0x1
+            li 5, 0x3
+            sc
         """
         self.run_one(
             "printf_pie",
-            [InsertInstructionPatch(0x11D2, instrs)],
+            [InsertInstructionPatch(0xA54, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_2_nopie(self):
         instrs = """
-            mov eax, 0x32
-            leave
-            ret
+            li 3, 0x32
+            li 0, 0x1
+            sc
         """
         self.run_one(
             "printf_nopie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0x80491A7, "jmp {return_0x32}"),
+                ModifyInstructionPatch(0x10000774, "b {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_insert_instruction_patch_2_pie(self):
         instrs = """
-            mov eax, 0x32
-            leave
-            ret
+            li 3, 0x32
+            li 0, 0x1
+            sc
         """
         self.run_one(
             "printf_pie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0x11D2, "jmp {return_0x32}"),
+                ModifyInstructionPatch(0xA54, "b {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_remove_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
-                RemoveInstructionPatch(0x804A009, num_bytes=1),
+                RemoveInstructionPatch(0x10000890, num_bytes=4),
             ],
-            expected_output=b"H\x90",
+            expected_output=b"H\x60",
             expected_returnCode=0,
         )
 
     def test_remove_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
-                RemoveInstructionPatch(0x200C, num_bytes=1),
+                RemoveInstructionPatch(0xB78, num_bytes=4),
             ],
-            expected_output=b"H\x90",
+            expected_output=b"H\x60",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyDataPatch(0x804A008, b"No")],
+            [ModifyDataPatch(0x1000088F, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyDataPatch(0x200B, b"No")],
+            [ModifyDataPatch(0xB77, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_insert_data_patch_nopie(self, tlen=5):
         p1 = InsertDataPatch("added_data", b"A" * tlen)
         instrs = """
-            mov eax, 0x4
-            mov ebx, 0x1
-            lea ecx, [{added_data}]
-            mov edx, %s
-            int 0x80
+            li 0, 0x4
+            li 3, 0x1
+            lis 4, {added_data}@h
+            addi 4, 4, {added_data}@l
+            li 5, %s
+            sc
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0x80491A7, instrs)
+        p2 = InsertInstructionPatch(0x10000774, instrs)
         self.run_one(
             "printf_nopie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="difficult to do with pie")
     def test_insert_data_patch_pie(self, tlen=5):
         p1 = InsertDataPatch("added_data", b"A" * tlen)
         instrs = """
-            mov eax, 0x4
-            mov ebx, 0x1
-            lea edx, [here]
-            here: and edx, 0xffff0000
-            lea ecx, [edx + {added_data}]
-            mov edx, %s
-            int 0x80
+            li 0, 0x4
+            li 3, 0x1
+            lis 4, {added_data}@h
+            addi 4, 4, {added_data}@l
+            li 5, %s
+            sc
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0x11D2, instrs)
+        p2 = InsertInstructionPatch(0xA54, instrs)
         self.run_one(
             "printf_pie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [RemoveDataPatch(0x804A009, 1)],
+            [RemoveDataPatch(0x10000890, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [RemoveDataPatch(0x200C, 1)],
+            [RemoveDataPatch(0xB78, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
-    def test_replace_function_patch_nopie(self):
+    def test_replace_function_patch(self):
         code = """
         int add(int a, int b){ for(;; b--, a+=2) if(b <= 0) return a; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x119D, code)],
+            [ModifyFunctionPatch(0xB44, code)],
             expected_output=b"70707070",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference(self):
         code = """
         extern int add(int, int);
         extern int subtract(int, int);
         int multiply(int a, int b){ for(int c = 0;; b = subtract(b, 1), c = subtract(c, a)) if(b <= 0) return c; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x11C9, code)],
+            [ModifyFunctionPatch(0xBEC, code)],
             expected_output=b"-21-21",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference_and_rodata(self):
         code = """
         extern int printf(const char *format, ...);
         int multiply(int a, int b){ printf("%sWorld %s %s %s %d\\n", "Hello ", "Hello ", "Hello ", "Hello ", a * b);printf("%sWorld\\n", "Hello "); return a * b; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0x11C9, code)],
+            [ModifyFunctionPatch(0xBEC, code)],
             expected_output=b"Hello World Hello  Hello  Hello  21\nHello World\n2121",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_insert_function_patch(self):
         insert_code = """
@@ -273,15 +274,15 @@
         extern int min(int, int);
         int max(int a, int b) { return min(a, b); }
         """
         self.run_one(
             "replace_function_patch",
             [
                 InsertFunctionPatch("min", insert_code),
-                ModifyFunctionPatch(0x1261, replace_code),
+                ModifyFunctionPatch(0xD2C, replace_code),
             ],
             expected_output=b"2121212121",
             expected_returnCode=0,
         )
 
     def run_one(
         self,
@@ -297,19 +298,19 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
-                [tmp_file],
+                ["qemu-ppc64", "-L", "/usr/powerpc64-linux-gnu", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
             )
             res = p.communicate(inputvalue)
             if expected_output:
                 if res[0] != expected_output:
```

### Comparing `patcherex2-0.1.9/tests/test_mips.py` & `patcherex2-0.2.0/tests/test_mips.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -299,15 +300,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-mips", "-L", "/usr/mips-linux-gnu", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_mips64.py` & `patcherex2-0.2.0/tests/test_mips64.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -296,15 +297,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-mips64", "-L", "/usr/mips64-linux-gnuabi64", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_mips64el.py` & `patcherex2-0.2.0/tests/test_mips64el.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -296,15 +297,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-mips64el", "-L", "/usr/mips64el-linux-gnuabi64", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_mipsel.py` & `patcherex2-0.2.0/tests/test_mipsel.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -299,15 +300,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-mipsel", "-L", "/usr/mipsel-linux-gnu", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_ppc.py` & `patcherex2-0.2.0/tests/test_ppc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
@@ -196,15 +197,15 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
                 ["qemu-ppc", "-L", "/usr/powerpc-linux-gnu", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
```

### Comparing `patcherex2-0.1.9/tests/test_ppc64.py` & `patcherex2-0.2.0/tests/test_ppc64le.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,191 +3,192 @@
 # ruff: noqa
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 import unittest
+
 import pytest
 
 from patcherex2 import *
 
 logging.getLogger("patcherex2").setLevel("DEBUG")
 
 
 class Tests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.bin_location = str(
             os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
-                "./test_binaries/ppc64",
+                "./test_binaries/ppc64le",
             )
         )
 
     def test_raw_file_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x88F, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0x8AB, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_file_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0xB74, b"No", addr_type="raw")],
+            [ModifyRawBytesPatch(0x9AF, b"No", addr_type="raw")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyRawBytesPatch(0x1000088F, b"No")],
+            [ModifyRawBytesPatch(0x100008AB, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_raw_mem_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyRawBytesPatch(0xB74, b"No")],
+            [ModifyRawBytesPatch(0x9AF, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
-                ModifyInstructionPatch(0x1000076C, "subi 4, 4, 0x7674"),
+                ModifyInstructionPatch(0x10000790, "subi 4, 4, 0x7658"),
             ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
     def test_modify_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
-                ModifyInstructionPatch(0xA4C, "subi 4, 4, 0x738C"),
+                ModifyInstructionPatch(0x890, "subi 4, 4, 0x7554"),
             ],
             expected_output=b"%s",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_nopie(self):
         instrs = """
             li 0, 0x4
             li 3, 1
-            lis 4, 0x1000088f@h
-            addi 4, 4, 0x1000088f@l
+            lis 4, 0x100008ab@h
+            addi 4, 4, 0x100008ab@l
             li 5, 0x3
             sc
         """
         self.run_one(
             "printf_nopie",
-            [InsertInstructionPatch(0x10000774, instrs)],
+            [InsertInstructionPatch(0x10000798, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_pie(self):
         instrs = """
             li 0, 0x4
             li 3, 1
             addi 4, 4, 0x1
             li 5, 0x3
             sc
         """
         self.run_one(
             "printf_pie",
-            [InsertInstructionPatch(0xA54, instrs)],
+            [InsertInstructionPatch(0x898, instrs)],
             expected_output=b"Hi\x00Hi",
             expected_returnCode=0,
         )
 
     def test_insert_instruction_patch_2_nopie(self):
         instrs = """
             li 3, 0x32
             li 0, 0x1
             sc
         """
         self.run_one(
             "printf_nopie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0x10000774, "b {return_0x32}"),
+                ModifyInstructionPatch(0x10000798, "b {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_insert_instruction_patch_2_pie(self):
         instrs = """
             li 3, 0x32
             li 0, 0x1
             sc
         """
         self.run_one(
             "printf_pie",
             [
                 InsertInstructionPatch("return_0x32", instrs),
-                ModifyInstructionPatch(0xA54, "b {return_0x32}"),
+                ModifyInstructionPatch(0x898, "b {return_0x32}"),
             ],
             expected_returnCode=0x32,
         )
 
     def test_remove_instruction_patch_nopie(self):
         self.run_one(
             "printf_nopie",
             [
-                RemoveInstructionPatch(0x10000890, num_bytes=4),
+                RemoveInstructionPatch(0x100008AC, num_bytes=4),
             ],
             expected_output=b"H\x60",
             expected_returnCode=0,
         )
 
     def test_remove_instruction_patch_pie(self):
         self.run_one(
             "printf_pie",
             [
-                RemoveInstructionPatch(0xB78, num_bytes=4),
+                RemoveInstructionPatch(0x9B0, num_bytes=4),
             ],
             expected_output=b"H\x60",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [ModifyDataPatch(0x1000088F, b"No")],
+            [ModifyDataPatch(0x100008AB, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_modify_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [ModifyDataPatch(0xB77, b"No")],
+            [ModifyDataPatch(0x9AF, b"No")],
             expected_output=b"No",
             expected_returnCode=0,
         )
 
     def test_insert_data_patch_nopie(self, tlen=5):
         p1 = InsertDataPatch("added_data", b"A" * tlen)
         instrs = """
             li 0, 0x4
             li 3, 0x1
             lis 4, {added_data}@h
             addi 4, 4, {added_data}@l
             li 5, %s
             sc
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0x10000774, instrs)
+        p2 = InsertInstructionPatch(0x10000798, instrs)
         self.run_one(
             "printf_nopie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
@@ -198,72 +199,72 @@
             li 0, 0x4
             li 3, 0x1
             lis 4, {added_data}@h
             addi 4, 4, {added_data}@l
             li 5, %s
             sc
         """ % hex(tlen)
-        p2 = InsertInstructionPatch(0xA54, instrs)
+        p2 = InsertInstructionPatch(0x898, instrs)
         self.run_one(
             "printf_pie",
             [p1, p2],
             expected_output=b"A" * tlen + b"Hi",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_nopie(self):
         self.run_one(
             "printf_nopie",
-            [RemoveDataPatch(0x10000890, 1)],
+            [RemoveDataPatch(0x100008AC, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
     def test_remove_data_patch_pie(self):
         self.run_one(
             "printf_pie",
-            [RemoveDataPatch(0xB78, 1)],
+            [RemoveDataPatch(0x9B0, 1)],
             expected_output=b"H",
             expected_returnCode=0,
         )
 
     def test_replace_function_patch(self):
         code = """
         int add(int a, int b){ for(;; b--, a+=2) if(b <= 0) return a; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0xB44, code)],
+            [ModifyFunctionPatch(0x860, code)],
             expected_output=b"70707070",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference(self):
         code = """
         extern int add(int, int);
         extern int subtract(int, int);
         int multiply(int a, int b){ for(int c = 0;; b = subtract(b, 1), c = subtract(c, a)) if(b <= 0) return c; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0xBEC, code)],
+            [ModifyFunctionPatch(0x920, code)],
             expected_output=b"-21-21",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_replace_function_patch_with_function_reference_and_rodata(self):
         code = """
         extern int printf(const char *format, ...);
         int multiply(int a, int b){ printf("%sWorld %s %s %s %d\\n", "Hello ", "Hello ", "Hello ", "Hello ", a * b);printf("%sWorld\\n", "Hello "); return a * b; }
         """
         self.run_one(
             "replace_function_patch",
-            [ModifyFunctionPatch(0xBEC, code)],
+            [ModifyFunctionPatch(0x920, code)],
             expected_output=b"Hello World Hello  Hello  Hello  21\nHello World\n2121",
             expected_returnCode=0,
         )
 
     @pytest.mark.skip(reason="waiting for cle relocation support")
     def test_insert_function_patch(self):
         insert_code = """
@@ -273,15 +274,15 @@
         extern int min(int, int);
         int max(int a, int b) { return min(a, b); }
         """
         self.run_one(
             "replace_function_patch",
             [
                 InsertFunctionPatch("min", insert_code),
-                ModifyFunctionPatch(0xD2C, replace_code),
+                ModifyFunctionPatch(0xA80, replace_code),
             ],
             expected_output=b"2121212121",
             expected_returnCode=0,
         )
 
     def run_one(
         self,
@@ -297,19 +298,19 @@
 
         with tempfile.TemporaryDirectory() as td:
             tmp_file = os.path.join(td, "patched")
             p = Patcherex(filepath)
             for patch in patches:
                 p.patches.append(patch)
             p.apply_patches()
-            p.binfmt_tool.save_binary(tmp_file)
+            p.save_binary(tmp_file)
             # os.system(f"readelf -hlS {tmp_file}")
 
             p = subprocess.Popen(
-                ["qemu-ppc64", "-L", "/usr/powerpc64-linux-gnu", tmp_file],
+                ["qemu-ppc64le", "-L", "/usr/powerpc64le-linux-gnu", tmp_file],
                 stdin=pipe,
                 stdout=pipe,
                 stderr=pipe,
             )
             res = p.communicate(inputvalue)
             if expected_output:
                 if res[0] != expected_output:
```

