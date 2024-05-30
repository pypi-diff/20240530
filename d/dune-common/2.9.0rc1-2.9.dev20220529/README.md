# Comparing `tmp/dune-common-2.9.0rc1.tar.gz` & `tmp/dune-common-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-common-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:49 2022, max compression
+gzip compressed data, was "dune-common-2.9.dev20220529.tar", last modified: Sun May 29 21:03:28 2022, max compression
```

## Comparing `dune-common-2.9.0rc1.tar` & `dune-common-2.9.dev20220529.tar`

### file list

```diff
@@ -1,553 +1,535 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.028029 dune-common-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/.mailmap
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.988029 dune-common-2.9.0rc1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (121)    19489 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    21568 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    21568 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.988029 dune-common-2.9.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/LICENSES/FSFAP.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19036 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2022-10-21 08:16:49.028029 dune-common-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.988029 dune-common-2.9.0rc1/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     8743 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/dune-ctest
--rwxr-xr-x   0 runner    (1001) docker     (121)     5679 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/dune-git-whitespace-hook
--rwxr-xr-x   0 runner    (1001) docker     (121)    32711 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/dunecontrol
--rwxr-xr-x   0 runner    (1001) docker     (121)     9576 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/dunepackaging.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19624 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/duneproject
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/find_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1895 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/rebuild-dune-pypi.sh
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/bin/rmgenerated.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.988029 dune-common-2.9.0rc1/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddBLASLapackFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddGMPFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddMETISFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddMPIFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddPTScotchFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddParMETISFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddQuadMathFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddSuiteSparseFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddTBBFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddThreadsFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/AddVcFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/CMakeBuiltinFunctionsDocumentation.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/CheckCXXFeatures.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    10627 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneAddLibrary.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneAddPybind11Module.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneCMakeCompat.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneCommonMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneDoc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneDoxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    15596 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneEnableAllPackages.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneExecuteProcess.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    35440 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneInstance.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    13832 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneModuleDependencies.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     6530 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneModuleInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePathHelper.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePkgConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    16986 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneProject.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     6519 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonCommonMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonCompiler.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonDeprecations.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonFindPackage.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    28731 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonInstallPackage.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonTestCommand.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    14350 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DunePythonVirtualenv.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneReplaceProperties.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7302 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneSphinxCMakeDoc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneSphinxDoc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneStreams.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneSymlinkOrCopy.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    18923 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneTestMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/DuneUtilities.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindInkscape.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindLatexMk.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindLatexMk.cmake.license
--rw-r--r--   0 runner    (1001) docker     (121)     6785 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindMETIS.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPTScotch.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindParMETIS.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/cmake/modules/FindPkgConfig/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPkgConfig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    32639 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPkgConfig/FindPkgConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPkgConfig/FindPkgConfig.cmake.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/cmake/modules/FindPython3/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPython3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15617 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPython3/FindPython3.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPython3/FindPython3.cmake.license
--rw-r--r--   0 runner    (1001) docker     (121)   161804 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPython3/Support.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindPython3/Support.cmake.license
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindQuadMath.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindSphinx.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    10339 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindSuiteSparse.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/FindTBB.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/Headercheck.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/OverloadCompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/UseInkscape.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    11383 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/UseLatexMk.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/UseLatexMk.cmake.license
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/latexmkrc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/modules/latexmkrc.cmake.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/cmake/pkg/
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/pkg/dune-common-config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/cmake/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/CreateDoxyFile.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/FinalizeHeadercheck.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/InstallFile.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/RunDoxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/WritePythonCMakeMetadata.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/checkvenvconf.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/conf.py.in
--rwxr-xr-x   0 runner    (1001) docker     (121)     4320 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/extract_cmake_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/index.rst.in
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/main77.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/module_library.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/pyversion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      661 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/run-in-dune-env.sh.in
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/setup.py.in
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/sphinx_cmake_dune.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/cmake/scripts/venvpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/doc/buildsystem/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/buildsystem/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17062 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/buildsystem/dune-common.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/doc/buildsystem/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/buildsystem/examples/Toolchain-Ubuntu-mingw32.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/buildsystem/examples/opts.mingw32
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/doc/comm/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/buildindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/communication.bib
--rw-r--r--   0 runner    (1001) docker     (121)    24664 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/communication.tex
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:48.996029 dune-common-2.9.0rc1/doc/comm/figures/
--rw-r--r--   0 runner    (1001) docker     (121)     6219 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/figures/darray.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/figures/darray.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)   192094 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/figures/distindex.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/figures/distindex.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/indexset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/poosc08.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/poosc08_test.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/comm/reverse.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.000029 dune-common-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)     7203 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/Doxystyle
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/doxygen-macros
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/doxygen/modules.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/doc/dunecontrol.1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.000029 dune-common-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.004029 dune-common-2.9.0rc1/dune/common/
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/alignedallocator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19756 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/arraylist.hh
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/assertandreturn.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/bartonnackmanifcheck.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18565 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/bigunsignedint.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/binaryfunctions.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17813 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/bitsetvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/boundschecking.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/classname.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10570 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/concept.hh
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/conditional.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/debugalign.cc
--rw-r--r--   0 runner    (1001) docker     (121)    19368 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/debugalign.hh
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/debugallocator.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9793 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/debugallocator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13000 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/debugstream.hh
--rw-r--r--   0 runner    (1001) docker     (121)    38719 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/densematrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21202 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/densevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/deprecated.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29578 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/diagonalmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/documentation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/dotproduct.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/dynmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/dynmatrixev.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5613 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/dynvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/enumset.hh
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/exceptions.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8129 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/filledarray.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19545 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/float_cmp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15351 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/float_cmp.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27995 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/fmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/fmatrixev.cc
--rw-r--r--   0 runner    (1001) docker     (121)    25302 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/fmatrixev.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/ftraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17310 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/fvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8005 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/genericiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/gmpfield.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13128 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/hash.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14246 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/hybridutilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/indent.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/indices.hh
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/interfaces.hh
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/ios_state.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/ios_state.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21889 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/iteratorfacades.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/iteratorrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/keywords.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/lru.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/mallocallocator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11553 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/math.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/matrixconcepts.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/matvectraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/modules.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/overloadset.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.008029 dune-common-2.9.0rc1/dune/common/parallel/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.008029 dune-common-2.9.0rc1/dune/common/parallel/benchmark/
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/benchmark/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12047 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/benchmark/mpi_collective_benchmark.cc
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/benchmark/options.ini
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/collectivecommunication.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20255 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/communication.hh
--rw-r--r--   0 runner    (1001) docker     (121)    52539 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/communicator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/future.hh
--rw-r--r--   0 runner    (1001) docker     (121)    31775 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    42015 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/indicessyncer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15515 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/localindex.hh
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpicollectivecommunication.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15676 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpicommunication.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpidata.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpifuture.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpiguard.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8904 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpihelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5891 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpipack.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/mpitraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/plocalindex.hh
--rw-r--r--   0 runner    (1001) docker     (121)    60447 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/remoteindices.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8693 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/selection.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.008029 dune-common-2.9.0rc1/dune/common/parallel/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/communicationtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/indexsettest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/mpidatatest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/mpifuturetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/mpigatherscattertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/mpipacktest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    18647 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/remoteindicestest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/selectiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12341 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/syncertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13983 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/test/variablesizecommunicatortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    42499 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parallel/variablesizecommunicator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parameterizedobject.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parametertree.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10215 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parametertree.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8167 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parametertreeparser.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/parametertreeparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/path.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8443 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/path.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14816 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/poolallocator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/power.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/precision.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/promotiontraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/propertymap.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/proxymemberaccess.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19262 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/quadmath.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29044 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/rangeutilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/referencehelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13187 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/reservedvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5148 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/scalarmatrixview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/scalarvectorview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/shared_ptr.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.008029 dune-common-2.9.0rc1/dune/common/simd/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10772 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/DESIGN.md
--rw-r--r--   0 runner    (1001) docker     (121)     9014 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/base.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/defaults.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21667 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/io.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25420 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/loop.hh
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/simd.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/standard.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.012029 dune-common-2.9.0rc1/dune/common/simd/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/looptest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/looptest.hh.in
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/looptest_vector.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/standardtest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/standardtest.hh.in
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/standardtest_vector.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vcarraytest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vcarraytest.hh.in
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vctest_mask.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vctest_simdarray.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vctest_simdmaskarray.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vctest_vector.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vcvectortest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test/vcvectortest.hh.in
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test.cc
--rw-r--r--   0 runner    (1001) docker     (121)    79510 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/test.hh
--rw-r--r--   0 runner    (1001) docker     (121)    31266 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd/vc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14307 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/simd.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/singleton.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19913 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/sllist.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.012029 dune-common-2.9.0rc1/dune/common/std/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/apply.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/functional.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/make_array.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10778 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/type_traits.hh
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/utility.hh
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/std/variant.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/stdstreams.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/stdstreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/stdthread.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/stdthread.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/streamoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/stringutility.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.016029 dune-common-2.9.0rc1/dune/common/test/
--rw-r--r--   0 runner    (1001) docker     (121)    13535 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/alignedallocatortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    23898 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/arithmetictestsuite.hh
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/arithmetictestsuitetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/arraylisttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/arraytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/assertandreturntest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/autocopytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/bigunsignedinttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/bitsetvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14998 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/boundscheckingmvtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/boundscheckingoptest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10293 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/boundscheckingtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/calloncetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/check_fvector_size.cc
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/check_fvector_size_fail.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/checkmatrixinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/classnametest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/collectorstream.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4365 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/concept.cc
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/constexprifelsetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/debugalignsimd.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/debugalignsimdtest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/debugalignsimdtest.hh.in
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/debugaligntest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11243 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/densematrixassignmenttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/densevectorassignmenttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/densevectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/diagonalmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/dummyiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10870 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/dynmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/dynvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12207 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/eigenvaluestest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/enumsettest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/filledarraytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    26863 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/fmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/functiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/fvectorconversion1d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16061 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/fvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/genericiterator_compile_fail.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/hybridutilitiestest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/indicestest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/iscallabletest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/iteratorfacadetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/iteratorfacadetest.hh
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/iteratorfacadetest2.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13159 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/iteratortest.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/lrutest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mathclassifierstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mathtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/metistest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mpicollectivecommunication.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mpicommunicationtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mpiguardtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/mpihelpertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/overloadsettest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parameterizedobjectfactorysingleton.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parameterizedobjectfactorysingleton.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parameterizedobjecttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parametertreelocaletest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parametertreetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/parmetistest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5731 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/pathtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/poolallocatortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/powertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/quadmathtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12296 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/rangeutilitiestest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4503 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/referencehelpertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4114 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/reservedvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/scotchtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/shared_ptrtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/singletontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/sllisttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/stdapplytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/stdchecktypes.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/stdidentity.cc
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/streamoperatorstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/streamtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/stringutilitytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/testdebugallocator.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/testfloatcmp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/testsuite.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/timing.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/transposetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/tupleutilitytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/typelisttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/typeutilitytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/utilitytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/vcexpectedimpltest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/test/versiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/timer.hh
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/to_unique_ptr.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8565 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/transpose.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18278 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/tupleutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/tuplevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7725 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/typelist.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21514 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/typetraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/typeutilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/unused.hh
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/vc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11137 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/version.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/common/visibility.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.016029 dune-common-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.020028 dune-common-2.9.0rc1/dune/python/common/
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/densematrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7668 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/densevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/dimrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/dynmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/dynvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/fmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/fvecmatregistry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/fvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/getdimension.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/logger.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3301 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/mpihelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/numpycommdatahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/numpyvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/pythonvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/string.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18528 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/typeregistry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9419 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/common/vector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.020028 dune-common-2.9.0rc1/dune/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    21396 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    93950 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)     8185 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.020028 dune-common-2.9.0rc1/dune/python/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27803 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (121)    39912 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (121)    16397 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (121)    16373 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (121)    29086 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (121)     7843 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/extensions.h
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (121)    69310 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (121)   107828 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (121)    65764 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (121)    14136 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (121)    23356 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.020028 dune-common-2.9.0rc1/dune/python/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/test/pythontests.py
--rw-r--r--   0 runner    (1001) docker     (121)     6200 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/test/test_embed1.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune/python/test/test_embed2.cc
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune-common.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.020028 dune-common-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18396 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/lib/dunemodules.lib
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/common/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/_common.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5329 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/checkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/hashit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/locking.py
--rw-r--r--   0 runner    (1001) docker     (121)    16594 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/module.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/project.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/common/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/deprecate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/generator/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)    37172 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/cmakebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7352 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/importclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/generator/template/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/CMakeLists.txt.template
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/config.h.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/dune-py.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/dune.module.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/generator/template/python/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/generated/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/generated/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/generated/CMakeLists.txt.template
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/generator/template/python/dune/generated/extractCompiler.cc
--rw-r--r--   0 runner    (1001) docker     (121)    24220 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    11330 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune/typeregistry/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/typeregistry/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/typeregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/typeregistry/_typeregistry.cc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/python/dune_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16560 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/dune_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/pyproject.toml.in
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/python/setup.py.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:49.028029 dune-common-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/share/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/share/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.024028 dune-common-2.9.0rc1/share/bash-completion/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/share/bash-completion/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:49.028029 dune-common-2.9.0rc1/share/bash-completion/completions/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/share/bash-completion/completions/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-10-21 08:16:48.000000 dune-common-2.9.0rc1/share/bash-completion/completions/dunecontrol
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.307653 dune-common-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (121)    17848 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5195 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    21568 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)    21568 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/TODO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.267653 dune-common-2.9.dev20220529/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8570 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/dune-ctest
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5503 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/dune-git-whitespace-hook
+-rwxr-xr-x   0 runner    (1001) docker     (121)    32538 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/dunecontrol
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9403 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/dunepackaging.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19451 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/duneproject
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/find_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1699 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/rebuild-dune-pypi.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/bin/rmgenerated.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.267653 dune-common-2.9.dev20220529/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.271653 dune-common-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddBLASLapackFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddGMPFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddMETISFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddMPIFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddPTScotchFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddParMETISFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddQuadMathFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddSuiteSparseFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddTBBFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddThreadsFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/AddVcFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/CMakeBuiltinFunctionsDocumentation.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7078 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/CheckCXXFeatures.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    10453 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneAddLibrary.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneAddPybind11Module.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneCMakeCompat.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneCommonMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneDoc.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneDoxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    15422 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneEnableAllPackages.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneExecuteProcess.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    35263 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneInstance.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    13657 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneModuleDependencies.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     6356 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneModuleInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePathHelper.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePkgConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    16810 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneProject.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonCommonMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonDeprecations.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4067 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonFindPackage.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    19396 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonInstallPackage.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonTestCommand.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    12777 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DunePythonVirtualenv.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneReplaceProperties.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7128 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneSphinxCMakeDoc.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneSphinxDoc.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneStreams.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneSymlinkOrCopy.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    18004 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneTestMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/DuneUtilities.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindGMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindInkscape.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindLatexMk.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     6611 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindMETIS.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     5587 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPTScotch.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindParMETIS.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.271653 dune-common-2.9.dev20220529/cmake/modules/FindPkgConfig/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPkgConfig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    32639 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPkgConfig/FindPkgConfig.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.271653 dune-common-2.9.dev20220529/cmake/modules/FindPython3/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPython3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15617 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPython3/FindPython3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)   161804 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindPython3/Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindQuadMath.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindSphinx.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    10164 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindSuiteSparse.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/FindTBB.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/Headercheck.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7332 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/OverloadCompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/UseInkscape.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    11383 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/UseLatexMk.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/modules/latexmkrc.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.271653 dune-common-2.9.dev20220529/cmake/pkg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/pkg/dune-common-config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/cmake/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/CreateDoxyFile.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/FinalizeHeadercheck.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/InstallFile.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/RunDoxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/WritePythonCMakeMetadata.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/checkvenvconf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/conf.py.in
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4147 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/extract_cmake_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/index.rst.in
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/main77.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/module_library.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/pyversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      487 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/run-in-dune-env.sh.in
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6639 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/sphinx_cmake_dune.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/cmake/scripts/venvpath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5753 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/buildsystem/
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/buildsystem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16885 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/buildsystem/dune-common.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/buildsystem/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/buildsystem/examples/Toolchain-Ubuntu-mingw32.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/buildsystem/examples/opts.mingw32
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/comm/
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/buildindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/communication.bib
+-rw-r--r--   0 runner    (1001) docker     (121)    24490 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/communication.tex
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/comm/figures/
+-rw-r--r--   0 runner    (1001) docker     (121)     6219 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/figures/darray.eps
+-rw-r--r--   0 runner    (1001) docker     (121)   192094 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/figures/distindex.eps
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/indexset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/poosc08.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/poosc08_test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/comm/reverse.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/Doxystyle
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/doxygen-macros
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/doxygen/modules.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/doc/dunecontrol.1
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.275653 dune-common-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.283653 dune-common-2.9.dev20220529/dune/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/alignedallocator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19581 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/arraylist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/assertandreturn.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/bartonnackmanifcheck.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18390 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/bigunsignedint.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/binaryfunctions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17638 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/bitsetvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/boundschecking.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/classname.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10395 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/concept.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/conditional.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/debugalign.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    19028 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/debugalign.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/debugallocator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9617 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/debugallocator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12825 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/debugstream.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    38543 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/densematrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21027 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/densevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/deprecated.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28261 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/diagonalmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/documentation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/dotproduct.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4057 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/dynmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/dynmatrixev.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5438 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/dynvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/enumset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/exceptions.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7954 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/filledarray.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19370 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/float_cmp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15176 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/float_cmp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22780 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/fmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10590 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/fmatrixev.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    25127 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/fmatrixev.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/ftraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17135 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/fvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7830 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/genericiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/gmpfield.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12951 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/hash.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14071 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/hybridutilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/indent.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/indices.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/interfaces.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/ios_state.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/ios_state.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21714 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/iteratorfacades.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/iteratorrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/keywords.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/lru.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/mallocallocator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11378 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/math.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/matvectraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/modules.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/overloadset.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.287653 dune-common-2.9.dev20220529/dune/common/parallel/
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.287653 dune-common-2.9.dev20220529/dune/common/parallel/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/benchmark/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11872 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/benchmark/mpi_collective_benchmark.cc
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/benchmark/options.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/collectivecommunication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20082 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/communication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    52369 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/communicator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/future.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    31581 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    41792 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/indicessyncer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15340 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/localindex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpicollectivecommunication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15501 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpicommunication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpidata.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpifuture.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6362 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpiguard.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8733 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpihelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5716 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpipack.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/mpitraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/plocalindex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    60265 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/remoteindices.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8518 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/selection.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.287653 dune-common-2.9.dev20220529/dune/common/parallel/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/communicationtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/indexsettest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/mpidatatest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/mpifuturetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/mpigatherscattertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/mpipacktest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    18472 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/remoteindicestest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/selectiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12166 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/syncertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13807 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/test/variablesizecommunicatortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    42317 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parallel/variablesizecommunicator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6306 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parameterizedobject.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parametertree.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10036 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parametertree.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7992 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parametertreeparser.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/parametertreeparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/path.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8268 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/path.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14640 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/poolallocator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/power.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/precision.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/promotiontraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8099 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/propertymap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/proxymemberaccess.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19086 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/quadmath.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28868 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/rangeutilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/referencehelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5482 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/reservedvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/scalarmatrixview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/scalarvectorview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/shared_ptr.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.287653 dune-common-2.9.dev20220529/dune/common/simd/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10596 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/DESIGN.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8838 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/base.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/defaults.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21490 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/io.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25013 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/loop.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/simd.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/standard.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.287653 dune-common-2.9.dev20220529/dune/common/simd/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/looptest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/looptest.hh.in
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/looptest_vector.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/standardtest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/standardtest.hh.in
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/standardtest_vector.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vcarraytest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vcarraytest.hh.in
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vctest_mask.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vctest_simdarray.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vctest_simdmaskarray.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vctest_vector.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vcvectortest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test/vcvectortest.hh.in
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    79335 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/test.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    31088 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd/vc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14132 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/simd.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/singleton.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19738 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/sllist.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.291653 dune-common-2.9.dev20220529/dune/common/std/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/apply.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/functional.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/make_array.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9853 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/type_traits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/utility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/std/variant.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/stdstreams.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/stdstreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/stdthread.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/stdthread.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/streamoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/stringutility.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.295653 dune-common-2.9.dev20220529/dune/common/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    13253 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/alignedallocatortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    23296 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/arithmetictestsuite.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/arithmetictestsuitetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4205 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/arraylisttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/arraytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/assertandreturntest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/autocopytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/bigunsignedinttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/bitsetvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14823 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/boundscheckingmvtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/boundscheckingoptest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10118 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/boundscheckingtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/calloncetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/check_fvector_size.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/check_fvector_size_fail.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12050 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/checkmatrixinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5265 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/classnametest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/collectorstream.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/concept.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/constexprifelsetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/debugalignsimd.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/debugalignsimdtest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/debugalignsimdtest.hh.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/debugaligntest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11068 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/densematrixassignmenttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/densevectorassignmenttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/densevectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/diagonalmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/dummyiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10422 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/dynmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/dynvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12032 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/eigenvaluestest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/enumsettest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/filledarraytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    26636 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/fmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/functiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/fvectorconversion1d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15886 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/fvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/genericiterator_compile_fail.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/hybridutilitiestest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/indicestest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/iscallabletest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/iteratorfacadetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/iteratorfacadetest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/iteratorfacadetest2.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12984 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/iteratortest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/lrutest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mathclassifierstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mathtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/metistest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mpicollectivecommunication.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mpicommunicationtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mpiguardtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/mpihelpertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/overloadsettest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parameterizedobjectfactorysingleton.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parameterizedobjectfactorysingleton.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parameterizedobjecttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parametertreelocaletest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11807 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parametertreetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/parmetistest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5556 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/pathtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/poolallocatortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/powertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/quadmathtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12121 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/rangeutilitiestest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/referencehelpertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/reservedvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/scotchtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/shared_ptrtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/singletontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9966 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/sllisttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/stdapplytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/stdidentity.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/streamoperatorstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/streamtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/stringutilitytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/testdebugallocator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7484 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/testfloatcmp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/testsuite.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/timing.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/transposetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/tupleutilitytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7934 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/typelisttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/typeutilitytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/utilitytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/vcexpectedimpltest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/test/versiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/timer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/to_unique_ptr.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/transpose.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18103 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/tupleutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/tuplevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/typelist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21341 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/typetraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/typeutilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/unused.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/vc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10962 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/version.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/common/visibility.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.295653 dune-common-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/dune/python/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2698 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/densematrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7493 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/densevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/dimrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/dynmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/dynvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3934 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/fmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/fvecmatregistry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6074 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/fvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/getdimension.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/logger.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/mpihelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/numpycommdatahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/numpyvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/pythonvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/string.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18353 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/typeregistry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9244 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/common/vector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/dune/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21396 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    93950 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8185 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/dune/python/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    27803 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (121)    39912 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16397 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16373 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29086 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7843 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/extensions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    69310 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (121)   107825 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (121)    65764 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (121)    14136 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23356 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/dune/python/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/test/pythontests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5984 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/test/test_embed1.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune/python/test/test_embed2.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune-common.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18223 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/lib/dunemodules.lib
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.299653 dune-common-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/_common.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5155 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/checkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/hashit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/locking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16419 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5751 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/common/utility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7997 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/deprecate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/generator/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5179 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17511 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/cmakebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7177 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/importclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/generator/template/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/CMakeLists.txt.template
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/config.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/dune-py.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/dune.module.template
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/generator/template/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/generator/template/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/generator/template/python/dune/generated/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/python/dune/generated/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/generator/template/python/dune/generated/CMakeLists.txt.template
+-rw-r--r--   0 runner    (1001) docker     (121)    23976 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11156 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune/typeregistry/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/typeregistry/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/typeregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/typeregistry/_typeregistry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/dune/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/python/dune_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-05-29 21:03:28.000000 dune-common-2.9.dev20220529/python/dune_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15923 2022-05-29 21:03:28.000000 dune-common-2.9.dev20220529/python/dune_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:28.000000 dune-common-2.9.dev20220529/python/dune_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-05-29 21:03:28.000000 dune-common-2.9.dev20220529/python/dune_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:28.000000 dune-common-2.9.dev20220529/python/dune_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/pyproject.toml.in
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/python/setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:28.307653 dune-common-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/share/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/share/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/share/bash-completion/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/share/bash-completion/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:28.303653 dune-common-2.9.dev20220529/share/bash-completion/completions/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/share/bash-completion/completions/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-05-29 21:03:27.000000 dune-common-2.9.dev20220529/share/bash-completion/completions/dunecontrol
```

### Comparing `dune-common-2.9.0rc1/CHANGELOG.md` & `dune-common-2.9.dev20220529/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 # Master (will become release 2.9)
 
 - Added feature test for lambdas in unevaluated contexts
   `DUNE_HAVE_CXX_UNEVALUATED_CONTEXT_LAMBDA`. When defined, the C++ language
   allows to declare lambdas in unevaluated contexts, e.g., `F = decltype([](){})`.
 
 ## Dependencies
@@ -14,36 +9,22 @@
 
 - C++ compiler supporting c++-17 language standard, e.g., LLVM Clang >= 5, GCC g++ >= 7
 - CMake >= 3.13
 - Optional: pkg-config to find other optional dependencies
 - Optional: Python >= 3.7 for Python bindings
 
 ## Changelog
-- Multiplication of two matrices using `a*b` is now also implemented if `a` or `b`
-  is a `FieldMatrix` or if both are `DiagonalMatrices`.
-
-- The utility function `transpose(m)` will now return `m.transposed()` if available.
-  Otherwise it returns a wrapper storing a copy (this was a reference before) of `m`.
-  References to matrices can still be captured using `transpose(std::ref(m))` or
-  `transposedView(m)`.
-
-- The transposed of a `FieldMatrix`, `DiagonalMatrix`, and `DynamicMatrix`
-  is now available using the `transposed()` member function.
-
 - Add helper function `resolveRef()` to transparently use `std::reference_wrapper`.
 
 - Add `pragma omp simd` annotations in the LoopSIMD class to improve compiler optimizations
 
 - deprecate Factorial in common/math.hh (use factorial function)
 
 - Add `python -m dune [info|configure|list|remove|dunetype|fix-dunepy]` command to manage just-in-time generated python modules in dune-py
 
-- The storage type `ReservedVector` is extended to follow more closely the `std::vector` and
-  `std::array` interfaces.
-
 ## Build System
 
 - Improve the the function `dune_add_library` by separating the target types normal, interface, and
   object. Additional properties can be passed to the cmake function like `LINK_LIBRARIES`,
   `OUTPUT_NAME`, and `EXPORT_NAME`
 
 - Remove the variable `DUNE_DEFAULT_LIBS`
@@ -57,34 +38,18 @@
   python bindings are now enabled by default. Packages are automatically installed
   either in an internal virtual environment or in an active environment during the
   module build process.
   See https://gitlab.dune-project.org/core/dune-common/-/merge_requests/960
   which also contains a detailed set of instructions on how to update
   existing python bindings.
 
-- Deprecated `dune_python_install_package`. Use either
-  `dune_python_configure_bindings` (for Python bindings)
-  `dune_python_configure_package` (for pure Python package).
-  See https://gitlab.dune-project.org/core/dune-common/-/merge_requests/1148
-  for more details.
-  Note that this MR also includes
-  https://gitlab.dune-project.org/core/dune-common/-/merge_requests/1103:
-  the Python bindings are not installed editable during the configure stage
-  instead of the build stage.
-
-- dune-py is now build using a simple 'Makefile' per module instead of
-  relying on cmake for each module. The old cmake builder can still be used
-  by exporting the environment variable `DUNE_PY_USE_CMAKEBUILDER=1`.
-
 - Remove deprecated cmake function overload `target_link_libraries`
 
 - Deprecate cmake function `remove_processed_modules`
 
-- The CI system now checks for common spelling mistakes using the `codespell` tool.
-
 ## Deprecations and removals
 
 - Helper fallback implementations for `Std::to_false_type`, `Std::to_true_type`,
   `Std::is_invocable`, and `Std::is_invocable_r` have been removed. Instead,
   use `Dune::AlwaysFalse`, `Dune::AlwaysTrue`, `std::is_invocable`, and
   `std::is_invocable_r`.
```

### Comparing `dune-common-2.9.0rc1/CMakeLists.txt` & `dune-common-2.9.dev20220529/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 cmake_minimum_required(VERSION 3.13)
 project(dune-common LANGUAGES C CXX)
 
 # make sure our own modules are found
 list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/cmake/modules)
 
 #include the dune macros
```

### Comparing `dune-common-2.9.0rc1/CONTRIBUTING.md` & `dune-common-2.9.dev20220529/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 Contributing to the Dune Core Modules
 =====================================
 
 You've squashed an annoying bug or implemented a nifty new feature in DUNE?
 And you're willing to share your improvements with the community? This page
 explains how to get those changes to us and what to take care of.
```

### Comparing `dune-common-2.9.0rc1/COPYING` & `dune-common-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/INSTALL` & `dune-common-2.9.dev20220529/INSTALL`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 Installation Instructions
 =========================
 
 For a full explanation of the DUNE installation process please read
 the installation notes [0]. The following introduction is meant for
 the impatient.
```

### Comparing `dune-common-2.9.0rc1/LICENSE.md` & `dune-common-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/PKG-INFO` & `dune-common-2.9.dev20220529/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-common
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Basis infrastructure for all Dune modules
 Home-page: https://gitlab.dune-project.org/core/dune-common
 Author: The Dune Core developers
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
-Description: <!--
-        SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-        SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-        -->
-        
-        DUNE-library
+Description: DUNE-library
         ============
         
         DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
         for solving partial differential equations with grid-based methods.
         
         The main intention is to create slim interfaces allowing an efficient use of
         legacy and/or new libraries. Using C++ techniques DUNE allows one to use very
@@ -85,15 +80,15 @@
         1. https://dune-project.org/releases/
         2. https://dune-project.org/buildsystem/
         3. http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
         
         [installation]: https://www.dune-project.org/doc/installation
         [licence]: http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
         
-        git-d7eff87fdf39ee6ad4fb9d993d9cabe9937d42c1
+        git-e8aec08f5a38b387f154ea7838c7e09d728c7615
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-common-2.9.0rc1/README.md` & `dune-common-2.9.dev20220529/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 DUNE-library
 ============
 
 DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
 for solving partial differential equations with grid-based methods.
 
 The main intention is to create slim interfaces allowing an efficient use of
@@ -77,8 +72,8 @@
 1. https://dune-project.org/releases/
 2. https://dune-project.org/buildsystem/
 3. http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
 
 [installation]: https://www.dune-project.org/doc/installation
 [licence]: http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
 
-git-d7eff87fdf39ee6ad4fb9d993d9cabe9937d42c1
+git-e8aec08f5a38b387f154ea7838c7e09d728c7615
```

### Comparing `dune-common-2.9.0rc1/bin/dune-ctest` & `dune-common-2.9.dev20220529/bin/dune-ctest`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #! /usr/bin/env python3
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #
 # Wrapper around CTest for DUNE
 #
 # CTest returns with an error status not only when tests failed, but also
 # when tests were only skipped.  This wrapper checks the log and returns
 # successfully if no tests failed; skipped tests do not result in an error.
 # This behaviour is needed in a continuous integration environment, when
```

### Comparing `dune-common-2.9.0rc1/bin/dune-git-whitespace-hook` & `dune-common-2.9.dev20220529/bin/dune-git-whitespace-hook`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/bin/sh
 # dune-git-whitespace-hook
 # DO NOT TOUCH THE PRECEDING LINE
 # It is used by dunecontrol to enable automatic updates of the whitespace hook
-#
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#
+
 # DUNE pre-commit hook to enforce whitespace policy
 # This hook prevents adding lines with trailing whitespace and or tab characters
 # in line indentation for certain files (see the TRAILING_WHITESPACE_DEFAULT and
 # TAB_IN_INDENT_DEFAULT variables below for the default sets of files that will
 # be checked).
 # You can tell the hook which files should be inspected by setting the Git
 # configuration variables "hooks.whitespace.trailing" and "hooks.whitespace.tabinindent".
```

### Comparing `dune-common-2.9.0rc1/bin/dunecontrol` & `dune-common-2.9.dev20220529/bin/dunecontrol`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/env bash
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 set -e
 
 ###############################################
 ###
 ### check for environment variables
 ###
@@ -51,15 +49,15 @@
     token=${val%%[\"\$\`\\]*}
     val=${val#"$token"}
     special=${val:0:1}
     val=${val:1}
     result=$result$token${special:+\\$special}
   done
   # if the value ends in \n, protect it by appending two double-quotes so it
-  # won't get stripped by the surrounding $(...)
+  # wont get stripped by the surrounding $(...)
   case $result in
     *"$nl") result=$result'""';;
   esac
   printf "%s" "$result"
 }
 
 canonicalname(){
@@ -815,15 +813,15 @@
   if test "x$REVERSE_FLAG" = "xyes"; then
     export MODULES="$REVERSEMODULES"
   fi
 
   if test "x$SKIPFIRST" = "xyes" ; then
     export MODULES=`echo $MODULES " " | cut '--delimiter= ' --fields=2-`
   fi
-  # warn about superseded modules:
+  # warn about superseeded modules:
   if test -n "$superseded_modules"; then
     # sort moules list and make it unique.
     superseded_modules=$(echo $superseded_modules | tr ' ' '\n'| sort -u)
     echo >&2
     echo "The following local modules do supersede the corresponding installed ones:"  >&2
     echo "$superseded_modules"  >&2
     echo  >&2
```

### Comparing `dune-common-2.9.0rc1/bin/dunepackaging.py` & `dune-common-2.9.dev20220529/bin/dunepackaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/env python3
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 try:
     import skbuild
 except ImportError:
     print("skbuild needed for packaging, run 'pip install scikit-build'")
     import sys
     sys.exit(0)
```

### Comparing `dune-common-2.9.0rc1/bin/duneproject` & `dune-common-2.9.dev20220529/bin/duneproject`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env bash
 # -*- indent-tabs-mode: nil; sh-basic-offset: 2; sh-indentation: 2 -*-
 # vi: set et sw=2:
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 # The sh-indentation in the emacs mode-line is needed for emacs <26, see
 # https://debbugs.gnu.org/21751
 
 #
 # TODO:
 #
@@ -70,18 +68,18 @@
     depends="$depends `pkg_config_dependencies $pkg`"
   done
   echo $depends
 }
 
 # modulesexist DEPS MODULES
 #
-# DEPS is a space-separated list of modules the new module should depend on.
-# MODULES is a space-separated list of modules that are known to be present.
+# DEPS is a space seperated list of modules the new module should depend on
+# MODULES is a space seperated list of modules that are known to be present
 #
-# Each name in DEPS is checked to see whether it is present in MODULES.  If
+# Each name in DEPS is checked to see wether it is present in MODULES.  If
 # not, is is checked whether it can be found with pkg-config.  If still no, an
 # error message is issued and modulesexist will return with an exit status
 # indicating failure.
 modulesexist(){
   local status dep found
   status=0
 
@@ -239,15 +237,15 @@
     read -p "4) Maintainer's email address? " MAINTAINER
   done
 
   echo
   echo "creating Project \"$PROJECT\", version $VERSION "
   echo "which depends on \"$DEPENDENCIES\""
   echo "with maintainer \"$MAINTAINER\""
-  read -p "Is this information correct? [y/N] " DATACORRECT
+  read -p "Are these informations correct? [y/N] " DATACORRECT
 
   # reset data if necessary
   if [ "$DATACORRECT" != "y" -a "$DATACORRECT" != "Y" ]; then
     PROJECT=""
     DEPENDENCIES=""
     VERSION=""
     MAINTAINER=""
```

### Comparing `dune-common-2.9.0rc1/bin/find_modules.py` & `dune-common-2.9.dev20220529/bin/find_modules.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 try:
     from dune.common.module import resolve_dependencies, resolve_order, select_modules
 
 except ImportError:
     import os
     here = os.path.dirname(os.path.abspath(__file__))
     mods = os.path.join(os.path.dirname(here), "python", "dune", "common")
```

### Comparing `dune-common-2.9.0rc1/bin/rebuild-dune-pypi.sh` & `dune-common-2.9.dev20220529/bin/rebuild-dune-pypi.sh`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/bin/bash
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
+
 #
 # This script builds a Python package index on gitlab.dune-project.org. Such an
 # index is necessary as a drop-in replacement for PyPI in continuous integration,
 # when runners operate with restricted network access.
 #
 # Running this script requires the following prerequisites to be met:
 # * Go to Gitlab Profile/Setting/Access Tokens and create a personal API access token with
@@ -32,32 +31,31 @@
 pushd $TMPDIR
 
 python3 -m venv env
 source env/bin/activate
 python -m pip install pip-download twine
 
 pip-download -d $(pwd)/downloads \
-  # dune-common \
-  # dune-geometry \
-  # dune-grid \
-  # dune-istl \
-  # dune-localfunctions \
-  # dune-alugrid \
-  # dune-fem \
+  dune-common \
+  dune-geometry \
+  dune-grid \
+  dune-istl \
+  dune-localfunctions \
+  dune-alugrid \
+  dune-fem \
   pyparsing \
   mpi4py \
   wheel \
   setuptools \
   jinja2 \
   portalocker \
   fenics-ufl==2019.1.0 \
   matplotlib \
   scipy \
   pip>=21 \
-  ninja \
   sortedcontainers
 
 
 # Upload the packages to the index
 for filename in downloads/*
 do
   # NB: The 133 here is the Gitlab project ID of dune-common.
```

### Comparing `dune-common-2.9.0rc1/bin/rmgenerated.py` & `dune-common-2.9.dev20220529/bin/rmgenerated.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/env python3
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 import sys
 from dune.generator.remove import removeGenerated
 from argparse import ArgumentParser
 parser = ArgumentParser(description='Removing generated module from dune-py')
 parser.add_argument('-a', '--all', help='remove all modules', action='store_true', default=False)
 parser.add_argument('modules', metavar='M', nargs='*',
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddBLASLapackFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddBLASLapackFlags.cmake`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use BLAS/Lapack
 #
 # .. cmake_function:: add_dune_blas_lapack_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddGMPFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddGMPFlags.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use GMP
 #
 # .. cmake_function:: add_dune_gmp_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddMETISFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddMETISFlags.cmake`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use METIS
 #
 # .. cmake_function:: add_dune_metis_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddMPIFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddMPIFlags.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # The DUNE way to compile MPI applications is to use the CXX
 # compiler with MPI flags usually used for C. CXX bindings
 # are deactivated to prevent ABI problems.
 #
 # .. cmake_function:: add_dune_mpi_flags
 #
 #    .. cmake_param:: targets
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddPTScotchFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddPTScotchFlags.cmake`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use PTScotch
 #
 # .. cmake_function:: add_dune_ptscotch_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddQuadMathFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddQuadMathFlags.cmake`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use QuadMath
 #
 # .. cmake_function:: add_dune_quadmath_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddSuiteSparseFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddSuiteSparseFlags.cmake`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use SuiteSparse
 #
 # .. cmake_function:: add_dune_suitesparse_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/AddTBBFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/AddTBBFlags.cmake`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use TBB
 #
 # .. cmake_function:: add_dune_tbb_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/CMakeBuiltinFunctionsDocumentation.cmake` & `dune-common-2.9.dev20220529/cmake/modules/CMakeBuiltinFunctionsDocumentation.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This modules contains only documentation for CMake builtins.
 # This is necessary to have an complete API documentation.
 #
 # .. cmake_function:: add_subdirectory
 #
 #    .. cmake_param:: dir
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/CMakeLists.txt` & `dune-common-2.9.dev20220529/cmake/modules/CMakeLists.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory(FindPkgConfig)
 add_subdirectory(FindPython3)
 
 install(FILES
   AddBLASLapackFlags.cmake
   AddGMPFlags.cmake
   AddMETISFlags.cmake
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/CheckCXXFeatures.cmake` & `dune-common-2.9.dev20220529/cmake/modules/CheckCXXFeatures.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Module that checks for supported C++20, C++17 and non-standard features.
 #
 #    The behaviour of this module can be modified by the following variable:
 #
 #    :ref:`DISABLE_CXX_VERSION_CHECK`
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneAddLibrary.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneAddLibrary.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneAddLibrary
 --------------
 
 Add a library to a Dune module.
 
 .. cmake:command:: dune_add_library
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneAddPybind11Module.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneAddPybind11Module.cmake`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This cmake module provides infrastructure for building modules using Pybind11
 #
 # .. cmake_function:: dune_add_pybind11_module
 #
 #    .. cmake_param:: NAME
 #       :required:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneCommonMacros.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneCommonMacros.cmake`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # enforce C++-14
 dune_require_cxx_standard(MODULE "dune-common" VERSION 14)
 
 include(DuneStreams)
 dune_set_minimal_debug_level()
 
 # search for lapack
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneDoc.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneDoc.cmake`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #
 # Module that provides a custom target make doc at the top level
 # directory and utility macros for creating install directives
 # that make sure that the files to be installed are previously
 # generated even if make doc was not called.
 #
 # All documentation (Latex, Doxygen) will be generated during
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneDoxygen.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneDoxygen.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module for building documentation using doxygen.
 #
 # .. cmake_function:: add_doxygen_target
 #
 #    .. cmake_param:: TARGET
 #       :single:
 #
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneEnableAllPackages.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneEnableAllPackages.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Implementation of a simplified CMake build system.
 #
 # .. cmake_function:: dune_enable_all_packages
 #
 #    .. cmake_brief::
 #
 #       Previously, the DUNE build system relied on the user to choose and add the compile and link flags
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneExecuteProcess.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneExecuteProcess.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # An error checking wrapper around the cmake command execute_process
 #
 # .. cmake_command:: dune_execute_process
 #
 #    .. cmake_param:: ERROR_MESSAGE
 #       :single:
 #
@@ -13,50 +10,39 @@
 #
 #    .. cmake_param:: WARNING_MESSAGE
 #       :single:
 #
 #       A warning message to show if command exited with non-zero exit code.
 #       This will not abort the current cmake run.
 #
-#    .. cmake_param:: WORKING_DIRECTORY
-#       :single:
-#
-#       The named directory will be set as the current working directory of the
-#       child processes.
-#
 #    Note, that if neither warning or error message is provided, no return
 #    code checking is done. If both are given the error message will be
 #    used and the cmake run aborted.
 #
 #    A thin wrapper around the cmake command :code:`execute_process`, that
 #    exits on non-zero exit codes. All arguments are forwarded to the actual
 #    cmake command.
 #
 include_guard(GLOBAL)
 
 function(dune_execute_process)
-  set(SINGLEARGS ERROR_MESSAGE WARNING_MESSAGE RESULT_VARIABLE OUTPUT_VARIABLE ERROR_VARIABLE WORKING_DIRECTORY)
+  set(SINGLEARGS ERROR_MESSAGE WARNING_MESSAGE RESULT_VARIABLE OUTPUT_VARIABLE ERROR_VARIABLE)
   cmake_parse_arguments(EXECUTE "" "${SINGLEARGS}" "" ${ARGN})
 
   # Decide whether stdout and stderr have to be split
   if(EXECUTE_OUTPUT_VARIABLE AND EXECUTE_ERROR_VARIABLE)
     set(SPLIT_ERROR TRUE)
     set(ERRLOGVAR errlog)
   else()
     set(SPLIT_ERROR FALSE)
     set(ERRLOGVAR log)
   endif()
 
-  if (NOT EXECUTE_WORKING_DIRECTORY)
-    set(EXECUTE_WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR})
-  endif()
-
   # Call the original cmake function
   execute_process(${EXECUTE_UNPARSED_ARGUMENTS}
-                  WORKING_DIRECTORY ${EXECUTE_WORKING_DIRECTORY}
                   RESULT_VARIABLE retcode
                   OUTPUT_VARIABLE log
                   ERROR_VARIABLE ${ERRLOGVAR}
                   )
 
   # Issue an error if requested!
   if(EXECUTE_ERROR_MESSAGE)
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneInstance.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneInstance.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module to generate instantiations, typically for some template
 #
 # .. cmake_module::
 #
 #    This module can be used to generate explicit template instantiations.
 #    Suppose you have a template test function that you want to call for a
 #    number of template arguments.  You want to explicitly instantiate the
-#    function for each set of template arguments, and put the instantiation
+#    function for each set of template arguments, and put the instanciation
 #    into its own translation unit.  (This can be beneficial in that it limits
 #    the amount of code that the optimizer sees at once, and thus it can
 #    reduce both memory and cpu requirements during compilation.)
 #
 #    .. rubric:: Examples
 #
 #    Let's say you are writing a test ``mytest.cc`` and need to call a
@@ -80,20 +77,20 @@
 #
 #      list(FILTER DUNE_INSTANCE_GENERATED INCLUDE REGEX [[\.cc$]])
 #      dune_add_test(NAME mytest
 #        SOURCES ${DUNE_INSTANCE_GENERATED})
 #
 #    The call to :ref:`dune_instance_begin() <dune_instance_begin>` reads
 #    ``mytest.cc.in`` and ``mytest.hh.in`` and splits them into embedded
-#    templates and other content.  It will replace occurrences of ``@VAR@``
+#    templates and other content.  It will replace occurrances of ``@VAR@``
 #    now in the other content and save the result for later.
 #
 #    The call to :ref:`dune_instance_add() <dune_instance_add>` occurs in a
-#    loop.  Each call will instantiate the embedded templates extracted
-#    earlier to replace an occurrence of ``@TYPE@`` by the value of the variable
+#    loop.  Each call will instanciate the embedded templates extracted
+#    earlier to replace occurance of ``@TYPE@`` by the value of the variable
 #    ``TYPE`` set in the for loop.  Then files containing explicit
 #    instantiatons will be generated as ``mytest_instance_bool.cc``,
 #    ``mytest_instance_bool.cc``, etc, from a template file
 #    ``mytest_instance.cc.in``.  The name of the generated files are the base
 #    file name from the template definition with the ``ID`` inserted before
 #    the extension.  The name of the template file is the same base file name
 #    with ``.in`` appended.
@@ -154,15 +151,15 @@
 #    instantiated by :ref:`dune_instance_add() <dune_instance_add>`, and all
 #    instantiations will be concatenated together and replace the original
 #    embedded template.
 #
 #    The begin of an embedded template is marked by a line containing
 #    ``@template@`` or ``@template NAME@``.  Leaving off the name is
 #    equivalent to an empty name.  ``dune_instance_add(TEMPLATE NAME)`` will
-#    only instantiate embedded templates whose name matches and ignore all
+#    only instanciate embedded templates whose name matches and ignore all
 #    others.
 #
 #    The end of an embedded template is marked by a line containing
 #    ``@endtemplate@`` or ``@endtemplate NAME@``.  If a name is given, it must
 #    match the name of the embedded template it closes.  If no name is given
 #    (or the name is empty), that check is omitted.
 #
@@ -180,15 +177,15 @@
 #    up the variables to substitute before calling :ref:`dune_instance_add()
 #    <dune_instance_add>` or :ref:`dune_instance_begin()
 #    <dune_instance_begin>`.
 #
 #    Refrain from using substitutions that begin with an underscore
 #    (i.e. ``@_my_local_var@``).  The generation functions in this module use
 #    such names for their local variables and may hide the variable you are
-#    trying to substitute.
+#    trying to substitude.
 #
 #    When instantiating files we set up a few convenience variables before
 #    calling ``configure_file()`` that can be used in substitutions:
 #    ``@TEMPLATE@`` contains the name of the template file.  ``@INSTANCE@``
 #    contains the name of the file being generated, not including an implied
 #    ``${CMAKE_CURRENT_BINARY_DIR}``.  Use ``@BINDIR_INSTANCE@`` if you do
 #    want the implied ``${CMAKE_CURRENT_BINARY_DIR}``.  ``@GENERATED_SOURCE@``
@@ -447,15 +444,15 @@
 #    includes hints for common editors telling them to switch to read-only
 #    mode.
 #
 #    Then generate the file as if by ``configure_file()``.
 #
 #    If the instance file has been registered as a generated source file
 #    before, this function generates a fatal error.  This ensures that any
-#    accidental attempt to generate the same file twice is caught.  As a
+#    accidential attempt to generate the same file twice is caught.  As a
 #    special exception, if the generated content is the same as before, the
 #    error is silently skipped.
 #
 #
 # .. cmake_variable:: DUNE_INSTANCE_GENERATED
 #
 #    After :ref:`dune_instance_end() <dune_instance_end>`, this holds the list
@@ -489,16 +486,16 @@
 # text is
 # - free of ';' characters.  This avoids problems when using list(APPEND),
 #   which does not quote ';' characters inside the appended element.  It would
 #   also avoid problems with list(INSERT), which mangles any cmake quoting in
 #   the list it inserts to, but we don't actually use that command.
 # - free of '\' characters.  This avoids problems with a list element that
 #   ends in a '\' merging with the next element, because the '\' quotes the
-#   ';' that is used to separate the elements
-# - non-empty.  This avoids the problem that cmake can't distinguish between
+#   ';' that is used to seperate the elements
+# - non-empty.  This avoids the problem that cmake can't destinguish between
 #   an empty list and a list with one empty element.
 function(dune_instance_quote_element VAR)
   set(content "${${VAR}}")
   string(REPLACE [[$]] [[$s]] content "${content}")
   string(REPLACE [[;]] [[$:]] content "${content}")
   string(REPLACE [[\]] [[$/]] content "${content}")
   if(content STREQUAL "")
@@ -676,15 +673,15 @@
         set(template_sep "${sep}")
         set(template_name "${sep_name}")
         set(template_lineno "${lineno}")
 
         set(in_template TRUE)
       endif()
       set(acc "")
-    else() # line did not match separator
+    else() # line did not match seperator
       string(APPEND acc "${line}")
     endif()
   endwhile()
 
   if(in_template)
     message(FATAL_ERROR "${name}:${template_lineno}: Unclosed '${template_sep}'")
   endif()
@@ -693,16 +690,16 @@
   list(APPEND content_list "${acc}")
 
   set("${content_parts}" "${content_list}" PARENT_SCOPE)
   set("${template_parts}" "${template_list}" PARENT_SCOPE)
   set("${template_names}" "${template_name_list}" PARENT_SCOPE)
 endfunction(dune_instance_parse_embedded)
 
-# Take the name of a list variable containing content parts other than
-# embedded templates and instantiate each part.  Put the result back into the
+# Take the name of a list variable containing content parts other then
+# embedded templates and instanciate each part.  Put the result back into the
 # same variable.  List elements are quoted.
 function(dune_instance_generate_parts _parts_list)
   set(_acc "")
   foreach(_part IN LISTS "${_parts_list}")
     dune_instance_unquote_element(_part)
     string(CONFIGURE "${_part}" _part)
     dune_instance_quote_element(_part)
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneMacros.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneMacros.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Core DUNE module for CMake.
 #
 # Documentation of the public API defined in this module:
 #
 # .. cmake_function:: dune_target_link_libraries
 #
 #    .. cmake_param:: BASENAME
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneModuleDependencies.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneModuleDependencies.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneModuleDependencies
 ----------------------
 
 Macros to extract dependencies between Dune modules by inspecting the
 ``dune.module`` files.
 
@@ -225,15 +222,15 @@
         ${${module}_PREFIX}/lib/dunecontrol/${module}/dune.module
         ${${module}_PREFIX}/lib64/dunecontrol/${module}/dune.module)
       if(EXISTS ${_dune_module_file})
         get_filename_component(_dune_module_file_path ${_dune_module_file} PATH)
         dune_module_information(${_dune_module_file_path})# QUIET)
         set(${module}_dune_module 1)
         set(DUNE_FIND_MOD_VERSION_STRING "${DUNE_VERSION_MAJOR}.${DUNE_VERSION_MINOR}.${DUNE_VERSION_REVISION}")
-        # check whether dependency matches version requirement
+        # check whether dependency mathes version requirement
         unset(module_version_wrong)
         if(DUNE_FIND_VERSION_OP MATCHES ">=")
           if(NOT (DUNE_FIND_MOD_VERSION_STRING VERSION_EQUAL DUNE_FIND_VERSION_STRING OR
                   DUNE_FIND_MOD_VERSION_STRING VERSION_GREATER DUNE_FIND_VERSION_STRING))
             set(module_version_wrong 1)
           endif()
         elseif(DUNE_FIND_VERSION_OP MATCHES "<=")
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneModuleInformation.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneModuleInformation.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneModuleInformation
 ---------------------
 
 Collect information about Dune Modules.
 
 .. cmake:command:: dune_module_information
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePathHelper.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePathHelper.cmake`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Some helper functions for people developing the CMake build system
 # to get quick and easy access to path variables of Dune modules.
 #
 # .. cmake_function:: dune_module_path
 #
 #    .. cmake_param:: MODULE
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePkgConfig.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePkgConfig.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # searches for pkg-config, creates the
 # file <module-name>.pc from <module-name>.pc.in,
 # and adds installation directives.
 #
 include_guard(GLOBAL)
 
 find_package(PkgConfig)
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneProject.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneProject.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneProject
 -----------
 
 Initialize and finalize a Dune module.
 
 .. cmake:command:: dune_project
@@ -49,17 +46,17 @@
 include(DuneSymlinkOrCopy)
 include(FeatureSummary)
 include(GNUInstallDirs)
 include(Headercheck)
 include(OverloadCompilerFlags)
 
 
-# Macro that should be called near the beginning of the top level CMakeLists.txt.
+# macro that should be called near the begin of the top level CMakeLists.txt.
 # Namely it sets up the module, defines basic variables and manages
-# dependencies.
+# depedencies.
 # Don't forget to call finalize_dune_project afterwards.
 macro(dune_project)
 
   # check if CXX flag overloading has been enabled (see OverloadCompilerFlags.cmake)
   initialize_compiler_script()
 
   # extract information from dune.module
@@ -123,27 +120,27 @@
   dune_process_dependency_macros()
 
   include(GNUInstallDirs)
   # Set variable where the cmake modules will be installed.
   # Thus the user can override it and for example install
   # directly into the CMake installation. We use a cache variable
   # that is overridden by a local variable of the same name if
-  # the user does not explicitly set a value for it. Thus the value
+  # the user does not explicitely set a value for it. Thus the value
   # will automatically change if the user changes CMAKE_INSTALL_DATAROOTDIR
   # or CMAKE_INSTALL_PREFIX
   if(NOT DUNE_INSTALL_MODULEDIR)
     set(DUNE_INSTALL_MODULEDIR ""
       CACHE PATH
-      "Installation directory for CMake modules. Default is \${CMAKE_INSTALL_DATAROOTDIR}/dune/cmake/modules when not set explicitly")
+      "Installation directory for CMake modules. Default is \${CMAKE_INSTALL_DATAROOTDIR}/dune/cmake/modules when not set explicitely")
     set(DUNE_INSTALL_MODULEDIR ${CMAKE_INSTALL_DATAROOTDIR}/dune/cmake/modules)
   endif()
   if(NOT DUNE_INSTALL_NONOBJECTLIBDIR)
     set(DUNE_INSTALL_NONOBJECTLIBDIR ""
       CACHE PATH
-      "Installation directory for libraries that are not architecture dependent. Default is lib when not set explicitly")
+      "Installation directory for libraries that are not architecture dependent. Default is lib when not set explicitely")
     set(DUNE_INSTALL_NONOBJECTLIBDIR lib)
   endif()
   # set up make headercheck
   include(Headercheck)
   setup_headercheck()
 
   # define that we found this module
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePythonCommonMacros.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePythonCommonMacros.cmake`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # The python extension of the Dune cmake build system
 #
 # .. cmake_module::
 #
 #    This module is the main entry point for the python extension of the Dune cmake
 #    build system. It handles the detection of the python installation, defines installation
 #    rules for python packages in Dune modules and provides virtual environments to
 #    run python code from cmake.
 #
-#    To disable any Python-related features use -DCMAKE_DISABLE_FIND_PACKAGE_Python3=TRUE
+#    To disable any python releated features use -DCMAKE_DISABLE_FIND_PACKAGE_Python3=TRUE
 #
 #    If you want to use Dune modules that provide Python functionality, you should be aware
 #    of some facts:
 #
 #    * CMake looks for your python interpreter during configure. If you want to have it
 #      work with a virtual environment, you should activate your virtualenv before configure.
 #    * Each module has an additional target :code:`make install_python`, that installs python packages
@@ -82,15 +79,15 @@
                    RESULT scriptdir
                    SCRIPT_DIR)
 
   # Check presence of python packages required by the buildsystem
   dune_python_find_package(PACKAGE pip)
 
   # Add python related meta targets
-  add_custom_target(test_python COMMAND ctest CMD_ARGS -L python)
+  add_custom_target(test_python)
   add_custom_target(install_python)
 
   # this option enables the build of Python bindings for DUNE modules
   option(DUNE_ENABLE_PYTHONBINDINGS "Enable Python bindings for DUNE" ON)
 
   if( DUNE_ENABLE_PYTHONBINDINGS )
     if(NOT Python3_Interpreter_FOUND)
@@ -120,28 +117,8 @@
 
     include(DuneAddPybind11Module)
   endif()
 
 
   # Set up the Dune-internal virtualenv
   include(DunePythonVirtualenv)
-
-  # Determine where to install python packages
-  if(DUNE_PYTHON_SYSTEM_IS_VIRTUALENV)
-    set(DUNE_PYTHON_INSTALL_LOCATION "system" CACHE STRING "Location of where to install python packages")
-  else()
-    set(DUNE_PYTHON_INSTALL_LOCATION "user" CACHE STRING "Location of where to install python packages")
-  endif()
-
-  if(NOT(("${DUNE_PYTHON_INSTALL_LOCATION}" STREQUAL "user") OR
-         ("${DUNE_PYTHON_INSTALL_LOCATION}" STREQUAL "system") OR
-         ("${DUNE_PYTHON_INSTALL_LOCATION}" STREQUAL "none") OR
-         ("${DUNE_PYTHON_INSTALL_LOCATION}" MATCHES "--target")   # this allows to provide a folder, i.e., --target /home/foo/site-packages
-    ))
-    message(FATAL_ERROR "DUNE_PYTHON_INSTALL_LOCATION must be user|system|none|--target <target>.")
-  endif()
-
-  if(("${DUNE_PYTHON_INSTALL_LOCATION}" STREQUAL "user") AND DUNE_PYTHON_SYSTEM_IS_VIRTUALENV)
-    message(FATAL_ERROR "Specifying 'user' as install location is incompatible with using virtual environments (as per pip docs)")
-  endif()
-
 endif()
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePythonFindPackage.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePythonFindPackage.cmake`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This module provides functions to check for the existence of python packages on the host system.
 #
 # .. cmake_function:: dune_python_find_package
 #
 #    .. cmake_param:: PACKAGE
 #       :required:
 #       :single:
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePythonTestCommand.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePythonTestCommand.cmake`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,69 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Wrap python testing commands into the CMake build system
 #
 # .. cmake_function:: dune_python_add_test
 #
 #    .. cmake_param:: SCRIPT
 #       :multi:
 #
 #       The script to execute using the python interpreter. It will be executed during :code:`make test_python`
 #       and during `ctest`. You are required to either pass SCRIPT or MODULE.
 #
 #       .. note::
 #
+#          The script will be executed using :code:`${Python3_EXECUTABLE} SCRIPT`. If the INTERPRETER
+#          option is given, that interpreter is used instead.
+#
 #    .. cmake_param:: MODULE
 #       :multi:
 #
-#       The Python module to execute using the python interpreter. It will be executed during :code:`make test_python`
+#       The Python module to be executed.  It will be executed during :code:`make test_python`
 #       and during `ctest`. You are required to either pass SCRIPT or MODULE.
 #
-#    .. cmake_param:: LABELS
-#       :multi:
+#       .. note::
 #
-#       A list of labels to add to the test. This sets
-#       the LABELS property on the test so :code:`ctest -L ${label_regex}` can
-#       be used to run all tests with certain labels. We always add the label
-#       :code:`python` per default. The labels are forwarded to
-#       :ref:`dune_add_test`. See :ref:`dune_add_test` for a
-#       more detailed documentation.
+#          The script will be executed using :code:`${Python3_EXECUTABLE} -m MODULE`. If the INTERPRETER
+#          option is given, that interpreter is used instead.
 #
 #    .. cmake_param:: WORKING_DIRECTORY
 #       :single:
 #       :argname: dir
 #
 #       The working directory of the command. Defaults to
 #       the current build directory.
 #
-#    .. cmake_param:: TIMEOUT
-#       :single:
-#
-#       If set, the test will time out after the given number of seconds. This supersedes
-#       any timeout setting in ctest (see `cmake --help-property TIMEOUT`). If you
-#       specify the MPI_RANKS option, you need to specify a TIMEOUT.
-#
 #    .. cmake_param:: NAME
 #       :single:
 #
 #       A name to identify this test in ctest. Names must be unique throughout
 #       the project. If omitted, defaults to mangling of the command.
 #
 #    Integrates a python testing framework command into the Dune
 #    build system. Added commands are run, when the target
 #    :code:`test_python` is built and during :code:`ctest`.
 #
-#    This function uses `dune_add_test` and forwards all unparsed arguments.
-#
 include_guard(GLOBAL)
 
 function(dune_python_add_test)
   # Parse Arguments
   set(OPTION)
-  set(SINGLE NAME WORKING_DIRECTORY)
-  set(MULTI SCRIPT MODULE LABELS TIMEOUT)
+  set(SINGLE WORKING_DIRECTORY NAME)
+  set(MULTI SCRIPT COMMAND LABELS MODULE)
   cmake_parse_arguments(PYTEST "" "${SINGLE}" "${MULTI}" ${ARGN})
   if(PYTEST_COMMAND)
     message(FATAL_ERROR "dune_python_add_test: COMMAND argument should not be used, use SCRIPT instead providing only the Python script and not the Python interpreter")
   endif()
-
-  # Apply defaults
-  set(PYTEST_LABELS ${PYTEST_LABELS} python)
-  if(NOT PYTEST_TIMEOUT)
-    set(PYTEST_TIMEOUT 3600)
+  if(PYTEST_UNPARSED_ARGUMENTS)
+    message(WARNING "Unparsed arguments in dune_python_add_test: This often indicates typos!")
   endif()
 
+  # Apply defaults
   if(NOT PYTEST_WORKING_DIRECTORY)
     set(PYTEST_WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR})
   endif()
-
   if((NOT PYTEST_MODULE) AND (NOT PYTEST_SCRIPT))
     message(FATAL_ERROR "dune_python_add_test: Either SCRIPT or MODULE need to be specified!")
   endif()
   if(PYTEST_MODULE AND PYTEST_SCRIPT)
     message(FATAL_ERROR "dune_python_add_test: You can only specify either SCRIPT or MODULE, not both!")
   endif()
   if(PYTEST_MODULE)
@@ -91,22 +74,32 @@
     foreach(comm ${PYTEST_SCRIPT})
       set(commandstr "${commandstr}_${comm}")
     endforeach()
     set(commandstr "${commandstr}_${PYTEST_WORKING_DIRECTORY}")
     string(REPLACE "/" "_" PYTEST_NAME ${commandstr})
   endif()
 
-  set(PYTEST_COMMAND ${CMAKE_BINARY_DIR}/run-in-dune-env)
-  set(PYTEST_CMD_ARGS python ${PYTEST_SCRIPT})
-
-  add_custom_target(target_${PYTEST_NAME})
-  dune_add_test(NAME ${PYTEST_NAME}
-                TARGET target_${PYTEST_NAME}
-                COMMAND ${PYTEST_COMMAND}
-                CMD_ARGS ${PYTEST_CMD_ARGS}
-                PYTHON_TEST
-                LABELS ${PYTEST_LABELS}
-                WORKING_DIRECTORY ${PYTEST_WORKING_DIRECTORY}
-                TIMEOUT ${PYTEST_TIMEOUT}
-                ${PYTEST_UNPARSED_ARGUMENTS}
-               )
+  if(DUNE_PYTHON_VENVSETUP)
+    # Actually run the command
+    add_custom_target(target_${PYTEST_NAME}
+                      COMMAND ${CMAKE_BINARY_DIR}/run-in-dune-env python ${PYTEST_SCRIPT}
+                      WORKING_DIRECTORY ${PYTEST_WORKING_DIRECTORY})
+  else()
+    add_custom_target(target_${PYTEST_NAME}
+                      COMMAND ${CMAKE_COMMAND} -E echo \"Test not run: python setup failed\")
+  endif()
+
+  # Build this during make test_python
+  add_dependencies(test_python target_${PYTEST_NAME})
+
+  # make sure each label exists and its name is acceptable
+  dune_declare_test_label(LABELS ${PYTEST_LABELS})
+
+  # Also build this during ctest
+  _add_test(NAME ${PYTEST_NAME}
+            COMMAND ${CMAKE_BINARY_DIR}/run-in-dune-env python ${PYTEST_SCRIPT}
+            WORKING_DIRECTORY ${PYTEST_WORKING_DIRECTORY}
+            )
+  set_tests_properties(${PYTEST_NAME} PROPERTIES SKIP_RETURN_CODE 77)
+  # Set the labels on the test
+  set_tests_properties(${PYTEST_NAME} PROPERTIES LABELS "${PYTEST_LABELS}")
 endfunction()
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DunePythonVirtualenv.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DunePythonVirtualenv.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Manage the creation of a configure-time virtual environment
 #
 # .. cmake_module::
 #
 #    This module manages the creation of virtual python environment during
 #    configuration. The purpose of this virtual environment is to be able to run
 #    python code from cmake in situations such as python-based code generation,
@@ -71,19 +68,14 @@
 #
 #    If that still does not help, set this variable to allow the Dune build system to download
 #    :code:`get-pip.py` from https://bootstrap.pypa.io/get-pip.py at configure time and execute
 #    it to install pip into the freshly set up virtual environment. While this should normally
 #    not be necessary anymore, see https://bugs.launchpad.net/debian/+source/python3.4/+bug/1290847
 #    for more information about the underlying distribution bug.
 #
-# .. cmake_variable:: DUNE_PYTHON_WHEELHOUSE
-#
-#    The place where python wheels are stored. Notice that this wheelhouse directory shall be
-#    the same for all dune installations.
-#
 include_guard(GLOBAL)
 
 # pre-populate DUNE_PYTHON_SYSTEM_IS_VIRTUALENV
 set(DUNE_PYTHON_SYSTEM_IS_VIRTUALENV "" CACHE PATH
   "Running in an external activated virtual environment"
   )
 # pre-populate DUNE_PYTHON_VIRTUALENV_PATH
@@ -91,31 +83,14 @@
   "Location of Python virtualenv created by the Dune build system"
   )
 # pre-populate DUNE_PYTHON_EXTERNAL_VIRTUALENV_FOR_ABSOLUTE_BUILDDIR
 set(DUNE_PYTHON_EXTERNAL_VIRTUALENV_FOR_ABSOLUTE_BUILDDIR ON CACHE BOOL
   "Place Python virtualenv in top-level directory \"dune-python-env\" when using an absolute build directory"
   )
 
-option(DUNE_RUNNING_IN_CI "This is turned on if running in dune gitlab ci" OFF)
-
-if(DUNE_RUNNING_IN_CI)
-  set(DUNE_PIP_INDEX "--index-url=https://gitlab.dune-project.org/api/v4/projects/133/packages/pypi/simple")
-else()
-  set(DUNE_PIP_INDEX "")
-endif()
-
-# Construct the wheel house installation option string
-# First set the path to a Dune wheelhouse that is to be used during installation
-# NB: Right now, the same logic is used to retrieve the location of the
-#     wheelhouse (which means that you have to use the same CMAKE_INSTALL_PREFIX
-#     when *using* installed modules, you used when *installing* them.
-#     TODO: Replace this with a better mechanism (like writing the location into
-#           dune-commons package config file)
-set(DUNE_PYTHON_WHEELHOUSE "${CMAKE_INSTALL_PREFIX}/share/dune/wheelhouse" CACHE PATH "The place where the wheels will be stored")
-
 # Determine whether the given interpreter is running inside a virtualenv
 dune_execute_process(COMMAND "${Python3_EXECUTABLE}" "${scriptdir}/venvpath.py"
                      RESULT_VARIABLE DUNE_PYTHON_SYSTEM_IS_VIRTUALENV
                      OUTPUT_VARIABLE DUNE_PYTHON_VIRTUALENV_PATH
                      OUTPUT_STRIP_TRAILING_WHITESPACE
                      )
 
@@ -278,14 +253,7 @@
     set(DUNE_ENABLE_PYTHONBINDINGS OFF)
     return()
   endif()
 endif()
 
 # if pip was not found before then we can set it here since it was now found
 set(DUNE_PYTHON_pip_FOUND ON)
-
-# install setuptools into the venv (needed to find dependencies later on)
-dune_execute_process(COMMAND ${DUNE_PYTHON_VIRTUALENV_EXECUTABLE} -m pip install
-      "${DUNE_PIP_INDEX}"
-      setuptools>=41 ninja
-  WARNING_MESSAGE "python 'setuptools' package could not be installed - possibly connection to the python package index failed"
-  )
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneReplaceProperties.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneReplaceProperties.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneReplaceProperties
 ---------------------
 
 Utility functions to modify target properties
 
 .. cmake:command:: replace_properties
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneSphinxCMakeDoc.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneSphinxCMakeDoc.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module to generate CMake API documentation with Sphinx
 #
 # .. cmake_function:: dune_cmake_sphinx_doc
 #
 #    .. cmake_brief::
 #
 #       Generate the documentation that you are just browsing!!!
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneSphinxDoc.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneSphinxDoc.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 include_guard(GLOBAL)
 find_package(Sphinx)
 find_package(Python3 COMPONENTS Interpreter Development)
 
 function(dune_sphinx_doc)
   # Only proceed if Sphinx was found on the system
   if(NOT SPHINX_FOUND)
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneStreams.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneStreams.cmake`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This Module configures the DUNE debug streams.
 #
 # .. cmake_variable:: MINIMAL_DEBUG_LEVEL
 #
 #    This variable configures the Dune debug streams.
 #    Standard debug streams with level below :code:`MINIMAL_DEBUG_LEVEL` will
 #    collapse to doing nothing if output is requested. Possible values are
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneSymlinkOrCopy.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneSymlinkOrCopy.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This module provides convenience macros to provide files from the source tree in the build tree.
 #
 # It provides the following macros:
 #
 #   dune_add_copy_command(filename)
 #
 # This macro adds a file-copy command.
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneTestMacros.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneTestMacros.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module that provides tools for testing the Dune way.
 #
 # Note that "the Dune way" of doing this has changed after
 # the 2.4 release. See the build system documentation for details.
 #
 # .. cmake_function:: dune_declare_test_label
 #
@@ -156,20 +153,14 @@
 #    .. cmake_param:: TIMEOUT
 #       :single:
 #
 #       If set, the test will time out after the given number of seconds. This supersedes
 #       any timeout setting in ctest (see `cmake --help-property TIMEOUT`). If you
 #       specify the MPI_RANKS option, you need to specify a TIMEOUT.
 #
-#    .. cmake_param:: WORKING_DIRECTORY
-#       :single:
-#
-#       Set the WORKING_DIRECTORY test property to specify the working directory in which to execute the test.
-#       If not specified the test will be run with the current working directory set to the build directory corresponding to the current source directory.
-#
 #    .. cmake_param:: LABELS
 #       :multi:
 #
 #       A list of labels to add to the test.  This has two effects: it sets
 #       the LABELS property on the test so :code:`ctest -L ${label_regex}` can
 #       be used to run all tests with certain labels.  It also adds any
 #       targets created as dependencies to a custom target, so you can build
@@ -177,15 +168,15 @@
 #       build_${label}_tests` without having to build all the other tests as
 #       well.
 #
 #       The :code:`build_${label}_tests` targets are created on-demand the
 #       first time a test with that label is added.  In some situations it can
 #       depend on the values of cmake cache variables whether a test is added,
 #       and then it can happen that the :code:`build_${target}_tests` target
-#       exists only sometimes.  If your workflow relies on the existence of
+#       exists only sometimes.  If your workflow relies on the existance of
 #       these targets, even if building them just returns successfully without
 #       doing anything, you can ensure they exist by calling
 #       :ref:`dune_declare_test_label` unconditionally.  The label
 #       :code:`quick` is always predeclared in this way.
 #
 #       The label names must be non-empty, and must only contain alphanumeric
 #       characters other than :code:`-` or :code:`_`.  This restriction is in
@@ -211,18 +202,14 @@
 # .. cmake_variable:: DUNE_BUILD_TESTS_ON_MAKE_ALL
 #
 #    You may set this variable through your opts file or on a per module level (in the toplevel
 #    :code:`CMakeLists.txt` before :code:`include(DuneMacros)`) to have the Dune build system
 #    build all tests during `make all`. Note, that this may take quite some time for some modules.
 #    If not in use, you have to build tests through the target :code:`build_tests`.
 #
-# .. cmake_variable:: PYTHON_TEST
-#
-#    This flag specifies a python test and is set by the dune_python_add_test command. It disables the check on the existence of the target file.
-#
 include_guard(GLOBAL)
 
 # enable the testing suite on the CMake side.
 enable_testing()
 include(CTest)
 
 # Introduce a target that triggers the building of all tests
@@ -258,16 +245,16 @@
 
 # Set the default on the variable DUNE_MAX_TEST_CORES
 if(NOT DUNE_MAX_TEST_CORES)
   set(DUNE_MAX_TEST_CORES 2)
 endif()
 
 function(dune_add_test)
-  set(OPTIONS EXPECT_COMPILE_FAIL EXPECT_FAIL SKIP_ON_77 COMPILE_ONLY PYTHON_TEST)
-  set(SINGLEARGS NAME TARGET TIMEOUT WORKING_DIRECTORY)
+  set(OPTIONS EXPECT_COMPILE_FAIL EXPECT_FAIL SKIP_ON_77 COMPILE_ONLY)
+  set(SINGLEARGS NAME TARGET TIMEOUT)
   set(MULTIARGS SOURCES COMPILE_DEFINITIONS COMPILE_FLAGS LINK_LIBRARIES CMD_ARGS MPI_RANKS COMMAND CMAKE_GUARD LABELS)
   cmake_parse_arguments(ADDTEST "${OPTIONS}" "${SINGLEARGS}" "${MULTIARGS}" ${ARGN})
 
   # Check whether the parser produced any errors
   if(ADDTEST_UNPARSED_ARGUMENTS)
     message(WARNING "Unrecognized arguments ('${ADDTEST_UNPARSED_ARGUMENTS}') for dune_add_test!")
   endif()
@@ -307,20 +294,17 @@
   endif()
   if(NOT ADDTEST_MPI_RANKS)
     set(ADDTEST_MPI_RANKS 1)
   endif()
   if(NOT ADDTEST_TIMEOUT)
     set(ADDTEST_TIMEOUT 300)
   endif()
-  if(NOT ADDTEST_WORKING_DIRECTORY)
-    set(ADDTEST_WORKING_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
-  endif()
   foreach(num ${ADDTEST_MPI_RANKS})
     if(NOT "${num}" MATCHES "[1-9][0-9]*")
-      message(FATAL_ERROR "${num} was given to the MPI_RANKS argument of dune_add_test, but it does not seem like a correct processor number")
+      message(FATAL_ERROR "${num} was given to the MPI_RANKS arugment of dune_add_test, but it does not seem like a correct processor number")
     endif()
   endforeach()
   if(ADDTEST_SKIP_ON_77)
     message(WARNING "The SKIP_ON_77 option for dune_add_test is obsolete, it is now enabled by default.")
   endif()
 
   # Discard all parallel tests if MPI was not found
@@ -409,19 +393,18 @@
         set(ACTUAL_TESTCOMMAND "$<TARGET_FILE:${ADDTEST_TARGET}>")
         set(ACTUAL_CMD_ARGS)
       endif()
 
       # Now add the actual test
       _add_test(NAME ${ACTUAL_NAME}
                 COMMAND "${ACTUAL_TESTCOMMAND}" ${ACTUAL_CMD_ARGS}
-                WORKING_DIRECTORY "${ADDTEST_WORKING_DIRECTORY}"
                )
 
       # Make the test depend on the existence of the target to trigger "Not Run" response
-      if(NOT ADDTEST_EXPECT_COMPILE_FAIL AND NOT ADDTEST_PYTHON_TEST)
+      if(NOT ADDTEST_EXPECT_COMPILE_FAIL)
         set_tests_properties(${ACTUAL_NAME} PROPERTIES REQUIRED_FILES $<TARGET_FILE:${ADDTEST_TARGET}>)
       endif()
       # Define the number of processors (ctest will coordinate this with the -j option)
       set_tests_properties(${ACTUAL_NAME} PROPERTIES PROCESSORS ${procnum})
       # Apply the timeout (which was defaulted to 5 minutes if not specified)
       set_tests_properties(${ACTUAL_NAME} PROPERTIES TIMEOUT ${ADDTEST_TIMEOUT})
       # Process the EXPECT_FAIL option
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/DuneUtilities.cmake` & `dune-common-2.9.dev20220529/cmake/modules/DuneUtilities.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 DuneUtilities
 -------------
 
 Utility functions used by multiple files.
 
 .. cmake:command:: dune_module_to_uppercase
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindGMP.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindGMP.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindGMP
 -------
 
 Find the GNU MULTI-Precision Bignum (GMP) library
 and the corresponding C++ bindings GMPxx.
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindInkscape.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindInkscape.cmake`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Module that checks for inkscape
 #
 #    Sets the following variables
 #
 #    :code:`INKSCAPE_FOUND`
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindLatexMk.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindLatexMk.cmake`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindMETIS.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindMETIS.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindMETIS
 ---------
 
 Find Serial Graph Partitioning library
 `METIS <http://glaros.dtc.umn.edu/gkhome/metis/metis/overview>`_
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindPTScotch.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindPTScotch.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindPTScotch
 ------------
 
 Find library `PTScotch <https://gitlab.inria.fr/scotch/scotch>`_, i.e. Software
 package and libraries for sequential and parallel graph partitioning, static
 mapping and clustering, sequential mesh and hypergraph partitioning, and
@@ -49,15 +46,15 @@
 Cache Variables
 ^^^^^^^^^^^^^^^
 
 The following variables may be set to influence this module's behavior:
 
 ``PTSCOTCH_SUFFIX``
   Scotch might be compiled using different integer sizes (int32, int64, long).
-  When this is set the headers and libraries are search under the suffix
+  When this is set the headers and libaries are search under the suffix
   :code:`include/scotch-${PTSCOTCH_SUFFIX}`, and :code:`lib/scotch-${PTSCOTCH_SUFFIX}`,
   respectively.
 
 ``SCOTCH_INCLUDE_DIR``
   Include directory where the scotch.h is found.
 
 ``PTSCOTCH_INCLUDE_DIR``
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindParMETIS.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindParMETIS.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindParMETIS
 ------------
 
 Find Parallel Graph Partitioning library
 `ParMETIS <http://glaros.dtc.umn.edu/gkhome/metis/parmetis/overview>`_
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindPkgConfig/FindPkgConfig.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindPkgConfig/FindPkgConfig.cmake`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindPython3/FindPython3.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindPython3/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindPython3/Support.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindPython3/Support.cmake`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindQuadMath.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindQuadMath.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindQuadMath
 ------------
 
 Find the GCC Quad-Precision library
 
 This module checks if the used compiler has built-in support for QuadMath
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindSphinx.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindSphinx.cmake`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Find Sphinx - the python documentation tool
 #
 #    You may set the following variables to modify the
 #    behaviour of this module:
 #
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindSuiteSparse.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindSuiteSparse.cmake`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindSuiteSparse
 ---------------
 
 Find the SuiteSparse libraries like UMFPACK or SPQR.
 
 Use this module by invoking find_package with the form:
@@ -176,15 +173,15 @@
   if (SUITESPARSE_PREFIX_VERSION GREATER_EQUAL 0)
     set(SuiteSparse_VERSION "${SuiteSparse_VERSION}.${SUITESPARSE_PREFIX_VERSION}")
   endif()
 endif()
 unset(SUITESPARSE_CONFIG_FILE CACHE)
 
 
-# check whether everything was found
+# check wether everything was found
 foreach(_component ${SUITESPARSE_COMPONENTS})
   if(${_component}_LIBRARY AND ${_component}_INCLUDE_DIR)
     set(SuiteSparse_${_component}_FOUND TRUE)
   else()
     set(SuiteSparse_${_component}_FOUND FALSE)
   endif()
 endforeach(_component)
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/FindTBB.cmake` & `dune-common-2.9.dev20220529/cmake/modules/FindTBB.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindTBB
 -------
 
 Finds the Threading Building Blocks (TBB) library.
 
 This is a fallback implementation in case the TBB library does not provide
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/Headercheck.cmake` & `dune-common-2.9.dev20220529/cmake/modules/Headercheck.cmake`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_variable:: ENABLE_HEADERCHECK
 #
 #    Set this variable to TRUE if you want to use the CMake
 #    reimplementation of the old autotools feaure :code:`make headercheck`.
 #    There has been a couple of issues with this implementation in
 #    the past, so it was deactivated by default.
 #
@@ -79,15 +76,15 @@
       string(REGEX REPLACE "/" "_" targname ${rel})
 
       #generate the headercheck .cc file
       file(WRITE ${CMAKE_BINARY_DIR}/headercheck/${rel}.cc "#ifdef HAVE_CONFIG_H\n#include<config.h>\n#endif\n#include<${simple}>\n#include<${simple}>\nint main(){return 0;}")
 
       # add target for the check of current header, this is implemented as a library
       # to prevent CMake from automatically trying to link the target, functionality
-      # of macro try_compile() is unfortunately not available due to it not being scriptable.
+      # of macro try_compile() is unfortunately not availbale due to it not being scriptable.
       add_library(headercheck_${targname} STATIC EXCLUDE_FROM_ALL
         ${CMAKE_BINARY_DIR}/headercheck/${rel}.cc)
       add_dependencies(headercheck headercheck_${targname})
 
       #add PKG_ALL_FLAGS and the directory where the header is located
       set_property(TARGET headercheck_${targname}
         APPEND_STRING PROPERTY COMPILE_FLAGS "-DHEADERCHECK -I${PROJECT_SOURCE_DIR}${relpath} -I${CMAKE_BINARY_DIR}")
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/OverloadCompilerFlags.cmake` & `dune-common-2.9.dev20220529/cmake/modules/OverloadCompilerFlags.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # check whether the user wants to overload compile flags upon calling make
 #
 # Provides the following macros:
 #
 #   initialize_compiler_script() : needs to be called before further flags are added to CMAKE_CXX_FLAGS
 #   finalize_compiler_script()   : needs to be called at the end of the cmake macros, e.g. in finalize_dune_project
 #
@@ -25,21 +22,14 @@
 #    .. note::
 #       If you don't know what this is or what it's good for, don't use it.
 #
 include_guard(GLOBAL)
 
 option(ALLOW_CXXFLAGS_OVERWRITE OFF)
 option(ALLOW_CFLAGS_OVERWRITE OFF)
-option(ALLOW_CXXFLAGS_OVERWRITE_FORCE OFF)
-
-set(WRITE_CXXFLAGS_COMPILER_SCRIPT FALSE)
-# write scripts if CMAKE_GENERATOR is Makefiles or if FORCE is on
-if(${CMAKE_GENERATOR} MATCHES ".*Unix Makefiles.*" OR ALLOW_CXXFLAGS_OVERWRITE_FORCE)
-  set(WRITE_CXXFLAGS_COMPILER_SCRIPT TRUE)
-endif()
 
 set(CXX_COMPILER_SCRIPT "${CMAKE_BINARY_DIR}/CXX_compiler.sh" )
 set(C_COMPILER_SCRIPT "${CMAKE_BINARY_DIR}/C_compiler.sh" )
 
 macro(find_extended_unix_commands)
   include(FindUnixCommands)
   set(FLAGSNAMES "ALLOW_CXXFLAGS_OVERWRITE and/or ALLOW_CFLAGS_OVERWRITE")
@@ -73,27 +63,27 @@
   mark_as_advanced(ENV_PROGRAM)
   mark_as_advanced(ECHO_PROGRAM)
   mark_as_advanced(CHMOD_PROGRAM)
 endmacro(find_extended_unix_commands)
 
 # init compiler script and store CXX flags
 macro(initialize_compiler_script)
-  if(ALLOW_CXXFLAGS_OVERWRITE AND WRITE_CXXFLAGS_COMPILER_SCRIPT)
+  if(ALLOW_CXXFLAGS_OVERWRITE AND (${CMAKE_GENERATOR} MATCHES ".*Unix Makefiles.*"))
     # check for unix commands necessary
     find_extended_unix_commands()
     # set CXXFLAGS as environment variable
     set( DEFAULT_CXXFLAGS ${CMAKE_CXX_FLAGS} CACHE STRING "default CXX flags")
     set( CMAKE_CXX_FLAGS "" )
     set( DEFAULT_CXX_COMPILER ${CMAKE_CXX_COMPILER} )
     set( CXX_COMPILER_SCRIPT_FILE "#!${BASH}\nexec ${CMAKE_CXX_COMPILER} \"\$@\"")
     file(WRITE ${CXX_COMPILER_SCRIPT} "${CXX_COMPILER_SCRIPT_FILE}")
     execute_process(COMMAND ${CHMOD_PROGRAM} 755 ${CXX_COMPILER_SCRIPT})
     set(CMAKE_CXX_COMPILER ${CXX_COMPILER_SCRIPT})
   endif()
-  if(ALLOW_CFLAGS_OVERWRITE AND WRITE_CXXFLAGS_COMPILER_SCRIPT)
+  if(ALLOW_CFLAGS_OVERWRITE AND (${CMAKE_GENERATOR} MATCHES ".*Unix Makefiles.*"))
     # check for unix commands necessary
     find_extended_unix_commands()
     # set CFLAGS as environment variable
     set( DEFAULT_CFLAGS ${CMAKE_C_FLAGS} CACHE STRING "default C flags")
     set( CMAKE_C_FLAGS "" )
     set( DEFAULT_C_COMPILER ${CMAKE_C_COMPILER} )
     set( C_COMPILER_SCRIPT_FILE "#!${BASH}\nexec ${CMAKE_C_COMPILER} \"\$@\"")
@@ -101,15 +91,15 @@
     execute_process(COMMAND ${CHMOD_PROGRAM} 755 ${C_COMPILER_SCRIPT})
     set(CMAKE_C_COMPILER ${C_COMPILER_SCRIPT})
   endif()
 endmacro()
 
 # finalize compiler script and write it
 macro(finalize_compiler_script)
-  if( WRITE_CXXFLAGS_COMPILER_SCRIPT )
+  if(${CMAKE_GENERATOR} MATCHES ".*Unix Makefiles.*")
     # check CXX compiler
     if((ALLOW_CXXFLAGS_OVERWRITE))
       set(COMPILERS "CXX")
     endif()
     # check C compiler
     if((ALLOW_CFLAGS_OVERWRITE))
       set(COMPILERS ${COMPILERS} "C")
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/UseInkscape.cmake` & `dune-common-2.9.dev20220529/cmake/modules/UseInkscape.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module that provides conversion routines using inkscape
 #
 # .. cmake_function:: inkscape_generate_png_from_svg
 #
 #    .. cmake_param:: OUTPUT_DIR
 #       :single:
 #
```

### Comparing `dune-common-2.9.0rc1/cmake/modules/UseLatexMk.cmake` & `dune-common-2.9.dev20220529/cmake/modules/UseLatexMk.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 # documents from incorrectly messing with a user’s files. If for $out_dir or $aux_dir you really do
 # need to specify an absolute pathname (e.g., "/tmp/foo") or a path (e.g., "../output") that includes a
 # higher-level directory, and you need to use makeindex or bibtex, then you need to disable the secu-
 # rity measures (and assume any risks). One way of doing this is to temporarily set an operating
 # system environment variable openout_any to "a" (as in "all"), to override the default "paranoid"
 # setting.
 #
-# UseLatexMk.cmake allows to re-enable the TeX security measure by setting LATEXMK_PARANOID to TRUE
+# UseLatexMk.cmake allows to reenable the TeX security measure by setting LATEXMK_PARANOID to TRUE
 # through cmake -D, but it is not guaranteed to work correctly in that case.
 #
-# For further information, visit https://github.com/dokempf/UseLatexMk
+# For further informations, visit https://github.com/dokempf/UseLatexMk
 #
 #
 # Copyright (c) 2017, Dominic Kempf, Steffen Müthing
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `dune-common-2.9.0rc1/cmake/scripts/CreateDoxyFile.cmake` & `dune-common-2.9.dev20220529/cmake/scripts/CreateDoxyFile.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # For now we just support appending Doxyfile and Doxylocal
 file(READ ${DOXYSTYLE} file_contents)
 file(WRITE Doxyfile.in ${file_contents})
 # Write the list of predefined C preprocessor macros
 file(READ ${DOXYGENMACROS} file_contents)
 file(APPEND Doxyfile.in ${file_contents})
 if(DOXYLOCAL)
```

### Comparing `dune-common-2.9.0rc1/cmake/scripts/extract_cmake_data.py` & `dune-common-2.9.dev20220529/cmake/scripts/extract_cmake_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/env python
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 """ This script will parse a cmake module and extract some
     rst documentation from it. This might not be as elegant as
     writing a Sphinx domain or using a custom extension with
     cmake related directives, but it provides a straightforward
     working way.
```

### Comparing `dune-common-2.9.0rc1/cmake/scripts/pyversion.py` & `dune-common-2.9.dev20220529/cmake/scripts/pyversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#
 # This python script tries to figure out the version of a given python
 # package. This is only intended to be used from DunePythonFindPackage.cmake
 #
 # There is no unified way of specifying the version of a python package. This
 # script implements some methods. For discussion on the implemented methods see
 # http://stackoverflow.com/questions/20180543
 #
```

### Comparing `dune-common-2.9.0rc1/cmake/scripts/sphinx_cmake_dune.py` & `dune-common-2.9.dev20220529/cmake/scripts/sphinx_cmake_dune.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 """ A cmake extension for Sphinx
 
 tailored for the Dune project.
 This is used during `make doc` to build the
 build system documentation.
 """
```

### Comparing `dune-common-2.9.0rc1/cmake/scripts/venvpath.py` & `dune-common-2.9.dev20220529/cmake/scripts/venvpath.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#
 # A python script that determines whether the current interpreter is
 # running inside a virtual environment. For discussion of the implemented
 # methods, see http://stackoverflow.com/questions/1871549
 #
 # Meant to be run from DunePythonCommonMacros.cmake. For that reason, it
 # exits with either 1 or 0, where 1 indicates that the interpreter
 # runs inside a virtualenv. It also prints the path to the venv (if active) to stdout
```

### Comparing `dune-common-2.9.0rc1/config.h.cmake` & `dune-common-2.9.dev20220529/config.h.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* begin dune-common
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 
 /* begin private */
```

### Comparing `dune-common-2.9.0rc1/doc/buildsystem/dune-common.rst` & `dune-common-2.9.dev20220529/doc/buildsystem/dune-common.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-::
-  SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-  SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 ===========
 dune-common
 ===========
 
 .. _whatis:
 
 What is CMake anyway?
```

### Comparing `dune-common-2.9.0rc1/doc/buildsystem/examples/Toolchain-Ubuntu-mingw32.cmake` & `dune-common-2.9.dev20220529/doc/buildsystem/examples/Toolchain-Ubuntu-mingw32.cmake`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Sample toolchain file for building for Windows from an Ubuntu Linux system.
 #
 # Typical usage:
 #    *) install cross compiler: `sudo apt-get install mingw-w64 g++-mingw-w64`
 #    *) cd build
 #    *) cmake -DCMAKE_TOOLCHAIN_FILE=~/Toolchain-Ubuntu-mingw32.cmake ..
```

### Comparing `dune-common-2.9.0rc1/doc/comm/communication.bib` & `dune-common-2.9.dev20220529/doc/comm/communication.bib`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-@Comment SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-@Comment SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 @InProceedings{ISTL,
   author = {Markus Blatt and Peter Bastian},
   title = 	 {The Iterative Solver Template Library},
   booktitle = {Applied Parallel Computing. State of the Art in Scientific Computing},
   editor = 	 {Bo K\r{a}gstr\"om and Erik Elmroth and Jack Dongarra and Jerzy Wa\'sniewski},
   year = 	 2007,
   volume = 	 4699,
```

### Comparing `dune-common-2.9.0rc1/doc/comm/communication.tex` & `dune-common-2.9.dev20220529/doc/comm/communication.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 \documentclass[11pt]{article}
 \usepackage{multicol}
 \usepackage{ifthen}
 \usepackage{amsthm}
 \usepackage{amsmath}
 \usepackage{amsfonts}
 \usepackage{color}
```

### Comparing `dune-common-2.9.0rc1/doc/comm/figures/darray.eps` & `dune-common-2.9.dev20220529/doc/comm/figures/darray.eps`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/doc/comm/figures/distindex.eps` & `dune-common-2.9.dev20220529/doc/comm/figures/distindex.eps`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/doc/comm/indexset.cc` & `dune-common-2.9.dev20220529/doc/comm/indexset.cc`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/plocalindex.hh>
 #include <dune/common/parallel/mpihelper.hh>
 #include <iostream>
 #include "buildindexset.hh"
 #include "reverse.hh"
 
 int main(int argc, char **argv)
 {
-  // This is a parallel program so we need to
+  // This is a parallel programm so we need to
   // initialize mpi first.
   Dune::MPIHelper& helper = Dune::MPIHelper::instance(argc, argv);
 
   // The rank of our process
   int rank = helper.rank();
 
   // The type used as the global index
@@ -37,15 +35,15 @@
   std::cout<<indexSet<<std::endl;
 
 
   reverseLocalIndex(indexSet);
 
   // Print the index set
   if(rank==0)
-    std::cout<<"Reordered local indices:"<<std::endl;
+    std::cout<<"Reordered lcoal indices:"<<std::endl;
 
   // Wait for all processes
   helper.getCommunication().barrier();
 
   std::cout<<indexSet<<std::endl;
   // Assign new local indices
```

### Comparing `dune-common-2.9.0rc1/doc/comm/poosc08.cc` & `dune-common-2.9.dev20220529/doc/comm/poosc08.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 # include "config.h"
 #endif
 #include <iostream>
 #include <dune/common/exceptions.hh> // We use exceptions
 #include <dune/common/parallel/mpihelper.hh> // An initializer of MPI
 #include <dune/common/parallel/indexset.hh>
```

### Comparing `dune-common-2.9.0rc1/doc/comm/poosc08_test.cc` & `dune-common-2.9.dev20220529/doc/comm/poosc08_test.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 # include "config.h"
 #endif
 #include <iostream>
 #include <dune/common/exceptions.hh> // We use exceptions
 #include <dune/common/parallel/mpihelper.hh> // An initializer of MPI
 #include <dune/common/parallel/indexset.hh>
```

### Comparing `dune-common-2.9.0rc1/doc/doxygen/Doxystyle` & `dune-common-2.9.dev20220529/doc/doxygen/Doxystyle`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #----------- Doxystyle -----------
 
 ##################################################################################
 # Project Details:
 
 PROJECT_NAME           = @DUNE_MOD_NAME@
 PROJECT_NUMBER         = @DUNE_MOD_VERSION@
```

### Comparing `dune-common-2.9.0rc1/doc/doxygen/modules.txt` & `dune-common-2.9.dev20220529/doc/doxygen/modules.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 /**
   @defgroup Common Common
   @brief foundation classes
 */
 
 /**
   @defgroup Allocators Allocators
```

### Comparing `dune-common-2.9.0rc1/doc/dunecontrol.1` & `dune-common-2.9.dev20220529/doc/dunecontrol.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.\" SPDX-FileCopyrightInfo: Copyright (C) 2013-2015 Oliver Sander
-.\" SPDX-License-Identifier: FSFAP
-.\"
 .\" First parameter, NAME, should be all caps
 .\" Second parameter, SECTION, should be 1-8, maybe w/ subsection
 .\" other parameters are allowed: see man(7), man(1)
 .TH DUNECONTROL 1 "November 8, 2016"
 .\" Please adjust this date whenever revising the manpage.
 .\"
 .\" Some roff macros, for reference:
```

### Comparing `dune-common-2.9.0rc1/dune/common/CMakeLists.txt` & `dune-common-2.9.dev20220529/dune/common/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory("parallel")
 add_subdirectory("simd")
 add_subdirectory("std")
 add_subdirectory("test")
 
 # add some sources to the dunecommon library
 target_sources(dunecommon PRIVATE
@@ -65,15 +62,14 @@
         ios_state.hh
         iteratorfacades.hh
         iteratorrange.hh
         keywords.hh
         lru.hh
         mallocallocator.hh
         math.hh
-        matrixconcepts.hh
         matvectraits.hh
         overloadset.hh
         parameterizedobject.hh
         parametertree.hh
         parametertreeparser.hh
         path.hh
         poolallocator.hh
```

### Comparing `dune-common-2.9.0rc1/dune/common/alignedallocator.hh` & `dune-common-2.9.dev20220529/dune/common/alignedallocator.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ALIGNED_ALLOCATOR_HH
 #define DUNE_ALIGNED_ALLOCATOR_HH
 
 #include "mallocallocator.hh"
 #include <cstdlib>
```

### Comparing `dune-common-2.9.0rc1/dune/common/arraylist.hh` & `dune-common-2.9.dev20220529/dune/common/arraylist.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_ARRAYLIST_HH
 #define DUNE_COMMON_ARRAYLIST_HH
 
 #include <array>
 #include <cassert>
 #include <memory>
```

### Comparing `dune-common-2.9.0rc1/dune/common/assertandreturn.hh` & `dune-common-2.9.dev20220529/dune/common/assertandreturn.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_ASSERTANDRETURN_HH
 #define DUNE_COMMON_ASSERTANDRETURN_HH
 
 #include <cassert>
 
 //! Asserts a condition and return on success in constexpr context.
 /**
```

### Comparing `dune-common-2.9.0rc1/dune/common/bartonnackmanifcheck.hh` & `dune-common-2.9.dev20220529/dune/common/bartonnackmanifcheck.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /** @file
    @author Robert Kloefkorn
    @brief Provides check for implementation of interface methods when using
    static polymorphism, i.e. the Barton-Nackman trick. This is purely for
    debugging purposes. To check the correct implementation of interface methods
    (and pick up possible infinite loops) NDEBUG must be undefined and
    DUNE_INTERFACECHECK has to be defined.
@@ -49,15 +47,15 @@
       call = false; \
       throw; \
     } \
   }
 #endif
 
 /** The macro CHECK_AND_CALL_INTERFACE_IMPLEMENTATION throws an exception,
-   if the interface method is not implemented and just calls the method
+   if the interface method ist not implemented and just calls the method
    otherwise. If NDEBUG is defined no
    checking is done and the method is just called.
  */
 #if defined NDEBUG || !defined DUNE_INTERFACECHECK
 #define CHECK_AND_CALL_INTERFACE_IMPLEMENTATION(__interface_method_to_call__) \
   (__interface_method_to_call__)
 #else
```

### Comparing `dune-common-2.9.0rc1/dune/common/bigunsignedint.hh` & `dune-common-2.9.dev20220529/dune/common/bigunsignedint.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_BIGUNSIGNEDINT_HH
 #define DUNE_BIGUNSIGNEDINT_HH
 
 #include <algorithm>
 #include <iostream>
 #include <limits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/binaryfunctions.hh` & `dune-common-2.9.dev20220529/dune/common/binaryfunctions.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_BINARYFUNCTIONS_HH
 #define DUNE_BINARYFUNCTIONS_HH
 
 /** \file
  * \brief helper classes to provide unique types for standard functions
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/bitsetvector.hh` & `dune-common-2.9.dev20220529/dune/common/bitsetvector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_BLOCK_BITFIELD_HH
 #define DUNE_BLOCK_BITFIELD_HH
 
 /** \file
     \brief Efficient implementation of a dynamic array of static arrays of booleans
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/boundschecking.hh` & `dune-common-2.9.dev20220529/dune/common/boundschecking.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_BOUNDSCHECKING_HH
 #define DUNE_BOUNDSCHECKING_HH
 
 #include <dune/common/exceptions.hh>
 
 /**
  * \file
```

### Comparing `dune-common-2.9.0rc1/dune/common/classname.hh` & `dune-common-2.9.dev20220529/dune/common/classname.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_CLASSNAME_HH
 #define DUNE_CLASSNAME_HH
 
 /** \file
  * \brief A free function to provide the demangled class name
  *        of a given object or type as a string
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/concept.hh` & `dune-common-2.9.dev20220529/dune/common/concept.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_CONCEPT_HH
 #define DUNE_COMMON_CONCEPT_HH
 
 #include <type_traits>
 #include <utility>
 #include <tuple>
```

### Comparing `dune-common-2.9.0rc1/dune/common/conditional.hh` & `dune-common-2.9.dev20220529/dune/common/conditional.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_CONDITIONAL_HH
 #define DUNE_COMMON_CONDITIONAL_HH
 
 namespace Dune
 {
 
     /** \brief conditional evaluate
```

### Comparing `dune-common-2.9.0rc1/dune/common/debugalign.cc` & `dune-common-2.9.dev20220529/dune/common/debugalign.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <cstddef>
 #include <cstdlib>
 #include <functional>
 #include <ios>
```

### Comparing `dune-common-2.9.0rc1/dune/common/debugalign.hh` & `dune-common-2.9.dev20220529/dune/common/debugalign.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DEBUGALIGN_HH
 #define DUNE_DEBUGALIGN_HH
 
 #include <algorithm>
 #include <cassert>
 #include <cmath>
 #include <complex>
@@ -181,27 +179,20 @@
        * silence warnings from GCC about using `~` on a bool
        * (when instantiated for T=bool)
        */
 #if __GNUC__ >= 7
 #  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wbool-operation"
 #endif
-#ifdef __clang__
-#  pragma clang diagnostic push
-#  pragma clang diagnostic ignored "-Wbool-operation"
-#endif
       template<class U = T,
                class = std::void_t<decltype(~std::declval<const U&>())> >
       decltype(auto) operator~() const { return aligned<align>(~value_); }
 #if __GNUC__ >= 7
 #  pragma GCC diagnostic pop
 #endif
-#ifdef __clang__
-#  pragma clang diagnostic pop
-#endif
 
       template<class U = T,
                class = std::void_t<decltype(!std::declval<const U&>())> >
       decltype(auto) operator!() const { return aligned<align>(!value_); }
 
       // assignment operators
 #define DUNE_ASSIGN_OP(OP)                                              \
```

### Comparing `dune-common-2.9.0rc1/dune/common/debugallocator.cc` & `dune-common-2.9.dev20220529/dune/common/debugallocator.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include "debugallocator.hh"
 
 #if HAVE_MPROTECT
```

### Comparing `dune-common-2.9.0rc1/dune/common/debugallocator.hh` & `dune-common-2.9.dev20220529/dune/common/debugallocator.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DEBUG_ALLOCATOR_HH
 #define DUNE_DEBUG_ALLOCATOR_HH
 
 #if __has_include(<sys/mman.h>)
 
 #include <sys/mman.h>
 #define HAVE_SYS_MMAN_H 1
@@ -222,15 +220,15 @@
      - list allocated memory chunks still in use upon destruction of the allocator
 
      When defining DEBUG_ALLOCATOR_KEEP to 1, we also check
      - double free
      - access after free
 
      When defining DEBUG_NEW_DELETE >= 1, we
-     - overload new/delete
+     - overload new/delte
      - use the Debug memory management for new/delete
      - DEBUG_NEW_DELETE > 2 gives extensive debug output
    */
   template <class T>
   class DebugAllocator {
   public:
     typedef std::size_t size_type;
```

### Comparing `dune-common-2.9.0rc1/dune/common/debugstream.hh` & `dune-common-2.9.dev20220529/dune/common/debugstream.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_DEBUGSTREAM_HH
 #define DUNE_DEBUGSTREAM_HH
 
 /** \file
  * \brief Defines several output streams for messages of different importance
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/densematrix.hh` & `dune-common-2.9.dev20220529/dune/common/densematrix.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DENSEMATRIX_HH
 #define DUNE_DENSEMATRIX_HH
 
 #include <cmath>
 #include <cstddef>
 #include <iostream>
 #include <type_traits>
@@ -793,15 +791,15 @@
      * <ul>
      * <li>Terminate as soon as one lane is discovered to be singular.  Early
      *     termination is done by throwing an \c FMatrixError.  On entry, \c
      *     Simd::allTrue(nonsingularLanes) and \c throwEarly==true should hold.
      *     After early termination, the contents of \c A should be considered
      *     bogus, and \c nonsingularLanes has the lane(s) that triggered the
      *     early termination unset.  There may be more singular lanes than the
-     *     one reported in \c nonsingularLanes, which just haven't been
+     *     one reported in \c nonsingularLanes, which just havent been
      *     discovered yet; so the value of \c nonsingularLanes is mostly
      *     useful for diagnostics.</li>
      * <li>Terminate only when all lanes are discovered to be singular.  Use
      *     this when you want to apply special postprocessing in singular
      *     lines (e.g. setting the determinant of singular lanes to 0 in \c
      *     determinant()).  On entry, \c nonsingularLanes may have any value
      *     and \c throwEarly==false should hold.  The function will not throw
```

### Comparing `dune-common-2.9.0rc1/dune/common/densevector.hh` & `dune-common-2.9.dev20220529/dune/common/densevector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DENSEVECTOR_HH
 #define DUNE_DENSEVECTOR_HH
 
 #include <algorithm>
 #include <limits>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/deprecated.hh` & `dune-common-2.9.dev20220529/dune/common/deprecated.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DEPRECATED_HH
 #define DUNE_DEPRECATED_HH
 
 /** \file
  * \brief Definition of the `DUNE_NO_DEPRECATED_*` macros
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/diagonalmatrix.hh` & `dune-common-2.9.dev20220529/dune/common/diagonalmatrix.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DIAGONAL_MATRIX_HH
 #define DUNE_DIAGONAL_MATRIX_HH
 
 /*! \file
    \brief  This file implements a quadratic diagonal matrix of fixed size.
  */
 
@@ -128,20 +126,14 @@
 
     /** \brief Check if matrix is the same object as the other matrix */
     bool identical(const DiagonalMatrix<K,n>& other) const
     {
       return (this==&other);
     }
 
-    /** \brief Return transposed of the matrix as DiagonalMatrix */
-    DiagonalMatrix<K, n> transposed() const
-    {
-      return *this;
-    }
-
     //===== iterator interface to rows of the matrix
     //! Iterator class for sequential access
     typedef ContainerWrapperIterator<const WrapperType, reference, reference> Iterator;
     //! typedef for stl compliant access
     typedef Iterator iterator;
     //! rename the iterators for easier access
     typedef Iterator RowIterator;
@@ -456,30 +448,14 @@
       for (int i=1; i<n; i++)
         det *= diag_[i];
       return det;
     }
 
 
 
-    //===== matrix-matrix multiplication
-
-    /** \brief Matrix-matrix multiplication
-     */
-    template <class OtherScalar>
-    friend auto operator* ( const DiagonalMatrix& matrixA,
-                            const DiagonalMatrix<OtherScalar, n>& matrixB)
-    {
-      auto result = DiagonalMatrix<typename PromotionTraits<K,OtherScalar>::PromotedType, n>{};
-      for(int i=0; i<n; ++i)
-        result.diagonal(i) = matrixA.diagonal(i)*matrixB.diagonal(i);
-      return result;
-    }
-
-
-
     //===== sizes
 
     //! number of blocks in row direction
     static constexpr size_type N ()
     {
       return n;
     }
@@ -622,29 +598,14 @@
 
     //! Get reference to diagonal vector
     FieldVector<K,1>& diagonal()
     {
       return (*this)[0];
     }
 
-    /** \brief Return transposed of the matrix as DiagonalMatrix */
-    DiagonalMatrix<K, 1> transposed() const
-    {
-      return *this;
-    }
-
-    /** \brief Matrix-matrix multiplication
-     */
-    template <class OtherScalar>
-    friend auto operator* ( const DiagonalMatrix& matrixA,
-                            const DiagonalMatrix<OtherScalar, 1>& matrixB)
-    {
-      return DiagonalMatrix<typename PromotionTraits<K,OtherScalar>::PromotedType, 1>{matrixA.diagonal(0)*matrixB.diagonal(0)};
-    }
-
   };
 #endif
 
 
   template<class DiagonalMatrixType>
   class DiagonalMatrixWrapper
   {
```

### Comparing `dune-common-2.9.0rc1/dune/common/documentation.hh` & `dune-common-2.9.dev20220529/dune/common/documentation.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_DOCUMENTATION_HH
 #define DUNE_COMMON_DOCUMENTATION_HH
 
 /** \file
     \brief Documentation related stuff
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/dotproduct.hh` & `dune-common-2.9.dev20220529/dune/common/dotproduct.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DOTPRODUCT_HH
 #define DUNE_DOTPRODUCT_HH
 
 #include "ftraits.hh"
 #include "typetraits.hh"
 
 namespace Dune {
```

### Comparing `dune-common-2.9.0rc1/dune/common/dynmatrix.hh` & `dune-common-2.9.dev20220529/dune/common/dynmatrix.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DYNMATRIX_HH
 #define DUNE_DYNMATRIX_HH
 
 #include <cmath>
 #include <cstddef>
 #include <iostream>
 #include <initializer_list>
@@ -124,24 +122,14 @@
     template <typename T,
               typename = std::enable_if_t<Dune::IsNumber<T>::value>>
     DynamicMatrix& operator=(T scalar) {
       std::fill(_data.begin(), _data.end(), scalar);
       return *this;
     }
 
-    //! Return transposed of the matrix as DynamicMatrix
-    DynamicMatrix transposed() const
-    {
-      DynamicMatrix AT(this->M(), this->N());
-      for( size_type i = 0; i < this->N(); ++i )
-        for( size_type j = 0; j < this->M(); ++j )
-          AT[j][i] = (*this)[i][j];
-      return AT;
-    }
-
     // make this thing a matrix
     size_type mat_rows() const { return _data.size(); }
     size_type mat_cols() const {
       assert(this->rows());
       return _data.front().size();
     }
     row_type & mat_access(size_type i) {
```

### Comparing `dune-common-2.9.0rc1/dune/common/dynmatrixev.hh` & `dune-common-2.9.dev20220529/dune/common/dynmatrixev.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DYNMATRIXEIGENVALUES_HH
 #define DUNE_DYNMATRIXEIGENVALUES_HH
 
 #include <algorithm>
 #include <memory>
 
 #include "dynmatrix.hh"
```

### Comparing `dune-common-2.9.0rc1/dune/common/dynvector.hh` & `dune-common-2.9.dev20220529/dune/common/dynvector.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DYNVECTOR_HH
 #define DUNE_DYNVECTOR_HH
 
 #include <cmath>
 #include <cstddef>
 #include <cstdlib>
 #include <complex>
@@ -173,15 +171,15 @@
     const container_type &container () const { return _data; }
     container_type &container () { return _data; }
   };
 
   /** \brief Read a DynamicVector from an input stream
    *  \relates DynamicVector
    *
-   *  \note This operator is STL compliant, i.e., the content of v is only
+   *  \note This operator is STL compilant, i.e., the content of v is only
    *        changed if the read operation is successful.
    *
    *  \param[in]  in  std :: istream to read from
    *  \param[out] v   DynamicVector to be read
    *
    *  \returns the input stream (in)
    */
```

### Comparing `dune-common-2.9.0rc1/dune/common/enumset.hh` & `dune-common-2.9.dev20220529/dune/common/enumset.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ENUMSET_HH
 #define DUNE_ENUMSET_HH
 
 #include <iostream>
 
 namespace Dune
 {
```

### Comparing `dune-common-2.9.0rc1/dune/common/exceptions.hh` & `dune-common-2.9.dev20220529/dune/common/exceptions.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_EXCEPTIONS_HH
 #define DUNE_EXCEPTIONS_HH
 
 #include <exception>
 #include <string>
 #include <sstream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/float_cmp.cc` & `dune-common-2.9.dev20220529/dune/common/float_cmp.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "float_cmp.hh"
 
 #include <vector>
 #include <limits>
 #include <algorithm>
 #include <cstdlib>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/float_cmp.hh` & `dune-common-2.9.dev20220529/dune/common/float_cmp.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_FLOAT_CMP_HH
 #define DUNE_COMMON_FLOAT_CMP_HH
 
 /** \file
  * \brief Various ways to compare floating-point numbers
  */
 
@@ -40,15 +38,15 @@
    next paragraph.
 
    There is another way of comparing approximately, using a @em relative
    epsilon which is then scaled with first:
    @code
     abs(first-second) <= epsilon * abs(first)
    @endcode
-   Of course the comparison should be symmetric in first and second so we
+   Of cource the comparison should be symmetric in first and second so we
    cannot arbitrarily select either first or second to scale epsilon.  The are
    two symmetric variants, @em relative_weak
    @code
     abs(first-second) <= epsilon * max(abs(first), abs(second))
    @endcode
    and @em relative_strong
    @code
```

### Comparing `dune-common-2.9.0rc1/dune/common/fmatrix.hh` & `dune-common-2.9.dev20220529/dune/common/fmatrix.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FMATRIX_HH
 #define DUNE_FMATRIX_HH
 
 #include <cmath>
 #include <cstddef>
 #include <iostream>
 #include <algorithm>
@@ -14,77 +12,31 @@
 #include <dune/common/boundschecking.hh>
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/densematrix.hh>
 #include <dune/common/precision.hh>
 #include <dune/common/promotiontraits.hh>
 #include <dune/common/typetraits.hh>
-#include <dune/common/matrixconcepts.hh>
 
 namespace Dune
 {
 
-  namespace Impl
-  {
-
-    template<class M>
-    class ColumnVectorView
-    {
-    public:
-
-      using value_type = typename M::value_type;
-      using size_type = typename M::size_type;
-
-      constexpr ColumnVectorView(M& matrix, size_type col) :
-        matrix_(matrix),
-        col_(col)
-      {}
-
-      constexpr size_type N () const {
-        return matrix_.N();
-      }
-
-      template<class M_ = M,
-        std::enable_if_t<std::is_same_v<M_,M> and not std::is_const_v<M_>, int> = 0>
-      constexpr value_type& operator[] (size_type row) {
-        return matrix_[row][col_];
-      }
-
-      constexpr const value_type& operator[] (size_type row) const {
-        return matrix_[row][col_];
-      }
-
-    protected:
-      M& matrix_;
-      const size_type col_;
-    };
-
-  }
-
-  template<typename M>
-  struct FieldTraits< Impl::ColumnVectorView<M> >
-  {
-    using field_type = typename FieldTraits<M>::field_type;
-    using real_type = typename FieldTraits<M>::real_type;
-  };
-
   /**
       @addtogroup DenseMatVec
       @{
    */
 
   /*! \file
 
      \brief  Implements a matrix constructed from a given type
      representing a field and compile-time given number of rows and columns.
    */
 
   template< class K, int ROWS, int COLS = ROWS > class FieldMatrix;
 
-
   template< class K, int ROWS, int COLS >
   struct DenseMatVecTraits< FieldMatrix<K,ROWS,COLS> >
   {
     typedef FieldMatrix<K,ROWS,COLS> derived_type;
 
     // each row is implemented by a field vector
     typedef FieldVector<K,COLS> row_type;
@@ -164,24 +116,14 @@
       return *this;
     }
 
     //! no copy assignment from FieldMatrix of different size
     template <typename T, int rows, int cols>
     FieldMatrix& operator=(FieldMatrix<T,rows,cols> const&) = delete;
 
-    //! Return transposed of the matrix as FieldMatrix
-    FieldMatrix<K, COLS, ROWS> transposed() const
-    {
-      Dune::FieldMatrix<K, COLS, ROWS> AT;
-      for( int i = 0; i < ROWS; ++i )
-        for( int j = 0; j < COLS; ++j )
-          AT[j][i] = (*this)[i][j];
-      return AT;
-    }
-
     //! vector space addition -- two-argument version
     template <class OtherScalar>
     friend auto operator+ ( const FieldMatrix& matrixA,
                             const FieldMatrix<OtherScalar,ROWS,COLS>& matrixB)
     {
       FieldMatrix<typename PromotionTraits<K,OtherScalar>::PromotedType,ROWS,COLS> result;
 
@@ -263,58 +205,14 @@
           for (size_type k = 0; k < matrixA.mat_cols(); ++k)
             result[i][j] += matrixA[i][k] * matrixB[k][j];
         }
 
       return result;
     }
 
-    /** \brief Matrix-matrix multiplication
-     *
-     * This implements multiplication of a FieldMatrix with another matrix
-     * of type OtherMatrix. The latter has to provide
-     * OtherMatrix::field_type, OtherMatrix::cols, and OtherMatrix::mtv(x,y).
-     */
-    template <class OtherMatrix, std::enable_if_t<
-      Impl::IsStaticSizeMatrix_v<OtherMatrix>
-      and not Impl::IsFieldMatrix_v<OtherMatrix>
-      , int> = 0>
-    friend auto operator* ( const FieldMatrix& matrixA,
-                            const OtherMatrix& matrixB)
-    {
-      using Field = typename PromotionTraits<K, typename OtherMatrix::field_type>::PromotedType;
-      Dune::FieldMatrix<Field, rows ,OtherMatrix::cols> result;
-      for (std::size_t j=0; j<rows; ++j)
-        matrixB.mtv(matrixA[j], result[j]);
-      return result;
-    }
-
-    /** \brief Matrix-matrix multiplication
-     *
-     * This implements multiplication of another matrix
-     * of type OtherMatrix with a FieldMatrix. The former has to provide
-     * OtherMatrix::field_type, OtherMatrix::rows, and OtherMatrix::mv(x,y).
-     */
-    template <class OtherMatrix, std::enable_if_t<
-      Impl::IsStaticSizeMatrix_v<OtherMatrix>
-      and not Impl::IsFieldMatrix_v<OtherMatrix>
-      , int> = 0>
-    friend auto operator* ( const OtherMatrix& matrixA,
-                            const FieldMatrix& matrixB)
-    {
-      using Field = typename PromotionTraits<K, typename OtherMatrix::field_type>::PromotedType;
-      Dune::FieldMatrix<Field, OtherMatrix::rows, cols> result;
-      for (std::size_t j=0; j<cols; ++j)
-      {
-        auto B_j = Impl::ColumnVectorView(matrixB, j);
-        auto result_j = Impl::ColumnVectorView(result, j);
-        matrixA.mv(B_j, result_j);
-      }
-      return result;
-    }
-
     //! Multiplies M from the left to this matrix, this matrix is not modified
     template<int l>
     FieldMatrix<K,l,cols> leftmultiplyany (const FieldMatrix<K,l,rows>& M) const
     {
       FieldMatrix<K,l,cols> C;
 
       for (size_type i=0; i<l; i++) {
@@ -428,20 +326,14 @@
     FieldMatrix(T const& rhs)
     {
       *this = rhs;
     }
 
     using Base::operator=;
 
-    //! Return transposed of the matrix as FieldMatrix
-    FieldMatrix<K, 1, 1> transposed() const
-    {
-      return *this;
-    }
-
     //! vector space addition -- two-argument version
     template <class OtherScalar>
     friend auto operator+ ( const FieldMatrix& matrixA,
                             const FieldMatrix<OtherScalar,1,1>& matrixB)
     {
       return FieldMatrix<typename PromotionTraits<K,OtherScalar>::PromotedType,1,1>{matrixA[0][0] + matrixB[0][0]};
     }
@@ -526,60 +418,14 @@
 
       for (size_type j = 0; j < matrixB.mat_cols(); ++j)
         result[0][j] = matrixA[0][0] * matrixB[0][j];
 
       return result;
     }
 
-    /** \brief Matrix-matrix multiplication
-     *
-     * This implements multiplication of a FieldMatrix with another matrix
-     * of type OtherMatrix. The latter has to provide
-     * OtherMatrix::field_type, OtherMatrix::cols, and OtherMatrix::mtv(x,y).
-     */
-    template <class OtherMatrix, std::enable_if_t<
-      Impl::IsStaticSizeMatrix_v<OtherMatrix>
-      and not Impl::IsFieldMatrix_v<OtherMatrix>
-      and (OtherMatrix::rows==1)
-      , int> = 0>
-    friend auto operator* ( const FieldMatrix& matrixA,
-                            const OtherMatrix& matrixB)
-    {
-      using Field = typename PromotionTraits<K, typename OtherMatrix::field_type>::PromotedType;
-      Dune::FieldMatrix<Field, rows ,OtherMatrix::cols> result;
-      for (std::size_t j=0; j<rows; ++j)
-        matrixB.mtv(matrixA[j], result[j]);
-      return result;
-    }
-
-    /** \brief Matrix-matrix multiplication
-     *
-     * This implements multiplication of another matrix
-     * of type OtherMatrix with a FieldMatrix. The former has to provide
-     * OtherMatrix::field_type, OtherMatrix::rows, and OtherMatrix::mv(x,y).
-     */
-    template <class OtherMatrix, std::enable_if_t<
-      Impl::IsStaticSizeMatrix_v<OtherMatrix>
-      and not Impl::IsFieldMatrix_v<OtherMatrix>
-      and (OtherMatrix::cols==1)
-      , int> = 0>
-    friend auto operator* ( const OtherMatrix& matrixA,
-                            const FieldMatrix& matrixB)
-    {
-      using Field = typename PromotionTraits<K, typename OtherMatrix::field_type>::PromotedType;
-      Dune::FieldMatrix<Field, OtherMatrix::rows, cols> result;
-      for (std::size_t j=0; j<cols; ++j)
-      {
-        auto B_j = Impl::ColumnVectorView(matrixB, j);
-        auto result_j = Impl::ColumnVectorView(result, j);
-        matrixA.mv(B_j, result_j);
-      }
-      return result;
-    }
-
     //! Multiplies M from the left to this matrix, this matrix is not modified
     template<int l>
     FieldMatrix<K,l,1> leftmultiplyany (const FieldMatrix<K,l,1>& M) const
     {
       FieldMatrix<K,l,1> C;
       for (size_type j=0; j<l; j++)
         C[j][0] = M[j][0]*(*this)[0][0];
```

### Comparing `dune-common-2.9.0rc1/dune/common/fmatrixev.cc` & `dune-common-2.9.dev20220529/dune/common/fmatrixev.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FMATRIXEIGENVALUES_CC
 #define DUNE_FMATRIXEIGENVALUES_CC
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
```

### Comparing `dune-common-2.9.0rc1/dune/common/fmatrixev.hh` & `dune-common-2.9.dev20220529/dune/common/fmatrixev.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FMATRIXEIGENVALUES_HH
 #define DUNE_FMATRIXEIGENVALUES_HH
 
 /** \file
  * \brief Eigenvalue computations for the FieldMatrix class
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/ftraits.hh` & `dune-common-2.9.dev20220529/dune/common/ftraits.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FTRAITS_HH
 #define DUNE_FTRAITS_HH
 
 /** \file
  * \brief Type traits to determine the type of reals (when working with complex numbers)
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/function.hh` & `dune-common-2.9.dev20220529/dune/common/function.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FUNCTION_HH_SILENCE_DEPRECATION
 #warning This file is deprecated after Dune 2.7!  Use C++ function objects and std::function stuff instead!
 #else // !DUNE_FUNCTION_HH_SILENCE_DEPRECATION
 #undef DUNE_FUNCTION_HH_SILENCE_DEPRECATION
 #endif // !DUNE_FUNCTION_HH_SILENCE_DEPRECATION
 
 #ifndef DUNE_FUNCTION_HH
```

### Comparing `dune-common-2.9.0rc1/dune/common/fvector.hh` & `dune-common-2.9.dev20220529/dune/common/fvector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_FVECTOR_HH
 #define DUNE_FVECTOR_HH
 
 #include <array>
 #include <cmath>
 #include <cstddef>
 #include <cstdlib>
```

### Comparing `dune-common-2.9.0rc1/dune/common/genericiterator.hh` & `dune-common-2.9.dev20220529/dune/common/genericiterator.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GENERICITERATOR_HH
 #define DUNE_GENERICITERATOR_HH
 
 #include <dune/common/iteratorfacades.hh>
 #include <cassert>
 
 namespace Dune {
```

### Comparing `dune-common-2.9.0rc1/dune/common/gmpfield.hh` & `dune-common-2.9.dev20220529/dune/common/gmpfield.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GMPFIELD_HH
 #define DUNE_GMPFIELD_HH
 
 /** \file
  * \brief Wrapper for the GNU multiprecision (GMP) library
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/hash.hh` & `dune-common-2.9.dev20220529/dune/common/hash.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_HASH_HH
 #define DUNE_COMMON_HASH_HH
 
 #include <functional>
 
 #include <dune/common/typetraits.hh>
 
@@ -177,15 +175,15 @@
 // are part of C99.
 #define DUNE_HASH_TEMPLATE_ARGS(...) (__VA_ARGS__)
 
 // Wrapper macro for type to be hashed.
 // See above for rationale.
 #define DUNE_HASH_TYPE(...) (__VA_ARGS__)
 
-// Expansion macro for the parenthesized argument lists created by
+// Expansion macro for the parenthesed argument lists created by
 // DUNE_HASH_TEMPLATE_ARGS and DUNE_HASH_TYPE.
 #define DUNE_HASH_EXPAND_VA_ARGS(...) __VA_ARGS__
 
 // Define specializations for all discovered hash implementations.
 #define DUNE_DEFINE_HASH(template_args,type)                                                  \
   DUNE_DEFINE_STD_HASH(DUNE_HASH_EXPAND_VA_ARGS template_args, DUNE_HASH_EXPAND_VA_ARGS type) \
 
@@ -330,15 +328,15 @@
   }
 
   //! Hashes all elements in the range [first,last) and combines the hashes in-place with seed.
   /**
    *
    * \param seed   Start value that will be combined with the hash values of all objects in
    *               the range using hash_combine() in sequential fashion.
-   * \param first  Iterator pointing to the first object to hash.
+   * \param first  Iterator pointing to the first ojbect to hash.
    * \param last   Iterator pointing one past the last object to hash.
    */
   template<typename It>
   inline void hash_range(std::size_t& seed, It first, It last)
   {
     for (; first != last; ++first)
     {
```

### Comparing `dune-common-2.9.0rc1/dune/common/hybridutilities.hh` & `dune-common-2.9.dev20220529/dune/common/hybridutilities.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_HYBRIDUTILITIES_HH
 #define DUNE_COMMON_HYBRIDUTILITIES_HH
 
 #include <tuple>
 #include <utility>
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/indent.hh` & `dune-common-2.9.dev20220529/dune/common/indent.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_INDENT_HH
 #define DUNE_COMMON_INDENT_HH
 
 #include <ostream>
 #include <string>
 
 namespace Dune {
```

### Comparing `dune-common-2.9.0rc1/dune/common/indices.hh` & `dune-common-2.9.dev20220529/dune/common/indices.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_INDICES_HH
 #define DUNE_COMMON_INDICES_HH
 
 #include <cstddef>
 #include <type_traits>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/common/interfaces.hh` & `dune-common-2.9.dev20220529/dune/common/interfaces.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_INTERFACES_HH
 #define DUNE_INTERFACES_HH
 
 /** @file
    @author Robert Kloefkorn
    @brief Provides interfaces for detection of specific behavior
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/ios_state.hh` & `dune-common-2.9.dev20220529/dune/common/ios_state.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_IOS_STATE_HH
 #define DUNE_COMMON_IOS_STATE_HH
 
 #include <ios>
 
 namespace Dune {
   /** @addtogroup Common
```

### Comparing `dune-common-2.9.0rc1/dune/common/iteratorfacades.hh` & `dune-common-2.9.dev20220529/dune/common/iteratorfacades.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ITERATORFACADES_HH
 #define DUNE_ITERATORFACADES_HH
 
 #include <iterator>
 #include <type_traits>
 
 #include "typetraits.hh"
```

### Comparing `dune-common-2.9.0rc1/dune/common/iteratorrange.hh` & `dune-common-2.9.dev20220529/dune/common/iteratorrange.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_ITERATORRANGE_HH
 #define DUNE_COMMON_ITERATORRANGE_HH
 
 namespace Dune {
 
   //! Simple range between a begin and an end iterator.
   /**
```

### Comparing `dune-common-2.9.0rc1/dune/common/keywords.hh` & `dune-common-2.9.dev20220529/dune/common/keywords.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_KEYWORDS_HH
 #define DUNE_COMMON_KEYWORDS_HH
 
 /** \file
  * \brief Definitions of several macros that conditionally make C++ syntax
  *      available.
  *
```

### Comparing `dune-common-2.9.0rc1/dune/common/lru.hh` & `dune-common-2.9.dev20220529/dune/common/lru.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_LRU_HH
 #define DUNE_COMMON_LRU_HH
 
 #include <list>
 #include <utility>
 #include <map>
 #include <memory>
```

### Comparing `dune-common-2.9.0rc1/dune/common/mallocallocator.hh` & `dune-common-2.9.dev20220529/dune/common/mallocallocator.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MALLOC_ALLOCATOR_HH
 #define DUNE_MALLOC_ALLOCATOR_HH
 
 #include <exception>
 #include <cstdlib>
 #include <new>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/common/math.hh` & `dune-common-2.9.dev20220529/dune/common/math.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MATH_HH
 #define DUNE_MATH_HH
 
 /** \file
  * \brief Some useful basic math stuff
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/matvectraits.hh` & `dune-common-2.9.dev20220529/dune/common/matvectraits.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MATVECTRAITS_HH
 #define DUNE_MATVECTRAITS_HH
 
 /** \file
  * \brief Documentation of the traits classes you need to write for each implementation of DenseVector or DenseMatrix
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/overloadset.hh` & `dune-common-2.9.dev20220529/dune/common/overloadset.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_OVERLOADSET_HH
 #define DUNE_COMMON_OVERLOADSET_HH
 
 #include <utility>
 #include <type_traits>
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/CMakeLists.txt` & `dune-common-2.9.dev20220529/dune/common/parallel/CMakeLists.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory(test)
 add_subdirectory(benchmark)
 
 #install headers
 install(FILES
         collectivecommunication.hh
         communication.hh
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/benchmark/mpi_collective_benchmark.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/benchmark/mpi_collective_benchmark.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /**
  * @brief Benchmark for measure the possible overlap of computation
  * and communication at MPI collective communications.
  *
  * This benchmark is inspired by the sandia micro benchmark:
  * W. Lawry, C. Wilson, A. Maccabe, R. Brightwell. COMB: A Portable Benchmark
@@ -38,15 +36,15 @@
  *
  * options:
  * -method: default: allreduce.
  *                   possible methods: allreduce, barrier,
  *                   broadcast, gather, allgather, scatter
  * -iterations: default: 10000. Number of iterations for
  *              measure the time for one communication
- * -allMethods: default:0. If 1 iterates over all available methods
+ * -allMethods: defaukt:0. If 1 iterates over all available methods
  * -startSize: default: n, where n is the size of MPI_COMM_WORLD. runs
  *             the benchmark for different communicator sizes, starting with
  *             startSize. After every run the size is doubled. Finally one run is
  *             made for the whole communicator.
  * -verbose: default: 0. If 1 prints intermediate information while determining
  *           the overhead.
  * -threshold: default: 2. The threshold when the work time is the dominant
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/communication.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/communication.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARALLEL_COMMUNICATION_HH
 #define DUNE_COMMON_PARALLEL_COMMUNICATION_HH
 /*!
    \file
    \brief Implements an utility class that provides
    collective communication methods for sequential programs.
 
@@ -533,12 +531,12 @@
   /**
    * \deprecated CollectiveCommunication is deprecated and will be removed after Dune 2.9.
    *
    * Use Communication instead.
    */
   template<class T>
   using CollectiveCommunication
-  [[deprecated("CollectiveCommunication is deprecated. Use Communication instead.")]]
+  //[[deprecated("CollectiveCommunication is deprecated. Use Communication instead.")]]
   = Communication<T>;
 }
 
 #endif
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/communicator.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/communicator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMUNICATOR
 #define DUNE_COMMUNICATOR
 
 #if HAVE_MPI
 
 #include <cassert>
 #include <cstddef>
@@ -82,17 +80,17 @@
    *
    * Based on the information about the distributed index sets,  data
    * independent interfaces between different sets of the index sets
    * can be setup using the class Interface.  For the actual communication
    * data dependent communicators can be setup using BufferedCommunicator,
    * DatatypeCommunicator VariableSizeCommunicator based on the interface
    * information. In contrast to the former
-   * the latter is independent of the class Interface which can work on a map
+   * the latter is independent of the class Interface can work on a map
    * from process number to a pair of index lists describing which local indices
-   * are sent and received from that process.
+   * are send and received from that processs, respectively.
    */
   /** @addtogroup Common_Parallel
    *
    * @{
    */
   /**
    * @file
@@ -159,15 +157,15 @@
      * get the address.
      * @param v An existing representation of the type that has more elements than index.
      * @param index The index of the entry.
      */
     static const void* getAddress(const V& v, int index);
 
     /**
-     * @brief Get the number of primitive elements at that index.
+     * @brief Get the number of primitve elements at that index.
      *
      * The default always returns 1.
      */
     static int getSize(const V&, int index);
   };
 
   template<class K, int n> class FieldVector;
@@ -617,22 +615,22 @@
      * @brief The type of the map that maps interface information to processors.
      */
     typedef std::map<int,std::pair<InterfaceInformation,InterfaceInformation> >
     InterfaceMap;
 
 
     /**
-     * @brief Functors for message size calculation
+     * @brief Functors for message size caculation
      */
     template<class Data, typename IndexedTypeFlag>
     struct MessageSizeCalculator
     {};
 
     /**
-     * @brief Functor for message size calculation for datatypes
+     * @brief Functor for message size caculation for datatypes
      * where at each index is only one value.
      */
     template<class Data>
     struct MessageSizeCalculator<Data,SizeOne>
     {
       /**
        * @brief Calculate the number of values in message
@@ -649,15 +647,15 @@
        * @param data ignored.
        * @return The number of values in th message.
        */
       inline int operator()(const Data& data, const InterfaceInformation& info) const;
     };
 
     /**
-     * @brief Functor for message size calculation for datatypes
+     * @brief Functor for message size caculation for datatypes
      * where at each index can be a variable number of values.
      */
     template<class Data>
     struct MessageSizeCalculator<Data,VariableSize>
     {
       /**
        * @brief Calculate the number of values in message
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/future.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/future.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARALLEL_FUTURE_HH
 #define DUNE_COMMON_PARALLEL_FUTURE_HH
 
 #include <memory>
 #include <dune/common/exceptions.hh>
 
 namespace Dune{
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/indexset.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/indexset.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_INDEXSET_HH
 #define DUNE_INDEXSET_HH
 
 #include <algorithm>
 #include <dune/common/arraylist.hh>
 #include <dune/common/exceptions.hh>
 #include <iostream>
@@ -756,15 +754,15 @@
   template<class TG, class TL>
   inline void IndexPair<TG,TL>::setLocal(int local){
     local_=local;
   }
 
   template<class TG, class TL, int N>
   ParallelIndexSet<TG,TL,N>::ParallelIndexSet()
-    : state_(GROUND), seqNo_(0), deletedEntries_()
+    : state_(GROUND), seqNo_(0)
   {}
 
   template<class TG, class TL, int N>
   void ParallelIndexSet<TG,TL,N>::beginResize()
   {
 
     // Checks in unproductive code
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/indicessyncer.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/indicessyncer.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_INDICESSYNCER_HH
 #define DUNE_INDICESSYNCER_HH
 
 #include "indexset.hh"
 #include "remoteindices.hh"
 #include <dune/common/stdstreams.hh>
 #include <dune/common/sllist.hh>
@@ -134,15 +132,15 @@
     /**
      * @brief Default numberer for sync().
      */
     class DefaultNumberer
     {
     public:
       /**
-       * @brief Provide the local index, always
+       * @brief Provide the lcoal index, always
        * std::numeric_limits<size_t>::max()
        * @param global The global index (ignored).
        */
       std::size_t operator()([[maybe_unused]] const GlobalIndex& global)
       {
         return std::numeric_limits<size_t>::max();
       }
@@ -179,20 +177,20 @@
      * resorting the index set entries one has store the corresponding
      * global index for each remote index. Thus the pointers can be adjusted
      * properly as a last step.
      */
     GlobalIndicesMap globalMap_;
 
     /**
-     * @brief The type of the singly linked list of bools.
+     * @brief The type of the single linked list of bools.
      */
     typedef SLList<bool, typename RemoteIndices::Allocator> BoolList;
 
     /**
-     * @brief The mutable iterator of the singly linked bool list.
+     * @brief The mutable iterator of the single linked bool list.
      */
     typedef typename BoolList::iterator BoolIterator;
 
     /** @brief The type of the modifying iterator for the list of bools. */
     typedef typename BoolList::ModifyIterator BoolListModifier;
 
     /** @brief The type of the map of bool lists. */
@@ -225,28 +223,28 @@
     /** @brief Type of the tuple of iterators needed for the adding of indices. */
     typedef std::tuple<RemoteIndexModifier,GlobalIndexModifier,BoolListModifier,
         const ConstRemoteIndexIterator> IteratorTuple;
 
     /**
      * @brief A tuple of iterators.
      *
-     * Insertion into a singly linked list is only possible at the position after the one of the iterator.
+     * Insertion into a single linked list is only possible at the position after the one of the iterator.
      * Therefore for each linked list two iterators are needed: One position before the actual entry
      * (for insertion) and one positioned at the actual position (for searching).
      */
     class Iterators
     {
       friend class IndicesSyncer<T>;
     public:
       /**
        * @brief Constructor.
        *
        * Initializes all iterator to first entry and the one before the first entry, respectively.
        * @param remoteIndices The list of the remote indices.
-       * @param globalIndices The list of the corresponding global indices. This is needed because the
+       * @param globalIndices The list of the coresponding global indices. This is needed because the
        * the pointers to the local index will become invalid due to the merging of the index sets.
        * @param booleans Whether the remote index was there before the sync process started.
        */
       Iterators(RemoteIndexList& remoteIndices, GlobalIndexList& globalIndices,
                 BoolList& booleans);
 
       /**
@@ -289,15 +287,15 @@
       bool isOld() const;
 
       /**
        * @brief Reset all the underlying iterators.
        *
        * Position them to first list entry and the entry before the first entry respectively.
        * @param remoteIndices The list of the remote indices.
-       * @param globalIndices The list of the corresponding global indices. This is needed because the
+       * @param globalIndices The list of the coresponding global indices. This is needed because the
        * the pointers to the local index will become invalid due to the merging of the index sets.
        * @param booleans Whether the remote index was there before the sync process started.
        */
       void reset(RemoteIndexList& remoteIndices, GlobalIndexList& globalIndices,
                  BoolList& booleans);
 
       /**
@@ -314,19 +312,19 @@
        */
       bool isAtEnd() const;
 
     private:
       /**
        * @brief The iterator tuple.
        *
-       * The tuple consists of one iterator over a singly linked list of remote indices
-       * initially positioned before the first entry, one over a singly linked list of global indices
-       * , one over a singly linked list of bool values both positioned at the same entry. The another three
+       * The tuple consists of one iterator over a single linked list of remote indices
+       * initially positioned before the first entry, one over a sll of global indices
+       * , one over a all of bool values both postioned at the same entry. The another three
        * iterators of the same type positioned at the first entry. Last an iterator over the
-       * singly linked list of remote indices positioned at the end.
+       * sll of remote indices positioned at the end.
        */
       IteratorTuple iterators_;
     };
 
     /** @brief Type of the map from ranks to iterator tuples. */
     typedef std::map<int,Iterators> IteratorsMap;
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/interface.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/interface.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_INTERFACE_HH
 #define DUNE_INTERFACE_HH
 
 #if HAVE_MPI
 
 #include "remoteindices.hh"
 #include <dune/common/enumset.hh>
@@ -368,15 +366,15 @@
 
     int rank;
 
     MPI_Comm_rank(remoteIndices.communicator(), &rank);
 
     // Allocate memory for the type construction.
     for(const_iterator process=remoteIndices.begin(); process != end; ++process) {
-      // Measure the number of indices sent to the remote process first
+      // Messure the number of indices send to the remote process first
       int size=0;
       typedef typename RemoteIndices::RemoteIndexList::const_iterator RemoteIterator;
       const RemoteIterator remoteEnd = send ? process->second.first->end() :
                                        process->second.second->end();
       RemoteIterator remote = send ? process->second.first->begin() : process->second.second->begin();
 
       while(remote!=remoteEnd) {
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/localindex.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/localindex.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_LOCALINDEX_HH
 #define DUNE_COMMON_LOCALINDEX_HH
 
 #include <cstddef>
 
 namespace Dune
@@ -18,15 +16,15 @@
    */
   /**
    * @file
    * @brief Provides classes for use as the local index in ParallelIndexSet.
    * @author Markus Blatt
    */
   /**
-   * @brief The states available for the local indices.
+   * @brief The states avaiable for the local indices.
    * @see LocalIndex::state()
    */
   enum LocalIndexState {VALID, DELETED};
 
 
   /**
    * @brief An index present on the local process.
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpicommunication.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpicommunication.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARALLEL_MPICOMMUNICATION_HH
 #define DUNE_COMMON_PARALLEL_MPICOMMUNICATION_HH
 
 /*!
    \file
    \brief Implements an utility class that provides
    MPI's collective communication methods.
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpidata.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpidata.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_PARALLEL_MPIDATA_HH
 #define DUNE_COMMON_PARALLEL_MPIDATA_HH
 
 #include <vector>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpifuture.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpifuture.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARALLEL_MPIFUTURE_HH
 #define DUNE_COMMON_PARALLEL_MPIFUTURE_HH
 
 #include <optional>
 
 #include <dune/common/parallel/communication.hh>
 #include <dune/common/parallel/future.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpiguard.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpiguard.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /**
  * @file
  * @brief Implements a MPIGuard which detects an error on a remote process
  * @author Christian Engwer
  * @ingroup ParallelCommunication
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpihelper.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpihelper.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MPIHELPER
 #define DUNE_MPIHELPER
 
 #if HAVE_MPI
 #include <cassert>
 #include <mpi.h>
 #endif
@@ -110,15 +108,15 @@
 
 
     /**
      * \deprecated getCollectionCommunication is deprecated and will be removed after Dune 2.9.
      *
      * Use getCommunication instead.
      */
-    [[deprecated("getCollectionCommunication is deprecated. Use getCommunication instead.")]]
+    //[[deprecated("getCollectionCommunication is deprecated. Use getCommunication instead.")]]
     static Communication<MPICommunicator> getCollectiveCommunication()
     {
       return Communication<MPICommunicator>(getCommunicator());
     }
 
     static Communication<MPICommunicator>
     getCommunication()
@@ -212,15 +210,15 @@
     }
 
     /**
      * \deprecated getCollectionCommunication is deprecated and will be removed after Dune 2.9.
      *
      * Use getCommunication instead.
      */
-    [[deprecated("getCollectionCommunication is deprecated. Use getCommunication instead.")]]
+    //[[deprecated("getCollectionCommunication is deprecated. Use getCommunication instead.")]]
     static Communication<MPICommunicator>
     getCollectiveCommunication()
     {
       return Communication<MPICommunicator>(getCommunicator());
     }
 
     static Communication<MPICommunicator>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpipack.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpipack.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /**
  * @file
  *
  * @brief See MPI_Pack.
  *
  * This Wrapper class takes care of the
  * memory management and provides methods to pack and unpack
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/mpitraits.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/mpitraits.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MPITRAITS_HH
 #define DUNE_MPITRAITS_HH
 
 /** @addtogroup ParallelCommunication
  *
  * @{
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/plocalindex.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/plocalindex.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_PLOCALINDEX_HH
 #define DUNE_PLOCALINDEX_HH
 
 #include "localindex.hh"
 #include "indexset.hh"
 #include "mpitraits.hh"
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/remoteindices.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/remoteindices.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REMOTEINDICES_HH
 #define DUNE_REMOTEINDICES_HH
 
 #if HAVE_MPI
 
 #include <cassert>
 #include <iostream>
@@ -358,28 +356,28 @@
      */
     template<bool mode, bool send>
     inline RemoteIndexListModifier<T,A,mode> getModifier(int process);
 
     /**
      * @brief Find an iterator over the remote index lists of a specific process.
      * @param proc The identifier of the process.
-     * @return The iterator the remote index lists positioned at the process.
-     * If there's is no list for this process, the end iterator is returned.
+     * @return The iterator the remote index lists postioned at the process.
+     * If theres is no list for this process, the end iterator is returned.
      */
     inline const_iterator find(int proc) const;
 
     /**
      * @brief Get an iterator over all remote index lists.
-     * @return The iterator over all remote index lists positioned at the first process.
+     * @return The iterator over all remote index lists postioned at the first process.
      */
     inline const_iterator begin() const;
 
     /**
      * @brief Get an iterator over all remote index lists.
-     * @return The iterator over all remote index lists positioned at the end.
+     * @return The iterator over all remote index lists postioned at the end.
      */
     inline const_iterator end() const;
 
     /**
      * @brief Get an iterator for colletively iterating over the remote indices of all remote processes.
      */
     template<bool send>
@@ -1152,15 +1150,15 @@
       destPublish = (ignorePublic) ? target_->size() : noPublic(*target_);
     else
       // we only need to send one set of indices
       destPublish = 0;
 
     int maxPublish, publish=sourcePublish+destPublish;
 
-    // Calculate maximum number of indices send
+    // Calucate maximum number of indices send
     MPI_Allreduce(&publish, &maxPublish, 1, MPI_INT, MPI_MAX, comm_);
 
     // allocate buffers
     PairType** destPairs;
     PairType** sourcePairs = new PairType*[sourcePublish>0 ? sourcePublish : 1];
 
     if(sendTwo)
@@ -1606,15 +1604,15 @@
   {
     static_assert(!mode,"Not allowed if the mode indicates that new indices"
                         "might be added to the underlying index set. Use "
                         "insert(const RemoteIndex&, const GlobalIndex&) instead");
 
 #ifdef DUNE_ISTL_WITH_CHECKING
     if(!first_ && index.localIndexPair().global()<last_)
-      DUNE_THROW(InvalidPosition, "Modification of remote indices have to occur with ascending global index.");
+      DUNE_THROW(InvalidPosition, "Modifcation of remote indices have to occur with ascending global index.");
 #endif
     // Move to the correct position
     while(iter_ != end_ && iter_->localIndexPair().global() < index.localIndexPair().global()) {
       ++iter_;
     }
 
     // No duplicate entries allowed
@@ -1650,15 +1648,15 @@
   }
 
   template<typename T, typename A, bool mode>
   bool RemoteIndexListModifier<T,A,mode>::remove(const GlobalIndex& global)
   {
 #ifdef DUNE_ISTL_WITH_CHECKING
     if(!first_ && global<last_)
-      DUNE_THROW(InvalidPosition, "Modification of remote indices have to occur with ascending global index.");
+      DUNE_THROW(InvalidPosition, "Modifcation of remote indices have to occur with ascending global index.");
 #endif
 
     bool found= false;
 
     if(MODIFYINDEXSET) {
       // Move to the correct position
       while(iter_!=end_ && *giter_< global) {
@@ -1835,28 +1833,28 @@
   inline std::ostream& operator<<(std::ostream& os, const RemoteIndices<T,A>& indices)
   {
     int rank;
     MPI_Comm_rank(indices.comm_, &rank);
     const auto rend = indices.remoteIndices_.end();
 
     for(auto rindex = indices.remoteIndices_.begin(); rindex!=rend; ++rindex) {
-      os<<rank<<": Process "<<rindex->first<<":";
+      os<<rank<<": Prozess "<<rindex->first<<":";
 
       if(!rindex->second.first->empty()) {
         os<<" send:";
 
         const auto send= rindex->second.first->end();
 
         for(auto index = rindex->second.first->begin();
             index != send; ++index)
           os<<*index<<" ";
         os<<std::endl;
       }
       if(!rindex->second.second->empty()) {
-        os<<rank<<": Process "<<rindex->first<<": "<<"receive: ";
+        os<<rank<<": Prozess "<<rindex->first<<": "<<"receive: ";
 
         for(const auto& index : *(rindex->second.second))
           os << index << " ";
       }
       os<<std::endl<<std::flush;
     }
     return os;
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/selection.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/selection.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_SELECTION_HH
 #define DUNE_SELECTION_HH
 
 #include "indexset.hh"
 #include <dune/common/iteratorfacades.hh>
 
 namespace Dune
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/CMakeLists.txt` & `dune-common-2.9.dev20220529/dune/common/parallel/test/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 dune_add_test(SOURCES communicationtest.cc
               LINK_LIBRARIES dunecommon
               MPI_RANKS 1 2 4
               TIMEOUT 300
               CMAKE_GUARD MPI_FOUND
               LABELS quick)
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/communicationtest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/communicationtest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #include <dune/common/parallel/mpihelper.hh>
 int main(int argc, char** argv)
 {
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/indexsettest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/indexsettest.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdlib>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/mpidatatest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/mpidatatest.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/dynmatrix.hh>
 #include <dune/common/parallel/mpidata.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/mpifuturetest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/mpifuturetest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <iostream>
 #include <numeric>
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/dynvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/mpipacktest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/mpipacktest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/remoteindicestest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/remoteindicestest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <algorithm>
 #include <iostream>
 #include <ostream>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/selectiontest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/selectiontest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/common/enumset.hh>
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/plocalindex.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/syncertest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/syncertest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <dune/common/parallel/indicessyncer.hh>
 #include <dune/common/sllist.hh>
 #include <string>
 #include <tuple>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/test/variablesizecommunicatortest.cc` & `dune-common-2.9.dev20220529/dune/common/parallel/test/variablesizecommunicatortest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 4 -*-
 // vi: set et ts=4 sw=4 sts=4:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <cstddef>
 #include <iostream>
 #include <set>
 #include <utility>
 #include <vector>
@@ -61,25 +59,25 @@
           std::cerr << rank << ": No data send at index " << idx << "!" << std::endl;
           std::abort();
         }
         dataSendAt.erase(it);
 
         it  = dataRecievedAt.find(idx);
         if(it == dataRecievedAt.end()) {
-          std::cerr << rank << ": No data received at index " << idx << "!" << std::endl;
+          std::cerr << rank << ": No data recieved at index " << idx << "!" << std::endl;
           std::abort();
         }
         dataRecievedAt.erase(it);
       }
       for(const int &i : dataSendAt) {
         std::cerr << rank << ": Unexpected data send at index " << i << "!" << std::endl;
         std::abort();
       }
       for(const int &i : dataRecievedAt) {
-        std::cerr << rank << ": Unexpected data received at index " << i << "!" << std::endl;
+        std::cerr << rank << ": Unexpected data recieved at index " << i << "!" << std::endl;
         std::abort();
       }
     }
     template<class B>
     void gather(B& buffer, int i)
     {
         if(!dataSendAt.insert(i).second) {
@@ -153,15 +151,15 @@
               std::abort();
             }
         }
         std::cout<<std::endl;
     }
 };
 
-// On the sending side, for each index to send, send between 0 and 4 numbers
+// On the sending side, for each index to send, send bewteen 0 and 4 numbers
 // (precisely: `index % 5` numbers).  The first number is the index converted
 // to `double`, incrementing by one for each consecutive number.  On the
 // receiving side just print the received numbers.
 struct VarDataHandle
 {
     std::set<int> dataSendAt;
     std::set<int> dataRecievedAt;
@@ -200,27 +198,27 @@
           std::cerr << rank << ": No data send at index " << idx << "!" << std::endl;
           std::abort();
         }
         dataSendAt.erase(it);
 
         it  = dataRecievedAt.find(idx);
         if(it == dataRecievedAt.end() && idx%5) {
-          std::cerr << rank << ": No data received at index " << idx << "!" << std::endl;
+          std::cerr << rank << ": No data recieved at index " << idx << "!" << std::endl;
           std::abort();
         }
         else if(it != dataRecievedAt.end()) {
           dataRecievedAt.erase(it);
         }
       }
       for(const int &i : dataSendAt) {
         std::cerr << rank << ": Unexpected data send at index " << i << "!" << std::endl;
         std::abort();
       }
       for(const int &i : dataRecievedAt) {
-        std::cerr << rank << ": Unexpected data received at index " << i << "!" << std::endl;
+        std::cerr << rank << ": Unexpected data recieved at index " << i << "!" << std::endl;
         std::abort();
       }
     }
     template<class B>
     void gather(B& buffer, int i)
     {
         if(!dataSendAt.insert(i).second) {
@@ -333,15 +331,15 @@
         std::cout<<"===================== backward ========================="<<std::endl;
         comm.backward(vhandle);
         vhandle.verify(procs, 0, 0);
     }
     else
     {
         // We also want to check the case where the interface is empty on some
-        // processes. Therefore we artificially lower the number of processes
+        // processes. Therefore we artificially lower the numer of processes
         // if it is larger than two. Thus the last rank will not send anything
         // and we check for deadlocks.
         if(procs>2)
             --procs;
 
         // Partition a consecutive set of indices among all active ranks
         // (where the final rank possibly excluded above is considered
```

### Comparing `dune-common-2.9.0rc1/dune/common/parallel/variablesizecommunicator.hh` & `dune-common-2.9.dev20220529/dune/common/parallel/variablesizecommunicator.hh`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARALLEL_VARIABLESIZECOMMUNICATOR_HH // Still fits the line!
 #define DUNE_COMMON_PARALLEL_VARIABLESIZECOMMUNICATOR_HH
 
 #if HAVE_MPI
 
 #include <algorithm>
 #include <cassert>
@@ -339,16 +337,16 @@
                    std::less<int>,
                    typename std::allocator_traits<Allocator>::template rebind_alloc< std::pair<const int,std::pair<InterfaceInformation,InterfaceInformation> > > > InterfaceMap;
 
 #ifndef DUNE_PARALLEL_MAX_COMMUNICATION_BUFFER_SIZE
   /**
    * @brief Creates a communicator with the default maximum buffer size.
    *
-   * The default size is either what the macro DUNE_MAX_COMMUNICATION_BUFFER_SIZE
-   * is set to, or 32768 if it is not set.
+   * The default size ist either what the macro DUNE_MAX_COMMUNICATION_BUFFER_SIZE
+   * is set to or 32768 if is not set.
    */
   VariableSizeCommunicator(MPI_Comm comm, const InterfaceMap& inf)
     : maxBufferSize_(32768), interface_(&inf)
   {
     MPI_Comm_dup(comm, &communicator_);
   }
   /**
@@ -360,16 +358,16 @@
   {
     MPI_Comm_dup(inf.communicator(), &communicator_);
   }
 #else
   /**
    * @brief Creates a communicator with the default maximum buffer size.
    *
-   * The default size is either what the macro DUNE_MAX_COMMUNICATION_BUFFER_SIZE
-   * is set to, or 32768 if it is not set.
+   * The default size ist either what the macro DUNE_MAX_COMMUNICATION_BUFFER_SIZE
+   * is set to or 32768 if is not set.
    */
   VariableSizeCommunicator(MPI_Comm comm, InterfaceMap& inf)
     : maxBufferSize_(DUNE_PARALLEL_MAX_COMMUNICATION_BUFFER_SIZE),
       interface_(&inf)
   {
     MPI_Comm_dup(comm, &communicator_);
   }
@@ -1014,15 +1012,15 @@
 
 /**
  * @brief Sets up all the send requests for the data.
  * @tparam DataHandle The type of the data handle.
  * @tparam Functor The type of the functor to set up the request.
  * @param handle The data handle describing the data.
  * @param trackers The trackers for the communication interfaces.
- * @param buffers The buffers for the communication. One for each neighbour.
+ * @param buffers The buffers for the comunication. One for each neighbour.
  * @param requests The send requests for each neighbour.
  * @param setupFunctor The functor responsible for setting up the request.
  */
 template<class DataHandle, class Functor>
 std::size_t setupRequests(DataHandle& handle,
                    std::vector<InterfaceTracker>& trackers,
                    std::vector<MessageBuffer<typename DataHandle::DataType> >& buffers,
```

### Comparing `dune-common-2.9.0rc1/dune/common/parameterizedobject.hh` & `dune-common-2.9.dev20220529/dune/common/parameterizedobject.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 4 -*-
 // vi: set et ts=4 sw=4 sts=4:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PARAMETERIZEDOBJECT_HH
 #define DUNE_COMMON_PARAMETERIZEDOBJECT_HH
 
 #include <functional>
 #include <map>
 #include <memory>
 
@@ -19,15 +17,15 @@
  *
  * It allows the construction of objects adhering to a certain interface that
  * might be constructed quite differently for one another.
  *
  * The Signature parameter defined the "virtual" constructor signature
  * in the form of Interface(Args...), where Interface is the type of
  * the (abstract) interface class and Args... is the set of
- * constructor parameters.
+ * constrcutor parameters.
  *
  * Each type constructed by this factory is identified by a different key. This class
  * allows for easy registration of type with new keys.
  *
  * @tparam Signature Signature of the "virtual" constructor call in the form for Interface(Args...). For default constructors one can omit the ()-brackets.
  * @tparam KeyT The type of the objects that are used as keys in the lookup [DEFAULT: std::string].
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/parametertree.cc` & `dune-common-2.9.dev20220529/dune/common/parametertree.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdlib>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/parametertree.hh` & `dune-common-2.9.dev20220529/dune/common/parametertree.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PARAMETERTREE_HH
 #define DUNE_PARAMETERTREE_HH
 
 /** \file
  * \brief A hierarchical structure of string parameters
  */
 
@@ -265,15 +263,15 @@
         DUNE_THROW(RangeError, " as a " << className<T>());
       return val;
     }
   };
 
   // "How do I convert a string into a wstring in C++?"  "Why, that very simple
   // son. You just need a these hundred lines of code."
-  // Instead im going to restrict myself to string with charT=char here.
+  // Instead im gonna restrict myself to string with charT=char here
   template<typename traits, typename Allocator>
   struct ParameterTree::Parser<std::basic_string<char, traits, Allocator> > {
     static std::basic_string<char, traits, Allocator>
     parse(const std::string& str) {
       std::string trimmed = ltrim(rtrim(str));
       return std::basic_string<char, traits, Allocator>(trimmed.begin(),
                                                         trimmed.end());
```

### Comparing `dune-common-2.9.0rc1/dune/common/parametertreeparser.cc` & `dune-common-2.9.dev20220529/dune/common/parametertreeparser.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include "parametertreeparser.hh"
```

### Comparing `dune-common-2.9.0rc1/dune/common/parametertreeparser.hh` & `dune-common-2.9.dev20220529/dune/common/parametertreeparser.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PARAMETER_PARSER_HH
 #define DUNE_PARAMETER_PARSER_HH
 
 /** \file
  * \brief Various parser methods to get data into a ParameterTree object
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/path.cc` & `dune-common-2.9.dev20220529/dune/common/path.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <algorithm>
 #include <iterator>
@@ -21,15 +19,15 @@
    * @ingroup Common
    * @{
    */
 
   /**
    * @file
    * @author Jö Fahlke <jorrit@jorrit.de>
-   * @brief Utilities for handling filesystem paths
+   * @brief Utilites for handling filesystem paths
    */
 
   //! concatenate two paths
   std::string concatPaths(const std::string& base, const std::string& p) {
     if(p == "") return base;
     if(p[0] == '/') return p;
     if(base == "") return p;
```

### Comparing `dune-common-2.9.0rc1/dune/common/path.hh` & `dune-common-2.9.dev20220529/dune/common/path.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PATH_HH
 #define DUNE_COMMON_PATH_HH
 
 #include <string>
 
 namespace Dune {
   /**
```

### Comparing `dune-common-2.9.0rc1/dune/common/poolallocator.hh` & `dune-common-2.9.dev20220529/dune/common/poolallocator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_POOLALLOCATOR_HH
 #define DUNE_COMMON_POOLALLOCATOR_HH
 
 /** \file
  * \brief An stl-compliant pool allocator
  */
 
@@ -423,15 +421,15 @@
   }
 
   template<class T, std::size_t S>
   inline Pool<T,S>::Pool()
     : head_(0), chunks_(0) //, allocated_(0)
   {
     static_assert(sizeof(T)<=unionSize, "Library Error: type T is too big");
-    static_assert(sizeof(Reference)<=unionSize, "Library Error: type of reference is too big");
+    static_assert(sizeof(Reference)<=unionSize, "Library Error: type of referene is too big");
     static_assert(unionSize<=alignedSize, "Library Error: alignedSize too small");
     static_assert(sizeof(T)<=chunkSize, "Library Error: chunkSize must be able to hold at least one value");
     static_assert(sizeof(Reference)<=chunkSize, "Library Error: chunkSize must be able to hold at least one reference");
     static_assert(chunkSize % alignment == 0, "Library Error: compiler cannot calculate!");
     static_assert(elements>=1, "Library Error: we need to hold at least one element!");
     static_assert(elements*alignedSize<=chunkSize, "Library Error: aligned elements must fit into chuck!");
   }
```

### Comparing `dune-common-2.9.0rc1/dune/common/power.hh` & `dune-common-2.9.dev20220529/dune/common/power.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_POWER_HH
 #define DUNE_COMMON_POWER_HH
 
 #warning The header power.hh is deprecated. Use power from math.hh instead.
 
 /** \file
     \brief Various implementations of the power function for run-time and static arguments
```

### Comparing `dune-common-2.9.0rc1/dune/common/precision.hh` & `dune-common-2.9.dev20220529/dune/common/precision.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PRECISION_HH
 #define DUNE_PRECISION_HH
 
 /** \file
  * \brief Various precision settings for calculations with FieldMatrix and FieldVector
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/promotiontraits.hh` & `dune-common-2.9.dev20220529/dune/common/promotiontraits.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PROMOTIONTRAITS_HH
 #define DUNE_PROMOTIONTRAITS_HH
 
 #include <utility>
 
 namespace Dune {
   /**
```

### Comparing `dune-common-2.9.0rc1/dune/common/propertymap.hh` & `dune-common-2.9.dev20220529/dune/common/propertymap.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PROPERTYMAP_HH
 #define DUNE_PROPERTYMAP_HH
 
 #include <cstddef>
 #include <iterator>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/proxymemberaccess.hh` & `dune-common-2.9.dev20220529/dune/common/proxymemberaccess.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_PROXYMEMBERACCESS_HH
 #define DUNE_COMMON_PROXYMEMBERACCESS_HH
 
 /**
  * \file
  * \brief infrastructure for supporting operator->() on both references and proxies
  * \ingroup CxxUtilities
```

### Comparing `dune-common-2.9.0rc1/dune/common/quadmath.hh` & `dune-common-2.9.dev20220529/dune/common/quadmath.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_QUADMATH_HH
 #define DUNE_QUADMATH_HH
 
 #if HAVE_QUADMATH
 #include <quadmath.h>
 
 #include <cmath>
@@ -207,15 +205,15 @@
 #define DUNE_UNARY_FUNC(name,func)                                         \
     inline Float128 name(const Float128& u) noexcept                       \
     {                                                                      \
       return Float128{func (float128_t(u))};                               \
     }                                                                      \
     static_assert(true, "Require semicolon to unconfuse editors")
 
-    // like DUNE_UNARY_FUNC but with custom return type
+    // like DUNE_UNARY_FUNC but with cutom return type
 #define DUNE_CUSTOM_UNARY_FUNC(type,name,func)                             \
     inline type name(const Float128& u) noexcept                           \
     {                                                                      \
       return (type)(func (float128_t(u)));                                 \
     }                                                                      \
     static_assert(true, "Require semicolon to unconfuse editors")
```

### Comparing `dune-common-2.9.0rc1/dune/common/rangeutilities.hh` & `dune-common-2.9.dev20220529/dune/common/rangeutilities.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_RANGE_UTILITIES_HH
 #define DUNE_COMMON_RANGE_UTILITIES_HH
 
 #include <dune/common/typetraits.hh>
 #include <algorithm>
 #include <utility>
 #include <type_traits>
@@ -782,15 +780,15 @@
    * the wrapped range. When dereferencing the iterator,
    * the given transformation function is applied to the wrapped
    * iterator on-the-fly and the result is returned.
    * I.e, if \code it \endcode is the wrapped iterator
    * and \code f \endcode is the transformation function,
    * then the result of \code f(it) \endcode is returned.
    *
-   * The transformation may either return temporary values
+   * The transformation may either return temorary values
    * or l-value references. In the former case the range behaves
    * like a proxy-container. In the latter case it forwards these
    * references allowing, e.g., to sort a subset of some container
    * by applying a transformation to an index-range for those values.
    *
    * The iterators of the TransformedRangeView have the same
    * iterator_category as the ones of the wrapped container.
```

### Comparing `dune-common-2.9.0rc1/dune/common/referencehelper.hh` & `dune-common-2.9.dev20220529/dune/common/referencehelper.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_REFERENCE_HELPER_HH
 #define DUNE_COMMON_REFERENCE_HELPER_HH
 
 #include <type_traits>
 #include <functional>
```

### Comparing `dune-common-2.9.0rc1/dune/common/scalarmatrixview.hh` & `dune-common-2.9.dev20220529/dune/common/scalarmatrixview.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SCALARMATRIXVIEW_HH
 #define DUNE_COMMON_SCALARMATRIXVIEW_HH
 
 #include <cstddef>
 #include <type_traits>
 #include <ostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/scalarvectorview.hh` & `dune-common-2.9.dev20220529/dune/common/scalarvectorview.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SCALARVECTORVIEW_HH
 #define DUNE_COMMON_SCALARVECTORVIEW_HH
 
 #include <cstddef>
 #include <type_traits>
 #include <istream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/shared_ptr.hh` & `dune-common-2.9.dev20220529/dune/common/shared_ptr.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_SHARED_PTR_HH
 #define DUNE_SHARED_PTR_HH
 
 #include <memory>
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/DESIGN.md` & `dune-common-2.9.dev20220529/dune/common/simd/DESIGN.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 This document is a collection of thoughts and rationals on a proper SIMD
 interface for Dune.
 
 What do we want?
 ================
 
 We want an abstraction layer for SIMD-libraries, that allows the core library
@@ -88,15 +83,15 @@
 
 Note 1: Short-circuiting may or may not happen for `&&` and `||` -- it will
 happen for the built-in types, but it cannot happen for proper multi-lane simd
 types.
 
 Note 2: For all expressions there is a lane-wise equality requirement with the
 scalar operation.  This requirement is formulated such that promotions of
-arguments are permitted, but not required.  This is necessary to allow both
+arguments are permitted, but not required.  This is neccessary to allow both
 the built-in types (which are promoted) and proper simd types (which typically
 are not promoted to stay within the same simd register).
 
 Note 3: The `==` in the lane-wise equality requirement may be overloaded to
 account for proxies returned by `lane()`.
 
 Note 4: Any expression that is invalid for the scalar case is not required for
@@ -110,15 +105,15 @@
 of the built-in scalar types.  Any code that only makes use of the abstraction
 layer needs to include this header, and only this header.
 
 Any compilation unit (generally a `.cc`-file) that creates vectorized types
 (other then the scalar built-in types) using some vectorization library, and
 hands those types to vectorization-enabled dune code, is responsible for
 
-1. including the necessary headers providing the abstraction for that
+1. including the neccessary headers providing the abstraction for that
    vectorization library, as specified in the documentation of the
    abstraction, and
 
 2. making sure the compilation with all the compiler/linker settings (flags,
    defines, libraries) needed by the vectorization library.
 
 The ADL-Problem
@@ -155,15 +150,15 @@
 ```
 
 This can then be used like this:
 
 ```c++
 #include <dune/common/foovector.hh>
 // provide dune-abstraction for mysimdlib
-// also pulls in the necessary includes for mysimdlib
+// also pulls in the neccessary includes for mysimdlib
 #include <dune/common/simd/mysimdlib.hh>
 
 int main()
 {
   using T = mysimdlib::Vector;
   Dune::FooVector<T> x(T(0));
   x.two_norm2();
@@ -242,15 +237,15 @@
   x.two_norm2();
 }
 ```
 
 At the time when the definition of `Dune::FooVector::two_norm2()` is read,
 only the declarations for `lane()` and `lanes()` for scalar built-in types are
 visible.  By the time `Dune::FooVector<mysimdlib::Vector>::two_norm2()` is
-instantiated, the proper declarations for `lane()` and `lanes()` are visible.
+instanciated, the proper declarations for `lane()` and `lanes()` are visible.
 But that is too late, because unqualified lookup does early binding.  It would
 be OK for late binding, but only ADL does that, and ADL does not work as noted
 above.
 
 Note that ADL is the _only_ type of lookup that does late binding.  So we
 cannot simply require the user to use another type of lookup.
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/base.hh` & `dune-common-2.9.dev20220529/dune/common/simd/base.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_BASE_HH
 #define DUNE_COMMON_SIMD_BASE_HH
 
 /** @file
  *  @brief Basic definitions for SIMD Implementations
  *  @ingroup SIMDAbstract
  *
  * This file provides basic definitions and template declarations that are
- * used to write SIMD abstraction layers.
+ * used to write SIMD abtraction layers.
  *
  * This file should never be included by users of the SIMD
  * abstraction. Include <dune/common/simd/simd.hh> instead.
  */
 
 /** @defgroup SIMD Vectorization
  * @ingroup Common
@@ -27,15 +25,15 @@
  *   have the knowledge which library abstraction is needed and are
  *   responsible for including that, as well as making sure the correct
  *   compiler flags are provided.
  *
  * - Library developers implement support in Dune for handling SIMD types,
  *   e.g. by extending some existing class.  By using the interfaces provided
  *   here, they should not have to worry about the exact vectorization library
- *   being used, or whether a vectorization library is used at all.
+ *   beeing used, or whether a vectorization library is used at all.
  *
  * - Abstraction developers provide the necessary hooks to make a
  *   vectorization library known to this interface.  They are also responsible
  *   for documenting for application developers how to meet the prerequisites
  *   for using the abstraction, e.g. which headers to include and how to add
  *   the necessary compiler flags.
  */
@@ -154,15 +152,15 @@
        * - `i==5,6`: these should normally be used by other implementations
        *
        * The lower priority should be used by default.  The higher priority
        * can be used by an implementation to resolve ambiguities, e.g. between
        * an overload with a by-value argument and an overload with an
        * lvalue-reference argument.
        *
-       * The following priorities should not normally be used.  However, they
+       * The folloing priorities should not normally be used.  However, they
        * may sometimes be necessary:
        * - \c i==4: override standard implementation, but prefer other
        *   implementations
        * - \c i==7: try to override other implementations
        *
        * \c i==7 is the highest supported priority.
        *
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/defaults.hh` & `dune-common-2.9.dev20220529/dune/common/simd/defaults.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_DEFAULTS_HH
 #define DUNE_COMMON_SIMD_DEFAULTS_HH
 
 /** @file
  *  @brief Default implementations for SIMD Implementations
  *  @ingroup SIMDAbstract
  *
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/interface.hh` & `dune-common-2.9.dev20220529/dune/common/simd/interface.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_INTERFACE_HH
 #define DUNE_COMMON_SIMD_INTERFACE_HH
 
 /** @file
  *  @brief User interface of the SIMD abstraction
  *  @ingroup SIMDLib
  *
@@ -105,15 +103,15 @@
      * the result of any operation back to the expected type.  In the above
      * example, the assertion would need to be written as `assert(lane(l,
      * vresult) == static_cast<unsigned short>(-lane(l, varg)));`.  In
      * practice, this should only be a problem with operations on unsigned
      * types where the result may be "negative".  Most code in Dune will want
      * to operate on floating point types, where this is a non-issue.
      *
-     * (Of course, this is also a problem for code that operates on untrusted
+     * (Of couse, this is also a problem for code that operates on untrusted
      * input, but you should not be doing that with Dune anyway).
      *
      * Still, when writing code using the SIMD abstractions, you should be
      * aware that in the following snippet
      * \code
      * auto var1 = lane(0, -vec);
      * auto var2 = -lane(0, vec);
@@ -310,15 +308,15 @@
     //! Extract an element of a SIMD type
     /**
      * \param l Number of lane to extract
      * \param v SIMD object to extract from
      *
      * \return If `v` is a non-`const` lvalue, a reference
      *         `Scalar<decay_t<V>>&`, or a proxy object through which the
-     *         element of `v` may be modified.  Otherwise, `v` is a `const`
+     *         element of `v` may be modified.  Overwise, `v` is a `const`
      *         lvalue or an rvalue, and the result is a prvalue (a temporary)
      *         of type `Scalar<decay_t<V>>`.
      *
      * Implemented by `Overloads::lane()`.
      */
     template<class V>
     decltype(auto) lane(std::size_t l, V &&v)
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/io.hh` & `dune-common-2.9.dev20220529/dune/common/simd/io.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_IO_HH
 #define DUNE_COMMON_SIMD_IO_HH
 
 /** @file
  *  @brief IO interface of the SIMD abstraction
  *  @ingroup SIMDLib
  *
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/loop.hh` & `dune-common-2.9.dev20220529/dune/common/simd/loop.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_LOOP_HH
 #define DUNE_COMMON_SIMD_LOOP_HH
 
 #include <array>
 #include <cmath>
 #include <cstddef>
 #include <cstdlib>
@@ -11,36 +9,32 @@
 
 #include <dune/common/math.hh>
 #include <dune/common/simd/simd.hh>
 #include <dune/common/typetraits.hh>
 
 namespace Dune {
 
+#  pragma GCC diagnostic push
 
 /*
  * silence warnings from GCC about using integer operands on a bool
  * (when instantiated for T=bool)
  */
 #if __GNUC__ >= 7
-#  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wbool-operation"
 #  pragma GCC diagnostic ignored "-Wint-in-bool-context"
-#  define GCC_WARNING_DISABLED
 #endif
 
 /*
  * silence warnings from Clang about using bitwise operands on
  * a bool (when instantiated for T=bool)
  */
 #ifdef __clang__
-#if __has_warning("-Wbitwise-instead-of-logical")
 #  pragma clang diagnostic push
 #  pragma clang diagnostic ignored "-Wbitwise-instead-of-logical"
-#  define CLANG_WARNING_DISABLED
-#endif
 #endif
 
 /*
  * Introduce a simd pragma if OpenMP is available in standard version >= 4
  */
 #if _OPENMP >= 201307
   #define DUNE_PRAGMA_OMP_SIMD _Pragma("omp simd")
@@ -600,27 +594,23 @@
     template<class T, std::size_t S, std::size_t A>
     auto isFinite(const LoopSIMD<T,S,A> &v, PriorityTag<3>, ADLTag) {
       Simd::Mask<LoopSIMD<T,S,A>> out;
       for(auto l : range(S))
         out[l] = Dune::isFinite(v[l]);
       return out;
     }
-  } //namespace MathOverloads
+  } //namepace MathOverloads
 
   template<class T, std::size_t S, std::size_t A>
   struct IsNumber<LoopSIMD<T,S,A>> :
           public std::integral_constant<bool, IsNumber<T>::value>{
   };
 
-#ifdef CLANG_WARNING_DISABLED
+#ifdef __clang__
 #  pragma clang diagnostic pop
-#  undef CLANG_WARNING_DISABLED
 #endif
 
-#ifdef GCC_WARNING_DISABLED
 #  pragma GCC diagnostic pop
-#  undef GCC_WARNING_DISABLED
-#endif
 
 } //namespace Dune
 
 #endif
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/standard.hh` & `dune-common-2.9.dev20220529/dune/common/simd/standard.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_STANDARD_HH
 #define DUNE_COMMON_SIMD_STANDARD_HH
 
 /** @file
  *  @ingroup SIMDStandard
  *  @brief SIMD abstractions for the standard built-in types
  *
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/CMakeLists.txt` & `dune-common-2.9.dev20220529/dune/common/simd/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # We need to explicitly instantiate the tests for small groups of types --
 # else the compiler will eat excessive amounts of memory.  This way it seems
 # to stay below 1GByte (with g++ 4.9.2 -O0 -g on x86_64 GNU/Linux, looking at
 # standardtest).
 include(DuneInstance)
 
 set(TYPES
@@ -12,15 +9,15 @@
   short int long "long long"
   "unsigned short" unsigned "unsigned long" "unsigned long long"
   bool
   float double "long double"
   std::complex<float> std::complex<double> "std::complex<long double>"
   )
 
-# Generate files with instantiations, external declarations, and also the
+# Generate files with instanciations, external declarations, and also the
 # invocations in the test for each instance.
 dune_instance_begin(FILES looptest.hh looptest.cc)
 foreach(SCALAR IN LISTS TYPES)
   dune_instance_add(ID "${SCALAR}")
   foreach(POINT IN ITEMS
       Type
       BinaryOpsScalarVector BinaryOpsVectorScalar)
@@ -43,15 +40,15 @@
   char "unsigned char" "signed char"
   short int long "long long"
   "unsigned short" unsigned "unsigned long" "unsigned long long"
   bool
   float double "long double"
   std::complex<float> std::complex<double> "std::complex<long double>")
 
-# Generate files with instantiations, external declarations, and also the
+# Generate files with instanciations, external declarations, and also the
 # invocations in the test for each instance.
 dune_instance_begin(FILES standardtest.hh standardtest.cc)
 foreach(SCALAR IN LISTS TYPES)
   dune_instance_add(ID "${SCALAR}" FILES standardtest_vector.cc)
 endforeach()
 dune_instance_end()
 
@@ -63,15 +60,15 @@
 # no need to install standardtest.hh, used by standardtest*.cc only
 
 
 # as of Vc-1.3.2: Vc/common/simdarray.h:561: SimdArray<T, N> may only be used
 # with T = { double, float, int32_t, uint32_t, int16_t, uint16_t }
 set(VCTEST_TYPES std::int16_t std::uint16_t std::int32_t std::uint32_t float double)
 
-# Generate files with instantiations, external declarations, and also the
+# Generate files with instanciations, external declarations, and also the
 # invocations in the test for each instance.
 dune_instance_begin(FILES vcarraytest.hh vcarraytest.cc)
 foreach(SCALAR IN LISTS VCTEST_TYPES)
   dune_instance_add(ID "${SCALAR}")
   foreach(POINT IN ITEMS
       Type
       BinaryOpsScalarVector BinaryOpsVectorScalar
@@ -86,15 +83,15 @@
   SOURCES ${DUNE_INSTANCE_GENERATED}
   LINK_LIBRARIES dunecommon
   CMAKE_GUARD Vc_FOUND
 )
 add_dune_vc_flags(vcarraytest)
 # no need to install vcarraytest.hh, used by vctest*.cc only
 
-# Generate files with instantiations, external declarations, and also the
+# Generate files with instanciations, external declarations, and also the
 # invocations in the test for each instance.
 dune_instance_begin(FILES vcvectortest.hh vcvectortest.cc)
 foreach(SCALAR IN LISTS VCTEST_TYPES)
   dune_instance_add(ID "${SCALAR}")
   foreach(POINT IN ITEMS
       Type
       BinaryOpsScalarVector BinaryOpsVectorScalar
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/looptest.cc.in` & `dune-common-2.9.dev20220529/dune/common/simd/test/looptest.cc.in`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdlib>
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/standardtest.cc.in` & `dune-common-2.9.dev20220529/dune/common/simd/test/standardtest.cc.in`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdlib>
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/standardtest.hh.in` & `dune-common-2.9.dev20220529/dune/common/simd/test/vcvectortest.hh.in`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
-#ifndef DUNE_COMMON_SIMD_TEST_STANDARDTEST_HH
-#define DUNE_COMMON_SIMD_TEST_STANDARDTEST_HH
+#ifndef DUNE_COMMON_SIMD_TEST_VCTEST_HH
+#define DUNE_COMMON_SIMD_TEST_VCTEST_HH
 
-#include <complex> // for substituted types
+#if HAVE_VC
+
+#include <cstdint>
 
 #include <dune/common/simd/test.hh>
+#include <dune/common/simd/vc.hh>
+#include <dune/common/typelist.hh>
 
 namespace Dune {
   namespace Simd {
 
-#cmake @template@
-    extern template void UnitTest::checkType<@SCALAR@>();
+#cmake @template POINT@
+    extern template void UnitTest::check@POINT@<Vc::Vector<@SCALAR@> >();
+    extern template void UnitTest::check@POINT@<Vc::Mask<@SCALAR@> >();
 #cmake @endtemplate@
 
   } // namespace Simd
 } // namespace Dune
 
-#endif // DUNE_COMMON_SIMD_TEST_STANDARDTEST_HH
+#endif // HAVE_VC
+#endif // DUNE_COMMON_SIMD_TEST_VCTEST_HH
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/vcarraytest.cc.in` & `dune-common-2.9.dev20220529/dune/common/simd/test/vcarraytest.cc.in`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #if !HAVE_VC
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test/vcvectortest.cc.in` & `dune-common-2.9.dev20220529/dune/common/simd/test/vcvectortest.cc.in`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #if !HAVE_VC
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/test.hh` & `dune-common-2.9.dev20220529/dune/common/simd/test.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_TEST_HH
 #define DUNE_COMMON_SIMD_TEST_HH
 
 /** @file
  *  @brief Common tests for simd abstraction implementations
  *
  * This file is an interface header and may be included without restrictions.
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd/vc.hh` & `dune-common-2.9.dev20220529/dune/common/simd/vc.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_VC_HH
 #define DUNE_COMMON_SIMD_VC_HH
 
 /** @file
  *  @ingroup SIMDVc
  *  @brief SIMD abstractions for Vc
  */
@@ -33,15 +31,15 @@
  *   the include in `#if HAVE_VC` and `#endif`
  *
  * - If you write a unit test, in your `CMakeLists.txt` use
  *   `dune_add_test(... CMAKE_GUARD Vc_FOUND)`
  *
  * You also need to make sure that the compiler uses the correct flags and
  * that the linker can find the library.  (The compilation flags include one
- * that ensures a name mangling scheme that can distinguish the
+ * that ensures a name mangling scheme that can distiguish the
  * compiler-intrinsic vector types from non-vector types is used.)
  *
  * - Either use `add_dune_vc_flags(your_application)` in `CMakeLists.txt`,
  *
  * - or use `dune_enable_all_packages()` in your module's toplevel
  *   `CMakeLists.txt`.
  *
@@ -201,15 +199,15 @@
         static_assert(std::is_same<V, std::decay_t<V> >::value, "Class Proxy "
                       "may only be instantiated with unqualified types");
       public:
         using value_type = typename V::value_type;
 
       private:
         static_assert(std::is_arithmetic<value_type>::value,
-                      "Only arithmetic types are supported");
+                      "Only artihmetic types are supported");
         V &vec_;
         std::size_t idx_;
 
       public:
         Proxy(std::size_t idx, V &vec)
           : vec_(vec), idx_(idx)
         { }
@@ -308,26 +306,26 @@
         //        friend auto operator@(MyClass, T);
         //      }
         //
         // This allows either for an exact match (in the case of option 1.) or
         // for conversions to be applied to the foreign argument (options 2.).
         // In contrast, allowing some of the template parameters being deduced
         // from the self argument also being deduced from the foreign argument
-        // will likely lead to ambiguous deduction when the foreign argument is
+        // will likely lead to ambigous deduction when the foreign argument is
         // a proxy:
         //   template<class T, class... Args>
         //   auto operator@(MyClass<T, Args...>, T);
-        // One class that suffers from this problem is std::complex.
+        // One class that suffers from this problem ist std::complex.
         //
         // Note that option 1. is a bit dangerous, as the foreign argument is
         // catch-all.  This seems tempting in the case of a proxy class, as
         // the operator could just be forwarded to the proxied object with the
         // foreign argument unchanged, immediately creating interoperability
         // with arbitrary foreign classes.  However, if the foreign class also
-        // choses option 1., this will result in ambiguous overloads, and there
+        // choses option 1., this will result in ambigous overloads, and there
         // is no clear guide to decide which class should provide the overload
         // and which should not.
         //
         // Fortunately, deferring to the conversion and the built-in operators
         // mostly works in the case of this proxy class, because only built-in
         // types can be proxied anyway.  Unfortunately, the Vc vectors and
         // arrays suffer from a slightly different problem.  They chose option
@@ -336,15 +334,15 @@
         // intrinsics.  So they check the argument whether it is one of the
         // expected types, and remove the operator from the overload set if it
         // isn't via SFINAE.  Of course, this proxy class is not one of the
         // expected types, even though it would convert to them...
         //
         // So what we have to do here, unfortunately, is to provide operators
         // for the Vc types explicitly, and hope that there won't be some Vc
-        // version that gets the operators right, thus creating ambiguous
+        // version that gets the operators right, thus creating ambigous
         // overloads.  Well, if guess it will be #ifdef time if it comes to
         // that.
 #define DUNE_SIMD_VC_BINARY(OP)                                         \
         template<class T, class Abi>                                    \
         friend auto operator OP(const Vc::Vector<T, Abi> &l, Proxy&& r) \
           -> decltype(l OP std::declval<value_type>())                  \
         {                                                               \
```

### Comparing `dune-common-2.9.0rc1/dune/common/simd.hh` & `dune-common-2.9.dev20220529/dune/common/simd.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_SIMD_HH
 #define DUNE_COMMON_SIMD_HH
 
 #warning dune/common/simd.hh is deprecated.
 #warning Use the new infrastructure from dune/common/simd/simd.h instead.
 
 /**
@@ -64,15 +62,15 @@
       static_assert(std::is_same<V, std::decay_t<V> >::value, "Class Proxy "
                     "may only be instantiated with unqualified types");
     public:
       using value_type = typename V::value_type;
 
     private:
       static_assert(std::is_arithmetic<value_type>::value,
-                    "Only arithmetic types are supported");
+                    "Only artihmetic types are supported");
       V &vec_;
       std::size_t idx_;
 
     public:
       Proxy(std::size_t idx, V &vec)
         : vec_(vec), idx_(idx)
       { }
```

### Comparing `dune-common-2.9.0rc1/dune/common/singleton.hh` & `dune-common-2.9.dev20220529/dune/common/singleton.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_SINGLETON_HH
 #define DUNE_SINGLETON_HH
 
 #include <dune/common/visibility.hh>
 
 /**
  * @file
```

### Comparing `dune-common-2.9.0rc1/dune/common/sllist.hh` & `dune-common-2.9.dev20220529/dune/common/sllist.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_SLLIST_HH
 #define DUNE_SLLIST_HH
 
 #include <memory>
 #include <cassert>
 #include "iteratorfacades.hh"
 #include <ostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/std/make_array.hh` & `dune-common-2.9.dev20220529/dune/common/std/make_array.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_STD_MAKE_ARRAY_HH
 #define DUNE_COMMON_STD_MAKE_ARRAY_HH
 
 #include <array>
 #include <type_traits>
 
 #if DUNE_HAVE_CXX_EXPERIMENTAL_MAKE_ARRAY
```

### Comparing `dune-common-2.9.0rc1/dune/common/std/type_traits.hh` & `dune-common-2.9.dev20220529/dune/common/std/type_traits.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_STD_TYPE_TRAITS_HH
 #define DUNE_COMMON_STD_TYPE_TRAITS_HH
 
 #include <type_traits>
 #include <dune/common/typetraits.hh>
 #include <dune/common/typeutilities.hh>
 
@@ -239,15 +237,15 @@
    * \brief forms the logical conjunction of the type traits B...
    *
    * \note This functionality is part of the C++17 standard.
    *
    * \ingroup CxxUtilities
    **/
   template< class... B >
-  struct [[deprecated("Will be removed after release 2.8. Use std::conjunction instead.")]] conjunction
+  struct [[deprecated("Will be removed after release 2.8. Use std::conjuction instead.")]] conjunction
     : std::conjunction<B...>
   {};
 
 
   // disjunction
   // -----------
 
@@ -277,29 +275,10 @@
   template<class B>
   struct [[deprecated("Will be removed after release 2.8. Use std::negation instead.")]] negation
     : std::negation<B>
   {};
 
 } // namespace Std
 
-
-namespace detail
-{
-  template <class Type>
-  [[deprecated("Type extraction of `TargetType` has failed. Inspect the code calling `detected_or_fallback_t` for getting the source of this warning!")]]
-  Type warningIfNotDefined(const Std::nonesuch*);
-
-  template <class Type, class T>
-  Type warningIfNotDefined(const T*);
-}
-
-//! This type will be either TargetType<Args...> if it exists, or the Fallback<Args...> type.
-template <template<typename...> class Fallback,
-          template<typename...> class TargetType, typename... Args>
-using detected_or_fallback_t = Std::detected_or_t<decltype(
-  detail::warningIfNotDefined<Std::detected_t<Fallback, Args...> >(std::declval<const Std::detected_t<TargetType, Args...>*>())),
-  TargetType, Args...>;
-
-
 } // namespace Dune
 
 #endif // #ifndef DUNE_COMMON_STD_TYPE_TRAITS_HH
```

### Comparing `dune-common-2.9.0rc1/dune/common/stdstreams.cc` & `dune-common-2.9.dev20220529/dune/common/stdstreams.cc`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include "stdstreams.hh"
```

### Comparing `dune-common-2.9.0rc1/dune/common/stdstreams.hh` & `dune-common-2.9.dev20220529/dune/common/stdstreams.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /**
    \file
    \brief Standard Dune debug streams
 
    The standard debug streams are compiled into libdune to exist
    globally. This file declares the stream types and the global debug
```

### Comparing `dune-common-2.9.0rc1/dune/common/stdthread.cc` & `dune-common-2.9.dev20220529/dune/common/stdthread.cc`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #include <cstdlib>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/stdthread.hh` & `dune-common-2.9.dev20220529/dune/common/stdthread.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_STDTHREAD_HH
 #define DUNE_COMMON_STDTHREAD_HH
 
 namespace Dune
 {
```

### Comparing `dune-common-2.9.0rc1/dune/common/streamoperators.hh` & `dune-common-2.9.dev20220529/dune/common/streamoperators.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_STREAMOPERATORS_HH
 #define DUNE_STREAMOPERATORS_HH
 
 /** \file
     \brief Implementation of stream operators for std::array and std::tuple
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/stringutility.hh` & `dune-common-2.9.dev20220529/dune/common/stringutility.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_STRINGUTILITY_HH
 #define DUNE_COMMON_STRINGUTILITY_HH
 
 /** \file
     \brief Miscellaneous helper stuff
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/CMakeLists.txt` & `dune-common-2.9.dev20220529/dune/common/test/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 include(DuneInstance)
 
 dune_add_test(SOURCES arithmetictestsuitetest.cc
               LINK_LIBRARIES dunecommon
               LABELS quick)
 
 dune_add_test(SOURCES arraylisttest.cc
@@ -89,15 +86,15 @@
               LINK_LIBRARIES dunecommon
               LABELS quick)
 
 dune_add_test(SOURCES debugaligntest.cc
               LINK_LIBRARIES dunecommon
               LABELS quick)
 
-# Generate files with instantiations, external declarations, and also the
+# Generate files with instanciations, external declarations, and also the
 # invocations in the test for each instance.
 dune_instance_begin(FILES debugalignsimdtest.hh debugalignsimdtest.cc)
 foreach(SCALAR IN ITEMS double bool)
   dune_instance_add(ID "${SCALAR}")
   foreach(POINT IN ITEMS Type BinaryOpsScalarVector BinaryOpsVectorScalar)
     dune_instance_add(TEMPLATE POINT
                       ID "${POINT}_${SCALAR}"
@@ -326,18 +323,14 @@
 dune_add_test(SOURCES stdidentity.cc
               LABELS quick)
 
 dune_add_test(SOURCES stdapplytest.cc
               LINK_LIBRARIES dunecommon
               LABELS quick)
 
-dune_add_test(SOURCES stdchecktypes.cc
-              LINK_LIBRARIES dunecommon
-              LABELS quick)
-
 dune_add_test(SOURCES streamoperatorstest.cc
               LABELS quick)
 
 dune_add_test(SOURCES streamtest.cc
               LINK_LIBRARIES dunecommon
               LABELS quick)
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/alignedallocatortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/alignedallocatortest.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <cstdint>
 #include <tuple>
 #include <vector>
 
 #include <dune/common/alignedallocator.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/arithmetictestsuite.hh` & `dune-common-2.9.dev20220529/dune/common/test/arithmetictestsuite.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TEST_ARITHMETICTESTSUITE_HH
 #define DUNE_COMMON_TEST_ARITHMETICTESTSUITE_HH
 
 #include <string>
 #include <type_traits>
 #include <utility>
 
@@ -18,25 +16,14 @@
  * silence warnings from GCC about using integer operands on a bool
  * (when instantiated for T=bool)
  */
 #if __GNUC__ >= 7
 #  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wbool-operation"
 #  pragma GCC diagnostic ignored "-Wint-in-bool-context"
-#  define GCC_WARNING_DISABLED
-#endif
-
-/*
- * silence warnings from Clang about using bitwise operands on
- * a bool (when instantiated for T=bool)
- */
-#ifdef __clang__
-#  pragma clang diagnostic push
-#  pragma clang diagnostic ignored "-Wbool-operation"
-#  define CLANG_WARNING_DISABLED
 #endif
 
   //! Test suite for arithmetic types
   /**
    * You usually want to call the member function `checkArithmetic()`.  The
    * individual component tests are however available for special needs.
    */
@@ -800,20 +787,14 @@
 
       checkAssignBitAnd<T>(arithmetic_tag);
       checkAssignBitXor<T>(arithmetic_tag);
       checkAssignBitOr<T>(arithmetic_tag);
     }
   };
 
-#ifdef CLANG_WARNING_DISABLED
-#  pragma clang diagnostic pop
-#  undef CLANG_WARNING_DISABLED
-#endif
-
-#ifdef GCC_WARNING_DISABLED
+#if __GNUC__ >= 7
 #  pragma GCC diagnostic pop
-#  undef GCC_WARNING_DISABLED
 #endif
 
 } // namespace Dune
 
 #endif // DUNE_COMMON_TEST_ARITHMETICTESTSUITE_HH
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/arithmetictestsuitetest.cc` & `dune-common-2.9.dev20220529/dune/common/test/arithmetictestsuitetest.cc`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <tuple>
 
 #include <dune/common/hybridutilities.hh>
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/test/arithmetictestsuite.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/arraylisttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/arraylisttest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/arraylist.hh>
 #include <dune/common/test/iteratortest.hh>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/assertandreturntest.cc` & `dune-common-2.9.dev20220529/dune/common/test/assertandreturntest.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #ifdef NDEBUG
     #undef NDEBUG
 #endif
 #ifdef TEST_NDEBUG
     #define NDEBUG TEST_NDEBUG
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/bigunsignedinttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/bigunsignedinttest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdint>
 #include <limits>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/bitsetvectortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/bitsetvectortest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/bitsetvector.hh>
 
 #if defined(__GNUC__) && ! defined(__clang__)
@@ -50,15 +48,15 @@
   const BBF & cbbf = bbf;
 
   bitset x = bbf[3];
   reference y = bbf[4];
   const_reference z = bbf[4];
   const reference v = bbf[4];
 
-  // assignment
+  // assignement
   y = false;
   y[2] = true;
   y = x;
   y = z;
   y = v;
   x = y;
   x = z;
@@ -142,15 +140,15 @@
 
   const BBF & cbbf = bbf;
 
   bitset x = bbf[3];
   [[maybe_unused]] value_type z;
   reference y = bbf[4];
 
-  // assignment
+  // assignement
   x = y;
   x = cbbf[1];
 
   // equality
   [[maybe_unused]] bool res;
   res = (y == cbbf[2]);
   res = (y == bbf[3]);
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/boundscheckingmvtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/boundscheckingmvtest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
 #include <dune/common/dynmatrix.hh>
 
 int main() try {
   bool passed = true;
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/boundscheckingoptest.cc` & `dune-common-2.9.dev20220529/dune/common/test/boundscheckingoptest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
 
 int main() try {
   bool passed = true;
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/boundscheckingtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/boundscheckingtest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <dune/common/bitsetvector.hh>
 #include <dune/common/diagonalmatrix.hh>
 #include <dune/common/dynvector.hh>
 #include <dune/common/dynmatrix.hh>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/checkmatrixinterface.hh` & `dune-common-2.9.dev20220529/dune/common/test/checkmatrixinterface.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_CHECK_MATRIX_INTERFACE_HH
 #define DUNE_COMMON_CHECK_MATRIX_INTERFACE_HH
 
 #include <algorithm>
 #include <limits>
 
 #include <dune/common/dynvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/classnametest.cc` & `dune-common-2.9.dev20220529/dune/common/test/classnametest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <bitset>
 #include <complex>
 #include <iostream>
 #include <regex>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/collectorstream.hh` & `dune-common-2.9.dev20220529/dune/common/test/collectorstream.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TEST_COLLECTORSTREAM_HH
 #define DUNE_COMMON_TEST_COLLECTORSTREAM_HH
 
 #include <sstream>
 #include <string>
 #include <functional>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/concept.cc` & `dune-common-2.9.dev20220529/dune/common/test/concept.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/typelist.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/debugalignsimdtest.cc.in` & `dune-common-2.9.dev20220529/dune/common/test/debugalignsimdtest.cc.in`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // @GENERATED_SOURCE@
 
 #include <config.h>
 
 #include <cstdlib>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/debugaligntest.cc` & `dune-common-2.9.dev20220529/dune/common/test/debugaligntest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <cstdint>
 #include <new>
 #include <tuple>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/densematrixassignmenttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/densematrixassignmenttest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #define DUNE_CHECK_BOUNDS
 
 #include <complex>
 
 #include <dune/common/boundschecking.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/densevectorassignmenttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/densevectorassignmenttest.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <iostream>
 
 #include <dune/common/densevector.hh>
 #include <dune/common/dynvector.hh>
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/densevectortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/densevectortest.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <algorithm>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/diagonalmatrixtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/diagonalmatrixtest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #ifndef DUNE_FMatrix_WITH_CHECKING
 #define DUNE_FMatrix_WITH_CHECKING
 #endif
@@ -59,19 +57,14 @@
   std::cout << f << std::endl;
 
   // assign to FieldMatrix
   [[maybe_unused]] FieldMatrix<K,n,n> AFM = FieldMatrix<K,n,n>(A);
   [[maybe_unused]] FieldMatrix<K,n,n> AFM2 = A;
   [[maybe_unused]] FieldMatrix<K,n,n> AFM3;
   AFM3 = A;
-
-  // test transposed
-  DiagonalMatrix<K,n> AT = A.transposed();
-  if (AT != A)
-    DUNE_THROW(FMatrixError, "Return value of DiagoalMatrix::transposed() incorrect!");
 }
 
 template<class K, int n>
 void test_interface()
 {
   typedef CheckMatrixInterface::UseFieldVector<K,n,n> Traits;
   typedef Dune::DiagonalMatrix<K,n> DiagonalMatrix;
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/dynmatrixtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/dynmatrixtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 // Activate checking
 #ifndef DUNE_FMatrix_WITH_CHECKING
 #define DUNE_FMatrix_WITH_CHECKING
 #endif
@@ -290,22 +288,14 @@
   std::sort(v.begin(), v.end());
 
   // print matrix
   std::cout << A << std::endl;
   // print vector
   std::cout << f << std::endl;
 
-  // transposed(Matrix)
-  {
-    DynamicMatrix<K> AT = A.transposed();
-    for (size_type i=0; i<AT.N(); i++)
-      for (size_type j=0; j<AT.M(); j++)
-        if (AT[i][j] != A[j][i])
-          DUNE_THROW(FMatrixError, "Return value of matrix.transposed() incorrect!");
-  }
 
   {
     DynamicMatrix<K> A2 = A;
     A2 *= 2;
 
     DynamicMatrix<K> B = A;
     B += A;
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/dynvectortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/dynvectortest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 
 #include <dune/common/dynvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/eigenvaluestest.cc` & `dune-common-2.9.dev20220529/dune/common/test/eigenvaluestest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
 #include <dune/common/dynmatrixev.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/enumsettest.cc` & `dune-common-2.9.dev20220529/dune/common/test/enumsettest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/enumset.hh>
 #include <iostream>
 int main()
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/filledarraytest.cc` & `dune-common-2.9.dev20220529/dune/common/test/filledarraytest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <array>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/fmatrixtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/fmatrixtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 // Activate checking.
 #ifndef DUNE_FMatrix_WITH_CHECKING
 #define DUNE_FMatrix_WITH_CHECKING
@@ -479,26 +477,28 @@
       FM neg = -A;
       FM ref = typename FM::field_type(-1)*A;
 
       if ((neg-ref).infinity_norm() > 1e-12)
         DUNE_THROW(FMatrixError, "Return value of operator-(matrix) incorrect!");
     }
 
-    // transposed(Matrix)
+    // Matrix * Matrix
     {
-      FieldMatrix<typename FM::field_type,FM::cols,FM::rows> AT = A.transposed();
-      for (int i=0; i<AT.rows; i++)
-        for (int j=0; j<AT.cols; j++)
-          if (AT[i][j] != A[j][i])
-            DUNE_THROW(FMatrixError, "Return value of matrix.transposed() incorrect!");
-    }
+      auto transposed = [](const FM& A)
+      {
+        FieldMatrix<typename FM::field_type,FM::cols,FM::rows> AT;
+        for (int i=0; i<AT.rows; i++)
+          for (int j=0; j<AT.cols; j++)
+            AT[i][j] = A[j][i];
 
+        return AT;
+      };
 
-    // Matrix * Matrix
-    [[maybe_unused]] auto product = A.transposed() * A;
+      [[maybe_unused]] auto product = transposed(A) * A;
+    }
 
   }
   {
     using std::abs;
 
     FieldMatrix<K,n,m> A3 = A;
     A3 *= 3;
@@ -812,15 +812,15 @@
 {
   typedef CheckMatrixInterface::UseFieldVector< K2, rows, cols > Traits;
   typedef Dune::FieldMatrix< K, rows, cols > FMatrix;
 
 #if __GNUC__ != 5 || defined(__clang__)
   static_assert(
     !std::is_trivially_copyable<K>::value || std::is_trivially_copyable<FMatrix>::value,
-    "FieldMatrix<T, ...> must be trivially copyable type when T is trivial type"
+    "FieldMatrix<T, ...> must be trivally copyable type when T is trivial type"
     );
 #endif
   static_assert(
     std::is_standard_layout<FMatrix>::value,
     "FieldMatrix<...> must be a standard layout type"
     );
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/fvectorconversion1d.cc` & `dune-common-2.9.dev20220529/dune/common/test/fvectorconversion1d.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <algorithm>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/fvectortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/fvectortest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <complex>
 #include <iostream>
 #include <limits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/hybridutilitiestest.cc` & `dune-common-2.9.dev20220529/dune/common/test/hybridutilitiestest.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <tuple>
 #include <vector>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/indicestest.cc` & `dune-common-2.9.dev20220529/dune/common/test/indicestest.cc`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <tuple>
 
 #include <dune/common/indices.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/iscallabletest.cc` & `dune-common-2.9.dev20220529/dune/common/test/iscallabletest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/typetraits.hh>
 #include <dune/common/test/testsuite.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/iteratorfacadetest.cc` & `dune-common-2.9.dev20220529/dune/common/test/iteratorfacadetest.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/test/iteratorfacadetest.hh>
 #include <dune/common/test/iteratortest.hh>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/iteratorfacadetest.hh` & `dune-common-2.9.dev20220529/dune/common/test/iteratorfacadetest.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ITERATORFACADETEST_HH
 #define DUNE_ITERATORFACADETEST_HH
 #include <dune/common/iteratorfacades.hh>
 #include <dune/common/genericiterator.hh>
 #include <dune/common/typetraits.hh>
 
 template<class T,
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/iteratortest.hh` & `dune-common-2.9.dev20220529/dune/common/test/iteratortest.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_COMMON_TEST_ITERATORTEST_HH
 #define DUNE_COMMON_TEST_ITERATORTEST_HH
 #include <iostream>
 #include <algorithm>
 #include <dune/common/classname.hh>
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/mathclassifierstest.cc` & `dune-common-2.9.dev20220529/dune/common/test/mathclassifierstest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <complex>
 #include <iostream>
 #include <limits>
 
 #include <dune/common/math.hh>
 
 int main() {
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/mathtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/mathtest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/common/hybridutilities.hh>
 #include <dune/common/indices.hh>
 #include <dune/common/math.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/metistest.cc` & `dune-common-2.9.dev20220529/dune/common/test/metistest.cc`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <iostream>
 #include <vector>
 
 #if ! HAVE_METIS
 #error "METIS is required for this test"
 #endif
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/mpicollectivecommunication.cc` & `dune-common-2.9.dev20220529/dune/common/test/mpicollectivecommunication.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <array>
 
 #include <dune/common/parallel/mpihelper.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/mpicommunicationtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/mpicommunicationtest.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <array>
 
 #include <dune/common/parallel/mpihelper.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/mpiguardtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/mpiguardtest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/parallel/mpiguard.hh>
 
 int main(int argc, char** argv)
 {
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/overloadsettest.cc` & `dune-common-2.9.dev20220529/dune/common/test/overloadsettest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 
 #include <tuple>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/parameterizedobjectfactorysingleton.hh` & `dune-common-2.9.dev20220529/dune/common/test/parameterizedobjectfactorysingleton.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TEST_PARAMETERIZEDOBJECTFACTORYSINGLETON_HH
 #define DUNE_COMMON_TEST_PARAMETERIZEDOBJECTFACTORYSINGLETON_HH
 
 #include <dune/common/parameterizedobject.hh>
 #include <dune/common/singleton.hh>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/parameterizedobjecttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/parameterizedobjecttest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 #include <iostream>
 #include <cassert>
 #include <memory>
 #include <tuple>
 #include <dune/common/parametertree.hh>
 #include <dune/common/shared_ptr.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/parametertreelocaletest.cc` & `dune-common-2.9.dev20220529/dune/common/test/parametertreelocaletest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #include <cstdlib>
 #include <iostream>
 #include <locale>
@@ -41,15 +39,15 @@
     catch(...) {                                                \
       std::cerr << __FILE__ << ":" << __LINE__ << ": " << #expr \
                 << " should throw " << #except << std::endl;    \
       std::abort();                                             \
     }                                                           \
   } while(false)
 
-// globally set a locale that uses "," as the decimal separator.
+// globally set a locale that uses "," as the decimal seperator.
 // return false if no such locale is installed on the system
 bool setCommaLocale()
 {
   static char const* const commaLocales[] = {
     "de", "de@euro", "de.UTF-8",
     "de_AT", "de_AT@euro", "de_AT.UTF-8",
     "de_BE", "de_BE@euro", "de_BE.UTF-8",
@@ -80,15 +78,15 @@
   return false;
 }
 
 int main()
 {
   if(!setCommaLocale())
   {
-    std::cerr << "No locale using comma as decimal separator found on system"
+    std::cerr << "No locale using comma as decimal seperator found on system"
               << std::endl;
     return 77;
   }
   { // Try with comma
     Dune::ParameterTree ptree;
     check_throw((ptree["setting"] = "42,42",
                  ptree.get<double>("setting")),
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/parametertreetest.cc` & `dune-common-2.9.dev20220529/dune/common/test/parametertreetest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <array>
 #include <cstdlib>
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/parmetistest.cc` & `dune-common-2.9.dev20220529/dune/common/test/parmetistest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <cassert>
 #include <iostream>
 #include <vector>
 
 #if ! HAVE_PARMETIS
 #error "ParMETIS is required for this test."
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/pathtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/pathtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <ostream>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/poolallocatortest.cc` & `dune-common-2.9.dev20220529/dune/common/test/poolallocatortest.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstdint>
 #include <vector>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/powertest.cc` & `dune-common-2.9.dev20220529/dune/common/test/powertest.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/deprecated.hh>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/quadmathtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/quadmathtest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include "config.h"
 
 #include <cassert>
 #include <iostream>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/rangeutilitiestest.cc` & `dune-common-2.9.dev20220529/dune/common/test/rangeutilitiestest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <array>
 #include <map>
 #include <vector>
 #include <numeric>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/referencehelpertest.cc` & `dune-common-2.9.dev20220529/dune/common/test/referencehelpertest.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <functional>
 
 #include <dune/common/parallel/mpihelper.hh>
 
 #include <dune/common/referencehelper.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/scotchtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/scotchtest.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
 
 #include <scotch.h>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/shared_ptrtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/shared_ptrtest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 // make sure assert works even when not compiling for debugging
 #ifdef NDEBUG
 #undef NDEBUG
 #endif
 
 #ifdef HAVE_CONFIG_H
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/singletontest.cc` & `dune-common-2.9.dev20220529/dune/common/test/singletontest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/singleton.hh>
 #include <iostream>
 class Foo : public Dune::Singleton<Foo>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/sllisttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/sllisttest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/common/sllist.hh>
 #include <dune/common/test/iteratortest.hh>
 #include <dune/common/poolallocator.hh>
@@ -78,15 +76,15 @@
 template<typename T,class A>
 int check(const Dune::SLList<T,A>& alist, const T* vals)
 {
   typedef typename Dune::SLList<T,A>::const_iterator iterator;
   int i=0;
   for(iterator iter = alist.begin(); iter != alist.end(); ++iter, i++) {
     if( vals[i] != *iter ) {
-      std::cerr<<" List mismatch! "<<__FILE__<<":"<<__LINE__<<std::endl;
+      std::cerr<<" List missmatch! "<<__FILE__<<":"<<__LINE__<<std::endl;
       return 1;
     }
   }
   return 0;
 }
 
 
@@ -137,15 +135,15 @@
 
   blist.push_back(-1);
 
   blist=alist;
   List::iterator biter=blist.begin(), aiter=alist.begin();
   for(; aiter!=alist.end(); ++aiter, ++biter)
     if(*aiter!=*biter) {
-      std::cerr<<"Assignment failed "<<__FILE__<<":"<<__LINE__<<std::endl;
+      std::cerr<<"Asignment failed "<<__FILE__<<":"<<__LINE__<<std::endl;
       return 1;
     }
   return 0;
 }
 
 int testDelete()
 {
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/stdapplytest.cc` & `dune-common-2.9.dev20220529/dune/common/test/stdapplytest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <tuple>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/stdidentity.cc` & `dune-common-2.9.dev20220529/dune/common/test/stdidentity.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 #include <dune/common/std/functional.hh>
 #include <iostream>
 #include <cassert>
 
 struct Foo {
   static int count;
   Foo() { ++count; std::cout << "construct" << std::endl; }
   Foo(const Foo&) { ++count; std::cout << "copy construct" << std::endl; }
   Foo(Foo&&) { ++count; std::cout << "move construct" << std::endl; }
-  ~Foo() { --count; std::cout << "destruct" << std::endl; }
+  ~Foo() { --count; std::cout << "deconstruct" << std::endl; }
 };
 int Foo::count = 0;
 
 template<typename T>
 T&& assert_count(T&& arg, int count)
 {
   std::cout << std::decay_t<T>::count << std::endl;
@@ -31,18 +29,18 @@
 int main()
 {
   auto id = Dune::Std::identity();
 
   assert_count(id(Foo()),1); // pass an r-value to identity, still constructed on the assert
 
   const auto& foo0 = id(Foo()); // pass an r-value to identity
-  assert_count(foo0,0); // id(Foo()) is already destructed at this point
+  assert_count(foo0,0); // id(Foo()) is alredy doconstructed at this point
 
   auto foo1 = id(Foo()); // pass an r-value to identity and move it to foo1
-  assert_count(foo1,1); // foo0 is already destructed at this point
+  assert_count(foo1,1); // foo0 is alredy doconstructed at this point
 
   Foo foo2;
   assert_count(id(foo2),2); // pass an l-value to identity
 
   const auto& foo3 = id(foo2); // pass an l-value to identity
   assert_count(foo3,2); // foo still exist at this point
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/streamoperatorstest.cc` & `dune-common-2.9.dev20220529/dune/common/test/streamoperatorstest.cc`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <sstream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/streamtest.cc` & `dune-common-2.9.dev20220529/dune/common/test/streamtest.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /*
 
    Test to check if the standard streams in libdune can be properly
    linked with this program and if they work
 
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/testdebugallocator.cc` & `dune-common-2.9.dev20220529/dune/common/test/testdebugallocator.cc`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 // #define DEBUG_ALLOCATOR_KEEP 1
 #define DEBUG_NEW_DELETE 3
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/testfloatcmp.cc` & `dune-common-2.9.dev20220529/dune/common/test/testfloatcmp.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // Test the new (Dune) interface of float_cmp
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/testsuite.hh` & `dune-common-2.9.dev20220529/dune/common/test/testsuite.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TEST_TESTSUITE_HH
 #define DUNE_COMMON_TEST_TESTSUITE_HH
 
 #include <iostream>
 #include <sstream>
 #include <string>
 
@@ -63,15 +61,15 @@
     {}
 
     /**
      * \brief Check condition
      *
      * This will throw an exception if the check fails and if the AlwaysThrow policy was used on creation.
      *
-     * \param condition Checks if this is true and increases the failure counter if not.
+     * \param conditon Checks if this is true and increases the failure counter if not.
      * \param name A name to identify this check. Defaults to ""
      * \returns A CollectorStream that can be used to create a diagnostic message to be printed on failure.
      */
     CollectorStream check(bool condition, std::string name="")
     {
       ++checks_;
       if (not condition)
@@ -84,15 +82,15 @@
     }
 
     /**
      * \brief Check a required condition
      *
      * This will always throw an exception if the check fails.
      *
-     * \param condition Checks if this is true and increases the failure counter if not.
+     * \param conditon Checks if this is true and increases the failure counter if not.
      * \param name A name to identify this check. Defaults to ""
      * \returns A CollectorStream that can be used to create a diagnostic message to be printed on failure.
      */
     CollectorStream require(bool condition, std::string name="")
     {
       ++checks_;
       if (not condition)
@@ -151,15 +149,15 @@
         std::cout << composeMessage("TEST   ", name(), std::to_string(failedChecks_)+"/"+std::to_string(checks_) + " checks failed in this test.") << std::endl;
       return (failedChecks_==0);
     }
 
     /**
      * \brief Exit the test.
      *
-     * This will print a summary of the test and return an integer
+     * This wil print a summary of the test and return an integer
      * to be used on program exit.
      *
      * \returns 1 if any of the executed tests failed, otherwise 0.
      */
     int exit() const
     {
       return (report() ? 0: 1);
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/timing.cc` & `dune-common-2.9.dev20220529/dune/common/test/timing.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <fstream>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/tupleutilitytest.cc` & `dune-common-2.9.dev20220529/dune/common/test/tupleutilitytest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cmath>
 #include <cstddef>
@@ -68,15 +66,15 @@
 static_assert((std::is_same<MyTupleTupleFlat1, MyTupleTupleFlat2>::value),
               "FlattenTuples failed!");
 
 
 
 //////////////////////////////////////////////////////////////////////
 //
-// check nested ReduceTuple with a little TMP
+// check nested ReduceTuple with a litte TMP
 
 // A tuple of a range of integers wrapped in integral_constant types
 template<int start, int end>
 struct Range
 {
   typedef typename Dune::PushBackTuple<
       typename Range<start, end-1>::type,
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/typelisttest.cc` & `dune-common-2.9.dev20220529/dune/common/test/typelisttest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <tuple>
 #include <type_traits>
@@ -59,17 +57,17 @@
   tl4 = { std::move(tl2) };
 
   // check literal type requirement
   constexpr TL tl7{};
 
   // specialization/overload resolution tests
   static_assert(IsTypeListBySpecialization<TL>::value,
-                "TypeList cannot be recognized by class specialization");
+                "TypeList cannot be recongized by class specialization");
   static_assert(IsTypeListByOverload<TL>::value,
-                "TypeList cannot be recognized by function overload resolution");
+                "TypeList cannot be recongized by function overload resolution");
 
   // avoid compiler warnings
   (void)tl1;
   (void)tl2;
   (void)tl3;
   (void)tl4;
   (void)tl5;
@@ -88,25 +86,25 @@
   static_assert(!Dune::IsTypeList<T>::value,
                 "IsTypeList accepts non-TypeList");
   static_assert(!Dune::IsEmptyTypeList<T>::value,
                 "IsEmptyTypeList accepts non-TypeList");
 
   // specialization tests
   static_assert(!IsTypeListBySpecialization<T>::value,
-                "Non-TypeList recognized as TypeList by class specialization");
+                "Non-TypeList recongized as TypeList by class specialization");
 }
 
 template<class T>
 void checkNonTypeList()
 {
   checkNonTypeList<T>(skipOverloadTest);
 
   // overload resolution tests
   static_assert(!IsTypeListByOverload<T>::value,
-                "Non-TypeList recognized as TypeList by function overload resolution");
+                "Non-TypeList recongized as TypeList by function overload resolution");
 }
 
 void staticTests()
 {
   {
     using TL = Dune::TypeList<>;
     static_assert(Dune::IsTypeList<TL>::value,
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/utilitytest.cc` & `dune-common-2.9.dev20220529/dune/common/test/utilitytest.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
 #include <tuple>
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/vcexpectedimpltest.cc` & `dune-common-2.9.dev20220529/dune/common/test/vcexpectedimpltest.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #if !HAVE_VC
 #error Inconsistent buildsystem.  This program should not be built in the \
   absence of Vc.
 #endif
 
@@ -43,15 +41,15 @@
 
   std::string expected_impl;
   if(auto env_impl = std::getenv(expected_var.c_str()))
     expected_impl = env_impl;
 
   if(expected_impl.empty())
   {
-    std::cerr << "No expected vc implementation provided, skipping test\n"
+    std::cerr << "No expected vc imlementation provided, skipping test\n"
               << "Please set " << expected_var
               << " environment variable to one of the following values:";
     for(const auto &item : impl_names)
       std::cerr << ' ' << item.second;
     std::cerr << std::endl;
     return 77;
   }
```

### Comparing `dune-common-2.9.0rc1/dune/common/test/versiontest.cc` & `dune-common-2.9.dev20220529/dune/common/test/versiontest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 // DUNE_MODTEST_VERSION 3.2.1
 #define DUNE_MODTEST_VERSION_MAJOR 3
 #define DUNE_MODTEST_VERSION_MINOR 2
 #define DUNE_MODTEST_VERSION_REVISION 1
 
 #if HAVE_CONFIG_H
```

### Comparing `dune-common-2.9.0rc1/dune/common/timer.hh` & `dune-common-2.9.dev20220529/dune/common/timer.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_TIMER_HH
 #define DUNE_TIMER_HH
 
 #ifndef TIMER_USE_STD_CLOCK
 // headers for std::chrono
 #include <chrono>
 #else
@@ -25,15 +23,15 @@
 
 
   /** \brief A simple stop watch
 
      This class reports the elapsed user-time, i.e. time spent computing,
      after the last call to Timer::reset(). The results are seconds and
      fractional seconds. Note that the resolution of the timing depends
-     on your OS kernel which should be somewhere in the millisecond range.
+     on your OS kernel which should be somewhere in the milisecond range.
 
      The class is basically a wrapper for the libc-function getrusage()
 
      \warning In a multi-threading situation, this class does NOT return wall-time!
      Instead, the run time for all threads will be added up.
      For example, if you have four threads running in parallel taking one second each,
      then the Timer class will return an elapsed time of four seconds.
```

### Comparing `dune-common-2.9.0rc1/dune/common/to_unique_ptr.hh` & `dune-common-2.9.dev20220529/dune/common/to_unique_ptr.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_TO_UNIQUE_PTR_HH
 #define DUNE_TO_UNIQUE_PTR_HH
 
 #warning to_unique_ptr.hh and ToUniquePtr are deprecated. Use std::unique_ptr or std::shared_ptr instead.
 
 #include <memory>
```

### Comparing `dune-common-2.9.0rc1/dune/common/tupleutility.hh` & `dune-common-2.9.dev20220529/dune/common/tupleutility.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_TUPLE_UTILITY_HH
 #define DUNE_TUPLE_UTILITY_HH
 
 #include <cstddef>
 #include <tuple>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/common/tuplevector.hh` & `dune-common-2.9.dev20220529/dune/common/tuplevector.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TUPLEVECTOR_HH
 #define DUNE_COMMON_TUPLEVECTOR_HH
 
 #include <tuple>
 #include <utility>
 
 #include <dune/common/indices.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/common/typelist.hh` & `dune-common-2.9.dev20220529/dune/common/typelist.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TYPELIST_HH
 #define DUNE_COMMON_TYPELIST_HH
 
 #include <type_traits>
 #include <tuple>
 #include <utility>
 
@@ -64,15 +62,15 @@
    *   std::cout << className<typename decltype(metaType)::type>()
    *             << std::endl;
    * });
    * \endcode
    *
    * It is also possible to iterate over complete-but-non-instantiable types,
    * e.g. `tuple<void>`.  But to do so you need to suppress ADL in the
-   * invocation of `forEach()`, since ADL would try to instantiate complete
+   * invocation of `forEach()`, since ADL would try to instanciate complete
    * types in the template argument list of `TypeList` in order to find the
    * associated namespaces.  To suppress ADL you can either use a qualified
    * lookup:
    * \code
    * Hybrid::forEach(TypeList<std::tuple<void> >{},
    *                 [] (auto metaType) { ... });
    * });
```

### Comparing `dune-common-2.9.0rc1/dune/common/typetraits.hh` & `dune-common-2.9.dev20220529/dune/common/typetraits.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_TYPETRAITS_HH
 #define DUNE_TYPETRAITS_HH
 
 #include <complex>
 #include <type_traits>
 #include <utility>
 #include <vector>
@@ -89,15 +87,15 @@
      members of this class in the non-specialized template, but you know that
      actually instantiating the non-specialized template is an error.  You
      can try something like this:
      \code
      template<typename T>
      struct Traits {
        static_assert(false,
-                          "Instantiating this non-specialized template is an "
+                          "Instanciating this non-specialized template is an "
                           "error.  You should use one of the specializations "
                           "instead.");
        //! The type used to frobnicate T
        typedef void FrobnicateType;
      };
      \endcode
      This will trigger static_assert() as soon as the compiler reads the
@@ -105,15 +103,15 @@
      never become true, no matter what the template parameters of Traits are.
      As a workaround you can use AlwaysFalse: replace <tt>false</tt> by
      <tt>AlwaysFalse<T>::value</tt>, like this:
      \code
      template<typename T>
      struct Traits {
        static_assert(AlwaysFalse<T>::value,
-                          "Instantiating this non-specialized template is an "
+                          "Instanciating this non-specialized template is an "
                           "error.  You should use one of the specializations "
                           "instead.");
        //! The type used to frobnicate T
        typedef void FrobnicateType;
      };
      \endcode
      Since there might be an specialization of AlwaysFalse for template
@@ -488,15 +486,15 @@
    * \brief Type free of internal references that `T` can be converted to.
    *
    * This is the specialization point for `AutonomousValue` and `autoCopy()`.
    *
    * If you need to specialize for a proxy type or similar, just specialize
    * for the plain type.  There are already specializations for
    * reference-qualified and cv-qualified types that will just forward to your
-   * specialization.
+   * specailixszation.
    *
    * \note For all specializations, the member type `type` should be
    *       constructible from `T`.
    */
   template<class T>
   struct AutonomousValueType { using type = T; };
 
@@ -597,15 +595,15 @@
    *   auto param(NumberType v)
    *   {
    *     return 2*v;
    *   }
    * ```
    * If the automatic differentiation library is Adept, this would lead to
    * use-after-end-of-life-bugs.  The reason is that for efficiency reasons
-   * Adept does not immediately evaluate the expression, but instead it
+   * Adept does not immidiately evaluate the expression, but instead it
    * constructs an expression object that records the kind of expression and
    * references to the operands.  The expression object is only evaluated when
    * it is assigned to an object of some number type -- which will only happen
    * after the operands (`v` and the temporary object representing `2`) have
    * gone out of scope and been destroyed.  Basically, Adept was invented
    * before `auto` and rvalue-references were a thing.
    *
```

### Comparing `dune-common-2.9.0rc1/dune/common/typeutilities.hh` & `dune-common-2.9.dev20220529/dune/common/typeutilities.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_TYPEUTILITIES_HH
 #define DUNE_COMMON_TYPEUTILITIES_HH
 
 #include <cstddef>
 #include <type_traits>
 #include <tuple>
```

### Comparing `dune-common-2.9.0rc1/dune/common/version.hh` & `dune-common-2.9.dev20220529/dune/common/version.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_VERSION_HH
 #define DUNE_VERSION_HH
 
 /** \file
  * \brief Various macros to work with %Dune module version numbers
  */
```

### Comparing `dune-common-2.9.0rc1/dune/common/visibility.hh` & `dune-common-2.9.dev20220529/dune/common/visibility.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COMMON_VISIBILITY_HH
 #define DUNE_COMMON_VISIBILITY_HH
 
 /** \file
  * \brief Definition of macros controlling symbol visibility at the ABI level.
  */
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/densematrix.hh` & `dune-common-2.9.dev20220529/dune/python/common/densematrix.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_DENSEMATRIX_HH
 #define DUNE_PYTHON_COMMON_DENSEMATRIX_HH
 
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/densevector.hh` & `dune-common-2.9.dev20220529/dune/python/common/densevector.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_DENSEVECTOR_HH
 #define DUNE_PYTHON_COMMON_DENSEVECTOR_HH
 
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/dimrange.hh` & `dune-common-2.9.dev20220529/dune/python/common/dimrange.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_DIMRANGE_HH
 #define DUNE_PYTHON_COMMON_DIMRANGE_HH
 
 #include <cstddef>
 
 #include <tuple>
 #include <type_traits>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/dynmatrix.hh` & `dune-common-2.9.dev20220529/dune/python/common/dynmatrix.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_PYTHON_COMMON_DYNMATRIX_HH
 #define DUNE_PYTHON_COMMON_DYNMATRIX_HH
 
 #include <string>
 #include <tuple>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/dynvector.hh` & `dune-common-2.9.dev20220529/dune/python/common/dynvector.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_PYTHON_COMMON_DYNVECTOR_HH
 #define DUNE_PYTHON_COMMON_DYNVECTOR_HH
 
 #include <string>
 #include <tuple>
 #include <utility>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/fmatrix.hh` & `dune-common-2.9.dev20220529/dune/python/common/fmatrix.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_FMATRIX_HH
 #define DUNE_PYTHON_COMMON_FMATRIX_HH
 
 #include <cstddef>
 
 #include <algorithm>
 #include <string>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/fvector.hh` & `dune-common-2.9.dev20220529/dune/python/common/fvector.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_FVECTOR_HH
 #define DUNE_PYTHON_COMMON_FVECTOR_HH
 
 #include <cstddef>
 
 #include <algorithm>
 #include <stdexcept>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/getdimension.hh` & `dune-common-2.9.dev20220529/dune/python/common/getdimension.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_GETDIMENSION_HH
 #define DUNE_PYTHON_COMMON_GETDIMENSION_HH
 
 #include <type_traits>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/logger.hh` & `dune-common-2.9.dev20220529/dune/python/common/logger.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_LOGGER_HH
 #define DUNE_PYTHON_COMMON_LOGGER_HH
 
 #include <string>
 #include <utility>
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/mpihelper.hh` & `dune-common-2.9.dev20220529/dune/python/common/mpihelper.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_MPIHELPER_HH
 #define DUNE_PYTHON_COMMON_MPIHELPER_HH
 
 #include <config.h>
 
 #include <vector>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/numpyvector.hh` & `dune-common-2.9.dev20220529/dune/python/common/numpyvector.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_NUMPYVECTOR_HH
 #define DUNE_PYTHON_COMMON_NUMPYVECTOR_HH
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/densevector.hh>
 #include <dune/common/ftraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/pythonvector.hh` & `dune-common-2.9.dev20220529/dune/python/common/pythonvector.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_PYTHONVECTOR_HH
 #define DUNE_PYTHON_COMMON_PYTHONVECTOR_HH
 
 #include <cstddef>
 
 #include <dune/common/densevector.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/string.hh` & `dune-common-2.9.dev20220529/dune/python/common/string.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_STRING_HH
 #define DUNE_PYTHON_COMMON_STRING_HH
 
 #include <string>
 #include <type_traits>
 
 namespace Dune
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/typeregistry.hh` & `dune-common-2.9.dev20220529/dune/python/common/typeregistry.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_TYPEREGISTRY_HH
 #define DUNE_PYTHON_COMMON_TYPEREGISTRY_HH
 
 #include <algorithm>
 #include <cassert>
 #include <iostream>
 #include <iterator>
```

### Comparing `dune-common-2.9.0rc1/dune/python/common/vector.hh` & `dune-common-2.9.dev20220529/dune/python/common/vector.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_COMMON_TYPE_TRAITS_HH
 #define DUNE_PYTHON_COMMON_TYPE_TRAITS_HH
 
 #include <type_traits>
 #include <utility>
 
 #include <dune/common/ftraits.hh>
```

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/LICENSE` & `dune-common-2.9.dev20220529/dune/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/attr.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/buffer_info.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/cast.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/chrono.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/complex.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/class.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/common.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/descr.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/init.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/internals.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/detail/typeid.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/eigen.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/embed.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/eval.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/extensions.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/extensions.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/functional.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/iostream.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/numpy.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/operators.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/options.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/pybind11.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/pybind11.h`

 * *Files 0% similar despite different names*

```diff
@@ -973,15 +973,15 @@
 #else
     struct module_def {};
 #endif
 
     /** \rst
         Create a new top-level module that can be used as the main module of a C extension.
 
-        For Python 3, ``def`` should point to a statically allocated module_def.
+        For Python 3, ``def`` should point to a staticly allocated module_def.
         For Python 2, ``def`` can be a nullptr and is completely ignored.
     \endrst */
     static module_ create_extension_module(const char *name, const char *doc, module_def *def) {
 #if PY_MAJOR_VERSION >= 3
         // module_def is PyModuleDef
         def = new (def) PyModuleDef {  // Placement new (not an allocation).
             /* m_base */     PyModuleDef_HEAD_INIT,
@@ -2250,15 +2250,15 @@
     return override;
 }
 PYBIND11_NAMESPACE_END(detail)
 
 /** \rst
   Try to retrieve a python method by the provided name from the instance pointed to by the this_ptr.
 
-  :this_ptr: The pointer to the object the overridden method should be retrieved for. This should be
+  :this_ptr: The pointer to the object the overriden method should be retrieved for. This should be
              the first non-trampoline class encountered in the inheritance chain.
   :name: The name of the overridden Python method to retrieve.
   :return: The Python method by this name from the object or an empty function wrapper.
  \endrst */
 template <class T> function get_override(const T *this_ptr, const char *name) {
     auto tinfo = detail::get_type_info(typeid(T));
     return tinfo ? detail::get_type_override(this_ptr, tinfo, name) : function();
```

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/pytypes.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/stl.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/pybind11/stl_bind.h` & `dune-common-2.9.dev20220529/dune/python/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/dune/python/test/pythontests.py` & `dune-common-2.9.dev20220529/dune/python/test/pythontests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from io import StringIO
 from numpy import array
 
 import os
 # enable DUNE_SAVE_BUILD to test various output options
 os.environ['DUNE_LOG_LEVEL'] = 'info'
 os.environ['DUNE_SAVE_BUILD'] = 'console'
```

### Comparing `dune-common-2.9.0rc1/dune/python/test/test_embed1.cc` & `dune-common-2.9.dev20220529/dune/python/test/test_embed1.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <iostream>
 
 #include <dune/common/fvector.hh>
 #include <dune/python/common/fvector.hh>
 #include <dune/python/pybind11/embed.h>
 
 int main()
 {
-  Py_SetProgramName(PYTHON_INTERPRETER);
   /*
      remark: combine getting the guard and loading
              dune.common in a single 'initialization' function -
              the dune.common module can also be used to register additional
              types - although a 'dummy' scope can also be used, i.e.,
              pybind11::handle scope;
   */
```

### Comparing `dune-common-2.9.0rc1/dune/python/test/test_embed2.cc` & `dune-common-2.9.dev20220529/dune/python/test/test_embed2.cc`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <iostream>
 
 #include <dune/common/fvector.hh>
 #include <dune/python/common/fvector.hh>
 #include <dune/python/pybind11/embed.h>
 
 #include<Python.h>
 int main()
 {
-  Py_SetProgramName(PYTHON_INTERPRETER);
+  const wchar_t* path = L"/home/domse/buildsytem/build/common-build/dune-python-env/bin/python";
+  Py_SetProgramName(path);
 
   pybind11::scoped_interpreter guard{};
   auto global = pybind11::dict(pybind11::module::import("__main__").attr("__dict__"));
   {
     pybind11::module dcommon = pybind11::module::import("dune.common");
     // the following not only returns a fv but more importantly registers
     // the FV (but leads to JIT (the first time it's called)
```

### Comparing `dune-common-2.9.0rc1/lib/dunemodules.lib` & `dune-common-2.9.dev20220529/lib/dunemodules.lib`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # -*-sh-*-
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 ###############################################
 ###
 ### Configuration
 ###
 
 # name of the "control" files
```

### Comparing `dune-common-2.9.0rc1/pyproject.toml` & `dune-common-2.9.dev20220529/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dune-common-2.9.0rc1/python/dune/__main__.py` & `dune-common-2.9.dev20220529/python/dune/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import sys
 from argparse import ArgumentParser
 from dune.commands import printinfo, configure, listgenerated, rmgenerated, fixdunepy, listdunetype, checkbuilddirs
 
 # NOTE: do not import from dune.common (and consequently from dune.generator)
 #       at top level to avoid failure due to missing mpi4py.
```

### Comparing `dune-common-2.9.0rc1/python/dune/commands.py` & `dune-common-2.9.dev20220529/python/dune/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os, glob, time, fileinput, subprocess, shutil
 from dune.packagemetadata import getBuildMetaData, forceConfigure
 
 # NOTE: do not import from dune.common (and consequently from dune.generator)
 #       at top level to avoid failure due to missing mpi4py.
 
 def printinfo():
@@ -78,21 +75,21 @@
         for line in fileinput.input( os.path.join(generated_dir, 'CMakeLists.txt') ):
             start = line.find(bracket[0])
             if start != -1:
               start = start + len(bracket[0])
               end = line.find(bracket[1], start)
               cmakeentries += [line[start:end]]
 
-        occurrences = {}
+        occurences = {}
         for i in ccfiles + sofiles + cmakedirs + cmakeentries:
-            occurrences[i] = occurrences.get(i, 0) + 1
+            occurences[i] = occurences.get(i, 0) + 1
 
         inconsistent = []
-        for o in occurrences:
-            if occurrences[o] != 4:
+        for o in occurences:
+            if occurences[o] != 4:
                 inconsistent += [o]
 
         if len(inconsistent) > 0:
             print("Fix inconsistencies:")
             for i in inconsistent:
                 print(" ", i)
             removeGenerated(inconsistent)
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/__init__.py` & `dune-common-2.9.dev20220529/python/dune/common/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import logging
 import numpy as np
 import os
 import textwrap
 from dune.packagemetadata import getCMakeFlags
 
 logger = logging.getLogger(__name__)
@@ -12,15 +9,15 @@
 # default log level is INFO
 loglevel = logging.INFO
 try:
     loglevel = getattr(logging, os.environ['DUNE_LOG_LEVEL'].upper())
 except KeyError:
     pass
 except AttributeError:
-    logger.warn('Invalid log level in environment variable DUNE_LOG_LEVEL. Valid are {debug,info,warn,error}')
+    logger.warn('Invalid log level in environment variable DUNE_LOG_LEVEL')
 
 logformat = os.environ.get('DUNE_LOG_FORMAT', 'DUNE-%(levelname)s: %(message)s')
 
 logging.basicConfig(format=logformat, level=loglevel)
 
 cmakeFlags = getCMakeFlags()
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/checkconfiguration.py` & `dune-common-2.9.dev20220529/python/dune/common/checkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import logging
 import os
 import re
 import subprocess
 
 import dune.common.module
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/deprecated.py` & `dune-common-2.9.dev20220529/python/dune/common/deprecated.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import logging
 
 class DeprecatedObject(object):
     def __init__(self, real, message):
         self.real = real
         self.logger = logging.getLogger(real.__module__)
         self.message = message
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/locking.py` & `dune-common-2.9.dev20220529/python/dune/common/locking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 ## By default use portalocker, if available.
 ## However, portalocker is not available on all systems
 ## and therefore a fallback implementation is also provided
 try:
     from portalocker import Lock as _Lock
     from portalocker.constants import LOCK_EX, LOCK_SH
     class Lock(_Lock):
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/module.py` & `dune-common-2.9.dev20220529/python/dune/common/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import logging
 import os
 import re
 import shlex
 import subprocess
 import sys
 
@@ -112,16 +109,16 @@
 def resolve_order(deps):
     """resolve module dependencies
 
     Args:
        deps:     dictionary mapping module name to its dependency names
 
     Return:
-       Ordered list of module names such that each module only depends on
-       modules preceding it.
+       Ordred list of module names such that each module only depends on
+       modules preceeding it.
     """
     order = []
 
     def resolve(m):
         if m not in order:
             for d, r in deps[m].depends:
                 if d not in order:
@@ -328,15 +325,15 @@
     if cmake.returncode != 0:
         raise RuntimeError(buffer_to_str(stderr))
     return buffer_to_str(stdout)
 
 def get_dune_py_version():
     # change this version on the following events:
     # - a release (major version numbers)
-    # - any incompatible change to the dune-py module (revision number)
+    # - any incompatible change to the dune-py module (revison number)
     return Version("2.8.0")
 
 
 def make_dune_py_module(dune_py_dir=None, deps=None):
     if dune_py_dir is None:
         dune_py_dir = getDunePyDir()
     os.makedirs(dune_py_dir, exist_ok=True)
```

### Comparing `dune-common-2.9.0rc1/python/dune/common/project.py` & `dune-common-2.9.dev20220529/python/dune/common/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os
 
 def write_cmake_file(dir, content=None, subdirs=None, install=None):
     if not os.path.isdir(dir):
         raise ValueError('Directory \'' + dir + '\' does not exist.')
 
     append = []
```

### Comparing `dune-common-2.9.0rc1/python/dune/create.py` & `dune-common-2.9.dev20220529/python/dune/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import importlib
 import sys
 import pkgutil
 import importlib
 import logging
 import inspect
 
@@ -105,15 +102,15 @@
 ## the second part is for the 'load' method
 
 # a helper class
 class Empty:
     pass
 
 def signatureDict(func):
-    # get signature from func, we simply fill a dictionary with the name of
+    # get signature from func, we simply fill a dictonary with the name of
     # all non var argument of the function as key and containing a either
     # Empty or the default argument provided by the function signature
 
     ret = {}
     sig = inspect.signature(func)
     for p,v in sig.parameters.items():
         # we only extract positional or keyword argument (i.e. not  *args,**kwargs)
@@ -125,16 +122,16 @@
 
 def _creatorCall(create, usedKeys, *args, **kwargs):
     # get signature of create function to call
     signature = signatureDict(create)
     # check if any of the parameter names correspond to some creator -
     # if a creator exists for that function name and the value passed in by
     # the user for that parameter is a string, call the creator otherwise
-    # use the object provided. If no creator exists use the value
-    # provided by the user or the default value.
+    # use the object provided. If no creator exsits use the the value
+    # provided by the user or the default value
     for name in signature:
         # special treatment of 'view'/'grid' parameter since a 'grid' is
         # also a view
         if name=='view' and not name in kwargs and 'grid' in kwargs:
             kwargs.update({"view":kwargs["grid"]})
             usedKeys.update(["grid"])
         creator = globals().get(name)
@@ -164,15 +161,15 @@
 def creatorCall(self, key, *args, **kwargs):
     key = key.upper().lower()
     try:
         create = self.registry[key][0]
     except KeyError:
         raise RuntimeError('No ' + self.obj + ' implementation: ' + key +\
                 '. Available: ' + ' '.join(r for r in self.registry) + '.' )
-    # the complex creation mechanism is only allowed with named arguments
+    # the complex creation mechanism is only allowed with named arguemtns
     # if positional arguments have been used, call the original function directly
     # without further checking the parameters
     if len(args)>0:
         return create(*args, **kwargs)
     else:
         usedKeys = set()
         # make a fix here for grids/views
```

### Comparing `dune-common-2.9.0rc1/python/dune/deprecate.py` & `dune-common-2.9.dev20220529/python/dune/deprecate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import warnings
 
 def deprecated(msg,name=None):
     '''This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used.'''
     def deprecated_decorator(func):
```

### Comparing `dune-common-2.9.0rc1/python/dune/generator/__init__.py` & `dune-common-2.9.dev20220529/python/dune/generator/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os
 import logging
 
 import dune.common.module as moduleInfo
 from .exceptions import CompileError, ConfigurationError
 from . import cmakebuilder as builderModule
+from .cmakebuilder import Builder
 
 logger = logging.getLogger(__name__)
 
-def _constructBuilder():
-    from .cmakebuilder import Builder, MakefileBuilder
-
-    env_force = os.environ.get('DUNE_FORCE_BUILD', 'FALSE').upper()
-    env_save  = os.environ.get('DUNE_SAVE_BUILD' , 'FALSE').upper()
-
-    use_cmake_builder = os.environ.get('DUNE_PY_USE_CMAKEBUILDER' , 'FALSE').upper()
-
-    if use_cmake_builder in ('1', 'TRUE'):
-        # old cmake based builder
-        return Builder(force=(env_force in ('1', 'TRUE')), saveOutput=env_save)
-    else:
-        # new Makefile based builder
-        return MakefileBuilder(force=(env_force in ('1', 'TRUE')), saveOutput=env_save)
+env_force = os.environ.get('DUNE_FORCE_BUILD', 'FALSE').upper()
+env_save  = os.environ.get('DUNE_SAVE_BUILD' , 'FALSE').upper()
 
-# builder object that builds the autogenerated Python modules
-builder = _constructBuilder()
+builder = Builder(force=(env_force in ('1', 'TRUE')), saveOutput=env_save)
 
 def setNoDependencyCheck():
     logger.debug("Switching off dependency check - modules will always be compiled")
     builderModule.noDepCheck = True
 def setDependencyCheck():
     logger.debug("Switching on dependency check")
     builderModule.noDepCheck = False
```

### Comparing `dune-common-2.9.0rc1/python/dune/generator/algorithm.py` & `dune-common-2.9.dev20220529/python/dune/generator/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import numpy
 
 from dune.common.hashit import hashIt
 from dune.common.utility import isString
 
 def cppType(arg):
     try:
```

### Comparing `dune-common-2.9.0rc1/python/dune/generator/generator.py` & `dune-common-2.9.dev20220529/python/dune/generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 """ Generator module:
 
     The module provides the main class for on the fly generation of pybind11
     Python wrappers for implementations of a gives interface. The necessary
     details for each implementation (the C++ typedef and the includes) are
-    provided by python dictionaries stored in files.
+    provided by python dictonaries stored in files.
 """
 
 import logging
 
 from dune.common.hashit import hashIt
 
 logger = logging.getLogger(__name__)
```

### Comparing `dune-common-2.9.0rc1/python/dune/generator/importclass.py` & `dune-common-2.9.dev20220529/python/dune/generator/importclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os
 
 from dune.common.hashit import hashIt
 from dune.common.utility import isString
 from dune.generator.algorithm import cppType
 
 def load(className, includeFiles, *args,
```

### Comparing `dune-common-2.9.0rc1/python/dune/generator/template/config.h.cmake` & `dune-common-2.9.dev20220529/python/dune/generator/template/config.h.cmake`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 /* begin dune-py
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 
 /* begin private */
```

### Comparing `dune-common-2.9.0rc1/python/dune/packagemetadata.py` & `dune-common-2.9.dev20220529/python/dune/packagemetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/env python3
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 
 """Module that helps with meta data for Dune Python packages
 
 This module implements helpers for two classes of meta data
 
   - Classical package meta data such as maintainer email, description, ...
   - Build meta data that is needed for the Dune generator module
@@ -212,15 +209,15 @@
                         deps.append((m.name, VersionRequirement(None)))
                     else:
                         deps.append((m, VersionRequirement(None)))
             else:
                 while s:
                     match = re.match(r'(?P<module>[a-zA-Z0-9_\-]+)(\s*\((?P<version>[^)]*)\))?((?P<pyversion>[^\s]*))?', s)
                     if not match:
-                        raise ValueError('Invalid dependency list: ' + s)
+                        raise ValueError('Invalid dependency list.')
                     deps.append((match.group('module'), VersionRequirement(match.group('version') or match.group('pyversion'))))
                     s = s[match.end():].strip()
             return deps
 
         self.depends = parse_deps(data.get('depends'))
         self.suggests = parse_deps(data.get('suggests'))
         self.python_requires = parse_deps(data.get('python-requires'))
@@ -323,15 +320,15 @@
     if cmakeFlags is not None:
         flags += shlex.split(cmakeFlags)
     return flags
 
 def defaultCMakeFlags():
     # defaults
     flags = dict([
-        ('CMAKE_CXX_FLAGS', '-O3 -DNDEBUG'),              # same as release
+        ('CMAKE_BUILD_TYPE', 'Release'),
         ('CMAKE_INSTALL_RPATH_USE_LINK_PATH', 'TRUE'),
         ('DUNE_ENABLE_PYTHONBINDINGS', 'TRUE'),
         ('ALLOW_CXXFLAGS_OVERWRITE', 'ON'),
         ('CMAKE_DISABLE_FIND_PACKAGE_LATEX', 'TRUE'),
         ('CMAKE_DISABLE_FIND_PACKAGE_Doxygen', 'TRUE'),
         ('INKSCAPE', 'FALSE'),
     ])
@@ -572,22 +569,21 @@
     return _buildMetaData
 
 
 def _extractCMakeFlags():
     duneOptsFile = None
     cmakeFlags = {}
     for x in _buildMetaData.combine_across_modules("CMAKE_FLAGS"):
-        for y in x.split("<SEP>"):
+        for y in x.split(";"):
             try:
                 k, v = y.split(":=", 1)
-                v = v.strip(' "')
                 if k == "DUNE_OPTS_FILE":
                     duneOptsFile = v
                 else:
-                    cmakeFlags[k] = v
+                    cmakeFlags[k] = v.strip()
             except ValueError:  # no '=' in line
                 pass
 
     # add flags from some opts file
     duneOptsFile = os.environ.get('DUNE_OPTS_FILE', duneOptsFile)
     cmakeArgs = []
     if duneOptsFile:
```

### Comparing `dune-common-2.9.0rc1/python/dune/plotting.py` & `dune-common-2.9.dev20220529/python/dune/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os
 try:
     s = os.environ['DUNEPY_BLOCK_PLOTTING']
     block = s in ['TRUE','True','true', '1', 't', 'y', 'yes']
 except KeyError:
     block = True
 try:
```

### Comparing `dune-common-2.9.0rc1/python/dune_common.egg-info/PKG-INFO` & `dune-common-2.9.dev20220529/python/dune_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-common
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Basis infrastructure for all Dune modules
 Home-page: https://gitlab.dune-project.org/core/dune-common
 Author: The Dune Core developers
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
-Description: <!--
-        SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-        SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-        -->
-        
-        DUNE-library
+Description: DUNE-library
         ============
         
         DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
         for solving partial differential equations with grid-based methods.
         
         The main intention is to create slim interfaces allowing an efficient use of
         legacy and/or new libraries. Using C++ techniques DUNE allows one to use very
@@ -85,15 +80,15 @@
         1. https://dune-project.org/releases/
         2. https://dune-project.org/buildsystem/
         3. http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
         
         [installation]: https://www.dune-project.org/doc/installation
         [licence]: http://gcc.gnu.org/onlinedocs/libstdc++/faq.html#faq.license
         
-        git-d7eff87fdf39ee6ad4fb9d993d9cabe9937d42c1
+        git-e8aec08f5a38b387f154ea7838c7e09d728c7615
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-common-2.9.0rc1/python/dune_common.egg-info/SOURCES.txt` & `dune-common-2.9.dev20220529/python/dune_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 README.md
 TODO
 config.h.cmake
 dune-common.pc.in
 dune.module
 pyproject.toml
 setup.py
-.reuse/dep5
-LICENSES/BSD-3-Clause.txt
-LICENSES/FSFAP.txt
-LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
 bin/CMakeLists.txt
 bin/dune-ctest
 bin/dune-git-whitespace-hook
 bin/dunecontrol
 bin/dunepackaging.py
 bin/duneproject
 bin/find_modules.py
@@ -54,15 +50,14 @@
 cmake/modules/DuneMacros.cmake
 cmake/modules/DuneModuleDependencies.cmake
 cmake/modules/DuneModuleInformation.cmake
 cmake/modules/DunePathHelper.cmake
 cmake/modules/DunePkgConfig.cmake
 cmake/modules/DuneProject.cmake
 cmake/modules/DunePythonCommonMacros.cmake
-cmake/modules/DunePythonCompiler.cmake
 cmake/modules/DunePythonDeprecations.cmake
 cmake/modules/DunePythonFindPackage.cmake
 cmake/modules/DunePythonInstallPackage.cmake
 cmake/modules/DunePythonTestCommand.cmake
 cmake/modules/DunePythonVirtualenv.cmake
 cmake/modules/DuneReplaceProperties.cmake
 cmake/modules/DuneSphinxCMakeDoc.cmake
@@ -70,37 +65,31 @@
 cmake/modules/DuneStreams.cmake
 cmake/modules/DuneSymlinkOrCopy.cmake
 cmake/modules/DuneTestMacros.cmake
 cmake/modules/DuneUtilities.cmake
 cmake/modules/FindGMP.cmake
 cmake/modules/FindInkscape.cmake
 cmake/modules/FindLatexMk.cmake
-cmake/modules/FindLatexMk.cmake.license
 cmake/modules/FindMETIS.cmake
 cmake/modules/FindPTScotch.cmake
 cmake/modules/FindParMETIS.cmake
 cmake/modules/FindQuadMath.cmake
 cmake/modules/FindSphinx.cmake
 cmake/modules/FindSuiteSparse.cmake
 cmake/modules/FindTBB.cmake
 cmake/modules/Headercheck.cmake
 cmake/modules/OverloadCompilerFlags.cmake
 cmake/modules/UseInkscape.cmake
 cmake/modules/UseLatexMk.cmake
-cmake/modules/UseLatexMk.cmake.license
 cmake/modules/latexmkrc.cmake
-cmake/modules/latexmkrc.cmake.license
 cmake/modules/FindPkgConfig/CMakeLists.txt
 cmake/modules/FindPkgConfig/FindPkgConfig.cmake
-cmake/modules/FindPkgConfig/FindPkgConfig.cmake.license
 cmake/modules/FindPython3/CMakeLists.txt
 cmake/modules/FindPython3/FindPython3.cmake
-cmake/modules/FindPython3/FindPython3.cmake.license
 cmake/modules/FindPython3/Support.cmake
-cmake/modules/FindPython3/Support.cmake.license
 cmake/pkg/dune-common-config.cmake.in
 cmake/scripts/CMakeLists.txt
 cmake/scripts/CreateDoxyFile.cmake
 cmake/scripts/FinalizeHeadercheck.cmake
 cmake/scripts/InstallFile.cmake
 cmake/scripts/RunDoxygen.cmake
 cmake/scripts/WritePythonCMakeMetadata.cmake
@@ -126,17 +115,15 @@
 doc/comm/communication.bib
 doc/comm/communication.tex
 doc/comm/indexset.cc
 doc/comm/poosc08.cc
 doc/comm/poosc08_test.cc
 doc/comm/reverse.hh
 doc/comm/figures/darray.eps
-doc/comm/figures/darray.eps.license
 doc/comm/figures/distindex.eps
-doc/comm/figures/distindex.eps.license
 doc/doxygen/CMakeLists.txt
 doc/doxygen/Doxylocal
 doc/doxygen/Doxystyle
 doc/doxygen/doxygen-macros
 doc/doxygen/mainpage.txt
 doc/doxygen/modules.txt
 dune/CMakeLists.txt
@@ -189,15 +176,14 @@
 dune/common/ios_state.hh
 dune/common/iteratorfacades.hh
 dune/common/iteratorrange.hh
 dune/common/keywords.hh
 dune/common/lru.hh
 dune/common/mallocallocator.hh
 dune/common/math.hh
-dune/common/matrixconcepts.hh
 dune/common/matvectraits.hh
 dune/common/modules.txt
 dune/common/overloadset.hh
 dune/common/parameterizedobject.hh
 dune/common/parametertree.cc
 dune/common/parametertree.hh
 dune/common/parametertreeparser.cc
@@ -377,15 +363,14 @@
 dune/common/test/referencehelpertest.cc
 dune/common/test/reservedvectortest.cc
 dune/common/test/scotchtest.cc
 dune/common/test/shared_ptrtest.cc
 dune/common/test/singletontest.cc
 dune/common/test/sllisttest.cc
 dune/common/test/stdapplytest.cc
-dune/common/test/stdchecktypes.cc
 dune/common/test/stdidentity.cc
 dune/common/test/streamoperatorstest.cc
 dune/common/test/streamtest.cc
 dune/common/test/stringutilitytest.cc
 dune/common/test/testdebugallocator.cc
 dune/common/test/testfloatcmp.cc
 dune/common/test/testsuite.hh
@@ -488,15 +473,14 @@
 python/dune/generator/template/config.h.cmake
 python/dune/generator/template/dune-py.pc.in
 python/dune/generator/template/dune.module.template
 python/dune/generator/template/python/CMakeLists.txt
 python/dune/generator/template/python/dune/CMakeLists.txt
 python/dune/generator/template/python/dune/generated/CMakeLists.txt
 python/dune/generator/template/python/dune/generated/CMakeLists.txt.template
-python/dune/generator/template/python/dune/generated/extractCompiler.cc
 python/dune/typeregistry/CMakeLists.txt
 python/dune/typeregistry/__init__.py
 python/dune/typeregistry/_typeregistry.cc
 python/dune_common.egg-info/PKG-INFO
 python/dune_common.egg-info/SOURCES.txt
 python/dune_common.egg-info/dependency_links.txt
 python/dune_common.egg-info/requires.txt
```

### Comparing `dune-common-2.9.0rc1/share/bash-completion/completions/dunecontrol` & `dune-common-2.9.dev20220529/share/bash-completion/completions/dunecontrol`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- shell-script -*-
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#
 # bash completion for dunecontrol
 
 _dunecontrol_complete ()
 {
   local COMMANDS="printdeps vcsetup update configure make all exec bexec status svn git"
   local COMMAND_OPTS="$(for i in printdeps vcsetup update configure make all exec bexec status svn git; do echo --$i-opts; done)"
   # per default we offer the list of all core modules and the advertised discretization modules
@@ -14,15 +11,15 @@
 	MODULES=$DUNE_MODULES
   fi
 
   # get completion information
   local cur prev words cword split
   _init_completion -s || return
 
-  # check whether we have already seen a command
+  # check wether we have already seen a command
   local have_command=0
   for i in `seq $COMP_CWORD`; do
     case ${COMP_WORDS[i]} in
     printdeps|vcsetup|update|configure|make|all|exec|bexec|status|svn|git)
 			have_command=1
 			;;
 	esac
```

