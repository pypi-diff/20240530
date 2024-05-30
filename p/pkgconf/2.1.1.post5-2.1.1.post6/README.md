# Comparing `tmp/pkgconf-2.1.1.post5.tar.gz` & `tmp/pkgconf-2.1.1.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgconf-2.1.1.post5.tar", last modified: Thu May 30 00:20:25 2024, max compression
+gzip compressed data, was "pkgconf-2.1.1.post6.tar", last modified: Thu May 30 00:24:20 2024, max compression
```

## Comparing `pkgconf-2.1.1.post5.tar` & `pkgconf-2.1.1.post6.tar`

### file list

```diff
@@ -1,206 +1,206 @@
--rw-r--r--   0        0        0     1647 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/.github/workflows/build.yml
--rw-r--r--   0        0        0      397 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/.github/workflows/test.yml
--rw-r--r--   0        0        0      108 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/.gitmodules
--rw-r--r--   0        0        0      214 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/.readthedocs.yaml
--rw-r--r--   0        0        0     1083 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/LICENSE
--rw-r--r--   0        0        0      513 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/README.md
--rw-r--r--   0        0        0      421 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/docs/conf.py
--rw-r--r--   0        0        0     1956 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/docs/index.rst
--rw-r--r--   0        0        0      308 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/environment.yml
--rw-r--r--   0        0        0       53 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/examples/header-only-library/example/include/example.h
--rw-r--r--   0        0        0      148 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/examples/header-only-library/example/pkgconf/example.pc
--rw-r--r--   0        0        0      240 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/examples/header-only-library/pyproject.toml
--rw-r--r--   0        0        0      994 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/meson.build
--rw-r--r--   0        0        0     2453 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/pyproject.toml
--rw-r--r--   0        0        0     1802 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/src/buildhack.py
--rw-r--r--   0        0        0     2925 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/src/pkgconf/__init__.py
--rw-r--r--   0        0        0      646 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/src/pkgconf/diagnose.py
--rw-r--r--   0        0        0       39 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.gitattributes
--rw-r--r--   0        0        0       51 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.github/FUNDING.yml
--rw-r--r--   0        0        0     3324 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.github/workflows/test.yml
--rw-r--r--   0        0        0      836 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.gitignore
--rw-r--r--   0        0        0       69 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.mailmap
--rw-r--r--   0        0        0     1633 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/.woodpecker.yml
--rw-r--r--   0        0        0     1498 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/AUTHORS
--rw-r--r--   0        0        0     1051 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      509 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/COPYING
--rw-r--r--   0        0        0       60 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/Kyuafile.in
--rw-r--r--   0        0        0     6005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/Makefile.am
--rw-r--r--   0        0        0     2442 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/Makefile.lite
--rw-r--r--   0        0        0    26691 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/NEWS
--rw-r--r--   0        0        0     6599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/README.md
--rwxr-xr-x   0        0        0     1543 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/autogen.sh
--rw-r--r--   0        0        0     9641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/bomtool/main.c
--rw-r--r--   0        0        0    17983 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/getopt_long.c
--rw-r--r--   0        0        0     2645 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/getopt_long.h
--rw-r--r--   0        0        0    46893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/main.c
--rw-r--r--   0        0        0     3354 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/renderer-msvc.c
--rw-r--r--   0        0        0      687 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/cli/renderer-msvc.h
--rw-r--r--   0        0        0     2488 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/configure.ac
--rw-r--r--   0        0        0     9790 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/conf.py
--rw-r--r--   0        0        0     5641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/extract.py
--rw-r--r--   0        0        0      136 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/index.rst
--rw-r--r--   0        0        0      709 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
--rw-r--r--   0        0        0     1453 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-audit.rst
--rw-r--r--   0        0        0     1796 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-cache.rst
--rw-r--r--   0        0        0     9972 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-client.rst
--rw-r--r--   0        0        0     4395 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-dependency.rst
--rw-r--r--   0        0        0     5951 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-fragment.rst
--rw-r--r--   0        0        0     2936 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-path.rst
--rw-r--r--   0        0        0      758 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-personality.rst
--rw-r--r--   0        0        0     8183 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-pkg.rst
--rw-r--r--   0        0        0     4361 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-queue.rst
--rw-r--r--   0        0        0     3890 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-tuple.rst
--rw-r--r--   0        0        0      375 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf.rst
--rw-r--r--   0        0        0     3070 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/argvsplit.c
--rw-r--r--   0        0        0     2893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/audit.c
--rw-r--r--   0        0        0     3959 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/bsdstubs.c
--rw-r--r--   0        0        0     1076 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/bsdstubs.h
--rw-r--r--   0        0        0     5693 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/cache.c
--rw-r--r--   0        0        0    20527 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/client.c
--rw-r--r--   0        0        0     1883 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/config.h.meson
--rw-r--r--   0        0        0    14306 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/dependency.c
--rw-r--r--   0        0        0     1953 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/fileio.c
--rw-r--r--   0        0        0    19221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/fragment.c
--rw-r--r--   0        0        0     2016 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/iter.h
--rw-r--r--   0        0        0      599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
--rw-r--r--   0        0        0    18850 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/libpkgconf.h
--rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/meson.build
--rw-r--r--   0        0        0     2945 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/parser.c
--rw-r--r--   0        0        0     8949 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/path.c
--rw-r--r--   0        0        0     9610 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/personality.c
--rw-r--r--   0        0        0    53445 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/pkg.c
--rw-r--r--   0        0        0    12364 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/queue.c
--rw-r--r--   0        0        0     1612 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/stdinc.h
--rw-r--r--   0        0        0    12752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/tuple.c
--rw-r--r--   0        0        0    23014 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/win-dirent.h
--rw-r--r--   0        0        0      339 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf.pc.in
--rw-r--r--   0        0        0     2104 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/m4/ax_check_compile_flag.m4
--rw-r--r--   0        0        0     5980 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/man/pc.5
--rw-r--r--   0        0        0     4005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkg.m4.7
--rw-r--r--   0        0        0     3417 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkgconf-personality.5
--rw-r--r--   0        0        0     7702 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkgconf.1
--rw-r--r--   0        0        0     4495 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/meson.build
--rw-r--r--   0        0        0      412 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/meson_options.txt
--rw-r--r--   0        0        0    12735 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/pkg.m4
--rw-r--r--   0        0        0      334 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/Kyuafile.in
--rwxr-xr-x   0        0        0     6956 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/basic.sh
--rwxr-xr-x   0        0        0     1242 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/builtins.sh
--rwxr-xr-x   0        0        0      388 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/conflicts.sh
--rwxr-xr-x   0        0        0      477 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/framework.sh
--rw-r--r--   0        0        0      237 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
--rw-r--r--   0        0        0      209 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
--rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/argv-parse.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/bar.pc
--rw-r--r--   0        0        0      253 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/baz.pc
--rw-r--r--   0        0        0      566 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/billion-laughs.pc
--rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
--rw-r--r--   0        0        0      196 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/cflags-internal.pc
--rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
--rw-r--r--   0        0        0      146 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
--rw-r--r--   0        0        0      142 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/circular-1.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/circular-2.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/circular-3.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
--rw-r--r--   0        0        0      122 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/comments.pc
--rw-r--r--   0        0        0      248 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/conflicts.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/depgraph-break.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
--rw-r--r--   0        0        0       84 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/empty-tuple.pc
--rw-r--r--   0        0        0      107 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
--rw-r--r--   0        0        0      163 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
--rw-r--r--   0        0        0      229 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/flag-order-1.pc
--rw-r--r--   0        0        0      244 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/flag-order-3.pc
--rw-r--r--   0        0        0      250 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/foo.pc
--rw-r--r--   0        0        0      262 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/foobar.pc
--rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
--rw-r--r--   0        0        0       98 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
--rw-r--r--   0        0        0      170 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
--rw-r--r--   0        0        0      199 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-collision.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-comment.pc
--rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
--rw-r--r--   0        0        0      168 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
--rw-r--r--   0        0        0      195 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/framework-1.pc
--rw-r--r--   0        0        0      217 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/framework-2.pc
--rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
--rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/idirafter.pc
--rw-r--r--   0        0        0      114 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/incomplete.pc
--rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/intermediary-1.pc
--rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/intermediary-2.pc
--rw-r--r--   0        0        0      235 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/isystem.pc
--rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/malformed-1.pc
--rw-r--r--   0        0        0       70 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
--rw-r--r--   0        0        0       95 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/malformed-version.pc
--rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/metapackage-1.pc
--rw-r--r--   0        0        0      126 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/metapackage-2.pc
--rw-r--r--   0        0        0      101 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/metapackage-3.pc
--rw-r--r--   0        0        0      116 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/metapackage.pc
--rw-r--r--   0        0        0      246 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/missing-require.pc
--rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
--rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/multiline.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
--rw-r--r--   0        0        0      174 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/nocflag.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/nolib.pc
--rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
--rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
--rw-r--r--   0        0        0      187 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
--rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/paren-quoting.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
--rw-r--r--   0        0        0      117 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
--rw-r--r--   0        0        0      151 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
--rw-r--r--   0        0        0      284 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/provides.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/quotes.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
--rw-r--r--   0        0        0      239 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
--rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
--rw-r--r--   0        0        0      223 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/requires-internal.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
--rw-r--r--   0        0        0      225 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
--rw-r--r--   0        0        0      254 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/static-libs.pc
--rw-r--r--   0        0        0      188 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
--rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
--rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
--rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
--rw-r--r--   0        0        0      157 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
--rw-r--r--   0        0        0      255 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/tilde.pc
--rw-r--r--   0        0        0      131 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/typelibdir.pc
--rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/unavailable-provider.pc
--rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/utf8.pc
--rw-r--r--   0        0        0      245 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
--rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib2/foo.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib3/bar.pc
--rw-r--r--   0        0        0      428 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/meson.build
--rwxr-xr-x   0        0        0     6752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/parser.sh
--rwxr-xr-x   0        0        0     6416 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/provides.sh
--rwxr-xr-x   0        0        0     7643 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/regress.sh
--rwxr-xr-x   0        0        0     3083 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/requires.sh
--rwxr-xr-x   0        0        0     2341 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/sysroot.sh
--rw-r--r--   0        0        0     1197 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/test_env.sh.in
--rwxr-xr-x   0        0        0      600 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post5/subprojects/pkgconf/tests/version.sh
--rw-r--r--   0        0        0      776 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/conftest.py
--rw-r--r--   0        0        0       74 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/data/needs-example-lib.c
--rw-r--r--   0        0        0       20 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/namespace/example/example.pc
--rw-r--r--   0        0        0      232 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/namespace/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/example/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/example/pkgconf/__init__.py
--rw-r--r--   0        0        0       41 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/lib.c
--rw-r--r--   0        0        0       23 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/lib.h
--rw-r--r--   0        0        0      445 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/meson.build
--rw-r--r--   0        0        0      178 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/register-pkg-config-path/pyproject.toml
--rw-r--r--   0        0        0      244 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/packages/use-pybind11/meson.build
--rw-r--r--   0        0        0      475 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/test_distribution.py
--rw-r--r--   0        0        0      903 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/test_entrypoints.py
--rw-r--r--   0        0        0      548 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/test_examples.py
--rw-r--r--   0        0        0     1199 2024-05-30 00:19:10.000000 pkgconf-2.1.1.post5/tests/test_python_module.py
--rw-r--r--   0        0        0     3160 2024-05-30 00:20:25.730679 pkgconf-2.1.1.post5/PKG-INFO
+-rw-r--r--   0        0        0     1653 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      397 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      108 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/.gitmodules
+-rw-r--r--   0        0        0      214 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/.readthedocs.yaml
+-rw-r--r--   0        0        0     1083 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/LICENSE
+-rw-r--r--   0        0        0      513 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/README.md
+-rw-r--r--   0        0        0      421 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/docs/conf.py
+-rw-r--r--   0        0        0     1956 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/docs/index.rst
+-rw-r--r--   0        0        0      308 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/environment.yml
+-rw-r--r--   0        0        0       53 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/examples/header-only-library/example/include/example.h
+-rw-r--r--   0        0        0      148 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/examples/header-only-library/example/pkgconf/example.pc
+-rw-r--r--   0        0        0      240 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/examples/header-only-library/pyproject.toml
+-rw-r--r--   0        0        0      994 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/meson.build
+-rw-r--r--   0        0        0     2453 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/pyproject.toml
+-rw-r--r--   0        0        0     1802 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/src/buildhack.py
+-rw-r--r--   0        0        0     2925 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/src/pkgconf/__init__.py
+-rw-r--r--   0        0        0      646 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/src/pkgconf/diagnose.py
+-rw-r--r--   0        0        0       39 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.gitattributes
+-rw-r--r--   0        0        0       51 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     3324 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.github/workflows/test.yml
+-rw-r--r--   0        0        0      836 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.gitignore
+-rw-r--r--   0        0        0       69 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.mailmap
+-rw-r--r--   0        0        0     1633 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/.woodpecker.yml
+-rw-r--r--   0        0        0     1498 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/AUTHORS
+-rw-r--r--   0        0        0     1051 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      509 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/COPYING
+-rw-r--r--   0        0        0       60 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/Kyuafile.in
+-rw-r--r--   0        0        0     6005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/Makefile.am
+-rw-r--r--   0        0        0     2442 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/Makefile.lite
+-rw-r--r--   0        0        0    26691 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/NEWS
+-rw-r--r--   0        0        0     6599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/README.md
+-rwxr-xr-x   0        0        0     1543 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/autogen.sh
+-rw-r--r--   0        0        0     9641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/bomtool/main.c
+-rw-r--r--   0        0        0    17983 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/getopt_long.c
+-rw-r--r--   0        0        0     2645 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/getopt_long.h
+-rw-r--r--   0        0        0    46893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/main.c
+-rw-r--r--   0        0        0     3354 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/renderer-msvc.c
+-rw-r--r--   0        0        0      687 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/cli/renderer-msvc.h
+-rw-r--r--   0        0        0     2488 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/configure.ac
+-rw-r--r--   0        0        0     9790 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/conf.py
+-rw-r--r--   0        0        0     5641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/extract.py
+-rw-r--r--   0        0        0      136 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/index.rst
+-rw-r--r--   0        0        0      709 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
+-rw-r--r--   0        0        0     1453 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-audit.rst
+-rw-r--r--   0        0        0     1796 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-cache.rst
+-rw-r--r--   0        0        0     9972 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-client.rst
+-rw-r--r--   0        0        0     4395 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-dependency.rst
+-rw-r--r--   0        0        0     5951 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-fragment.rst
+-rw-r--r--   0        0        0     2936 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-path.rst
+-rw-r--r--   0        0        0      758 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-personality.rst
+-rw-r--r--   0        0        0     8183 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-pkg.rst
+-rw-r--r--   0        0        0     4361 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-queue.rst
+-rw-r--r--   0        0        0     3890 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-tuple.rst
+-rw-r--r--   0        0        0      375 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf.rst
+-rw-r--r--   0        0        0     3070 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/argvsplit.c
+-rw-r--r--   0        0        0     2893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/audit.c
+-rw-r--r--   0        0        0     3959 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/bsdstubs.c
+-rw-r--r--   0        0        0     1076 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/bsdstubs.h
+-rw-r--r--   0        0        0     5693 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/cache.c
+-rw-r--r--   0        0        0    20527 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/client.c
+-rw-r--r--   0        0        0     1883 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/config.h.meson
+-rw-r--r--   0        0        0    14306 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/dependency.c
+-rw-r--r--   0        0        0     1953 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/fileio.c
+-rw-r--r--   0        0        0    19221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/fragment.c
+-rw-r--r--   0        0        0     2016 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/iter.h
+-rw-r--r--   0        0        0      599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
+-rw-r--r--   0        0        0    18850 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/libpkgconf.h
+-rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/meson.build
+-rw-r--r--   0        0        0     2945 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/parser.c
+-rw-r--r--   0        0        0     8949 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/path.c
+-rw-r--r--   0        0        0     9610 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/personality.c
+-rw-r--r--   0        0        0    53445 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/pkg.c
+-rw-r--r--   0        0        0    12364 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/queue.c
+-rw-r--r--   0        0        0     1612 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/stdinc.h
+-rw-r--r--   0        0        0    12752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/tuple.c
+-rw-r--r--   0        0        0    23014 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/win-dirent.h
+-rw-r--r--   0        0        0      339 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf.pc.in
+-rw-r--r--   0        0        0     2104 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/m4/ax_check_compile_flag.m4
+-rw-r--r--   0        0        0     5980 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/man/pc.5
+-rw-r--r--   0        0        0     4005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkg.m4.7
+-rw-r--r--   0        0        0     3417 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkgconf-personality.5
+-rw-r--r--   0        0        0     7702 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkgconf.1
+-rw-r--r--   0        0        0     4495 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/meson.build
+-rw-r--r--   0        0        0      412 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/meson_options.txt
+-rw-r--r--   0        0        0    12735 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/pkg.m4
+-rw-r--r--   0        0        0      334 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/Kyuafile.in
+-rwxr-xr-x   0        0        0     6956 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/basic.sh
+-rwxr-xr-x   0        0        0     1242 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/builtins.sh
+-rwxr-xr-x   0        0        0      388 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/conflicts.sh
+-rwxr-xr-x   0        0        0      477 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/framework.sh
+-rw-r--r--   0        0        0      237 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
+-rw-r--r--   0        0        0      209 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
+-rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/argv-parse.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/bar.pc
+-rw-r--r--   0        0        0      253 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/baz.pc
+-rw-r--r--   0        0        0      566 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/billion-laughs.pc
+-rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
+-rw-r--r--   0        0        0      196 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/cflags-internal.pc
+-rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
+-rw-r--r--   0        0        0      146 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
+-rw-r--r--   0        0        0      142 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/circular-1.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/circular-2.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/circular-3.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
+-rw-r--r--   0        0        0      122 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/comments.pc
+-rw-r--r--   0        0        0      248 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/conflicts.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/depgraph-break.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
+-rw-r--r--   0        0        0       84 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/empty-tuple.pc
+-rw-r--r--   0        0        0      107 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
+-rw-r--r--   0        0        0      163 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
+-rw-r--r--   0        0        0      229 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/flag-order-1.pc
+-rw-r--r--   0        0        0      244 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/flag-order-3.pc
+-rw-r--r--   0        0        0      250 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/foo.pc
+-rw-r--r--   0        0        0      262 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/foobar.pc
+-rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
+-rw-r--r--   0        0        0       98 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
+-rw-r--r--   0        0        0      170 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
+-rw-r--r--   0        0        0      199 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-collision.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-comment.pc
+-rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
+-rw-r--r--   0        0        0      168 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
+-rw-r--r--   0        0        0      195 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/framework-1.pc
+-rw-r--r--   0        0        0      217 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/framework-2.pc
+-rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
+-rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/idirafter.pc
+-rw-r--r--   0        0        0      114 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/incomplete.pc
+-rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/intermediary-1.pc
+-rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/intermediary-2.pc
+-rw-r--r--   0        0        0      235 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/isystem.pc
+-rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/malformed-1.pc
+-rw-r--r--   0        0        0       70 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
+-rw-r--r--   0        0        0       95 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/malformed-version.pc
+-rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/metapackage-1.pc
+-rw-r--r--   0        0        0      126 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/metapackage-2.pc
+-rw-r--r--   0        0        0      101 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/metapackage-3.pc
+-rw-r--r--   0        0        0      116 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/metapackage.pc
+-rw-r--r--   0        0        0      246 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/missing-require.pc
+-rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
+-rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/multiline.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
+-rw-r--r--   0        0        0      174 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/nocflag.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/nolib.pc
+-rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
+-rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
+-rw-r--r--   0        0        0      187 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
+-rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/paren-quoting.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
+-rw-r--r--   0        0        0      117 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
+-rw-r--r--   0        0        0      151 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
+-rw-r--r--   0        0        0      284 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/provides.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/quotes.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
+-rw-r--r--   0        0        0      239 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
+-rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
+-rw-r--r--   0        0        0      223 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/requires-internal.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
+-rw-r--r--   0        0        0      225 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
+-rw-r--r--   0        0        0      254 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/static-libs.pc
+-rw-r--r--   0        0        0      188 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
+-rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
+-rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
+-rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
+-rw-r--r--   0        0        0      157 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
+-rw-r--r--   0        0        0      255 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/tilde.pc
+-rw-r--r--   0        0        0      131 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/typelibdir.pc
+-rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/unavailable-provider.pc
+-rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/utf8.pc
+-rw-r--r--   0        0        0      245 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
+-rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib2/foo.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib3/bar.pc
+-rw-r--r--   0        0        0      428 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/meson.build
+-rwxr-xr-x   0        0        0     6752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/parser.sh
+-rwxr-xr-x   0        0        0     6416 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/provides.sh
+-rwxr-xr-x   0        0        0     7643 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/regress.sh
+-rwxr-xr-x   0        0        0     3083 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/requires.sh
+-rwxr-xr-x   0        0        0     2341 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/sysroot.sh
+-rw-r--r--   0        0        0     1197 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/test_env.sh.in
+-rwxr-xr-x   0        0        0      600 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post6/subprojects/pkgconf/tests/version.sh
+-rw-r--r--   0        0        0      776 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/conftest.py
+-rw-r--r--   0        0        0       74 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/data/needs-example-lib.c
+-rw-r--r--   0        0        0       20 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/namespace/example/example.pc
+-rw-r--r--   0        0        0      232 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/namespace/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/example/pkgconf/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/lib.c
+-rw-r--r--   0        0        0       23 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/lib.h
+-rw-r--r--   0        0        0      445 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/meson.build
+-rw-r--r--   0        0        0      178 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/register-pkg-config-path/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/packages/use-pybind11/meson.build
+-rw-r--r--   0        0        0      475 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/test_distribution.py
+-rw-r--r--   0        0        0      903 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/test_entrypoints.py
+-rw-r--r--   0        0        0      548 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/test_examples.py
+-rw-r--r--   0        0        0     1199 2024-05-30 00:23:23.000000 pkgconf-2.1.1.post6/tests/test_python_module.py
+-rw-r--r--   0        0        0     3160 2024-05-30 00:24:20.978272 pkgconf-2.1.1.post6/PKG-INFO
```

### Comparing `pkgconf-2.1.1.post5/.github/workflows/build.yml` & `pkgconf-2.1.1.post6/.github/workflows/build.yml`

 * *Files 17% similar despite different names*

```diff
@@ -46,15 +46,15 @@
           platforms: all
       - uses: pypa/cibuildwheel@v2.18.1
         env:
           CIBW_ARCHS_LINUX: auto aarch64 ppc64le s390x
       - uses: actions/upload-artifact@v4
         with:
           name: wheels-${{ matrix.os }}
-          path: dist/*.whl
+          path: wheelhouse/*.whl
   release:
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs:
       - sdist
       - wheels
     environment:
```

### Comparing `pkgconf-2.1.1.post5/LICENSE` & `pkgconf-2.1.1.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/README.md` & `pkgconf-2.1.1.post6/README.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/docs/index.rst` & `pkgconf-2.1.1.post6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/meson.build` & `pkgconf-2.1.1.post6/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2024 The pypackaging-native developers
 #
 # SPDX-License-Identifier: MIT
 
 project('pkgconf-pypi',
-  version : '2.1.1-5',
+  version : '2.1.1-6',
   license : 'MIT AND ISC',
   license_files : ['LICENSE'],
   meson_version : '>=1.3.2',
 )
 
 py = import('python').find_installation(pure: false)
 python_bin_dir = py.get_install_dir() / 'pkgconf' / '.bin'
```

### Comparing `pkgconf-2.1.1.post5/pyproject.toml` & `pkgconf-2.1.1.post6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   'Operating System :: Unix',
   'Operating System :: MacOS'
 ]
 description = '`pkgconf` is a program which helps with discovering library dependencies and configuring compiler and linker flags.'
 license = {file = 'LICENSE'}
 name = 'pkgconf'
 readme = 'README.md'
-version = '2.1.1-5'
+version = '2.1.1-6'
 
 [project.optional-dependencies]
 docs = [
   'sphinx ~= 7.0',
   'furo',
   'sphinx-design'
 ]
```

### Comparing `pkgconf-2.1.1.post5/src/buildhack.py` & `pkgconf-2.1.1.post6/src/buildhack.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/src/pkgconf/__init__.py` & `pkgconf-2.1.1.post6/src/pkgconf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import sysconfig
 
 from collections.abc import Sequence
 from typing import Any
 
 
-__version__ = '2.1.1-5'
+__version__ = '2.1.1-6'
 
 
 def get_executable() -> pathlib.Path:
     """Get the pkgconf executable."""
     if os.name == 'posix':
         executable_name = 'pkgconf'
     else:
```

### Comparing `pkgconf-2.1.1.post5/src/pkgconf/diagnose.py` & `pkgconf-2.1.1.post6/src/pkgconf/diagnose.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/.github/workflows/test.yml` & `pkgconf-2.1.1.post6/subprojects/pkgconf/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/.gitignore` & `pkgconf-2.1.1.post6/subprojects/pkgconf/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/.woodpecker.yml` & `pkgconf-2.1.1.post6/subprojects/pkgconf/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/AUTHORS` & `pkgconf-2.1.1.post6/subprojects/pkgconf/AUTHORS`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/CODE_OF_CONDUCT.md` & `pkgconf-2.1.1.post6/subprojects/pkgconf/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/Makefile.am` & `pkgconf-2.1.1.post6/subprojects/pkgconf/Makefile.am`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/Makefile.lite` & `pkgconf-2.1.1.post6/subprojects/pkgconf/Makefile.lite`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/NEWS` & `pkgconf-2.1.1.post6/subprojects/pkgconf/NEWS`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/README.md` & `pkgconf-2.1.1.post6/subprojects/pkgconf/README.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/autogen.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/autogen.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/bomtool/main.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/bomtool/main.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/getopt_long.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/getopt_long.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/getopt_long.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/getopt_long.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/main.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/main.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/renderer-msvc.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/renderer-msvc.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/cli/renderer-msvc.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/cli/renderer-msvc.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/configure.ac` & `pkgconf-2.1.1.post6/subprojects/pkgconf/configure.ac`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/conf.py` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/extract.py` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/extract.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-audit.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-audit.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-cache.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-cache.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-client.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-client.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-dependency.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-dependency.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-fragment.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-fragment.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-path.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-path.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-personality.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-personality.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-pkg.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-pkg.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-queue.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-queue.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/doc/libpkgconf-tuple.rst` & `pkgconf-2.1.1.post6/subprojects/pkgconf/doc/libpkgconf-tuple.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/argvsplit.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/argvsplit.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/audit.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/audit.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/bsdstubs.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/bsdstubs.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/bsdstubs.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/bsdstubs.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/cache.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/cache.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/client.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/client.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/config.h.meson` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/config.h.meson`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/dependency.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/dependency.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/fileio.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/fileio.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/fragment.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/fragment.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/iter.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/iter.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/libpkgconf-api.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/libpkgconf-api.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/libpkgconf.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/libpkgconf.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/parser.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/parser.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/path.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/path.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/personality.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/personality.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/pkg.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/pkg.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/queue.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/queue.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/stdinc.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/stdinc.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/tuple.c` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/tuple.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/libpkgconf/win-dirent.h` & `pkgconf-2.1.1.post6/subprojects/pkgconf/libpkgconf/win-dirent.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/m4/ax_check_compile_flag.m4` & `pkgconf-2.1.1.post6/subprojects/pkgconf/m4/ax_check_compile_flag.m4`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/man/pc.5` & `pkgconf-2.1.1.post6/subprojects/pkgconf/man/pc.5`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkg.m4.7` & `pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkg.m4.7`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkgconf-personality.5` & `pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkgconf-personality.5`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/man/pkgconf.1` & `pkgconf-2.1.1.post6/subprojects/pkgconf/man/pkgconf.1`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/meson.build` & `pkgconf-2.1.1.post6/subprojects/pkgconf/meson.build`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/pkg.m4` & `pkgconf-2.1.1.post6/subprojects/pkgconf/pkg.m4`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/basic.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/basic.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/builtins.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/builtins.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/lib1/billion-laughs.pc` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/lib1/billion-laughs.pc`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/parser.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/parser.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/provides.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/provides.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/regress.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/regress.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/requires.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/requires.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/sysroot.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/sysroot.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/test_env.sh.in` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/test_env.sh.in`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/subprojects/pkgconf/tests/version.sh` & `pkgconf-2.1.1.post6/subprojects/pkgconf/tests/version.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/tests/conftest.py` & `pkgconf-2.1.1.post6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/tests/test_entrypoints.py` & `pkgconf-2.1.1.post6/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/tests/test_examples.py` & `pkgconf-2.1.1.post6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/tests/test_python_module.py` & `pkgconf-2.1.1.post6/tests/test_python_module.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post5/PKG-INFO` & `pkgconf-2.1.1.post6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgconf
-Version: 2.1.1.post5
+Version: 2.1.1.post6
 Summary: `pkgconf` is a program which helps with discovering library dependencies and configuring compiler and linker flags.
 Home-page: https://pkgconf-pypi.readthedocs.io/en/latest/
 Author-Email: Ralf Gommers <ralf.gommers@gmail.com>, =?utf-8?q?Filipe_La=C3=ADns?= <lains@riseup.net>
 License: Copyright (c) 2024 pypackaging-native contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
```

